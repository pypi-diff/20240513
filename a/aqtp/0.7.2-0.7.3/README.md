# Comparing `tmp/aqtp-0.7.2.tar.gz` & `tmp/aqtp-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtp-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aqtp-0.7.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aqtp-0.7.2.tar` & `aqtp-0.7.3.tar`

### file list

```diff
@@ -1,268 +1,272 @@
--rw-r--r--   0        0        0       39 2024-04-23 00:00:20.337048 aqtp-0.7.2/.gitignore
--rw-r--r--   0        0        0      107 2024-04-23 00:00:20.341048 aqtp-0.7.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2024-04-23 00:00:20.341048 aqtp-0.7.2/LICENSE
--rw-r--r--   0        0        0    17310 2024-04-23 00:00:20.341048 aqtp-0.7.2/README.md
--rw-r--r--   0        0        0      641 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/__init__.py
--rw-r--r--   0        0        0      576 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/__init__.py
--rw-r--r--   0        0        0     4354 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_common.py
--rw-r--r--   0        0        0    16011 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config.py
--rw-r--r--   0        0        0    13928 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config_schedule_test.py
--rw-r--r--   0        0        0     5177 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config_utils.py
--rw-r--r--   0        0        0    15655 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/emulated_floating_points.py
--rw-r--r--   0        0        0     5730 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/emulation_utils.py
--rw-r--r--   0        0        0      576 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/__init__.py
--rw-r--r--   0        0        0    13641 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_conv_general.py
--rw-r--r--   0        0        0    12151 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0        0        0     8861 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_dot_general.py
--rw-r--r--   0        0        0    14977 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0        0        0     3693 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_matmul.py
--rw-r--r--   0        0        0     3293 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_matmul_test.py
--rw-r--r--   0        0        0     1083 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_ops.py
--rw-r--r--   0        0        0    18180 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_tensor.py
--rw-r--r--   0        0        0     4751 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0        0        0     2705 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_utils.py
--rw-r--r--   0        0        0     4724 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_conv_general.py
--rw-r--r--   0        0        0    29466 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_dot_general.py
--rw-r--r--   0        0        0    36485 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_dot_general_test.py
--rw-r--r--   0        0        0     5305 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_quantizer.py
--rw-r--r--   0        0        0     9578 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_tensor.py
--rw-r--r--   0        0        0     2568 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_tensor_test.py
--rw-r--r--   0        0        0     2608 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/calibration.py
--rw-r--r--   0        0        0    20942 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/config.py
--rw-r--r--   0        0        0    37619 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/config_test.py
--rw-r--r--   0        0        0     5550 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/examples.ipynb
--rw-r--r--   0        0        0    15399 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model.py
--rw-r--r--   0        0        0    25621 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model_test.py
--rw-r--r--   0        0        0    20961 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax.py
--rw-r--r--   0        0        0     7542 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_calibration.py
--rw-r--r--   0        0        0     3835 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_dg_core.py
--rw-r--r--   0        0        0     7540 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_test.py
--rw-r--r--   0        0        0     3183 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/freezer.py
--rw-r--r--   0        0        0     7422 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/freezer_test.py
--rw-r--r--   0        0        0     1672 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/README.md
--rw-r--r--   0        0        0     6896 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
--rw-r--r--   0        0        0     3997 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
--rw-r--r--   0        0        0     6087 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
--rw-r--r--   0        0        0     8989 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
--rw-r--r--   0        0        0     4731 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics.py
--rw-r--r--   0        0        0     8823 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics_test.py
--rw-r--r--   0        0        0     4451 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/int_numerics.py
--rw-r--r--   0        0        0     1426 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/no_numerics.py
--rw-r--r--   0        0        0     1338 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/numerics.py
--rw-r--r--   0        0        0     2539 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops.py
--rw-r--r--   0        0        0     2095 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops_test.py
--rw-r--r--   0        0        0     1846 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/stochastic_rounding.py
--rw-r--r--   0        0        0    15088 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/tiled_dot_general.py
--rw-r--r--   0        0        0     6972 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/tiled_dot_general_test.py
--rw-r--r--   0        0        0     6727 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/transpose.py
--rw-r--r--   0        0        0     4741 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/transpose_test.py
--rw-r--r--   0        0        0     3680 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/utils.py
--rw-r--r--   0        0        0     1590 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/__init__.py
--rw-r--r--   0        0        0    14397 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
--rw-r--r--   0        0        0     1921 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0        0        0    17225 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils.py
--rw-r--r--   0        0        0    24127 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils_test.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0        0        0     5671 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0        0        0    35156 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0        0        0    25400 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0        0        0    43061 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers.py
--rw-r--r--   0        0        0    75454 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0        0        0     6897 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0        0        0     7682 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0        0        0     9842 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0        0        0    11477 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0        0        0     3477 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0        0        0     2570 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils_test.py
--rw-r--r--   0        0        0    10045 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/__init__.py
--rw-r--r--   0        0        0     1963 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/check_config_util.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0        0        0     7382 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py
--rw-r--r--   0        0        0     1207 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0        0        0      853 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0        0        0     1230 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0        0        0     1439 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0        0        0     1231 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
--rw-r--r--   0        0        0     6443 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
--rw-r--r--   0        0        0     1647 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
--rw-r--r--   0        0        0     7476 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
--rw-r--r--   0        0        0      855 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0        0        0      855 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0        0        0      925 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0        0        0     1439 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0        0        0     1440 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0        0        0     1390 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0        0        0     1514 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0        0        0     1383 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0        0        0     1025 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0        0        0      925 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0        0        0     1232 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0        0        0     6856 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0        0        0     9732 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0        0        0     2423 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0        0        0     2130 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0        0        0   331485 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/imagenet.png
--rw-r--r--   0        0        0     8129 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0        0        0     7345 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0        0        0     9773 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0        0        0    15474 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0        0        0     3119 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0        0        0       62 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/requirements.txt
--rw-r--r--   0        0        0     5749 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0        0        0    19735 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0        0        0     2611 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py
--rw-r--r--   0        0        0     2547 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_test.py
--rw-r--r--   0        0        0     7991 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0        0        0     5854 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0        0        0     6508 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0        0        0     3927 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0        0        0    63283 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0        0        0    45534 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0        0        0     1654 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0        0        0    22231 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
--rw-r--r--   0        0        0    23430 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
--rw-r--r--   0        0        0     9798 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0        0        0     6060 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag.py
--rw-r--r--   0        0        0     9777 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0        0        0    10461 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0        0        0     4637 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0        0        0     5435 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0        0        0     6454 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0        0        0      995 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/utils.py
--rw-r--r--   0        0        0     2888 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
--rw-r--r--   0        0        0     7056 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0        0        0    15134 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py
--rw-r--r--   0        0        0    12107 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0        0        0    11082 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0        0        0    13257 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
--rw-r--r--   0        0        0     6573 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1069 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1056 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1041 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0        0        0     1006 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1193 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1101 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0        0        0     1002 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1042 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0        0        0     1002 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0        0        0     1060 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1175 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0        0        0     1244 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
--rw-r--r--   0        0        0     1664 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
--rw-r--r--   0        0        0     1661 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
--rw-r--r--   0        0        0     1662 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
--rw-r--r--   0        0        0     1662 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
--rw-r--r--   0        0        0     2172 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
--rw-r--r--   0        0        0     1600 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1849 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1323 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1448 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1344 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
--rw-r--r--   0        0        0     1568 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1801 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1584 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
--rw-r--r--   0        0        0     1479 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
--rw-r--r--   0        0        0     1495 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
--rw-r--r--   0        0        0     1531 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
--rw-r--r--   0        0        0     1046 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
--rw-r--r--   0        0        0     1245 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
--rw-r--r--   0        0        0     1245 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
--rw-r--r--   0        0        0     1549 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1380 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1380 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2052 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
--rw-r--r--   0        0        0     1340 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
--rw-r--r--   0        0        0     1340 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     2032 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1757 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
--rw-r--r--   0        0        0     1729 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
--rw-r--r--   0        0        0     2133 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
--rw-r--r--   0        0        0     1238 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     1238 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
--rw-r--r--   0        0        0     1587 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1379 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1379 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2123 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
--rw-r--r--   0        0        0     1213 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
--rw-r--r--   0        0        0     1213 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
--rw-r--r--   0        0        0     1554 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1375 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1375 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2063 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
--rw-r--r--   0        0        0     2523 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
--rw-r--r--   0        0        0      995 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
--rw-r--r--   0        0        0     1672 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
--rw-r--r--   0        0        0     2392 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
--rw-r--r--   0        0        0     1222 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
--rw-r--r--   0        0        0     2101 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
--rw-r--r--   0        0        0     3356 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
--rw-r--r--   0        0        0     1531 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
--rw-r--r--   0        0        0     1965 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
--rw-r--r--   0        0        0      382 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0        0        0     1096 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1014 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1096 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1018 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0        0        0      995 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0        0        0     1925 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0        0        0    23300 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0        0        0    33382 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0        0        0    38051 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0        0        0     4055 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0        0        0      160 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
--rw-r--r--   0        0        0    51590 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0        0        0     5666 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0        0        0    10503 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0        0        0     3939 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0        0        0    25395 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0        0        0     3284 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
--rw-r--r--   0        0        0      118 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/requirements.txt
--rw-r--r--   0        0        0    10519 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/README.md
--rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0        0        0     4810 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0        0        0     5109 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0        0        0     1045 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/common.py
--rw-r--r--   0        0        0     8505 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0        0        0    11978 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0        0        0     6844 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0        0        0    10185 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0        0        0    10192 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0        0        0    20428 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0        0        0    23689 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0        0        0     2538 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0        0        0     3451 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0        0        0     6640 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils.py
--rw-r--r--   0        0        0     4307 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils_test.py
--rw-r--r--   0        0        0    15648 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_conv_test_base.py
--rw-r--r--   0        0        0    11192 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_matmul_test_base.py
--rw-r--r--   0        0        0    12101 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_stats_test_base.py
--rw-r--r--   0        0        0    23072 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_tensor_test_base.py
--rw-r--r--   0        0        0     4694 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_test_shared_base.py
--rw-r--r--   0        0        0   129585 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/aqt/aqt.pdf
--rw-r--r--   0        0        0     1303 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/aqt/aqt.tex
--rw-r--r--   0        0        0     1468 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/pokebnn/README.md
--rw-r--r--   0        0        0     2862 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/pokebnn/cloudtpu_train_pokebnn.sh
--rw-r--r--   0        0        0   117523 2024-04-23 00:00:20.357049 aqtp-0.7.2/papers/pokebnn/tensorboard.ipynb
--rw-r--r--   0        0        0      727 2024-04-23 00:00:20.357049 aqtp-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     1852 2024-04-23 00:00:20.357049 aqtp-0.7.2/setup.py
--rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-13 01:45:52.043967 aqtp-0.7.3/.gitignore
+-rw-r--r--   0        0        0      107 2024-05-13 01:45:52.043967 aqtp-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2024-05-13 01:45:52.043967 aqtp-0.7.3/LICENSE
+-rw-r--r--   0        0        0    17310 2024-05-13 01:45:52.047967 aqtp-0.7.3/README.md
+-rw-r--r--   0        0        0      641 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/__init__.py
+-rw-r--r--   0        0        0      576 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/__init__.py
+-rw-r--r--   0        0        0     4354 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_common.py
+-rw-r--r--   0        0        0    16011 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config.py
+-rw-r--r--   0        0        0    13928 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config_schedule_test.py
+-rw-r--r--   0        0        0     5177 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/aqt_config_utils.py
+-rw-r--r--   0        0        0    15655 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/emulated_floating_points.py
+-rw-r--r--   0        0        0     5730 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/common/emulation_utils.py
+-rw-r--r--   0        0        0      576 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/__init__.py
+-rw-r--r--   0        0        0    13641 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_conv_general.py
+-rw-r--r--   0        0        0    12151 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_conv_general_test.py
+-rw-r--r--   0        0        0     8861 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_dot_general.py
+-rw-r--r--   0        0        0    14977 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     3693 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_matmul.py
+-rw-r--r--   0        0        0     3293 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_matmul_test.py
+-rw-r--r--   0        0        0     1083 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_ops.py
+-rw-r--r--   0        0        0    18180 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_tensor.py
+-rw-r--r--   0        0        0     4751 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2705 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/aqt_utils.py
+-rw-r--r--   0        0        0     4724 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_conv_general.py
+-rw-r--r--   0        0        0    28934 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_dot_general.py
+-rw-r--r--   0        0        0    37153 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     5315 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_quantizer.py
+-rw-r--r--   0        0        0    10687 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_tensor.py
+-rw-r--r--   0        0        0     2926 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2632 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/calibration.py
+-rw-r--r--   0        0        0    20892 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax/v2/config.py
+-rw-r--r--   0        0        0    37689 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/config_test.py
+-rw-r--r--   0        0        0     5550 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/examples.ipynb
+-rw-r--r--   0        0        0    15825 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model.py
+-rw-r--r--   0        0        0    27434 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model_test.py
+-rw-r--r--   0        0        0     2703 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model.py
+-rw-r--r--   0        0        0     5971 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/examples/gptq_flax_e2e_model_test.py
+-rw-r--r--   0        0        0    11994 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer.py
+-rw-r--r--   0        0        0     2284 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/extensions/gptq/gptq_dot_general_quantizer_test.py
+-rw-r--r--   0        0        0    23224 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax.py
+-rw-r--r--   0        0        0     7548 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_calibration.py
+-rw-r--r--   0        0        0     3835 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_dg_core.py
+-rw-r--r--   0        0        0     7966 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_test.py
+-rw-r--r--   0        0        0     3183 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/freezer.py
+-rw-r--r--   0        0        0     7422 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/freezer_test.py
+-rw-r--r--   0        0        0     1672 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/README.md
+-rw-r--r--   0        0        0     6896 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
+-rw-r--r--   0        0        0     3997 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
+-rw-r--r--   0        0        0     6354 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
+-rw-r--r--   0        0        0     9016 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
+-rw-r--r--   0        0        0     4739 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics.py
+-rw-r--r--   0        0        0     8823 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics_test.py
+-rw-r--r--   0        0        0     4459 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/int_numerics.py
+-rw-r--r--   0        0        0     1434 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/no_numerics.py
+-rw-r--r--   0        0        0     1338 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/numerics/numerics.py
+-rw-r--r--   0        0        0     2539 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops.py
+-rw-r--r--   0        0        0     2095 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops_test.py
+-rw-r--r--   0        0        0     1862 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/stochastic_rounding.py
+-rw-r--r--   0        0        0    15088 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/tiled_dot_general.py
+-rw-r--r--   0        0        0     8820 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/tiled_dot_general_test.py
+-rw-r--r--   0        0        0     6727 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/transpose.py
+-rw-r--r--   0        0        0     4741 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/transpose_test.py
+-rw-r--r--   0        0        0     3983 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax/v2/utils.py
+-rw-r--r--   0        0        0     1590 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/__init__.py
+-rw-r--r--   0        0        0    14397 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
+-rw-r--r--   0        0        0     1921 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/__init__.py
+-rw-r--r--   0        0        0    17225 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils.py
+-rw-r--r--   0        0        0    24127 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils_test.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax/__init__.py
+-rw-r--r--   0        0        0     5671 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax/struct.py
+-rw-r--r--   0        0        0    35156 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention.py
+-rw-r--r--   0        0        0    25400 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention_test.py
+-rw-r--r--   0        0        0    43061 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers.py
+-rw-r--r--   0        0        0    75454 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers_test.py
+-rw-r--r--   0        0        0     6897 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast.py
+-rw-r--r--   0        0        0     7682 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast_test.py
+-rw-r--r--   0        0        0     9842 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds.py
+-rw-r--r--   0        0        0    11477 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds_test.py
+-rw-r--r--   0        0        0     3477 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils.py
+-rw-r--r--   0        0        0     2570 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils_test.py
+-rw-r--r--   0        0        0    10045 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/__init__.py
+-rw-r--r--   0        0        0     1963 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/check_config_util.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-r--r--   0        0        0     7382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/base_config.py
+-rw-r--r--   0        0        0     1207 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-r--r--   0        0        0      853 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-r--r--   0        0        0     1230 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-r--r--   0        0        0     1439 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-r--r--   0        0        0     1231 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
+-rw-r--r--   0        0        0     2000 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
+-rw-r--r--   0        0        0     6443 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
+-rw-r--r--   0        0        0     1647 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
+-rw-r--r--   0        0        0     7476 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
+-rw-r--r--   0        0        0      855 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-r--r--   0        0        0      855 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-r--r--   0        0        0      925 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-r--r--   0        0        0     1439 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-r--r--   0        0        0     1440 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-r--r--   0        0        0     1390 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-r--r--   0        0        0     1514 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-r--r--   0        0        0     1383 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-r--r--   0        0        0     1025 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-r--r--   0        0        0      925 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-r--r--   0        0        0     1232 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-r--r--   0        0        0     6856 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-r--r--   0        0        0     9732 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-r--r--   0        0        0     2423 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_test.py
+-rw-r--r--   0        0        0     2130 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/hparams_config.py
+-rw-r--r--   0        0        0   331485 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/imagenet.png
+-rw-r--r--   0        0        0     8129 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-r--r--   0        0        0     7345 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models.py
+-rw-r--r--   0        0        0     9773 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models_test.py
+-rw-r--r--   0        0        0    15474 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn.py
+-rw-r--r--   0        0        0     3119 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-r--r--   0        0        0       62 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/requirements.txt
+-rw-r--r--   0        0        0     5749 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-r--r--   0        0        0    19735 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train.py
+-rw-r--r--   0        0        0     2611 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-r--r--   0        0        0     2547 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_test.py
+-rw-r--r--   0        0        0     7991 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_utils.py
+-rw-r--r--   0        0        0     5854 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/primitives.py
+-rw-r--r--   0        0        0     6508 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/primitives_test.py
+-rw-r--r--   0        0        0     3927 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quant_config.py
+-rw-r--r--   0        0        0    63283 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quantization.py
+-rw-r--r--   0        0        0    45534 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/quantization_test.py
+-rw-r--r--   0        0        0     1654 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/shape_utils.py
+-rw-r--r--   0        0        0    22231 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
+-rw-r--r--   0        0        0    23430 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
+-rw-r--r--   0        0        0     9798 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/stats.py
+-rw-r--r--   0        0        0     6060 2024-05-13 01:45:52.063967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag.py
+-rw-r--r--   0        0        0     9777 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag_test.py
+-rw-r--r--   0        0        0    10461 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/stats_test.py
+-rw-r--r--   0        0        0     4637 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/test_utils.py
+-rw-r--r--   0        0        0     5435 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/train_utils.py
+-rw-r--r--   0        0        0     6454 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/train_utils_test.py
+-rw-r--r--   0        0        0      995 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/utils.py
+-rw-r--r--   0        0        0     2888 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-r--r--   0        0        0     7056 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-r--r--   0        0        0    15134 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-r--r--   0        0        0    12107 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-r--r--   0        0        0    11082 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-r--r--   0        0        0    13257 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-r--r--   0        0        0     6573 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1069 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1056 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1041 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-r--r--   0        0        0     1006 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1193 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1101 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-r--r--   0        0        0     1002 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1042 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-r--r--   0        0        0     1002 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-r--r--   0        0        0     1060 2024-05-13 01:45:52.047967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1175 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-r--r--   0        0        0     1244 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+-rw-r--r--   0        0        0     1664 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
+-rw-r--r--   0        0        0     1661 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
+-rw-r--r--   0        0        0     1662 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
+-rw-r--r--   0        0        0     1662 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
+-rw-r--r--   0        0        0     2172 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
+-rw-r--r--   0        0        0     1600 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1849 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1323 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1448 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1344 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
+-rw-r--r--   0        0        0     1568 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1801 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1584 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
+-rw-r--r--   0        0        0     1479 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
+-rw-r--r--   0        0        0     1495 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
+-rw-r--r--   0        0        0     1531 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
+-rw-r--r--   0        0        0     1046 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
+-rw-r--r--   0        0        0     1245 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
+-rw-r--r--   0        0        0     1245 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
+-rw-r--r--   0        0        0     1549 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1380 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1380 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2052 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
+-rw-r--r--   0        0        0     1340 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
+-rw-r--r--   0        0        0     1340 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     2032 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1757 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
+-rw-r--r--   0        0        0     1729 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
+-rw-r--r--   0        0        0     2133 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1238 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1238 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1587 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1379 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1379 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2123 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1213 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1213 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1554 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1375 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1375 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2063 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
+-rw-r--r--   0        0        0     2523 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
+-rw-r--r--   0        0        0      995 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1672 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
+-rw-r--r--   0        0        0     2392 2024-05-13 01:45:52.051967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
+-rw-r--r--   0        0        0     1222 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
+-rw-r--r--   0        0        0     2101 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
+-rw-r--r--   0        0        0     3356 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
+-rw-r--r--   0        0        0     1531 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
+-rw-r--r--   0        0        0     1965 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
+-rw-r--r--   0        0        0      382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-r--r--   0        0        0     1096 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1014 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1096 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1018 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-r--r--   0        0        0      995 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1925 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-r--r--   0        0        0    23300 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-r--r--   0        0        0    33382 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models.py
+-rw-r--r--   0        0        0    38051 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-r--r--   0        0        0     4055 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-r--r--   0        0        0      160 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
+-rw-r--r--   0        0        0    51590 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train.py
+-rw-r--r--   0        0        0     5666 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-r--r--   0        0        0    10503 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-r--r--   0        0        0     3939 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-r--r--   0        0        0    25395 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-r--r--   0        0        0     3284 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+-rw-r--r--   0        0        0      118 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/requirements.txt
+-rw-r--r--   0        0        0    10519 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/README.md
+-rw-r--r--   0        0        0      577 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/__init__.py
+-rw-r--r--   0        0        0     4810 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils.py
+-rw-r--r--   0        0        0     5109 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils_test.py
+-rw-r--r--   0        0        0     1045 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/common.py
+-rw-r--r--   0        0        0     8505 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils.py
+-rw-r--r--   0        0        0    11978 2024-05-13 01:45:52.055967 aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils_test.py
+-rw-r--r--   0        0        0     6844 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/hparams_utils.py
+-rw-r--r--   0        0        0    10185 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils.py
+-rw-r--r--   0        0        0    10192 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils_test.py
+-rw-r--r--   0        0        0    20428 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/report_utils.py
+-rw-r--r--   0        0        0    23689 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/report_utils_test.py
+-rw-r--r--   0        0        0     2538 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils.py
+-rw-r--r--   0        0        0     3451 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils_test.py
+-rw-r--r--   0        0        0     6640 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils.py
+-rw-r--r--   0        0        0     4307 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils_test.py
+-rw-r--r--   0        0        0    15648 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_conv_test_base.py
+-rw-r--r--   0        0        0    11192 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_matmul_test_base.py
+-rw-r--r--   0        0        0    12101 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_stats_test_base.py
+-rw-r--r--   0        0        0    23072 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_tensor_test_base.py
+-rw-r--r--   0        0        0     4694 2024-05-13 01:45:52.059967 aqtp-0.7.3/aqt/test/aqt_test_shared_base.py
+-rw-r--r--   0        0        0   129585 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/aqt/aqt.pdf
+-rw-r--r--   0        0        0     1303 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/aqt/aqt.tex
+-rw-r--r--   0        0        0     1468 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/README.md
+-rw-r--r--   0        0        0     2862 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/cloudtpu_train_pokebnn.sh
+-rw-r--r--   0        0        0   117523 2024-05-13 01:45:52.059967 aqtp-0.7.3/papers/pokebnn/tensorboard.ipynb
+-rw-r--r--   0        0        0      727 2024-05-13 01:45:52.059967 aqtp-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     1852 2024-05-13 01:45:52.059967 aqtp-0.7.3/setup.py
+-rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.3/PKG-INFO
```

