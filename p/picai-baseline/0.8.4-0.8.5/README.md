# Comparing `tmp/picai_baseline-0.8.4.tar.gz` & `tmp/picai_baseline-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picai_baseline-0.8.4.tar", last modified: Mon May 15 16:55:07 2023, max compression
+gzip compressed data, was "picai_baseline-0.8.5.tar", last modified: Mon May 13 13:17:19 2024, max compression
```

## Comparing `picai_baseline-0.8.4.tar` & `picai_baseline-0.8.5.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422766 picai_baseline-0.8.4/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-12-13 09:52:15.000000 picai_baseline-0.8.4/LICENSE
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12928 2023-05-15 16:55:07.422936 picai_baseline-0.8.4/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12133 2023-04-04 06:58:41.000000 picai_baseline-0.8.4/README.md
--rw-r--r--   0 joeranbosma   (501) staff       (20)      472 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/pyproject.toml
--rw-r--r--   0 joeranbosma   (501) staff       (20)      870 2023-05-15 16:55:07.423324 picai_baseline-0.8.4/setup.cfg
--rw-r--r--   0 joeranbosma   (501) staff       (20)      727 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/setup.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.390154 picai_baseline-0.8.4/src/
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.393066 picai_baseline-0.8.4/src/picai_baseline/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      856 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5232 2023-01-12 14:14:37.000000 picai_baseline-0.8.4/src/picai_baseline/__main__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.395628 picai_baseline-0.8.4/src/picai_baseline/nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-08-31 20:12:51.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10618 2022-12-21 09:40:52.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/eval.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5686 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/nnunet_baseline.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10820 2022-08-31 20:12:51.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/softmax_export.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.397801 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/__init__.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6708 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/focal_loss.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3692 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/io.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     2490 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     7957 2023-03-25 11:22:48.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py
--rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6302 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    23090 2023-05-02 09:49:54.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12650 2023-03-12 12:34:38.000000 picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/run_training.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     8937 2023-02-28 11:37:27.000000 picai_baseline-0.8.4/src/picai_baseline/prepare_data.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10485 2023-02-28 11:36:42.000000 picai_baseline-0.8.4/src/picai_baseline/prepare_data_semi_supervised.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.397954 picai_baseline-0.8.4/src/picai_baseline/splits/
--rw-r--r--   0 joeranbosma   (501) staff       (20)   202261 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/__init__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.402204 picai_baseline-0.8.4/src/picai_baseline/splits/picai/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      333 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30030 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30080 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29980 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    29930 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    30130 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7530 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7480 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7580 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7630 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     7430 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   217842 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.404792 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      345 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      180 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      205 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      130 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)      105 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1792 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.405230 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1705 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      347 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)   188117 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.409610 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     3126 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      349 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)   181905 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182355 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182230 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182080 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)   182280 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45830 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45380 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45505 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45655 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)    45455 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json
--rw-r--r--   0 joeranbosma   (501) staff       (20)  1320857 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.411924 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1761 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      419 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__main__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)  1191517 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.417561 picai_baseline-0.8.4/src/picai_baseline/unet/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5647 2022-12-20 10:42:09.000000 picai_baseline-0.8.4/src/picai_baseline/unet/plan_overview.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     8439 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/src/picai_baseline/unet/train.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.420665 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/__init__.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.421491 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    11063 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     9507 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1806 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      667 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    10436 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/callbacks.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1192 2022-08-15 08:53:24.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/compute_spec.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5856 2023-05-15 14:35:12.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/data_generator.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1501 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/default_hyperparam.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5146 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/image_reader.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.421802 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1765 2023-05-15 14:34:37.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/focal.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1287 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_network_selector.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422232 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/
--rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/__init__.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)    14022 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/unets.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)      852 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/poly_lr.py
--rw-r--r--   0 joeranbosma   (501) staff       (20)     1644 2022-07-03 16:12:55.000000 picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/preprocess_utils.py
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.394174 picai_baseline-0.8.4/src/picai_baseline.egg-info/
--rw-r--r--   0 joeranbosma   (501) staff       (20)    12928 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/PKG-INFO
--rw-r--r--   0 joeranbosma   (501) staff       (20)     5131 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/SOURCES.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/dependency_links.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-01-11 10:53:56.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/not-zip-safe
--rw-r--r--   0 joeranbosma   (501) staff       (20)      149 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/requires.txt
--rw-r--r--   0 joeranbosma   (501) staff       (20)       15 2023-05-15 16:55:07.000000 picai_baseline-0.8.4/src/picai_baseline.egg-info/top_level.txt
-drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2023-05-15 16:55:07.422400 picai_baseline-0.8.4/tests/
--rw-r--r--   0 joeranbosma   (501) staff       (20)     4719 2022-12-12 13:16:27.000000 picai_baseline-0.8.4/tests/test_splits.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.284851 picai_baseline-0.8.5/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11357 2022-12-13 09:52:15.000000 picai_baseline-0.8.5/LICENSE
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    15026 2024-05-13 13:17:19.284646 picai_baseline-0.8.5/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    13813 2023-09-17 17:40:40.000000 picai_baseline-0.8.5/README.md
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      472 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/pyproject.toml
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      870 2024-05-13 13:17:19.285197 picai_baseline-0.8.5/setup.cfg
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      727 2024-05-13 13:08:06.000000 picai_baseline-0.8.5/setup.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.250213 picai_baseline-0.8.5/src/
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.254065 picai_baseline-0.8.5/src/picai_baseline/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      856 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5232 2023-01-12 14:14:37.000000 picai_baseline-0.8.5/src/picai_baseline/__main__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.256451 picai_baseline-0.8.5/src/picai_baseline/nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-08-31 20:12:51.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10618 2022-12-21 09:40:52.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/eval.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5686 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/nnunet_baseline.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10820 2022-08-31 20:12:51.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/softmax_export.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.258997 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/__init__.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6708 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/focal_loss.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3692 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/io.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     2490 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     7957 2023-03-25 11:22:48.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py
+-rwxr-xr-x   0 joeranbosma   (501) staff       (20)     6302 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    23090 2023-05-02 09:49:54.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    12650 2023-03-12 12:34:38.000000 picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/run_training.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     8977 2023-05-30 10:18:48.000000 picai_baseline-0.8.5/src/picai_baseline/prepare_data.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10485 2023-02-28 11:36:42.000000 picai_baseline-0.8.5/src/picai_baseline/prepare_data_semi_supervised.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        0 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/py.typed
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.259188 picai_baseline-0.8.5/src/picai_baseline/splits/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   202261 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/__init__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.262927 picai_baseline-0.8.5/src/picai_baseline/splits/picai/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      333 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30030 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30080 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29980 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    29930 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    30130 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7530 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7480 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7580 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7630 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     7430 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   217842 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.265745 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1304 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      345 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      180 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      255 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      205 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      130 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       55 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      105 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1792 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.266229 picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1705 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      347 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   188117 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.271148 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     3126 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      349 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   181905 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182355 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182230 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182080 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)   182280 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45830 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45380 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45505 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45655 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    45455 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json
+-rw-r--r--   0 joeranbosma   (501) staff       (20)  1320857 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.273231 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1761 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      419 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/__main__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)  1191517 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.277367 picai_baseline-0.8.5/src/picai_baseline/unet/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5647 2022-12-20 10:42:09.000000 picai_baseline-0.8.5/src/picai_baseline/unet/plan_overview.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     8439 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/src/picai_baseline/unet/train.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.281618 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/__init__.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.282702 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    11063 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     9507 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1806 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      667 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    10869 2023-11-14 17:11:01.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/callbacks.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1192 2022-08-15 08:53:24.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/compute_spec.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5856 2023-05-15 14:35:12.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/data_generator.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1501 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/default_hyperparam.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5146 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/image_reader.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.283015 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/loss_functions/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/loss_functions/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1614 2023-11-14 17:11:01.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/loss_functions/focal.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1287 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_network_selector.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.283401 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_networks/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_networks/__init__.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    14022 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_networks/unets.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      852 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/poly_lr.py
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     1644 2022-07-03 16:12:55.000000 picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/preprocess_utils.py
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.283896 picai_baseline-0.8.5/src/picai_baseline.egg-info/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)    15026 2024-05-13 13:17:19.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/PKG-INFO
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     5159 2024-05-13 13:17:19.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/SOURCES.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2024-05-13 13:17:19.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/dependency_links.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)        1 2023-01-11 10:53:56.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/not-zip-safe
+-rw-r--r--   0 joeranbosma   (501) staff       (20)      149 2024-05-13 13:17:19.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/requires.txt
+-rw-r--r--   0 joeranbosma   (501) staff       (20)       15 2024-05-13 13:17:19.000000 picai_baseline-0.8.5/src/picai_baseline.egg-info/top_level.txt
+drwxr-xr-x   0 joeranbosma   (501) staff       (20)        0 2024-05-13 13:17:19.283569 picai_baseline-0.8.5/tests/
+-rw-r--r--   0 joeranbosma   (501) staff       (20)     4719 2022-12-12 13:16:27.000000 picai_baseline-0.8.5/tests/test_splits.py
```

### Comparing `picai_baseline-0.8.4/LICENSE` & `picai_baseline-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/PKG-INFO` & `picai_baseline-0.8.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,10 @@
-Metadata-Version: 2.1
-Name: picai_baseline
-Version: 0.8.4
-Summary: PICAI Baselines
-Home-page: https://github.com/DIAGNijmegen/picai_baseline
-Author: Joeran Bosma
-Author-email: Joeran.Bosma@radboudumc.nl
-License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_baseline/issues
-Platform: unix
-Platform: linux
-Platform: osx
-Platform: cygwin
-Platform: win32
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # Baseline AI Models for Prostate Cancer Detection in MRI
 
