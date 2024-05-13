# Comparing `tmp/PipelineTS-0.3.8.tar.gz` & `tmp/PipelineTS-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PipelineTS-0.3.8.tar", last modified: Tue Oct 31 03:39:23 2023, max compression
+gzip compressed data, was "PipelineTS-0.3.9.tar", last modified: Tue Oct 31 10:15:49 2023, max compression
```

## Comparing `PipelineTS-0.3.8.tar` & `PipelineTS-0.3.9.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.921123 PipelineTS-0.3.8/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-03-20 06:25:30.000000 PipelineTS-0.3.8/LICENSE
--rw-r--r--   0 guobingming   (501) staff       (20)    13702 2023-10-31 03:39:23.920635 PipelineTS-0.3.8/PKG-INFO
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.907644 PipelineTS-0.3.8/PipelineTS/
--rw-r--r--   0 guobingming   (501) staff       (20)       50 2023-10-27 09:45:45.000000 PipelineTS-0.3.8/PipelineTS/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.909377 PipelineTS-0.3.8/PipelineTS/base/
--rw-r--r--   0 guobingming   (501) staff       (20)      188 2023-10-26 03:49:21.000000 PipelineTS-0.3.8/PipelineTS/base/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    12411 2023-10-27 09:06:59.000000 PipelineTS-0.3.8/PipelineTS/base/base.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5878 2023-10-26 07:15:46.000000 PipelineTS-0.3.8/PipelineTS/base/sps_nn_model_base.py
--rw-r--r--   0 guobingming   (501) staff       (20)      233 2023-09-27 07:38:18.000000 PipelineTS-0.3.8/PipelineTS/dataset.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.909707 PipelineTS-0.3.8/PipelineTS/io/
--rw-r--r--   0 guobingming   (501) staff       (20)     8798 2023-10-27 15:26:07.000000 PipelineTS-0.3.8/PipelineTS/io/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)      335 2023-10-09 07:25:43.000000 PipelineTS-0.3.8/PipelineTS/metrics.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.911178 PipelineTS-0.3.8/PipelineTS/ml_model/
--rw-r--r--   0 guobingming   (501) staff       (20)      290 2023-10-08 15:36:29.000000 PipelineTS-0.3.8/PipelineTS/ml_model/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    13061 2023-10-25 09:35:13.000000 PipelineTS-0.3.8/PipelineTS/ml_model/gbdt.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6525 2023-10-26 03:21:27.000000 PipelineTS-0.3.8/PipelineTS/ml_model/multi_output_model.py
--rw-r--r--   0 guobingming   (501) staff       (20)     6980 2023-10-26 07:04:00.000000 PipelineTS-0.3.8/PipelineTS/ml_model/wide_gbrt.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.915558 PipelineTS-0.3.8/PipelineTS/nn_model/
--rw-r--r--   0 guobingming   (501) staff       (20)      613 2023-10-20 10:37:44.000000 PipelineTS-0.3.8/PipelineTS/nn_model/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4613 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/d_linear.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1974 2023-10-30 15:30:51.000000 PipelineTS-0.3.8/PipelineTS/nn_model/gau.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5015 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/n_beats.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4947 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/n_hits.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4645 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/n_linear.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2029 2023-10-30 15:30:51.000000 PipelineTS-0.3.8/PipelineTS/nn_model/rnn.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1941 2023-10-30 15:30:51.000000 PipelineTS-0.3.8/PipelineTS/nn_model/seg_rnn.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4711 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/tcn.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5129 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/tft.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5187 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/tide.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2088 2023-10-30 15:30:51.000000 PipelineTS-0.3.8/PipelineTS/nn_model/time2vec.py
--rw-r--r--   0 guobingming   (501) staff       (20)     5029 2023-10-25 10:04:55.000000 PipelineTS-0.3.8/PipelineTS/nn_model/transformer.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.917058 PipelineTS-0.3.8/PipelineTS/pipeline/
--rw-r--r--   0 guobingming   (501) staff       (20)      120 2023-10-17 10:25:11.000000 PipelineTS-0.3.8/PipelineTS/pipeline/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    15176 2023-10-30 15:32:29.000000 PipelineTS-0.3.8/PipelineTS/pipeline/pipeline.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2189 2023-10-17 10:25:11.000000 PipelineTS-0.3.8/PipelineTS/pipeline/pipeline_configs.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1203 2023-10-20 11:03:33.000000 PipelineTS-0.3.8/PipelineTS/pipeline/pipeline_models.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.917344 PipelineTS-0.3.8/PipelineTS/plot/
--rw-r--r--   0 guobingming   (501) staff       (20)     2566 2023-10-27 09:47:08.000000 PipelineTS-0.3.8/PipelineTS/plot/__init__.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.917902 PipelineTS-0.3.8/PipelineTS/preprocessing/
--rw-r--r--   0 guobingming   (501) staff       (20)       28 2023-10-26 05:59:16.000000 PipelineTS-0.3.8/PipelineTS/preprocessing/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1472 2023-10-26 06:04:56.000000 PipelineTS-0.3.8/PipelineTS/preprocessing/scalers.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.918694 PipelineTS-0.3.8/PipelineTS/statistic_model/
--rw-r--r--   0 guobingming   (501) staff       (20)      196 2023-10-17 09:50:26.000000 PipelineTS-0.3.8/PipelineTS/statistic_model/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2371 2023-10-25 02:50:26.000000 PipelineTS-0.3.8/PipelineTS/statistic_model/auto_arima.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2830 2023-10-25 02:50:26.000000 PipelineTS-0.3.8/PipelineTS/statistic_model/prophet.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 03:39:23.908680 PipelineTS-0.3.8/PipelineTS.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    13702 2023-10-31 03:39:23.000000 PipelineTS-0.3.8/PipelineTS.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)     1313 2023-10-31 03:39:23.000000 PipelineTS-0.3.8/PipelineTS.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-10-31 03:39:23.000000 PipelineTS-0.3.8/PipelineTS.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-10-09 03:21:14.000000 PipelineTS-0.3.8/PipelineTS.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      783 2023-10-31 03:39:23.000000 PipelineTS-0.3.8/PipelineTS.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       11 2023-10-31 03:39:23.000000 PipelineTS-0.3.8/PipelineTS.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    10777 2023-10-31 03:31:26.000000 PipelineTS-0.3.8/README.md
--rw-r--r--   0 guobingming   (501) staff       (20)      104 2023-10-17 08:55:37.000000 PipelineTS-0.3.8/pyproject.toml
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2023-10-31 03:39:23.921197 PipelineTS-0.3.8/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1594 2023-10-27 09:45:45.000000 PipelineTS-0.3.8/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.150900 PipelineTS-0.3.9/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-03-20 06:25:30.000000 PipelineTS-0.3.9/LICENSE
+-rw-r--r--   0 guobingming   (501) staff       (20)    13885 2023-10-31 10:15:49.150595 PipelineTS-0.3.9/PKG-INFO
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.138109 PipelineTS-0.3.9/PipelineTS/
+-rw-r--r--   0 guobingming   (501) staff       (20)       50 2023-10-31 07:16:49.000000 PipelineTS-0.3.9/PipelineTS/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.140355 PipelineTS-0.3.9/PipelineTS/base/
+-rw-r--r--   0 guobingming   (501) staff       (20)      188 2023-10-26 03:49:21.000000 PipelineTS-0.3.9/PipelineTS/base/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    12411 2023-10-27 09:06:59.000000 PipelineTS-0.3.9/PipelineTS/base/base.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5878 2023-10-26 07:15:46.000000 PipelineTS-0.3.9/PipelineTS/base/sps_nn_model_base.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      233 2023-09-27 07:38:18.000000 PipelineTS-0.3.9/PipelineTS/dataset.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.140835 PipelineTS-0.3.9/PipelineTS/io/
+-rw-r--r--   0 guobingming   (501) staff       (20)     8798 2023-10-27 15:26:07.000000 PipelineTS-0.3.9/PipelineTS/io/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      335 2023-10-09 07:25:43.000000 PipelineTS-0.3.9/PipelineTS/metrics.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.142231 PipelineTS-0.3.9/PipelineTS/ml_model/
+-rw-r--r--   0 guobingming   (501) staff       (20)      290 2023-10-08 15:36:29.000000 PipelineTS-0.3.9/PipelineTS/ml_model/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    13061 2023-10-25 09:35:13.000000 PipelineTS-0.3.9/PipelineTS/ml_model/gbdt.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6525 2023-10-26 03:21:27.000000 PipelineTS-0.3.9/PipelineTS/ml_model/multi_output_model.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     6980 2023-10-26 07:04:00.000000 PipelineTS-0.3.9/PipelineTS/ml_model/wide_gbrt.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.145981 PipelineTS-0.3.9/PipelineTS/nn_model/
+-rw-r--r--   0 guobingming   (501) staff       (20)      613 2023-10-20 10:37:44.000000 PipelineTS-0.3.9/PipelineTS/nn_model/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4613 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/d_linear.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1974 2023-10-30 15:30:51.000000 PipelineTS-0.3.9/PipelineTS/nn_model/gau.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5015 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/n_beats.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4947 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/n_hits.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4645 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/n_linear.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2029 2023-10-30 15:30:51.000000 PipelineTS-0.3.9/PipelineTS/nn_model/rnn.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1941 2023-10-30 15:30:51.000000 PipelineTS-0.3.9/PipelineTS/nn_model/seg_rnn.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4711 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/tcn.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5129 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/tft.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5187 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/tide.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2089 2023-10-31 08:50:23.000000 PipelineTS-0.3.9/PipelineTS/nn_model/time2vec.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     5029 2023-10-25 10:04:55.000000 PipelineTS-0.3.9/PipelineTS/nn_model/transformer.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.147264 PipelineTS-0.3.9/PipelineTS/pipeline/
+-rw-r--r--   0 guobingming   (501) staff       (20)      120 2023-10-17 10:25:11.000000 PipelineTS-0.3.9/PipelineTS/pipeline/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    16393 2023-10-31 08:06:28.000000 PipelineTS-0.3.9/PipelineTS/pipeline/pipeline.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2751 2023-10-31 09:59:52.000000 PipelineTS-0.3.9/PipelineTS/pipeline/pipeline_configs.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1203 2023-10-20 11:03:33.000000 PipelineTS-0.3.9/PipelineTS/pipeline/pipeline_models.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.147515 PipelineTS-0.3.9/PipelineTS/plot/
+-rw-r--r--   0 guobingming   (501) staff       (20)     2566 2023-10-27 09:47:08.000000 PipelineTS-0.3.9/PipelineTS/plot/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.147976 PipelineTS-0.3.9/PipelineTS/preprocessing/
+-rw-r--r--   0 guobingming   (501) staff       (20)       28 2023-10-26 05:59:16.000000 PipelineTS-0.3.9/PipelineTS/preprocessing/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1472 2023-10-26 06:04:56.000000 PipelineTS-0.3.9/PipelineTS/preprocessing/scalers.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.148721 PipelineTS-0.3.9/PipelineTS/statistic_model/
+-rw-r--r--   0 guobingming   (501) staff       (20)      196 2023-10-17 09:50:26.000000 PipelineTS-0.3.9/PipelineTS/statistic_model/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2371 2023-10-25 02:50:26.000000 PipelineTS-0.3.9/PipelineTS/statistic_model/auto_arima.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2830 2023-10-25 02:50:26.000000 PipelineTS-0.3.9/PipelineTS/statistic_model/prophet.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2023-10-31 10:15:49.139302 PipelineTS-0.3.9/PipelineTS.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    13885 2023-10-31 10:15:49.000000 PipelineTS-0.3.9/PipelineTS.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)     1298 2023-10-31 10:15:49.000000 PipelineTS-0.3.9/PipelineTS.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-10-31 10:15:49.000000 PipelineTS-0.3.9/PipelineTS.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2023-10-09 03:21:14.000000 PipelineTS-0.3.9/PipelineTS.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      783 2023-10-31 10:15:49.000000 PipelineTS-0.3.9/PipelineTS.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       11 2023-10-31 10:15:49.000000 PipelineTS-0.3.9/PipelineTS.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    10960 2023-10-31 09:54:38.000000 PipelineTS-0.3.9/README.md
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2023-10-31 10:15:49.150945 PipelineTS-0.3.9/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1594 2023-10-31 07:16:49.000000 PipelineTS-0.3.9/setup.py
```

### Comparing `PipelineTS-0.3.8/LICENSE` & `PipelineTS-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PKG-INFO` & `PipelineTS-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PipelineTS
-Version: 0.3.8
+Version: 0.3.9
 Summary: One-stop time series analysis tool, supporting time series data preprocessing, feature engineering, model training, model evaluation, model prediction, etc. Based on spinesTS and darts.
 Home-page: https://github.com/BirchKwok/PipelineTS
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: time series forecasting
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: xgboost>=1.6.0
 Requires-Dist: darts>=0.24.0
 Requires-Dist: catboost>=1.2.2
 Requires-Dist: lightgbm>=3.3.5