### Comparing `aqtp-0.7.2/LICENSE` & `aqtp-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/README.md` & `aqtp-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/__init__.py` & `aqtp-0.7.3/aqt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Accurate Quantized Training library."""
 
-__version__ = "0.7.2"
+__version__ = "0.7.3"
```

### Comparing `aqtp-0.7.2/aqt/common/__init__.py` & `aqtp-0.7.3/aqt/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/aqt_common.py` & `aqtp-0.7.3/aqt/common/aqt_common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/aqt_config.py` & `aqtp-0.7.3/aqt/common/aqt_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/aqt_config_schedule_test.py` & `aqtp-0.7.3/aqt/common/aqt_config_schedule_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/aqt_config_utils.py` & `aqtp-0.7.3/aqt/common/aqt_config_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/emulated_floating_points.py` & `aqtp-0.7.3/aqt/common/emulated_floating_points.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/common/emulation_utils.py` & `aqtp-0.7.3/aqt/common/emulation_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/__init__.py` & `aqtp-0.7.3/aqt/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_conv_general.py` & `aqtp-0.7.3/aqt/jax/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.7.3/aqt/jax/aqt_conv_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_dot_general.py` & `aqtp-0.7.3/aqt/jax/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.7.3/aqt/jax/aqt_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_matmul.py` & `aqtp-0.7.3/aqt/jax/aqt_matmul.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_matmul_test.py` & `aqtp-0.7.3/aqt/jax/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_ops.py` & `aqtp-0.7.3/aqt/jax/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_tensor.py` & `aqtp-0.7.3/aqt/jax/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_tensor_test.py` & `aqtp-0.7.3/aqt/jax/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/aqt_utils.py` & `aqtp-0.7.3/aqt/jax/aqt_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_conv_general.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_dot_general.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_dot_general.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,54 +60,43 @@
   # Compatible with both CalibrationMode.
   THIS_INPUT = 2
   # Multiply other argument of dot general by appropriately transposed scale.
   # Compatible with REMAINING_AXIS.
   OTHER_INPUT = 3
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class Tensor:
   """Configuration of quantization of one tensor or one side of tensor op."""
 
   # Controls at what value of input tensor should be used.
   # Setting it to True, but not quantizing fwd pass will assert-fail.
