# Comparing `tmp/mist_medical-0.4.6a0.tar.gz` & `tmp/mist_medical-0.4.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mist_medical-0.4.6a0.tar", last modified: Wed Apr 24 19:44:17 2024, max compression
+gzip compressed data, was "mist_medical-0.4.7a0.tar", last modified: Mon May 13 15:39:58 2024, max compression
```

## Comparing `mist_medical-0.4.6a0.tar` & `mist_medical-0.4.7a0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/analyze_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/analyze_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/analyze_data/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/conversion_tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/csv.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/conversion_tools/msd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/convert_to_mist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/data_loading/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/data_loading/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/data_loading/dali_loader.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/eval_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.430225 mist_medical-0.4.6a0/mist/evaluate_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/evaluate_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/evaluate_preds/evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/inference/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/inference/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11828 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/inference/main_inference.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/metrics/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/lookup_tables.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/attn_unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/get_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/layers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/mgnets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/nnunet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/swin_unetr.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/models/unet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/post_preds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/postprocess_preds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/postprocess_preds/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/postprocess_preds/postprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/preprocess_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/preprocess_data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/preprocess_data/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.434224 mist_medical-0.4.6a0/mist/runtime/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/args.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/progress_bar.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/runtime/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/mist/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/analyze_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/preprocess_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/run_all_entrypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/mist/scripts/train_entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/mist_medical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 19:44:17.000000 mist_medical-0.4.6a0/mist_medical.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 19:44:17.438225 mist_medical-0.4.6a0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-04-24 19:44:04.000000 mist_medical-0.4.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2554 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/analyze_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/analyze_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16741 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/analyze_data/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/conversion_tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3775 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5762 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/conversion_tools/msd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1313 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/convert_to_mist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/data_loading/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/data_loading/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12303 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/data_loading/dali_loader.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1552 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/eval_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/evaluate_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/evaluate_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5350 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/evaluate_preds/evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/inference/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/inference/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11958 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/inference/main_inference.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3689 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.135692 mist_medical-0.4.7a0/mist/metrics/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22757 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/lookup_tables.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18301 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/attn_unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9112 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/get_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6272 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/layers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15447 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/mgnets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16466 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/nnunet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      589 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/swin_unetr.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8118 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/models/unet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2488 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/post_preds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/postprocess_preds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/postprocess_preds/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8387 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/postprocess_preds/postprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2588 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/preprocess_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/preprocess_data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10643 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/preprocess_data/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/runtime/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8099 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/args.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7534 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1849 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/progress_bar.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21551 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22443 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/runtime/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.139692 mist_medical-0.4.7a0/mist/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      291 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/analyze_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      372 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/preprocess_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      865 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/run_all_entrypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      863 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/mist/scripts/train_entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/mist_medical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 15:39:58.000000 mist_medical-0.4.7a0/mist_medical.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2132 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:39:58.143692 mist_medical-0.4.7a0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       68 2024-05-13 15:39:49.000000 mist_medical-0.4.7a0/setup.py
```

### Comparing `mist_medical-0.4.6a0/PKG-INFO` & `mist_medical-0.4.7a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.6a0
+Version: 0.4.7a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
```

### Comparing `mist_medical-0.4.6a0/README.md` & `mist_medical-0.4.7a0/README.md`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/analyze_data/analyze.py` & `mist_medical-0.4.7a0/mist/analyze_data/analyze.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/conversion_tools/csv.py` & `mist_medical-0.4.7a0/mist/conversion_tools/csv.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/conversion_tools/msd.py` & `mist_medical-0.4.7a0/mist/conversion_tools/msd.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/convert_to_mist.py` & `mist_medical-0.4.7a0/mist/convert_to_mist.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/data_loading/dali_loader.py` & `mist_medical-0.4.7a0/mist/data_loading/dali_loader.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/eval_preds.py` & `mist_medical-0.4.7a0/mist/eval_preds.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/evaluate_preds/evaluate.py` & `mist_medical-0.4.7a0/mist/evaluate_preds/evaluate.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/inference/main_inference.py` & `mist_medical-0.4.7a0/mist/inference/main_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,17 @@
     pred.set_direction(og_ants_img.direction)
     pred.set_origin(og_ants_img.origin)
 
     # Appropriately pad back to original size
     if fg_bbox is not None:
         pred = decrop_from_fg(pred, fg_bbox)
 
+    # FIX: Copy header from original image onto the prediction so they match
+    pred = og_ants_img.new_image_like(pred.numpy())
+
     return pred
 
 
 def predict_single_example(torch_img,
                            og_ants_img,
                            config,
                            models,
```