-Requires-Dist: spinesTS>=0.4.1
+Requires-Dist: spinesTS>=0.4.2
 Requires-Dist: frozendict>=2.3.0
 Requires-Dist: spinesUtils>=0.3.12
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: torch>=1.8.0
 Requires-Dist: MAPIE>=0.7.0
 Requires-Dist: cloudpickle>=2.2.1
 Provides-Extra: all
@@ -38,15 +38,15 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3; extra == "all"
 Requires-Dist: pandas>=2.0.3; extra == "all"
 Requires-Dist: scikit-learn>=1.3.0; extra == "all"
 Requires-Dist: xgboost>=1.6.0; extra == "all"
 Requires-Dist: darts>=0.24.0; extra == "all"
 Requires-Dist: catboost>=1.2.2; extra == "all"
 Requires-Dist: lightgbm>=3.3.5; extra == "all"
-Requires-Dist: spinesTS>=0.4.1; extra == "all"
+Requires-Dist: spinesTS>=0.4.2; extra == "all"
 Requires-Dist: frozendict>=2.3.0; extra == "all"
 Requires-Dist: spinesUtils>=0.3.12; extra == "all"
 Requires-Dist: tabulate>=0.8.9; extra == "all"
 Requires-Dist: torch>=1.8.0; extra == "all"
 Requires-Dist: MAPIE>=0.7.0; extra == "all"
 Requires-Dist: cloudpickle>=2.2.1; extra == "all"
 Requires-Dist: prophet>=1.1.4; extra == "all"
