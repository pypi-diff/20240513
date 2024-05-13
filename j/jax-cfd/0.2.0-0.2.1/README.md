# Comparing `tmp/jax-cfd-0.2.0.tar.gz` & `tmp/jax_cfd-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jax-cfd-0.2.0.tar", last modified: Tue Jul 19 17:28:58 2022, max compression
+gzip compressed data, was "jax_cfd-0.2.1.tar", last modified: Mon May 13 15:47:11 2024, max compression
```

## Comparing `jax-cfd-0.2.0.tar` & `jax_cfd-0.2.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.246874 jax-cfd-0.2.0/
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/LICENSE
--rw-r--r--   0 shoyer   (365133) eng       (5000)      343 2022-07-19 17:28:58.246735 jax-cfd-0.2.0/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6261 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/README.md
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.234497 jax-cfd-0.2.0/jax_cfd/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      687 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/jax_cfd/__init__.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.240379 jax-cfd-0.2.0/jax_cfd/base/
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1188 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    13534 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/advection.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11537 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/advection_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8119 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/array_utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5902 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/array_utils_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    12379 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/boundaries.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    26736 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/boundaries_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4157 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/diffusion.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2215 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/diffusion_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6746 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/equations.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8404 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/equations_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    10647 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/fast_diagonalization.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4889 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/jax_cfd/base/fast_diagonalization_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1559 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/filter_utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7323 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/finite_differences.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    13355 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/jax_cfd/base/finite_differences_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7467 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/forcings.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5577 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/forcings_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4144 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/funcutils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1801 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/jax_cfd/base/funcutils_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    22869 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/grids.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    27120 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/grids_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5938 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/initial_conditions.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5541 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/initial_conditions_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    13846 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/interpolation.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    14299 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/interpolation_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5008 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/pressure.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6300 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/pressure_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4764 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/resize.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6872 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/resize_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     9683 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/subgrid_models.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7876 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/jax_cfd/base/subgrid_models_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3191 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/test_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4109 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/time_stepping.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2648 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/jax_cfd/base/time_stepping_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3288 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/validation_problems.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6860 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/base/validation_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.241660 jax-cfd-0.2.0/jax_cfd/collocated/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2427 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/advection.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2245 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/advection_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1356 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/diffusion.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1450 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/diffusion_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3037 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/equations.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5111 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/equations_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3775 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/initial_conditions.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1977 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/initial_conditions_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3368 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/pressure.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2591 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/collocated/pressure_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.242316 jax-cfd-0.2.0/jax_cfd/data/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      740 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/jax_cfd/data/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    13233 2021-05-17 19:23:46.000000 jax-cfd-0.2.0/jax_cfd/data/evaluation.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4950 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/jax_cfd/data/visualization.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2546 2021-05-18 17:23:39.000000 jax-cfd-0.2.0/jax_cfd/data/visualization_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    14868 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/data/xarray_utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2721 2021-04-16 19:52:03.000000 jax-cfd-0.2.0/jax_cfd/data/xarray_utils_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.245446 jax-cfd-0.2.0/jax_cfd/ml/
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1246 2021-05-18 17:23:39.000000 jax-cfd-0.2.0/jax_cfd/ml/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2798 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/advections.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5480 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/decoders.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2874 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/diffusions.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8753 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/encoders.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     9351 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/equations.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11830 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/equations_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3550 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/forcings.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8597 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/interpolations.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    24951 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/layers.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    20039 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/jax_cfd/ml/layers_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    15790 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/layers_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    12918 2021-05-17 19:23:46.000000 jax-cfd-0.2.0/jax_cfd/ml/layers_util_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5667 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/metrics.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4829 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/model_builder.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3033 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/model_utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6592 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/networks.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      400 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/nonlinearities.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      518 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/optimizer_modules.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1301 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/physics_specifications.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      905 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/pressures.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5464 2021-05-17 19:23:46.000000 jax-cfd-0.2.0/jax_cfd/ml/tiling.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      967 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/time_integrators.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    10752 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/towers.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2736 2021-05-17 19:23:46.000000 jax-cfd-0.2.0/jax_cfd/ml/towers_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8036 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/train_utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     9708 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/ml/viscosities.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.246541 jax-cfd-0.2.0/jax_cfd/spectral/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      745 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7696 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/equations.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11933 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/equations_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1572 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/forcings.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     8747 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/time_stepping.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     7069 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/time_stepping_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)      798 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/types.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5631 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/utils.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3063 2022-07-19 17:23:51.000000 jax-cfd-0.2.0/jax_cfd/spectral/utils_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2022-07-19 17:28:58.235075 jax-cfd-0.2.0/jax_cfd.egg-info/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      343 2022-07-19 17:28:57.000000 jax-cfd-0.2.0/jax_cfd.egg-info/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2883 2022-07-19 17:28:58.000000 jax-cfd-0.2.0/jax_cfd.egg-info/SOURCES.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2022-07-19 17:28:57.000000 jax-cfd-0.2.0/jax_cfd.egg-info/dependency_links.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)      263 2022-07-19 17:28:58.000000 jax-cfd-0.2.0/jax_cfd.egg-info/requires.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        8 2022-07-19 17:28:58.000000 jax-cfd-0.2.0/jax_cfd.egg-info/top_level.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2022-07-19 17:28:58.246919 jax-cfd-0.2.0/setup.cfg
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1421 2022-07-19 17:27:22.000000 jax-cfd-0.2.0/setup.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.234015 jax_cfd-0.2.1/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-04-16 19:52:03.000000 jax_cfd-0.2.1/LICENSE
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1332 2024-05-13 15:47:11.233768 jax_cfd-0.2.1/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6274 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/README.md
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.213281 jax_cfd-0.2.1/jax_cfd/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      687 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/__init__.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.222416 jax_cfd-0.2.1/jax_cfd/base/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1188 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    16448 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/advection.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    16299 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/advection_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    17146 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/base/array_utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    13829 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/array_utils_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    29949 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/boundaries.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    50366 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/boundaries_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7551 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/diffusion.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4430 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/diffusion_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6794 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/equations.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8404 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/equations_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    10641 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/fast_diagonalization.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4889 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/fast_diagonalization_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1559 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/filter_utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7595 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/finite_differences.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    13355 2022-07-19 17:27:22.000000 jax_cfd-0.2.1/jax_cfd/base/finite_differences_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7467 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/forcings.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5577 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/forcings_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4144 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/funcutils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1801 2021-04-16 19:52:03.000000 jax_cfd-0.2.1/jax_cfd/base/funcutils_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    24054 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/grids.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    27124 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/grids_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6213 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/initial_conditions.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5552 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/initial_conditions_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    13834 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/interpolation.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    14299 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/interpolation_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6511 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/pressure.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7936 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/pressure_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     9351 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/resize.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    15526 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/resize_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     9675 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/base/subgrid_models.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7876 2022-07-19 17:27:22.000000 jax_cfd-0.2.1/jax_cfd/base/subgrid_models_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3183 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/base/test_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4109 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/time_stepping.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2641 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/base/time_stepping_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3288 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/validation_problems.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6860 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/base/validation_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.224149 jax_cfd-0.2.1/jax_cfd/collocated/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      836 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2629 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/collocated/advection.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4403 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/collocated/advection_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1356 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/diffusion.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1450 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/diffusion_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3037 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/equations.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5111 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/collocated/equations_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3780 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/collocated/initial_conditions.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1988 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/collocated/initial_conditions_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3368 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/pressure.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2591 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/collocated/pressure_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.225246 jax_cfd-0.2.1/jax_cfd/data/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      740 2021-04-16 19:52:03.000000 jax_cfd-0.2.1/jax_cfd/data/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    13233 2021-05-17 19:23:46.000000 jax_cfd-0.2.1/jax_cfd/data/evaluation.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4992 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/data/visualization.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2546 2021-05-18 17:23:39.000000 jax_cfd-0.2.1/jax_cfd/data/visualization_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    15332 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/data/xarray_utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2780 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/data/xarray_utils_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.230067 jax_cfd-0.2.1/jax_cfd/ml/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1246 2021-05-18 17:23:39.000000 jax_cfd-0.2.1/jax_cfd/ml/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2798 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/advections.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5480 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/decoders.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2874 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/diffusions.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8939 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/encoders.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     9351 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/equations.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11960 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/ml/equations_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3550 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/forcings.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8597 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/interpolations.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    27978 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/layers.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    20039 2022-07-19 17:27:22.000000 jax_cfd-0.2.1/jax_cfd/ml/layers_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    15853 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/layers_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    12918 2021-05-17 19:23:46.000000 jax_cfd-0.2.1/jax_cfd/ml/layers_util_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5667 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/metrics.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4829 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/model_builder.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3033 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/model_utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8726 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/networks.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      400 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/nonlinearities.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      518 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/optimizer_modules.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1301 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/physics_specifications.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      905 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/pressures.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5464 2021-05-17 19:23:46.000000 jax_cfd-0.2.1/jax_cfd/ml/tiling.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      967 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/time_integrators.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11396 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/towers.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2736 2021-05-17 19:23:46.000000 jax_cfd-0.2.1/jax_cfd/ml/towers_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8036 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/ml/train_utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     9873 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/ml/viscosities.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.232017 jax_cfd-0.2.1/jax_cfd/spectral/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      745 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/spectral/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     9013 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/spectral/equations.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    13756 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/spectral/equations_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1572 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/spectral/forcings.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     8747 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/spectral/time_stepping.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     7062 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/spectral/time_stepping_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      779 2023-08-09 20:43:37.000000 jax_cfd-0.2.1/jax_cfd/spectral/types.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6804 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/jax_cfd/spectral/utils.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3063 2022-07-19 17:23:51.000000 jax_cfd-0.2.1/jax_cfd/spectral/utils_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2024-05-13 15:47:11.232315 jax_cfd-0.2.1/jax_cfd.egg-info/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1332 2024-05-13 15:47:11.000000 jax_cfd-0.2.1/jax_cfd.egg-info/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2883 2024-05-13 15:47:11.000000 jax_cfd-0.2.1/jax_cfd.egg-info/SOURCES.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2024-05-13 15:47:11.000000 jax_cfd-0.2.1/jax_cfd.egg-info/dependency_links.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      263 2024-05-13 15:47:11.000000 jax_cfd-0.2.1/jax_cfd.egg-info/requires.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        8 2024-05-13 15:47:11.000000 jax_cfd-0.2.1/jax_cfd.egg-info/top_level.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2024-05-13 15:47:11.234068 jax_cfd-0.2.1/setup.cfg
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1421 2024-05-13 15:42:16.000000 jax_cfd-0.2.1/setup.py
```

### Comparing `jax-cfd-0.2.0/LICENSE` & `jax_cfd-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/README.md` & `jax_cfd-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # JAX-CFD: Computational Fluid Dynamics in JAX
 
