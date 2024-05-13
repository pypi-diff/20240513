# Comparing `tmp/effector-0.0.272.tar.gz` & `tmp/effector-0.0.273.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-r08pb4w6/effector-0.0.272.tar", last modified: Sun May  5 20:51:36 2024, max compression
+gzip compressed data, was "/home/runner/work/effector/effector/dist/.tmp-h8y2lnxk/effector-0.0.273.tar", last modified: Mon May 13 16:12:50 2024, max compression
```

## Comparing `effector-0.0.272.tar` & `effector-0.0.273.tar`

### file list

```diff
@@ -1,279 +1,279 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-05 20:51:29.000000 effector-0.0.272/.github/workflows/publish_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-05 20:51:29.000000 effector-0.0.272/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-05 20:51:29.000000 effector-0.0.272/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-05 20:51:29.000000 effector-0.0.272/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-05 20:51:29.000000 effector-0.0.272/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-05 20:51:36.000000 effector-0.0.272/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-05 20:51:29.000000 effector-0.0.272/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/Bike-Sharing-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-05 20:51:29.000000 effector-0.0.272/data/Bike-Sharing-Dataset/Readme.txt
--rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-05-05 20:51:29.000000 effector-0.0.272/data/Bike-Sharing-Dataset/day.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-05-05 20:51:29.000000 effector-0.0.272/data/Bike-Sharing-Dataset/hour.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/California-Housing/
--rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-05-05 20:51:29.000000 effector-0.0.272/data/California-Housing/housing.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/Diabetes-Dataset/
--rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-05-05 20:51:29.000000 effector-0.0.272/data/Diabetes-Dataset/diabetes.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/cervical-cancer/
--rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-05-05 20:51:29.000000 effector-0.0.272/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/data/titanic/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-05 20:51:29.000000 effector-0.0.272/data/titanic/gender_submission.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-05-05 20:51:29.000000 effector-0.0.272/data/titanic/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-05-05 20:51:29.000000 effector-0.0.272/data/titanic/train.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-05 20:51:29.000000 effector-0.0.272/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/Guides/
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/Guides/wrap_models.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
--rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
--rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/
--rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    94845 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    60885 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    49603 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    94376 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    22926 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/
--rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20932 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    21292 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20769 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18879 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/
--rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25416 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    27030 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    96087 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61308 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    60089 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    89398 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    22926 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
--rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/global_effect_intro.md
--rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/regional_effect_intro.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_global_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_global_rhale.png
--rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
--rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_regional_pdp_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_regional_rhale_weekends.png
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
--rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/concept_example_black_box.png
--rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/concept_example_dataset.png
--rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
--rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/effector_intro.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/github-mark-white.png
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/github-mark-white.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/github-mark.png
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-05 20:51:29.000000 effector-0.0.272/docs/docs/static/github-mark.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/docs/javascript/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 20:51:29.000000 effector-0.0.272/docs/javascript/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-05 20:51:29.000000 effector-0.0.272/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/effector/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-05 20:51:29.000000 effector-0.0.272/effector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-05 20:51:29.000000 effector-0.0.272/effector/bin_splitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-05 20:51:29.000000 effector-0.0.272/effector/binning_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-05 20:51:29.000000 effector-0.0.272/effector/global_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-05 20:51:29.000000 effector-0.0.272/effector/global_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-05-05 20:51:29.000000 effector-0.0.272/effector/global_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-05 20:51:29.000000 effector-0.0.272/effector/global_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-05 20:51:29.000000 effector-0.0.272/effector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-05 20:51:29.000000 effector-0.0.272/effector/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-05-05 20:51:29.000000 effector-0.0.272/effector/partitioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-05 20:51:29.000000 effector-0.0.272/effector/regional_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-05-05 20:51:29.000000 effector-0.0.272/effector/regional_effect_ale.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-05-05 20:51:29.000000 effector-0.0.272/effector/regional_effect_pdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-05 20:51:29.000000 effector-0.0.272/effector/regional_effect_shap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-05-05 20:51:29.000000 effector-0.0.272/effector/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-05 20:51:29.000000 effector-0.0.272/effector/utils_integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-05 20:51:29.000000 effector-0.0.272/effector/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-05 20:51:36.000000 effector-0.0.272/effector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-05 20:51:29.000000 effector-0.0.272/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/real-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-05-05 20:51:29.000000 effector-0.0.272/real-examples/01_bike_sharing_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-05 20:51:29.000000 effector-0.0.272/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 20:51:29.000000 effector-0.0.272/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 20:51:36.000000 effector-0.0.272/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/synthetic-examples/
--rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/01_linear_model.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   791563 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/02_global_effect_methods_comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   600519 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/02_regional_pdp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   225230 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/02_regional_rhale.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   258931 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/02_regional_shapdp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1075793 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/03_regional_effects_synthetic_f.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-05-05 20:51:29.000000 effector-0.0.272/synthetic-examples/04_regional_effects_real_f.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:36.000000 effector-0.0.272/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 20:51:29.000000 effector-0.0.272/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-05 20:51:29.000000 effector-0.0.272/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-05 20:51:29.000000 effector-0.0.272/tests/test_functional_gam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-05 20:51:29.000000 effector-0.0.272/tests/test_functional_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-05 20:51:29.000000 effector-0.0.272/tests/test_regional_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-05 20:51:29.000000 effector-0.0.272/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-13 16:12:35.000000 effector-0.0.273/.github/workflows/publish_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-13 16:12:35.000000 effector-0.0.273/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 16:12:35.000000 effector-0.0.273/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-13 16:12:35.000000 effector-0.0.273/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 16:12:35.000000 effector-0.0.273/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-13 16:12:50.000000 effector-0.0.273/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-13 16:12:35.000000 effector-0.0.273/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/Bike-Sharing-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     5496 2024-05-13 16:12:35.000000 effector-0.0.273/data/Bike-Sharing-Dataset/Readme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    57569 2024-05-13 16:12:35.000000 effector-0.0.273/data/Bike-Sharing-Dataset/day.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1156736 2024-05-13 16:12:35.000000 effector-0.0.273/data/Bike-Sharing-Dataset/hour.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/California-Housing/
+-rw-r--r--   0 runner    (1001) docker     (127)  1423529 2024-05-13 16:12:35.000000 effector-0.0.273/data/California-Housing/housing.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/Diabetes-Dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2024-05-13 16:12:35.000000 effector-0.0.273/data/Diabetes-Dataset/diabetes.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/cervical-cancer/
+-rw-r--r--   0 runner    (1001) docker     (127)   102059 2024-05-13 16:12:35.000000 effector-0.0.273/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/data/titanic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-13 16:12:35.000000 effector-0.0.273/data/titanic/gender_submission.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-05-13 16:12:35.000000 effector-0.0.273/data/titanic/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    61194 2024-05-13 16:12:35.000000 effector-0.0.273/data/titanic/train.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 16:12:35.000000 effector-0.0.273/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/Guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/Guides/wrap_models.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    25851 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25217 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27129 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    74048 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)   104555 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    28636 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    15998 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14268 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17150 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    85909 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11524 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18929 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20685 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19333 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18741 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18654 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19090 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19706 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19684 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25706 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16923 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    15115 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20653 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21065 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31929 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20442 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25683 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22800 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82693 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93083 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    78989 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    70340 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27778 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27329 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13492 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    13129 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94845 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18512 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18065 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60885 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49603 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10078 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    94376 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13654 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11084 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22926 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12980 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    21294 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20932 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21292 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20769 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18514 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18879 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    23153 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25416 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19078 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23179 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19226 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23715 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27030 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    13246 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    96087 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18519 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61308 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    60089 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13460 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89398 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13926 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11528 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11031 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18870 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16888 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18887 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23337 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19138 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24132 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22926 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25366 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41075 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    28119 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13626 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95212 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45458 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    63502 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    64573 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    61231 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    77057 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44284 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33786 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44470 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48588 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18154 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19813 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21673 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20356 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18315 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25080 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21805 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24421 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22247 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27083 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24762 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/global_effect_intro.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/regional_effect_intro.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    25907 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_global_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98424 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28145 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_global_rhale.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31328 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png
+-rw-r--r--   0 runner    (1001) docker     (127)   100395 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_regional_pdp_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    73994 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_regional_pdp_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25151 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_regional_rhale_weekends.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/bike_sharing_regional_rhale_workingdays.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31146 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/concept_example_black_box.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14193 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/concept_example_dataset.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89602 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/concept_example_global_effect_feat_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    65825 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57999 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png
+-rw-r--r--   0 runner    (1001) docker     (127)   132369 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/effector_intro.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/github-mark-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/github-mark-white.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/github-mark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-13 16:12:35.000000 effector-0.0.273/docs/docs/static/github-mark.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/docs/javascript/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 16:12:35.000000 effector-0.0.273/docs/javascript/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-13 16:12:35.000000 effector-0.0.273/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/effector/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-13 16:12:35.000000 effector-0.0.273/effector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14794 2024-05-13 16:12:35.000000 effector-0.0.273/effector/bin_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-13 16:12:35.000000 effector-0.0.273/effector/binning_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-13 16:12:35.000000 effector-0.0.273/effector/global_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20482 2024-05-13 16:12:35.000000 effector-0.0.273/effector/global_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26002 2024-05-13 16:12:35.000000 effector-0.0.273/effector/global_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14405 2024-05-13 16:12:35.000000 effector-0.0.273/effector/global_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-13 16:12:35.000000 effector-0.0.273/effector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-13 16:12:35.000000 effector-0.0.273/effector/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25993 2024-05-13 16:12:35.000000 effector-0.0.273/effector/partitioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13283 2024-05-13 16:12:35.000000 effector-0.0.273/effector/regional_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14143 2024-05-13 16:12:35.000000 effector-0.0.273/effector/regional_effect_ale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-13 16:12:35.000000 effector-0.0.273/effector/regional_effect_pdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-13 16:12:35.000000 effector-0.0.273/effector/regional_effect_shap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15370 2024-05-13 16:12:35.000000 effector-0.0.273/effector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-13 16:12:35.000000 effector-0.0.273/effector/utils_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-13 16:12:35.000000 effector-0.0.273/effector/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19205 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 16:12:50.000000 effector-0.0.273/effector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-13 16:12:35.000000 effector-0.0.273/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/real-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   427021 2024-05-13 16:12:35.000000 effector-0.0.273/real-examples/01_bike_sharing_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-13 16:12:35.000000 effector-0.0.273/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 16:12:35.000000 effector-0.0.273/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:12:50.000000 effector-0.0.273/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/synthetic-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   753343 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/01_linear_model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   791563 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/02_global_effect_methods_comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   600519 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/02_regional_pdp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   225024 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/02_regional_rhale.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   258931 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/02_regional_shapdp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1075793 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/03_regional_effects_synthetic_f.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1437013 2024-05-13 16:12:35.000000 effector-0.0.273/synthetic-examples/04_regional_effects_real_f.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:50.000000 effector-0.0.273/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:12:35.000000 effector-0.0.273/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-05-13 16:12:35.000000 effector-0.0.273/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-13 16:12:35.000000 effector-0.0.273/tests/test_functional_gam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-13 16:12:35.000000 effector-0.0.273/tests/test_functional_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-13 16:12:35.000000 effector-0.0.273/tests/test_regional_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-13 16:12:35.000000 effector-0.0.273/tests/test_unit.py
```

### Comparing `effector-0.0.272/.github/workflows/publish_documentation.yml` & `effector-0.0.273/.github/workflows/publish_documentation.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/.github/workflows/publish_to_pypi.yml` & `effector-0.0.273/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/.gitignore` & `effector-0.0.273/.gitignore`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/LICENSE` & `effector-0.0.273/LICENSE`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/PKG-INFO` & `effector-0.0.273/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.272
+Version: 0.0.273
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
 Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
 License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