@@ -55,39 +55,39 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3; extra == "core"
 Requires-Dist: pandas>=2.0.3; extra == "core"
 Requires-Dist: scikit-learn>=1.3.0; extra == "core"
 Requires-Dist: xgboost>=1.6.0; extra == "core"
 Requires-Dist: darts>=0.24.0; extra == "core"
 Requires-Dist: catboost>=1.2.2; extra == "core"
 Requires-Dist: lightgbm>=3.3.5; extra == "core"
-Requires-Dist: spinesTS>=0.4.1; extra == "core"
+Requires-Dist: spinesTS>=0.4.2; extra == "core"
 Requires-Dist: frozendict>=2.3.0; extra == "core"
 Requires-Dist: spinesUtils>=0.3.12; extra == "core"
 Requires-Dist: tabulate>=0.8.9; extra == "core"
 Requires-Dist: torch>=1.8.0; extra == "core"
 Requires-Dist: MAPIE>=0.7.0; extra == "core"
 Requires-Dist: cloudpickle>=2.2.1; extra == "core"
 
 # PipelineTS
-[中文文档](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
+[\[中文文档\]](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
 
 One-stop time series analysis tool, supporting time series data preprocessing, feature engineering, model training, model evaluation, model prediction, etc. Based on spinesTS and darts.
 ## Installation
 
 ```bash
 # if you don't want to use the prophet model
 # run this
 python -m pip install PipelineTS[core]
 
 # if you want to use all models
 # run this
 python -m pip install PipelineTS[all]
 ```
 
-## Quick Start [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
+## Quick Start [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
 
 ### list all available models
 ```python
 from PipelineTS.dataset import LoadWebSales
 
 init_data = LoadWebSales()[['date', 'type_a']]
 
@@ -143,15 +143,15 @@
 pipeline.fit(data, valid_data=valid_data)
 
 # use best model to predict next 30 steps data point
 res = pipeline.predict(30)
 
 ```
 ## Training and prediction of a single model
-###  Without predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
+###  Without predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
 
 #### Data Preprocessing
 
 ```python
 
 from PipelineTS.dataset import LoadMessagesSentDataSets
 import pandas as pd
@@ -194,15 +194,15 @@
     time_col=time_col, target_col=target_col, lags=lags, random_state=42, 
     quantile=0.9, enable_progress_bar=False, enable_model_summary=False
 )
 tide.fit(data)
 tide.predict(n)
 ```
 
-### With predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
+### With predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
 ```python
 tide.predict(n, series=valid_data)
 ```
 
 
 ## PipelineTS Module
 
@@ -211,46 +211,48 @@
 from xgboost import XGBRegressor
 from catboost import CatBoostRegressor
 from PipelineTS.pipeline import ModelPipeline, PipelineConfigs
 
 # If you want to try multiple configurations of a model at once for comparison or tuning purposes, you can use `PipelineConfigs`.
 # This feature allows for customizing the models returned by each `ModelPipeline.list_all_available_models()` call.
 # The first one is the name of the model, which needs to be in the list of available models provided by PipelineTS.list_all_available_models(). 
-# The second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
+# If you want to customize the name of the model, then the second argument can be a string of the model name, 
+# otherwise, the second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
 # The remaining keys will be automatically filled with default parameters.
 # Among them, 'init_configs' represents the initialization parameters of the model, 'fit_configs' represents the parameters during model training, 
 # and 'predict_configs' represents the parameters during model prediction.
+
 pipeline_configs = PipelineConfigs([
-    ('lightgbm', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
+    ('lightgbm', 'lightgbm_linear_tree', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
     ('multi_output_model', {'init_configs': {'verbose': -1}}),
     ('multi_step_model', {'init_configs': {'verbose': -1}}),
     ('multi_output_model', {
         'init_configs': {'estimator': XGBRegressor, 'random_state': 42, 'kwargs': {'verbosity': 0}}
     }
      ),
     ('multi_output_model', {
         'init_configs': {'estimator': CatBoostRegressor, 'random_state': 42, 'verbose': False}
     }
      ),
 ])
 ```
 <table>
 <thead>
-<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_with_index  </th><th>model_configs                                                                                                                                                    </th></tr>
+<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_after_rename  </th><th>model_configs                                                                                                                                                    </th></tr>
 </thead>
 <tbody>
-<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_1             </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
-<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1   </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
-<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
-<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
-<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_linear_tree     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
+<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
+<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
+<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1       </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
 </tbody>
 </table>
 
-### Non-Interval Forecasting [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
+### Non-Interval Forecasting [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
@@ -294,15 +296,15 @@
 
 plot_data_period(init_data.iloc[-100:, :], prediction, 
                  time_col=time_col, target_col=target_col)
 ```
 
 ![image1](https://github.com/BirchKwok/PipelineTS/blob/main/pics/pic2.png)
 
-### Interval prediction [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
+### Interval prediction [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
```

### Comparing `PipelineTS-0.3.8/PipelineTS/base/base.py` & `PipelineTS-0.3.9/PipelineTS/base/base.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/base/sps_nn_model_base.py` & `PipelineTS-0.3.9/PipelineTS/base/sps_nn_model_base.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/io/__init__.py` & `PipelineTS-0.3.9/PipelineTS/io/__init__.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/ml_model/gbdt.py` & `PipelineTS-0.3.9/PipelineTS/ml_model/gbdt.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/ml_model/multi_output_model.py` & `PipelineTS-0.3.9/PipelineTS/ml_model/multi_output_model.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/ml_model/wide_gbrt.py` & `PipelineTS-0.3.9/PipelineTS/ml_model/wide_gbrt.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/__init__.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/__init__.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/d_linear.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/d_linear.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/gau.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/gau.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/n_beats.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/n_beats.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/n_hits.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/n_hits.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/n_linear.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/n_linear.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/rnn.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/rnn.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/seg_rnn.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/seg_rnn.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/tcn.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/tcn.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/tft.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/tft.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/tide.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/tide.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/time2vec.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/time2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             time_col,
             target_col,
             lags=30,
             quantile=0.9,
             random_state=None,
             flip_features=False,
             kernel_size=3,
-            learning_rate=0.01,
+            learning_rate=0.001,
             accelerator='auto',
             verbose=False,
             epochs=1000,
             batch_size='auto',
             patience=100,
             min_delta=0,
             lr_scheduler='CosineAnnealingLR',
```

### Comparing `PipelineTS-0.3.8/PipelineTS/nn_model/transformer.py` & `PipelineTS-0.3.9/PipelineTS/nn_model/transformer.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/pipeline/pipeline.py` & `PipelineTS-0.3.9/PipelineTS/pipeline/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import sys
 from copy import deepcopy
 import gc
 
 import pandas as pd
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from frozendict import frozendict
 
+from spinesTS.base._torch_mixin import detect_available_device
 from spinesTS.metrics import mae
 from spinesTS.utils import func_has_params
 from spinesUtils import ParameterTypeAssert, ParameterValuesAssert
 from spinesUtils.preprocessing import gc_collector
 from spinesUtils.asserts import (
     check_obj_is_function,
     augmented_isinstance,
@@ -23,14 +25,20 @@
 from PipelineTS.metrics import quantile_acc
 from PipelineTS.pipeline.pipeline_models import get_all_available_models
 from PipelineTS.pipeline.pipeline_configs import PipelineConfigs
 
 
 # TODO: 传入数据，进行数据采集周期检验，看看是否有漏数据，如果有，进行插值（可选），如果有异常值，进行噪音去除（可选）
 
+def update_dict_without_conflict(dict_a, dict_b):
+    for i in dict_b:
+        if i not in dict_a:
+            dict_a[i] = dict_b[i]
+    return dict_a
+
 
 class ModelPipeline:
     @ParameterTypeAssert({
         'time_col': str,
         'target_col': str,
         'lags': int,
         'with_quantile_prediction': bool,
@@ -39,15 +47,15 @@
         'metric_less_is_better': bool,
         'configs': (None, PipelineConfigs),
         'random_state': (int, None),
         'verbose': (bool, int),
         'include_init_config_model': bool,
         'use_standard_scale': (bool, None),
         'accelerator': (str, None),
-        'cv': int
+        'cv': int,
     }, 'Pipeline')
     @ParameterValuesAssert({
         'metric': lambda s: check_obj_is_function(s),
         'accelerator': (
                 lambda s: s in ("cpu", "gpu", "tpu", "ipu", "hpu", "mps", "auto", "cuda")
                           or augmented_isinstance(s, None)
         )
@@ -121,22 +129,34 @@
         self.accelerator = accelerator
         self.cv = cv
 
         self._timer = Timer()
 
         self._model_init_kwargs = {}
 
+        model_init_kwargs = update_dict_without_conflict(model_init_kwargs,
+                                                         {
+                                                             'multi_output_model__verbose': -1,
+                                                             'multi_step_model__verbose': -1,
+                                                             'lightgbm__verbose': -1,
+                                                             'wide_gbrt__verbose': -1,
+                                                             'catboost__verbose': False,
+                                                             'xgboost__verbose': 0
+                                                         })
+
         for k, v in model_init_kwargs.items():
             raise_if(ValueError, '__' not in k,
                      f"{k} must has double underline.")
 
             raise_if(ValueError, k.split('__')[0] not in self._available_models,
                      f"{k.split('__')[0]} is not a valid model name")
             self._model_init_kwargs[k] = v
 
+        sys.stderr.write(detect_available_device(self.accelerator)[1]+'\n\n')
+
     def _initial_models(self):
         initial_models = []
         ms = tuple(sorted(self._available_models.items(), key=lambda s: s[0])) if self._given_models is None else (
             drop_duplicates_with_order([(k, self._available_models[k]) for k in self._given_models]))
 
         # 模型训练顺序
         for (model_name, model) in ms:
@@ -395,27 +415,29 @@
                 if model_name == md_name:
                     return model.all_configs
 
     @ParameterTypeAssert({
         'n': int,
         'model_name': (None, str)
     })
-    def predict(self, n, model_name=None):
+    def predict(self, n, series=None, model_name=None):
         """By default, the best model is used for prediction
 
         :parameter
         n: predict steps
+        series: the sequence to predict from the last time point in the sequence,
+                accepting only a pandas DataFrame type
         model_name: str, model's name, specifying the model used, default None
 
         :return
         pd.DataFrame
         """
         if model_name is not None:
-            res = self.get_model(model_name).predict(n)
+            res = self.get_model(model_name).predict(n, series=series)
         else:
-            res = self.best_model_.predict(n)
+            res = self.best_model_.predict(n, series=series)
 
         for i in res.columns:
             if i.startswith(self.target_col):
                 res = self._inverse_data(res, columns=i)
 
         return res
```

### Comparing `PipelineTS-0.3.8/PipelineTS/pipeline/pipeline_configs.py` & `PipelineTS-0.3.9/PipelineTS/pipeline/pipeline_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,49 +10,67 @@
 
 from PipelineTS.pipeline.pipeline_models import get_all_available_models
 
 
 MODELS = get_all_available_models()
 
 
+def configs_check(configs):
+    condition_a = all(
+        isinstance(i, tuple) and 2 <= len(i) <= 3 and isinstance(i[-1], dict) for i in configs
+    )
+
+    condition_b = all(
+       isinstance(i[0], str) if len(i) == 2 else isinstance(i[0], str) and isinstance(i[1], str) for i in configs
+    )
+
+    return condition_a and condition_b
+
+
 class PipelineConfigs:
     @ParameterTypeAssert({
         'configs': list
-    })
+    }, 'PipelineConfigs')
     @ParameterValuesAssert({
-        'configs': lambda s: all(isinstance(i, tuple) and len(i) == 2 and isinstance(i[1], dict) for i in s)
-    })
+        'configs': configs_check
+    }, 'PipelineConfigs')
     def __init__(self, configs):
         self.sub_configs = {'init_configs': {}, 'fit_configs': {}, 'predict_configs': {}}
 
         _to_process_configs = drop_duplicates_with_order(configs)
 
         self.configs = []
         for models_group in reindex_iterable_object(_to_process_configs, key=lambda s: s[0], index_start=1):
-            for (index, (model_name, model_configs)) in models_group:
+            for (index, (*model_name_list, model_configs)) in models_group:
+                model_name = model_name_list[0]
+                if len(model_name_list) == 2:
+                    model_name_after_rename = model_name_list[1]
+                else:
+                    model_name_after_rename = f"{model_name}_{index}"
+
                 if not all(i in self.sub_configs for i in model_configs):
                     raise KeyError
 
                 if model_name not in MODELS:
                     raise KeyError
 
                 if len(model_configs) < 3:
                     model_configs.update({k: self.sub_configs[k]
                                           for k in self.sub_configs if k not in model_configs})
 
-                self.configs.append((model_name, f"{model_name}_{index}", model_configs))
+                self.configs.append((model_name, model_name_after_rename, model_configs))
 
         if is_in_ipython():
             display(
-                tabulate(self.configs, headers=['model_name', 'model_name_with_index', 'model_configs'],
+                tabulate(self.configs, headers=['model_name', 'model_name_after_rename', 'model_configs'],
                          tablefmt='html', colalign=("right", "left", "left"), showindex='always')
             )
         else:
             print(
-                tabulate(self.configs, headers=['model_name', 'model_name_with_index', 'model_configs'],
+                tabulate(self.configs, headers=['model_name', 'model_name_after_rename', 'model_configs'],
                          tablefmt='pretty', colalign=("right", "left", "left"), showindex='always')
             )
 
     def get_configs(self, model_name_after_rename):
-        for (model_name, mnwi, model_configs) in self.configs:
-            if model_name_after_rename == mnwi:
+        for (model_name, mnar, model_configs) in self.configs:
+            if model_name_after_rename == mnar:
                 return model_configs
```

### Comparing `PipelineTS-0.3.8/PipelineTS/pipeline/pipeline_models.py` & `PipelineTS-0.3.9/PipelineTS/pipeline/pipeline_models.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/plot/__init__.py` & `PipelineTS-0.3.9/PipelineTS/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/preprocessing/scalers.py` & `PipelineTS-0.3.9/PipelineTS/preprocessing/scalers.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/statistic_model/auto_arima.py` & `PipelineTS-0.3.9/PipelineTS/statistic_model/auto_arima.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS/statistic_model/prophet.py` & `PipelineTS-0.3.9/PipelineTS/statistic_model/prophet.py`

 * *Files identical despite different names*

### Comparing `PipelineTS-0.3.8/PipelineTS.egg-info/PKG-INFO` & `PipelineTS-0.3.9/PipelineTS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PipelineTS
-Version: 0.3.8
+Version: 0.3.9
 Summary: One-stop time series analysis tool, supporting time series data preprocessing, feature engineering, model training, model evaluation, model prediction, etc. Based on spinesTS and darts.
 Home-page: https://github.com/BirchKwok/PipelineTS
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: time series forecasting
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
@@ -22,15 +22,15 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: xgboost>=1.6.0
 Requires-Dist: darts>=0.24.0
 Requires-Dist: catboost>=1.2.2
 Requires-Dist: lightgbm>=3.3.5
-Requires-Dist: spinesTS>=0.4.1
+Requires-Dist: spinesTS>=0.4.2
 Requires-Dist: frozendict>=2.3.0
 Requires-Dist: spinesUtils>=0.3.12
 Requires-Dist: tabulate>=0.8.9
 Requires-Dist: torch>=1.8.0
 Requires-Dist: MAPIE>=0.7.0
 Requires-Dist: cloudpickle>=2.2.1
 Provides-Extra: all
@@ -38,15 +38,15 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3; extra == "all"
 Requires-Dist: pandas>=2.0.3; extra == "all"
 Requires-Dist: scikit-learn>=1.3.0; extra == "all"
 Requires-Dist: xgboost>=1.6.0; extra == "all"
 Requires-Dist: darts>=0.24.0; extra == "all"
 Requires-Dist: catboost>=1.2.2; extra == "all"
 Requires-Dist: lightgbm>=3.3.5; extra == "all"
-Requires-Dist: spinesTS>=0.4.1; extra == "all"
+Requires-Dist: spinesTS>=0.4.2; extra == "all"
 Requires-Dist: frozendict>=2.3.0; extra == "all"
 Requires-Dist: spinesUtils>=0.3.12; extra == "all"
 Requires-Dist: tabulate>=0.8.9; extra == "all"
 Requires-Dist: torch>=1.8.0; extra == "all"
 Requires-Dist: MAPIE>=0.7.0; extra == "all"
 Requires-Dist: cloudpickle>=2.2.1; extra == "all"
 Requires-Dist: prophet>=1.1.4; extra == "all"
@@ -55,39 +55,39 @@
 Requires-Dist: numpy<=1.25.0,>=1.24.3; extra == "core"
 Requires-Dist: pandas>=2.0.3; extra == "core"
 Requires-Dist: scikit-learn>=1.3.0; extra == "core"
 Requires-Dist: xgboost>=1.6.0; extra == "core"
 Requires-Dist: darts>=0.24.0; extra == "core"
 Requires-Dist: catboost>=1.2.2; extra == "core"
 Requires-Dist: lightgbm>=3.3.5; extra == "core"
-Requires-Dist: spinesTS>=0.4.1; extra == "core"
+Requires-Dist: spinesTS>=0.4.2; extra == "core"
 Requires-Dist: frozendict>=2.3.0; extra == "core"
 Requires-Dist: spinesUtils>=0.3.12; extra == "core"
 Requires-Dist: tabulate>=0.8.9; extra == "core"
 Requires-Dist: torch>=1.8.0; extra == "core"
 Requires-Dist: MAPIE>=0.7.0; extra == "core"
 Requires-Dist: cloudpickle>=2.2.1; extra == "core"
 
 # PipelineTS
-[中文文档](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
+[\[中文文档\]](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
 
 One-stop time series analysis tool, supporting time series data preprocessing, feature engineering, model training, model evaluation, model prediction, etc. Based on spinesTS and darts.
 ## Installation
 
 ```bash
 # if you don't want to use the prophet model
 # run this
 python -m pip install PipelineTS[core]
 
 # if you want to use all models
 # run this
 python -m pip install PipelineTS[all]
 ```
 
-## Quick Start [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
+## Quick Start [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
 
 ### list all available models
 ```python
 from PipelineTS.dataset import LoadWebSales
 
 init_data = LoadWebSales()[['date', 'type_a']]
 
@@ -143,15 +143,15 @@
 pipeline.fit(data, valid_data=valid_data)
 
 # use best model to predict next 30 steps data point
 res = pipeline.predict(30)
 
 ```
 ## Training and prediction of a single model
-###  Without predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
+###  Without predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
 
 #### Data Preprocessing
 
 ```python
 
 from PipelineTS.dataset import LoadMessagesSentDataSets
 import pandas as pd
@@ -194,15 +194,15 @@
     time_col=time_col, target_col=target_col, lags=lags, random_state=42, 
     quantile=0.9, enable_progress_bar=False, enable_model_summary=False
 )
 tide.fit(data)
 tide.predict(n)
 ```
 
-### With predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
+### With predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
 ```python
 tide.predict(n, series=valid_data)
 ```
 
 
 ## PipelineTS Module
 
@@ -211,46 +211,48 @@
 from xgboost import XGBRegressor
 from catboost import CatBoostRegressor
 from PipelineTS.pipeline import ModelPipeline, PipelineConfigs
 
 # If you want to try multiple configurations of a model at once for comparison or tuning purposes, you can use `PipelineConfigs`.
 # This feature allows for customizing the models returned by each `ModelPipeline.list_all_available_models()` call.
 # The first one is the name of the model, which needs to be in the list of available models provided by PipelineTS.list_all_available_models(). 
-# The second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
+# If you want to customize the name of the model, then the second argument can be a string of the model name, 
+# otherwise, the second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
 # The remaining keys will be automatically filled with default parameters.
 # Among them, 'init_configs' represents the initialization parameters of the model, 'fit_configs' represents the parameters during model training, 
 # and 'predict_configs' represents the parameters during model prediction.
+
 pipeline_configs = PipelineConfigs([
-    ('lightgbm', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
+    ('lightgbm', 'lightgbm_linear_tree', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
     ('multi_output_model', {'init_configs': {'verbose': -1}}),
     ('multi_step_model', {'init_configs': {'verbose': -1}}),
     ('multi_output_model', {
         'init_configs': {'estimator': XGBRegressor, 'random_state': 42, 'kwargs': {'verbosity': 0}}
     }
      ),
     ('multi_output_model', {
         'init_configs': {'estimator': CatBoostRegressor, 'random_state': 42, 'verbose': False}
     }
      ),
 ])
 ```
 <table>
 <thead>
-<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_with_index  </th><th>model_configs                                                                                                                                                    </th></tr>
+<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_after_rename  </th><th>model_configs                                                                                                                                                    </th></tr>
 </thead>
 <tbody>
-<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_1             </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
-<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1   </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
-<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
-<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
-<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_linear_tree     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
+<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
+<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
+<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1       </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
 </tbody>
 </table>
 
-### Non-Interval Forecasting [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
+### Non-Interval Forecasting [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
@@ -294,15 +296,15 @@
 
 plot_data_period(init_data.iloc[-100:, :], prediction, 
                  time_col=time_col, target_col=target_col)
 ```
 
 ![image1](https://github.com/BirchKwok/PipelineTS/blob/main/pics/pic2.png)
 
-### Interval prediction [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
+### Interval prediction [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
```

### Comparing `PipelineTS-0.3.8/PipelineTS.egg-info/SOURCES.txt` & `PipelineTS-0.3.9/PipelineTS.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 LICENSE
 README.md
-pyproject.toml
 setup.py
 PipelineTS/__init__.py
 PipelineTS/dataset.py
 PipelineTS/metrics.py
 PipelineTS.egg-info/PKG-INFO
 PipelineTS.egg-info/SOURCES.txt
 PipelineTS.egg-info/dependency_links.txt
```

### Comparing `PipelineTS-0.3.8/PipelineTS.egg-info/requires.txt` & `PipelineTS-0.3.9/PipelineTS.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 numpy<=1.25.0,>=1.24.3
 pandas>=2.0.3
 scikit-learn>=1.3.0
 xgboost>=1.6.0
 darts>=0.24.0
 catboost>=1.2.2
 lightgbm>=3.3.5
-spinesTS>=0.4.1
+spinesTS>=0.4.2
 frozendict>=2.3.0
 spinesUtils>=0.3.12
 tabulate>=0.8.9
 torch>=1.8.0
 MAPIE>=0.7.0
 cloudpickle>=2.2.1
 
@@ -19,15 +19,15 @@
 numpy<=1.25.0,>=1.24.3
 pandas>=2.0.3
 scikit-learn>=1.3.0
 xgboost>=1.6.0
 darts>=0.24.0
 catboost>=1.2.2
 lightgbm>=3.3.5
-spinesTS>=0.4.1
+spinesTS>=0.4.2
 frozendict>=2.3.0
 spinesUtils>=0.3.12
 tabulate>=0.8.9
 torch>=1.8.0
 MAPIE>=0.7.0
 cloudpickle>=2.2.1
 prophet>=1.1.4
@@ -37,14 +37,14 @@
 numpy<=1.25.0,>=1.24.3
 pandas>=2.0.3
 scikit-learn>=1.3.0
 xgboost>=1.6.0
 darts>=0.24.0
 catboost>=1.2.2
 lightgbm>=3.3.5
-spinesTS>=0.4.1
+spinesTS>=0.4.2
 frozendict>=2.3.0
 spinesUtils>=0.3.12
 tabulate>=0.8.9
 torch>=1.8.0
 MAPIE>=0.7.0
 cloudpickle>=2.2.1
```

### Comparing `PipelineTS-0.3.8/README.md` & `PipelineTS-0.3.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # PipelineTS
-[中文文档](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
+[\[中文文档\]](https://github.com/BirchKwok/PipelineTS/blob/main/README_CN.md)
 
 One-stop time series analysis tool, supporting time series data preprocessing, feature engineering, model training, model evaluation, model prediction, etc. Based on spinesTS and darts.
 ## Installation
 
 ```bash
 # if you don't want to use the prophet model
 # run this
 python -m pip install PipelineTS[core]
 
 # if you want to use all models
 # run this
 python -m pip install PipelineTS[all]
 ```
 
-## Quick Start [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
+## Quick Start [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/QuickStart.ipynb)
 
 ### list all available models
 ```python
 from PipelineTS.dataset import LoadWebSales
 
 init_data = LoadWebSales()[['date', 'type_a']]
 
@@ -74,15 +74,15 @@
 pipeline.fit(data, valid_data=valid_data)
 
 # use best model to predict next 30 steps data point
 res = pipeline.predict(30)
 
 ```
 ## Training and prediction of a single model
-###  Without predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
+###  Without predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling.ipynb)
 
 #### Data Preprocessing
 
 ```python
 
 from PipelineTS.dataset import LoadMessagesSentDataSets
 import pandas as pd
@@ -125,15 +125,15 @@
     time_col=time_col, target_col=target_col, lags=lags, random_state=42, 
     quantile=0.9, enable_progress_bar=False, enable_model_summary=False
 )
 tide.fit(data)
 tide.predict(n)
 ```
 
-### With predict specify series [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
+### With predict specify series [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/modeling-with-predict-specify-series.ipynb)
 ```python
 tide.predict(n, series=valid_data)
 ```
 
 
 ## PipelineTS Module
 
@@ -142,46 +142,48 @@
 from xgboost import XGBRegressor
 from catboost import CatBoostRegressor
 from PipelineTS.pipeline import ModelPipeline, PipelineConfigs
 
 # If you want to try multiple configurations of a model at once for comparison or tuning purposes, you can use `PipelineConfigs`.
 # This feature allows for customizing the models returned by each `ModelPipeline.list_all_available_models()` call.
 # The first one is the name of the model, which needs to be in the list of available models provided by PipelineTS.list_all_available_models(). 
-# The second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
+# If you want to customize the name of the model, then the second argument can be a string of the model name, 
+# otherwise, the second one is of type dict. The dict can have three keys: 'init_configs', 'fit_configs', 'predict_configs', or any combination of them. 
 # The remaining keys will be automatically filled with default parameters.
 # Among them, 'init_configs' represents the initialization parameters of the model, 'fit_configs' represents the parameters during model training, 
 # and 'predict_configs' represents the parameters during model prediction.
+
 pipeline_configs = PipelineConfigs([
-    ('lightgbm', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
+    ('lightgbm', 'lightgbm_linear_tree', {'init_configs': {'verbose': -1, 'linear_tree': True}}),
     ('multi_output_model', {'init_configs': {'verbose': -1}}),
     ('multi_step_model', {'init_configs': {'verbose': -1}}),
     ('multi_output_model', {
         'init_configs': {'estimator': XGBRegressor, 'random_state': 42, 'kwargs': {'verbosity': 0}}
     }
      ),
     ('multi_output_model', {
         'init_configs': {'estimator': CatBoostRegressor, 'random_state': 42, 'verbose': False}
     }
      ),
 ])
 ```
 <table>
 <thead>
-<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_with_index  </th><th>model_configs                                                                                                                                                    </th></tr>
+<tr><th style="text-align: right;">  </th><th>model_name        </th><th>model_name_after_rename  </th><th>model_configs                                                                                                                                                    </th></tr>
 </thead>
 <tbody>
-<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_1             </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
-<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1   </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
-<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
-<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3   </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
-<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 0</td><td>lightgbm          </td><td>lightgbm_linear_tree     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1, &#x27;linear_tree&#x27;: True}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                 </td></tr>
+<tr><td style="text-align: right;"> 1</td><td>multi_output_model</td><td>multi_output_model_1     </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
+<tr><td style="text-align: right;"> 2</td><td>multi_output_model</td><td>multi_output_model_2     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;xgboost.sklearn.XGBRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;kwargs&#x27;: {&#x27;verbosity&#x27;: 0}}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}</td></tr>
+<tr><td style="text-align: right;"> 3</td><td>multi_output_model</td><td>multi_output_model_3     </td><td>{&#x27;init_configs&#x27;: {&#x27;estimator&#x27;: &lt;class &#x27;catboost.core.CatBoostRegressor&#x27;&gt;, &#x27;random_state&#x27;: 42, &#x27;verbose&#x27;: False}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}       </td></tr>
+<tr><td style="text-align: right;"> 4</td><td>multi_step_model  </td><td>multi_step_model_1       </td><td>{&#x27;init_configs&#x27;: {&#x27;verbose&#x27;: -1}, &#x27;fit_configs&#x27;: {}, &#x27;predict_configs&#x27;: {}}                                                                                      </td></tr>
 </tbody>
 </table>
 
-### Non-Interval Forecasting [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
+### Non-Interval Forecasting [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
@@ -225,15 +227,15 @@
 
 plot_data_period(init_data.iloc[-100:, :], prediction, 
                  time_col=time_col, target_col=target_col)
 ```
 
 ![image1](https://github.com/BirchKwok/PipelineTS/blob/main/pics/pic2.png)
 
-### Interval prediction [notebook](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
+### Interval prediction [\[notebook\]](https://github.com/BirchKwok/PipelineTS/blob/main/examples/pipeline-with-quantile-prediction.ipynb)
 
 ```python
 from sklearn.metrics import mean_absolute_error
 
 from PipelineTS.pipeline import ModelPipeline
 
 pipeline = ModelPipeline(
```

### Comparing `PipelineTS-0.3.8/setup.py` & `PipelineTS-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 all_reqs = base_reqs + extra_reqs
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='PipelineTS',
-    version="0.3.8",
+    version="0.3.9",
     description='One-stop time series analysis tool, supporting time series data preprocessing,'
                 ' feature engineering, model training, model evaluation, model prediction, etc. '
                 'Based on spinesTS and darts.',
     keywords='time series forecasting',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