-  use_fwd_quant: Optional[bool] = utils.static_field()
+  use_fwd_quant: bool = utils.static_field(default=False)
   # Dequantization mode.
-  dequant_mode: DequantMode = utils.static_field()
+  dequant_mode: DequantMode = utils.static_field(default=DequantMode.OUTPUT)
   # Calibration axis mode.
-  calibration_mode: CalibrationMode = utils.static_field()
-
-  @classmethod
-  def make(cls, *args, **kwargs) -> Self:
-    return tensor_make(*args, **kwargs)
+  calibration_mode: CalibrationMode = utils.static_field(
+      default=CalibrationMode.CONTRACTING_AXIS
+  )
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class LocalAqt:
   contraction_axis_shard_count: int = utils.static_field()
 
 
-def tensor_make() -> 'Tensor':
-  """Makes config.Tensor."""
-  return Tensor(
-      use_fwd_quant=None,
-      dequant_mode=DequantMode.OUTPUT,
-      calibration_mode=CalibrationMode.CONTRACTING_AXIS,
-  )
-
-
 def dot_general_raw_make(
     lhs_bits=None,
     rhs_bits=None,
     local_aqt=None,
     jax_scope_name='aqt',
 ) -> 'DotGeneralRaw':
   """Create quantization configs for input matrices to a matmul."""
-  lhs_cfg = tensor_make()
-  rhs_cfg = tensor_make()
+  lhs_cfg = Tensor()
+  rhs_cfg = Tensor()
 
   # Binary uses 0.5 right now.
   if (
       lhs_bits is not None
       and rhs_bits is not None
       and 2 <= lhs_bits <= 8
       and 2 <= rhs_bits <= 8
@@ -179,29 +168,29 @@
   assert cfg.fwd.local_aqt is None, 'local_aqt is not yet supported in fwd.'
   return cfg
 
 
 # ------------------------------------------------------------------------------
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class MultiTensor:
   x: jnp.ndarray
   qx: aqt_tensor.QTensor
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class TensorRes:
   """All the things we pass from the forward pass to the backward pass."""
 
   mt: MultiTensor
   quant_grad: aqt_tensor.GradientFn
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class DotGeneralRes:
   lhs: TensorRes
   rhs: TensorRes
 
 
 def einsum(eqn: str, lhs: jnp.ndarray, rhs: jnp.ndarray, dg=lax.dot_general):
   """A copy of jnp.einsum but without the default jit so as to be injectable."""
@@ -220,23 +209,23 @@
 
 def _get_scale_t(
     qt: aqt_tensor.QTensor,
     transpose_fn: Any,
     dimension_numbers: lax.DotDimensionNumbers,
     lhs_shape: Sequence[int],
     rhs_shape: Sequence[int],
-) -> aqt_tensor.QTensor:
+) -> Sequence[jnp.ndarray]:
   list_scale_t = []
   for scale in qt.scale:
     scale_t = transpose_fn(scale, dimension_numbers, lhs_shape, rhs_shape)
     list_scale_t.append(scale_t)
-  return qt.replace(scale_t=list_scale_t)
+  return list_scale_t
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class DotGeneralQuantizer(abc.ABC):
   """Abstract class for dot_general quantizer."""
 
   def __call__(
       self,
       lhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
       rhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
@@ -295,15 +284,15 @@
       lhs_context: utils.Context,
       rhs_context: utils.Context,
   ) -> None:
     """Sets context for lhs and rhs."""
     pass
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class DefaultDotGeneralQuantizer(DotGeneralQuantizer):
   """Default dot_general quantizer."""
 
   lhs: aqt_quantizer.Quantizer
   rhs: aqt_quantizer.Quantizer
 
   def calibrate(
@@ -350,15 +339,15 @@
       lhs_context: utils.Context,
       rhs_context: utils.Context,
   ) -> None:
     self.lhs.context = lhs_context
     self.rhs.context = rhs_context
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class DotGeneralRaw:
   """Configuration of quantization of one dot_general without gradient."""
 
   lhs: Tensor
   rhs: Tensor
   dg_quantizer: DotGeneralQuantizer
   dg_accumulator_dtype: Optional[jnp.dtype] = utils.static_field()
@@ -396,36 +385,35 @@
       # TODO(lew):
       #  - Use qx.value with the int type.
       #  - Handle qx.value with the int type in an optimized way.
       #  - Add a "FQ" case we multiply qx.value*qx.value_scale (not transposed).
       #  - Can we carry untransposed scale and transpose here?
       if isinstance(rhs, MultiTensor):
         # We are in gradient code.
-        fwd_quantized = rhs.qx.scale_t is not None and len(rhs.qx.scale_t) == 1  # pytype: disable=attribute-error
-        expect_fwd_quantized = self.rhs.use_fwd_quant is not None
+        fwd_quantized = rhs.qx.scale is not None and len(rhs.qx.scale) == 1  # pytype: disable=attribute-error
         msg = (
-            'If fwd is quantized, use_fwd_quant should be either True/False;'
-            ' otherwise, use_fwd_quant should be None. Misconfiguration: found'
-            f' use_fwd_quant is {self.rhs.use_fwd_quant} in bwd, but fwd'
-            f' quantization is {fwd_quantized}.'
+            f'Found use_fwd_quant is {self.rhs.use_fwd_quant} in bwd, but fwd'
+            ' is not quantized.'
         )
-        assert fwd_quantized == expect_fwd_quantized, msg
         if self.rhs.use_fwd_quant:
           assert fwd_quantized, msg
+          scale_t = transpose.rhs_scale_transpose_for_lhs_input(
+              rhs.qx.scale[0], dimension_numbers, lhs.shape  # pytype: disable=attribute-error
+          )
+
           # Cast rhs scales to lhs dtype when multiplying with lhs. This is to
           # avoid an unexpected upcast when rhs is float32 but lhs is float16.
-          lhs = lhs * rhs.qx.scale_t[0].astype(lhs.dtype)  # pytype: disable=attribute-error
+          lhs = lhs * scale_t.astype(lhs.dtype)  # pytype: disable=attribute-error
+
           # rhs qvalue may be integer. It will be quantized again later, so cast
           # its dtype back to dequant dtype.
           # TODO(yichizh): avoid double quantization and evaluate model quality.
           rhs = rhs.qx.qvalue.astype(rhs.qx.dequant_dtype)  # pytype: disable=attribute-error
         else:
           rhs = rhs.x  # pytype: disable=attribute-error
-      else:
-        assert self.rhs.use_fwd_quant is None, 'cannot set use_fwd_quant in fwd'
 
       if self.local_aqt is not None:
         local_aqt = self.local_aqt
         factor = local_aqt.contraction_axis_shard_count  # pytype: disable=attribute-error
         msg = 'Custom calib_shared_axes not implemented for local AQT.'
         if isinstance(self.dg_quantizer, DefaultDotGeneralQuantizer):
           self.dg_quantizer.assert_calib_shared_axes_value(None, None, msg)
@@ -470,43 +458,27 @@
             )
         return calibration_axes
 
       def _postprocess_qtensor(
           input_qtensor: Optional[aqt_tensor.QTensor],
           calculated_qtensor: aqt_tensor.QTensor,
           quant_grad: aqt_tensor.GradientFn,
-          tensor_cfg: Tensor,
-          transpose_fn: Any,
       ) -> tuple[aqt_tensor.QTensor, str | aqt_tensor.GradientFn]:
         """Compute qtensor from input or input_qtensor."""
         if input_qtensor is not None:
           if not self.allow_dummy_gradient_into_qtensor:
             quant_grad = (
                 'Poison. '
                 + 'Gradients are not generally expected in serving. '
                 + 'Please set allow_dummy_gradient_into_qtensor to True '
                 + 'if this is the intended behavior.'
             )
           output_qtensor = input_qtensor
         else:
           output_qtensor = calculated_qtensor
-        mode = tensor_cfg.calibration_mode
-        if (
-            output_qtensor.scale_t is None
-            and mode == CalibrationMode.CONTRACTING_AXIS
-        ):
-          msg = 'scale, scale_t cannot be both unknown'
-          assert output_qtensor.scale is not None, msg
-          output_qtensor = _get_scale_t(
-              qt=output_qtensor,
-              transpose_fn=transpose_fn,
-              dimension_numbers=dimension_numbers,
-              lhs_shape=lhs.shape,
-              rhs_shape=rhs.shape,
-          )
         return output_qtensor, quant_grad
 
       lhs_calib_axes = _get_calibration_axes(self.lhs, lhs.ndim, lhs_ca, lhs_ba)
       rhs_calib_axes = _get_calibration_axes(self.rhs, rhs.ndim, rhs_ca, rhs_ba)
 
       lhs_incomplete_qt, rhs_incomplete_qt = self.dg_quantizer.calibrate(
           (lhs, lhs_calib_axes), (rhs, rhs_calib_axes)
@@ -527,26 +499,22 @@
       lhs_qt_calculated, lhs_quant_grad = lhs_quantized
       rhs_qt_calculated, rhs_quant_grad = rhs_quantized
 
       lhs_qt, lhs_quant_grad = _postprocess_qtensor(
           lhs_qt,
           lhs_qt_calculated,
           lhs_quant_grad,
-          self.lhs,
-          transpose.lhs_scale_transpose_to_output,
       )
       lhs_mt = MultiTensor(x=lhs, qx=lhs_qt)
       lhs_res = TensorRes(mt=lhs_mt, quant_grad=lhs_quant_grad)
 
       rhs_qt, rhs_quant_grad = _postprocess_qtensor(
           rhs_qt,
           rhs_qt_calculated,
           rhs_quant_grad,
-          self.rhs,
-          transpose.rhs_scale_transpose_to_output,
       )
       rhs_mt = MultiTensor(x=rhs, qx=rhs_qt)
       rhs_res = TensorRes(mt=rhs_mt, quant_grad=rhs_quant_grad)
 
       # TODO(lew): mt.x above should be clipped for clipping calibrations
 
       out = _qtensor_dot_general(
@@ -647,21 +615,36 @@
       scale=[],
       scale_t=None,
       dequant_dtype=dequant_dtype,
   )
   assert out.scale is not None  # pytype help
 
   if cfg.lhs.dequant_mode == DequantMode.OUTPUT:
-    out.scale.extend(lhs_qt.scale_t)
+    extend_scale = _get_scale_t(
+        qt=lhs_qt,
+        transpose_fn=transpose.lhs_scale_transpose_to_output,
+        dimension_numbers=dimension_numbers,
+        lhs_shape=lhs_qin.shape,
+        rhs_shape=rhs_qin.shape,
+    )
+
+    out.scale.extend(extend_scale)
   if cfg.rhs.dequant_mode == DequantMode.OUTPUT:
-    out.scale.extend(rhs_qt.scale_t)
+    extend_scale = _get_scale_t(
+        qt=rhs_qt,
+        transpose_fn=transpose.rhs_scale_transpose_to_output,
+        dimension_numbers=dimension_numbers,
+        lhs_shape=lhs_qin.shape,
+        rhs_shape=rhs_qin.shape,
+    )
+    out.scale.extend(extend_scale)
   return out
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class DotGeneral:
   """Configuration of quantization of dot_general and its gradients."""
 
   fwd: DotGeneralRaw
   dlhs: DotGeneralRaw
   drhs: DotGeneralRaw
 
@@ -720,32 +703,34 @@
     )
     return out
 
   def assert_config_validity(self: Self):
     """Asserts if configuration is valid."""
 
     # use_fwd_quant is not enabled when calibration_axis = remaining_axis.
+    # TODO: b/336198483 - Enable use_fwd_quant flag in the case.
+    expected_fwd_quant = False
     msg_fwd_quant = (
-        'use_fwd_quant should be set to None when remaining axis are used for'
-        ' calibration axis.'
+        f'use_fwd_quant should be set to {expected_fwd_quant} when remaining'
+        ' axis are used for calibration axis.'
     )
 
     if self.fwd.rhs.calibration_mode == CalibrationMode.REMAINING_AXIS:
       msg_fwd_quant += (
           f'rhs.calibration_mode: {self.fwd.rhs.calibration_mode},'
           f' dlhs use_fwd_quant: {self.dlhs.rhs.use_fwd_quant}'
       )
-      assert self.dlhs.rhs.use_fwd_quant is None, msg_fwd_quant
+      assert self.dlhs.rhs.use_fwd_quant is expected_fwd_quant, msg_fwd_quant
 
     if self.fwd.lhs.calibration_mode == CalibrationMode.REMAINING_AXIS:
       msg_fwd_quant += (
           f'lhs.calibration_mode: {self.fwd.lhs.calibration_mode},'
           f' drhs use_fwd_quant: {self.drhs.rhs.use_fwd_quant}'
       )