-Authors: Dmitrii Kochkov, Jamie A. Smith, Peter Norgaard, Gideon Dresdner, Stephan Hoyer
+Authors: Dmitrii Kochkov, Jamie A. Smith, Peter Norgaard, Gideon Dresdner, Ayya Alieva, Stephan Hoyer
 
 JAX-CFD is an experimental research project for exploring the potential of
 machine learning, automatic differentiation and hardware accelerators (GPU/TPU)
 for computational fluid dynamics. It is implemented in
 [JAX](https://github.com/google/jax).
 
 To learn more about our general approach, read our paper [Machine learning accelerated computational fluid dynamics](https://www.pnas.org/content/118/21/e2101784118)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/__init__.py` & `jax_cfd-0.2.1/jax_cfd/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Defines the JAX-CFD module for computational fluid dynamics."""
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 import jax_cfd.base
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/__init__.py` & `jax_cfd-0.2.1/jax_cfd/base/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/advection.py` & `jax_cfd-0.2.1/jax_cfd/base/advection.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module for functionality related to advection."""
 
 from typing import Optional, Tuple
+
 import jax
 import jax.numpy as jnp
 from jax_cfd.base import boundaries
 from jax_cfd.base import finite_differences as fd
 from jax_cfd.base import grids
 from jax_cfd.base import interpolation
 
@@ -66,16 +67,18 @@
   """
   # TODO(jamieas): add more sophisticated alignment checks, ensuring that the
   # values are located on the faces of a control volume.
   if len(cs) != len(v):
     raise ValueError('`cs` and `v` must have the same length;'
                      f'got {len(cs)} vs. {len(v)}.')
   flux = tuple(c.array * u.array for c, u in zip(cs, v))
-  # Flux inherits boundary conditions from cs
-  flux = tuple(grids.GridVariable(f, c.bc) for f, c in zip(flux, cs))
+  bcs = tuple(
+      boundaries.get_advection_flux_bc_from_velocity_and_scalar(v[i], cs[i], i)
+      for i in range(len(v)))
+  flux = tuple(bc.impose_bc(f) for f, bc in zip(flux, bcs))
   return -fd.divergence(flux)
 
 
 def advect_general(
     c: GridVariable,
     v: GridVariableVector,
     u_interpolation_fn: InterpolationFn,
@@ -98,14 +101,17 @@
     u_interpolation_fn: method for interpolating velocity field `v`.
     c_interpolation_fn: method for interpolating scalar field `c`.
     dt: unused time-step.
 
   Returns:
     The time derivative of `c` due to advection by `v`.
   """
+  if not boundaries.has_all_periodic_boundary_conditions(c):
+    raise NotImplementedError(
+        'Non-periodic boundary conditions are not implemented.')
   target_offsets = grids.control_volume_offsets(c)
   aligned_v = tuple(u_interpolation_fn(u, target_offset, v, dt)
                     for u, target_offset in zip(v, target_offsets))
   aligned_c = tuple(c_interpolation_fn(c, target_offset, aligned_v, dt)
                     for target_offset in target_offsets)
   return _advect_aligned(aligned_c, aligned_v)
 
@@ -162,18 +168,18 @@
     `aligned_v`. The entry `flux[i][j]` is `aligned_v[i][j] * aligned_v[j][i]`.
   """
   ndim = len(aligned_v)
   flux = [tuple() for _ in range(ndim)]
   for i in range(ndim):
     for j in range(ndim):
       if i <= j:
-        bc = grids.consistent_boundary_conditions(
-            aligned_v[i][j], aligned_v[j][i])
-        flux[i] += (GridVariable(aligned_v[i][j].array * aligned_v[j][i].array,
-                                 bc),)
+        bc = boundaries.get_advection_flux_bc_from_velocity_and_scalar(
+            aligned_v[j][i], aligned_v[i][j], j)
+        flux[i] += (bc.impose_bc(aligned_v[i][j].array *
+                                 aligned_v[j][i].array),)
       else:
         flux[i] += (flux[j][i],)
   return tuple(flux)
 
 
 def convect_linear(v: GridVariableVector) -> GridArrayVector:
   """Computes convection/self-advection of the velocity field `v`.
@@ -200,85 +206,143 @@
   fluxes = _velocities_to_flux(aligned_v)
   return tuple(-fd.divergence(flux) for flux in fluxes)
 
 
 def advect_van_leer(
     c: GridVariable,
     v: GridVariableVector,
-    dt: float
+    dt: float,
+    mode: str = boundaries.Padding.MIRROR,
 ) -> GridArray:
   """Computes advection of a scalar quantity `c` by the velocity field `v`.
 
   Implements Van-Leer flux limiting scheme that uses second order accurate
   approximation of fluxes for smooth regions of the solution. This scheme is
   total variation diminishing (TVD). For regions with high gradients flux
   limitor transformes the scheme into a first order method. For [1] for
   reference. This function follows the following procedure:
 
-    1. Interpolate each component of `v` to the corresponding face of the
-       control volume centered on `c`. In most cases satisfied by design.
-    2. Computes upwind flux for each direction.
-    3. Computes higher order flux correction based on neighboring values of `c`.
-    4. Combines fluxes and assigns flux boundary condition.
-    5. Returns the negative divergence of fluxes.
+    1. Shifts c to offset < 1 if necessary.
+    2. Scalar c now has a well defined right-hand (upwind) value.
+    3. Computes upwind flux for each direction.
+    4. Computes van leer flux limiter:
+      a. Use the shifted c to interpolate each component of `v` to the
+        right-hand (upwind) face of the control volume centered on  `c`.
+      b. Compute the ratio of successive gradients:
+        In nonperiodic case, the value outside the boundary is not defined.
+        Mode is used to interpolate past the boundary.
+      c. Compute flux limiter function.
+      d. Computes higher order flux correction.
+    5. Combines fluxes and assigns flux boundary condition.
+    6. Computes the negative divergence of fluxes.
+    7. Shifts the computed values back to original offset of c.
 
   Args:
     c: the quantity to be transported.
     v: a velocity field. Should be defined on the same Grid as c.
     dt: time step for which this scheme is TVD and second order accurate
       in time.
+    mode: For non-periodic BC, specifies extrapolation of values beyond the
+      boundary, which is used by nonlinear interpolation.
 
   Returns:
     The time derivative of `c` due to advection by `v`.
 
   #### References
 
   [1]:  MIT 18.336 spring 2009 Finite Volume Methods Lecture 19.
         go/mit-18.336-finite_volume_methods-19
+  [2]:
+    www.ita.uni-heidelberg.de/~dullemond/lectures/num_fluid_2012/Chapter_4.pdf
 
   """
   # TODO(dkochkov) reimplement this using apply_limiter method.
-  offsets = grids.control_volume_offsets(c)
+  c_left_var = c
+  # if the offset is 1., shift by 1 to offset 0.
+  # otherwise c_right is not defined.
+  for ax in range(c.grid.ndim):
+    # int(c.offset[ax] % 1 - c.offset[ax]) = -1 if c.offset[ax] is 1 else
+    # int(c.offset[ax] % 1 - c.offset[ax]) = 0.
+    # i.e. this shifts the 1 aligned data to 0 offset, the rest is unchanged.
+    c_left_var = c.bc.impose_bc(
+        c_left_var.shift(int(c.offset[ax] % 1 - c.offset[ax]), axis=ax))
+  offsets = grids.control_volume_offsets(c_left_var)
+  # if c offset is 0, aligned_v is at 0.5.
+  # if c offset is at .5, aligned_v is at 1.
   aligned_v = tuple(interpolation.linear(u, offset)
                     for u, offset in zip(v, offsets))
   flux = []
-  for axis, (u, h) in enumerate(zip(aligned_v, c.grid.step)):
-    c_center = c.data
-    c_left = c.shift(-1, axis=axis).data
-    c_right = c.shift(+1, axis=axis).data
+  # Assign flux boundary condition
+  flux_bc = [
+      boundaries.get_advection_flux_bc_from_velocity_and_scalar(u, c, direction)
+      for direction, u in enumerate(v)
+  ]
+  # first, compute upwind flux.
+  for axis, u in enumerate(aligned_v):
+    c_center = c_left_var.data
+    # by shifting c_left + 1, c_right is well-defined.
+    c_right = c_left_var.shift(+1, axis=axis).data
     upwind_flux = grids.applied(jnp.where)(
         u.array > 0, u.array * c_center, u.array * c_right)
-
-    # Van-Leer Flux correction is computed in steps to avoid `nan`s.
-    # Formula for the flux correction df for advection with positive velocity is
-    # df_{i} = 0.5 * (1-gamma) * dc_{i}
-    # dc_{i} = 2(c_{i+1} - c_{i})(c_{i} - c_{i-1})/(c_{i+1}-c_{i})
-    # gamma is the courant number = u * dt / h
-    diffs_prod = 2 * (c_right - c_center) * (c_center - c_left)
-    neighbor_diff = c_right - c_left
-    safe = diffs_prod > 0
-    # https://jax.readthedocs.io/en/latest/faq.html#gradients-contain-nan-where-using-where
-    forward_correction = jnp.where(
-        safe, diffs_prod / jnp.where(safe, neighbor_diff, 1), 0
-    )
-    # for negative velocity we simply need to shift the correction along v axis.
-    # Cast to GridVariable so that we can apply a shift() operation.
-    forward_correction_array = grids.GridVariable(
-        grids.GridArray(forward_correction, u.offset, u.grid), u.bc)
-    backward_correction_array = forward_correction_array.shift(+1, axis)
-    backward_correction = backward_correction_array.data
-    abs_velocity = abs(u.array)
+    flux.append(upwind_flux)
+  # next, compute van_leer correction.
+  for axis, (u, h) in enumerate(zip(aligned_v, c.grid.step)):
+    u = u.bc.shift(u.array, int(u.offset[axis] % 1 - u.offset[axis]), axis=axis)
+    # c is put to offset .5 or 1.
+    c_center_arr = c.shift(int(1 - c.offset[ax]), axis=ax)
+    # if c offset is 1, u offset is .5.
+    # if c offset is .5, u offset is 0.
+    # u_i is always on the left of c_center_var_i
+    c_center = c_center_arr.data
+    # shift -1 are well defined now
+    # shift +1 is not well defined for c offset 1 because then c(wall + 1) is
+    # not defined.
+    # However, the flux that uses c(wall + 1) offset gets overridden anyways
+    # when flux boundary condition is overridden.
+    # Thus, any mode can be used here.
+    c_right = c.bc.shift(c_center_arr, +1, axis=axis, mode=mode).data
+    c_left = c.bc.shift(c_center_arr, -1, axis=axis).data
+    # shift -2 is tricky:
+    # It is well defined if c is periodic.
+    # Else, c(-1) or c(-1.5) are not defined.
+    # Then, mode is used to interpolate the values.
+    c_left_left = c.bc.shift(
+        c_center_arr, -2, axis, mode=mode).data
+
+    numerator_positive = c_left - c_left_left
+    numerator_negative = c_right - c_center
+    numerator = grids.applied(jnp.where)(u > 0, numerator_positive,
+                                         numerator_negative)
+    denominator = grids.GridArray(c_center - c_left, u.offset, u.grid)
+    # We want to calculate denominator / (abs(denominator) + abs(numerator))
+    # To make it differentiable, it needs to be done in stages.
+
+    # ensures that there is no division by 0
+    phi_van_leer_denominator_avoid_nans = grids.applied(jnp.where)(
+        abs(denominator) > 0, (abs(denominator) + abs(numerator)), 1.)
+
+    phi_van_leer_denominator_inv = denominator / phi_van_leer_denominator_avoid_nans
+
+    phi_van_leer = numerator * (grids.applied(jnp.sign)(denominator) +
+                                grids.applied(jnp.sign)
+                                (numerator)) * phi_van_leer_denominator_inv
+    abs_velocity = abs(u)
     courant_numbers = (dt / h) * abs_velocity
     pre_factor = 0.5 * (1 - courant_numbers) * abs_velocity
-    flux_correction = pre_factor * grids.applied(jnp.where)(
-        u.array > 0, forward_correction, backward_correction)
-    flux.append(upwind_flux + flux_correction)
-  # Assign flux boundary condition
-  flux = tuple(GridVariable(f, c.bc) for f in flux)
+    flux_correction = pre_factor * phi_van_leer
+    # Shift back onto original offset.
+    flux_correction = flux_bc[axis].shift(
+        flux_correction, int(offsets[axis][axis] - u.offset[axis]), axis=axis)
+    flux[axis] += flux_correction
+  flux = tuple(flux_bc[axis].impose_bc(f) for axis, f in enumerate(flux))
   advection = -fd.divergence(flux)
+  # shift the variable back onto the original offset
+  for ax in range(c.grid.ndim):
+    advection = c.bc.shift(
+        advection, -int(c.offset[ax] % 1 - c.offset[ax]), axis=ax)
   return advection
 
 
 def advect_step_semilagrangian(
     c: GridVariable,
     v: GridVariableVector,
     dt: float
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/diffusion_test.py` & `jax_cfd-0.2.1/jax_cfd/collocated/diffusion_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,20 +11,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Tests for jax_cfd.diffusion."""
 
 from absl.testing import absltest
-from absl.testing import parameterized
 import jax.numpy as jnp
 from jax_cfd.base import boundaries
-from jax_cfd.base import diffusion
 from jax_cfd.base import grids
 from jax_cfd.base import test_util
+from jax_cfd.collocated import diffusion
 
 
 class DiffusionTest(test_util.TestCase):
   """Some simple sanity tests for diffusion on constant fields."""
 
   def test_explicit_diffusion(self):
     nu = 1.
@@ -36,31 +35,10 @@
     c = grids.GridVariable(
         array=grids.GridArray(jnp.ones(shape), offset, grid),
         bc=boundaries.periodic_boundary_conditions(grid.ndim))
     diffused = diffusion.diffuse(c, nu)
     expected = grids.GridArray(jnp.zeros_like(diffused.data), offset, grid)
     self.assertAllClose(expected, diffused)
 
-  @parameterized.parameters(
-      dict(solve=diffusion.solve_cg, atol=1e-6),
-      dict(solve=diffusion.solve_fast_diag, atol=1e-6),
-  )
-  def test_implicit_diffusion(self, solve, atol):
-    nu = 1.
-    dt = 0.1
-    shape = (100, 100)
-    grid = grids.Grid(shape, step=1)
-    periodic_bc = boundaries.periodic_boundary_conditions(grid.ndim)
-    v = (
-        grids.GridVariable(
-            grids.GridArray(jnp.ones(shape), (1, 0.5), grid), periodic_bc),
-        grids.GridVariable(
-            grids.GridArray(jnp.ones(shape), (0.5, 1), grid), periodic_bc),
-    )
-    actual = solve(v, nu, dt)
-    expected = v
-    self.assertAllClose(expected[0], actual[0], atol=atol)
-    self.assertAllClose(expected[1], actual[1], atol=atol)
-
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/equations.py` & `jax_cfd-0.2.1/jax_cfd/base/equations.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 def dynamic_time_step(v: GridVariableVector,
                       max_courant_number: float,
                       viscosity: float,
                       grid: grids.Grid,
                       implicit_diffusion: bool = False) -> float:
   """Pick a dynamic time-step for Navier-Stokes based on stable advection."""
   v_max = jnp.sqrt(jnp.max(sum(u.data ** 2 for u in v)))
-  return stable_time_step(
+  return stable_time_step(  # pytype: disable=wrong-arg-types  # jax-types
       v_max, max_courant_number, viscosity, grid, implicit_diffusion)
 
 
 def _wrap_term_as_vector(fun, *, name):
   return tree_math.unwrap(jax.named_call(fun, name=name), vector_argnums=0)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/equations_test.py` & `jax_cfd-0.2.1/jax_cfd/base/equations_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/fast_diagonalization.py` & `jax_cfd-0.2.1/jax_cfd/base/fast_diagonalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import jax
 from jax import lax
 import jax.numpy as jnp
 import numpy as np
 
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 
 
 def transform(
     func: Callable[[Array], Array],
     operators: Sequence[np.ndarray],
     dtype: np.dtype,
     *,
@@ -214,15 +214,15 @@
     if rhs.dtype != dtype:
       raise ValueError(f'rhs.dtype={rhs.dtype} does not match dtype={dtype}')
     return jnp.fft.irfftn(diagonals * jnp.fft.rfftn(rhs)).astype(dtype)
 
   return apply
 
 
-def psuedoinverse(
+def pseudoinverse(
     operators: Sequence[np.ndarray],
     dtype: np.dtype,
     *,
     hermitian: bool = False,
     circulant: bool = False,
     implementation: Optional[str] = None,
     precision: lax.Precision = lax.Precision.HIGHEST,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/fast_diagonalization_test.py` & `jax_cfd-0.2.1/jax_cfd/base/fast_diagonalization_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,54 +45,54 @@
 class FastDiagonalizationTest(test_util.TestCase):
 
   def test_random_1d_matmul(self):
     rs = np.random.RandomState(0)
     a = rs.randn(3, 3)
     a = jnp.array(a + a.T, np.float32)
     b = rs.randn(3).astype(np.float32)
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         [a], b.dtype, hermitian=True, implementation='matmul')
     actual = a_inv(b)
     expected = jnp.linalg.solve(a, b)
     self.assertAllClose(actual, expected, atol=1e-6)
 
   @parameterized.parameters('fft', 'rfft')
   def test_random_1d_fft(self, implementation):
     rs = np.random.RandomState(0)
     a = jnp.array(scipy.linalg.circulant(rs.randn(4)), np.float32)
     b = rs.randn(4).astype(np.float32)
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         [a], b.dtype, circulant=True, implementation=implementation)
     actual = a_inv(b)
     expected = jnp.linalg.solve(a, b)
     self.assertAllClose(actual, expected, atol=1e-5)
 
   @parameterized.parameters(
       *[(ndim, 'matmul') for ndim in [1, 2, 3]],
       *[(ndim, 'fft') for ndim in [1, 2, 3]],
       *[(ndim, 'rfft') for ndim in [1, 2, 3]],
   )
   def test_identity_nd(self, ndim, implementation):
     rs = np.random.RandomState(0)
     b = rs.randn(*(2, 4, 6)[:ndim]).astype(np.float32)
     ops = [np.eye(2), 2 * np.eye(4), 3 * np.eye(6)]
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         ops[:ndim], b.dtype, hermitian=True, circulant=True,
         implementation=implementation)
     actual = a_inv(b)
     expected = b / sum(range(1, 1 + ndim))
     self.assertAllClose(actual, expected, rtol=1e-5, atol=1e-5)
 
   @parameterized.parameters('matmul', 'fft', 'rfft')
   def test_poisson_1d(self, implementation):
     rs = np.random.RandomState(0)
     a = jnp.array([[-2, 1, 0, 1], [1, -2, 1, 0], [0, 1, -2, 1], [1, 0, 1, -2]],
                   np.float32)
     b = rs.randn(4).astype(np.float32)
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         [a], a.dtype, hermitian=True, circulant=True,
         implementation=implementation)
     x = a_inv(b)
     self.assertAllClose(jnp.dot(a, x), b - b.mean(), atol=1e-5)
 
   @parameterized.parameters(
       dict(periodic_x=False, periodic_y=False),
@@ -103,30 +103,30 @@
     a1 = jnp.array([[-2, 1, 0, periodic_x], [1, -2, 1, 0], [0, 1, -2, 1],
                     [periodic_x, 0, 1, -2]], dtype=np.float32)
     a2 = jnp.array([[-2, 1, periodic_y], [1, -2, 1], [periodic_y, 1, -2]],
                    dtype=np.float32)
 
     b = np.random.RandomState(0).randn(4, 3).astype(np.float32)
     operators = [a1, a2]
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         operators, b.dtype, hermitian=True)
     x = a_inv(b)
     actual = apply_operators(operators, x)
     expected = b.copy()
     if periodic_x and periodic_y:
       expected -= expected.mean()
     self.assertAllClose(actual, expected, atol=1e-5)
 
   @parameterized.parameters('fft', 'rfft')
   def test_poisson_2d_fft(self, implementation):
     a1 = array_utils.laplacian_matrix(size=4, step=1.0)
     a2 = array_utils.laplacian_matrix(size=6, step=1.0)
     b = np.random.RandomState(0).randn(4, 6).astype(np.float32)
     operators = [a1, a2]
-    a_inv = fast_diagonalization.psuedoinverse(
+    a_inv = fast_diagonalization.pseudoinverse(
         operators, b.dtype, circulant=True, implementation=implementation)
     x = a_inv(b)
     actual = apply_operators(operators, x)
     expected = b - b.mean()
     self.assertAllClose(actual, expected, atol=1e-5)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/filter_utils.py` & `jax_cfd-0.2.1/jax_cfd/base/filter_utils.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/finite_differences.py` & `jax_cfd-0.2.1/jax_cfd/base/finite_differences.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 
 def central_difference(u, axis=None):
   """Approximates grads with central differences."""
   if axis is None:
     axis = range(u.grid.ndim)
   if not isinstance(axis, int):
-    return tuple(central_difference(u, a) for a in axis)
+    return tuple(central_difference(u, a) for a in axis)  # pytype: disable=wrong-arg-types  # always-use-return-annotations
   diff = stencil_sum(u.shift(+1, axis), -u.shift(-1, axis))
   return diff / (2 * u.grid.step[axis])
 
 
 @typing.overload
 def backward_difference(u: GridVariable, axis: int) -> GridArray:
   ...
@@ -93,15 +93,15 @@
 
 
 def backward_difference(u, axis=None):
   """Approximates grads with finite differences in the backward direction."""
   if axis is None:
     axis = range(u.grid.ndim)
   if not isinstance(axis, int):
-    return tuple(backward_difference(u, a) for a in axis)
+    return tuple(backward_difference(u, a) for a in axis)  # pytype: disable=wrong-arg-types  # always-use-return-annotations
   diff = stencil_sum(u.array, -u.shift(-1, axis))
   return diff / u.grid.step[axis]
 
 
 @typing.overload
 def forward_difference(u: GridVariable, axis: int) -> GridArray:
   ...
@@ -115,15 +115,15 @@
 
 
 def forward_difference(u, axis=None):
   """Approximates grads with finite differences in the forward direction."""
   if axis is None:
     axis = range(u.grid.ndim)
   if not isinstance(axis, int):
-    return tuple(forward_difference(u, a) for a in axis)
+    return tuple(forward_difference(u, a) for a in axis)  # pytype: disable=wrong-arg-types  # always-use-return-annotations
   diff = stencil_sum(u.shift(+1, axis), -u.array)
   return diff / u.grid.step[axis]
 
 
 def laplacian(u: GridVariable) -> GridArray:
   """Approximates the Laplacian of `u`."""
   scales = np.square(1 / np.array(u.grid.step, dtype=u.dtype))
@@ -162,15 +162,15 @@
 def gradient_tensor(v: Sequence[GridVariable]) -> GridArrayTensor:
   ...
 
 
 def gradient_tensor(v):
   """Approximates the cell-centered gradient of `v`."""
   if not isinstance(v, GridVariable):
-    return GridArrayTensor(np.stack([gradient_tensor(u) for u in v], axis=-1))
+    return GridArrayTensor(np.stack([gradient_tensor(u) for u in v], axis=-1))  # pytype: disable=wrong-arg-types  # always-use-return-annotations
   grad = []
   for axis in range(v.grid.ndim):
     offset = v.offset[axis]
     if offset == 0:
       derivative = forward_difference(v, axis)
     elif offset == 1:
       derivative = backward_difference(v, axis)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/finite_differences_test.py` & `jax_cfd-0.2.1/jax_cfd/base/finite_differences_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/forcings.py` & `jax_cfd-0.2.1/jax_cfd/base/forcings.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/forcings_test.py` & `jax_cfd-0.2.1/jax_cfd/base/forcings_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/funcutils.py` & `jax_cfd-0.2.1/jax_cfd/base/funcutils.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/funcutils_test.py` & `jax_cfd-0.2.1/jax_cfd/base/funcutils_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/grids.py` & `jax_cfd-0.2.1/jax_cfd/base/grids.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 import dataclasses
 import numbers
 import operator
 from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import jax
+from jax import core
 import jax.numpy as jnp
 from jax.tree_util import register_pytree_node_class
-from jax_cfd.base import array_utils
 import numpy as np
 
 # TODO(jamieas): consider moving common types to a separate module.
 # TODO(shoyer): consider adding jnp.ndarray?
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 IntOrSequence = Union[int, Sequence[int]]
 
 # There is currently no good way to indicate a jax "pytree" with arrays at its
 # leaves. See https://jax.readthedocs.io/en/latest/jax.tree_util.html for more
 # information about PyTrees and https://github.com/google/jax/issues/3340 for
 # discussion of this issue.
 PyTree = Any
@@ -80,16 +80,15 @@
   def dtype(self):
     return self.data.dtype
 
   @property
   def shape(self) -> Tuple[int, ...]:
     return self.data.shape
 
-  _HANDLED_TYPES = (numbers.Number, np.ndarray, jnp.DeviceArray,
-                    jax.ShapedArray, jax.core.Tracer)
+  _HANDLED_TYPES = (numbers.Number, np.ndarray, jax.Array, core.ShapedArray)
 
   def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
     """Define arithmetic on GridArrays using NumPy's mixin."""
     for x in inputs:
       if not isinstance(x, self._HANDLED_TYPES + (GridArray,)):
         return NotImplemented
     if method != '__call__':
@@ -149,21 +148,24 @@
   types: Tuple[Tuple[str, str], ...]
 
   def shift(
       self,
       u: GridArray,
       offset: int,
       axis: int,
+      mode: Optional[str] = 'extend',
   ) -> GridArray:
     """Shift an GridArray by `offset`.
 
     Args:
       u: an `GridArray` object.
       offset: positive or negative integer offset to shift.
       axis: axis to shift along.
+      mode: specifies how to extend past the boundary/ghost cells.
+        Valid options contained in boundaries.Padding.
 
     Returns:
       A copy of `u`, shifted by `offset`. The returned `GridArray` has offset
       `u.offset + offset`.
     """
     raise NotImplementedError(
         'shift() not implemented in BoundaryConditions base class.')
@@ -182,14 +184,87 @@
     Returns:
       A tuple of arrays of grid.ndim - 1 dimensions that specify values on the
       boundary. In case of periodic boundaries, returns a tuple(None,None).
     """
     raise NotImplementedError(
         'values() not implemented in BoundaryConditions base class.')
 
+  def pad(
+      self,
+      u: GridArray,
+      width: int,
+      axis: int,
+      mode: Optional[str] = 'extend',
+  ) -> GridArray:
+    """Returns Arrays padded according to boundary condition.
+
+    Args:
+      u: a `GridArray` object.
+      width: number of elements to pad along axis. Use negative value for lower
+        boundary or positive value for upper boundary.
+      axis: axis to pad along.
+      mode: specifies how to extend past the boundary/ghost cells.
+        Valid options contained in boundaries.Padding.
+
+    Returns:
+      A GridArray that is elongated along axis with padded values.
+    """
+    raise NotImplementedError(
+        'pad() not implemented in BoundaryConditions base class.')
+
+  def trim_boundary(self, u: GridArray) -> GridArray:
+    """Returns GridArray without the grid points on the boundary.
+
+    Some grid points of GridArray might coincide with boundary. This trims those
+    values.
+
+    Args:
+      u: a `GridArray` object.
+
+    Returns:
+      A GridArray shrunk along certain dimensions.
+    """
+    raise NotImplementedError(
+        'trim_boundary() not implemented in BoundaryConditions base class.')
+
+  def pad_and_impose_bc(
+      self,
+      u: GridArray,
+      offset_to_pad_to: Optional[Tuple[float, ...]] = None) -> GridVariable:
+    """Returns GridVariable with correct boundary condition.
+
+    Some grid points of GridArray might coincide with boundary. This ensures
+    that the GridVariable.array agrees with GridVariable.bc.
+    Args:
+      u: a `GridArray` object that specifies only scalar values on the internal
+        nodes.
+      offset_to_pad_to: a Tuple of desired offset to pad to. Note that if the
+        function is given just an interior array in dirichlet case, it can pad
+        to both 0 offset and 1 offset.
+
+    Returns:
+      A GridVariable that has correct boundary.
+    """
+    raise NotImplementedError(
+        'pad_and_impose_bc() not implemented in BoundaryConditions base class.')
+
+  def impose_bc(self, u: GridArray) -> GridVariable:
+    """Returns GridVariable with correct boundary condition.
+
+    Some grid points of GridArray might coincide with boundary. This ensures
+    that the GridVariable.array agrees with GridVariable.bc.
+    Args:
+      u: a `GridArray` object.
+
+    Returns:
+      A GridVariable that has correct boundary.
+    """
+    raise NotImplementedError(
+        'impose_bc() not implemented in BoundaryConditions base class.')
+
 
 @register_pytree_node_class
 @dataclasses.dataclass
 class GridVariable:
   """Associates a GridArray with BoundaryConditions.
 
   Performing pad and shift operations, e.g. for finite difference calculations,
@@ -253,26 +328,29 @@
   def grid(self) -> Grid:
     return self.array.grid
 
   def shift(
       self,
       offset: int,
       axis: int,
+      mode: Optional[str] = 'extend',
   ) -> GridArray:
     """Shift this GridVariable by `offset`.
 
     Args:
       offset: positive or negative integer offset to shift.
       axis: axis to shift along.
+      mode: specifies how to extend past the boundary/ghost cells.
+        Valid options contained in boundaries.Padding.
 
     Returns:
       A copy of the encapsulated GridArray, shifted by `offset`. The returned
       GridArray has offset `u.offset + offset`.
     """
-    return self.bc.shift(self.array, offset, axis)
+    return self.bc.shift(self.array, offset, axis, mode)
 
   def _interior_grid(self) -> Grid:
     """Returns only the interior grid points."""
     grid = self.array.grid
     domain = list(grid.domain)
     shape = list(grid.shape)
     for axis in range(self.grid.ndim):
@@ -285,30 +363,15 @@
         shape[axis] -= 1
         domain[axis] = (domain[axis][0], domain[axis][1] - grid.step[axis])
       elif np.isclose(self.array.offset[axis], 0.0):
         shape[axis] -= 1
         domain[axis] = (domain[axis][0] + grid.step[axis], domain[axis][1])
     return Grid(shape, domain=tuple(domain))
 
-  def _interior_array(self) -> Array:
-    """Returns only the interior points of self.array."""
-    data = self.array.data
-    for axis in range(self.grid.ndim):
-      # nothing happens in periodic case
-      if self.bc.types[axis][1] == 'periodic':
-        continue
-      # nothing happens if the offset is not 0.0 or 1.0
-      if np.isclose(self.offset[axis], 1.0):
-        data, _ = array_utils.split_along_axis(data, -1, axis)
-      elif np.isclose(self.offset[axis], 0.0):
-        _, data = array_utils.split_along_axis(data, 1, axis)
-
-    return data
-
-  def interior(self) -> GridArray:
+  def trim_boundary(self) -> GridArray:
     """Returns a GridArray associated only with interior points.
 
      Interior is defined as the following:
        for d in range(u.grid.ndim):
         points = u.grid.axes(offset=u.offset[d])
         interior_points =
           all points where grid.domain[d][0] < points < grid.domain[d][1]
@@ -316,45 +379,24 @@
     The exception is when the boundary conditions are periodic,
     in which case all points are included in the interior.
 
     In case of dirichlet with edge offset, the grid and array size is reduced,
     since one scalar lies exactly on the boundary. In all other cases,
     self.grid and self.array are returned.
     """
-    interior_array = self._interior_array()
-    interior_grid = self._interior_grid()
-    return GridArray(interior_array, self.array.offset, interior_grid)
+    return self.bc.trim_boundary(self.array)
 
-  def enforce_edge_bc(self, *args) -> GridVariable:
+  def impose_bc(self) -> GridVariable:
     """Returns the GridVariable with edge BC enforced, if applicable.
 
     For GridVariables having nonperiodic BC and offset 0 or 1, there are values
     in the array data that are dependent on the boundary condition.
-    enforce_edge_bc() changes these boundary values to match the prescribed BC.
-
-    Args:
-      *args: any optional values passed into BoundaryConditions values method.
+    impose_bc() changes these boundary values to match the prescribed BC.
     """
-    if self.grid.shape != self.array.data.shape:
-      raise ValueError('Stored array and grid have mismatched sizes.')
-    data = jnp.array(self.array.data)
-    for axis in range(self.grid.ndim):
-      if 'periodic' not in self.bc.types[axis]:
-        values = self.bc.values(axis, self.grid, *args)
-        for boundary_side in range(2):
-          if np.isclose(self.array.offset[axis], boundary_side):
-            # boundary data is set to match self.bc:
-            all_slice = [
-                slice(None, None, None),
-            ] * self.grid.ndim
-            all_slice[axis] = -boundary_side
-            data = data.at[tuple(all_slice)].set(values[boundary_side])
-    return GridVariable(
-        array=GridArray(data, self.array.offset, self.grid),
-        bc=self.bc)
+    return self.bc.impose_bc(self.array)
 
 
 GridVariableVector = Tuple[GridVariable, ...]
 
 
 def applied(func):
   """Convert an array function into one defined on GridArrays.
@@ -440,15 +482,15 @@
   return grid
 
 
 class InconsistentBoundaryConditionsError(Exception):
   """Raised for cases of inconsistent bc between GridVariables."""
 
 
-def consistent_boundary_conditions(*arrays: GridVariable) -> BoundaryConditions:
+def unique_boundary_conditions(*arrays: GridVariable) -> BoundaryConditions:
   """Returns the unique BCs, or raises InconsistentBoundaryConditionsError."""
   bcs = {array.bc for array in arrays}
   if len(bcs) != 1:
     raise InconsistentBoundaryConditionsError(
         f'arrays do not have a unique bc: {bcs}')
   bc, = bcs
   return bc
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/grids_test.py` & `jax_cfd-0.2.1/jax_cfd/base/grids_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,43 +164,43 @@
   def test_constructor_and_attributes(self):
     with self.subTest('1d'):
       grid = grids.Grid((10,))
       data = np.zeros((10,), dtype=np.float32)
       array = grids.GridArray(data, offset=(0.5,), grid=grid)
       bc = boundaries.periodic_boundary_conditions(grid.ndim)
       variable = grids.GridVariable(array, bc)
-      self.assertEqual(variable.array, array)
+      self.assertArrayEqual(variable.array, array)
       self.assertEqual(variable.bc, bc)
       self.assertEqual(variable.dtype, np.float32)
       self.assertEqual(variable.shape, (10,))
       self.assertArrayEqual(variable.data, data)
       self.assertEqual(variable.offset, (0.5,))
       self.assertEqual(variable.grid, grid)
 
     with self.subTest('2d'):
       grid = grids.Grid((10, 10))
       data = np.zeros((10, 10), dtype=np.float32)
       array = grids.GridArray(data, offset=(0.5, 0.5), grid=grid)
       bc = boundaries.periodic_boundary_conditions(grid.ndim)
       variable = grids.GridVariable(array, bc)
-      self.assertEqual(variable.array, array)
+      self.assertArrayEqual(variable.array, array)
       self.assertEqual(variable.bc, bc)
       self.assertEqual(variable.dtype, np.float32)
       self.assertEqual(variable.shape, (10, 10))
       self.assertArrayEqual(variable.data, data)
       self.assertEqual(variable.offset, (0.5, 0.5))
       self.assertEqual(variable.grid, grid)
 
     with self.subTest('batch dim data'):
       grid = grids.Grid((10, 10))
       data = np.zeros((5, 10, 10), dtype=np.float32)
       array = grids.GridArray(data, offset=(0.5, 0.5), grid=grid)
       bc = boundaries.periodic_boundary_conditions(grid.ndim)
       variable = grids.GridVariable(array, bc)
-      self.assertEqual(variable.array, array)
+      self.assertArrayEqual(variable.array, array)
       self.assertEqual(variable.bc, bc)
       self.assertEqual(variable.dtype, np.float32)
       self.assertEqual(variable.shape, (5, 10, 10))
       self.assertArrayEqual(variable.data, data)
       self.assertEqual(variable.offset, (0.5, 0.5))
       self.assertEqual(variable.grid, grid)
 
@@ -237,16 +237,16 @@
   )
   def test_interior_consistency_periodic(self, shape, offset):
     grid = grids.Grid(shape)
     data = np.random.randint(0, 10, shape)
     array = grids.GridArray(data, offset=offset, grid=grid)
     bc = boundaries.periodic_boundary_conditions(ndim=len(shape))
     u = grids.GridVariable(array, bc)
-    u_interior = u.interior()
-    self.assertEqual(u_interior, u.array)
+    u_interior = u.trim_boundary()
+    self.assertArrayEqual(u_interior, u.array)
 
   @parameterized.parameters(
       dict(
           shape=(10,),
           bc=boundaries.dirichlet_boundary_conditions(ndim=1),
       ),
       dict(
@@ -271,55 +271,63 @@
       ),
   )
   def test_interior_consistency_no_edge_offsets(self, bc, shape):
     grid = grids.Grid(shape)
     data = np.random.randint(0, 10, shape)
     array = grids.GridArray(data, offset=(0.5,) * len(shape), grid=grid)
     u = grids.GridVariable(array, bc)
-    u_interior = u.interior()
-    self.assertEqual(u_interior, u.array)
+    u_interior = u.trim_boundary()
+    self.assertArrayEqual(u_interior, u.array)
 
   @parameterized.parameters(
       dict(
           shape=(10,),
-          bc=boundaries.dirichlet_boundary_conditions(ndim=1),
-          offset=(0.0,)),
+          bc=boundaries.neumann_boundary_conditions(ndim=1),
+          offset=(0.5,)),
+      dict(
+          shape=(10, 10),
+          bc=boundaries.neumann_boundary_conditions(ndim=2),
+          offset=(0.5, 0.5)),
+      dict(
+          shape=(10, 10, 10),
+          bc=boundaries.neumann_boundary_conditions(ndim=3),
+          offset=(0.5, 0.5, 0.5)),
+  )
+  def test_interior_consistency_neumann(self, shape, bc, offset):
+    grid = grids.Grid(shape)
+    data = np.random.randint(0, 10, shape)
+    array = grids.GridArray(data, offset=offset, grid=grid)
+    u = grids.GridVariable(array, bc)
+    u_interior = u.trim_boundary()
+    self.assertArrayEqual(u_interior, u.array)
+
+  @parameterized.parameters(
       dict(
           shape=(10,),
-          bc=boundaries.neumann_boundary_conditions(ndim=1),
+          bc=boundaries.dirichlet_boundary_conditions(ndim=1),
           offset=(0.0,)),
       dict(
           shape=(10, 10),
           bc=boundaries.dirichlet_boundary_conditions(ndim=2),
           offset=(0.0, 0.0)),
       dict(
-          shape=(10, 10),
-          bc=boundaries.neumann_boundary_conditions(ndim=2),
-          offset=(0.0, 0.0)),
-      dict(
           shape=(10, 10, 10),
           bc=boundaries.dirichlet_boundary_conditions(ndim=3),
           offset=(0.0, 0.0, 0.0)),
-      dict(
-          shape=(10, 10, 10),
-          bc=boundaries.neumann_boundary_conditions(ndim=3),
-          offset=(0.0, 0.0, 0.0)),
   )
-  def test_interior_consistency_edge_offsets(self, shape, bc, offset):
+  def test_interior_consistency_edge_offsets_dirichlet(self, shape, bc, offset):
     grid = grids.Grid(shape)
     data = np.random.randint(0, 10, shape)
     array = grids.GridArray(data, offset=offset, grid=grid)
     u = grids.GridVariable(array, bc)
-    u_interior = u.interior()
-
-    self.assertEqual(u_interior.offset, u.array.offset)
+    u_interior = u.trim_boundary()
+    self.assertEqual(u_interior.offset,
+                     tuple(offset + 1 for offset in u.array.offset))
     self.assertEqual(u_interior.grid.ndim, u.array.grid.ndim)
     self.assertEqual(u_interior.grid.step, u.array.grid.step)
-    self.assertEqual(
-        u_interior.grid.mesh(offset)[0].shape, u_interior.data.shape)
 
   def test_interior_dirichlet(self):
     data = np.array([
         [11, 12, 13, 14, 15],
         [21, 22, 23, 24, 25],
         [31, 32, 33, 34, 35],
         [41, 42, 43, 44, 45],
@@ -328,71 +336,65 @@
     grid = grids.Grid(shape=(4, 5), domain=((0, 1), (0, 1)))
     bc = boundaries.dirichlet_boundary_conditions(ndim=2)
 
     with self.subTest('offset=(1, 0.5)'):
       offset = (1., 0.5)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       answer = np.array([[11, 12, 13, 14, 15], [21, 22, 23, 24, 25],
                          [31, 32, 33, 34, 35]])
       self.assertArrayEqual(u_interior.data, answer)
       self.assertEqual(u_interior.offset, offset)
-      self.assertEqual(u_interior.grid,
-                       grids.Grid(shape=(3, 5), domain=((0, 0.75), (0, 1))))
+      self.assertEqual(u.grid, grid)
 
     with self.subTest('offset=(1, 1)'):
       offset = (1., 1.)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       answer = np.array([[11, 12, 13, 14], [21, 22, 23, 24], [31, 32, 33, 34]])
       self.assertArrayEqual(u_interior.data, answer)
-      self.assertEqual(u_interior.grid,
-                       grids.Grid(shape=(3, 4), domain=((0, 0.75), (0, 0.8))))
+      self.assertEqual(u_interior.grid, grid)
 
     with self.subTest('offset=(0.0, 0.5)'):
       offset = (0., 0.5)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       answer = np.array([[21, 22, 23, 24, 25], [31, 32, 33, 34, 35],
                          [41, 42, 43, 44, 45]])
       self.assertArrayEqual(u_interior.data, answer)
-      self.assertEqual(u_interior.grid,
-                       grids.Grid(shape=(3, 5), domain=((0.25, 1.), (0., 1.))))
+      self.assertEqual(u_interior.grid, grid)
 
     with self.subTest('offset=(0.0, 0.0)'):
       offset = (0.0, 0.0)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       answer = np.array([[22, 23, 24, 25], [32, 33, 34, 35], [42, 43, 44, 45]])
       self.assertArrayEqual(u_interior.data, answer)
-      self.assertEqual(
-          u_interior.grid,
-          grids.Grid(shape=(3, 4), domain=((0.25, 1.), (0.2, 1.0))))
+      self.assertEqual(u_interior.grid, grid)
 
     with self.subTest('offset=(0.5, 0.0)'):
       offset = (0.5, 0.0)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       answer = np.array([[12, 13, 14, 15], [22, 23, 24, 25], [32, 33, 34, 35],
                          [42, 43, 44, 45]])
       self.assertArrayEqual(u_interior.data, answer)
-      self.assertEqual(u_interior.grid,
-                       grids.Grid(shape=(4, 4), domain=((0.0, 1.), (0.2, 1.0))))
+      self.assertEqual(u_interior.grid, grid)
 
     # this is consistent for all offsets, not just edge and center.
     with self.subTest('offset=(0.25, 0.75)'):
       offset = (0.25, 0.75)
       array = grids.GridArray(data, offset, grid)
       u = grids.GridVariable(array, bc)
-      u_interior = u.interior()
+      u_interior = u.trim_boundary()
       self.assertArrayEqual(u_interior.data, data)
       self.assertEqual(u_interior.grid, grid)
 
   @parameterized.parameters(
       dict(
           shape=(10,),
           bc=boundaries.periodic_boundary_conditions(ndim=1),
@@ -427,28 +429,28 @@
                                   'Incompatible dimension between grid and bc'):
         grid = grids.Grid((10,))
         data = np.zeros((10,))
         array = grids.GridArray(data, offset=(0.5,), grid=grid)  # 1D
         bc = boundaries.periodic_boundary_conditions(ndim=2)  # 2D
         grids.GridVariable(array, bc)
 
-  def test_consistent_boundary_conditions(self):
+  def test_unique_boundary_conditions(self):
     grid = grids.Grid((5,))
     array = grids.GridArray(np.arange(5), offset=(0.5,), grid=grid)
     bc1 = boundaries.periodic_boundary_conditions(grid.ndim)
     bc2 = boundaries.dirichlet_boundary_conditions(grid.ndim)
     x_bc1 = grids.GridVariable(array, bc1)
     y_bc1 = grids.GridVariable(array, bc1)
     z_bc2 = grids.GridVariable(array, bc2)
 
-    bc = grids.consistent_boundary_conditions(x_bc1, y_bc1)
+    bc = grids.unique_boundary_conditions(x_bc1, y_bc1)
     self.assertEqual(bc, bc1)
 
     with self.assertRaises(grids.InconsistentBoundaryConditionsError):
-      grids.consistent_boundary_conditions(x_bc1, y_bc1, z_bc2)
+      grids.unique_boundary_conditions(x_bc1, y_bc1, z_bc2)
 
 
 class GridArrayTensorTest(test_util.TestCase):
 
   def test_tensor_transpose(self):
     grid = grids.Grid((5, 5))
     offset = (0.5, 0.5)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/initial_conditions.py` & `jax_cfd-0.2.1/jax_cfd/base/initial_conditions.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,41 +25,51 @@
 from jax_cfd.base import grids
 from jax_cfd.base import pressure
 import numpy as np
 
 # Specifying the full signatures of Callable would get somewhat onerous
 # pylint: disable=g-bare-generic
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariable = grids.GridVariable
 GridVariableVector = grids.GridVariableVector
 BoundaryConditions = grids.BoundaryConditions
 
 
-def wrap_velocities(
-    v: Sequence[Array],
+def wrap_variables(
+    var: Sequence[Array],
     grid: grids.Grid,
     bcs: Sequence[BoundaryConditions],
+    offsets: Optional[Sequence[Tuple[float, ...]]] = None,
+    batch_dim: bool = False,
 ) -> GridVariableVector:
-  """Wrap velocity arrays for input into simulations."""
-  return tuple(grids.GridVariable(grids.GridArray(u, offset, grid), bc)
-               for u, offset, bc in zip(v, grid.cell_faces, bcs))
+  """Associates offsets, grid, and boundary conditions with a sequence of arrays."""
+  if offsets is None:
+    offsets = grid.cell_faces
+  def impose_bc(arrays):
+    return tuple(
+        bc.impose_bc(grids.GridArray(u, offset, grid))
+        for u, offset, bc in zip(arrays, offsets, bcs))
+  if batch_dim:
+    return jax.vmap(impose_bc)(var)
+  else:
+    return impose_bc(var)
 
 
 def _log_normal_pdf(x, mode, variance=.25):
   """Unscaled PDF for a log normal given `mode` and log variance 1."""
   mean = jnp.log(mode) + variance
   logx = jnp.log(x)
   return jnp.exp(-(mean - logx)**2 / 2 / variance - logx)
 
 
 def _max_speed(v):
-  return jnp.linalg.norm([u.data for u in v], axis=0).max()
+  return jnp.linalg.norm(jnp.array([u.data for u in v]), axis=0).max()
 
 
 def filtered_velocity_field(
     rng_key: grids.Array,
     grid: grids.Grid,
     maximum_velocity: float = 1,
     peak_wavenumber: float = 3,
@@ -93,15 +103,15 @@
   boundary_conditions = []
   for k in keys:
     noise = jax.random.normal(k, grid.shape)
     velocity_components.append(
         filter_utils.filter(spectral_density, noise, grid))
     boundary_conditions.append(
         boundaries.periodic_boundary_conditions(grid.ndim))
-  velocity = wrap_velocities(velocity_components, grid, boundary_conditions)
+  velocity = wrap_variables(velocity_components, grid, boundary_conditions)
 
   def project_and_normalize(v: GridVariableVector):
     v = pressure.projection(v)
     vmax = _max_speed(v)
     v = tuple(
         grids.GridVariable(maximum_velocity * u.array / vmax, u.bc) for u in v)
     return v
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/initial_conditions_test.py` & `jax_cfd-0.2.1/jax_cfd/base/initial_conditions_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
            maximum_velocity=10.,
            peak_wavenumber=17),
   )
   def test_filtered_velocity_field(
       self, seed, grid, maximum_velocity, peak_wavenumber):
     v = ic.filtered_velocity_field(
         jax.random.PRNGKey(seed), grid, maximum_velocity, peak_wavenumber)
-    actual_maximum_velocity = jnp.linalg.norm([u.data for u in v], axis=0).max()
+    actual_maximum_velocity = jnp.linalg.norm(jnp.array([u.data for u in v]), axis=0).max()
     max_divergence = fd.divergence(v).data.max()
 
     # Assert that initial velocity is divergence free
     self.assertAllClose(0., max_divergence, atol=5e-4)
 
     # Assert that the specified maximum velocity is obtained.
     self.assertAllClose(maximum_velocity, actual_maximum_velocity, atol=1e-5)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/interpolation.py` & `jax_cfd-0.2.1/jax_cfd/base/interpolation.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import jax
 import jax.numpy as jnp
 from jax_cfd.base import boundaries
 from jax_cfd.base import grids
 import numpy as np
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariable = grids.GridVariable
 GridVariableVector = grids.GridVariableVector
 InterpolationFn = Callable[
     [GridVariable, Tuple[float, ...], GridVariableVector, float],
     GridVariable]
@@ -307,15 +307,15 @@
 # Not required since no .shift() method is used
 def point_interpolation(
     point: Array,
     c: GridArray,
     order: int = 1,
     mode: str = 'nearest',
     cval: float = 0.0,
-) -> jnp.DeviceArray:
+) -> jax.Array:
   """Interpolate `c` at `point`.
 
   Args:
     point: length N 1-D Array. The point to interpolate to.
     c: N-dimensional GridArray. The values that will be interpolated.
     order: Integer in the range 0-1. The order of the spline interpolation.
     mode: one of {'reflect', 'constant', 'nearest', 'mirror', 'wrap'}.
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/interpolation_test.py` & `jax_cfd-0.2.1/jax_cfd/base/interpolation_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/pressure_test.py` & `jax_cfd-0.2.1/jax_cfd/base/pressure_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
 """Tests for jax_cfd.pressure."""
 
 import functools
 
 from absl.testing import absltest
 from absl.testing import parameterized
-
 import jax
+from jax_cfd.base import array_utils
 from jax_cfd.base import boundaries
+from jax_cfd.base import fast_diagonalization
 from jax_cfd.base import finite_differences as fd
 from jax_cfd.base import grids
 from jax_cfd.base import pressure
 from jax_cfd.base import test_util
 import numpy as np
 
 USE_FLOAT64 = True
@@ -34,14 +35,31 @@
 
 class PressureTest(test_util.TestCase):
 
   def setUp(self):
     jax.config.update('jax_enable_x64', USE_FLOAT64)
     super(PressureTest, self).setUp()
 
+  def poisson_setup(self, bc, offset):
+    rs = np.random.RandomState(0)
+    b = rs.randn(4, 4).astype(np.float32)
+    grid = grids.Grid((4, 4), domain=((0, 4), (0, 4)))  # has step = 1.0
+    b = grids.GridArray(b, offset, grid)
+    a = array_utils.laplacian_matrix_w_boundaries(grid, offset, bc)
+    b_transformed = pressure._rhs_transform(
+        bc.trim_boundary(b), bc)
+    a_inv = fast_diagonalization.pseudoinverse(
+        a, b.dtype, hermitian=True, circulant=False, implementation='matmul')
+    x = a_inv(b_transformed)
+    x = grids.GridArray(x, b.offset, grid)
+    # laplacian is defined only on the interior
+    x = grids.GridVariable(x, bc)
+    x = fd.laplacian(x).data
+    return x, b
+
   @parameterized.named_parameters(
       dict(testcase_name='_1D_cg',
            shape=(301,),
            solve=solve_cg,
            step=(.1,),
            seed=111),
       dict(testcase_name='_2D_cg',
@@ -155,15 +173,15 @@
 
     v = tuple(
         grids.GridArray(
             1. + .3 * rand_array(seed=d), offset=grid.cell_faces[d], grid=grid)
         for d in range(ndim))
 
     # Associate and enforce boundary conditions
-    v = tuple(grids.GridVariable(u, u_bc).enforce_edge_bc()
+    v = tuple(grids.GridVariable(u, u_bc).impose_bc()
               for u, u_bc in zip(v, velocity_bc))
 
     # y-velocity = 0 for the edge y=y_max (homogeneous Diriclet BC)
     # y-velocity on lower y-boundary is not on an edge
     # Note, x- and z-velocity do not have an edge value on the y-boundaries
     self.assertAllClose(v[1].data[:, -1, ...], 0)
 
@@ -172,9 +190,27 @@
 
     # The corrected velocity should be divergence free.
     div = fd.divergence(v_corrected)
     for u, u_corrected in zip(v, v_corrected):
       np.testing.assert_allclose(u.offset, u_corrected.offset)
     np.testing.assert_allclose(div.data, 0., atol=1e-4)
 
+  @parameterized.parameters(((1.0, 0.5),), ((1.0, 1.0),), ((1.0, 0.0),))
+  def test_poisson_periodic_and_dirichlet(self, offset):
+    bc = boundaries.periodic_and_dirichlet_boundary_conditions()
+    x, b = self.poisson_setup(bc, offset)
+    self.assertAllClose(x, bc.trim_boundary(b).data, atol=1e-5)
+
+  @parameterized.parameters(((1.0, 0.5),), ((0.5, 0.5),))
+  def test_poisson_periodic_and_neumann(self, offset):
+    bc = boundaries.periodic_and_neumann_boundary_conditions()
+    x, b = self.poisson_setup(bc, offset)
+    self.assertAllClose(x, b.data - b.data.mean(), atol=1e-5)
+
+  @parameterized.parameters(((1.0, 0.5),), ((1.0, 1.0),), ((1.0, 0.0),))
+  def test_poisson_2d_periodic(self, offset):
+    bc = boundaries.periodic_boundary_conditions(2)
+    x, b = self.poisson_setup(bc, offset)
+    self.assertAllClose(x, b.data - b.data.mean(), atol=1e-5)
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/subgrid_models.py` & `jax_cfd-0.2.1/jax_cfd/base/subgrid_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
   #
   # This should be revised so that s_ij is computed by first interpolating
   # velocity and then computing s_ij via finite differences, producing
   # a `GridVariableTensor`. Then no wrapper or GridArray/GridVariable
   # conversion hacks are needed.
   if not boundaries.has_all_periodic_boundary_conditions(*v):
     raise ValueError('smagorinsky_viscosity only valid for periodic BC.')
-  bc = grids.consistent_boundary_conditions(*v)
+  bc = grids.unique_boundary_conditions(*v)
 
   def wrapped_interp_fn(c, offset, v, dt):
     return interpolate_fn(grids.GridVariable(c, bc), offset, v, dt).array
 
   grid = grids.consistent_grid(*s_ij.ravel(), *v)
   bc = boundaries.periodic_boundary_conditions(grid.ndim)
   s_ij_offsets = [array.offset for array in s_ij.ravel()]
@@ -162,15 +162,15 @@
   cg_kwargs = dict(cg_kwargs)
   cg_kwargs.setdefault('tol', 1e-6)
   cg_kwargs.setdefault('atol', 1e-6)
 
   if not boundaries.has_all_periodic_boundary_conditions(*v):
     raise ValueError(
         'implicit_evm_solve_with_diffusion only valid for periodic BC.')
-  bc = grids.consistent_boundary_conditions(*v)
+  bc = grids.unique_boundary_conditions(*v)
   vector_laplacian = np.vectorize(finite_differences.laplacian)
 
   # the arg v from the outer function.
   def linear_op(velocity):
     v_var = tuple(grids.GridVariable(u, bc) for u in velocity)
     acceleration = configured_evm_model(v_var)
     return tuple(
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/subgrid_models_test.py` & `jax_cfd-0.2.1/jax_cfd/base/subgrid_models_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/test_util.py` & `jax_cfd-0.2.1/jax_cfd/base/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Shared test utilities."""
 
 from absl.testing import parameterized
 
-from jax.config import config
+from jax import config
 from jax_cfd.base import grids
 import numpy as np
 
 config.parse_flags_with_absl()
 
 
 class TestCase(parameterized.TestCase):
@@ -65,15 +65,15 @@
       except grids.InconsistentOffsetError as e:
         raise AssertionError(str(e)) from None
       try:
         grids.consistent_grid(*arrays)
       except grids.InconsistentGridError as e:
         raise AssertionError(str(e)) from None
       try:
-        grids.consistent_boundary_conditions(*arrays)
+        grids.unique_boundary_conditions(*arrays)
       except grids.InconsistentBoundaryConditionsError as e:
         raise AssertionError(str(e)) from None
       arrays = tuple(array.array.data for array in arrays)
     return arrays
 
   # pylint: disable=unbalanced-tuple-unpacking
   def assertArrayEqual(self, expected, actual, **kwargs):
@@ -83,7 +83,9 @@
 
   def assertAllClose(self, expected, actual, **kwargs):
     expected, actual = self._check_and_remove_alignment_and_grid(
         expected, actual)
     np.testing.assert_allclose(expected, actual, **kwargs)
 
   # pylint: enable=unbalanced-tuple-unpacking
+
+
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/time_stepping.py` & `jax_cfd-0.2.1/jax_cfd/base/time_stepping.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/time_stepping_test.py` & `jax_cfd-0.2.1/jax_cfd/base/time_stepping_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 """Tests for time_stepping."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import jax
-from jax.config import config
+from jax import config
 import jax.numpy as jnp
 from jax_cfd.base import funcutils
 from jax_cfd.base import time_stepping
 import numpy as np
 
 
 def harmonic_oscillator(x0, t):
```

### Comparing `jax-cfd-0.2.0/jax_cfd/base/validation_problems.py` & `jax_cfd-0.2.1/jax_cfd/base/validation_problems.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/base/validation_test.py` & `jax_cfd-0.2.1/jax_cfd/base/validation_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/__init__.py` & `jax_cfd-0.2.1/jax_cfd/collocated/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/advection.py` & `jax_cfd-0.2.1/jax_cfd/collocated/advection.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,30 +12,35 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Module for functionality related to advection."""
 
 from typing import Optional, Tuple
 
+from jax_cfd.base import boundaries
 from jax_cfd.base import finite_differences as fd
 from jax_cfd.base import grids
 
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariable = grids.GridVariable
 GridVariableVector = grids.GridVariableVector
 
 
 def advect_linear(c: GridVariable,
                   v: GridVariableVector,
                   dt: Optional[float] = None) -> GridArray:
   """Computes advection for collocated scalar `c` with velocity `v`."""
   del dt
-  # Flux inherits boundary conditions from c
-  flux = tuple(grids.GridVariable(c.array * u.array, c.bc) for u in v)
+  flux_bc = [
+      boundaries.get_advection_flux_bc_from_velocity_and_scalar(u, c, direction)
+      for direction, u in enumerate(v)
+  ]
+  flux = tuple(flux_bc[axis].impose_bc(c.array * v[axis].array)
+               for axis in range(c.grid.ndim))
   return -fd.centered_divergence(flux)
 
 
 def _velocities_to_flux(v: GridVariableVector) -> Tuple[GridVariableVector]:
   """Computes the cell-centered convective flux for a velocity field.
 
   This is the flux associated with the nonlinear term `vv` for velocity `v`.
@@ -50,16 +55,17 @@
   ndim = len(v)
   flux = [tuple() for _ in range(ndim)]
   ndim = len(v)
   flux = [tuple() for _ in range(ndim)]
   for i in range(ndim):
     for j in range(ndim):
       if i <= j:
-        bc = grids.consistent_boundary_conditions(v[i], v[j])
-        flux[i] += (GridVariable(v[i].array * v[j].array, bc),)
+        bc = boundaries.get_advection_flux_bc_from_velocity_and_scalar(
+            v[j], v[i], j)
+        flux[i] += (bc.impose_bc(v[i].array * v[j].array),)
       else:
         flux[i] += (flux[j][i],)
   return tuple(flux)
 
 
 def convect_linear(v: GridVariableVector) -> GridArrayVector:
   """Computes convection/self-advection of the velocity field `v`.
```

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/diffusion.py` & `jax_cfd-0.2.1/jax_cfd/collocated/diffusion.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/equations.py` & `jax_cfd-0.2.1/jax_cfd/collocated/equations.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/equations_test.py` & `jax_cfd-0.2.1/jax_cfd/collocated/equations_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
            density=1.,
            viscosity=1e-4,
            convect=None,
            pressure_solve=pressure.solve_cg,
            dt=1e-3,
            time_steps=1000,
            divergence_atol=1e-3,
-           momentum_atol=2e-3),
+           momentum_atol=5e-3),
       dict(testcase_name='semi_implicit_gaussian_force_upwind',
            velocity=zero_velocity_field,
            forcing=gaussian_forcing,
            shape=(40, 40, 40),
            step=(1., 1., 1.),
            density=1.,
            viscosity=None,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/initial_conditions.py` & `jax_cfd-0.2.1/jax_cfd/collocated/initial_conditions.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from jax_cfd.base import grids
 from jax_cfd.collocated import pressure
 import numpy as np
 
 # Specifying the full signatures of Callable would get somewhat onerous
 # pylint: disable=g-bare-generic
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariable = grids.GridVariable
 GridVariableVector = grids.GridVariableVector
 BoundaryConditions = grids.BoundaryConditions
 
 
@@ -40,15 +40,15 @@
   """Unscaled PDF for a log normal given `mode` and log variance 1."""
   mean = jnp.log(mode) + variance
   logx = jnp.log(x)
   return jnp.exp(-(mean - logx)**2 / 2 / variance - logx)
 
 
 def _max_speed(v):
-  return jnp.linalg.norm([u.data for u in v], axis=0).max()
+  return jnp.linalg.norm(jnp.array([u.data for u in v]), axis=0).max()
 
 
 def filtered_velocity_field(
     rng_key: grids.Array,
     grid: grids.Grid,
     maximum_velocity: float = 1,
     peak_wavenumber: float = 3,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/initial_conditions_test.py` & `jax_cfd-0.2.1/jax_cfd/collocated/initial_conditions_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
            maximum_velocity=1.,
            peak_wavenumber=2),
   )
   def test_filtered_velocity_field(
       self, seed, grid, maximum_velocity, peak_wavenumber):
     v = initial_conditions.filtered_velocity_field(
         jax.random.PRNGKey(seed), grid, maximum_velocity, peak_wavenumber)
-    actual_maximum_velocity = jnp.linalg.norm([u.data for u in v], axis=0).max()
+    actual_maximum_velocity = jnp.linalg.norm(jnp.array([u.data for u in v]), axis=0).max()
     max_divergence = fd.centered_divergence(v).data.max()
 
     # Assert that initial velocity is divergence free
     self.assertAllClose(0., max_divergence, atol=1e-4)
 
     # Assert that the specified maximum velocity is obtained.
     self.assertAllClose(maximum_velocity, actual_maximum_velocity, atol=1e-4)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/pressure.py` & `jax_cfd-0.2.1/jax_cfd/collocated/pressure.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/collocated/pressure_test.py` & `jax_cfd-0.2.1/jax_cfd/collocated/pressure_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/data/__init__.py` & `jax_cfd-0.2.1/jax_cfd/data/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/data/evaluation.py` & `jax_cfd-0.2.1/jax_cfd/data/evaluation.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/data/visualization.py` & `jax_cfd-0.2.1/jax_cfd/data/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
   norm = mpl.colors.Normalize(vmin=-max_to_include, vmax=max_to_include)
   return norm
 
 
 def resize_image(
     image: Image.Image,
     longest_side: int,
-    resample: int = Image.NEAREST,
+    resample: int = Image.Resampling.NEAREST,
 ) -> Image.Image:
   """Resize an image, preserving its aspect ratio."""
   resize_factor = longest_side / max(image.size)
   new_size = tuple(round(s * resize_factor) for s in image.size)
   return image.resize(new_size, resample)
 
 
 def trajectory_to_images(
     trajectory: grids.Array,
     compute_norm_fn: NormFn = quantile_normalize_fn,
-    cmap: mpl.colors.ListedColormap = sns.cm.icefire,
+    cmap: mpl.colors.ListedColormap = sns.cm.icefire,  # pytype: disable=module-attr
     longest_side: Optional[int] = None,
 ) -> List[Image.Image]:
   """Converts scalar trajectory with leading time axis into a list of images."""
   images = []
   for i, image_data in enumerate(trajectory):
     norm = compute_norm_fn(image_data, i)
     mappable = cm.ScalarMappable(norm=norm, cmap=cmap)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/data/visualization_test.py` & `jax_cfd-0.2.1/jax_cfd/data/visualization_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/data/xarray_utils.py` & `jax_cfd-0.2.1/jax_cfd/data/xarray_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 XR_SPATIAL_DIMS = ('x', 'y', 'z')
 XR_WAVENUMBER_DIMS = ('kx', 'ky', 'kz')
 XR_SAMPLE_NAME = 'sample'
 XR_TIME_NAME = 'time'
 XR_OFFSET_NAME = 'offset'
 
 XR_SAVE_GRID_SIZE_ATTR_NAME = 'save_grid_size'
+XR_SAVE_GRID_SIZE_ATTR_NAME_RECTANGLE = ('save_grid_size_x', 'save_grid_size_y')
+
 XR_DOMAIN_SIZE_NAME = 'domain_size'
 XR_NDIM_ATTR_NAME = 'ndim'
 XR_STABLE_TIME_STEP_ATTR_NAME = 'stable_time_step'
 
 
 def velocity_trajectory_to_xarray(
     trajectory: Tuple[Union[Array, GridArray, GridVariable], ...],
@@ -71,31 +73,33 @@
   if grid is not None:
     dimension = grid.ndim
   dims = (((XR_SAMPLE_NAME,) if samples else ())
           + (XR_TIME_NAME,)
           + XR_SPATIAL_DIMS[:dimension])
 
   data_vars = {}
-  for component in range(dimension):
-    name = XR_VELOCITY_NAMES[component]
+  num_scalars = len(trajectory) - dimension
+
+  for component in range(num_scalars):
+    name = XR_SCALAR_NAMES[component]
     data = trajectory[component]
+    var_attrs = {}
     if isinstance(data, GridArray) or isinstance(data, GridVariable):
+      var_attrs[XR_OFFSET_NAME] = data.offset
       data = data.data
-    var_attrs = {}
-    if grid is not None:
-      var_attrs[XR_OFFSET_NAME] = grid.cell_faces[component]
     data_vars[prefix_name + name] = xarray.Variable(dims, data, var_attrs)
 
-  for component in range(dimension, len(trajectory)):
-    name = XR_SCALAR_NAMES[component - dimension]
-    data = trajectory[component]
-    var_attrs = {}
+  for component in range(dimension):
+    name = XR_VELOCITY_NAMES[component]
+    data = trajectory[component + num_scalars]
     if isinstance(data, GridArray) or isinstance(data, GridVariable):
-      var_attrs[XR_OFFSET_NAME] = data.offset
       data = data.data
+    var_attrs = {}
+    if grid is not None:
+      var_attrs[XR_OFFSET_NAME] = grid.cell_faces[component]
     data_vars[prefix_name + name] = xarray.Variable(dims, data, var_attrs)
 
   if samples:
     num_samples = next(iter(data_vars.values())).shape[0]
     sample_ids = np.arange(num_samples)
   else:
     sample_ids = None
@@ -119,27 +123,35 @@
   if sample_ids is not None:
     coords[XR_SAMPLE_NAME] = sample_ids
   return coords
 
 
 def grid_from_attrs(dataset_attrs) -> grids.Grid:
   """Constructs a `Grid` object from dataset attributes."""
-  grid_size = dataset_attrs[XR_SAVE_GRID_SIZE_ATTR_NAME]
   ndim = dataset_attrs[XR_NDIM_ATTR_NAME]
-  grid_shape = (grid_size,) * ndim
-  if XR_DOMAIN_SIZE_NAME in dataset_attrs:
-    domain_size = dataset_attrs[XR_DOMAIN_SIZE_NAME]
-  elif 'domain_size_multiple' in dataset_attrs:
-    # TODO(shoyer): remove this legacy case, once we no longer use datasets
-    # generated prior to 2020-09-18
-    domain_size = 2 * np.pi * dataset_attrs['domain_size_multiple']
+  if XR_SAVE_GRID_SIZE_ATTR_NAME in dataset_attrs:
+    grid_size = dataset_attrs[XR_SAVE_GRID_SIZE_ATTR_NAME]
+    grid_shape = (grid_size,) * ndim
+    if XR_DOMAIN_SIZE_NAME in dataset_attrs:
+      domain_size = dataset_attrs[XR_DOMAIN_SIZE_NAME]
+    elif 'domain_size_multiple' in dataset_attrs:
+      # TODO(shoyer): remove this legacy case, once we no longer use datasets
+      # generated prior to 2020-09-18
+      domain_size = 2 * np.pi * dataset_attrs['domain_size_multiple']
+    else:
+      raise ValueError(
+          f'could not figure out domain size from attrs:\n{dataset_attrs}')
+    grid_domain = [(0, domain_size)] * ndim
   else:
-    raise ValueError(
-        f'could not figure out domain size from attrs:\n{dataset_attrs}')
-  grid_domain = [(0, domain_size)] * ndim
+    grid_shape = tuple(dataset_attrs[attr]
+                       for attr in XR_SAVE_GRID_SIZE_ATTR_NAME_RECTANGLE[:ndim])
+    aspect_ratio = dataset_attrs['aspect_ratio']
+    domain_z = (0, 1)
+    domain_x = (0, aspect_ratio)
+    grid_domain = (domain_x, domain_z)
   grid = grids.Grid(grid_shape, domain=grid_domain)
   return grid
 
 
 def vorticity_2d(ds: xarray.Dataset) -> xarray.DataArray:
   """Calculate vorticity on a 2D dataset."""
   # Vorticity is calculated from staggered velocities at offset=(1, 1).
```

### Comparing `jax-cfd-0.2.0/jax_cfd/data/xarray_utils_test.py` & `jax_cfd-0.2.1/jax_cfd/data/xarray_utils_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,16 @@
       dict(all_dims=('x', 'y', 'z', 'sample'), state_dims=('x', 'z', 'y'),),
       dict(all_dims=('time', 'x'), state_dims=('x'),),
       dict(all_dims=('x', 'sample', 'y'), state_dims=('x', 'y'),),
       dict(all_dims=('x', 'z', 'y'), state_dims=('x', 'y', 'z'),),
   )
   def test_normalize(self, all_dims, state_dims):
     """Tests that `normalize` returns data with expected shapes and norms."""
+    self.skipTest("test is sensitive to its random seed")
+
     shape_key, value_key = jax.random.split(jax.random.PRNGKey(42), 2)
     input_shape = jax.random.randint(shape_key, (len(all_dims),), 1, 4)
     inputs = jax.random.normal(value_key, input_shape)
 
     non_state_dims = [dim for dim in all_dims if dim not in state_dims]
     get_dim_axis_fn = lambda dim: np.where(np.asarray(all_dims) == dim)[0][0]
     state_axes = [get_dim_axis_fn(dim) for dim in state_dims]
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/__init__.py` & `jax_cfd-0.2.1/jax_cfd/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/advections.py` & `jax_cfd-0.2.1/jax_cfd/ml/advections.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/decoders.py` & `jax_cfd-0.2.1/jax_cfd/ml/decoders.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/diffusions.py` & `jax_cfd-0.2.1/jax_cfd/ml/diffusions.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/encoders.py` & `jax_cfd-0.2.1/jax_cfd/ml/encoders.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,24 +28,31 @@
 def aligned_array_encoder(
     grid: grids.Grid,
     dt: float,
     physics_specs: physics_specifications.BasePhysicsSpecs,
     data_offsets: Optional[Tuple[Tuple[float, ...], ...]] = None,
 ) -> EncodeFn:
   """Generates encoder that wraps last data slice as GridVariables."""
-  del dt, physics_specs  # unused.
-  data_offsets = data_offsets or grid.cell_faces
+  del dt  # unused.
+  if hasattr(physics_specs, 'combo_offsets'):
+    data_offsets = physics_specs.combo_offsets()
+  else:
+    data_offsets = data_offsets or grid.cell_faces
   slice_last_fn = lambda x: array_utils.slice_along_axis(x, 0, -1)
 
-  # TODO(pnorgaard) Make the encoder/decoder/network register for BC
   def encode_fn(inputs):
-    bc = boundaries.periodic_boundary_conditions(grid.ndim)
+    if hasattr(physics_specs, 'combo_boundaries'):
+      bcs = physics_specs.combo_boundaries()
+    else:
+      bcs = tuple(
+          boundaries.periodic_boundary_conditions(grid.ndim)
+          for _ in range(len(inputs)))
     return tuple(
-        grids.GridVariable(grids.GridArray(slice_last_fn(x), offset, grid), bc)
-        for x, offset in zip(inputs, data_offsets))
+        bc.impose_bc(grids.GridArray(slice_last_fn(x), offset, grid))
+        for x, offset, bc in zip(inputs, data_offsets, bcs))
 
   return encode_fn
 
 
 @gin.register
 def collocated_to_staggered_encoder(
     grid: grids.Grid,
@@ -251,7 +258,8 @@
     u, v = slice_last_fn(u), slice_last_fn(v)
     uhat, vhat = jnp.fft.rfft2(u), jnp.fft.rfft2(v)
     kx, ky = grid.rfft_mesh()
     vorticity = 2j * jnp.pi * (vhat * kx - uhat * ky)
     return vorticity
 
   return encode_fn
+
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/equations.py` & `jax_cfd-0.2.1/jax_cfd/ml/equations.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/equations_test.py` & `jax_cfd-0.2.1/jax_cfd/ml/equations_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,8 +289,11 @@
     ]
     inputs, outputs = self._generate_inputs_and_outputs(config, grid)
     for u_input, u_output in zip(inputs, outputs):
       self.assertEqual(u_input.shape, u_output.shape)
 
 
 if __name__ == '__main__':
+  # Temporarily disable async dispatch on JAX CPU due to tsan error.
+  jax.config.update('jax_cpu_enable_async_dispatch', False)
+
   absltest.main()
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/forcings.py` & `jax_cfd-0.2.1/jax_cfd/ml/forcings.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/interpolations.py` & `jax_cfd-0.2.1/jax_cfd/ml/interpolations.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/layers.py` & `jax_cfd-0.2.1/jax_cfd/ml/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,23 @@
     Any, Callable, Dict, Optional, Sequence, Tuple, TypeVar, Union,
 )
 
 import haiku as hk
 import jax
 from jax import lax
 import jax.numpy as jnp
+from jax_cfd.base import array_utils
+from jax_cfd.base import boundaries
+from jax_cfd.base import grids
 from jax_cfd.ml import layers_util
 from jax_cfd.ml import tiling
 import numpy as np
 import scipy.linalg
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 IntOrSequence = Union[int, Sequence[int]]
 
 
 class PeriodicConvGeneral(hk.Module):
   """General periodic convolution module."""
 
   def __init__(
@@ -131,14 +134,91 @@
         rate=rate,
         tile_layout=tile_layout,
         name=name,
         **conv_kwargs
     )
 
 
+class MirrorConvGeneral(hk.Module):
+  """General periodic convolution module."""
+
+  def __init__(self,
+               base_convolution: Callable[..., Any],
+               output_channels: int,
+               kernel_shape: Tuple[int, ...],
+               rate: int = 1,
+               tile_layout: Optional[Tuple[int, ...]] = None,
+               name: str = 'mirror_conv_general',
+               **conv_kwargs: Any):
+    """Constructs MirrorConvGeneral module.
+
+    We use `VALID` padding on `base_convolution` and explicit padding beyond
+    the boudaries. This function computes paddings` and combines `jnp.pad` 
+    function calls with `base_convolution` module.
+
+    Args:
+      base_convolution: standard convolution module e.g. hk.Conv1D.
+      output_channels: number of output channels.
+      kernel_shape: shape of the kernel, compatible with `base_convolution`.
+      rate: dilation rate of the convolution.
+      tile_layout: optional layout for tiling spatial dimensions in a batch.
+      name: name of the module.
+      **conv_kwargs: additional arguments passed to `base_convolution`.
+    """
+    super().__init__(name=name)
+    self._padding = np.zeros(2).astype('int')
+    for kernel_size in kernel_shape:
+      effective_kernel = kernel_size + (rate - 1) * (kernel_size - 1)
+      pad_left = effective_kernel // 2
+      self._padding += np.array([pad_left,
+                                 effective_kernel - pad_left - 1]).astype('int')
+    self._tile_layout = tile_layout
+    self._conv_module = base_convolution(
+        output_channels=output_channels, kernel_shape=kernel_shape,
+        padding='VALID', rate=rate, **conv_kwargs)
+
+  def _expand_var(self, var):
+    var = var.bc.pad_all(
+        var, (self._padding,) * var.grid.ndim, mode=boundaries.Padding.MIRROR)
+    return jnp.expand_dims(var.data, axis=-1)
+
+  def __call__(self, inputs):
+    input_data = tuple(self._expand_var(var) for var in inputs)
+    input_data = array_utils.concat_along_axis(
+        jax.tree_leaves(input_data), axis=-1)
+    outputs = self._conv_module(input_data)
+    outputs = array_utils.split_axis(outputs, -1)
+    outputs = tuple(
+        var_input.bc.impose_bc(
+            grids.GridArray(var, var_input.offset, var_input.grid))
+        for var, var_input in zip(outputs, inputs))
+    return outputs
+
+
+class MirrorConv2D(MirrorConvGeneral):
+  """Mirror convolution module in 2D."""
+
+  def __init__(self,
+               output_channels: int,
+               kernel_shape: Tuple[int, int],
+               rate: int = 1,
+               tile_layout: Optional[Tuple[int, int]] = None,
+               name='mirror_conv_2d',
+               **conv_kwargs):
+    """Constructs MirrorConv2D module."""
+    super().__init__(
+        base_convolution=hk.Conv2D,
+        output_channels=output_channels,
+        kernel_shape=kernel_shape,
+        rate=rate,
+        tile_layout=tile_layout,
+        name=name,
+        **conv_kwargs)
+
+
 class PeriodicConvTransposeGeneral(hk.Module):
   """General periodic transpose convolution module."""
 
   def __init__(
       self,
       base_convolution: Callable[..., Any],
       output_channels: int,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/layers_test.py` & `jax_cfd-0.2.1/jax_cfd/ml/layers_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/layers_util.py` & `jax_cfd-0.2.1/jax_cfd/ml/layers_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from typing import Iterator, Optional, Sequence, Tuple, Union
 
 import jax
 from jax import lax
 import jax.numpy as jnp
 from jax_cfd.ml import tiling
 import numpy as np
-import scipy
+import scipy.special
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 
 
 class Method(enum.Enum):
   """Discretization method."""
   FINITE_DIFFERENCE = 1
   FINITE_VOLUME = 2
 
@@ -329,15 +329,15 @@
 
 
 # Caching the result of _patch_kernel() ensures that only one constant value is
 # used as a side-input into JAX's jit/pmap. This ensures that XLA's Common
 # Subexpression Elimination (CSE) pass can consolidate calls to extract patches
 # on the same array.
 @functools.lru_cache()
-def _patch_kernel(
+def _patch_kernel(  # pytype: disable=annotation-type-mismatch  # numpy-scalars
     patch_shape: Tuple[int, ...],
     dtype: np.dtype = np.float32
 ) -> np.ndarray:
   """Returns a convolutional kernel that extracts patches."""
   patch_size = np.prod(patch_shape)
   kernel_2d = np.eye(patch_size, dtype=dtype)
   kernel_shape = (patch_size, 1) + patch_shape
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/layers_util_test.py` & `jax_cfd-0.2.1/jax_cfd/ml/layers_util_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/metrics.py` & `jax_cfd-0.2.1/jax_cfd/ml/metrics.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/model_builder.py` & `jax_cfd-0.2.1/jax_cfd/ml/model_builder.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/model_utils.py` & `jax_cfd-0.2.1/jax_cfd/ml/model_utils.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/networks.py` & `jax_cfd-0.2.1/jax_cfd/ml/networks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Network modules that interface with numerical methods."""
 
+import functools
 import itertools
 from typing import Callable, Optional, Tuple
 
 import gin
 import haiku as hk
 import jax
 import jax.numpy as jnp
 from jax_cfd.base import array_utils
 from jax_cfd.base import boundaries
 from jax_cfd.base import finite_differences
 from jax_cfd.base import grids
+from jax_cfd.base import interpolation
 from jax_cfd.ml import physics_specifications
 from jax_cfd.ml import towers
 import numpy as np
 
 
 def _identity(grid, dt, physics_specs):
   del grid, dt, physics_specs  # unused.
@@ -22,26 +24,64 @@
 
 
 @gin.register
 def split_to_aligned_field(
     grid: grids.Grid,
     dt: float,
     physics_specs: physics_specifications.BasePhysicsSpecs,
-    data_offsets: Optional[Tuple[Tuple[float, ...], ...]] = None,
+    network_offsets: Optional[Tuple[Tuple[float, float], ...]] = None,
 ):
   """Returns module that splits inputs along last axis into GridArrayVector."""
-  del dt, physics_specs  # unused.
-  data_offsets = data_offsets or grid.cell_faces
-
+  del dt  # unused.
+  if hasattr(physics_specs, "combo_offsets"):
+    data_offsets = physics_specs.combo_offsets()
+  else:
+    data_offsets = grid.cell_faces
+
+  if hasattr(physics_specs, "combo_boundaries"):
+    boundary_conditions = physics_specs.combo_boundaries()
+  else:
+    boundary_conditions = tuple(
+        boundaries.periodic_boundary_conditions(grid.ndim)
+        for _ in range(grid.ndim))
+  network_offsets = network_offsets or data_offsets
   def process(inputs):
     split_inputs = array_utils.split_axis(inputs, -1)
-    # TODO(pnorgaard) Make the encoder/decoder/network configurable for BC
-    bc = boundaries.periodic_boundary_conditions(grid.ndim)
-    return tuple(grids.GridVariable(grids.GridArray(x, offset, grid), bc)
-                 for x, offset in zip(split_inputs, data_offsets))
+    output = tuple(
+        grids.GridVariable(grids.GridArray(x, offset, grid), bc) for x, offset,
+        bc in zip(split_inputs, network_offsets, boundary_conditions))
+    output = tuple(
+        interpolation.linear(x, offset)
+        for x, offset in zip(output, data_offsets))
+    return output
+  return hk.to_module(process)()
+
+
+@gin.configurable()
+def interpolate_gridvar(
+    grid: grids.Grid,
+    dt: float,
+    physics_specs: physics_specifications.BasePhysicsSpecs,
+    final_offsets: Optional[Tuple[Tuple[float, float], ...]] = None,
+    process_fn: Optional[Callable] = lambda x: x,  # pylint: disable=g-bare-generic
+):
+  """Returns module that splits inputs along last axis into GridArrayVector."""
+  del dt  # unused.
+  if hasattr(physics_specs, "combo_offsets"):
+    data_offsets = physics_specs.combo_offsets()
+  else:
+    data_offsets = grid.cell_faces
+  final_offsets = final_offsets or data_offsets
+
+  def process(inputs):
+    inputs = process_fn(inputs)
+    inputs = tuple(
+        interpolation.linear(x, offset)
+        for x, offset in zip(inputs, final_offsets))
+    return inputs
 
   return hk.to_module(process)()
 
 
 @gin.register
 def aligned_field_from_split_divergence(
     grid: grids.Grid,
@@ -120,15 +160,15 @@
   def process(inputs):
     inputs = tuple(jnp.expand_dims(x.data, axis=-1) for x in inputs)
     return array_utils.concat_along_axis(jax.tree_leaves(inputs), axis=-1)
 
   return hk.to_module(process)()
 
 
-@gin.register
+@gin.configurable
 def tower_module(
     grid: grids.Grid,
     dt: float,
     physics_specs: physics_specifications.BasePhysicsSpecs,
     tower_factory: towers.TowerFactory,
     pre_process_module: Callable = _identity,  # pylint: disable=g-bare-generic
     post_process_module: Callable = _identity,  # pylint: disable=g-bare-generic
@@ -146,14 +186,36 @@
     else:
       network = tower_factory(num_output_channels, grid.ndim)
     return post_process(network(x))
 
   return hk.to_module(forward_pass)(name=name)
 
 
+@gin.configurable
+def velocity_corrector_network_w_boundaries(
+    grid: grids.Grid,
+    dt: float,
+    physics_specs: physics_specifications.BasePhysicsSpecs,
+    tower_factory: towers.TowerFactory,
+    network_offsets: Tuple[Tuple[float, ...], ...],
+    num_output_channels: int,
+    name: Optional[str] = None,
+    process_fn: Optional[Callable] = _identity,  # pylint: disable=g-bare-generic
+):
+  """Returns a module that computes corrections to the velocity field."""
+  pre_process = functools.partial(
+      interpolate_gridvar, final_offsets=network_offsets, process_fn=process_fn)
+  post_process = interpolate_gridvar
+  return tower_module(
+      grid=grid, dt=dt, physics_specs=physics_specs,
+      tower_factory=tower_factory, pre_process_module=pre_process,
+      post_process_module=post_process, num_output_channels=num_output_channels,
+      name=name)
+
+
 @gin.register
 def velocity_corrector_network(
     grid: grids.Grid,
     dt: float,
     physics_specs: physics_specifications.BasePhysicsSpecs,
     tower_factory: towers.TowerFactory,
     name: Optional[str] = None,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/optimizer_modules.py` & `jax_cfd-0.2.1/jax_cfd/ml/optimizer_modules.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/physics_specifications.py` & `jax_cfd-0.2.1/jax_cfd/ml/physics_specifications.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/pressures.py` & `jax_cfd-0.2.1/jax_cfd/ml/pressures.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/tiling.py` & `jax_cfd-0.2.1/jax_cfd/ml/tiling.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/time_integrators.py` & `jax_cfd-0.2.1/jax_cfd/ml/time_integrators.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/towers.py` & `jax_cfd-0.2.1/jax_cfd/ml/towers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Definitions of towers (neural networks based on multioke CNN layers)."""
 
 import functools
 from typing import Any, Callable, List, Optional, Tuple, Union
 import gin
+import jax
 import haiku as hk
 
 from jax_cfd.ml import layers
 from jax_cfd.ml import nonlinearities
 
 Array = layers.Array
 ConvModule = Callable[..., Any]
@@ -48,22 +49,44 @@
   if rate is not None and rate != 1:
     raise ValueError('transpose convolutions do not support dilation rate')
   return PERIODIC_CONV_TRANSPOSE_MODULES[ndim](
       output_channels, kernel_shape, **kwargs)
 
 
 @gin.register
-def fixed_scale(
+def mirror_convolution(
+    output_channels: int,
+    kernel_shape: Tuple[int, ...],
+    ndim: int,
+    **kwargs
+):
+  """Returns MirrorConv2D module with specified parameters."""
+  del ndim
+  return layers.MirrorConv2D(
+      output_channels, kernel_shape, **kwargs)
+
+
+@gin.register
+def fixed_scale(inputs: Array,
+                axes: Tuple[int, ...],
+                rescaled_one: float = gin.REQUIRED) -> Array:
+  """Linearly scales `inputs` such that `1` maps to `rescaled_one`."""
+  del axes  # unused.
+  return inputs * rescaled_one
+
+
+@gin.register
+def fixed_scale_gridvar(
     inputs: Array,
     axes: Tuple[int, ...],
     rescaled_one: float = gin.REQUIRED
 ) ->Array:
   """Linearly scales `inputs` such that `1` maps to `rescaled_one`."""
   del axes  # unused.
-  return inputs * rescaled_one
+  return tuple(x.bc.impose_bc(x.array * rescaled_one) for x in inputs)  # pytype: disable=bad-return-type  # jax-devicearray
 
 
 @gin.register
 def scale_to_range(
     inputs: Array,
     axes: Tuple[int, ...],
     min_value: float = gin.REQUIRED,
@@ -237,15 +260,15 @@
       components.append(nonlinearity)
     components.append(conv_module(num_output_channels, output_kernel_shape,
                                   ndim, rate=output_rate, stride=output_stride))
     components.append(functools.partial(output_scale_fn, axes=ndim_axes))
     return hk.Sequential(components)(inputs)
 
   module = hk.to_module(forward_pass)(name=name)
-  return hk.experimental.named_call(module, name=name)
+  return jax.named_call(module, name=name)
 
 
 @gin.register
 def residual_block_tower_factory(
     num_output_channels: int,
     ndim: int,
     num_blocks: int = 2,
@@ -262,15 +285,15 @@
       skip = skip_connection_fn(inputs, block_num)
       block = block_factory(skip.shape[-1], ndim)
       inputs = skip + block(inputs)
     last_block = block_factory(num_output_channels, ndim)
     return output_scale_fn(last_block(inputs), list(range(ndim)))
 
   module = hk.to_module(forward_pass)(name=name)
-  return hk.experimental.named_call(module, name=name)
+  return jax.named_call(module, name=name)
 
 
 @gin.register
 def residual_connection(*args, module_factory, **kwargs):
   """Apply module_factory() as a residual correction to inputs."""
   def forward_pass(inputs):
     return inputs + module_factory(*args, **kwargs)(inputs)
```

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/towers_test.py` & `jax_cfd-0.2.1/jax_cfd/ml/towers_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/train_utils.py` & `jax_cfd-0.2.1/jax_cfd/ml/train_utils.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/ml/viscosities.py` & `jax_cfd-0.2.1/jax_cfd/ml/viscosities.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from jax_cfd.base import grids
 from jax_cfd.base import subgrid_models
 from jax_cfd.ml import interpolations
 from jax_cfd.ml import physics_specifications
 from jax_cfd.ml import towers
 import numpy as np
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 GridArray = grids.GridArray
 GridArrayVector = grids.GridArrayVector
 GridVariableVector = grids.GridVariableVector
 InterpolationModule = interpolations.InterpolationModule
 ViscosityFn = Callable[[grids.GridArrayTensor, GridArrayVector, grids.Grid],
                        grids.GridArrayTensor]
 ViscosityModule = Callable[..., ViscosityFn]
@@ -89,15 +89,15 @@
     viscosity_net = tower_factory(1, grid.ndim)
     inputs = jnp.stack([u.data for u in v], axis=-1)
     predicted_viscosity = (viscosity_scale + 1e-6) * viscosity_net(inputs)
     predicted_viscosity = grids.GridArray(
         data=jnp.squeeze(predicted_viscosity, -1),
         offset=grid.cell_center, grid=grid)
     interpolated_viscosities = {
-        offset: interpolate(predicted_viscosity, offset, v, dt)
+        offset: interpolate(predicted_viscosity, offset, v, dt)  # pytype: disable=wrong-arg-types  # always-use-return-annotations
         for offset in unique_offsets}
     viscosities = [interpolated_viscosities[offset] for offset in s_ij_offsets]
     tree_def = jax.tree_util.tree_structure(s_ij)
     return jax.tree_unflatten(tree_def, [x.data for x in viscosities])
 
   return hk.to_module(viscosity_fn)()
 
@@ -143,23 +143,23 @@
       tensor containing values of the eddy viscosity at the same grid offsets
       as the strain tensor `s_ij`.
     """
     s_ij_offsets = [array.offset for array in s_ij.ravel()]
     unique_offsets = list(set(s_ij_offsets))
     viscosity_net = tower_factory(1, grid.ndim)
     cell_center = grid.cell_center
-    interpolate_to_center = lambda x: interpolate(x, cell_center, v, dt)
+    interpolate_to_center = lambda x: interpolate(x, cell_center, v, dt)  # pytype: disable=wrong-arg-types
     centered_s_ij = np.vectorize(interpolate_to_center)(s_ij)
     inputs = jnp.stack([array.data for array in centered_s_ij.ravel()], axis=-1)
     predicted_viscosity = (viscosity_scale + 1e-6) * viscosity_net(inputs)
     predicted_viscosity = grids.GridArray(
         data=jnp.squeeze(predicted_viscosity, -1),
         offset=grid.cell_center, grid=grid)
     interpolated_viscosities = {
-        offset: interpolate(predicted_viscosity, offset, v, dt)
+        offset: interpolate(predicted_viscosity, offset, v, dt)  # pytype: disable=wrong-arg-types  # always-use-return-annotations
         for offset in unique_offsets}
     viscosities = [interpolated_viscosities[offset] for offset in s_ij_offsets]
     tree_def = jax.tree_util.tree_structure(s_ij)
     return jax.tree_unflatten(tree_def, [x.data for x in viscosities])
 
   return hk.to_module(viscosity_fn)()
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/__init__.py` & `jax_cfd-0.2.1/jax_cfd/spectral/__init__.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/equations.py` & `jax_cfd-0.2.1/jax_cfd/spectral/equations.py`

 * *Files 5% similar despite different names*

```diff
@@ -214,7 +214,44 @@
       grid, k=wave_number, offsets=offsets)
   return NavierStokes2D(
       viscosity,
       grid,
       drag=0.1,
       smooth=smooth,
       forcing_fn=forcing_fn)
+
+
+@dataclasses.dataclass
+class NonlinearSchrodinger(time_stepping.ImplicitExplicitODE):
+  """Nonlinear schrodinger equation split in implicit and explicit parts.
+
+  The NLS equation is
+    `psi_t = -i psi_xx/8 - i|psi|^2 psi/2`
+
+  Attributes:
+    grid: underlying grid of the process
+    smooth: smooth the non-linear by upsampling 2x in fourier and truncating
+  """
+  grid: grids.Grid
+  smooth: bool = True
+
+  def __post_init__(self):
+    self.kx, = self.grid.fft_axes()
+    assert len(self.kx) % 2 == 0, "Odd grid sizes not supported, try N even"
+    self.two_pi_i_k = 2j * jnp.pi * self.kx
+    self.fft = spectral_utils.truncated_fft_2x if self.smooth else jnp.fft.fft
+    self.ifft = spectral_utils.padded_ifft_2x if self.smooth else jnp.fft.ifft
+
+  def explicit_terms(self, psihat):
+    """Non-linear part of the equation `-i|psi|^2 psi/2`."""
+    psi = self.ifft(psihat)
+    ipsi_cubed = 1j * psi * jnp.abs(psi)**2
+    ipsi_cubed_hat = self.fft(ipsi_cubed)
+    return -ipsi_cubed_hat / 2
+
+  def implicit_terms(self, psihat):
+    """The diffusion term `-i psi_xx/8` to be handled implicitly."""
+    return -1j * psihat * self.two_pi_i_k**2 / 8
+
+  def implicit_solve(self, psihat, time_step):
+    """Solves for `implicit_terms`, implicitly."""
+    return psihat / (1 - time_step * (-1j * self.two_pi_i_k**2 / 8))
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/equations_test.py` & `jax_cfd-0.2.1/jax_cfd/spectral/equations_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -161,14 +161,55 @@
     step_fn = time_stepping.crank_nicolson_rk2(eq, time_step)
     step_fn = cfd.funcutils.repeated(step_fn, num_steps)
     uhat0 = initial_condition_fn(grid)
     t0 = 0.0
     uhat1, _ = step_fn((uhat0, t0))
     self.assertFalse(jnp.isnan(uhat1).any())
 
+  def test_nls_equation(self):
+    """Check that trajectory matches Peregrine soliton analytic solution.
+
+    Soln from https://en.wikipedia.org/wiki/Peregrine_soliton,
+    however as we implement `psi_t = -i psi_xx/8 - i|psi|^2 psi/2`
+    rather than `psi_t = +i psi_xx/2 -+i|psi|^2 psi` from the wiki,
+    the solution needs to be rescaled and conjugated.
+    """
+
+    def solve_nls(u0, t_final=1., max_samples=1024, dt=1e-2, extent=500):
+      N = len(u0)  # pylint: disable=invalid-name
+      grid = grids.Grid((N,), domain=((-extent / 2, extent / 2),))
+      xs, = grid.axes(offset=(0,))
+      eq = spectral_equations.NonlinearSchrodinger(grid=grid)
+      stepfn = time_stepping.crank_nicolson_rk4(eq, dt)
+      uhat0 = jnp.fft.fft(u0)
+      numsteps = int(t_final / dt)
+      ds_period = max(numsteps // max_samples, 1)
+      multistepfn = jax.jit(cfd.funcutils.repeated(stepfn, ds_period))
+      _, uhat_traj = cfd.funcutils.trajectory(multistepfn, max_samples)(uhat0)
+      u_traj = jax.vmap(jnp.fft.ifft)(uhat_traj)
+      timesteps = (1 + jnp.arange(min(max_samples, numsteps))) * dt * ds_period
+      return u_traj, xs, timesteps
+
+    L = 40 * jnp.pi  # pylint: disable=invalid-name
+    grid = grids.Grid((2**10,), domain=((-L / 2, L / 2),))
+    dt = 3e-4
+    tau = 8
+    T = tau * 2  # pylint: disable=invalid-name
+    xs, = grid.axes(offset=(0,))
+    zs = xs * jnp.sqrt(2)
+    u0 = (4 * zs**2 - 3) / (1 + 4 * zs**2)
+    soln, x_ds, t_ds = solve_nls(u0, T, dt=dt, extent=L)
+    z_ds = x_ds * jnp.sqrt(2)
+    tau_ds = t_ds / 2
+    gt_soln = 1 - 4 * (1 +
+                       2j * tau_ds[:, None]) / (1 + 4 *
+                                                (z_ds**2 + tau_ds[:, None]**2))
+    gt_soln = jnp.conj(gt_soln * jnp.exp(1j * tau_ds[:, None]))
+    self.assertLess(jnp.abs(soln - gt_soln).mean(), 1e-3)
+
 
 class EquationsTest2D(test_util.TestCase):
 
   @parameterized.named_parameters(ALL_TIME_STEPPERS)
   def test_forced_turbulence(self, time_stepper):
     """Check that forced turbulence runs for 100 steps without blowing up."""
     grid = grids.Grid((128, 128), domain=((0, 2 * jnp.pi), (0, 2 * jnp.pi)))
@@ -269,15 +310,15 @@
           max_velocity=2.0,
           peak_wavenumber=4,
           seed=0,
           density=1.0,
           n_steps=500,
           grid_size=512,
           is_forced=False,
-          atol=0.07,
+          atol=0.09,
           ),
       dict(
           testcase_name='_forced_turbulence',
           viscosity=1e-2,
           cfl_safety_factor=.1,
           max_velocity=2.0,
           peak_wavenumber=4,
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/forcings.py` & `jax_cfd-0.2.1/jax_cfd/spectral/forcings.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/time_stepping.py` & `jax_cfd-0.2.1/jax_cfd/spectral/time_stepping.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/time_stepping_test.py` & `jax_cfd-0.2.1/jax_cfd/spectral/time_stepping_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 """Tests for time_stepping."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 import jax
 from jax import tree_util
-from jax.config import config
+from jax import config
 import jax.numpy as jnp
 from jax_cfd.base import funcutils
 from jax_cfd.spectral import time_stepping
 import numpy as np
 
 
 def harmonic_oscillator(x0, t):
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/types.py` & `jax_cfd-0.2.1/jax_cfd/spectral/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Common types that are used throughout the spectral codes."""
 
 from typing import Callable, Union
 
-import jax.numpy as jnp
+import jax
 import numpy as np
 
-Array = Union[np.ndarray, jnp.DeviceArray]
+Array = Union[np.ndarray, jax.Array]
 StepFn = Callable[[Array], Array]
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/utils.py` & `jax_cfd-0.2.1/jax_cfd/spectral/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -49,14 +49,50 @@
   n, = uhat.shape
   final_shape = int(3 / 2 * n)
   smoothed = jnp.pad(uhat, (0, final_shape - n))
   assert smoothed.shape == (final_shape,), "incorrect padded shape"
   return 1.5 * jnp.fft.irfft(smoothed)
 
 
+def truncated_fft_2x(u: spectral_types.Array) -> spectral_types.Array:
+  """Applies the 1/2 rule to complex u by truncating higher Fourier modes.
+
+  Args:
+    u: the (complex) input signal
+
+  Returns:
+    Downsampled version of `u` in fft-space.
+  """
+  uhat = jnp.fft.fftshift(jnp.fft.fft(u))
+  k, = uhat.shape
+  final_size = (k + 1) // 2
+  return jnp.fft.ifftshift(uhat[final_size // 2:(-final_size + 1) // 2]) / 2
+
+
+def padded_ifft_2x(uhat: spectral_types.Array) -> spectral_types.Array:
+  """Applies the 2x rule to complex F[u] by padding higher frequencies.
+
+     Pads with zeros in the Fourier domain before performing the ifft
+      (effectively performing 2x interpolation in the spatial domain)
+
+  Args:
+    uhat: the fft representation of signal
+
+  Returns:
+    An upsampled signal in real space interpolated to 2x more points than
+    `jax.fft.ifft(uhat)`.
+  """
+  n, = uhat.shape
+  final_size = n + 2 * (n // 2)
+  added = n // 2
+  smoothed = jnp.pad(jnp.fft.fftshift(uhat), (added, added))
+  assert smoothed.shape == (final_size,), "incorrect padded shape"
+  return 2 * jnp.fft.ifft(jnp.fft.ifftshift(smoothed))
+
+
 def circular_filter_2d(grid: grids.Grid) -> spectral_types.Array:
   """Circular filter which roughly matches the 2/3 rule but is smoother.
 
   Follows the technique described in Equation 1 of [1]. We use a different value
   for alpha as used by pyqg [2].
 
   Args:
@@ -87,18 +123,18 @@
   filter_ = jnp.exp(-filterfac * (circle - cphi)**4.)
   filter_ = jnp.where(circle <= cphi, jnp.ones_like(filter_), filter_)
   return filter_
 
 
 def brick_wall_filter_2d(grid: grids.Grid):
   """Implements the 2/3 rule."""
-  n, _ = grid.shape
-  filter_ = jnp.zeros((n, n // 2 + 1))
-  filter_ = filter_.at[:int(2 / 3 * n) // 2, :int(2 / 3 * (n // 2 + 1))].set(1)
-  filter_ = filter_.at[-int(2 / 3 * n) // 2:, :int(2 / 3 * (n // 2 + 1))].set(1)
+  n, m = grid.shape
+  filter_ = jnp.zeros((n, m // 2 + 1))
+  filter_ = filter_.at[:int(2 / 3 * n) // 2, :int(2 / 3 * (m // 2 + 1))].set(1)
+  filter_ = filter_.at[-int(2 / 3 * n) // 2:, :int(2 / 3 * (m // 2 + 1))].set(1)
   return filter_
 
 
 def exponential_filter(signal, alpha=1e-6, order=2):
   """Apply a low-pass smoothing filter to remove noise from 2D signal."""
   # Based on:
   # 1. Gottlieb and Hesthaven (2001), "Spectral methods for hyperbolic problems"
@@ -138,15 +174,15 @@
     Navier–Stokes turbulence, Computers & Fluids, Volume 33, Issue 4, 2004,
     Pages 509-520, ISSN 0045-7930,
     https://doi.org/10.1016/j.compfluid.2003.06.003.
   """
   kx, ky = grid.rfft_mesh()
   two_pi_i = 2 * jnp.pi * 1j
   laplace = two_pi_i ** 2 * (abs(kx)**2 + abs(ky)**2)
-  laplace = laplace.at[0, 0].set(1)
+  laplace = laplace.at[0, 0].set(1)  # pytype: disable=attribute-error  # jnp-type
 
   def ret(vorticity_hat):
     psi_hat = -1 / laplace * vorticity_hat
     vxhat = two_pi_i * ky * psi_hat
     vyhat = -two_pi_i * kx * psi_hat
     return vxhat, vyhat
```

### Comparing `jax-cfd-0.2.0/jax_cfd/spectral/utils_test.py` & `jax_cfd-0.2.1/jax_cfd/spectral/utils_test.py`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/jax_cfd.egg-info/SOURCES.txt` & `jax_cfd-0.2.1/jax_cfd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jax-cfd-0.2.0/setup.py` & `jax_cfd-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 base_requires = ['jax', 'numpy', 'scipy', 'tree-math']
 data_requires = ['matplotlib', 'seaborn', 'Pillow', 'xarray']
 ml_requires = ['dm-haiku', 'einops', 'gin-config']
 tests_requires = ['absl-py', 'pytest', 'pytest-xdist', 'scikit-image']
 
 setuptools.setup(
     name='jax-cfd',
-    version='0.2.0',
+    version='0.2.1',
     license='Apache 2.0',
     author='Google LLC',
     author_email='noreply@google.com',
     install_requires=base_requires,
     extras_require={
         'data': data_requires,
         'ml': ml_requires,
```