```

### Comparing `effector-0.0.272/README.md` & `effector-0.0.273/README.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/Bike-Sharing-Dataset/Readme.txt` & `effector-0.0.273/data/Bike-Sharing-Dataset/Readme.txt`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/Bike-Sharing-Dataset/day.csv` & `effector-0.0.273/data/Bike-Sharing-Dataset/day.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/Bike-Sharing-Dataset/hour.csv` & `effector-0.0.273/data/Bike-Sharing-Dataset/hour.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/California-Housing/housing.csv` & `effector-0.0.273/data/California-Housing/housing.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/Diabetes-Dataset/diabetes.csv` & `effector-0.0.273/data/Diabetes-Dataset/diabetes.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv` & `effector-0.0.273/data/cervical-cancer/kag_risk_factors_cervical_cancer.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/titanic/gender_submission.csv` & `effector-0.0.273/data/titanic/gender_submission.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/titanic/test.csv` & `effector-0.0.273/data/titanic/test.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/data/titanic/train.csv` & `effector-0.0.273/data/titanic/train.csv`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/Guides/wrap_models.md` & `effector-0.0.273/docs/docs/Tutorials/Guides/wrap_models.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_23_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_29_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png` & `effector-0.0.273/docs/docs/Tutorials/real-examples/01_bike_sharing_dataset_files/01_bike_sharing_dataset_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_11_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_16_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_18_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_22_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_24_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_30_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_34_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_39_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/01_linear_model_files/01_linear_model_9_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_11_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_15_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_19_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_38_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_41_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_global_effect_methods_comparison_files/02_global_effect_methods_comparison_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_15_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_18_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_22_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_26_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_29_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_33_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_37_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_43_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_52_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_56_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_pdp_files/02_regional_pdp_61_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_13_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_19_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_20_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_rhale_files/02_regional_rhale_9_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_13_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_18_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/02_regional_shapdp_files/02_regional_shapdp_9_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_32_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_36_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_42_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/03_regional_effects_synthetic_f_files/03_regional_effects_synthetic_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_10_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_14_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_17_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_21_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_25_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_28_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_33_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_37_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_43_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_51_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_55_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_0.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_1.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png` & `effector-0.0.273/docs/docs/Tutorials/synthetic-examples/04_regional_effects_real_f_files/04_regional_effects_real_f_60_2.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/api.md` & `effector-0.0.273/docs/docs/api.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/global_effect_intro.md` & `effector-0.0.273/docs/docs/global_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/index.md` & `effector-0.0.273/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/references.md` & `effector-0.0.273/docs/docs/references.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/regional_effect_intro.md` & `effector-0.0.273/docs/docs/regional_effect_intro.md`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_global_pdp.png` & `effector-0.0.273/docs/docs/static/bike_sharing_global_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png` & `effector-0.0.273/docs/docs/static/bike_sharing_global_pdp_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_global_rhale.png` & `effector-0.0.273/docs/docs/static/bike_sharing_global_rhale.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png` & `effector-0.0.273/docs/docs/static/bike_sharing_global_rhale_heterogeneity.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_regional_pdp_weekends.png` & `effector-0.0.273/docs/docs/static/bike_sharing_regional_pdp_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_regional_pdp_workingdays.png` & `effector-0.0.273/docs/docs/static/bike_sharing_regional_pdp_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_regional_rhale_weekends.png` & `effector-0.0.273/docs/docs/static/bike_sharing_regional_rhale_weekends.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/bike_sharing_regional_rhale_workingdays.png` & `effector-0.0.273/docs/docs/static/bike_sharing_regional_rhale_workingdays.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/concept_example_black_box.png` & `effector-0.0.273/docs/docs/static/concept_example_black_box.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/concept_example_dataset.png` & `effector-0.0.273/docs/docs/static/concept_example_dataset.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/concept_example_global_effect_feat_1_pdp.png` & `effector-0.0.273/docs/docs/static/concept_example_global_effect_feat_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png` & `effector-0.0.273/docs/docs/static/concept_example_regional_effect_feat_1_index_1_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png` & `effector-0.0.273/docs/docs/static/concept_example_regional_effect_feat_1_index_2_pdp.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/effector_intro.gif` & `effector-0.0.273/docs/docs/static/effector_intro.gif`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/github-mark-white.png` & `effector-0.0.273/docs/docs/static/github-mark-white.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/github-mark-white.svg` & `effector-0.0.273/docs/docs/static/github-mark-white.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/github-mark.png` & `effector-0.0.273/docs/docs/static/github-mark.png`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/docs/static/github-mark.svg` & `effector-0.0.273/docs/docs/static/github-mark.svg`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/docs/mkdocs.yml` & `effector-0.0.273/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/bin_splitting.py` & `effector-0.0.273/effector/bin_splitting.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/binning_methods.py` & `effector-0.0.273/effector/binning_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/global_effect.py` & `effector-0.0.273/effector/global_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/global_effect_ale.py` & `effector-0.0.273/effector/global_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/global_effect_pdp.py` & `effector-0.0.273/effector/global_effect_pdp.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,60 +29,63 @@
 
         super(PDPBase, self).__init__(
             method_name,
             data,
             model, nof_instances, axis_limits, avg_output, feature_names, target_name
         )
 
