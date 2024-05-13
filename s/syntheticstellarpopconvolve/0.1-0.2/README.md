# Comparing `tmp/syntheticstellarpopconvolve-0.1.tar.gz` & `tmp/syntheticstellarpopconvolve-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syntheticstellarpopconvolve-0.1.tar", last modified: Thu May  2 02:55:42 2024, max compression
+gzip compressed data, was "syntheticstellarpopconvolve-0.2.tar", last modified: Mon May 13 14:26:40 2024, max compression
```

## Comparing `syntheticstellarpopconvolve-0.1.tar` & `syntheticstellarpopconvolve-0.2.tar`

### file list

```diff
@@ -1,68 +1,72 @@
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-02 02:55:42.205412 syntheticstellarpopconvolve-0.1/
--rw-rw-r--   0 david     (1002) david     (1002)    32894 2024-04-28 22:36:09.000000 syntheticstellarpopconvolve-0.1/LICENSE
--rw-r--r--   0 david     (1002) david     (1002)     1491 2024-05-02 02:55:42.205412 syntheticstellarpopconvolve-0.1/PKG-INFO
--rw-rw-r--   0 david     (1002) david     (1002)      192 2024-05-01 00:20:21.000000 syntheticstellarpopconvolve-0.1/README.md
--rw-rw-r--   0 david     (1002) david     (1002)      668 2024-05-01 00:59:25.000000 syntheticstellarpopconvolve-0.1/pyproject.toml
--rw-rw-r--   0 david     (1002) david     (1002)       38 2024-05-02 02:55:42.205412 syntheticstellarpopconvolve-0.1/setup.cfg
--rw-rw-r--   0 david     (1002) david     (1002)     3045 2024-05-02 02:47:35.000000 syntheticstellarpopconvolve-0.1/setup.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-02 02:55:42.177413 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/
--rw-rw-r--   0 david     (1002) david     (1002)      881 2024-05-01 00:30:06.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/SFR_plotting_routine.py
--rw-rw-r--   0 david     (1002) david     (1002)      254 2024-05-01 03:16:01.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/__init__.py
--rw-rw-r--   0 david     (1002) david     (1002)    16607 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/archive.py
--rw-rw-r--   0 david     (1002) david     (1002)      987 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/check_convolution_input_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     2563 2024-05-02 02:45:50.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_calculate_birth_redshift_array.py
--rw-rw-r--   0 david     (1002) david     (1002)     9093 2024-04-28 23:05:08.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_check_config.py
--rw-rw-r--   0 david     (1002) david     (1002)    13885 2024-05-01 00:20:22.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_default_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)    14746 2024-05-01 00:30:23.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_general_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)     7060 2024-05-01 00:49:44.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_metallicity_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     5113 2024-05-01 00:30:47.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_sfr_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     2302 2024-04-28 23:05:49.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve.py
--rw-rw-r--   0 david     (1002) david     (1002)      868 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_custom_data.py
--rw-rw-r--   0 david     (1002) david     (1002)    40366 2024-05-01 00:26:49.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_ensembles.py
--rw-rw-r--   0 david     (1002) david     (1002)     3989 2024-05-01 00:26:20.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_events.py
--rw-rw-r--   0 david     (1002) david     (1002)    16860 2024-04-28 23:06:20.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_populations.py
--rw-rw-r--   0 david     (1002) david     (1002)     1508 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/cosmology_utils.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-02 02:55:42.201412 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/
--rw-rw-r--   0 david     (1002) david     (1002)    56408 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
--rw-rw-r--   0 david     (1002) david     (1002)  9053345 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_ensemble.json
--rw-rw-r--   0 david     (1002) david     (1002)   330384 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_population_settings.json
--rw-rw-r--   0 david     (1002) david     (1002)      730 2024-05-02 02:30:36.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/extract_population_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)    16579 2024-05-01 00:21:25.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/functions_to_review.py
--rw-rw-r--   0 david     (1002) david     (1002)      842 2024-05-01 00:20:24.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/prepare_output_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     5150 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/prepare_redshift_interpolator.py
--rw-rw-r--   0 david     (1002) david     (1002)     3074 2024-04-28 23:06:35.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/store_redshift_shell_info.py
--rw-rw-r--   0 david     (1002) david     (1002)     3338 2024-05-01 00:20:21.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/store_sfr_info.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-02 02:55:42.205412 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/
--rw-rw-r--   0 david     (1002) david     (1002)     3883 2024-05-02 02:47:03.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/main.py
--rw-rw-r--   0 david     (1002) david     (1002)      143 2024-04-30 23:58:15.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
--rw-rw-r--   0 david     (1002) david     (1002)     2170 2024-05-02 02:47:03.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_check_convolution_input_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     2419 2024-05-02 02:47:03.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_calculate_birth_redshift_array.py
--rw-rw-r--   0 david     (1002) david     (1002)    13401 2024-05-01 00:01:15.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_check_config.py
--rw-rw-r--   0 david     (1002) david     (1002)     3407 2024-05-01 00:38:24.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_default_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)    23069 2024-05-02 02:46:27.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_general_functions.py
--rw-rw-r--   0 david     (1002) david     (1002)      343 2024-05-01 00:41:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_metallicity_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)      314 2024-05-01 00:41:48.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_sfr_distributions.py
--rw-rw-r--   0 david     (1002) david     (1002)     5184 2024-05-01 00:41:53.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py
--rw-rw-r--   0 david     (1002) david     (1002)     4911 2024-05-01 00:42:32.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_with_events.py
--rw-rw-r--   0 david     (1002) david     (1002)      266 2024-05-01 00:42:38.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve.py
--rw-rw-r--   0 david     (1002) david     (1002)      875 2024-05-01 00:42:45.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py
--rw-rw-r--   0 david     (1002) david     (1002)    45297 2024-05-01 00:20:25.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py
--rw-rw-r--   0 david     (1002) david     (1002)    13230 2024-05-01 00:44:51.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_events.py
--rw-rw-r--   0 david     (1002) david     (1002)    16741 2024-05-01 00:45:29.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_populations.py
--rw-rw-r--   0 david     (1002) david     (1002)     8305 2024-05-02 02:30:45.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_cosmology_utils.py
--rw-rw-r--   0 david     (1002) david     (1002)     4288 2024-05-01 00:46:18.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_extract_population_settings.py
--rw-rw-r--   0 david     (1002) david     (1002)      142 2024-04-28 23:09:56.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_functions_to_review.py
--rw-rw-r--   0 david     (1002) david     (1002)     1616 2024-05-01 00:47:05.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_prepare_output_file.py
--rw-rw-r--   0 david     (1002) david     (1002)     6062 2024-05-01 00:47:49.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py
--rw-rw-r--   0 david     (1002) david     (1002)     4996 2024-05-01 00:48:31.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py
--rw-rw-r--   0 david     (1002) david     (1002)      284 2024-05-01 00:49:13.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_store_sfr_info.py
--rw-rw-r--   0 david     (1002) david     (1002)      126 2024-05-01 00:49:14.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_tmp.py
--rw-rw-r--   0 david     (1002) david     (1002)     2134 2024-05-01 00:49:38.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_update_convolution_config.py
--rw-rw-r--   0 david     (1002) david     (1002)      691 2024-04-28 23:05:37.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tmp.py
--rw-rw-r--   0 david     (1002) david     (1002)      566 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/update_convolution_config.py
-drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-02 02:55:42.205412 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/
--rw-r--r--   0 david     (1002) david     (1002)     1491 2024-05-02 02:55:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1002) david     (1002)     3394 2024-05-02 02:55:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1002) david     (1002)        1 2024-05-02 02:55:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1002) david     (1002)       70 2024-05-02 02:55:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/requires.txt
--rw-rw-r--   0 david     (1002) david     (1002)       28 2024-05-02 02:55:42.000000 syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/
+-rw-rw-r--   0 david     (1002) david     (1002)    32894 2024-04-28 22:36:09.000000 syntheticstellarpopconvolve-0.2/LICENSE
+-rw-rw-r--   0 david     (1002) david     (1002)      174 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/MANIFEST.in
+-rw-r--r--   0 david     (1002) david     (1002)     4181 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/PKG-INFO
+-rw-rw-r--   0 david     (1002) david     (1002)     2836 2024-05-05 23:07:49.000000 syntheticstellarpopconvolve-0.2/README.md
+-rw-rw-r--   0 david     (1002) david     (1002)      668 2024-05-01 00:59:25.000000 syntheticstellarpopconvolve-0.2/pyproject.toml
+-rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-03 12:39:25.000000 syntheticstellarpopconvolve-0.2/requirements.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       38 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/setup.cfg
+-rw-rw-r--   0 david     (1002) david     (1002)     3336 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/setup.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.620218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/
+-rw-rw-r--   0 david     (1002) david     (1002)      869 2024-05-05 16:27:07.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/SFR_plotting_routine.py
+-rw-rw-r--   0 david     (1002) david     (1002)      297 2024-05-13 14:23:10.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/__init__.py
+-rw-rw-r--   0 david     (1002) david     (1002)       20 2024-05-13 14:22:49.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/_version.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16607 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/archive.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2563 2024-05-02 02:45:50.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/calculate_birth_redshift_array.py
+-rw-rw-r--   0 david     (1002) david     (1002)     9660 2024-05-05 22:55:24.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)      978 2024-05-05 02:59:48.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_input_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2257 2024-05-05 03:19:16.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve.py
+-rw-rw-r--   0 david     (1002) david     (1002)      868 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_custom_data.py
+-rw-rw-r--   0 david     (1002) david     (1002)    46881 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_ensembles.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3977 2024-05-05 16:27:28.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16848 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_populations.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1508 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/cosmology_utils.py
+-rw-rw-r--   0 david     (1002) david     (1002)    19995 2024-05-05 21:26:05.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/default_convolution_config.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.628218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/
+-rw-rw-r--   0 david     (1002) david     (1002)    56408 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
+-rw-rw-r--   0 david     (1002) david     (1002)  9053345 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_ensemble.json
+-rw-rw-r--   0 david     (1002) david     (1002)   330384 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_population_settings.json
+-rw-rw-r--   0 david     (1002) david     (1002)      730 2024-05-02 02:30:36.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/extract_population_settings.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16579 2024-05-01 00:21:25.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/functions_to_review.py
+-rw-rw-r--   0 david     (1002) david     (1002)    14734 2024-05-05 03:08:05.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/general_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     7060 2024-05-01 00:49:44.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/metallicity_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)      830 2024-05-05 16:23:51.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_output_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5150 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_redshift_interpolator.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5113 2024-05-01 00:30:47.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/starformation_rate_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3053 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_redshift_shell_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3338 2024-05-01 00:20:21.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_sfr_info.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/
+-rw-rw-r--   0 david     (1002) david     (1002)       85 2024-05-01 00:02:02.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/generate_coverage_report.sh
+-rw-rw-r--   0 david     (1002) david     (1002)     3833 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/main.py
+-rw-rw-r--   0 david     (1002) david     (1002)      143 2024-04-30 23:58:15.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2377 2024-05-05 16:27:45.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py
+-rw-rw-r--   0 david     (1002) david     (1002)    13441 2024-05-05 22:55:24.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2013 2024-05-05 16:28:16.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_input_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)      307 2024-05-05 21:32:57.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_metallicity_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     5168 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4895 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)      254 2024-05-05 16:26:10.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve.py
+-rw-rw-r--   0 david     (1002) david     (1002)      863 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py
+-rw-rw-r--   0 david     (1002) david     (1002)    45263 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py
+-rw-rw-r--   0 david     (1002) david     (1002)    13212 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_events.py
+-rw-rw-r--   0 david     (1002) david     (1002)    16721 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_populations.py
+-rw-rw-r--   0 david     (1002) david     (1002)     8293 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_cosmology_utils.py
+-rw-rw-r--   0 david     (1002) david     (1002)     3389 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_default_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4272 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_extract_population_settings.py
+-rw-rw-r--   0 david     (1002) david     (1002)      142 2024-04-28 23:09:56.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_functions_to_review.py
+-rw-rw-r--   0 david     (1002) david     (1002)    23145 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_general_functions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     1600 2024-05-05 16:25:46.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_output_file.py
+-rw-rw-r--   0 david     (1002) david     (1002)     6042 2024-05-05 16:31:52.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py
+-rw-rw-r--   0 david     (1002) david     (1002)      318 2024-05-05 16:31:51.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_starformation_rate_distributions.py
+-rw-rw-r--   0 david     (1002) david     (1002)     4976 2024-05-05 16:28:50.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)      272 2024-05-05 16:28:42.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_sfr_info.py
+-rw-rw-r--   0 david     (1002) david     (1002)      126 2024-05-01 00:49:14.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_tmp.py
+-rw-rw-r--   0 david     (1002) david     (1002)     2118 2024-05-05 16:26:15.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_update_convolution_config.py
+-rw-rw-r--   0 david     (1002) david     (1002)      691 2024-04-28 23:05:37.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tmp.py
+-rw-rw-r--   0 david     (1002) david     (1002)      566 2024-04-28 22:33:30.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/update_convolution_config.py
+drwxrwxr-x   0 david     (1002) david     (1002)        0 2024-05-13 14:26:40.632218 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/
+-rw-r--r--   0 david     (1002) david     (1002)     4181 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1002) david     (1002)     3443 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1002) david     (1002)        1 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       86 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/requires.txt
+-rw-rw-r--   0 david     (1002) david     (1002)       28 2024-05-13 14:26:40.000000 syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/top_level.txt
```

### Comparing `syntheticstellarpopconvolve-0.1/LICENSE` & `syntheticstellarpopconvolve-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/pyproject.toml` & `syntheticstellarpopconvolve-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/setup.py` & `syntheticstellarpopconvolve-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,22 @@
 
 # Functions
 def version():
     """
     opens VERSION and returns version number
     """
 