-      assert self.drhs.rhs.use_fwd_quant is None, msg_fwd_quant
+      assert self.drhs.rhs.use_fwd_quant is expected_fwd_quant, msg_fwd_quant
 
     # Check valid combination between calibration_mode and dequant_mode
     unsupported_calibration_dequant_pairs = [
         (DequantMode.OUTPUT, CalibrationMode.REMAINING_AXIS),
         (DequantMode.OTHER_INPUT, CalibrationMode.CONTRACTING_AXIS),
     ]
     msg_mode_mismatch = (
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_dot_general_test.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_dot_general_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -462,16 +462,24 @@
       dict(dg=config.dot_general_make(None, None)),
       dict(dg=config.dot_general_make(1, 1)),
       dict(dg=config.dot_general_make(1, 2)),
       dict(dg=config.dot_general_make(2, 1)),
       dict(dg=config.dot_general_make(2, 2)),
       dict(dg=config.dot_general_make(8, 8)),
       dict(dg=config.dot_general_make(8, 8), clip_gradient=True),
-      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, dlhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, drhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
       dict(dg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
       dict(dg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
       dict(dg=config.dot_general_make(None, 8)),
@@ -484,15 +492,15 @@
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       dict(
           dg=fqt_param_dict(
               s=10,
               use_fwd_quant=True,
-              dlhs_local_aqt=aqt.LocalAqt(2),
+              dlhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
           )["dg"],
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
@@ -592,20 +600,26 @@
             dict(),
         ),
     ])
 
     check([
         (
             "default    ",
-            aqt_dg_full(aqt.DequantMode.OUTPUT, local_aqt=aqt.LocalAqt(2)),
+            aqt_dg_full(
+                aqt.DequantMode.OUTPUT,
+                local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
+            ),
             dict(),
         ),
         (
             "default    ",
-            aqt_dg_full(aqt.DequantMode.THIS_INPUT, local_aqt=aqt.LocalAqt(2)),
+            aqt_dg_full(
+                aqt.DequantMode.THIS_INPUT,
+                local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
+            ),
             dict(),
         ),
     ])
 
     if isinstance(
         readonly_dg.fwd.dg_quantizer.lhs.numerics,
         int_numerics.IntNumerics,
@@ -644,16 +658,24 @@
       dict(dg=config.dot_general_make(None, None)),
       dict(dg=config.dot_general_make(1, 1)),
       dict(dg=config.dot_general_make(1, 2)),
       dict(dg=config.dot_general_make(2, 1)),
       dict(dg=config.dot_general_make(2, 2)),
       dict(dg=config.dot_general_make(8, 8)),
       dict(dg=config.dot_general_make(8, 8), clip_gradient=True),
-      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, dlhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, drhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
       dict(dg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
       dict(dg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
       dict(dg=config.dot_general_make(None, 8)),
@@ -662,15 +684,15 @@
           dg=config.dot_general_make(2, 2),
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
-      *[fqt_param_dict(s, use_fwd_quant=None) for s in range(10)],
+      *[fqt_param_dict(s, use_fwd_quant=False) for s in range(10)],
   ])
   def test_dot_general_calibration_with_remaining_axis(
       self,
       dg: config.DotGeneral | Callable[[], config.DotGeneral],
       lhs_maxval=10.0,
       rhs_maxval=20.0,
       gra_maxval=30.0,
@@ -683,17 +705,17 @@
       clip_gradient=False,
   ):
     # Deferred evaluation of config function calls. 4-bit config initialization
     # triggers jax.local_devices(), which shouldn't be called before
     # absl.app.run() in some environments.
     if not isinstance(dg, config.DotGeneral):
       dg = dg()
-    # Set use_fwd_quant to None.
-    dg.drhs.rhs.use_fwd_quant = None
-    dg.dlhs.rhs.use_fwd_quant = None
+    # Set use_fwd_quant to False.
+    dg.drhs.rhs.use_fwd_quant = False
+    dg.dlhs.rhs.use_fwd_quant = False
     readonly_dg = dg
     del dg
 
     lhs = rand_unif(lhs_shape, lhs_maxval, seed, dtype)
     rhs = rand_unif(rhs_shape, rhs_maxval, seed + 1, dtype)
     gra = rand_unif(gra_shape, gra_maxval, seed + 2, dtype)
 
@@ -780,44 +802,44 @@
 
     check([
         (
             "RA fake    ",
             aqt_dg_full(
                 aqt.DequantMode.THIS_INPUT,
                 aqt.CalibrationMode.REMAINING_AXIS,
-                local_aqt=aqt.LocalAqt(2),
+                local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
             ),
             dict(),
         ),
         (
             "RA L      ",
             aqt_dg_full_lr_diff(
                 aqt.DequantMode.OTHER_INPUT,
                 aqt.DequantMode.THIS_INPUT,
                 aqt.CalibrationMode.REMAINING_AXIS,
                 aqt.CalibrationMode.REMAINING_AXIS,
-                local_aqt=aqt.LocalAqt(2),
+                local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
             ),
             dict(),
         ),
         (
             "RA R       ",
             aqt_dg_full_lr_diff(
                 aqt.DequantMode.THIS_INPUT,
                 aqt.DequantMode.OTHER_INPUT,
                 aqt.CalibrationMode.REMAINING_AXIS,
                 aqt.CalibrationMode.REMAINING_AXIS,
-                local_aqt=aqt.LocalAqt(2),
+                local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2),
             ),
             dict(),
         ),
     ])
 
   def test_dot_general_calibrate_dequant_mode_mismatch(self):
-    dg = config.dot_general_make(8, 8, use_fwd_quant=None)
+    dg = config.dot_general_make(8, 8, use_fwd_quant=False)
     dims = (((1,), (0,)), ((), ()))
     lhs = rand_unif((10, 20), 10.0, 0, jnp.float32)
     rhs = rand_unif((20, 30), 20.0, 1, jnp.float32)
 
     # 1. Raise error when OTHER_INPUT + CONTRACTING_AXIS
     with self.assertRaisesRegex(
         AssertionError,
@@ -842,52 +864,57 @@
           aqt.DequantMode.OUTPUT,
           aqt.CalibrationMode.CONTRACTING_AXIS,
           aqt.CalibrationMode.REMAINING_AXIS,
           readonly_dg=copy.deepcopy(dg),
           dims=dims,
       )(lhs, rhs)
 
-  @parameterized.parameters([False, True])
-  def test_dot_general_prevent_fwd_quant_with_remaining_axis(
-      self, use_fwd_quant
-  ):
-    """If calibration axis is remaining_axis, use_fwd_quant should be None."""
-    dg = config.dot_general_make(8, 8, use_fwd_quant=use_fwd_quant)
+  def test_dot_general_prevent_fwd_quant_with_remaining_axis(self):
+    """If calibration axis is remaining_axis, use_fwd_quant should be False."""
+    dg = config.dot_general_make(8, 8, use_fwd_quant=True)
     dims = (((1,), (0,)), ((), ()))
     lhs = rand_unif((10, 20), 10.0, 0, jnp.float32)
     rhs = rand_unif((20, 30), 20.0, 1, jnp.float32)
 
     with self.assertRaisesRegex(
         AssertionError,
-        ".*use_fwd_quant should be set to None.*",
+        ".*use_fwd_quant should be set to False.*",
     ):
       _aqt_dg_full_lr_diff(
           aqt.DequantMode.THIS_INPUT,
           aqt.DequantMode.OTHER_INPUT,
           aqt.CalibrationMode.CONTRACTING_AXIS,
           aqt.CalibrationMode.REMAINING_AXIS,
           readonly_dg=copy.deepcopy(dg),
           dims=dims,
       )(lhs, rhs)
 
   @parameterized.parameters([
       dict(dg=config.dot_general_make(8, 8)),
-      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, dlhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
+      dict(
+          dg=config.dot_general_make(
+              8, 8, drhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=2)
+          )
+      ),
   ])
   def test_dot_general_equality_between_different_calibration_axes(
       self,
       dg: config.DotGeneral,
   ):
     """Check equality between different calibration axes."""
     dims = (((1,), (0,)), ((), ()))
 
-    # Set use_fwd_quant to None.
-    dg.drhs.rhs.use_fwd_quant = None
-    dg.dlhs.rhs.use_fwd_quant = None
+    # Set use_fwd_quant to False.
+    dg.drhs.rhs.use_fwd_quant = False
+    dg.dlhs.rhs.use_fwd_quant = False
     readonly_dg = dg
     del dg
 
     # Set the two arguments as powers of 2, to prevent it from having the
     # quantization loss.
     lhs = 2 ** jnp.floor(rand_unif((10, 20), 3.0, 1, jnp.float32) + 3.0)
     rhs = 2 ** jnp.floor(rand_unif((20, 30), 3.0, 2, jnp.float32) + 3.0)
@@ -1037,15 +1064,15 @@
   def test_local_aqt(self, shard_count, lhs, expected_product):
     # create a config that quantizes both forward and backward passes to int8
     # set the number of shards (local aqt) to 2
     dg = config.fully_quantized(
         fwd_bits=8,
         bwd_bits=8,
         use_stochastic_rounding=False,
-        drhs_local_aqt=aqt.LocalAqt(shard_count),
+        drhs_local_aqt=aqt.LocalAqt(contraction_axis_shard_count=shard_count),
     )
     dg.fwd.dg_quantizer.lhs.numerics = (
         dg.fwd.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
     )
     dg.fwd.dg_quantizer.rhs.numerics = (
         dg.fwd.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
     )
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_quantizer.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import jax.numpy as jnp
 
 
 AbstractAqtNumerics = numerics.AqtNumerics
 AbstractAqtCalibration = calibration.Calibration
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class Quantizer:
   """Configuration of quantization of one tensor."""
 
   numerics: AbstractAqtNumerics = utils.static_field()
   calib_shared_axes: Sequence[utils.AxisIdx] | Literal["per_tensor"] | None = (
       utils.static_field()
   )
@@ -57,15 +57,15 @@
     qt, quant_grad = self.calculate_qvalue(x, qt)
     return qt, quant_grad
 
   def calibrate(self, x, *, calibration_axes) -> aqt_tensor.QTensor:
     """Create incomplete QTensor with only quantization parameters."""
     if isinstance(self.numerics, no_numerics.NoNumerics):
       qt = aqt_tensor.QTensor(
-          qvalue=x, scale=[], scale_t=[], dequant_dtype=x.dtype
+          qvalue=x, scale=[], scale_t=None, dequant_dtype=x.dtype
       )
       return qt
 
     dequant_dtype = x.dtype
     # TODO(lew): We should cast earlier. xhs_q should be in cfg.xhs.dtype
     # TODO(lew): After we implement optimization to not double-quantize,
     #   what would happen if we pass fq value (xhs_q2) in residual?
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_tensor.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_tensor.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
   # | jax.sharding.PartitionSpec, will trigger an error to logics where the
   # values are used as jax.array, since they could be sharding.
   ArrayT: TypeAlias = Any
 else:
   ArrayT: TypeAlias = jnp.ndarray
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class QTensor:
   """Quantized tensor."""
 
   # Quantized (compressed) representation of tensor.
   # Use dequant() method to "decompress" to the original tensor.
   qvalue: Optional[ArrayT]
 
@@ -66,25 +66,33 @@
   # - we store scale_t in the checkpoint to avoid transposition per inference.
   # - scale_t is used both in backprop of dot_general and in post-scaling.
   #   We avoid transposing scale twice.
   # TODO(lew): Move scale_t from QTensor to some dot-general specific type?
   scale_t: Optional[list[ArrayT]]
 
   # DType of the tensor before quantized.
+  # NOTE: AQT Users should use the public property, dtype, instead.
   dequant_dtype: Optional[jnp.dtype] = flax.struct.field(
       pytree_node=False, default=None
   )
 
+  @property
+  def dtype(self) -> jnp.dtype | None:
+    return self.dequant_dtype
+
   def is_full(self) -> bool:
     return self.qvalue is not None
 
   def without_qvalue(self) -> Self:
     """Returns a copy of the QTensor without the qvalue."""
     return self.replace(qvalue=None)  # pytype: disable=attribute-error
 
+  def astype(self, dtype: jnp.dtype) -> Self:
+    return self.replace(dequant_dtype=dtype)  # pytype: disable=attribute-error
+
   def quant(self, x):
     assert not self.is_full(), 'Already quantized QTensor.'
     assert self.scale is not None, 'Missing scales to be used for quantization.'
 
     qvalue = x
     for s in self.scale:
       qvalue = qvalue * jax.lax.reciprocal(s)