-    def _predict(self, data, xx, feature):
+    def _predict(self, data, xx, feature, use_vectorized=True):
+        method = pdp_1d_vectorized if use_vectorized else pdp_1d_non_vectorized
         if self.method_name == "pdp":
-            y = pdp_1d_vectorized(
+            y = method(
                 self.model, data, xx, feature, False, False, True
             )
         else:
             if self.model_jac is not None:
-                y = pdp_1d_vectorized(self.model_jac, self.data, xx, feature, False, True, True)
+                y = method(self.model_jac, self.data, xx, feature, False, True, True)
             else:
-                y = pdp_1d_vectorized(self.model, self.data, xx, feature, False, False, True, True)
+                y = method(self.model, self.data, xx, feature, False, False, True, True)
         return y
 
     def _fit_feature(
         self,
         feature: int,
         centering: Union[bool, str] = False,
         points_for_centering: int = 100,
+        use_vectorized: bool = True,
     ) -> dict:
 
         # drop points outside of limits
         self.data = self.data[self.data[:, feature] >= self.axis_limits[0, feature]]
         self.data = self.data[self.data[:, feature] <= self.axis_limits[1, feature]]
         data = self.data
 
         if centering is True or centering == "zero_integral":
             xx = np.linspace(
                 self.axis_limits[0, feature],
                 self.axis_limits[1, feature],
                 points_for_centering,
             )
-            y = self._predict(data, xx, feature)
+            y = self._predict(data, xx, feature, use_vectorized)
             norm_const = np.mean(y, axis=0)
             fe = {"norm_const": norm_const}
         elif centering == "zero_start":
             xx = self.axis_limits[0, feature, np.newaxis]
-            y = self._predict(data, xx, feature)
+            y = self._predict(data, xx, feature, use_vectorized)
             fe = {"norm_const": y[0]}
         else:
             fe = {"norm_const": helpers.EMPTY_SYMBOL}
         return fe
 
     def fit(
         self,
         features: Union[int, str, list] = "all",
         centering: Union[bool, str] = True,
         points_for_centering: int = 100,
+        use_vectorized: bool = True,
     ):
         """
         Fit the PDP or d-PDP.
 
         Notes:
             You can use `.eval` or `.plot` without calling `.fit` explicitly.
             The only thing that `.fit` does is to compute the normalization constant for centering the PDP and ICE plots.
@@ -97,36 +100,39 @@
                 - `False` means no centering
                 - `True` or `zero_integral` centers around the `y` axis.
                 - `zero_start` starts the plot from `y=0`.
 
             points_for_centering: number of linspaced points along the feature axis used for centering.
 
                 - If set to `"all"`, all the dataset points will be used.
+                
+            use_vectorized: whether to use the vectorized version of the PDP computation
 
         """
         centering = helpers.prep_centering(centering)
         features = helpers.prep_features(features, self.dim)
 
         for s in features:
             self.feature_effect["feature_" + str(s)] = self._fit_feature(
-                s, centering, points_for_centering
+                s, centering, points_for_centering, use_vectorized
             )
             self.is_fitted[s] = True
             self.method_args["feature_" + str(s)] = {
                 "centering": centering,
                 "points_for_centering": points_for_centering,
             }
 
     def eval(
         self,
         feature: int,
         xs: np.ndarray,
         heterogeneity: bool = False,
         centering: typing.Union[bool, str] = False,
         return_all: bool = False,
+        use_vectorized: bool = True,
     ) -> typing.Union[np.ndarray, typing.Tuple[np.ndarray, np.ndarray]]:
         """Evaluate the effect of the s-th feature at positions `xs`.
 
         Args:
             feature: index of feature of interest
             xs: the points along the s-th axis to evaluate the FE plot
 
@@ -143,29 +149,31 @@
                 - If `centering` is `True` or `zero_integral`, the PDP is centered around the `y` axis.
                 - If `centering` is `zero_start`, the PDP starts from `y=0`.
 
             return_all: whether to return PDP and ICE plots evaluated at `xs`
 
                 - If `return_all=False`, the function returns the mean effect at the given `xs`
                 - If `return_all=True`, the function returns a `ndarray` of shape `(T, N)` with the `N` ICE plots evaluated at `xs`
+                
+            use_vectorized: whether to use the vectorized version of the PDP computation
 
         Returns:
             the mean effect `y`, if `heterogeneity=False` (default) or a tuple `(y, std)` otherwise
 
         """
         centering = helpers.prep_centering(centering)
 
         if self.refit(feature, centering):
-            self.fit(features=feature, centering=centering)
+            self.fit(features=feature, centering=centering, use_vectorized=use_vectorized)
 
         # Check if the lower bound is less than the upper bound
         assert self.axis_limits[0, feature] < self.axis_limits[1, feature]
 
         # new implementation
-        yy = self._predict(self.data, xs, feature)
+        yy = self._predict(self.data, xs, feature, use_vectorized)
 
         if centering:
             norm_consts = np.expand_dims(
                 self.feature_effect["feature_" + str(feature)]["norm_const"], axis=0
             )
             yy = yy - norm_consts
 
@@ -187,14 +195,15 @@
         centering: Union[bool, str] = False,
         nof_points: int = 30,
         scale_x: Optional[dict] = None,
         scale_y: Optional[dict] = None,
         nof_ice: Union[int, str] = "all",
         show_avg_output: bool = False,
         y_limits: Optional[List] = None,
+        use_vectorized: bool = True,
     ):
         """
         Plot the PDP or d-PDP.
 
         Args:
             feature: index of the plotted feature
             heterogeneity: whether to output the heterogeneity of the SHAP values
@@ -211,24 +220,25 @@
 
             nof_points: number of points to evaluate the SDP plot
             scale_x: dictionary with keys "mean" and "std" for scaling the x-axis
             scale_y: dictionary with keys "mean" and "std" for scaling the y-axis
             nof_ice: number of shap values to show on top of the SHAP curve
             show_avg_output: whether to show the average output of the model
             y_limits: limits of the y-axis
+            use_vectorized: whether to use the vectorized version of the PDP computation
         """
         heterogeneity = helpers.prep_confidence_interval(heterogeneity)
         centering = helpers.prep_centering(centering)
 
         x = np.linspace(
             self.axis_limits[0, feature], self.axis_limits[1, feature], nof_points
         )
 
         yy = self.eval(
-            feature, x, heterogeneity=False, centering=centering, return_all=True
+            feature, x, heterogeneity=False, centering=centering, return_all=True, use_vectorized=use_vectorized
         )
 
         if show_avg_output:
             avg_output = helpers.prep_avg_output(self.data, self.model, self.avg_output, scale_y)
         else:
             avg_output = None
 