-    with open("VERSION") as file:
-        return file.read().strip()
+    # with open("VERSION") as file:
+    #     return file.read().strip()
+
+    about = {}
+    with open("syntheticstellarpopconvolve/_version.py") as f:
+        exec(f.read(), about)
+
+    return about["__version__"]
 
 
 def readme():
     """
     Opens readme file and returns content
     """
 
@@ -78,27 +84,30 @@
         "population synthesis",
         "starformation rate history",
         "convolution",
     ],  # Keywords that define your package best
     packages=[
         "syntheticstellarpopconvolve",
         "syntheticstellarpopconvolve.tests",
+        "syntheticstellarpopconvolve.example_data",
     ],
-    package_data={
-        "": [
-            "example_data/*.dat",
-            "example_data/*.json",
-        ],
-        # "convolution": [
-        #     "example_data",
-        #     "example_data",
-        # ],
-    },
-    install_requires=requirements(this_file_dir),
+    # package_data={
+    #     "syntheticstellarpopconvolve": [
+    #         "example_data/*.dat",
+    #         "example_data/*.json",
+    #     ],
+    #     # "convolution": [
+    #     #     "example_data",
+    #     #     "example_data",
+    #     # ],
+    # },
+    # setup_requires=['pbr'],
+    # pbr=True,
     include_package_data=True,
+    install_requires=requirements(this_file_dir),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/SFR_plotting_routine.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/SFR_plotting_routine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Functionality to plot a starformation distribution
 """
 
-# from syntheticstellarpopconvolve.convolution_general_functions import (
+# from syntheticstellarpopconvolve.general_functions import (
 #     calculate_bincenters,
 # )
 
 # def plot_sfr(sfr_dict, fig=None, return_fig=False):  # DH0001
 #     """
 #     Function to plot a starformation distribution
 #     """
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/archive.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/archive.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/check_convolution_input_file.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_input_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Function to check the input file
 """
 
 import h5py
 
 
-def check_convolution_input_file(config):
+def check_input_file(config):
     """