@@ -136,45 +144,68 @@
 
   def __len__(self) -> int:
     assert self.qvalue is not None, _MSG_NO_QVALUE
     return len(self.qvalue)
 
 
 def zeros(
-    shape: Sequence[int], qdtype: jnp.dtype, dequant_dtype: jnp.dtype
+    shape: Sequence[int],
+    *,
+    container_dtype: jnp.dtype,
+    dequant_dtype: jnp.dtype = jnp.bfloat16,
 ) -> QTensor:
   return QTensor(
-      qvalue=jnp.zeros(shape, dtype=qdtype),
+      qvalue=jnp.zeros(shape, dtype=container_dtype),
       scale=[],
-      scale_t=[],
+      scale_t=None,
       dequant_dtype=dequant_dtype,
   )
 
 
 def zeros_with_scale(
     shape: Sequence[int],
     calibration_axis: Sequence[utils.AxisIdx],
-    qdtype: jnp.dtype,
-    dequant_dtype: jnp.dtype,
+    *,
+    container_dtype: jnp.dtype | None = None,
+    scale_dtype: jnp.dtype | None = None,
+    dequant_dtype: jnp.dtype = jnp.bfloat16,
 ) -> QTensor:
   """Initializes a QTensor with empty qvalue along with empty scale value."""
   scale_shape = list(shape)
   for axis in calibration_axis:
     scale_shape[axis] = 1
+  scale_dtype = scale_dtype or dequant_dtype
 
   # TODO(lew): hardcode dequant_dtype to bf16. This requires updating
   # other libraries to not break their functionality.
   return QTensor(
-      jnp.zeros(shape, dtype=qdtype),
-      [jnp.ones(scale_shape, dtype=dequant_dtype)],
-      None,
+      qvalue=jnp.zeros(shape, dtype=container_dtype),
+      scale=[jnp.ones(scale_shape, dtype=scale_dtype)],
+      scale_t=None,
       dequant_dtype=dequant_dtype,
   )
 
 
+def partition_spec(
+    partitions: Sequence[Any],
+    calibration_axis: Sequence[utils.AxisIdx],
+    dtype: jnp.dtype,
+) -> QTensor:
+  """Returns a QTensor filled with partition specs."""
+  scale_partitions = list(partitions)
+  for axis in calibration_axis:
+    scale_partitions[axis] = None
+  return QTensor(
+      qvalue=jax.sharding.PartitionSpec(*partitions),
+      scale=[jax.sharding.PartitionSpec(*scale_partitions)],
+      scale_t=None,
+      dequant_dtype=dtype,
+  )
+
+
 def dynamic_slice(
     operand: QTensor,
     start_indices: Sequence[int],
     slice_sizes: Sequence[int],
 ) -> QTensor:
   """Dynamically slices the value at start_indices using the given shape."""
   msg = 'scale_t is not supported in the dynamic_slice of a QTensor.'
@@ -199,18 +230,18 @@
       assert (
           scale_start_indices[axis] + scale_slice_sizes[axis]
           <= scale.shape[axis]
       ), msg
     return jax.lax.dynamic_slice(scale, scale_start_indices, scale_slice_sizes)
 
   return QTensor(
-      jax.lax.dynamic_slice(operand.qvalue, start_indices, slice_sizes),
-      [get_sliced_scales(s) for s in operand.scale],
-      None,
-      operand.dequant_dtype,
+      qvalue=jax.lax.dynamic_slice(operand.qvalue, start_indices, slice_sizes),
+      scale=[get_sliced_scales(s) for s in operand.scale],
+      scale_t=None,
+      dequant_dtype=operand.dequant_dtype,
   )
 
 
 def dynamic_update_slice(
     operand: QTensor, update: QTensor, start_indices: Sequence[int]
 ) -> QTensor:
   """Updates the value at start_indices with the given QTensor value."""
@@ -246,24 +277,29 @@
       operand.qvalue, update.qvalue, start_indices
   )
   scales = [
       jax.lax.dynamic_update_slice(scale, update_scale, start_indices)
       for scale, update_scale in zip(operand.scale, update.scale)
   ]
 
-  return QTensor(qvalues, scales, None, operand.dequant_dtype)
+  return QTensor(
+      qvalue=qvalues,
+      scale=scales,
+      scale_t=None,
+      dequant_dtype=operand.dequant_dtype,
+  )
 
 
 def update_frame(operand: QTensor, frame: int, update: QTensor) -> QTensor:
   """Updates the value at frame with the given QTensor value."""
   assert operand.ndim == update.ndim + 1
   assert operand.dequant_dtype == update.dequant_dtype, 'Dequant dtype mismatch'
 
   return QTensor(
-      operand.qvalue.at[frame].set(update.qvalue),
-      [
+      qvalue=operand.qvalue.at[frame].set(update.qvalue),
+      scale=[
           target_scale.at[frame].set(update_scale)
           for target_scale, update_scale in zip(operand.scale, update.scale)
       ],
-      None,
-      operand.dequant_dtype,
+      scale_t=None,
+      dequant_dtype=operand.dequant_dtype,
   )
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/aqt_tensor_test.py` & `aqtp-0.7.3/aqt/jax/v2/aqt_tensor_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -83,10 +83,21 @@
         dequant_dtype=update_scale.dtype,
     )
     y = aqt_tensor.dynamic_update_slice(q, update, (0, 1))
     print("======")
     print(y.qvalue)
     print(y.scale[0])
 
+  def test_dtype(self):
+    qt = aqt_tensor.zeros(
+        shape=(1,), container_dtype=jnp.int8, dequant_dtype=jnp.float32
+    )
+    self.assertEqual(qt.dtype, jnp.float32)
+    self.assertEqual(qt.dequant_dtype, jnp.float32)
+
+    qt = qt.astype(jnp.bfloat16)
+    self.assertEqual(qt.dtype, jnp.bfloat16)
+    self.assertEqual(qt.dequant_dtype, jnp.bfloat16)
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/calibration.py` & `aqtp-0.7.3/aqt/jax/v2/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 
 import abc
 from typing import Union, Sequence
 from aqt.jax.v2 import utils
 import jax.numpy as jnp
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class Calibration(abc.ABC):
   """Abstract class for calibration."""
 
   @abc.abstractmethod
   def get_bound(
       self,
       x: jnp.ndarray,
       shared_axes: Sequence[utils.AxisIdx] | None,
       context: utils.Context | None = None
   ) -> jnp.ndarray:
     pass
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class ConstantCalibration(Calibration):
   """Calibration with a constant value."""
 
   bound: Union[jnp.ndarray, float]
 
   def get_bound(
       self,
@@ -48,15 +48,15 @@
     """Calibration."""
     del shared_axes, context
     assert self.bound > 0, 'Bound should be positive.'
     # TODO(yichizh): hardcode bf16 for the scales, subject to quality evaluation
     return jnp.asarray(self.bound).reshape((1,) * len(x.shape)).astype(x.dtype)
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class AbsMaxCalibration(Calibration):
   """Simple max(abs(x)) calibration.
 
   Attributes:
     scale: Set it to something like 0.3, 0.1, 0.03. If scale < 1.0, setting
       IntNumerics.clip_gradient=True is likely to be important.
   """
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/config.py` & `aqtp-0.7.3/aqt/jax/v2/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from aqt.jax.v2.aqt_dot_general import dot_general_make
 from aqt.jax.v2.aqt_dot_general import dot_general_raw_make
 from aqt.jax.v2.aqt_dot_general import DotGeneral
 from aqt.jax.v2.aqt_dot_general import DotGeneralRaw
 from aqt.jax.v2.aqt_dot_general import dtypes_allowed_for_int32_accum
 from aqt.jax.v2.aqt_dot_general import LocalAqt
 from aqt.jax.v2.aqt_dot_general import Tensor
-from aqt.jax.v2.aqt_dot_general import tensor_make
 
 from aqt.jax.v2.aqt_quantizer import quantizer_make
 
 from aqt.jax.v2.numerics import fp8_numerics
 from aqt.jax.v2.numerics import int_numerics
 from aqt.jax.v2.numerics import no_numerics
 from aqt.jax.v2.numerics import numerics
@@ -360,15 +359,15 @@
 
 
 def default_unquantized_config() -> DotGeneral:
   """Aqt config for floating-point dot general."""
 
   def tensor_cfg() -> Tensor:
     cfg = Tensor(
-        use_fwd_quant=None,
+        use_fwd_quant=False,
         dequant_mode=DequantMode.OUTPUT,
         calibration_mode=CalibrationMode.CONTRACTING_AXIS,
     )
     return cfg
 
   def quantizer() -> aqt_quantizer.Quantizer:
     return aqt_quantizer.Quantizer(
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/config_test.py` & `aqtp-0.7.3/aqt/jax/v2/config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 
   def test_config_v4(self):
     cfg = config.config_v4(
         fwd_bits=8,
         dlhs_bits=7,
         drhs_bits=6,
         rng_type='custom-1',
-        dlhs_local_aqt=config.LocalAqt(2),
-        drhs_local_aqt=config.LocalAqt(3),
+        dlhs_local_aqt=config.LocalAqt(contraction_axis_shard_count=2),
+        drhs_local_aqt=config.LocalAqt(contraction_axis_shard_count=3),
         fwd_accumulator_dtype=jnp.int16,
         dlhs_accumulator_dtype=jnp.int8,
         drhs_accumulator_dtype=jnp.int4,
     )
-    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
                                                                                                         preserve_zero=True,
                                                                                                         preserve_max_val=False,
                                                                                                         clip=True,
                                                                                                         clip_gradient=False,
@@ -79,15 +79,15 @@
                                                                                                    train_step=None,
                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.int16'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
                              allow_dummy_gradient_into_qtensor=False,
                              dot_general=<function dot_general>),
-           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=7,
                                                                                                          preserve_zero=True,
@@ -120,15 +120,15 @@
                                                                                                     train_step=None,
                                                                                                     quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=<class 'jax.numpy.int8'>,
                               local_aqt=LocalAqt(contraction_axis_shard_count=2),
                               jax_scope_name='aqt_dlhs',
                               allow_dummy_gradient_into_qtensor=False,
                               dot_general=<function dot_general>),
-           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=6,
                                                                                                          preserve_zero=True,
@@ -165,18 +165,18 @@
                               jax_scope_name='aqt_drhs',
                               allow_dummy_gradient_into_qtensor=False,
                               dot_general=<function dot_general>),
            apply_custom_vjp_on_jax=True)"""
     utils.test_pprint_eq(cfg, expected_cfg_str, remove_memory_addresses=True)
 
   def test_configv4_original(self):
-    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+    expected_cfg_str = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
                                                                                                         preserve_zero=True,
                                                                                                         preserve_max_val=False,
                                                                                                         clip=True,
                                                                                                         clip_gradient=False,
@@ -206,15 +206,15 @@
                                                                                                    train_step=None,
                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.int32'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
                              allow_dummy_gradient_into_qtensor=False,
                              dot_general=<function dot_general>),
-           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=IntNumerics(bits=8,
                                                                                                          preserve_zero=True,
@@ -247,15 +247,15 @@
                                                                                                     train_step=None,
                                                                                                     quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=<class 'jax.numpy.int32'>,
                               local_aqt=None,
                               jax_scope_name='aqt_dlhs',
                               allow_dummy_gradient_into_qtensor=False,
                               dot_general=<function dot_general>),
-           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=JaxUniform(),
                                                                                                         dtype=None),
@@ -282,18 +282,18 @@
                               dot_general=<function dot_general>),
            apply_custom_vjp_on_jax=True)"""
     utils.test_pprint_eq(
         config.config_v4(), expected_cfg_str, remove_memory_addresses=True
     )
 
   def test_config_fwd_fp8(self):