@@ -406,62 +416,85 @@
 
 def pdp_1d_non_vectorized(
     model: callable,
     data: np.ndarray,
     x: np.ndarray,
     feature: int,
     heterogeneity: bool,
-    is_jac: bool,
+    model_returns_jac: bool,
+    return_all: bool = False,
+    ask_for_derivatives: bool = False,
 ) -> typing.Union[np.ndarray, typing.Tuple[np.ndarray, np.ndarray, np.ndarray]]:
     """Computes the unnormalized 1-dimensional PDP, in a non-vectorized way.
 
     Notes:
         The non-vectorized version is slower than the vectorized one, but it requires less memory.
 
     Examples:
         >>> # check the gradient of the PDP of a linear model
         >>> import numpy as np
         >>> model = lambda x: np.sum(x, axis=1)
         >>> data = np.random.rand(100, 10)
         >>> x = np.linspace(0.1, 1, 10)
         >>> feature = 0
-        >>> y = pdp_1d_vectorized(model, data, x, feature, heterogeneity=False, model_returns_jac=False)
+        >>> y = pdp_1d_non_vectorized(model, data, x, feature, heterogeneity=False, model_returns_jac=False)
         >>> (y[1:] - y[:-1]) / (x[1:] - x[:-1])
         array([1., 1., 1., 1., 1., 1., 1., 1., 1.])
+        >>> # check the gradient of the PDP of a linear model with heterogeneity
+        >>> dpdp, _, _ = pdp_1d_non_vectorized(model, data, x, feature, heterogeneity=True, model_returns_jac=False, return_all=False, ask_for_derivatives=True)
+        >>> dpdp
+        array([1., 1., 1., 1., 1., 1., 1., 1., 1., 1.])
+
 
     Args:
         model: The black-box function (N, D) -> (N)
         data: The design matrix, (N, D)
         x: positions to evaluate pdp, (T)
         feature: index of the feature of interest
         heterogeneity: whether to also compute the heterogeneity of the PDP
-        is_jac (bool): whether the model returns the prediction (False) or the Jacobian wrt the input (True)
+        model_returns_jac (bool): whether the model returns the prediction (False) or the Jacobian wrt the input (True)
+        return_all (bool): whether to return all the predictions or only the mean (and std and stderr)
+        ask_for_derivatives (bool): whether to ask the model to return the derivatives wrt the input
 
     Returns:
         The PDP values `y` that correspond to `x`, if heterogeneity is False, `(y, std, stderr)` otherwise
 
     """