-    TODO
+    TODO aa
     """
 
     #
     config["logger"].debug("Checking convolution input file")
 
     #
     input_file = h5py.File(config["input_filename"], "r")
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_calculate_birth_redshift_array.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/calculate_birth_redshift_array.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_check_config.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/check_convolution_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 TODO: handle logic of SFR
 """
 
 import astropy.units as u
 import voluptuous as vol
 
-from syntheticstellarpopconvolve.convolution_default_settings import (
-    convolution_options_defaults_dict,
+from syntheticstellarpopconvolve.default_convolution_config import (
+    default_convolution_config_dict,
 )
 
 
 def check_metallicity(convolution_instruction, data_key):
     """
     Function to check the metallicity
     """
@@ -40,29 +40,38 @@
     # Check if the correct time bins are present
     if time_type == "lookback_time":
         if "lookback_time_bin_edges" not in sfr_dict:
             raise ValueError(
                 "lookback_time_bin_edges is required in the sfr dictionary"
             )
 
+        # TODO: allow any time-type unit
         # check if has units
         if not sfr_dict["lookback_time_bin_edges"].unit == u.yr:
             raise ValueError(
                 "Please express 'lookback_time_bin_edges' in units of years (u.yr)"
             )
 
     elif time_type == "redshift":
         if "redshift_bin_edges" not in sfr_dict:
             raise ValueError("redshift_bin_edges is required in the sfr dictionary")
 
+        # TODO: check if
+
     ##########
     # Check if the correct time bins are present
     if "starformation_array" not in sfr_dict:
         raise ValueError("starformation_array is required in the sfr dictionary")
 
+    # check if starformation array has any unit
+    try:
+        sfr_dict["starformation_array"].unit
+    except AttributeError:
+        raise AttributeError("starformation_array requires an astropy unit")
+
     ##########
     # Check if the shape of the time_bin_edges is 1 smaller than the starformation array
 
     ##########
     # check if metallicity information is present
     if requires_metallicity_info:
         # Check if the metallicity bins are present
@@ -71,14 +80,22 @@
 
         # check if the MSSFR is present
         if "metallicity_weighted_starformation_array" not in sfr_dict:
             raise ValueError(
                 "metallicity_weighted_starformation_array is required in the sfr dictionary"
             )
 
+        # check if starformation array has any unit
+        try:
+            sfr_dict["metallicity_weighted_starformation_array"].unit
+        except AttributeError:
+            raise AttributeError(
+                "metallicity_weighted_starformation_array requires an astropy unit"
+            )
+
 
 def check_required(config, required_list):
     """
     Function to check if the keys in the required_list are present in the convolution_instruction dict
     """
 
     for key in required_list:
@@ -174,15 +191,15 @@
     if not config["check_convolution_config"]:
         return
 
     ##########
     # from the main dictionary, create a validation scheme
     validation_dict = {
         key: value["validation"]
-        for key, value in convolution_options_defaults_dict.items()
+        for key, value in default_convolution_config_dict.items()
         if "validation" in value
     }
     validation_schema = vol.Schema(validation_dict, extra=vol.ALLOW_EXTRA)
 
     ##########
     # do the validation: some parameters require others to be set,
     for parameter, parameter_dict in config.items():
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_general_functions.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/general_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import astropy.units as u
 import numpy as np
 import psutil
 from astropy.cosmology import Planck13 as cosmo  # Planck 2013
 from scipy import interpolate
 
-from syntheticstellarpopconvolve.convolution_calculate_birth_redshift_array import (
+from syntheticstellarpopconvolve.calculate_birth_redshift_array import (
     calculate_origin_redshift_array,
 )
 
 logger = logging.getLogger(__name__)
 
 
 def get_username():
@@ -229,15 +229,15 @@
     return extra_weights
 
 
 def calculate_origin_time_array(config, data_dict, convolution_time_bin_center):
     """
     Function to calculate the origin time array
 
-    TODO: more elsewhere
+    TODO: move elsewhere
     """
 
     config["logger"].debug("Calculating origin-time array")
 
     # if convolution method and SFR is the in lookback time, then we can just subtract
     if config["time_type"] == "lookback_time":
         origin_time_array = (
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_metallicity_distributions.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/metallicity_distributions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolution_sfr_distributions.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/starformation_rate_distributions.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 Main entry point to the convolution code. This code handles passing choosing the correct code to do the convolution with.
 
 TODO: make wrappers to handle timing logging to debug.
 TODO: allow usage of astropy units
 """
 
-from syntheticstellarpopconvolve.check_convolution_input_file import (
-    check_convolution_input_file,
-)
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
 )
+from syntheticstellarpopconvolve.check_input_file import check_input_file
 from syntheticstellarpopconvolve.convolve_populations import convolve_populations
 from syntheticstellarpopconvolve.extract_population_settings import (
     extract_population_settings,
 )
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 from syntheticstellarpopconvolve.prepare_redshift_interpolator import (
     prepare_redshift_interpolator,
@@ -43,15 +41,15 @@
 
     ###########
     # Update the config with some extra calculated stuff
     update_convolution_config(config=config)
 
     ###########
     # Check the input file
-    check_convolution_input_file(config=config)
+    check_input_file(config=config)
 
     ###########
     # Copy the input file and
     prepare_output_file(config=config)
 
     # ###########
     # # Calculate SFR information and add to hdf5 file
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_custom_data.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_custom_data.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_ensembles.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_ensembles.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,254 @@
 """
 Ensemble convolution functions
 
 TODO: put all the general ensemble files into the ensemble file
 TODO: allow the yield-rate and extra weights function to pass units to the ensemble and when
 stripping the end-points we should make sure to handle that properly.
+TODO: move the ensemble utils functions to a different place maybe.
 """
 
+import bz2
 import collections
 import copy
+import gzip
 import json
+import sys
+import time
 from collections import OrderedDict
 
 import astropy.units as u
 import h5py
+import msgpack
 import numpy as np
+import simplejson
+from halo import Halo
 
-from syntheticstellarpopconvolve.convolution_default_settings import (
+from syntheticstellarpopconvolve.default_convolution_config import (
     ALLOWED_NUMERICAL_TYPES,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import (
+from syntheticstellarpopconvolve.general_functions import (
     calculate_digitized_sfr_rates,
     calculate_edge_values,
     handle_custom_scaling_or_conversion,
     handle_extra_weights_function,
 )
 
 
+def ensemble_compression(filename):
+    """
+    Return the compression type of the ensemble file, based on its filename extension.
+    """
+
+    if filename.endswith(".bz2"):
+        return "bzip2"
+    if filename.endswith(".gz"):
+        return "gzip"
+    return None
+
+
+def open_ensemble(filename, encoding="utf-8"):
+    """
+    Function to open an ensemble at filename for reading and decompression if required.
+    """
+
+    compression = ensemble_compression(filename)
+    if ensemble_file_type(filename) == "msgpack":
+        flags = "rb"
+    else:
+        flags = "rt"
+    if compression == "bzip2":
+        file_object = bz2.open(filename, flags, encoding=encoding)
+    elif compression == "gzip":
+        file_object = gzip.open(filename, flags, encoding=encoding)
+    else:
+        file_object = open(filename, flags, encoding=encoding)
+    return file_object
+
+
+def keys_to_floats(input_dict: dict) -> dict:
+    """
+    Function to convert all the keys of the dictionary to float to float
+
+    we need to convert keys to floats:
+        this is ~ a factor 10 faster than David's ``recursive_change_key_to_float`` routine, probably because this version only does the float conversion, nothing else.
+
+    Args:
+        input_dict: dict of which we want to turn all the keys to float types if possible
+
+    Returns:
+        new_dict: dict of which the keys have been turned to float types where possible
+    """
+
+    # this adopts the type correctly *and* is fast
+    new_dict = type(input_dict)()
+
+    for k, v in input_dict.items():
+        # convert key to a float, if we can
+        # otherwise leave as is
+        try:
+            newkey = float(k)
+        except ValueError:
+            newkey = k
+
+        # act on value(s)
+        if isinstance(v, list):
+            # list data
+            new_dict[newkey] = [
+                (
+                    keys_to_floats(item)
+                    if isinstance(item, collections.abc.Mapping)
+                    else item
+                )
+                for item in v
+            ]
+        elif isinstance(v, collections.abc.Mapping):
+            # dict, ordereddict, etc. data
+            new_dict[newkey] = keys_to_floats(v)
+        else:
+            # assume all other data are scalars
+            new_dict[newkey] = v
+
+    return new_dict
+
+
+def ensemble_file_type(filename):
+    """
+    Returns the file type of an ensemble file.
+    """
+
+    if ".json" in filename:
+        filetype = "JSON"
+    elif ".msgpack" in filename:
+        filetype = "msgpack"
+    else:
+        filetype = None
+    return filetype
+
+
+def load_ensemble(
+    filename,
+    convert_float_keys=True,
+    select_keys=None,
+    timing=False,
+    flush=False,
+    quiet=False,
+):
+    """
+    Function to load an ensemeble file, even if it is compressed,
+    and return its contents to as a Python dictionary.
+
+    Args:
+        convert_float_keys : if True, converts strings to floats.
+        select_keys : a list of keys to be selected from the ensemble.
+    """
+
+    # open the file
+
+    # load with some info to the terminal
+    if not quiet:
+        print("Loading JSON...", flush=flush)
+
+    # open the ensemble and get the file type
+    file_object = open_ensemble(filename)
+    filetype = ensemble_file_type(filename)
+
+    if not filetype or not file_object:
+        print(
+            "Unknown filetype : your ensemble should be saved either as JSON or msgpack data.",
+            flush=flush,
+        )
+        sys.exit()
+
+    if quiet:
+        tstart = time.time()
+        if filetype == "JSON":
+            data = simplejson.load(file_object)
+            file_object.close()
+        elif filetype == "msgpack":
+            data = msgpack.load(file_object, object_hook=_hook)  # noqa: F821
+            file_object.close()
+        if timing:
+            print(
+                "\n\nTook {} s to load the data\n\n".format(time.time() - tstart),
+                flush=True,
+            )
+    else:
+        with Halo(text="Loading", interval=250, spinner="moon", color="yellow"):
+            tstart = time.time()
+            _loaded = False
+
+            def _hook(obj):
+                """
+                Hook to load ensemble
+                """
+
+                nonlocal _loaded
+                if not _loaded:
+                    _loaded = True
+                    print(
+                        "\nLoaded {} data, now putting in a dictionary".format(
+                            filetype
+                        ),
+                        flush=True,
+                    )
+                return obj
+
+            if filetype == "JSON":
+                # orjson promises to be fast, but it doesn't seem to be
+                # and fails on "Infinity"... oops
+                # data = orjson.loads(file_object.read())
+
+                # simplejson is faster than standard json and "just works"
+                # on the big Moe set in 37s
+                if not quiet:
+                    data = simplejson.load(file_object, object_hook=_hook)
+                else:
+                    data = simplejson.load(file_object)
+                file_object.close()
+
+                # standard json module
+                # on the big Moe set takes 42s
+                # data = json.load(file_object,
+                #                 object_hook=_hook)
+            elif filetype == "msgpack":
+                data = msgpack.load(file_object, object_hook=_hook)
+                file_object.close()
+
+            if timing:
+                print(
+                    "\n\nTook {} s to load the data\n\n".format(time.time() - tstart),
+                    flush=True,
+                )
+
+    # strip non-selected keys, if a list is given in select_keys
+    if select_keys:
+        keys = list(data["ensemble"].keys())
+        for key in keys:
+            if key not in select_keys:
+                del data["ensemble"][key]
+
+    # perhaps convert floats?
+    tstart = time.time()
+    if convert_float_keys:
+        # timings are for 100 iterations on the big Moe data set
+        # data = format_ensemble_results(data) # 213s
+        # data = recursive_change_key_to_float(data) # 61s
+        data = keys_to_floats(data)  # 6.94s
+
+        if timing:
+            print(
+                "\n\nTook {} s to convert floats\n\n".format(time.time() - tstart),
+                flush=True,
+            )
+
+    # return data
+    return data
+
+
 class AutoVivificationDict(dict):
     """
     Implementation of perl's autovivification feature, by overriding the
     get item and the __iadd__ operator (https://docs.python.org/3/reference/datamodel.html?highlight=iadd#object.__iadd__)
 
     This allows to set values within a subdict that might not exist yet:
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_events.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Functions to convolve events
 """
 
 import pandas as pd
 
-from syntheticstellarpopconvolve.convolution_general_functions import (
+from syntheticstellarpopconvolve.general_functions import (
     calculate_digitized_sfr_rates,
     handle_custom_scaling_or_conversion,
     handle_extra_weights_function,
 )
 
 
 def extract_event_data(config, convolution_instruction):
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/convolve_populations.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/convolve_populations.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 import multiprocessing
 import os
 import pickle
 
 import h5py
 import setproctitle
 
-from syntheticstellarpopconvolve.convolution_general_functions import (
-    JsonCustomEncoder,
-    generate_group_name,
-    get_tmp_dir,
-    pad_function,
-)
 from syntheticstellarpopconvolve.convolve_custom_data import (
     custom_convolution_function,
     extract_custom_data,
 )
 from syntheticstellarpopconvolve.convolve_ensembles import (
     ensemble_convolution_function,
     extract_ensemble_data,
 )
 from syntheticstellarpopconvolve.convolve_events import (
     event_convolution_function,
     extract_event_data,
 )
+from syntheticstellarpopconvolve.general_functions import (
+    JsonCustomEncoder,
+    generate_group_name,
+    get_tmp_dir,
+    pad_function,
+)
 from syntheticstellarpopconvolve.store_redshift_shell_info import (
     store_redshift_shell_info,
 )
 
 CONVOLUTION_FUNCTION_DICT = {
     "event": event_convolution_function,
     "ensemble": ensemble_convolution_function,
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/cosmology_utils.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/cosmology_utils.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_ensemble.json` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_ensemble.json`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/example_data/example_population_settings.json` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/example_data/example_population_settings.json`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/extract_population_settings.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/extract_population_settings.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/functions_to_review.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/functions_to_review.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/prepare_output_file.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_output_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json
 import os
 import shutil
 
 import h5py
 
-from syntheticstellarpopconvolve.convolution_general_functions import JsonCustomEncoder
+from syntheticstellarpopconvolve.general_functions import JsonCustomEncoder
 
 
 def prepare_output_file(config):
     """
     Function to prepare the output file, create some initial groups and store the configuration
     """
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/prepare_redshift_interpolator.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/prepare_redshift_interpolator.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/store_redshift_shell_info.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_redshift_shell_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """
 Functions to calculate redshift shell info
 """
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve.convolution_general_functions import (
-    calculate_bincenters,
-)
 from syntheticstellarpopconvolve.cosmology_utils import redshift_to_lookback_time
+from syntheticstellarpopconvolve.general_functions import calculate_bincenters
 
 
 def create_shell_volume_dict(redshift_bin_edges, config):
     """
     Function that can generate a dictionary of shell volumes based on an input center redshift array
     """
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/store_sfr_info.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/store_sfr_info.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/main.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,46 +2,26 @@
 Main convolution test script
 """
 
 # pylint: disable=W0611
 # flake8: noqa
 import unittest
 
-from syntheticstellarpopconvolve.tests.test_check_convolution_input_file import (
-    test_check_convolution_input_file,
-)
-from syntheticstellarpopconvolve.tests.test_convolution_calculate_birth_redshift_array import (
+from syntheticstellarpopconvolve.tests.test_calculate_birth_redshift_array import (
     test_calculate_origin_redshift_array,
 )
-from syntheticstellarpopconvolve.tests.test_convolution_check_config import (
+from syntheticstellarpopconvolve.tests.test_check_convolution_config import (
     test_check_convolution_config,
     test_check_convolution_instruction,
     test_check_metallicity,
     test_check_required,
     test_check_sfr_dict,
 )
-from syntheticstellarpopconvolve.tests.test_convolution_default_settings import (
-    test_array_validation,
-    test_callable_or_none_validation,
-    test_callable_validation,
-    test_existing_path_validation,
-    test_logger_validation,
-    test_unit_validation,
-)
-from syntheticstellarpopconvolve.tests.test_convolution_general_functions import (
-    test_calculate_bincenters,
-    test_calculate_digitized_sfr_rates,
-    test_calculate_edge_values,
-    test_calculate_origin_time_array,
-    test_extract_arguments,
-    test_generate_group_name,
-    test_get_tmp_dir,
-    test_handle_custom_scaling_or_conversion,
-    test_handle_extra_weights_function,
-    test_pad_function,
+from syntheticstellarpopconvolve.tests.test_check_input_file import (
+    test_check_input_file,
 )
 from syntheticstellarpopconvolve.tests.test_convolution_with_ensemble import (
     test_convolution_with_ensemble,
 )
 from syntheticstellarpopconvolve.tests.test_convolution_with_events import (
     test_convolution_with_events,
 )
@@ -88,17 +68,37 @@
 )
 from syntheticstellarpopconvolve.tests.test_cosmology_utils import (
     test_age_of_universe_to_redshift,
     test_lookback_time_to_redshift,
     test_redshift_to_age_of_universe,
     test_redshift_to_lookback_time,
 )
+from syntheticstellarpopconvolve.tests.test_default_convolution_config import (
+    test_array_validation,
+    test_callable_or_none_validation,
+    test_callable_validation,
+    test_existing_path_validation,
+    test_logger_validation,
+    test_unit_validation,
+)
 from syntheticstellarpopconvolve.tests.test_extract_population_settings import (
     test_extract_population_settings,
 )
+from syntheticstellarpopconvolve.tests.test_general_functions import (
+    test_calculate_bincenters,
+    test_calculate_digitized_sfr_rates,
+    test_calculate_edge_values,
+    test_calculate_origin_time_array,
+    test_extract_arguments,
+    test_generate_group_name,
+    test_get_tmp_dir,
+    test_handle_custom_scaling_or_conversion,
+    test_handle_extra_weights_function,
+    test_pad_function,
+)
 from syntheticstellarpopconvolve.tests.test_prepare_output_file import (
     test_prepare_output_file,
 )
 from syntheticstellarpopconvolve.tests.test_prepare_redshift_interpolator import (
     test_create_interpolation_datasets,
     test_load_interpolation_data,
     test_prepare_redshift_interpolator,
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_check_convolution_input_file.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_output_file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 """
-Testcases for check_convolution_input_file
+Testcases for prepare_output_file file
 """
 
 import copy
 import os
-import sys
 import unittest
 
 import h5py
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.check_convolution_input_file import (
-    check_convolution_input_file,
-)
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.general_functions import temp_dir
+from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 
 TMP_DIR = temp_dir(
-    "tests", "tests_convolution", "tests_check_convolution_input_file", clean_path=True
+    "tests", "tests_convolution", "test_prepare_output_file", clean_path=True
 )
 
 
-def assertMayRaise(self, exception, expr, **kwargs):
-    if exception is None:
-        try:
-            expr(kwargs)
-        except:
-            info = sys.exc_info()
-            self.fail("%s raised" % repr(info[0]))
-    else:
-        self.assertRaises(exception, expr, **kwargs)
-
-
-unittest.TestCase.assertMayRaise = assertMayRaise
-
-
-class test_check_convolution_input_file(unittest.TestCase):
+class test_prepare_output_file(unittest.TestCase):
     """ """
 
     def setUp(self):
         """
         create input files
         """
 
-        self.config_working = copy.copy(convolution_options_defaults)
+        self.config_working = copy.copy(default_convolution_config)
         self.config_working["input_filename"] = os.path.join(
             TMP_DIR, "working_file.hdf5"
         )
-
-        self.config_not_working = copy.copy(convolution_options_defaults)
-        self.config_not_working["input_filename"] = os.path.join(
-            TMP_DIR, "not_working_file.hdf5"
+        self.config_working["output_filename"] = os.path.join(
+            TMP_DIR, "output_file.hdf5"
         )
 
         #
         self.working_hdf5_file = h5py.File(self.config_working["input_filename"], "w")
         self.working_hdf5_file.create_group("input_data")
         self.working_hdf5_file.create_group("config")
         self.working_hdf5_file.create_group("config/population")
         self.working_hdf5_file.close()
 
-        #
-        self.not_working_hdf5_file = h5py.File(
-            self.config_not_working["input_filename"], "w"
-        )
-        self.not_working_hdf5_file.close()
+    def test_prepare_output_file(self):
 
-    def test_check_convolution_input_file_not_working(self):
-        self.assertRaises(
-            ValueError, check_convolution_input_file, self.config_not_working
-        )
+        # run preparing of output file
+        prepare_output_file(self.config_working)
+
+        #
+        self.assertTrue(os.path.isfile(self.config_working["output_filename"]))
 
-    def test_check_convolution_input_file_working(self):
-        check_convolution_input_file(self.config_working)
+        with h5py.File(self.config_working["output_filename"], "r") as output_hdf5file:
+            self.assertTrue("convolution" in output_hdf5file["config"].keys())
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_calculate_birth_redshift_array.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import copy
 import os
 import unittest
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_calculate_birth_redshift_array import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.calculate_birth_redshift_array import (
     calculate_origin_redshift_array,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_redshift_interpolator import (
     prepare_redshift_interpolator,
 )
 
 TMP_DIR = temp_dir(
     "tests",
     "tests_convolution",
-    "tests_convolution_calculate_birth_redshift_array",
+    "tests_calculate_birth_redshift_array",
     clean_path=True,
 )
 
 
 class test_calculate_origin_redshift_array(unittest.TestCase):
     def test_calculate_origin_redshift_array_all_good(self):
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["redshift_interpolator_data_output_filename"] = os.path.join(
             TMP_DIR, "interpolator_dict.p"
         )
         convolution_config = prepare_redshift_interpolator(convolution_config)
         convolution_config["time_type"] = "redshift"
 
         #
@@ -45,15 +45,15 @@
         np.testing.assert_array_almost_equal(
             origin_redshift_array,
             np.array([0.6501032923316669, 0.8336451543045214, 1.0661079791875108]),
         )
 
     def test_calculate_origin_redshift_array_one_too_far(self):
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["redshift_interpolator_data_output_filename"] = os.path.join(
             TMP_DIR, "interpolator_dict.p"
         )
         convolution_config = prepare_redshift_interpolator(convolution_config)
         convolution_config["time_type"] = "redshift"
 
         #
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_check_config.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_check_convolution_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 """
-Testcases for convolution_check_config file
-
-functions to cover:
-
-TODO: check_required
-TODO: check_convolution_instruction
-TODO: check_convolution_config
+Testcases for check_convolution_config file
 """
 
 import unittest
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
     check_convolution_instruction,
     check_metallicity,
     check_required,
     check_sfr_dict,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
-    "tests", "tests_convolution", "tests_convolution_check_config", clean_path=True
+    "tests", "tests_convolution", "tests_check_convolution_config", clean_path=True
 )
 
 
 class test_check_convolution_config(unittest.TestCase):
     def test_check_convolution_config_with_valid_input(self):
         config_with_valid_convolution = {
             "check_convolution_config": True,
-            "logger": convolution_options_defaults["logger"],
+            "logger": default_convolution_config["logger"],
             "time_type": "lookback_time",
             "convolution_lookback_time_bin_edges": np.array([1, 2]) * u.yr,
             "convolution_instructions": [
                 {
                     "input_data_type": "event",
                     "input_data_name": "event_data",
                     "output_data_name": "output_event_data",
@@ -56,51 +50,55 @@
                     },
                 },
             ],
             "SFR_info": [
                 {
                     "name": "test",
                     "lookback_time_bin_edges": np.array([0, 1, 2, 3]) * 1e9 * u.yr,
-                    "starformation_array": np.array([1, 2, 3]),
+                    "starformation_array": np.array([1, 2, 3]) * u.Msun / u.yr,
                     "metallicity_bin_edges": np.array([0.1, 0.2, 0.3]),
                     "metallicity_weighted_starformation_array": np.array(
                         [[0.5, 0.6, 0.7], [0.5, 0.6, 0.7], [0.5, 0.6, 0.7]]
-                    ),
+                    )
+                    * u.Msun
+                    / u.yr,
                 }
             ],
         }
 
         check_convolution_config(config_with_valid_convolution)
         # No exception should be raised
 
     def test_check_convolution_config_missing_convolution_instruction(self):
 
         config_with_missing_convolution_instruction = {
             "check_convolution_config": True,
-            "logger": convolution_options_defaults["logger"],
+            "logger": default_convolution_config["logger"],
             "time_type": "redshift",
             "convolution_instructions": [],  # Missing convolution instruction
             "SFR_info": [
                 {
                     "lookback_time_bin_edges": [0, 1, 2, 3],
-                    "starformation_array": [1, 2, 3],
+                    "starformation_array": [1, 2, 3] * u.Msun / u.yr,
                     "metallicity_bin_edges": [0.1, 0.2, 0.3],
-                    "metallicity_weighted_starformation_array": [0.5, 0.6, 0.7],
+                    "metallicity_weighted_starformation_array": [0.5, 0.6, 0.7]
+                    * u.Msun
+                    / u.yr,
                 }
             ],
         }
 
         with self.assertRaises(ValueError):
             check_convolution_config(config_with_missing_convolution_instruction)
 
     def test_check_convolution_config_missing_SFR_info(self):
         #
         config_with_missing_SFR_info = {
             "check_convolution_config": True,
-            "logger": convolution_options_defaults["logger"],
+            "logger": default_convolution_config["logger"],
             "time_type": "redshift",
             "convolution_instructions": [
                 {
                     "input_data_type": "event",
                     "input_data_name": "event_data",
                     "output_data_name": "output_event_data",
                     "data_column_dict": {"delay_time": "delay", "yield_rate": "rate"},
@@ -244,19 +242,19 @@
 
 
 class test_check_sfr_dict(unittest.TestCase):
     def setUp(self):
         self.sfr_dict = {
             "name": "test_sfr_dict",
             "lookback_time_bin_edges": np.array([1, 2, 3]) * 1e9 * u.yr,
-            "starformation_array": np.array([10, 20, 30]),
+            "starformation_array": np.array([10, 20, 30]) * u.Msun / u.yr,
             "metallicity_bin_edges": np.array([0.01, 0.1, 0.2]),
-            "metallicity_weighted_starformation_array": np.array(
-                [[1, 2, 3], [4, 5, 6]]
-            ),
+            "metallicity_weighted_starformation_array": np.array([[1, 2, 3], [4, 5, 6]])
+            * u.Msun
+            / u.yr,
         }
 
     def test_check_sfr_dict_with_name(self):
         requires_name = True
         requires_metallicity_info = True
         time_type = "lookback_time"
         check_sfr_dict(
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_default_settings.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_default_convolution_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """
-Testcases for convolution_default_settings.
+Testcases for default_convolution_config.
 """
 
 import logging
 import os
 import unittest
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve.convolution_default_settings import (
+from syntheticstellarpopconvolve.default_convolution_config import (
     array_validation,
     callable_or_none_validation,
     callable_validation,
     existing_path_validation,
     logger_validation,
     unit_validation,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
-    "tests", "tests_convolution", "tests_convolution_default_settings", clean_path=True
+    "tests", "tests_convolution", "tests_default_convolution_config", clean_path=True
 )
 
 
 def assertDoesNotRaise(self, exception, expr, *args, **kwargs):
 
     # Use try-except block to catch exceptions
     try:
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_general_functions.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_general_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """
-Testcases for convolution_general_functions file
+Testcases for general_functions file
 """
 
 import copy
 import json
 import logging
 import os
 import unittest
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pandas as pd
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_general_functions import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.convolve_populations import update_sfr_dict
+from syntheticstellarpopconvolve.general_functions import (
     calculate_bincenters,
     calculate_digitized_sfr_rates,
     calculate_edge_values,
     calculate_origin_time_array,
     extract_arguments,
     generate_group_name,
     get_tmp_dir,
     handle_custom_scaling_or_conversion,
     handle_extra_weights_function,
     pad_function,
     temp_dir,
 )
-from syntheticstellarpopconvolve.convolve_populations import update_sfr_dict
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 from syntheticstellarpopconvolve.prepare_redshift_interpolator import (
     prepare_redshift_interpolator,
 )
 
 TMP_DIR = temp_dir(
-    "tests", "tests_convolution", "tests_convolution_general_functions", clean_path=True
+    "tests", "tests_convolution", "tests_general_functions", clean_path=True
 )
 
 
 class test_calculate_digitized_sfr_rates(unittest.TestCase):
     def setUp(self):
         #
         input_hdf5_filename = os.path.join(TMP_DIR, "input_hdf5_sfr_only.h5")
@@ -82,15 +82,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]) * 1e9 * u.yr,
             "starformation_array": np.array([1, 2, 3, 4, 5]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -139,17 +139,18 @@
 
         digitized_sfr_rates = calculate_digitized_sfr_rates(
             config=self.convolution_config,
             convolution_time_bin_center=0.5 * 1e9 * u.yr,
             data_dict={"delay_time": np.array([-1, 1, 2, 3, 100]) * 1e9 * u.yr},
             sfr_dict=sfr_dict,
         )
+        output_unit = u.Msun / u.yr / u.Gpc**3
 
         np.testing.assert_array_equal(
-            digitized_sfr_rates, np.array([0.0, 2.0, 3.0, 4.0, 0.0])
+            digitized_sfr_rates, np.array([0.0, 2.0, 3.0, 4.0, 0.0]) * output_unit
         )
 
     # def test_calculate_digitized_sfr_rates_metallicity(self):
 
     #     self.convolution_config["SFR_info"]["metallicity_bin_edges"] = (
     #         self.convolution_config["SFR_info"]["starformation_array"]
     #         * np.ones(
@@ -174,43 +175,46 @@
     #     np.testing.assert_array_equal(
     #         digitized_sfr_rates, np.array([0.0, 2.0, 3.0, 4.0, 0.0])
     #     )
 
 
 class test_calculate_origin_time_array(unittest.TestCase):
     def test_calculate_origin_time_array_lookback(self):
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["redshift_interpolator_data_output_filename"] = os.path.join(
             TMP_DIR, "interpolator_dict.p"
         )
         convolution_config = prepare_redshift_interpolator(convolution_config)
         convolution_config["time_type"] = "lookback_time"
 
         origin_time_array = calculate_origin_time_array(
             config=convolution_config,
             data_dict={"delay_time": np.array([1, 2, 3]) * 1e9 * u.yr},
-            convolution_time_bin_center=0.5 * 1e9,
+            convolution_time_bin_center=0.5 * 1e9 * u.yr,
         )
+
         np.testing.assert_array_equal(
-            origin_time_array, np.array([1.5, 2.5, 3.5]) * 1e9
+            origin_time_array, np.array([1.5, 2.5, 3.5]) * 1e9 * u.yr
         )
 
     def test_calculate_origin_time_array_redshift(self):
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["redshift_interpolator_data_output_filename"] = os.path.join(
             TMP_DIR, "interpolator_dict.p"
         )
         convolution_config = prepare_redshift_interpolator(convolution_config)
         convolution_config["time_type"] = "redshift"
 
         origin_time_array = calculate_origin_time_array(
             config=convolution_config,
             data_dict={"delay_time": np.array([1, 2, 3]) * 1e9 * u.yr},
             convolution_time_bin_center=0.5,
         )
+        # output_unit = u.Msun/u.yr/u.Gpc**3
+
         np.testing.assert_array_almost_equal(
             origin_time_array,
             np.array([0.6501032923316669, 0.8336451543045214, 1.0661079791875108]),
         )
 
 
 class test_handle_extra_weights_function(unittest.TestCase):
@@ -256,15 +260,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 import unittest
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults, convolve
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import convolve, default_convolution_config
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "test_convolution_with_ensemble", clean_path=True
 )
 
 
 class test_convolution_with_ensemble(unittest.TestCase):
     """ """
 
     def test_convolution_with_events_with_lookback_time(self):
 
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["logger"].setLevel(logging.CRITICAL)
 
         #
         input_hdf5_filename = os.path.join(TMP_DIR, "input_hdf5_sfr_only.h5")
         output_hdf5_filename = os.path.join(TMP_DIR, "output_hdf5_sfr_only.h5")
 
         ##############
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolution_with_events.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolution_with_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pandas as pd
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults, convolve
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import convolve, default_convolution_config
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "test_convolution_with_events", clean_path=True
 )
 
 
 class test_convolution_with_events(unittest.TestCase):
@@ -71,15 +71,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]) * u.yr,
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_custom_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Testcases for convolve_custom_data file
 """
 
 import unittest
 
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
 from syntheticstellarpopconvolve.convolve_custom_data import (
     custom_convolution_function,
     extract_custom_data,
 )
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_convolve_custom_data", clean_path=True
 )
 
 
 class test_extract_custom_data(unittest.TestCase):
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_ensembles.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 import unittest
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
 from syntheticstellarpopconvolve.convolve_ensembles import (
     _get_ensemble_structure,
     attach_endpoints,
     check_if_value_layer,
     check_if_value_layer_and_get_layer_iterable,
     ensemble_convolution_function,
     ensemble_handle_marginalisation,
@@ -42,24 +41,25 @@
     set_endpoints,
     shift_data_layer,
     shift_layers_dict,
     shift_layers_list,
     strip_ensemble_endpoints,
 )
 from syntheticstellarpopconvolve.convolve_populations import update_sfr_dict
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_convolve_ensembles", clean_path=True
 )
 
 
 class test_handle_binsize_multiplication_factor(unittest.TestCase):
     def test_handle_binsize_multiplication_factor_no_binsize_multiplication(self):
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes, extra_value_dict = handle_binsize_multiplication_factor(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={"binsizes": [1, 2]},
             key="0.1",
             key_i=0,
@@ -67,30 +67,30 @@
             extra_value_dict={},
             name="delay_time",
         )
 
         self.assertFalse(extra_value_dict)
 
     def test_handle_binsize_multiplication_factor_binsizes_passed(self):
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes, extra_value_dict = handle_binsize_multiplication_factor(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={"multiply_by_binsize": True},
             key="0.1",
             key_i=0,
             binsizes=[0.1, 0.15, 0.2],
             extra_value_dict={},
             name="delay_time",
         )
         self.assertTrue(extra_value_dict == {"delay_time_binsize": 0.1})
 
     def test_handle_binsize_multiplication_factor_binsizes_calculated(self):
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes, extra_value_dict = handle_binsize_multiplication_factor(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={"multiply_by_binsize": True},
             key="0.2",
             key_i=1,
@@ -110,41 +110,41 @@
             data_layer_dict_entry={"binsizes": [1, 2]},
         )
 
         self.assertTrue(binsizes == [1, 2])
 
     def test_get_ensemble_binsizes_no_scaling(self):
 
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes = get_ensemble_binsizes(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={},
         )
 
         #
         np.testing.assert_array_almost_equal(binsizes, np.array([0.1, 0.15, 0.2]))
 
     def test_get_ensemble_binsizes_factor_scaling(self):
 
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes = get_ensemble_binsizes(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={"conversion_factor": 2},
         )
 
         #
         np.testing.assert_array_almost_equal(binsizes, np.array([0.2, 0.3, 0.4]))
 
     def test_get_ensemble_binsizes_factor_function(self):
 
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
 
         binsizes = get_ensemble_binsizes(
             config=convolution_config,
             ensemble={"0.1": 2, "0.2": 2, "0.4": 3},
             data_layer_dict_entry={"conversion_function": lambda x: 10**x},
         )
 
@@ -205,15 +205,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([2, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -363,15 +363,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]) * u.yr,
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -550,15 +550,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -776,15 +776,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_events.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pandas as pd
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
 from syntheticstellarpopconvolve.convolve_events import (
     event_convolution_function,
     extract_event_data,
 )
 from syntheticstellarpopconvolve.convolve_populations import update_sfr_dict
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_convolve_events", clean_path=True
 )
 
 
@@ -75,15 +75,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -269,15 +269,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]) * u.yr,
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_convolve_populations.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_convolve_populations.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import astropy.units as u
 import h5py
 import numpy as np
 import pandas as pd
 import pkg_resources
 from astropy.cosmology import Planck13 as cosmo  # Planck 2013
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
 from syntheticstellarpopconvolve.convolve_populations import (
     generate_data_dict,
     pad_sfr_dict,
     update_sfr_dict,
 )
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_convolve_populations", clean_path=True
 )
 
 
@@ -118,15 +118,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]) * u.yr,
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -241,15 +241,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -349,15 +349,15 @@
 
             #
             input_hdf5_file.create_dataset(
                 "input_data/ensemble/dummy", data=json.dumps(self.dummy_ensemble)
             )
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_cosmology_utils.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_cosmology_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 Testcases for convolve_ensembles file
 """
 
 import unittest
 
 from astropy.cosmology import Planck13 as cosmo  # Planck 2013
 
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
 from syntheticstellarpopconvolve.cosmology_utils import (
     age_of_universe_to_redshift,
     lookback_time_to_redshift,
     redshift_to_age_of_universe,
     redshift_to_lookback_time,
 )
+from syntheticstellarpopconvolve.general_functions import temp_dir
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_cosmology_utils", clean_path=True
 )
 
 
 class test_age_of_universe_to_redshift(unittest.TestCase):
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_extract_population_settings.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_extract_population_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 import astropy.units as u
 import h5py
 import numpy as np
 import pandas as pd
 import pkg_resources
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import default_convolution_config
 from syntheticstellarpopconvolve.extract_population_settings import (
     extract_population_settings,
 )
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_output_file import prepare_output_file
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_extract_population_settings", clean_path=True
 )
 
 
@@ -70,15 +70,15 @@
             )
 
         ##############
         # Store data in pandas
         dummy_df.to_hdf(input_hdf5_filename, key="input_data/events/{}".format("dummy"))
 
         #
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 import pickle
 import unittest
 
 import astropy.units as u
 import numpy as np
 from scipy import interpolate
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import default_convolution_config
 from syntheticstellarpopconvolve.cosmology_utils import redshift_to_lookback_time
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.prepare_redshift_interpolator import (
     create_interpolation_datasets,
     load_interpolation_data,
     prepare_redshift_interpolator,
 )
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_prepare_redshift_interpolator", clean_path=True
 )
 
 
 class test_prepare_redshift_interpolator(unittest.TestCase):
     def setUp(self):
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
 
@@ -111,15 +111,15 @@
 
         config = prepare_redshift_interpolator(self.convolution_config)
         self.assertTrue("interpolators" not in config)
 
 
 class test_create_interpolation_datasets(unittest.TestCase):
     def setUp(self):
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
         self.convolution_config["redshift_interpolator_data_output_filename"] = (
             os.path.join(TMP_DIR, "interpolator_dict.p")
         )
 
     def test_create_interpolation_datasets(self):
         create_interpolation_datasets(self.convolution_config)
 
@@ -142,15 +142,15 @@
         self.assertTrue("max_redshift" in interpolation_data_dict)
         self.assertTrue("redshift_stepsize" in interpolation_data_dict)
         self.assertTrue("interpolate_log" in interpolation_data_dict)
 
 
 class test_load_interpolation_data(unittest.TestCase):
     def setUp(self):
-        self.convolution_config = copy.copy(convolution_options_defaults)
+        self.convolution_config = copy.copy(default_convolution_config)
 
         # Set up SFR
         self.convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 
 import copy
 import unittest
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.store_redshift_shell_info import (
     create_shell_volume_dict,
     store_redshift_shell_info,
 )
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_store_redshift_shell_info", clean_path=True
 )
 
 
 class test_store_redshift_shell_info(unittest.TestCase):
     def test_store_redshift_shell_info_redshift(self):
 
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["time_type"] = "redshift"
 
         # Set up SFR
         convolution_config["SFR_info"] = {
             "redshift_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
@@ -72,15 +72,15 @@
             "delta_shell_redshift"
             in convolution_config["redshift_shell_volume_dict"][0.5]
         )
 
     def test_store_redshift_shell_info_no_redshift(self):
 
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["time_type"] = "lookback_time"
 
         # Set up SFR
         convolution_config["SFR_info"] = {
             "lookback_time_bin_edges": np.array([0, 1, 2, 3, 4, 5]),
             "starformation_array": np.array([1, 1, 1, 1, 1]) * u.Msun / u.yr / u.Gpc**3,
         }
@@ -93,15 +93,15 @@
         self.assertTrue("redshift_shell_volume_dict" not in convolution_config.keys())
 
 
 class test_create_shell_volume_dict(unittest.TestCase):
     def test_create_shell_volume_dict(self):
 
         #
-        convolution_config = copy.copy(convolution_options_defaults)
+        convolution_config = copy.copy(default_convolution_config)
         convolution_config["time_type"] = "redshift"
 
         #
         shell_volume_dict = create_shell_volume_dict(
             redshift_bin_edges=np.array([0, 1, 2, 3, 4, 5]),
             config=convolution_config,
         )
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tests/test_update_convolution_config.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tests/test_update_convolution_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import copy
 import os
 import unittest
 
 import astropy.units as u
 import numpy as np
 
-from syntheticstellarpopconvolve import convolution_options_defaults
-from syntheticstellarpopconvolve.convolution_check_config import (
+from syntheticstellarpopconvolve import default_convolution_config
+from syntheticstellarpopconvolve.check_convolution_config import (
     check_convolution_config,
 )
-from syntheticstellarpopconvolve.convolution_general_functions import temp_dir
+from syntheticstellarpopconvolve.general_functions import temp_dir
 from syntheticstellarpopconvolve.update_convolution_config import (
     update_convolution_config,
 )
 
 TMP_DIR = temp_dir(
     "tests", "tests_convolution", "tests_update_convolution_config", clean_path=True
 )
 
 
 class test_update_convolution_config(unittest.TestCase):
     """ """
 
     def test_update_convolution_config(self):
 
-        config = copy.copy(convolution_options_defaults)
+        config = copy.copy(default_convolution_config)
         config["redshift_interpolator_data_output_filename"] = os.path.join(
             TMP_DIR, "interpolator_dict.p"
         )
         #
         config["input_filename"] = os.path.join(TMP_DIR, "input_hdf5_sfr_only.h5")
         config["output_filename"] = os.path.join(TMP_DIR, "output_hdf5_sfr_only.h5")
```

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/tmp.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/tmp.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve/update_convolution_config.py` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve/update_convolution_config.py`

 * *Files identical despite different names*

### Comparing `syntheticstellarpopconvolve-0.1/syntheticstellarpopconvolve.egg-info/SOURCES.txt` & `syntheticstellarpopconvolve-0.2/syntheticstellarpopconvolve.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
+requirements.txt
 setup.py
 syntheticstellarpopconvolve/SFR_plotting_routine.py
 syntheticstellarpopconvolve/__init__.py
+syntheticstellarpopconvolve/_version.py
 syntheticstellarpopconvolve/archive.py
-syntheticstellarpopconvolve/check_convolution_input_file.py
-syntheticstellarpopconvolve/convolution_calculate_birth_redshift_array.py
-syntheticstellarpopconvolve/convolution_check_config.py
-syntheticstellarpopconvolve/convolution_default_settings.py
-syntheticstellarpopconvolve/convolution_general_functions.py
-syntheticstellarpopconvolve/convolution_metallicity_distributions.py
-syntheticstellarpopconvolve/convolution_sfr_distributions.py
+syntheticstellarpopconvolve/calculate_birth_redshift_array.py
+syntheticstellarpopconvolve/check_convolution_config.py
+syntheticstellarpopconvolve/check_input_file.py
 syntheticstellarpopconvolve/convolve.py
 syntheticstellarpopconvolve/convolve_custom_data.py
 syntheticstellarpopconvolve/convolve_ensembles.py
 syntheticstellarpopconvolve/convolve_events.py
 syntheticstellarpopconvolve/convolve_populations.py
 syntheticstellarpopconvolve/cosmology_utils.py
+syntheticstellarpopconvolve/default_convolution_config.py
 syntheticstellarpopconvolve/extract_population_settings.py
 syntheticstellarpopconvolve/functions_to_review.py
+syntheticstellarpopconvolve/general_functions.py
+syntheticstellarpopconvolve/metallicity_distributions.py
 syntheticstellarpopconvolve/prepare_output_file.py
 syntheticstellarpopconvolve/prepare_redshift_interpolator.py
+syntheticstellarpopconvolve/starformation_rate_distributions.py
 syntheticstellarpopconvolve/store_redshift_shell_info.py
 syntheticstellarpopconvolve/store_sfr_info.py
 syntheticstellarpopconvolve/tmp.py
 syntheticstellarpopconvolve/update_convolution_config.py
 syntheticstellarpopconvolve.egg-info/PKG-INFO
 syntheticstellarpopconvolve.egg-info/SOURCES.txt
 syntheticstellarpopconvolve.egg-info/dependency_links.txt
 syntheticstellarpopconvolve.egg-info/requires.txt
 syntheticstellarpopconvolve.egg-info/top_level.txt
 syntheticstellarpopconvolve/example_data/example_RLOF_event_data.dat
 syntheticstellarpopconvolve/example_data/example_ensemble.json
 syntheticstellarpopconvolve/example_data/example_population_settings.json
+syntheticstellarpopconvolve/tests/generate_coverage_report.sh
 syntheticstellarpopconvolve/tests/main.py
 syntheticstellarpopconvolve/tests/test_SFR_plotting_routine.py
-syntheticstellarpopconvolve/tests/test_check_convolution_input_file.py
-syntheticstellarpopconvolve/tests/test_convolution_calculate_birth_redshift_array.py
-syntheticstellarpopconvolve/tests/test_convolution_check_config.py
-syntheticstellarpopconvolve/tests/test_convolution_default_settings.py
-syntheticstellarpopconvolve/tests/test_convolution_general_functions.py
+syntheticstellarpopconvolve/tests/test_calculate_birth_redshift_array.py
+syntheticstellarpopconvolve/tests/test_check_convolution_config.py
+syntheticstellarpopconvolve/tests/test_check_input_file.py
 syntheticstellarpopconvolve/tests/test_convolution_metallicity_distributions.py
-syntheticstellarpopconvolve/tests/test_convolution_sfr_distributions.py
 syntheticstellarpopconvolve/tests/test_convolution_with_ensemble.py
 syntheticstellarpopconvolve/tests/test_convolution_with_events.py
 syntheticstellarpopconvolve/tests/test_convolve.py
 syntheticstellarpopconvolve/tests/test_convolve_custom_data.py
 syntheticstellarpopconvolve/tests/test_convolve_ensembles.py
 syntheticstellarpopconvolve/tests/test_convolve_events.py
 syntheticstellarpopconvolve/tests/test_convolve_populations.py
 syntheticstellarpopconvolve/tests/test_cosmology_utils.py
+syntheticstellarpopconvolve/tests/test_default_convolution_config.py
 syntheticstellarpopconvolve/tests/test_extract_population_settings.py
 syntheticstellarpopconvolve/tests/test_functions_to_review.py
+syntheticstellarpopconvolve/tests/test_general_functions.py
 syntheticstellarpopconvolve/tests/test_prepare_output_file.py
 syntheticstellarpopconvolve/tests/test_prepare_redshift_interpolator.py
+syntheticstellarpopconvolve/tests/test_starformation_rate_distributions.py
 syntheticstellarpopconvolve/tests/test_store_redshift_shell_info.py
 syntheticstellarpopconvolve/tests/test_store_sfr_info.py
 syntheticstellarpopconvolve/tests/test_tmp.py
 syntheticstellarpopconvolve/tests/test_update_convolution_config.py
```