### Comparing `mist_medical-0.4.6a0/mist/main.py` & `mist_medical-0.4.7a0/mist/main.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/metrics/lookup_tables.py` & `mist_medical-0.4.7a0/mist/metrics/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/metrics/metrics.py` & `mist_medical-0.4.7a0/mist/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/attn_unet.py` & `mist_medical-0.4.7a0/mist/models/attn_unet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/get_model.py` & `mist_medical-0.4.7a0/mist/models/get_model.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/layers.py` & `mist_medical-0.4.7a0/mist/models/layers.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/mgnets.py` & `mist_medical-0.4.7a0/mist/models/mgnets.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/nnunet.py` & `mist_medical-0.4.7a0/mist/models/nnunet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/swin_unetr.py` & `mist_medical-0.4.7a0/mist/models/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/models/unet.py` & `mist_medical-0.4.7a0/mist/models/unet.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/post_preds.py` & `mist_medical-0.4.7a0/mist/post_preds.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/postprocess_preds/postprocess.py` & `mist_medical-0.4.7a0/mist/postprocess_preds/postprocess.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/predict.py` & `mist_medical-0.4.7a0/mist/predict.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/preprocess_data/preprocess.py` & `mist_medical-0.4.7a0/mist/preprocess_data/preprocess.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/runtime/args.py` & `mist_medical-0.4.7a0/mist/runtime/args.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/runtime/loss.py` & `mist_medical-0.4.7a0/mist/runtime/loss.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/runtime/progress_bar.py` & `mist_medical-0.4.7a0/mist/runtime/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/runtime/run.py` & `mist_medical-0.4.7a0/mist/runtime/run.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/runtime/utils.py` & `mist_medical-0.4.7a0/mist/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/scripts/run_all_entrypoint.py` & `mist_medical-0.4.7a0/mist/scripts/run_all_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist/scripts/train_entrypoint.py` & `mist_medical-0.4.7a0/mist/scripts/train_entrypoint.py`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/mist_medical.egg-info/PKG-INFO` & `mist_medical-0.4.7a0/mist_medical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mist-medical
-Version: 0.4.6a0
+Version: 0.4.7a0
 Summary: MIST is a simple, fully automated framework for 3D medical imaging segmentation.
 Author: Rice University, The University of Texas MD Anderson Cancer Center
 Author-email: Adrian Celaya <aecelaya@rice.edu>, David Fuentes <dtfuentes@mdanderson.org>, Beatrice Riviere <riviere@rice.edu>, Evan Lim <EMLim@mdanderson.org>, Rachel Glenn <rglenn1@mdanderson.org>, Alex Balsells <atb8@rice.edu>
 License: Medical Imaging Segmentation Toolkit (MIST) (c) 2024 by Adrian Celaya
         is licenced under Attribution-NonCommercial-ShareAlike 4.0 International.
         To view a copy of this license, visit http://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: homepage, https://github.com/aecelaya/MIST
```

### Comparing `mist_medical-0.4.6a0/mist_medical.egg-info/SOURCES.txt` & `mist_medical-0.4.7a0/mist_medical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mist_medical-0.4.6a0/pyproject.toml` & `mist_medical-0.4.7a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mist-medical"
-version = "0.4.6-alpha"
+version = "0.4.7-alpha"
 requires-python = ">= 3.8"
 description = "MIST is a simple, fully automated framework for 3D medical imaging segmentation."
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Adrian Celaya", email = "aecelaya@rice.edu"},
     {name = "David Fuentes", email = "dtfuentes@mdanderson.org"},
```