-    nof_points = x.shape[0]
-    mean_pdp = []
-    sigma_pdp = []
-    stderr = []
-    for i in range(nof_points):
-        x_new = copy.deepcopy(data)
-        x_new[:, feature] = x[i]
-        y = model(x_new)[:, feature] if is_jac else model(x_new)
-        mean_pdp.append(np.mean(y))
-        if heterogeneity:
-            std = np.std(y)
-            sigma_pdp.append(std)
-            stderr.append(std / np.sqrt(data.shape[0]))
-    return (
-        (np.array(mean_pdp), np.array(sigma_pdp), np.array(stderr))
-        if heterogeneity
-        else np.array(mean_pdp)
-    )
+    nof_instances = x.shape[0]
+
+    y_list = []
+    if ask_for_derivatives and not model_returns_jac:
+        for k in range(nof_instances):
+            x_new = copy.deepcopy(data)
+            x_new[:, feature] = x[k] + 1e-6
+            y_1 = model(x_new)
+            x_new[:, feature] = x[k] - 1e-6
+            y_2 = model(x_new)
+            y = (y_1 - y_2) / (2 * 1e-6)
+            y_list.append(y)
+        y = np.array(y_list)
+    else:
+        for k in range(nof_instances):
+            x_new = copy.deepcopy(data)
+            x_new[:, feature] = x[k]
+            y = model(x_new)[:, feature] if model_returns_jac else model(x_new)
+            y_list.append(y)
+        y = np.array(y_list)
+
+    mean_pdp = np.mean(y, axis=1)
+    if return_all:
+        return y
+
+    if heterogeneity:
+        std = np.std(y, axis=1)
+        sigma_pdp = std
+        stderr = std / np.sqrt(data.shape[0])
+        return mean_pdp, sigma_pdp, stderr
+    else:
+        return mean_pdp
 
 
 def pdp_1d_vectorized(
     model: callable,
     data: np.ndarray,
     x: np.ndarray,
     feature: int,
@@ -492,16 +525,16 @@
     Args:
         model: The black-box function (N, D) -> (N)
         data: The design matrix, (N, D)
         x: positions to evaluate pdp, (T)
         feature: index of the feature of interest
         heterogeneity: whether to also compute the heterogeneity of the PDP
         model_returns_jac (bool): whether the model returns the prediction (False) or the Jacobian wrt the input (True)
-        ask_for_derivatives (bool): whether to ask the model to return the derivatives wrt the input
         return_all (bool): whether to return all the predictions or only the mean (and std and stderr)
+        ask_for_derivatives (bool): whether to ask the model to return the derivatives wrt the input
 
     Returns:
         The PDP values `y` that correspond to `x`, if heterogeneity is False, `(y, std, stderr)` otherwise
 
     """
 
     nof_instances = data.shape[0]
```

### Comparing `effector-0.0.272/effector/global_effect_shap.py` & `effector-0.0.273/effector/global_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/helpers.py` & `effector-0.0.273/effector/helpers.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/interaction.py` & `effector-0.0.273/effector/interaction.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/partitioning.py` & `effector-0.0.273/effector/partitioning.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/regional_effect.py` & `effector-0.0.273/effector/regional_effect.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/regional_effect_ale.py` & `effector-0.0.273/effector/regional_effect_ale.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/regional_effect_pdp.py` & `effector-0.0.273/effector/regional_effect_pdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,35 +31,35 @@
             nof_instances,
             axis_limits,
             feature_types,
             cat_limit,
             feature_names,
             target_name)
 
-    def _create_heterogeneity_function(self, foi, min_points, centering, nof_instances, points_for_centering):
+    def _create_heterogeneity_function(self, foi, min_points, centering, nof_instances, points_for_centering, use_vectorized=True):
         def heter(data) -> float:
             if data.shape[0] < min_points:
                 return BIG_M
 
             if self.method_name == "pdp":
                 pdp = PDP(data, self.model, self.axis_limits, nof_instances=nof_instances)
             else:
                 pdp = DerPDP(data, self.model, self.model_jac, self.axis_limits, nof_instances=nof_instances)
 
             try:
-                pdp.fit(features=foi, centering=centering, points_for_centering=points_for_centering)
+                pdp.fit(features=foi, centering=centering, points_for_centering=points_for_centering, use_vectorized=use_vectorized)
             except:
                 return BIG_M
 
             # heterogeneity is the mean heterogeneity over the curve
             axis_limits = helpers.axis_limits_from_data(data)
 
             xx = np.linspace(axis_limits[:, foi][0], axis_limits[:, foi][1], 10)
             try:
-                _, z = pdp.eval(feature=foi, xs=xx, heterogeneity=True)
+                _, z = pdp.eval(feature=foi, xs=xx, heterogeneity=True, use_vectorized=use_vectorized)
             except:
                 return BIG_M
             return np.mean(z)
 
         return heter
 
     def fit(
@@ -71,14 +71,15 @@
         nof_candidate_splits_for_numerical: int = 20,
         min_points_per_subregion: int = 10,
         candidate_conditioning_features: typing.Union["str", list] = "all",
         split_categorical_features: bool = False,
         centering: typing.Union[bool, str] = False,
         nof_instances: int = "all",
         points_for_centering: int = 100,
+        use_vectorized: bool = True,
     ):
         """
         Find the Regional PDP for a list of features.
 
         Args:
             features: list of features to fit
             heter_pcg_drop_thres: heterogeneity drop threshold for a split to be considered important
@@ -89,15 +90,15 @@
             candidate_conditioning_features: list of features to consider as conditioning features for the candidate splits
             split_categorical_features
         """
 
         assert min_points_per_subregion >= 2, "min_points_per_subregion must be >= 2"
         features = helpers.prep_features(features, self.dim)
         for feat in tqdm(features):
-            heter = self._create_heterogeneity_function(feat, min_points_per_subregion, centering, nof_instances, points_for_centering)
+            heter = self._create_heterogeneity_function(feat, min_points_per_subregion, centering, nof_instances, points_for_centering, use_vectorized)
 
             self._fit_feature(
                 feat,
                 heter,
                 heter_pcg_drop_thres,
                 heter_small_enough,
                 max_depth,
```

### Comparing `effector-0.0.272/effector/regional_effect_shap.py` & `effector-0.0.273/effector/regional_effect_shap.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/utils.py` & `effector-0.0.273/effector/utils.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/utils_integrate.py` & `effector-0.0.273/effector/utils_integrate.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector/visualization.py` & `effector-0.0.273/effector/visualization.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/effector.egg-info/PKG-INFO` & `effector-0.0.273/effector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effector
-Version: 0.0.272
+Version: 0.0.273
 Summary: A Python library for global and regional effects
 Author-email: Vasilis Gkolemis <ntipakos@gmail.com>
 Maintainer-email: Julia Herbinger <julia.herbinger@gmail.com>, Christos Diou <cdiou@hua.gr>, Giuseppe Casalicchio <giuseppe.casalicchio@gmail.com>
 License: MIT License
 Project-URL: documentation, https://xai-effector.github.io
 Project-URL: source, https://github.com/givasile/effector
 Project-URL: tracker, https://github.com/givasile/effector/issues
```

### Comparing `effector-0.0.272/effector.egg-info/SOURCES.txt` & `effector-0.0.273/effector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/pyproject.toml` & `effector-0.0.273/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     {name = "Julia Herbinger", email = "julia.herbinger@gmail.com"},
     {name = "Christos Diou", email = "cdiou@hua.gr"},
     {name = "Giuseppe Casalicchio", email = "giuseppe.casalicchio@gmail.com"}
 ]
 license = {text = "MIT License"}
 requires-python = ">=3.7"
 keywords = ["explainability", "machine learning", "deep learning", "interpretability", "feature effect"]
-version = "0.0.272"
+version = "0.0.273"
 readme = "README.md"
 dependencies = [
     "matplotlib",
     "numpy",
     "scipy",
     "tqdm",
     "shap"
```

### Comparing `effector-0.0.272/real-examples/01_bike_sharing_dataset.ipynb` & `effector-0.0.273/real-examples/01_bike_sharing_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/01_linear_model.ipynb` & `effector-0.0.273/synthetic-examples/01_linear_model.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/02_global_effect_methods_comparison.ipynb` & `effector-0.0.273/synthetic-examples/02_global_effect_methods_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/02_regional_pdp.ipynb` & `effector-0.0.273/synthetic-examples/02_regional_pdp.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/02_regional_rhale.ipynb` & `effector-0.0.273/synthetic-examples/02_regional_rhale.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999137931034483%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(3, ' $$ y = 3x_1I_{x_3>0} - 3x_1I_{x_3\\\\leq0} + "*

 * *            "x_3$$.\\n')], delete: [5, 4, 3]}}}"}*

```diff
@@ -72,17 +72,15 @@
             "cell_type": "markdown",
             "id": "83240f12",
             "metadata": {},
             "source": [
                 "### Black-box function\n",
                 "\n",
                 "We will use the following linear model with a subgroup-specific interaction term:\n",
-                " $$ y = 3x_1I_{x_3>0} - 3x_1I_{x_3\\leq0} + x_3$$ \n",
-                "\n",
-                "The presence of interaction terms ($3x_1I_{x_3>0}$, $3x_1I_{x_3\\leq0}$) makes it impossible to define a solid ground truth effect. However, under some mild assumptions, we can agree tha\n",
+                " $$ y = 3x_1I_{x_3>0} - 3x_1I_{x_3\\leq0} + x_3$$.\n",
                 "\n",
                 "## Ground truth effect (uncorrelated setting)\n",
                 "\n",
                 "In the uncorrelated scenario, the effects are as follows:\n",
                 "\n",
                 "- For the feature $x_1$, the global effect will be $3x_1$ half of the time (when $I_{x_3>0}$) and $-3x_1$ the other half (when $3x_1I_{x_3\\leq0}$). This results in a zero global effect with high heterogeneity. The regional effect should be divided into two subregions: $x_3>0$ and $x_3 \\leq 0$, leading to two regional effects with zero heterogeneity: $3x_1$ and $-3x_1$.\n",
                 "\n",
```

### Comparing `effector-0.0.272/synthetic-examples/02_regional_shapdp.ipynb` & `effector-0.0.273/synthetic-examples/02_regional_shapdp.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/03_regional_effects_synthetic_f.ipynb` & `effector-0.0.273/synthetic-examples/03_regional_effects_synthetic_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/synthetic-examples/04_regional_effects_real_f.ipynb` & `effector-0.0.273/synthetic-examples/04_regional_effects_real_f.ipynb`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/tests/test_functional.py` & `effector-0.0.273/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/tests/test_functional_gam.py` & `effector-0.0.273/tests/test_functional_gam.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/tests/test_functional_linear.py` & `effector-0.0.273/tests/test_functional_linear.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/tests/test_regional_methods.py` & `effector-0.0.273/tests/test_regional_methods.py`

 * *Files identical despite different names*

### Comparing `effector-0.0.272/tests/test_unit.py` & `effector-0.0.273/tests/test_unit.py`

 * *Files identical despite different names*