-    expected_cfg = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+    expected_cfg = """DotGeneral(fwd=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
-                             rhs=Tensor(use_fwd_quant=None,
+                             rhs=Tensor(use_fwd_quant=False,
                                         dequant_mode=<DequantMode.OUTPUT: 1>,
                                         calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                              dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=Fp8Numerics(dtype=<class 'jax.numpy.float8_e4m3fn'>,
                                                                                                         exponent_bits=4,
                                                                                                         mantissa_bits=3,
                                                                                                         stochastic_rounding=False),
                                                                                    calib_shared_axes=None,
@@ -315,15 +315,15 @@
                                                                                                    train_step=None,
                                                                                                    quant_mode=<QuantMode.TRAIN: 1>))),
                              dg_accumulator_dtype=<class 'jax.numpy.float32'>,
                              local_aqt=None,
                              jax_scope_name='aqt_fwd',
                              allow_dummy_gradient_into_qtensor=False,
                              dot_general=<function dot_general>),
-           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           dlhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=None,
                                                                                                         dtype=None),
@@ -344,15 +344,15 @@
                                                                                                     train_step=None,
                                                                                                     quant_mode=<QuantMode.TRAIN: 1>))),
                               dg_accumulator_dtype=None,
                               local_aqt=None,
                               jax_scope_name='aqt_dlhs',
                               allow_dummy_gradient_into_qtensor=False,
                               dot_general=<function dot_general>),
-           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=None,
+           drhs=DotGeneralRaw(lhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               rhs=Tensor(use_fwd_quant=False,
                                          dequant_mode=<DequantMode.OUTPUT: 1>,
                                          calibration_mode=<CalibrationMode.CONTRACTING_AXIS: 1>),
                               dg_quantizer=DefaultDotGeneralQuantizer(lhs=Quantizer(numerics=NoNumerics(noise_fn=None,
                                                                                                         dtype=None),
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/examples/examples.ipynb` & `aqtp-0.7.3/aqt/jax/v2/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model.py` & `aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 class CNN(nn.Module):
   """A simple CNN model."""
   bn_use_stats: bool
   aqt_cfg: aqt_config.DotGeneral
   weights_quant_mode: utils.QuantMode = utils.QuantMode.TRAIN
   activation_quant_mode: utils.QuantMode = utils.QuantMode.TRAIN
+  use_legacy_freezer: bool = False
 
   @nn.compact
   def __call__(self, x):
     tiling_cfg = tiled_dot_general.Cfg(
         lhs=tiled_dot_general.TensorTiling(
             contraction_axes=[
                 tiled_dot_general.AxisTiling(
@@ -62,16 +63,17 @@
     )
     aqt_dg = functools.partial(
         aqt_flax.AqtDotGeneral,
         self.aqt_cfg,
         lhs_quant_mode=self.activation_quant_mode,
         rhs_quant_mode=self.weights_quant_mode,
         tiling_cfg=tiling_cfg,
-        use_legacy_freezer=False,
-        lhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION
+        use_legacy_freezer=self.use_legacy_freezer,
+        lhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION,
+        rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
     )
     use_running_avg = not self.bn_use_stats
     x = nn.Conv(features=32, kernel_size=(3, 3))(x)
     x = nn.BatchNorm(use_running_average=use_running_avg, dtype=x.dtype)(x)
     x = nn.relu(x)
     x = nn.avg_pool(x, window_shape=(2, 2), strides=(2, 2))
     x = nn.Conv(features=64, kernel_size=(3, 3))(x)
@@ -97,15 +99,15 @@
         # These assertions are useful when AqtEinsum definition is far away
         # from usage spot (through injection).
         # This is especially useful when specifying tiling.
         assert_eqn='bc,ab->ac',
         assert_lhs_shape=(10, 10),
         assert_rhs_shape=(None, 10),
         tile_sizes={'b': 5},
-        use_legacy_freezer=False,
+        use_legacy_freezer=self.use_legacy_freezer,
         lhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
         rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION,
     )
     # Note for AQT developers:
     #   This equation is harder because jnp.einsum and einsum swap lhs and rhs.
     x = einsum('bc,ab->ac', identity, x)
     return x
@@ -265,50 +267,56 @@
 
   summary_writer.flush()
   return state
 
 
 def serving_conversion(
     train_state: TrainState,
-    weight_only: bool = True
+    weight_only: bool = True,
+    legacy_for_freeze: bool = False,
+    legacy_for_serve: bool = False
 ) -> tuple[Callable[..., Any], dict[str, Any]]:
   """Model conversion (quantized weights freezing).
 
   Convert the model parameter for serving. During conversion, quantized weights
   are created as variables, along with their scales.
 
   Args:
     train_state: TrainState containing model definitions and params.
     weight_only: If set, does not quantize activations.