-This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models will be provided and supported:
+This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models are provided and supported:
 
 - [U-Net](unet_baseline.md)
 - [nnU-Net](nnunet_baseline.md)
 - [nnDetection](nndetection_baseline.md)
 
 All three solutions share the same starting point, with respect to their expected [folder structure](#folder-structure) and [data preparation](#data-preparation) pipeline.
 
@@ -48,24 +23,24 @@
 
 ```bash
 git clone https://github.com/DIAGNijmegen/picai_baseline
 cd picai_baseline
 pip install -e .
 ```
 
-This ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option. Furthermore, this ensures the latest version is installed.
+Installing from source ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option.
 
 
 ## General Setup
-We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
+We define setup steps that are shared between the different baseline algorithms. To follow the model-specific baseline algorithm tutorials, these steps must be completed first.
 
 
 ### Folder Structure
-We define three main folders that must be prepared apriori:
-- `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
+We define three main folders that must be prepared:
+- `/input/` contains the [PI-CAI dataset](https://pi-cai.grand-challenge.org/DATA/). In this tutorial we assume this is the PI-CAI Public Training and Development Dataset.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
   - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
@@ -143,34 +118,37 @@
 
 ```bash
 python -m picai_baseline.splits.picai_nnunet --output "/workdir/splits/picai_nnunet"
 ```
 
 
 ### Data Preprocessing
-We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
+We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. The [`picai_prep`][picai_prep] module allows to resample all cases to the same resolution (you can resample each case indivudually to the same resolution between the different sequences, or choose to resample the full dataset to the same resolution). For details on the available options to convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please see the instructions [provided here][picai_prep_mha2nnunet]. Below we give the conversion as performed for the [baseline semi-supervised nnU-Net](https://grand-challenge.org/algorithms/pi-cai-pubpriv-nnu-net-semi-supervised/). For the U-Net baseline, please see the [U-Net tutorial](src/picai_baseline/unet_baseline.md#u-net---data-preparation) for extra instructions.
 
-To convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please follow the instructions [provided here][picai_prep_mha2nnunet], or set your target paths in [`prepare_data.py`](src/picai_baseline/prepare_data.py) and execute it:
+Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
 
 ```bash
-python src/picai_baseline/prepare_data.py
+python src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
-To adapt/modify the preprocessing pipeline or its default specifications, please make changes to the [`prepare_data.py`](src/picai_baseline/prepare_data.py) script accordingly.
+For the baseline semi-supervised U-Net algorithm, specify the dataset-wise resolution: `--spacing 3.0 0.5 0.5`.
+To adapt/modify the preprocessing pipeline or its default specifications, either check out the various command like options (use flag `-h` to show these) or make changes to the [`prepare_data_semi_supervised.py`](src/picai_baseline/prepare_data_semi_supervised.py) script.
 
 Alternatively, you can use Docker to run the Python script:
 
 ```bash
 docker run --cpus=2 --memory=16gb --rm \
     -v /path/to/input/:/input/ \
     -v /path/to/workdir/:/workdir/ \
     -v /path/to/picai_baseline:/scripts/picai_baseline/ \
-    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data.py
+    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
+If you don't want to include the AI-generated annotations, you can also use the supervised data preparation script: [`prepare_data.py`](src/picai_baseline/prepare_data.py).
+
 
 ## Baseline Algorithms
 We provide end-to-end training pipelines for csPCa detection/diagnosis in 3D. Each baseline includes a template to encapsulate the trained AI model in a Docker container, and uploading the same to the [grand-challenge.org](https://grand-challenge.org/) platform as an ["algorithm"](https://grand-challenge.org/documentation/algorithms/). 
 
 
 ### U-Net
 We include a baseline [U-Net](https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28) to provide a playground environment for participants and kickstart their development cycle. The U-Net baseline generates quick results with minimal complexity, but does so at the expense of sub-optimal performance and low flexibility in adapting to any other task.
@@ -205,21 +183,33 @@
 
 
 ##
 If you are using this codebase or some part of it, please cite the following article:
 
 ● [A. Saha, J. J. Twilt, J. S. Bosma, B. van Ginneken, D. Yakar, M. Elschot, J. Veltman, J. J. Fütterer, M. de Rooij, H. Huisman, "Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)", DOI: 10.5281/zenodo.6667655](https://zenodo.org/record/6667655)
 
+If you are using the AI-generated annotations (i.e., semi-supervised learning), please cite the following article:
+● [J. S. Bosma, A. Saha, M. Hosseinzadeh, I. Slootweg, M. de Rooij, and H. Huisman, "Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI", Radiology: Artificial Intelligence, 230031, 2023. doi:10.1148/ryai.230031](https://doi.org/10.1148/ryai.230031)
+
 **BibTeX:**
 ```
-@ARTICLE{PICAI_BIAS,
-    author = {Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
-    title  = {{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}}, 
-    year   = {2022},
-    doi    = {10.5281/zenodo.6667655}
+@article{PICAI_BIAS,
+    author={Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
+    title={{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}},
+    year={2022},
+    doi={10.5281/zenodo.6667655}
+}
+@article{Bosma23,
+    author={Joeran S. Bosma, Anindo Saha, Matin Hosseinzadeh, Ivan Slootweg, Maarten de Rooij, and Henkjan Huisman},
+    title={Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI},
+    journal={Radiology: Artificial Intelligence},
+    pages={e230031},
+    year={2023},
+    doi={10.1148/ryai.230031},
+    publisher={Radiological Society of North America}
 }
 ```
 
 [picai_nnunet_docker]: https://hub.docker.com/r/joeranbosma/picai_nnunet
 [picai_nndetection_docker]: https://hub.docker.com/r/joeranbosma/picai_nndetection
 [picai_prep]: https://github.com/DIAGNijmegen/picai_prep
 [nnunet_raw_data_format]: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/dataset_conversion.md
```

### Comparing `picai_baseline-0.8.4/README.md` & `picai_baseline-0.8.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,47 @@
+Metadata-Version: 2.1
+Name: picai_baseline
+Version: 0.8.5
+Summary: PICAI Baselines
+Home-page: https://github.com/DIAGNijmegen/picai_baseline
+Author: Joeran Bosma
+Author-email: Joeran.Bosma@radboudumc.nl
+License: Apache 2.0
+Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_baseline/issues
+Platform: unix
+Platform: linux
+Platform: osx
+Platform: cygwin
+Platform: win32
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: SimpleITK
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: picai_eval>=1.4.1
+Requires-Dist: picai_prep>=2.0.1
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
+Requires-Dist: tox>=3.24; extra == "testing"
+
 # Baseline AI Models for Prostate Cancer Detection in MRI
 
-This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models will be provided and supported:
+This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models are provided and supported:
 
 - [U-Net](unet_baseline.md)
 - [nnU-Net](nnunet_baseline.md)
 - [nnDetection](nndetection_baseline.md)
 
 All three solutions share the same starting point, with respect to their expected [folder structure](#folder-structure) and [data preparation](#data-preparation) pipeline.
 
@@ -23,24 +60,24 @@
 
 ```bash
 git clone https://github.com/DIAGNijmegen/picai_baseline
 cd picai_baseline
 pip install -e .
 ```
 
-This ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option. Furthermore, this ensures the latest version is installed.
+Installing from source ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option.
 
 
 ## General Setup
-We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
+We define setup steps that are shared between the different baseline algorithms. To follow the model-specific baseline algorithm tutorials, these steps must be completed first.
 
 
 ### Folder Structure
-We define three main folders that must be prepared apriori:
-- `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
+We define three main folders that must be prepared:
+- `/input/` contains the [PI-CAI dataset](https://pi-cai.grand-challenge.org/DATA/). In this tutorial we assume this is the PI-CAI Public Training and Development Dataset.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
   - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
@@ -118,34 +155,37 @@
 
 ```bash
 python -m picai_baseline.splits.picai_nnunet --output "/workdir/splits/picai_nnunet"
 ```
 
 
 ### Data Preprocessing
-We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
+We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. The [`picai_prep`][picai_prep] module allows to resample all cases to the same resolution (you can resample each case indivudually to the same resolution between the different sequences, or choose to resample the full dataset to the same resolution). For details on the available options to convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please see the instructions [provided here][picai_prep_mha2nnunet]. Below we give the conversion as performed for the [baseline semi-supervised nnU-Net](https://grand-challenge.org/algorithms/pi-cai-pubpriv-nnu-net-semi-supervised/). For the U-Net baseline, please see the [U-Net tutorial](src/picai_baseline/unet_baseline.md#u-net---data-preparation) for extra instructions.
 
-To convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please follow the instructions [provided here][picai_prep_mha2nnunet], or set your target paths in [`prepare_data.py`](src/picai_baseline/prepare_data.py) and execute it:
+Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
 
 ```bash
-python src/picai_baseline/prepare_data.py
+python src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
-To adapt/modify the preprocessing pipeline or its default specifications, please make changes to the [`prepare_data.py`](src/picai_baseline/prepare_data.py) script accordingly.
+For the baseline semi-supervised U-Net algorithm, specify the dataset-wise resolution: `--spacing 3.0 0.5 0.5`.
+To adapt/modify the preprocessing pipeline or its default specifications, either check out the various command like options (use flag `-h` to show these) or make changes to the [`prepare_data_semi_supervised.py`](src/picai_baseline/prepare_data_semi_supervised.py) script.
 
 Alternatively, you can use Docker to run the Python script:
 
 ```bash
 docker run --cpus=2 --memory=16gb --rm \
     -v /path/to/input/:/input/ \
     -v /path/to/workdir/:/workdir/ \
     -v /path/to/picai_baseline:/scripts/picai_baseline/ \
-    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data.py
+    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
+If you don't want to include the AI-generated annotations, you can also use the supervised data preparation script: [`prepare_data.py`](src/picai_baseline/prepare_data.py).
+
 
 ## Baseline Algorithms
 We provide end-to-end training pipelines for csPCa detection/diagnosis in 3D. Each baseline includes a template to encapsulate the trained AI model in a Docker container, and uploading the same to the [grand-challenge.org](https://grand-challenge.org/) platform as an ["algorithm"](https://grand-challenge.org/documentation/algorithms/). 
 
 
 ### U-Net
 We include a baseline [U-Net](https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28) to provide a playground environment for participants and kickstart their development cycle. The U-Net baseline generates quick results with minimal complexity, but does so at the expense of sub-optimal performance and low flexibility in adapting to any other task.
@@ -180,21 +220,33 @@
 
 
 ##
 If you are using this codebase or some part of it, please cite the following article:
 
 ● [A. Saha, J. J. Twilt, J. S. Bosma, B. van Ginneken, D. Yakar, M. Elschot, J. Veltman, J. J. Fütterer, M. de Rooij, H. Huisman, "Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)", DOI: 10.5281/zenodo.6667655](https://zenodo.org/record/6667655)
 
+If you are using the AI-generated annotations (i.e., semi-supervised learning), please cite the following article:
+● [J. S. Bosma, A. Saha, M. Hosseinzadeh, I. Slootweg, M. de Rooij, and H. Huisman, "Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI", Radiology: Artificial Intelligence, 230031, 2023. doi:10.1148/ryai.230031](https://doi.org/10.1148/ryai.230031)
+
 **BibTeX:**
 ```
-@ARTICLE{PICAI_BIAS,
-    author = {Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
-    title  = {{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}}, 
-    year   = {2022},
-    doi    = {10.5281/zenodo.6667655}
+@article{PICAI_BIAS,
+    author={Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
+    title={{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}},
+    year={2022},
+    doi={10.5281/zenodo.6667655}
+}
+@article{Bosma23,
+    author={Joeran S. Bosma, Anindo Saha, Matin Hosseinzadeh, Ivan Slootweg, Maarten de Rooij, and Henkjan Huisman},
+    title={Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI},
+    journal={Radiology: Artificial Intelligence},
+    pages={e230031},
+    year={2023},
+    doi={10.1148/ryai.230031},
+    publisher={Radiological Society of North America}
 }
 ```
 
 [picai_nnunet_docker]: https://hub.docker.com/r/joeranbosma/picai_nnunet
 [picai_nndetection_docker]: https://hub.docker.com/r/joeranbosma/picai_nndetection
 [picai_prep]: https://github.com/DIAGNijmegen/picai_prep
 [nnunet_raw_data_format]: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/dataset_conversion.md
```

### Comparing `picai_baseline-0.8.4/setup.cfg` & `picai_baseline-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/setup.py` & `picai_baseline-0.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 if __name__ == '__main__':
     with open("README.md", "r", encoding="utf-8") as fh:
         long_description = fh.read()
 
     setuptools.setup(
-        version='0.8.4',
+        version='0.8.5',
         author_email='Joeran.Bosma@radboudumc.nl',
         long_description=long_description,
         long_description_content_type="text/markdown",
         url='https://github.com/DIAGNijmegen/picai_baseline',
         project_urls={
             "Bug Tracker": "https://github.com/DIAGNijmegen/picai_baseline/issues"
         },
```

### Comparing `picai_baseline-0.8.4/src/picai_baseline/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/__main__.py` & `picai_baseline-0.8.5/src/picai_baseline/__main__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/eval.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/eval.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/nnunet_baseline.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/nnunet_baseline.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/softmax_export.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/softmax_export.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/focal_loss.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/focal_loss.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/io.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/io.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_CE_checkpoints.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_Loss_FL_and_CE.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnUNetTrainerV2_focalLoss.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/nnunet_wrapper.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/nnunet/training_docker/run_training.py` & `picai_baseline-0.8.5/src/picai_baseline/nnunet/training_docker/run_training.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/prepare_data.py` & `picai_baseline-0.8.5/src/picai_baseline/prepare_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,14 +150,15 @@
         # prepare dataset in nnUNet format
         archive = MHA2nnUNetConverter(
             output_dir=nnUNet_raw_data_path,
             scans_dir=imagesdir,
             annotations_dir=annotations_dir,
             mha2nnunet_settings=mha2nnunet_settings,
         )
+        # TODO: check logging of errors
         archive.convert()
         archive.create_dataset_json()
 
     if nnUNet_splits_path.exists():
         print(f"Found cross-validation splits at {nnUNet_splits_path}, skipping..")
     else:
         # save cross-validation splits to disk
```

### Comparing `picai_baseline-0.8.4/src/picai_baseline/prepare_data_semi_supervised.py` & `picai_baseline-0.8.5/src/picai_baseline/prepare_data_semi_supervised.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-0.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-1.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-2.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-3.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-train-fold-4.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-train-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/ds-config-valid-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai/splits.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_debug/splits.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_debug/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_nnunet/splits.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_nnunet/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-train-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-0.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-1.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-2.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-3.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/ds-config-valid-fold-4.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv/splits.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json` & `picai_baseline-0.8.5/src/picai_baseline/splits/picai_pubpriv_nnunet/splits.json`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/plan_overview.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/plan_overview.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/train.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/train.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/multi_threaded_augmenter.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/nnUNet_DA.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/single_threaded_augmenter.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/augmentations/test_time_augmentations.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/callbacks.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import os
 import time
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import torch
+import torch.nn.functional as F
 from picai_eval import Metrics
 from picai_eval.eval import evaluate_case
 from report_guided_annotation import extract_lesion_candidates
 from scipy.ndimage import gaussian_filter
 
 from picai_baseline.unet.training_setup.poly_lr import poly_lr
 
@@ -111,14 +112,23 @@
         step += 1
         try:
             inputs = batch_data['data'].to(device)
             labels = batch_data['seg'].to(device)
         except Exception:
             inputs = torch.from_numpy(batch_data['data']).to(device)
             labels = torch.from_numpy(batch_data['seg']).to(device)
+
+        # bugfix for shape of targets
+        if labels.shape[1] == 1:
+            # labels now has shape (B, 1, D, H, W)
+            labels = labels[:, 0, ...]  # shape: (B, D, H, W)
+            labels = F.one_hot(labels.long(), num_classes=args.num_classes).float()  # shape: (B, D, H, W, C)
+            # reshape to (B, C, D, H, W)
+            labels = labels.permute(0, 4, 1, 2, 3).contiguous()
+
         outputs = model(inputs)
         loss = loss_func(outputs, labels)
         train_loss += loss.item()
 
         # backpropagate + optimize
         optimizer.zero_grad()
         loss.backward()
```

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/compute_spec.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/compute_spec.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/data_generator.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/data_generator.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/default_hyperparam.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/default_hyperparam.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/image_reader.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/image_reader.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/loss_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/loss_functions/focal.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/loss_functions/focal.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,16 +25,14 @@
         self.alpha = alpha
         self.gamma = gamma
         self.num_classes = num_classes
         self.reduction = reduction
 
     def forward(self, inputs, targets):
         inputs = torch.sigmoid(inputs)
-        targets = F.one_hot(targets, num_classes=self.num_classes).float()
-        targets = torch.moveaxis(targets, (0, 1, 2, 3, 4), (0, 2, 3, 4, 1))
         ce_loss = F.binary_cross_entropy(inputs, targets, reduction="none")
         p_t = (inputs * targets) + ((1 - inputs) * (1 - targets))
         loss = ce_loss * ((1 - p_t) ** self.gamma)
 
         if self.alpha >= 0:
             alpha_t = self.alpha * targets + (1 - self.alpha) * (1 - targets)
             loss = alpha_t * loss
```

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_network_selector.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_network_selector.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/__init__.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/neural_networks/unets.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/neural_networks/unets.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/poly_lr.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/poly_lr.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline/unet/training_setup/preprocess_utils.py` & `picai_baseline-0.8.5/src/picai_baseline/unet/training_setup/preprocess_utils.py`

 * *Files identical despite different names*

### Comparing `picai_baseline-0.8.4/src/picai_baseline.egg-info/PKG-INFO` & `picai_baseline-0.8.5/src/picai_baseline.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: picai-baseline
-Version: 0.8.4
+Name: picai_baseline
+Version: 0.8.5
 Summary: PICAI Baselines
 Home-page: https://github.com/DIAGNijmegen/picai_baseline
 Author: Joeran Bosma
 Author-email: Joeran.Bosma@radboudumc.nl
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/DIAGNijmegen/picai_baseline/issues
 Platform: unix
@@ -16,20 +16,32 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: testing
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: tqdm
+Requires-Dist: SimpleITK
+Requires-Dist: scipy
+Requires-Dist: scikit-learn
+Requires-Dist: picai_eval>=1.4.1
+Requires-Dist: picai_prep>=2.0.1
+Provides-Extra: testing
+Requires-Dist: pytest>=6.0; extra == "testing"
+Requires-Dist: pytest-cov>=2.0; extra == "testing"
+Requires-Dist: mypy>=0.910; extra == "testing"
+Requires-Dist: flake8>=3.9; extra == "testing"
+Requires-Dist: tox>=3.24; extra == "testing"
 
 # Baseline AI Models for Prostate Cancer Detection in MRI
 
-This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models will be provided and supported:
+This repository contains utilities to set up and train deep learning-based detection models for clinically significant prostate cancer (csPCa) in MRI. In turn, these models serve as the official baseline AI solutions for the [PI-CAI challenge](https://pi-cai.grand-challenge.org/). As of now, the following three models are provided and supported:
 
 - [U-Net](unet_baseline.md)
 - [nnU-Net](nnunet_baseline.md)
 - [nnDetection](nndetection_baseline.md)
 
 All three solutions share the same starting point, with respect to their expected [folder structure](#folder-structure) and [data preparation](#data-preparation) pipeline.
 
@@ -48,24 +60,24 @@
 
 ```bash
 git clone https://github.com/DIAGNijmegen/picai_baseline
 cd picai_baseline
 pip install -e .
 ```
 
-This ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option. Furthermore, this ensures the latest version is installed.
+Installing from source ensures the scripts are present locally, which enables you to run the provided Python scripts. Additionally, this allows you to modify the baseline solutions, due to the `-e` option.
 
 
 ## General Setup
-We define setup steps that are shared between the different baseline algorithms. To follow the baseline algorithm tutorials, this setup must be completed first.
+We define setup steps that are shared between the different baseline algorithms. To follow the model-specific baseline algorithm tutorials, these steps must be completed first.
 
 
 ### Folder Structure
-We define three main folders that must be prepared apriori:
-- `/input/` contains one of the [PI-CAI datasets](https://pi-cai.grand-challenge.org/DATA/). This can be the Public Training and Development Dataset, the Private Training Dataset, the Hidden Validation and Tuning Cohort, or the Hidden Testing Cohort.
+We define three main folders that must be prepared:
+- `/input/` contains the [PI-CAI dataset](https://pi-cai.grand-challenge.org/DATA/). In this tutorial we assume this is the PI-CAI Public Training and Development Dataset.
   - `/input/images/` contains the imaging files. For the Public Training and Development Dataset, these can be retrieved [here](https://zenodo.org/record/6624726).
   - `/input/picai_labels/` contains the annotations. For the Public Training and Development Dataset, these can be retrieved [here](https://github.com/DIAGNijmegen/picai_labels).
 - `/workdir/` stores intermediate results, such as preprocessed images and annotations.
   - `/workdir/results/[model name]/` stores model checkpoints/weights during training (enables the ability to pause/resume training).    
 - `/output/` stores training output, such as trained model weights and preprocessing plan.
 
 
@@ -143,34 +155,37 @@
 
 ```bash
 python -m picai_baseline.splits.picai_nnunet --output "/workdir/splits/picai_nnunet"
 ```
 
 
 ### Data Preprocessing
-We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
+We follow the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format to prepare our dataset for usage. For this, you can use the [`picai_prep`][picai_prep] module. The [`picai_prep`][picai_prep] module allows to resample all cases to the same resolution (you can resample each case indivudually to the same resolution between the different sequences, or choose to resample the full dataset to the same resolution). For details on the available options to convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please see the instructions [provided here][picai_prep_mha2nnunet]. Below we give the conversion as performed for the [baseline semi-supervised nnU-Net](https://grand-challenge.org/algorithms/pi-cai-pubpriv-nnu-net-semi-supervised/). For the U-Net baseline, please see the [U-Net tutorial](src/picai_baseline/unet_baseline.md#u-net---data-preparation) for extra instructions.
 
-To convert the dataset in `/input/` into the [`nnU-Net Raw Data Archive`][nnunet_raw_data_format] format, and store it in `/workdir/nnUNet_raw_data`, please follow the instructions [provided here][picai_prep_mha2nnunet], or set your target paths in [`prepare_data.py`](src/picai_baseline/prepare_data.py) and execute it:
+Note, the [`picai_prep`][picai_prep] module should be automatically installed when installing the `picai_baseline` module, and is installed within the [`picai_nnunet`][picai_nnunet_docker] and [`picai_nndetection`][picai_nndetection_docker] Docker containers as well. 
 
 ```bash
-python src/picai_baseline/prepare_data.py
+python src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
-To adapt/modify the preprocessing pipeline or its default specifications, please make changes to the [`prepare_data.py`](src/picai_baseline/prepare_data.py) script accordingly.
+For the baseline semi-supervised U-Net algorithm, specify the dataset-wise resolution: `--spacing 3.0 0.5 0.5`.
+To adapt/modify the preprocessing pipeline or its default specifications, either check out the various command like options (use flag `-h` to show these) or make changes to the [`prepare_data_semi_supervised.py`](src/picai_baseline/prepare_data_semi_supervised.py) script.
 
 Alternatively, you can use Docker to run the Python script:
 
 ```bash
 docker run --cpus=2 --memory=16gb --rm \
     -v /path/to/input/:/input/ \
     -v /path/to/workdir/:/workdir/ \
     -v /path/to/picai_baseline:/scripts/picai_baseline/ \
-    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data.py
+    joeranbosma/picai_nnunet:latest python3 /scripts/picai_baseline/src/picai_baseline/prepare_data_semi_supervised.py
 ```
 
+If you don't want to include the AI-generated annotations, you can also use the supervised data preparation script: [`prepare_data.py`](src/picai_baseline/prepare_data.py).
+
 
 ## Baseline Algorithms
 We provide end-to-end training pipelines for csPCa detection/diagnosis in 3D. Each baseline includes a template to encapsulate the trained AI model in a Docker container, and uploading the same to the [grand-challenge.org](https://grand-challenge.org/) platform as an ["algorithm"](https://grand-challenge.org/documentation/algorithms/). 
 
 
 ### U-Net
 We include a baseline [U-Net](https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28) to provide a playground environment for participants and kickstart their development cycle. The U-Net baseline generates quick results with minimal complexity, but does so at the expense of sub-optimal performance and low flexibility in adapting to any other task.
@@ -205,21 +220,33 @@
 
 
 ##
 If you are using this codebase or some part of it, please cite the following article:
 
 ● [A. Saha, J. J. Twilt, J. S. Bosma, B. van Ginneken, D. Yakar, M. Elschot, J. Veltman, J. J. Fütterer, M. de Rooij, H. Huisman, "Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)", DOI: 10.5281/zenodo.6667655](https://zenodo.org/record/6667655)
 
+If you are using the AI-generated annotations (i.e., semi-supervised learning), please cite the following article:
+● [J. S. Bosma, A. Saha, M. Hosseinzadeh, I. Slootweg, M. de Rooij, and H. Huisman, "Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI", Radiology: Artificial Intelligence, 230031, 2023. doi:10.1148/ryai.230031](https://doi.org/10.1148/ryai.230031)
+
 **BibTeX:**
 ```
-@ARTICLE{PICAI_BIAS,
-    author = {Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
-    title  = {{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}}, 
-    year   = {2022},
-    doi    = {10.5281/zenodo.6667655}
+@article{PICAI_BIAS,
+    author={Anindo Saha, Jasper J. Twilt, Joeran S. Bosma, Bram van Ginneken, Derya Yakar, Mattijs Elschot, Jeroen Veltman, Jurgen Fütterer, Maarten de Rooij, Henkjan Huisman},
+    title={{Artificial Intelligence and Radiologists at Prostate Cancer Detection in MRI: The PI-CAI Challenge (Study Protocol)}},
+    year={2022},
+    doi={10.5281/zenodo.6667655}
+}
+@article{Bosma23,
+    author={Joeran S. Bosma, Anindo Saha, Matin Hosseinzadeh, Ivan Slootweg, Maarten de Rooij, and Henkjan Huisman},
+    title={Semisupervised Learning with Report-guided Pseudo Labels for Deep Learning–based Prostate Cancer Detection Using Biparametric MRI},
+    journal={Radiology: Artificial Intelligence},
+    pages={e230031},
+    year={2023},
+    doi={10.1148/ryai.230031},
+    publisher={Radiological Society of North America}
 }
 ```
 
 [picai_nnunet_docker]: https://hub.docker.com/r/joeranbosma/picai_nnunet
 [picai_nndetection_docker]: https://hub.docker.com/r/joeranbosma/picai_nndetection
 [picai_prep]: https://github.com/DIAGNijmegen/picai_prep
 [nnunet_raw_data_format]: https://github.com/MIC-DKFZ/nnUNet/blob/master/documentation/dataset_conversion.md
```

### Comparing `picai_baseline-0.8.4/src/picai_baseline.egg-info/SOURCES.txt` & `picai_baseline-0.8.5/src/picai_baseline.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 src/picai_baseline/__init__.py
 src/picai_baseline/__main__.py
 src/picai_baseline/prepare_data.py
 src/picai_baseline/prepare_data_semi_supervised.py
+src/picai_baseline/py.typed
 src/picai_baseline.egg-info/PKG-INFO
 src/picai_baseline.egg-info/SOURCES.txt
 src/picai_baseline.egg-info/dependency_links.txt
 src/picai_baseline.egg-info/not-zip-safe
 src/picai_baseline.egg-info/requires.txt
 src/picai_baseline.egg-info/top_level.txt
 src/picai_baseline/nnunet/__init__.py
```

### Comparing `picai_baseline-0.8.4/tests/test_splits.py` & `picai_baseline-0.8.5/tests/test_splits.py`

 * *Files identical despite different names*