+    legacy_for_freeze: If set, use legacy freezer during freeze.
+    legacy_for_serve: If set, use legacy freezer during serve.
 
   Returns:
     A tuple of serving function, and converted model parameters.
   """
   aqt_cfg = train_state.cnn_eval.aqt_cfg
   input_shape = (1, 28, 28, 1)
   activation_quant_mode = (
       utils.QuantMode.TRAIN if weight_only else utils.QuantMode.CONVERT
   )
   cnn_freeze = CNN(
       bn_use_stats=False,
       aqt_cfg=aqt_cfg,
       weights_quant_mode=utils.QuantMode.CONVERT,
       activation_quant_mode=activation_quant_mode,
+      use_legacy_freezer=legacy_for_freeze
   )
   _, model_serving = cnn_freeze.apply(
       train_state.model,
       jnp.ones(input_shape),
       rngs={'params': jax.random.PRNGKey(0)},
       mutable=True,
   )
   cnn_serve = CNN(
       bn_use_stats=False,
       aqt_cfg=aqt_cfg,
       weights_quant_mode=utils.QuantMode.SERVE,
       activation_quant_mode=activation_quant_mode,
+      use_legacy_freezer=legacy_for_serve
   )
 
   return cnn_serve.apply, model_serving
 
 
 def _merge_pytrees(from_model, to_model):
   """Copies the parameters from from_model to to_model."""
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model_test.py` & `aqtp-0.7.3/aqt/jax/v2/examples/flax_e2e_model_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -66,16 +66,16 @@
             "cpu": [
                 3.123474359512329101562500000000,
                 3.123474597930908203125000000000,
                 3.123473882675170898437500000000,  # colab
             ],
             "TPU v2": [3.198328018188476562500000000000],
             "TPU v3": [3.198328018188476562500000000000],
-            "TPU v4": [3.198297500610351562500000000000],
-            "TPU v5 lite": [3.198297500610351562500000000000],
+            "TPU v4": [3.198297739028930664062500000000],
+            "TPU v5 lite": [3.198297977447509765625000000000],
         },
         4: {
             "cpu": [2.258865118026733398437500000000],
             "TPU v2": [2.302409172058105468750000000000],
             "TPU v3": [2.302409172058105468750000000000],
             "TPU v4": [2.302409172058105468750000000000],
             "TPU v5 lite": [2.302409172058105468750000000000],
@@ -133,15 +133,15 @@
         "aqt": {
             "AqtEinsum_0": {
                 "AqtDotGeneral_0": {
                     "qlhs": {
                         "frozen": aqt_tensor.QTensor(
                             qvalue=(expected_dtype, (1, 2, 5, 1, 10)),
                             scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
-                            scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                            scale_t=None,
                             dequant_dtype=dtype("float32")
                         )
                     }
                 }
             },
             "Dense_0": {
                 "AqtDotGeneral_0": {
@@ -153,15 +153,15 @@
                             # The remaining shape 256 is not tiled, so (1, 256).
                             # Broadcast to other side adds a leading shape of 1.
                             qvalue=(expected_dtype, (1, 2, 1568, 1, 256)),
                             scale=[(dtype("float32"), (1, 2, 1, 1, 256))],
                             # The scale_t shape was (1, 256) before tiling.
                             # After tiling the scale shape is (1, 2, 1, 1, 256),
                             # then transposed to (2, 1, 1, 1, 256).
-                            scale_t=[(dtype("float32"), (2, 1, 1, 1, 256))],
+                            scale_t=None,
                             dequant_dtype=dtype("float32")
                         )
                     }
                 }
             },
             "Dense_1": {
                 "AqtDotGeneral_0": {
@@ -173,15 +173,15 @@
                             # The remaining shape 10 is not tiled, so (1, 10).
                             # Broadcast to other side adds a leading shape of 1.
                             qvalue=(expected_dtype, (1, 2, 128, 1, 10)),
                             scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
                             # The scale_t shape was (1, 10) before tiling.
                             # After tiling the scale shape is (1, 2, 1, 1, 10),
                             # then transposed to (2, 1, 1, 1, 10).
-                            scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                            scale_t=None,
                             dequant_dtype=dtype("float32")
                         )
                     }
                 }
             }
         },
         "batch_stats": {
@@ -397,63 +397,63 @@
     expected_aqt_pytree = {
         "AqtEinsum_0": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 5, 1, 10)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         },
         "Dense_0": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 1568, 1, 256)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 256))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 256))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         },
         "Dense_1": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 128, 1, 10)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         }
     }
 
@@ -608,63 +608,63 @@
     expected_aqt_pytree = {
         "AqtEinsum_0": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 5, 1, 10)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         },
         "Dense_0": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 1568, 1, 256)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 256))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 256))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         },
         "Dense_1": {
             "AqtDotGeneral_0": {
                 "qlhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=None,
                         scale=[(dtype("float32"), (1, 1, 1, 1, 1))],
-                        scale_t=[(dtype("float32"), (1, 1, 1, 1, 1))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 },
                 "qrhs": {
                     "frozen": aqt_tensor.QTensor(
                         qvalue=(expected_dtype, (1, 2, 128, 1, 10)),
                         scale=[(dtype("float32"), (1, 2, 1, 1, 10))],
-                        scale_t=[(dtype("float32"), (2, 1, 1, 1, 10))],
+                        scale_t=None,
                         dequant_dtype=dtype("float32")
                     )
                 }
             }
         }
     }
 
@@ -673,10 +673,86 @@
     )
     utils.test_pprint_eq(expected_aqt_pytree, serving_pytree["aqt"])
 
     # Compare logits of models before conversion and after conversion.
     logits_after_conversion, _ = forward(model_serving, serve_fn)
     assert (logits_before_conversion == logits_after_conversion).all()
 
+  def test_mnist_training_backward_compatibility(self):
+    aqt_cfg = config.config_v4()
+
+    def forward(model, apply_fn):
+      return apply_fn(
+          model,
+          ds["image"],
+          rngs={"params": jax.random.PRNGKey(0)},
+          mutable=True,
+      )
+
+    # RNGs
+    rng = jax.random.key(0)
+    rng, init_rng = jax.random.split(rng)
+    rng, image_rng = jax.random.split(rng)
+    rng, label_rng = jax.random.split(rng)
+    rng, input_rng = jax.random.split(rng)
+    del rng
+
+    # Dataset
+    ds_size = 8
+    ds = _dummy_dataset(ds_size, image_rng, label_rng)
+
+    # Stage 1: regular training
+    state = flax_e2e_model.create_train_state(init_rng, aqt_cfg)
+
+    state, _, _ = flax_e2e_model.train_epoch(
+        state, ds, batch_size=ds_size // 2, rng=input_rng
+    )
+
+    # Run forward once more in the same mode to get logits for testing below.
+    logits_s1, _ = forward(state.model, state.cnn_eval.apply)
+
+    # Stage 2: Model conversion (quantized weights freezing)
+    # Freeze with legacy freezer; serve with new freezer.
+    apply_serving, model_serving = flax_e2e_model.serving_conversion(
+        state, legacy_for_freeze=True, legacy_for_serve=False
+    )
+
+    dtype = jnp.dtype
+    expected_aqt_pytree = {
+        "AqtEinsum_0": {
+            "AqtDotGeneral_0": {
+                "qlhs": {
+                    "scale": (dtype("float32"), (2, 1, 1, 1, 10)),
+                    "value": (dtype("int8"), (1, 2, 5, 1, 10)),
+                }
+            }
+        },
+        "Dense_0": {
+            "AqtDotGeneral_0": {
+                "qrhs": {
+                    "scale": (dtype("float32"), (2, 1, 1, 1, 256)),
+                    "value": (dtype("int8"), (1, 2, 1568, 1, 256)),
+                }
+            }
+        },
+        "Dense_1": {
+            "AqtDotGeneral_0": {
+                "qrhs": {
+                    "scale": (dtype("float32"), (2, 1, 1, 1, 10)),
+                    "value": (dtype("int8"), (1, 2, 128, 1, 10)),
+                }
+            }
+        }
+    }
+
+    serving_pytree = jax.tree_util.tree_map(
+        lambda x: (x.dtype, x.shape), model_serving
+    )
+    utils.test_pprint_eq(expected_aqt_pytree, serving_pytree["aqt"])
+
+    # Stage 3: inference mode.
+    logits_s3, _ = forward(model_serving, apply_serving)
+    assert (logits_s3 == logits_s1).all()
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax.py` & `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,59 +89,98 @@
     if self.quant_mode == QuantMode.TRAIN:
       return None
     elif self.quant_mode == QuantMode.CALIBRATE:
       return None
     elif self.quant_mode == QuantMode.CONVERT:
       return None
     elif self.quant_mode == QuantMode.SERVE:
-      qvalue = self.qvalue.value
-      # TODO(b/325626080): Remove the optional logic.
-      if self.q_dtype == jnp.int4:
-        qvalue = qvalue.astype(jnp.int4)
       return aqt_tensor.QTensor(
-          qvalue,
+          qvalue=self.qvalue.value,
           scale=None,
           scale_t=[self.scale_t.value],
           # TODO(lew): Ideal solution: To find out this dequant_dtype one should
           # use the dtype of inputs of the quant function. We should store it as
           # a dtype of small-sized scale tensor.
           dequant_dtype=self.scale_t.value.dtype,
       )
     else:
       assert False, 'Unknown quant mode.'
 
   def set(self, inputs: aqt_tensor.QTensor) -> None:
-    # TODO(b/325626080): Uncomment the assert.
+    # TODO(b/325626080): Uncommenting the assert will fail.
     # assert inputs.qvalue.dtype == self.q_dtype, (
     #     f'Freezer got a QTensor of type {inputs.qvalue.dtype} but expected'
     #     f' {self.q_dtype}.'
     # )
     if self.quant_mode == QuantMode.TRAIN:
       pass
     elif self.quant_mode == QuantMode.CALIBRATE:
       pass
     elif self.quant_mode == QuantMode.CONVERT:
-      qvalue = inputs.qvalue
-      # TODO(b/325626080): Remove the optional logic.
-      if self.q_dtype == jnp.int4:
-        assert qvalue.dtype == jnp.int4
-        qvalue = qvalue.astype(jnp.int8)
-      self.qvalue.value = qvalue
+      self.qvalue.value = inputs.qvalue
       assert inputs.scale_t is not None and len(inputs.scale_t) == 1
       self.scale_t.value = inputs.scale_t[0]
     elif self.quant_mode == QuantMode.SERVE:
       # TODO(lew): Optionally compare stored and served value.
       pass
     else:
       assert False, 'Unknown quant mode.'
     return None
 
 
+def _maybe_recover_scale_from_scale_t(
+    qt: aqt_tensor.QTensor | None,
+    dimension_numbers: jax.lax.DotDimensionNumbers,
+    is_rhs: bool,
+    lhs_shape: Sequence[int],
+    rhs_shape: Sequence[int],
+) -> aqt_tensor.QTensor:
+  """Recovers scale from scale_t if necessary."""
+  if qt is None or qt.scale is not None or qt.scale_t is None:
+    return qt
+
+  transpose_fn = transpose.lhs_recover_scale_from_scale_t
+  if is_rhs:
+    transpose_fn = transpose.rhs_recover_scale_from_scale_t
+
+  return qt.replace(
+      scale=[
+          transpose_fn(scale_t, dimension_numbers, lhs_shape, rhs_shape)
+          for scale_t in qt.scale_t
+      ],
+      scale_t=None,
+  )
+
+
+def _populate_scale_t(
+    qt: aqt_tensor.QTensor,
+    dimension_numbers: jax.lax.DotDimensionNumbers,
+    is_rhs: bool,
+    lhs_shape: Sequence[int],
+    rhs_shape: Sequence[int],
+) -> aqt_tensor.QTensor:
+  """Populates scale_t from scale."""
+  if qt.scale is None:
+    return qt
+
+  transpose_fn = transpose.lhs_scale_transpose_to_output
+  if is_rhs:
+    transpose_fn = transpose.rhs_scale_transpose_to_output
+
+  return qt.replace(
+      scale_t=[
+          transpose_fn(scale, dimension_numbers, lhs_shape, rhs_shape)
+          for scale in qt.scale
+      ]
+  )
+
+
 class AqtDotGeneral(nn.Module):
   """A layer that can be injected into flax.nn.Dense, etc."""
+
   cfg: Optional[aqt_dot_general.DotGeneral] = None
   prng_name: Optional[str] = 'params'
 
   # TODO(lew): split out separate class for each side.
   # Quant mode determines whether flax variables are created to store quantized
   # inputs. Refer to the Freezer doc str to see variable creation in each mode.
   lhs_quant_mode: QuantMode = QuantMode.TRAIN
@@ -165,15 +204,15 @@
   # Variables only for the new Freezer.
   lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
   rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
 
   # Freeze mode. Set as FreezerMode.CALIBRATION to store only scales; set as
   # CALIBRATION_AND_VALUE to store both scales and quantized values.
   lhs_freeze_mode: FreezerMode = FreezerMode.NONE
-  rhs_freeze_mode: FreezerMode = FreezerMode.CALIBRATION_AND_VALUE
+  rhs_freeze_mode: FreezerMode = FreezerMode.NONE
 
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
   tiling_cfg: Optional[tiled_dot_general.Cfg] = None
 
   # If set to True, use the current Freezer. Otherwise, use the new
@@ -243,40 +282,51 @@
           QuantMode.CALIBRATE: general_freezer.FreezerMode.NONE,
           QuantMode.CONVERT: general_freezer.FreezerMode.WRITE,
           QuantMode.SERVE: general_freezer.FreezerMode.READ,
       }
 
       def init_wrapper(
           qt: aqt_tensor.QTensor,
+          contracting_axis: Sequence[utils.AxisIdx],
           axis_metadata_wrapper: Optional[AxisMetadataWrapper],
       ):
         if axis_metadata_wrapper is None:
           return qt
 
-        # We are not doing any sharding for scale and scale_t, for now.
-        scale_non_shard_axis = range(qt.ndim)
+        scale_non_shard_axis_all = list(range(qt.ndim))
+        scale_non_shard_axis_contracting = list(contracting_axis)
 
         qt = qt.replace(
             qvalue=axis_metadata_wrapper(qt.qvalue, []),
             scale=jax.tree_map(
-                lambda x: axis_metadata_wrapper(x, scale_non_shard_axis),
+                lambda x: axis_metadata_wrapper(
+                    x, scale_non_shard_axis_contracting
+                ),
                 qt.scale,
             ),
+            # Passing scale_non_shard_axis_contracting would be incorrect due to
+            # scale transposition. scale_t is being removed from QTensor anyway
+            # so we just pass scale_non_shard_axis_all.
             scale_t=jax.tree_map(
-                lambda x: axis_metadata_wrapper(x, scale_non_shard_axis),
+                lambda x: axis_metadata_wrapper(x, scale_non_shard_axis_all),
                 qt.scale_t,
             ),
         )
         return qt
 
+      lhs_ca, rhs_ca = contr
       lhs_init_wrapper = functools.partial(
-          init_wrapper, axis_metadata_wrapper=self.lhs_axis_metadata_wrapper
+          init_wrapper,
+          contracting_axis=lhs_ca,
+          axis_metadata_wrapper=self.lhs_axis_metadata_wrapper
       )
       rhs_init_wrapper = functools.partial(
-          init_wrapper, axis_metadata_wrapper=self.rhs_axis_metadata_wrapper
+          init_wrapper,
+          contracting_axis=rhs_ca,
+          axis_metadata_wrapper=self.rhs_axis_metadata_wrapper
       )
 
       lhs_freezer = general_freezer.Freezer(
           name=self.lhs_var_name,
           mode=quant_to_freezer_mode[lhs_qm],
           collection=self.quant_collection,
           axis_metadata_wrapper=lhs_init_wrapper,
@@ -322,14 +372,23 @@
 
       # Getter
       lhs_apply_quant_mode = self.lhs_apply_quant_mode
       rhs_apply_quant_mode = self.rhs_apply_quant_mode
       lhs_qt = lhs_freezer.get() if lhs_apply_quant_mode else self.lhs_qtensor
       rhs_qt = rhs_freezer.get() if rhs_apply_quant_mode else self.rhs_qtensor
 
+      # Recover scale from scale_t, if necessary.
+      # The quantized tensor loaded from the legacy freezer has only scale_t.
+      lhs_qt = _maybe_recover_scale_from_scale_t(
+          lhs_qt, dimension_numbers, False, lhs_shape, rhs_shape
+      )
+      rhs_qt = _maybe_recover_scale_from_scale_t(
+          rhs_qt, dimension_numbers, True, lhs_shape, rhs_shape
+      )
+
       cfg.apply_custom_vjp_on_jax = False
       out, (out_lhs_qt, out_rhs_qt) = aqt_flax_dg_core.dg_core_flax_lifted(
           lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self, cfg
       )
 
       # Remove qvalue of the activation to not to store it in Freezer.
       match self.lhs_freeze_mode:
@@ -357,14 +416,26 @@
           out_rhs_qt = out_rhs_qt.without_qvalue()
         case FreezerMode.CALIBRATION_AND_VALUE:
           pass
         case _:
           raise ValueError('Unknown freeze mode: %s' % self.rhs_freeze_mode)
 
       # Setter
+      calib_contracting_axis = aqt_dot_general.CalibrationMode.CONTRACTING_AXIS
+      if self.use_legacy_freezer:
+        # We need to populate the stored QTensor with scale_t.
+        if cfg.fwd.lhs.calibration_mode == calib_contracting_axis:
+          out_lhs_qt = _populate_scale_t(
+              out_lhs_qt, dimension_numbers, False, lhs_shape, rhs_shape
+          )
+        if cfg.fwd.rhs.calibration_mode == calib_contracting_axis:
+          out_rhs_qt = _populate_scale_t(
+              out_rhs_qt, dimension_numbers, True, lhs_shape, rhs_shape
+          )
+
       if self.lhs_apply_quant_mode:
         lhs_freezer.set(out_lhs_qt)
       if self.rhs_apply_quant_mode:
         rhs_freezer.set(out_rhs_qt)
 
       return out
 
@@ -439,15 +510,15 @@
   # Variables only for the new Freezer.
   lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
   rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
 
   # Freeze mode. Set as FreezerMode.CALIBRATION to store only scales; set as
   # CALIBRATION_AND_VALUE to store both scales and quantized values.
   lhs_freeze_mode: FreezerMode = FreezerMode.NONE
-  rhs_freeze_mode: FreezerMode = FreezerMode.CALIBRATION_AND_VALUE
+  rhs_freeze_mode: FreezerMode = FreezerMode.NONE
 
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
 
   assert_eqn: Optional[str] = None
   assert_lhs_shape: Optional[utils.ShapeTemplate] = None
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_calibration.py` & `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_calibration.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 _SUM_OF_ONES = "sum_of_ones"
 _SUM_OF_VALS = "sum_of_vals"
 _MAX_OF_ABS_VALS = "max_of_abs_vals"
 _SUM_OF_L1_VALS = "sum_of_l1_vals"
 _SUM_OF_LP_VALS = "sum_of_lp_vals"
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class MeanOfAbsMaxCalibration(calibration.Calibration, nn.Module):
   """State for static range AQT/PTQ/QAT."""
 
   quant_collection: str
 
   @nn.compact
   def get_bound(
@@ -218,9 +218,7 @@
 
     return (
         self.l1_dev_coeff * self._l1_dev()
         + self.lp_dev_coeff * self._lp_dev()
         + self.max_dev_coeff * self._max_dev()
         + self.const_bound_coeff
     )
-
-
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_dg_core.py` & `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_dg_core.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_test.py` & `aqtp-0.7.3/aqt/jax/v2/flax/aqt_flax_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,15 +49,19 @@
           lhs_dtype = self.aqt_cfg.fwd.dg_quantizer.lhs.numerics.get_dtype()
           rhs_dtype = self.aqt_cfg.fwd.dg_quantizer.rhs.numerics.get_dtype()
           if self.lhs_qt_external:
             lhs_in = lhs_q.qvalue_astype(lhs_dtype)
           if self.rhs_qt_external:
             rhs_in = rhs_q.qvalue_astype(rhs_dtype)
 
-        einsum = aqt_flax.AqtEinsum(cfg=self.aqt_cfg)
+        einsum = aqt_flax.AqtEinsum(
+            cfg=self.aqt_cfg,
+            lhs_freeze_mode=aqt_flax.FreezerMode.NONE,
+            rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
+        )
         # xhs_qt can be inputs to AqtEinsum
         # xhs->xhs_qt can happen outside of AqtEinsum, e.g., k/v cache quant
         # input xhs_qt will force get_tensor() to always return xhs_qt
         out = einsum('ijkh,mkh->ijm', lhs_in, rhs_in)
         return out
 
     key = jax.random.PRNGKey(0)
@@ -93,15 +97,19 @@
 
   def test_einsum_grad_leak(self):
     class CNN(nn.Module):
       aqt_cfg: config.DotGeneral
 
       @nn.compact
       def __call__(self, x):
-        einsum = aqt_flax.AqtEinsum(self.aqt_cfg)
+        einsum = aqt_flax.AqtEinsum(
+            self.aqt_cfg,
+            lhs_freeze_mode=aqt_flax.FreezerMode.NONE,
+            rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE
+        )
         x = einsum('bc,ab->ac', jnp.identity(10, dtype=x.dtype), x)
         return x
 
     model = CNN(aqt_cfg=config.fully_quantized())
     var = model.init({'params': jax.random.PRNGKey(0)}, jnp.ones(shape=(1, 10)))
 
     @jax.jit
@@ -130,14 +138,16 @@
         kernel = self.param(
             'kernel', nn.initializers.lecun_normal(), shape=(2, 5, 6)
         )
         einsum = aqt_flax.AqtEinsum(
             cfg=self.aqt_cfg,
             lhs_quant_mode=self.lhs_quant_mode,
             rhs_quant_mode=self.rhs_quant_mode,
+            lhs_freeze_mode=aqt_flax.FreezerMode.NONE,
+            rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
             use_legacy_freezer=self.use_legacy_freezer,
         )
         out = einsum('ijkh,mkh->ijm', lhs, kernel)
         return out
 
     key = jax.random.PRNGKey(0)
     subkeys = jax.random.split(key, num=6)
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/freezer.py` & `aqtp-0.7.3/aqt/jax/v2/flax/freezer.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/freezer_test.py` & `aqtp-0.7.3/aqt/jax/v2/flax/freezer_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/intercept/README.md` & `aqtp-0.7.3/aqt/jax/v2/flax/intercept/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py` & `aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py` & `aqtp-0.7.3/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py` & `aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 """Mnist example for intercept method API."""
 
 from absl import app
 from aqt.jax.v2 import config as aqt_config
 from aqt.jax.v2 import tiled_dot_general
 from aqt.jax.v2 import utils as aqt_utils
 from aqt.jax.v2.examples import flax_e2e_model
+from aqt.jax.v2.flax import aqt_flax
 from aqt.jax.v2.flax.intercept import aqt_intercept_methods
 from flax import linen as nn
 from flax.metrics import tensorboard
 import jax
 import jax.numpy as jnp
 import optax
 
@@ -118,14 +119,16 @@
   input_shape = (1, 28, 28, 1)
   cnn_freeze = CNN(
       bn_use_stats=False,
   )
   with aqt_intercept_methods.intercept_methods(
       aqt_cfg,
       rhs_quant_mode=aqt_utils.QuantMode.CONVERT,
+      lhs_freeze_mode=aqt_flax.FreezerMode.NONE,
+      rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
       tiling_cfg=tiling_cfg):
     _, model_serving = cnn_freeze.apply(
         train_state.model,
         jnp.ones(input_shape),
         rngs={'params': jax.random.PRNGKey(0)},
         mutable=True,
     )
@@ -133,14 +136,16 @@
       bn_use_stats=False,
   )
 
   serve_fn = aqt_intercept_methods.intercept_wrapper(
       cnn_serve.apply,
       aqt_cfg,
       rhs_quant_mode=aqt_utils.QuantMode.SERVE,
+      lhs_freeze_mode=aqt_flax.FreezerMode.NONE,
+      rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
       tiling_cfg=tiling_cfg)
   return serve_fn, model_serving
 
 
 @jax.jit
 def serve(state,
           aqt_cfg: aqt_config.DotGeneral,
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py` & `aqtp-0.7.3/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 ),
             ],
             remaining_axes=[],
         ),
     )
     target_loss = {
         8: {
-            "TPU v5 lite": [3.222228527069091796875000000000],
+            "TPU v5 lite": [3.222529888153076171875000000000],
         },
         4: {
             "TPU v5 lite": [2.292296886444091796875000000000],
         },
     }
     # below 3 lines are differences between config_v4/v3 and fully_quantized
     config.set_stochastic_rounding(aqt_cfg, True, True, "jax.uniform")
@@ -127,15 +127,15 @@
 
     # Stage 2: Model conversion (quantized weights freezing)
 
     apply_serving, model_serving = flax_e2e_intercept_model.serving_conversion(
         state, aqt_cfg, tiling_cfg)
 
     dtype = jnp.dtype
-    expected_dtype = jnp.int8
+    expected_dtype = jnp.int4 if bits == 4 else jnp.int8
     expected_aqt_pytree = {
         "aqt": {
             "Dense_0": {
                 "AqtDotGeneral_0": {
                     "qrhs": {
                         # The scale_t shape was (1, 256) before tiling.
                         # After tiling the scale shape is (1, 2, 1, 1, 256),
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics.py` & `aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   # TODO(lew): Is bitwise_and needed? Maybe round_to_nearest_even is ok.
   x = jax.lax.bitwise_and(x, ~noise_mask)  # zero-out lowest bits in mantissa
   x = jax.lax.bitcast_convert_type(x, input_dtype)
 
   return x
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class Fp8Numerics(numerics.AqtNumerics):
   """Numerics for fp8."""
 
   # Storage type.
   dtype: Literal[jnp.float8_e4m3fn, jnp.float8_e5m2, jnp.bfloat16]
 
   # Requested rounding precision.
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics_test.py` & `aqtp-0.7.3/aqt/jax/v2/numerics/fp8_numerics_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,28 +127,28 @@
                 # Different CPU models are not bit exact and sometimes produce
                 # different losses under the same training setting.
                 3.167505979537963867187500000000,
                 3.167067050933837890625000000000,  # skylake, cascadelake
             ],
             "TPU v2": [3.210080146789550781250000000000],
             "TPU v3": [3.210082530975341796875000000000],
-            "TPU v4": [3.213466644287109375000000000000],
-            "TPU v5 lite": [3.213290691375732421875000000000],
+            "TPU v4": [3.210082530975341796875000000000],
+            "TPU v5 lite": [3.212916374206542968750000000000],
         },
         "e5m2": {
             "cpu": [
                 # Different CPU models are not bit exact and sometimes produce
                 # different losses under the same training setting.
                 3.112026929855346679687500000000,
                 3.112026691436767578125000000000,
             ],
             "TPU v2": [3.181228160858154296875000000000],
             "TPU v3": [3.181227684020996093750000000000],
-            "TPU v4": [3.181212902069091796875000000000],
-            "TPU v5 lite": [3.181214332580566406250000000000],
+            "TPU v4": [3.181228160858154296875000000000],
+            "TPU v5 lite": [3.181028842926025390625000000000],
         },
     }
 
     # RNGs
     rng = jax.random.key(0)
     rng, init_rng = jax.random.split(rng)
     rng, image_rng = jax.random.split(rng)
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/numerics/int_numerics.py` & `aqtp-0.7.3/aqt/jax/v2/numerics/int_numerics.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from aqt.jax.v2 import stochastic_rounding
 from aqt.jax.v2 import utils
 from aqt.jax.v2.numerics import numerics
 from jax import lax
 import jax.numpy as jnp
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class IntNumerics(numerics.AqtNumerics):
   """Numerics for int8, int4, binary, etc."""
 
   bits: int
   preserve_zero: bool
   # false = map max val on the end of the last bucket
   # true = map max val on the middle of the last
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/numerics/no_numerics.py` & `aqtp-0.7.3/aqt/jax/v2/numerics/no_numerics.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from typing import Any, Optional
 from aqt.jax.v2 import stochastic_rounding
 from aqt.jax.v2 import utils
 from aqt.jax.v2.numerics import numerics
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class NoNumerics(numerics.AqtNumerics):
   """No quantization, use a native type such as bf16."""
 
   # TODO(lew): This is a workaround. We should separate Stochastic Rounding.
   # noise_fn has no effect in NoNumerics.
   noise_fn: Optional[stochastic_rounding.NoiseFn] = None
   dtype: Optional[Any] = None
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/numerics/numerics.py` & `aqtp-0.7.3/aqt/jax/v2/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops.py` & `aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops_test.py` & `aqtp-0.7.3/aqt/jax/v2/pax/pax_base_ops_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/stochastic_rounding.py` & `aqtp-0.7.3/aqt/jax/v2/stochastic_rounding.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 import jax
 import jax.numpy as jnp
 
 
 NoiseFn = Callable[[tuple[int, ...], jax.Array], jnp.ndarray]
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class JaxUniform:
   """Jax uniform noise."""
 
   def __call__(self, shape: tuple[int, ...], key: jax.Array) -> jnp.ndarray:
     return jax.random.uniform(key, shape) - 0.5
 
 
-@utils.flax_slots_dataclass
+@utils.flax_slots_kw_only_dataclass
 class RandomCenteredUniform:
   """Customized efficient implementation for random centered uniform noise."""
 
   def __call__(self, shape: tuple[int, ...], key: jax.Array) -> jnp.ndarray:
     """Generates uniform number in [-0.5, 0.5]."""
     dtype = jnp.dtype('uint16')
     nbits = jnp.iinfo(dtype).bits
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/tiled_dot_general.py` & `aqtp-0.7.3/aqt/jax/v2/tiled_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/tiled_dot_general_test.py` & `aqtp-0.7.3/aqt/jax/v2/tiled_dot_general_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Test for AQT Tiled Dot General."""
+import functools
 import itertools
 
 from absl.testing import absltest
 from absl.testing import parameterized
 from aqt.jax.v2 import tiled_dot_general
 from aqt.jax.v2 import utils
 import jax
@@ -135,14 +136,59 @@
         )
   print(f'{len(cfgs)} configs in total.')
   return cfgs
 
 
 class TiledDotGeneralTest(parameterized.TestCase):
 
+  def test_tiled_dot_general_shape(self):
+    for i in range(10):
+      key1, key2 = jax.random.split(jax.random.PRNGKey(i), 2)
+      hypers = jax.random.randint(key1, shape=(4,), minval=2, maxval=7)
+      num_ca = hypers[0]
+      num_ba = hypers[1]
+      num_lhs_ra = hypers[2]
+      num_rhs_ra = hypers[3]
+      max_shape_val = 6
+      lhs, rhs, lhs_axes, rhs_axes = generate_inputs(
+          key2, num_ca, num_ba, num_lhs_ra, num_rhs_ra, max_shape_val
+      )
+      lhs_ca, lhs_ba, lhs_ra = lhs_axes
+      rhs_ca, rhs_ba, rhs_ra = rhs_axes
+      dims = ((tuple(lhs_ca), tuple(rhs_ca)), (tuple(lhs_ba), tuple(rhs_ba)))
+
+      def _lax_dg(dims, lhs_in, rhs_in):
+        return jax.lax.dot_general(lhs_in, rhs_in, dims)
+
+      def _tiled_dg(cfg_in, dims, lhs_in, rhs_in):
+        return tiled_dot_general.tiled_dot_general(cfg_in, lhs_in, rhs_in, dims)
+
+      lax_dg_test = functools.partial(_lax_dg, dims)
+      expected_output_shape = jax.eval_shape(lax_dg_test, lhs, rhs).shape
+
+      tiling_cfgs = generate_tiling_cfgs(
+          lhs.shape, lhs_ca, lhs_ra, rhs.shape, rhs_ca, rhs_ra
+      )
+      for i in range(len(tiling_cfgs)):
+        cfg_in = tiling_cfgs[i]
+        tiled_dg_test = functools.partial(_tiled_dg, cfg_in, dims)
+        output_shape = jax.eval_shape(tiled_dg_test, lhs, rhs).shape
+        msg = (
+            'Test failed. Please try the following single test:\n'
+            f'lhs_shape = {lhs.shape}\n'
+            f'rhs_shape = {rhs.shape}\n'
+            'lhs = jnp.ones(lhs_shape)\n'
+            'rhs = jnp.ones(rhs_shape)\n'
+            f'cfg = {cfg_in}\n'
+            f'dims = {dims}\n'
+            'out = tiled_dot_general.local_dg(cfg, lhs, rhs, dims)\n'
+            'assert out.shape == jax.lax.dot_general(lhs, rhs, dims).shape'
+        )
+        assert output_shape == expected_output_shape, msg
+
   def test_tiled_dot_general(self):
     num_ca = 2
     num_ba = 2
     num_lhs_ra = 2
     num_rhs_ra = 2
     max_shape_val = 32
     key = jax.random.PRNGKey(7)
```

### Comparing `aqtp-0.7.2/aqt/jax/v2/transpose.py` & `aqtp-0.7.3/aqt/jax/v2/transpose.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/transpose_test.py` & `aqtp-0.7.3/aqt/jax/v2/transpose_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax/v2/utils.py` & `aqtp-0.7.3/aqt/jax/v2/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,14 +55,22 @@
   assert value == expected, msg
 
 
 flax_slots_dataclass = functools.partial(
     flax.struct.dataclass, frozen=False, slots=True
 )
 
+# TODO: b/332418233 - Consolidate flax_slots_kw_only_dataclass and
+# flax_slots_dataclass into a single decorator once the migration is
+# done. This will exist only temporarily while completing the
+# migration.
+flax_slots_kw_only_dataclass = functools.partial(
+    flax_slots_dataclass, kw_only=True
+)
+
 
 class QuantMode(enum.Enum):
   TRAIN = 1
   CALIBRATE = 2
   CONVERT = 3
   SERVE = 4
```

### Comparing `aqtp-0.7.2/aqt/jax_legacy/README.md` & `aqtp-0.7.3/aqt/jax_legacy/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb` & `aqtp-0.7.3/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/README.md` & `aqtp-0.7.3/aqt/jax_legacy/jax/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax_attention_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/flax_layers_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/get_bounds_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/README.md` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/imagenet.png` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/imagenet.png`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_benchmark.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/imagenet/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/primitives.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/quant_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/quantization_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/stats.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/train_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/train_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/utils.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/README.md` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py` & `aqtp-0.7.3/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/README.md` & `aqtp-0.7.3/aqt/jax_legacy/utils/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/analysis_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/common.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/config_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/hparams_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.7.3/aqt/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/test/aqt_conv_test_base.py` & `aqtp-0.7.3/aqt/test/aqt_conv_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/test/aqt_matmul_test_base.py` & `aqtp-0.7.3/aqt/test/aqt_matmul_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/test/aqt_stats_test_base.py` & `aqtp-0.7.3/aqt/test/aqt_stats_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/test/aqt_tensor_test_base.py` & `aqtp-0.7.3/aqt/test/aqt_tensor_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/aqt/test/aqt_test_shared_base.py` & `aqtp-0.7.3/aqt/test/aqt_test_shared_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/papers/aqt/aqt.pdf` & `aqtp-0.7.3/papers/aqt/aqt.pdf`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/papers/aqt/aqt.tex` & `aqtp-0.7.3/papers/aqt/aqt.tex`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/papers/pokebnn/README.md` & `aqtp-0.7.3/papers/pokebnn/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/papers/pokebnn/cloudtpu_train_pokebnn.sh` & `aqtp-0.7.3/papers/pokebnn/cloudtpu_train_pokebnn.sh`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/papers/pokebnn/tensorboard.ipynb` & `aqtp-0.7.3/papers/pokebnn/tensorboard.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/pyproject.toml` & `aqtp-0.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/setup.py` & `aqtp-0.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.2/PKG-INFO` & `aqtp-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtp
-Version: 0.7.2
+Version: 0.7.3
 Summary: Accurate Quantized Training library.
 Author-email: Lukasz Lew <lew@google.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

