# Comparing `tmp/survivors-1.6.2.tar.gz` & `tmp/survivors-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survivors-1.6.2.tar", last modified: Wed Feb 28 08:07:13 2024, max compression
+gzip compressed data, was "survivors-1.6.3.tar", last modified: Mon May 13 05:14:05 2024, max compression
```

## Comparing `survivors-1.6.2.tar` & `survivors-1.6.3.tar`

### file list

```diff
@@ -1,82 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.930347 survivors-1.6.2/
--rw-rw-rw-   0        0        0     1548 2024-02-19 13:25:28.000000 survivors-1.6.2/LICENSE
--rw-rw-rw-   0        0        0       46 2024-02-28 07:34:46.000000 survivors-1.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6340 2024-02-28 08:07:13.930347 survivors-1.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     6043 2024-02-19 13:28:57.000000 survivors-1.6.2/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.868831 survivors-1.6.2/requirements/
--rw-rw-rw-   0        0        0      222 2024-02-24 06:25:57.000000 survivors-1.6.2/requirements/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-02-28 08:07:13.931350 survivors-1.6.2/setup.cfg
--rw-rw-rw-   0        0        0     2118 2024-02-28 08:06:45.000000 survivors-1.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.871895 survivors-1.6.2/survivors/
--rw-rw-rw-   0        0        0        0 2022-04-18 18:19:42.000000 survivors-1.6.2/survivors/__init__.py
--rw-rw-rw-   0        0        0     2903 2023-09-30 21:03:45.000000 survivors-1.6.2/survivors/constants.py
--rw-rw-rw-   0        0        0     9601 2024-01-01 20:47:18.000000 survivors-1.6.2/survivors/criteria.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.885060 survivors-1.6.2/survivors/datasets/
--rw-rw-rw-   0        0        0      483 2023-12-05 09:19:43.000000 survivors-1.6.2/survivors/datasets/__init__.py
--rw-rw-rw-   0        0        0     2398 2024-01-11 19:12:41.000000 survivors-1.6.2/survivors/datasets/backblaze.py
--rw-rw-rw-   0        0        0    12785 2024-02-24 06:28:01.000000 survivors-1.6.2/survivors/datasets/covid.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.898171 survivors-1.6.2/survivors/datasets/data/
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.903185 survivors-1.6.2/survivors/datasets/data/COVID/
--rw-rw-rw-   0        0        0        0 2022-07-29 21:18:19.000000 survivors-1.6.2/survivors/datasets/data/COVID/__init__.py
--rw-rw-rw-   0        0        0   231218 2023-05-22 20:08:51.000000 survivors-1.6.2/survivors/datasets/data/Framingham.csv
--rw-rw-rw-   0        0        0    21013 2021-05-09 11:49:28.000000 survivors-1.6.2/survivors/datasets/data/GBSG.csv
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.904187 survivors-1.6.2/survivors/datasets/data/ONK/
--rw-rw-rw-   0        0        0        0 2022-07-29 21:18:20.000000 survivors-1.6.2/survivors/datasets/data/ONK/__init__.py
--rw-rw-rw-   0        0        0        0 2022-04-19 10:19:46.000000 survivors-1.6.2/survivors/datasets/data/__init__.py
--rw-rw-rw-   0        0        0    91017 2023-05-22 20:08:51.000000 survivors-1.6.2/survivors/datasets/data/actg.csv
--rw-rw-rw-   0        0        0   510734 2020-04-25 15:10:49.000000 survivors-1.6.2/survivors/datasets/data/covid_train.xlsx
--rw-rw-rw-   0        0        0   426689 2023-05-22 20:08:51.000000 survivors-1.6.2/survivors/datasets/data/flchain.csv
--rw-rw-rw-   0        0        0    36167 2021-05-09 09:54:13.000000 survivors-1.6.2/survivors/datasets/data/pbc.csv
--rw-rw-rw-   0        0        0   193738 2023-05-22 20:08:50.000000 survivors-1.6.2/survivors/datasets/data/rott2.csv
--rw-rw-rw-   0        0        0   421993 2023-05-22 20:08:51.000000 survivors-1.6.2/survivors/datasets/data/smarto.csv
--rw-rw-rw-   0        0        0  2160683 2023-05-22 20:08:50.000000 survivors-1.6.2/survivors/datasets/data/support2.csv
--rw-rw-rw-   0        0        0     9104 2023-12-16 07:55:36.000000 survivors-1.6.2/survivors/datasets/onk.py
--rw-rw-rw-   0        0        0     4718 2024-02-12 19:36:56.000000 survivors-1.6.2/survivors/datasets/other.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.912255 survivors-1.6.2/survivors/ensemble/
--rw-rw-rw-   0        0        0      280 2024-02-24 17:02:09.000000 survivors-1.6.2/survivors/ensemble/__init__.py
--rw-rw-rw-   0        0        0    11634 2024-02-24 17:17:26.000000 survivors-1.6.2/survivors/ensemble/base_ensemble.py
--rw-rw-rw-   0        0        0    10621 2023-05-30 09:53:46.000000 survivors-1.6.2/survivors/ensemble/base_ensemble_iter.py
--rw-rw-rw-   0        0        0     7973 2024-01-31 10:33:40.000000 survivors-1.6.2/survivors/ensemble/boosting.py
--rw-rw-rw-   0        0        0     3993 2024-02-24 17:09:52.000000 survivors-1.6.2/survivors/ensemble/bootstrap.py
--rw-rw-rw-   0        0        0     2182 2023-03-31 08:40:28.000000 survivors-1.6.2/survivors/ensemble/bootstrap_iter.py
--rw-rw-rw-   0        0        0    12662 2024-02-18 16:19:31.000000 survivors-1.6.2/survivors/ensemble/clever_boosting.py
--rw-rw-rw-   0        0        0     6302 2024-01-12 12:34:22.000000 survivors-1.6.2/survivors/ensemble/clever_boosting_iter.py
--rw-rw-rw-   0        0        0     5492 2023-08-28 20:28:59.000000 survivors-1.6.2/survivors/ensemble/clever_boosting_old.py
--rw-rw-rw-   0        0        0     3475 2024-01-12 12:34:55.000000 survivors-1.6.2/survivors/ensemble/ibsboosting.py
--rw-rw-rw-   0        0        0     2363 2024-01-12 12:35:17.000000 survivors-1.6.2/survivors/ensemble/proboosting.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.913259 survivors-1.6.2/survivors/experiments/
--rw-rw-rw-   0        0        0        0 2022-02-08 20:02:58.000000 survivors-1.6.2/survivors/experiments/__init__.py
--rw-rw-rw-   0        0        0    20957 2024-02-25 16:07:58.000000 survivors-1.6.2/survivors/experiments/grid.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.916275 survivors-1.6.2/survivors/external/
--rw-rw-rw-   0        0        0      475 2024-02-21 08:37:38.000000 survivors-1.6.2/survivors/external/__init__.py
--rw-rw-rw-   0        0        0     4964 2024-02-25 15:16:20.000000 survivors-1.6.2/survivors/external/leaf_model.py
--rw-rw-rw-   0        0        0     7174 2024-02-25 15:31:05.000000 survivors-1.6.2/survivors/external/nonparametric.py
--rw-rw-rw-   0        0        0     3111 2024-02-22 20:47:26.000000 survivors-1.6.2/survivors/external/parametric.py
--rw-rw-rw-   0        0        0    24791 2024-01-11 19:21:11.000000 survivors-1.6.2/survivors/metrics.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.918271 survivors-1.6.2/survivors/scheme/
--rw-rw-rw-   0        0        0       70 2022-09-14 11:38:55.000000 survivors-1.6.2/survivors/scheme/__init__.py
--rw-rw-rw-   0        0        0     5922 2022-09-20 20:44:45.000000 survivors-1.6.2/survivors/scheme/scheme.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.924308 survivors-1.6.2/survivors/tree/
--rw-rw-rw-   0        0        0      192 2024-02-18 17:31:01.000000 survivors-1.6.2/survivors/tree/__init__.py
--rw-rw-rw-   0        0        0    16535 2024-02-24 11:59:06.000000 survivors-1.6.2/survivors/tree/decision_tree.py
--rw-rw-rw-   0        0        0    12091 2022-09-18 18:27:46.000000 survivors-1.6.2/survivors/tree/find_split(p-value).py
--rw-rw-rw-   0        0        0    12511 2022-10-23 18:14:00.000000 survivors-1.6.2/survivors/tree/find_split.py
--rw-rw-rw-   0        0        0    21585 2024-02-24 09:48:13.000000 survivors-1.6.2/survivors/tree/find_split_hist.py
--rw-rw-rw-   0        0        0    13659 2024-02-18 16:19:57.000000 survivors-1.6.2/survivors/tree/find_split_hist_int.py
--rw-rw-rw-   0        0        0    16955 2024-02-24 11:12:39.000000 survivors-1.6.2/survivors/tree/node.py
--rw-rw-rw-   0        0        0    24040 2024-02-18 17:17:02.000000 survivors-1.6.2/survivors/tree/stratified_model.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.927339 survivors-1.6.2/survivors/tree_pandas/
--rw-rw-rw-   0        0        0       56 2022-02-08 22:46:18.000000 survivors-1.6.2/survivors/tree_pandas/__init__.py
--rw-rw-rw-   0        0        0    11220 2024-01-12 11:11:11.000000 survivors-1.6.2/survivors/tree_pandas/decision_tree.py
--rw-rw-rw-   0        0        0    12075 2022-07-22 11:11:53.000000 survivors-1.6.2/survivors/tree_pandas/find_split.py
--rw-rw-rw-   0        0        0    16732 2023-12-19 08:05:34.000000 survivors-1.6.2/survivors/tree_pandas/node.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.929345 survivors-1.6.2/survivors/visualize/
--rw-rw-rw-   0        0        0      111 2024-02-17 17:32:18.000000 survivors-1.6.2/survivors/visualize/__init__.py
--rw-rw-rw-   0        0        0      402 2024-02-17 17:29:45.000000 survivors-1.6.2/survivors/visualize/base.py
--rw-rw-rw-   0        0        0     2207 2024-02-17 17:29:50.000000 survivors-1.6.2/survivors/visualize/comparison.py
-drwxrwxrwx   0        0        0        0 2024-02-28 08:07:13.878013 survivors-1.6.2/survivors.egg-info/
--rw-rw-rw-   0        0        0     6340 2024-02-28 08:07:13.000000 survivors-1.6.2/survivors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2024-02-28 08:07:13.000000 survivors-1.6.2/survivors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 08:07:13.000000 survivors-1.6.2/survivors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2024-02-28 08:07:13.000000 survivors-1.6.2/survivors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-28 08:07:13.000000 survivors-1.6.2/survivors.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.660340 survivors-1.6.3/
+-rw-rw-rw-   0        0        0     1548 2024-02-19 13:25:28.000000 survivors-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0       46 2024-02-28 07:34:46.000000 survivors-1.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7400 2024-05-13 05:14:05.659304 survivors-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7087 2024-05-05 06:38:47.000000 survivors-1.6.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.360987 survivors-1.6.3/requirements/
+-rw-rw-rw-   0        0        0       47 2024-05-08 14:19:51.000000 survivors-1.6.3/requirements/docs-requirements.txt
+-rw-rw-rw-   0        0        0      191 2024-05-05 06:38:41.000000 survivors-1.6.3/requirements/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 05:14:05.660340 survivors-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0     1800 2024-05-13 05:11:34.000000 survivors-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.383120 survivors-1.6.3/survivors/
+-rw-rw-rw-   0        0        0        0 2022-04-18 18:19:42.000000 survivors-1.6.3/survivors/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-05-05 09:46:23.000000 survivors-1.6.3/survivors/constants.py
+-rw-rw-rw-   0        0        0    19170 2024-05-02 19:21:59.000000 survivors-1.6.3/survivors/criteria.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.440393 survivors-1.6.3/survivors/datasets/
+-rw-rw-rw-   0        0        0      646 2024-03-05 08:13:41.000000 survivors-1.6.3/survivors/datasets/__init__.py
+-rw-rw-rw-   0        0        0     2398 2024-01-11 19:12:41.000000 survivors-1.6.3/survivors/datasets/backblaze.py
+-rw-rw-rw-   0        0        0    12894 2024-05-05 05:37:25.000000 survivors-1.6.3/survivors/datasets/covid.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.505690 survivors-1.6.3/survivors/datasets/data/
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.507695 survivors-1.6.3/survivors/datasets/data/BACKBLAZE/
+-rw-rw-rw-   0        0        0        0 2024-03-05 09:18:49.000000 survivors-1.6.3/survivors/datasets/data/BACKBLAZE/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.508723 survivors-1.6.3/survivors/datasets/data/COVID/
+-rw-rw-rw-   0        0        0        0 2022-07-29 21:18:19.000000 survivors-1.6.3/survivors/datasets/data/COVID/__init__.py
+-rw-rw-rw-   0        0        0   231218 2023-05-22 20:08:51.000000 survivors-1.6.3/survivors/datasets/data/Framingham.csv
+-rw-rw-rw-   0        0        0    21013 2021-05-09 11:49:28.000000 survivors-1.6.3/survivors/datasets/data/GBSG.csv
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.509726 survivors-1.6.3/survivors/datasets/data/ONK/
+-rw-rw-rw-   0        0        0        0 2022-07-29 21:18:20.000000 survivors-1.6.3/survivors/datasets/data/ONK/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-04-19 10:19:46.000000 survivors-1.6.3/survivors/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0    91017 2023-05-22 20:08:51.000000 survivors-1.6.3/survivors/datasets/data/actg.csv
+-rw-rw-rw-   0        0        0   510734 2020-04-25 15:10:49.000000 survivors-1.6.3/survivors/datasets/data/covid_train.xlsx
+-rw-rw-rw-   0        0        0   426689 2023-05-22 20:08:51.000000 survivors-1.6.3/survivors/datasets/data/flchain.csv
+-rw-rw-rw-   0        0        0    36167 2021-05-09 09:54:13.000000 survivors-1.6.3/survivors/datasets/data/pbc.csv
+-rw-rw-rw-   0        0        0   193738 2023-05-22 20:08:50.000000 survivors-1.6.3/survivors/datasets/data/rott2.csv
+-rw-rw-rw-   0        0        0   421993 2023-05-22 20:08:51.000000 survivors-1.6.3/survivors/datasets/data/smarto.csv
+-rw-rw-rw-   0        0        0  2160683 2023-05-22 20:08:50.000000 survivors-1.6.3/survivors/datasets/data/support2.csv
+-rw-rw-rw-   0        0        0     2480 2024-04-16 11:28:15.000000 survivors-1.6.3/survivors/datasets/new_backblaze.py
+-rw-rw-rw-   0        0        0     9104 2023-12-16 07:55:36.000000 survivors-1.6.3/survivors/datasets/onk.py
+-rw-rw-rw-   0        0        0     5977 2024-05-08 11:05:17.000000 survivors-1.6.3/survivors/datasets/other.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.572947 survivors-1.6.3/survivors/ensemble/
+-rw-rw-rw-   0        0        0      280 2024-02-24 17:02:09.000000 survivors-1.6.3/survivors/ensemble/__init__.py
+-rw-rw-rw-   0        0        0    11501 2024-03-14 13:20:46.000000 survivors-1.6.3/survivors/ensemble/base_ensemble.py
+-rw-rw-rw-   0        0        0    10622 2024-03-14 09:32:01.000000 survivors-1.6.3/survivors/ensemble/base_ensemble_iter.py
+-rw-rw-rw-   0        0        0     7969 2024-04-17 05:54:19.000000 survivors-1.6.3/survivors/ensemble/boosting.py
+-rw-rw-rw-   0        0        0     4012 2024-05-05 15:33:34.000000 survivors-1.6.3/survivors/ensemble/bootstrap.py
+-rw-rw-rw-   0        0        0     2182 2023-03-31 08:40:28.000000 survivors-1.6.3/survivors/ensemble/bootstrap_iter.py
+-rw-rw-rw-   0        0        0    12589 2024-04-11 17:45:24.000000 survivors-1.6.3/survivors/ensemble/clever_boosting.py
+-rw-rw-rw-   0        0        0     6304 2024-04-30 18:14:01.000000 survivors-1.6.3/survivors/ensemble/clever_boosting_iter.py
+-rw-rw-rw-   0        0        0     5492 2023-08-28 20:28:59.000000 survivors-1.6.3/survivors/ensemble/clever_boosting_old.py
+-rw-rw-rw-   0        0        0     3475 2024-01-12 12:34:55.000000 survivors-1.6.3/survivors/ensemble/ibsboosting.py
+-rw-rw-rw-   0        0        0     2363 2024-01-12 12:35:17.000000 survivors-1.6.3/survivors/ensemble/proboosting.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.580993 survivors-1.6.3/survivors/experiments/
+-rw-rw-rw-   0        0        0        0 2022-02-08 20:02:58.000000 survivors-1.6.3/survivors/experiments/__init__.py
+-rw-rw-rw-   0        0        0    20806 2024-04-30 18:17:22.000000 survivors-1.6.3/survivors/experiments/grid.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.604052 survivors-1.6.3/survivors/external/
+-rw-rw-rw-   0        0        0      475 2024-02-21 08:37:38.000000 survivors-1.6.3/survivors/external/__init__.py
+-rw-rw-rw-   0        0        0     6159 2024-05-05 14:09:46.000000 survivors-1.6.3/survivors/external/leaf_model.py
+-rw-rw-rw-   0        0        0     7193 2024-04-30 18:19:28.000000 survivors-1.6.3/survivors/external/nonparametric.py
+-rw-rw-rw-   0        0        0     3313 2024-04-23 19:03:34.000000 survivors-1.6.3/survivors/external/parametric.py
+-rw-rw-rw-   0        0        0    23502 2024-04-23 18:58:51.000000 survivors-1.6.3/survivors/metrics.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.614135 survivors-1.6.3/survivors/scheme/
+-rw-rw-rw-   0        0        0       70 2022-09-14 11:38:55.000000 survivors-1.6.3/survivors/scheme/__init__.py
+-rw-rw-rw-   0        0        0     5955 2024-05-02 19:24:58.000000 survivors-1.6.3/survivors/scheme/scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.638250 survivors-1.6.3/survivors/tree/
+-rw-rw-rw-   0        0        0       58 2024-04-11 17:45:12.000000 survivors-1.6.3/survivors/tree/__init__.py
+-rw-rw-rw-   0        0        0    14832 2024-04-12 15:35:50.000000 survivors-1.6.3/survivors/tree/decision_tree.py
+-rw-rw-rw-   0        0        0    22772 2024-05-05 15:08:35.000000 survivors-1.6.3/survivors/tree/find_split_hist.py
+-rw-rw-rw-   0        0        0    16144 2024-05-08 06:55:14.000000 survivors-1.6.3/survivors/tree/node.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.657299 survivors-1.6.3/survivors/visualize/
+-rw-rw-rw-   0        0        0      112 2024-05-08 11:43:53.000000 survivors-1.6.3/survivors/visualize/__init__.py
+-rw-rw-rw-   0        0        0      643 2024-05-08 11:50:09.000000 survivors-1.6.3/survivors/visualize/base.py
+-rw-rw-rw-   0        0        0     2744 2024-05-08 11:43:04.000000 survivors-1.6.3/survivors/visualize/comparison.py
+drwxrwxrwx   0        0        0        0 2024-05-13 05:14:05.405248 survivors-1.6.3/survivors.egg-info/
+-rw-rw-rw-   0        0        0     7400 2024-05-13 05:14:04.000000 survivors-1.6.3/survivors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1883 2024-05-13 05:14:05.000000 survivors-1.6.3/survivors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 05:14:04.000000 survivors-1.6.3/survivors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2024-05-13 05:14:05.000000 survivors-1.6.3/survivors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 05:14:05.000000 survivors-1.6.3/survivors.egg-info/top_level.txt
```

### Comparing `survivors-1.6.2/LICENSE` & `survivors-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/PKG-INFO` & `survivors-1.6.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,137 @@
 Metadata-Version: 2.1
 Name: survivors
-Version: 1.6.2
+Version: 1.6.3
 Summary: UNKNOWN
 Author: Iulii Vasilev
 Author-email: iuliivasilev@gmail.com
-License: UNKNOWN
+License: BSD 3-Clause License
 Keywords: survival analysis,time-to-event,event data,machine learning
 Platform: UNKNOWN
 Requires-Python: >=3.10
 License-File: LICENSE
 
-|License| |PyPi|_ |DOI|_
+.. -*- mode: rst -*-
 
-===============
+|Price| |License| |PyPi|_ |DOI|_
+
+.. |Price| image:: https://img.shields.io/badge/price-FREE-0098f7.svg
+   :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+
+.. |PyPi| image:: https://img.shields.io/pypi/v/survivors
+.. _PyPi: https://pypi.org/project/survivors/
+
+.. |License| image:: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg
+   :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10649986.svg
+.. _DOI: https://zenodo.org/doi/10.5281/zenodo.10649777
+
+=========
 survivors
-===============
+=========
+
+Event analysis has many applications: healthcare, hardware, social science, bioinformatics, and more.вЂЁSurvival analysis allows you to predict not only the time and probability of an event but also how the probability of that event changes over time.
+In particular, there are three functions: the survival function *S(t)*, the density function *f(t)*, and the hazard function *h(t)*:
+
+.. math::
+    S(t)=P(T>t), f(t)=P(T=t), h(t)=P(T=t|T>=t)
 
-`survivors <https://pypi.org/project/survivors/>`_ is a Python library for **survival analysis**.
+The open-source **survivors** library aims to fit accurate data-sensitive tree-based models. 
+These models handle categorical features and deal with missing values,overcoming the limitations of existing `lifelines <https://github.com/lifelines/lifelines?ysclid=lta0m13i2b832399887>`_, `scikit-survival <https://github.com/sebp/scikit-survival>`_, and `pycox <https://github.com/havakv/pycox>`_ models.
+Survivors is a platform for conducting experimental research. The experiment module is compatible with scikit-survival and lifelines models (non-parametric and parametric models have already been embedded into the library).
 
-It allows for building survival models: Survival Tree, Bagging ensemble, Adaptive Boosting ensemble.
+Developed models published in scientific articles [1]_, [2]_, [3]_ and outperformed existing models in terms of accuracy based on open medical data. We invite survival analysis researchers to join the development of survivors, using the library for their projects, reporting any problems, and creating new solutions.
+Documentation is available on https://iuliivasilev.github.io/dev-survivors/
 
-=======================
-About Survival Analysis
-=======================
+Principles
+-----------
 
-The objective in `survival analysis`_ (also referred to as time-to-event or reliability analysis)
-is to establish a connection between covariates and the time of an event.
+Built-in **survivors** models were developed as part of a PhD thesis at Lomonosov Moscow State University. The goal of the library is to analyze existing methods of survival analysis and develop new techniques to overcome these limitations.
 
-Survival analysis is a set of statistical models and methods used for estimating time until the occurrence of an event (or the probability that an event has not occurred). These methods are widely used in demography, e.g. for estimating lifespan or age at the first childbirth, in healthcare, e.g. for estimating the duration of staying in a hospital or survival time after the diagnosis of a disease, in engineering (for reliability analysis), in insurance, economics, and social sciences.
+Existing methods are not suitable for real-world data. Discrete methods use a fixed time scale. Statistical methods are based on strong assumptions, and tree-based methods use the log-rank statistic with low sensitivity.
+**Survivors** has the following features:
 
-Statistical methods need data, but complete data may not be available, i.e. the exact time of the event may be unknown for certain reasons  (the event did not occur before the end of the study or it is unknown whether it occurred). In this case, events are called censored. The data are censored from below (left-censored) when below a given value the exact values of observations are unknown. Right censored data (censored from above) does not have exact observations above a given value. Further in this paper, right censoring is considered.
+1. Continuous Predictions: The timeline is user-friendly and only needs to be set at the prediction stage.
+2. Modified Quality Metrics: Existing metrics are excessively sensitive to data features, such as class imbalance, event distribution, and timeline.
+3. Weighted Survival Tree. For the first time, CRAID uses weighted log-rank criteria. Wilcoxon, Peto, and Tarone-Ware weights increase the significance of events within a certain time interval.
+4. Speed of work. The models are developed from scratch and utilize parallelization, vectorization, and JIT compilation. A new histogram-based method is employed to identify splits in censored data. This method optimizes memory usage and has a high level of operation speed.
+5. Ease of Use. CRAID and ensembles work out-of-the-box. Categorical and missing data are processed within the models.
+6. A Platform for Experiments. The experiments module provides a flexible interface for working with built-in and external survival models, their hyperparameters, and experiment strategies, such as hold-out, cross-validation, grid search with cross-validation and sampling, and time-aware cross-validation.
+
+Installation
+------------
 
-============
 Requirements
-============
+~~~~~~~~~~~~
 
-- Python 3.9 or later
-- joblib
-- pickle-mixin
-- numpy >= 1.22
-- numba >= 0.58.0
-- matplotlib >= 3.5.0
+- Python (>= 3.9)
+- NumPy (>= 1.22)
+- Pandas (>=0.25)
+- Numba (>= 0.58.0)
+- matplotlib (>= 3.5.0)
 - seaborn
-- graphviz >= 2.50.0
-- pandas >=0.25
-- scipy
-- python-dateutil
-- scikit-learn >= 1.0.2
-- lifelines >= 0.27.8
-- scikit-survival >= 0.17.2
+- graphviz (>= 2.50.0)
+- joblib
+- scikit-learn (>= 1.0.2)
 - openpyxl
 
-============
-Installation
-============
+Optional for comprehensive experiments:
 
-The easiest way to install survivors is to use by running::
+- lifelines (>= 0.27.8)
+- scikit-survival (>= 0.17.2)
 
-  pip install survivors
+User Installation
+~~~~~~~~~~~~~~~~~
 
-========
-Examples
-========
+The most convenient and fastest way to install a package is to directly download the library from the Python package catalog (Python Package Index, PyPI).
+The version of the source files in the directory is up-to-date and consistent with the GitHub repository::
 
-The user guides at *doc* and *demonstration* directories provide in-depth information on the key concepts of survivors, an overview of available survival models,
-and hands-on examples in the form of `Jupyter notebooks <https://jupyter.org/>`_.
+  pip install survivors
 
-There are examples of using the library with Jupyter Notebook.
-The example is a variant of solving a multi-stage problem:
+An alternative installation method is based on the use of source files. 
+The first step is to download the source files using Github::
 
-1. Import the library
-2. Loading and preparing data
-3. Model training
-4. Getting a forecast
-5. Visualization of the constructed model
-6. Visualization of true and predicted survival functions
+  git clone command https://github.com/iuliivasilev/dev-survivors.git
 
-==========
-Scenarios
-==========
+Or getting and unpacking the archive of `the latest published version <https://github.com/iuliivasilev/dev-survivors/releases/>`_. Next, use the command line to go to the **dev-survivors** directory. Finally, the manual installation of the library is completed after executing the following command::
 
-The library allows to carry out the following work scenarios:
+  python command setup.py install
 
-1. Collecting data from patient medical histories (hospital tests, medications, treatment) from various medical institutions. The medical history can be presented as a set of tables in csv or xlsx format, or as a hierarchical structure of xml files.
 
-2. Building survival analysis models. There are available the following models: a decision tree, a bagging ensemble, and a boosting ensemble. For each model, there is a wide range of hyperparameters, which provide the flexibility of the model.
+Examples
+------------
 
-3. Predicting the probability and time of the event. Forecasts can be used by the user to solve the problem of classifying or ranking new patients according to the expected severity of the disease.
+The user guides in the *doc* and *demonstration* directories provide detailed information on the key concepts for **survivors**. 
+They also include hands-on examples in the form of `Jupyter notebooks <https://jupyter.org/>`_.
+In particular, the library allows users to carry out a range of scenarios.
+
+1. Loading and preparing 9 open medical datasets: GBSG, PBC, SMARTO, SUPPORT2, WUHAN, ACTG, FLCHAIN, ROTT2, FRAMINGHAM.
+2. Fitting Survival Analysis Models: There are the following models available: a Decision Tree (CRAID), a Bootstrap Ensemble (BootstrapCRAID), and an Adaptive Boosting Ensemble (BoostingCRAID). Each model has a wide range of hyperparameters, providing flexibility for the model.
+3. Predict the probability and timing of the event. Forecasts can help users solve the problem of classifying or ranking new patients based on the expected severity of their disease. 
+4. Predict the individual survival functions and cumulative hazards of patients. Forecasts can be used to support medical decisions and adjust treatments.
+5. Visualizing and interpreting dependencies in data.
 
-4. Predicting the individual survival functions and cumulative hazard of patients. Forecasts can be used to support medical decisions and adjust treatment.
+Help and Support
+----------------
 
-==============
 Communication
-==============
+~~~~~~~~~~~~~
 
-- Mail: iuliivasilev@gmail.com
+- Email: iuliivasilev@gmail.com
 - LinkedIn: https://www.linkedin.com/in/iulii-vasilev
 
-==========
-References
-==========
-
-Please cite the following paper if you are using **survivors**.
-
-    Vasilev I., Petrovskiy M., Mashechkin I. Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria. - 2022.
-
-    Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Sensitivity of Survival Analysis Metrics." Mathematics 11.20 (2023): 4246.
-
-    Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting." International Conference on Pattern Recognition Applications and Methods. Cham: Springer International Publishing, 2021.
-
-.. code::
-
-    @inproceedings{vasilev2022survival,
-        title={Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria.},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor V},
-        booktitle={ICPRAM},
-        pages={132--140},
-        year={2022}
-    }
-
-    @inproceedings{vasilev2023adaptive,
-        title={Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor},
-        booktitle={Pattern Recognition Applications and Methods: 10th International Conference, ICPRAM 2021, and 11th International Conference, ICPRAM 2022, Virtual Event, February 4--6, 2021 and February 3--5, 2022, Revised Selected Papers},
-        pages={98--115},
-        year={2023},
-        organization={Springer}
-    }
-
-    @article{vasilev2023sensitivity,
-        title={Sensitivity of Survival Analysis Metrics},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor},
-        journal={Mathematics},
-        volume={11},
-        number={20},
-        pages={4246},
-        year={2023},
-        publisher={MDPI}
-    }
 
-.. _survival analysis: https://en.wikipedia.org/wiki/Survival_analysis
+Citation
+~~~~~~~~~~
 
-.. |PyPi| image:: https://img.shields.io/pypi/v/survivors
-.. _PyPi: https://pypi.org/project/survivors/
+If you use **survivors** in a scientific publication, we would appreciate citations:
 
-.. |License| image:: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg
-  :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+.. [1] Vasilev I., Petrovskiy M., Mashechkin I. Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria. - 2022.
+
+.. [2] Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Sensitivity of Survival Analysis Metrics." Mathematics 11.20 (2023): 4246.
+
+.. [3] Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting." International Conference on Pattern Recognition Applications and Methods. Cham: Springer International Publishing, 2021.
+
+.. _survival analysis: https://en.wikipedia.org/wiki/Survival_analysis
 
-.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10649986.svg
-.. _DOI: https://zenodo.org/doi/10.5281/zenodo.10649777
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `survivors-1.6.2/survivors/constants.py` & `survivors-1.6.3/survivors/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,26 +46,26 @@
 def pd_to_xy(df):
     """
     Splitting pandas dataframe to feature space and target variables
 
     Parameters
     ----------
     df : pandas DataFrame
-        Must to have columns CENS_NAME and TIME_NAME.
+        Must contain columns CENS_NAME and TIME_NAME.
 
     Returns
     -------
     X : pandas DataFrame
         Feature space with remaining features.
     y : structured array
         y containing the binary event indicator as first field,
         and time of event or time of censoring as second field.
 
     """
-    X = df.loc[:, list(set(df.columns) - {CENS_NAME, TIME_NAME})]
+    X = df[list(set(df.columns) - {CENS_NAME, TIME_NAME})]
     y = get_y(df[CENS_NAME], df[TIME_NAME])
     return X, y
 
 
 def get_bins(time, cens=None, mode='a', num_bins=100):
     """
     Generate array of time points in timeline (from sample)
@@ -82,18 +82,18 @@
         'q' : quantile points (quantity is based on num_bins)
     num_bins : int, optional
         Quantity of required points. The default is 100.
 
     Returns
     -------
     bins : array
-        Array of time points in timeline
+        Timeline
 
     """
-    if not(cens is None):
+    if not (cens is None):
         time = time[np.where(cens)]
     time = time.astype(np.int32)
     bins = np.array([])
     if mode == 'q':
         bins = np.quantile(time, np.arange(num_bins) / num_bins)
     elif mode == 'a':
         bins = np.arange(time.min(), time.max()+1)  # all bins
```

### Comparing `survivors-1.6.2/survivors/datasets/backblaze.py` & `survivors-1.6.3/survivors/datasets/backblaze.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/covid.py` & `survivors-1.6.3/survivors/datasets/covid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 import numpy as np
 import pandas as pd
-import re
+from re import sub
 from os.path import dirname, join
-from dateutil import parser  # python-dateutil
 from ..constants import TIME_NAME, CENS_NAME, get_y
 
+try:
+    from dateutil import parser
+except ImportError:
+    raise ImportError('Please, install python-dateutil: pip install python-dateutil')
+
+
 schemes_list = [
     'light_1', 'light_2', 'light_3',
     'middle_1', 'middle_2', 'middle_3', 'middle_4', 'middle_5', 'middle_6', 'middle_7', 'middle_8',
     'hard_1', 'hard_2', 'hard_3', 'hard_4', 'hard_5',
     'cyto_1', 'cyto_2', 'cyto_3', 'cyto_4', 'cyto_5', 'cyto_6',
     'MOS_AM', 'MOS_AM_AZ', 'N_MOS_AM_AZ', 'MOS_AM_LVF', 'N_MOS_AM_LVF',
     'MOS_CFTR', 'MOS_CFT', 'MOS_CFP', 'MOS_CFP_LVF', 'N_MOS_CFP_LVF',
@@ -206,15 +211,15 @@
     cyto = pd.read_csv(join(dir_env, "cyto_with_schemes.csv"))
     cyto = create_none_ft(cyto, sign)
     cyto[TIME_NAME] = cyto.apply(lambda row: dest_date(row['Дата создания ЭС'], row['Дата закрытия ЭС']), axis=1)
     cyto[CENS_NAME] = cyto['Причина закрытия ЭС'].apply(lambda x: int(x[0] == 'У') if x == x else 0)
     cyto['SUM_M'] = 0
     sec = cyto.loc[:, sign+important]
     
-    repl = {sc: re.sub("[^0-9A-Za-zА-Яа-я_]", "", sc) for sc in sec.columns}
+    repl = {sc: sub("[^0-9A-Za-zА-Яа-я_]", "", sc) for sc in sec.columns}
     sec = sec.rename(columns=repl)
     sec['idx'] = sec.index 
     sec = sec[sec[TIME_NAME] == sec[TIME_NAME]]
     for sch in schemes_list:
         sec[sch] = sec[sch].fillna(0)
     new_sign = [repl[s] for s in sign]
     new_categ = [repl[s] for s in categ_cyto]
```

### Comparing `survivors-1.6.2/survivors/datasets/data/Framingham.csv` & `survivors-1.6.3/survivors/datasets/data/Framingham.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/GBSG.csv` & `survivors-1.6.3/survivors/datasets/data/GBSG.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/actg.csv` & `survivors-1.6.3/survivors/datasets/data/actg.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/covid_train.xlsx` & `survivors-1.6.3/survivors/datasets/data/covid_train.xlsx`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/flchain.csv` & `survivors-1.6.3/survivors/datasets/data/flchain.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/pbc.csv` & `survivors-1.6.3/survivors/datasets/data/pbc.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/rott2.csv` & `survivors-1.6.3/survivors/datasets/data/rott2.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/smarto.csv` & `survivors-1.6.3/survivors/datasets/data/smarto.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/data/support2.csv` & `survivors-1.6.3/survivors/datasets/data/support2.csv`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/datasets/onk.py` & `survivors-1.6.3/survivors/datasets/onk.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/ensemble/base_ensemble.py` & `survivors-1.6.3/survivors/ensemble/base_ensemble.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     def fit(self):
         pass
 
     def add_model(self, model, x_oob):
         self.models.append(model)
         self.oob.append(x_oob)
-        if self.ens_metric_name == "conc":
+        if self.ens_metric_name == "CI":
             tree_pred = pd.DataFrame(model.predict(x_oob, target=cnt.TIME_NAME), index=x_oob.index)
         elif self.ens_metric_name == "roc":
             tree_pred = pd.DataFrame(model.predict(x_oob, target=cnt.CENS_NAME), index=x_oob.index)
         else:
             tree_pred = pd.DataFrame(model.predict_at_times(x_oob, bins=self.bins, mode="surv"), index=x_oob.index)
             tree_pred = tree_pred.apply(lambda r: np.array(r), axis=1)
         self.list_pred_oob.append(tree_pred)
@@ -155,37 +155,37 @@
             score = self.separate_score_oob()
         return np.round(score, 4)
 
     def separate_score_oob(self):
         scores = np.array([])
         for i in range(len(self.models)):
             X_v = self.oob[i]
-            if self.ens_metric_name == "conc":
+            if self.ens_metric_name == "CI":
                 pred = self.models[i].predict(X_v, target=cnt.TIME_NAME)
                 score = concordance_index(X_v[cnt.TIME_NAME], pred)
             else:
                 pred = self.models[i].predict_at_times(X_v, bins=self.bins, mode="surv")
                 y_true = cnt.get_y(X_v[cnt.CENS_NAME], X_v[cnt.TIME_NAME])
                 score = metr.ibs(self.y_train, y_true, pred, self.bins)
             scores = np.append(scores, score)
         return np.round(np.mean(scores), 4)
 
     def aggregate_score_selfoob(self, bins=None):
         is_ibs = self.ens_metric_name.upper().find("IBS") >= 0
-        if self.ens_metric_name in ["conc"] or is_ibs:
+        if self.ens_metric_name in ["CI"] or is_ibs:
             list_target_time = [oob_[cnt.TIME_NAME].to_frame() for oob_ in self.oob]
             target_time = pd.concat(list_target_time, axis=1).mean(axis=1)
 
         if self.ens_metric_name in ["roc"] or is_ibs:
             list_target_cens = [oob_[cnt.CENS_NAME].to_frame() for oob_ in self.oob]
             target_cens = pd.concat(list_target_cens, axis=1).mean(axis=1)
 
-        if self.ens_metric_name in ["conc", "roc"]:
+        if self.ens_metric_name in ["CI", "roc"]:
             pred = pd.concat(self.list_pred_oob, axis=1).mean(axis=1)
-            if self.ens_metric_name == "conc":
+            if self.ens_metric_name == "CI":
                 return concordance_index(target_time, pred)
             return roc_auc_score(target_cens, pred)
 
         if is_ibs:
             pred = pd.concat(self.list_pred_oob, axis=1).apply(lambda r: r.mean(axis=0), axis=1)
             pred = np.array(pred.to_list())
             y_true = cnt.get_y(target_cens, target_time)
@@ -210,14 +210,20 @@
 
     def select_model(self, start, end):
         self.models = self.models[start:end]
         self.oob_index = self.oob_index[start:end]
 
     def tolerance_find_best(self, ens_metric_name="bic"):
         self.ens_metric_name = ens_metric_name
+
+        self.is_ci = self.ens_metric_name.upper().find("CI") >= 0
+        self.is_ibs = self.ens_metric_name.upper().find("IBS") >= 0
+        self.is_auprc = self.ens_metric_name.upper().find("AUPRC") >= 0
+        self.is_iauc = self.ens_metric_name.upper().find("IAUC") >= 0
+
         ens_metr_arr = np.zeros(self.n_estimators)
 
         self.prepare_for_tolerance()
         for i in range(self.n_estimators):
             self.tolerance_iter = i
             self.predict_by_i(i)
             ens_metr_arr[i] = self.score_oob()
@@ -228,61 +234,53 @@
         else:
             best_index = np.argmax(ens_metr_arr)
         self.select_model(0, best_index + 1)
         # print(ens_metr_arr)
         # print(f"fitted: {len(self.models)} models.")
 
     def prepare_for_tolerance(self):
-        if self.ens_metric_name in ["iauc", "likelihood", "bic"] or self.ens_metric_name.upper().find("IBS") >= 0:
+        if self.ens_metric_name in ["LOGLIKELIHOOD", "bic"] or self.is_ibs or self.is_iauc or self.is_auprc:
             dim = (self.X_train.shape[0], self.bins.shape[0])
         else:
             dim = (self.X_train.shape[0])
         self.oob_prediction = np.zeros(dim, dtype=np.float)
 
-        if self.ens_metric_name in ["likelihood", "bic"]:
+        if self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
             self.oob_prediction_hf = np.zeros(dim, dtype=np.float)
         self.oob_count = np.zeros((self.X_train.shape[0]), dtype=np.int)
 
     def predict_by_i(self, ind_model):
         model = self.models[ind_model]
         oob_index = self.oob_index[ind_model]
         x_oob = self.X_train.iloc[oob_index, :]
 
         self.oob_count[oob_index] += 1
-        if self.ens_metric_name == "conc":
+        if self.is_ci:
             self.oob_prediction[oob_index] += model.predict(x_oob, target=cnt.TIME_NAME)
         elif self.ens_metric_name == "roc":
             self.oob_prediction[oob_index] += model.predict(x_oob, target=cnt.CENS_NAME)
-        elif self.ens_metric_name in ["likelihood", "bic"]:
-            self.oob_count = np.ones((self.X_train.shape[0]), dtype=np.int)
+        elif self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
             self.oob_prediction_hf += model.predict_at_times(self.X_train, bins=self.bins, mode="hazard")
             self.oob_prediction += model.predict_at_times(self.X_train, bins=self.bins, mode="surv")
-        else:
+        elif self.is_iauc:
+            self.oob_prediction[oob_index] += model.predict_at_times(x_oob, bins=self.bins, mode="hazard")
+        elif self.is_ibs or self.is_auprc:
             self.oob_prediction[oob_index] += model.predict_at_times(x_oob, bins=self.bins, mode="surv")
 
     def aggregate_score_selfoob(self):
         index_join_oob = np.where(self.oob_count != 0)
-        is_ibs = self.ens_metric_name.upper().find("IBS") >= 0
-        if is_ibs:
-            pred = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob][:, None]
-        elif self.ens_metric_name in ["likelihood", "bic"]:
-            pred_hf = self.oob_prediction_hf[index_join_oob]  # / self.oob_count[index_join_oob][:, None]
-            pred_sf = self.oob_prediction[index_join_oob]  # / self.oob_count[index_join_oob][:, None]
-        else:
-            pred = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob]
 
-        join_oob = self.y_train[index_join_oob]
-        target_time = join_oob[cnt.TIME_NAME]
-        target_cens = join_oob[cnt.CENS_NAME]
+        pred_time = None
+        pred_sf, pred_hf = None, None
+        if self.is_ibs or self.is_auprc:
+            pred_sf = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob][:, None]
+        elif self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
+            pred_hf = self.oob_prediction_hf[index_join_oob] / (self.tolerance_iter + 1)
+            pred_sf = self.oob_prediction[index_join_oob] / (self.tolerance_iter + 1)
+        elif self.is_iauc:
+            pred_hf = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob][:, None]
+        elif self.is_ci:
+            pred_time = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob]
 
-        if self.ens_metric_name == "conc":
-            return concordance_index(target_time, pred)
-        elif self.ens_metric_name == "roc":
-            return roc_auc_score(target_cens, pred)
-        elif is_ibs:
-            y_true = cnt.get_y(target_cens, target_time)
-            return metr.METRIC_DICT[self.ens_metric_name.upper()](self.y_train, y_true, None, pred, None, self.bins)
-        elif self.ens_metric_name == "likelihood":
-            return metr.loglikelihood(target_time, target_cens, pred_sf, pred_hf, self.bins)
-        elif self.ens_metric_name == "bic":
-            return metr.bic(self.tolerance_iter+1, self.size_sample, target_time, target_cens, pred_sf, pred_hf, self.bins)
-        return None
+        join_oob = self.y_train[index_join_oob]
+        y_true = cnt.get_y(cens=join_oob[cnt.CENS_NAME], time=join_oob[cnt.TIME_NAME])
+        return metr.METRIC_DICT[self.ens_metric_name.upper()](self.y_train, y_true, pred_time, pred_sf, pred_hf, self.bins)
```

### Comparing `survivors-1.6.2/survivors/ensemble/base_ensemble_iter.py` & `survivors-1.6.3/survivors/ensemble/base_ensemble_iter.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     
     def fit(self):
         pass
 
     def add_model(self, model, x_oob):
         self.models.append(model)
         self.oob.append(x_oob)
-        if self.ens_metric_name == "conc":
+        if self.ens_metric_name == "CI":
             tree_pred = pd.DataFrame(model.predict(x_oob, target=cnt.TIME_NAME), index=x_oob.index)
         elif self.ens_metric_name == "roc":
             tree_pred = pd.DataFrame(model.predict(x_oob, target=cnt.CENS_NAME), index=x_oob.index)
         else:
             tree_pred = pd.DataFrame(model.predict_at_times(x_oob, bins=self.bins, mode="surv"), index=x_oob.index)
             tree_pred = tree_pred.apply(lambda r: np.array(r), axis=1)
         self.list_pred_oob.append(tree_pred)
@@ -151,37 +151,37 @@
             score = self.separate_score_oob()
         return np.round(score, 4)
     
     def separate_score_oob(self):
         scores = np.array([])
         for i in range(len(self.models)):
             X_v = self.oob[i]
-            if self.ens_metric_name == "conc":
+            if self.ens_metric_name == "CI":
                 pred = self.models[i].predict(X_v, target=cnt.TIME_NAME)
                 score = concordance_index(X_v[cnt.TIME_NAME], pred)
             else:
                 pred = self.models[i].predict_at_times(X_v, bins=self.bins, mode="surv")
                 y_true = cnt.get_y(X_v[cnt.CENS_NAME], X_v[cnt.TIME_NAME])
                 score = metr.ibs(self.y_train, y_true, pred, self.bins)
             scores = np.append(scores, score)
         return np.round(np.mean(scores), 4)
 
     def aggregate_score_selfoob(self, bins=None):
         is_ibs = self.ens_metric_name.upper().find("IBS") >= 0
-        if self.ens_metric_name in ["conc"] or is_ibs:
+        if self.ens_metric_name in ["CI"] or is_ibs:
             list_target_time = [oob_[cnt.TIME_NAME].to_frame() for oob_ in self.oob]
             target_time = pd.concat(list_target_time, axis=1).mean(axis=1)
 
         if self.ens_metric_name in ["roc"] or is_ibs:
             list_target_cens = [oob_[cnt.CENS_NAME].to_frame() for oob_ in self.oob]
             target_cens = pd.concat(list_target_cens, axis=1).mean(axis=1)
 
-        if self.ens_metric_name in ["conc", "roc"]:
+        if self.ens_metric_name in ["CI", "roc"]:
             pred = pd.concat(self.list_pred_oob, axis=1).mean(axis=1)
-            if self.ens_metric_name == "conc":
+            if self.ens_metric_name == "CI":
                 return concordance_index(target_time, pred)
             return roc_auc_score(target_cens, pred)
 
         if is_ibs:
             pred = pd.concat(self.list_pred_oob, axis=1).apply(lambda r: r.mean(axis=0), axis=1)
             pred = np.array(pred.to_list())
             y_true = cnt.get_y(target_cens, target_time)
@@ -195,65 +195,65 @@
         self.ens_metr = np.zeros(self.n_estimators)
 
         if isinstance(self.size_sample, float):
             self.size_sample = int(self.size_sample * self.X_train.shape[0])
         self.bins = cnt.get_bins(time=self.y_train[cnt.TIME_NAME],
                                  cens=self.y_train[cnt.CENS_NAME])
 
-        if self.ens_metric_name in ["iauc", "likelihood", "bic"] or self.ens_metric_name.upper().find("IBS") >= 0:
+        if self.ens_metric_name in ["iauc", "LOGLIKELIHOOD", "bic"] or self.ens_metric_name.upper().find("IBS") >= 0:
             dim = (self.X_train.shape[0], self.bins.shape[0])
         else:
             dim = (self.X_train.shape[0])
         self.oob_prediction = np.zeros(dim, dtype=np.float)
 
-        if self.ens_metric_name in ["likelihood", "bic"]:
+        if self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
             self.oob_prediction_hf = np.zeros(dim, dtype=np.float)
         self.oob_count = np.zeros((self.X_train.shape[0]), dtype=np.int)
 
         cnt.set_seed(10)
 
     def add_model(self, model, x_oob):
         self.models.append(model)
 
         oob_index = x_oob.index.values
         self.oob_count[oob_index] += 1
-        if self.ens_metric_name == "conc":
+        if self.ens_metric_name == "CI":
             self.oob_prediction[oob_index] += model.predict(x_oob, target=cnt.TIME_NAME)
         elif self.ens_metric_name == "roc":
             self.oob_prediction[oob_index] += model.predict(x_oob, target=cnt.CENS_NAME)
-        elif self.ens_metric_name in ["likelihood", "bic"]:
+        elif self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
             self.oob_count = np.ones((self.X_train.shape[0]), dtype=np.int)
             self.oob_prediction_hf += model.predict_at_times(self.X_train, bins=self.bins, mode="hazard")
             self.oob_prediction += model.predict_at_times(self.X_train, bins=self.bins, mode="surv")
         else:
             self.oob_prediction[oob_index] += model.predict_at_times(x_oob, bins=self.bins, mode="surv")
 
     def select_model(self, start, end):
         self.models = self.models[start:end]
 
     def aggregate_score_selfoob(self):
         index_join_oob = np.where(self.oob_count != 0)
         is_ibs = self.ens_metric_name.upper().find("IBS") >= 0
         if is_ibs:
             pred = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob][:, None]
-        elif self.ens_metric_name in ["likelihood", "bic"]:
+        elif self.ens_metric_name in ["LOGLIKELIHOOD", "bic"]:
             pred_hf = self.oob_prediction_hf[index_join_oob]  # / self.oob_count[index_join_oob][:, None]
             pred_sf = self.oob_prediction[index_join_oob]  # / self.oob_count[index_join_oob][:, None]
         else:
             pred = self.oob_prediction[index_join_oob] / self.oob_count[index_join_oob]
 
         join_oob = self.y_train[index_join_oob]
         target_time = join_oob[cnt.TIME_NAME]
         target_cens = join_oob[cnt.CENS_NAME]
 
-        if self.ens_metric_name == "conc":
+        if self.ens_metric_name == "CI":
             return concordance_index(target_time, pred)
         elif self.ens_metric_name == "roc":
             return roc_auc_score(target_cens, pred)
         elif is_ibs:
             y_true = cnt.get_y(target_cens, target_time)
             return metr.METRIC_DICT[self.ens_metric_name.upper()](self.y_train, y_true, None, pred, None, self.bins)
-        elif self.ens_metric_name == "likelihood":
+        elif self.ens_metric_name == "LOGLIKELIHOOD":
             return metr.loglikelihood(target_time, target_cens, pred_sf, pred_hf, self.bins)
         elif self.ens_metric_name == "bic":
             return metr.bic(len(self.models), self.size_sample, target_time, target_cens, pred_sf, pred_hf, self.bins)
         return None
```

### Comparing `survivors-1.6.2/survivors/ensemble/boosting.py` & `survivors-1.6.3/survivors/ensemble/boosting.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,16 +137,16 @@
             #         break
         
         # if self.tolerance:
         #     self.tolerance_find_best()
         print('fitted:', len(self.models), 'models.')
     
     # def count_model_weights(self, model):
-    #     pred_surv = model.predict_at_times(self.X_train, bins = self.bins, mode = "surv")
-    #     losses = metr.ibs(self.y_train, self.y_train, pred_surv, self.bins, axis = 0)
+    #     pred_sf = model.predict_at_times(self.X_train, bins = self.bins, mode = "surv")
+    #     losses = metr.ibs(self.y_train, self.y_train, pred_sf, self.bins, axis = 0)
     #     wei, betta = count_weight(losses, mode = self.mode_wei)
     #     return wei, betta
     
     # def update_weight(self, wei_i):
     #     self.weights[self.X_train.index] *= wei_i
     
     def count_model_weights(self, model, X_sub, y_sub):
```

### Comparing `survivors-1.6.2/survivors/ensemble/bootstrap.py` & `survivors-1.6.3/survivors/ensemble/bootstrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,18 @@
             x_sub = self.X_train.sample(n=self.size_sample, replace=self.bootstrap, random_state=i)
             x_sub_ind.append(x_sub.index)
 
             x_sub = x_sub.reset_index(drop=True)
             params = self.tree_kwargs.copy()
             params['random_state'] = i
             params['features'] = self.features
+            params['n_jobs'] = 1
             p_s.append({"x_sub": x_sub, "params": params})
 
-        with Parallel(n_jobs=self.tree_kwargs.get("n_jobs", 10), verbose=False, batch_size=10) as parallel:
+        with Parallel(n_jobs=self.tree_kwargs.get("n_jobs", 10), verbose=False) as parallel:
             ml = parallel(delayed(self.fit_tree)(**p) for p in p_s)
 
         for model, x_sub_ind in zip(ml, x_sub_ind):
             x_oob = self.X_train.loc[self.X_train.index.difference(x_sub_ind), :]
             self.add_model(model, x_oob)
         # print(f"fitted: {len(self.models)} models.")
```

### Comparing `survivors-1.6.2/survivors/ensemble/bootstrap_iter.py` & `survivors-1.6.3/survivors/ensemble/bootstrap_iter.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/ensemble/clever_boosting.py` & `survivors-1.6.3/survivors/ensemble/clever_boosting.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .. import metrics as metr
 from ..tree import CRAID
 from .. import constants as cnt
 from .boosting import BoostingCRAID
 import matplotlib.pyplot as plt
 
-# from ..tree.stratified_model import KaplanMeierZeroAfter, NelsonAalen
 from ..external import NelsonAalen, KaplanMeierZeroAfter
 
 
 def f_predict_survival_at_times(ch, bins=None):
     mean, std, prob = ch
     durs = np.random.normal(mean, std, 1000)
     events = np.random.binomial(1, prob, size=1000)
```

### Comparing `survivors-1.6.2/survivors/ensemble/clever_boosting_iter.py` & `survivors-1.6.3/survivors/ensemble/clever_boosting_iter.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -150,8 +150,8 @@
             res_all = self.get_aggreg(res_all, np.array(self.bettas)[:i + 1])
             res_all[:, -1] = 0
             res_all[:, 0] = 1
             if metric == "ibs":
                 metr_vals.append(metr.ibs_WW(self.y_train, y_tmp, res_all, bins))
             else:
                 metr_vals.append(metr.auprc(self.y_train, y_tmp, res_all, bins))
-        plt.plot(range(len(self.models)), metr_vals, label=label)
+        plt.plot(range(len(self.models)), metr_vals, label=label)
```

### Comparing `survivors-1.6.2/survivors/ensemble/clever_boosting_old.py` & `survivors-1.6.3/survivors/ensemble/clever_boosting_old.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/ensemble/ibsboosting.py` & `survivors-1.6.3/survivors/ensemble/ibsboosting.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/ensemble/proboosting.py` & `survivors-1.6.3/survivors/ensemble/proboosting.py`

 * *Files identical despite different names*

### Comparing `survivors-1.6.2/survivors/experiments/grid.py` & `survivors-1.6.3/survivors/experiments/grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 import pandas as pd
 import time
 import os
 import pickle
+import mgzip  # Custom
 
-from sklearn.model_selection import StratifiedKFold
-from sklearn.model_selection import ParameterGrid
-from sklearn.model_selection import train_test_split
+from sklearn.model_selection import StratifiedKFold, ParameterGrid, train_test_split
+from sklearn.preprocessing import StandardScaler
 
 from .. import constants as cnt
 from .. import metrics as metr
 from ..external import LeafModel
 
 
-def to_str_from_dict_list(d, strat):
-    if isinstance(strat, str):
-        return str(d.get(strat, ""))
-    elif isinstance(strat, list):
-        return ";".join([str(d.get(e, "")) for e in strat])
+def to_str_from_dict_list(d, stratify):
+    if isinstance(stratify, str):
+        return str(d.get(stratify, ""))
+    elif isinstance(stratify, list):
+        return ";".join([str(d.get(e, "")) for e in stratify])
     return None
 
 
 def prepare_sample(X, y, train_index, test_index):
     X_train, X_test = X.iloc[train_index, :], X.iloc[test_index, :]
     y_train, y_test = y[train_index], y[test_index]
 
@@ -49,14 +49,16 @@
     ----------
     X : Pandas dataframe
         Contain input features of events.
     y : structured array
         Contain censuring flag and time of events.
     folds : int
         Quantity of cross-validate folds.
+    mode : str
+        Validation scenario.
 
     Yields
     ------
     X_train : Pandas dataframe
         Contain input features of train sample.
     y_train : array-like
         Contain censuring flag and time of train sample.
@@ -98,45 +100,49 @@
     elif mode == "CV":
         for train_index, test_index in skf.split(X, discr):  # y[cnt.CENS_NAME]):
             X_train, y_train, X_test, y_test, bins = prepare_sample(X, y, train_index, test_index)
             yield X_train, y_train, X_test, y_test, bins
     pass
 
 
-def count_metric(y_train, y_test, pred_time, pred_surv, pred_haz, bins, metrics_names):
-    return np.array([metr.METRIC_DICT[metr_name](y_train, y_test, pred_time, pred_surv, pred_haz, bins)
+def count_metric(y_train, y_test, pred_time, pred_sf, pred_hf, bins, metrics_names):
+    return np.array([metr.METRIC_DICT[metr_name](y_train, y_test, pred_time, pred_sf, pred_hf, bins)
                      for metr_name in metrics_names])
 
 
 def get_name_file(method, params, mode, fold):
-    filter_params = ["categ", "ens_metric_name", "aggreg_func"]
+    filter_params = ["categ", "ens_metric_name", "aggreg_func", "n_jobs"]
     name_lst = [method.__name__]
-    name_lst += [v for k, v in params.items() if not(k in filter_params)]
+    name_lst += [v for k, v in params.items() if not (k in filter_params)]
     name_lst += [mode, fold]
     return "_".join(map(str, name_lst))
 
 
 def get_fit_eval_func(method, X, y, folds, metrics_names=['CI'], mode="CV", dir_path=None):
     """
     Return function, which on sample X, y apply cross-validation and calculate 
-    metrics on each folds. 
+    metrics for each fold.
 
     Parameters
     ----------
-    method : object
+    method : class
         Must have methods for fitting, predicting time, hazard and survival func
             
     X : Pandas dataframe
         Contain input features of events.
     y : structured array
         Contain censuring flag and time of events.
     folds : int
         Quantity of cross-validate folds.
     metrics_names : TYPE, optional
         DESCRIPTION. The default is ['CI'].
+    mode : str
+        Validation scenario.
+    dir_path : str
+        Path to cache directory (for loading pretrained models).
 
     Returns
     -------
     functions
         Recieve hyperparameters and return list of metrics arrays.
         Allow to use in ParameterGrid.
 
@@ -155,55 +161,59 @@
                     est.aggreg_func = kwargs.get("aggreg_func", "mean")
                     est.tolerance_find_best(kwargs["ens_metric_name"])
                 else:
                     name = os.path.join(dir_path, get_name_file(method, kwargs, mode, fold) + '.pkl')
                     if not os.path.exists(name):
                         print("Fitted from scratch")
                         est.fit(X_train, y_train)
-                        with open(name, 'wb') as out:
+                        with mgzip.open(name, 'wb') as out:  # Custom
                             pickle.dump(est, out, pickle.HIGHEST_PROTOCOL)
 
-                    with open(name, 'rb') as inp:
+                    with mgzip.open(name, 'rb') as inp:
                         est = pickle.load(inp)
                         est.aggreg_func = kwargs.get("aggreg_func", None)
                         est.tolerance_find_best(kwargs["ens_metric_name"])
 
-                pred_surv = est.predict_at_times(X_test, bins=bins, mode="surv")
-                pred_surv[:, -1] = 0
-                pred_surv[:, 0] = 1
+                pred_sf = est.predict_at_times(X_test, bins=bins, mode="surv")
+                pred_sf[:, -1] = 0
+                pred_sf[:, 0] = 1
                 pred_time = est.predict(X_test, target=cnt.TIME_NAME)
-                pred_haz = est.predict_at_times(X_test, bins=bins, mode="hazard")
+                pred_hf = est.predict_at_times(X_test, bins=bins, mode="hazard")
             elif isinstance(est, LeafModel):
                 X_train[cnt.TIME_NAME] = y_train[cnt.TIME_NAME]
                 X_train[cnt.CENS_NAME] = y_train[cnt.CENS_NAME]
                 est.fit(X_train)
-                pred_surv = est.predict_survival_at_times(X_test, bins=bins)
+                pred_sf = est.predict_survival_at_times(X_test, bins=bins)
                 pred_time = est.predict_feature(X_test, feature_name=cnt.TIME_NAME)
-                pred_haz = est.predict_hazard_at_times(X_test, bins=bins)
+                pred_hf = est.predict_hazard_at_times(X_test, bins=bins)
             else:  # Methods from scikit-survival
                 s = pd.isna(X_train).sum(axis=0) != X_train.shape[0]
                 valid_feat = s[s].index
-                # X_train = X_train[valid_feat].fillna(0).replace(np.nan, 0).replace(np.inf, 0)
-                # X_test = X_test[valid_feat].fillna(0).replace(np.nan, 0).replace(np.inf, 0)
-                med_val = X_train[valid_feat].median()
+                med_val = 0
+                # med_val = X_train[valid_feat].median()
+                # med_val = X_train[valid_feat].mean()
                 X_train = X_train[valid_feat].fillna(med_val).replace(np.nan, med_val).replace(np.inf, med_val)
                 X_test = X_test[valid_feat].fillna(med_val).replace(np.nan, med_val).replace(np.inf, med_val)
 
+                scaler = StandardScaler()
+                X_train = scaler.fit_transform(X_train)
+                X_test = scaler.transform(X_test)
+
                 est = est.fit(X_train, y_train)
                 survs = est.predict_survival_function(X_test)
                 hazards = est.predict_cumulative_hazard_function(X_test)
-                pred_surv = np.array(list(map(lambda x: x(bins), survs)))
-                pred_haz = np.array(list(map(lambda x: x(bins), hazards)))
-                pred_time = -1*est.predict(X_test)
-                # pred_time = np.trapz(pred_surv, bins)
+                pred_sf = np.array(list(map(lambda x: x(bins), survs)))
+                pred_hf = np.array(list(map(lambda x: x(bins), hazards)))
+                pred_time = -1 * est.predict(X_test)
+                # pred_time = np.trapz(pred_sf, bins)
                 # Integral version from: https://lifelines.readthedocs.io/en/latest/fitters/regression/CoxPHFitter.html
 
             exec_times.append(time.time() - s_time)
             metr_lst.append(count_metric(y_train, y_test, pred_time,
-                                         pred_surv, pred_haz, bins, metrics_names))
+                                         pred_sf, pred_hf, bins, metrics_names))
             fold += 1
             del est
         return np.vstack(metr_lst), np.array(exec_times)
     return f
 
 
 def bins_scheme(val, scheme=""):
@@ -268,24 +278,21 @@
         self.metric_best_p = "IBS"
         self.way_best_p = "min"
 
         self.is_table = False
         self.folds = folds
         self.except_stop = except_stop
         self.dataset_name = dataset_name
+        self.dir_path = None
 
         self.result_table = None
         self.mode = mode
         self.bins_sch = bins_sch
 
     def add_metric_best(self, metric):
-        if metric == "conc":
-            metric = "CI"
-        if metric == "likelihood":
-            metric = "LOGLIKELIHOOD"
         if metric in self.metrics:
             self.metric_best_p = metric
             self.way_best_p = "min" if metric in metr.DESCEND_METRICS else "max"
 
     def add_method(self, method, grid):
         self.methods.append(method)
         self.methods_grid.append(grid)
@@ -311,49 +318,45 @@
             p_size = len(grid_params)
             for i_p, p in enumerate(grid_params):
                 try:
                     eval_metr, exec_times = fit_eval_func(**p)
                     curr_dict = {"METHOD": method.__name__, "CRIT": p.get("criterion", ""),
                                  "PARAMS": str(p), "TIMES": exec_times, "TIME": np.sum(exec_times)}
                     eval_metr = {m: eval_metr[:, i] for i, m in enumerate(self.metrics)}
-                    curr_dict.update(eval_metr)  # dict(zip(self.metrics, eval_metr))
-                    # self.result_table = self.result_table.append(curr_dict, ignore_index=True)
+                    curr_dict.update(eval_metr)
                     self.result_table = pd.concat([self.result_table, pd.DataFrame([curr_dict])], ignore_index=True)
                     if verbose > 0:
                         print(f"Iteration: {i_p + 1}/{p_size}")
                         print(f"EXECUTION TIME OF {method.__name__}: {exec_times}",
-                                  {k: [np.mean(v), np.mean(v[:-1]), v[-1]] for k, v in eval_metr.items()})  # np.mean(v)
+                              {k: [np.mean(v), np.mean(v[:-1]), v[-1]] for k, v in eval_metr.items()})  # np.mean(v)
                 except KeyboardInterrupt:
-                    print("HANDELED KeyboardInterrupt")
+                    print("Handled KeyboardInterrupt")
                     break
                 except Exception as e:
                     print("Method: %s, Param: %s finished with except '%s'" % (method.__name__, str(p), e))
-                    #if self.except_stop == "all":
-                    #    break
+                    if self.except_stop == "all":
+                        break
                     curr_dict = {"METHOD": method.__name__, "CRIT": p.get("criterion", ""),
                                  "PARAMS": str(p), "TIME": -1}
                     curr_dict.update({m: np.array([np.nan, np.nan]) for i, m in enumerate(self.metrics)})
                     self.result_table = pd.concat([self.result_table, pd.DataFrame([curr_dict])], ignore_index=True)
         if self.mode in ["TIME-CV", "CV+HOLD-OUT"]:
             for m in self.metrics:
                 self.result_table[f"{m}_pred_mean"] = self.result_table[m].apply(lambda x: np.mean(x[:-1]))
             for m in self.metrics:
                 self.result_table[f"{m}_last"] = self.result_table[m].apply(lambda x: x[-1])
 
         for m in self.metrics:
             self.result_table[f"{m}_mean"] = self.result_table[m].apply(np.mean)
 
         self.is_table = True
-        # if not(dir_path is None):
-        #     # add_time = strftime("%H:%M:%S", gmtime(time.time()))
-        #     self.save(dir_path)
 
     def run_effective(self, X, y, dir_path=None, verbose=0,
                       stratify_best=["criterion", "balance", "leaf_model", "l_reg"]):
-        if not(self.mode in ["CV+SAMPLE"]):
+        if not (self.mode in ["CV+SAMPLE"]):
             self.run(X, y, dir_path=dir_path, verbose=verbose)
             return None
 
         y["time"] = bins_scheme(y["time"], scheme=self.bins_sch)
         self.bins_sch = ""
 
         folds = 20 if self.mode == "CV+SAMPLE" else 1
@@ -431,16 +434,16 @@
         df_time_cv_best = self.get_agg_results(self.result_table, self.metric_best_p + "_pred_mean",
                                                choose=self.way_best_p, stratify=stratify)
         return df_time_cv_best
 
     def get_hold_out_result(self, stratify="criterion"):
         df_hold_out_best = self.get_agg_results(self.result_table, self.metric_best_p + "_pred_mean",
                                                 choose=self.way_best_p, stratify=stratify)
-        rename_d = {metr + "_pred_mean": metr + "_CV_mean" for metr in self.metrics}
-        rename_d.update({metr + "_last": metr + "_HO" for metr in self.metrics})
+        rename_d = {m + "_pred_mean": m + "_CV_mean" for m in self.metrics}
+        rename_d.update({m + "_last": m + "_HO" for m in self.metrics})
         return df_hold_out_best.rename(rename_d, axis=1)
 
     def get_result(self):
         return self.result_table
 
     def get_sample_result(self):
         return self.sample_table
```

### Comparing `survivors-1.6.2/survivors/external/leaf_model.py` & `survivors-1.6.3/survivors/external/leaf_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,62 @@
 import numpy as np
 from .. import constants as cnt
 
 
 class LeafModel(object):
+    """
+    Unified wrapper for external models.
+    Can be used as leaf model in tree-based methods.
+    Supported in Experiments module.
 
+    Attributes
+    ----------
+    features : list
+        Covariates for fitting
+    features_predict : dict
+        Description values of features (mean by default)
+    lists: dict
+        Source values of target variables
+    weights_name : str
+        Name of the weighting column
+    kwargs : dict
+        Internal parameters for the leaf model
+
+    Methods
+    -------
+    fit : build ensemble on source X_node data
+    predict_list_feature : return full data of variables
+    predict_feature : return aggregated data of variables
+    predict_survival_at_times : return survival function by bins
+    predict_hazard_at_times : return hazard function by bins
+
+    """
     def __init__(self, features=[], weights_name=None, **kwargs):
         self.kwargs = kwargs
         self.features = features
         self.shape = None
         self.features_predict = dict()
         self.lists = dict()
-        self.default_bins = np.array([1, 10, 100, 1000])
         self.weights_name = weights_name
+        self.weights = None
 
     def fit(self, X_node, *args, **kwargs):
         if self.features == []:
             self.features = X_node.columns
+        # self.features = sorted(list(set(self.features + [cnt.TIME_NAME, cnt.CENS_NAME])))
+        # X_sub = X_node[self.features]
+        # self.shape = X_sub.shape
+        # self.features_predict = X_sub.mean(axis=0).to_dict()
+        # self.lists = X_sub[[cnt.TIME_NAME, cnt.CENS_NAME]].to_dict(orient="list")
+
+        self.shape = (X_node.shape[0], len(self.features))
+        l = dict(zip(X_node.columns, X_node.values.T))
+        self.lists = {k: v for k, v in l.items() if k in ["time", "cens"]}
+        self.features_predict = {k: np.mean(v) for k, v in l.items() if k in self.features}
 
-        X_sub = X_node[self.features]
-        self.shape = X_sub.shape
-        self.features_predict = X_sub.mean(axis=0).to_dict()
-        self.lists = X_sub[[cnt.TIME_NAME, cnt.CENS_NAME]].to_dict(orient="list")
         if self.weights_name is None:
             self.weights = None
         else:
             if self.weights_name in X_node.columns:
                 self.weights = X_node[self.weights_name].to_numpy()
             else:
                 self.weights = np.ones(self.shape[0])
```

### Comparing `survivors-1.6.2/survivors/external/nonparametric.py` & `survivors-1.6.3/survivors/external/nonparametric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
-import scipy.stats as ss
+from scipy.stats import norm
 from .leaf_model import NonparamLeafModel, MixLeafModel, NormalizedLeafModel, MeaningLeafModel
 from lifelines import KaplanMeierFitter, NelsonAalenFitter
 
+
 def epanechnikov_kernel(t, T, bandwidth=1.0):
     M = 0.75 * (1 - ((t - T) / bandwidth) ** 2)
     M[abs((t - T)) >= bandwidth] = 0
     return M
 
 
 class KaplanMeier:
@@ -26,16 +27,16 @@
         dur_ = np.searchsorted(self.timeline, durations)
         hist_dur = np.bincount(dur_, weights=weights)
         self.hist_cens = np.bincount(dur_, weights=right_censor * weights)
         self.cumul_hist_dur = np.cumsum(hist_dur[::-1])[::-1]
         self.survival_function = np.hstack([1.0, np.cumprod((1.0 - self.hist_cens / (self.cumul_hist_dur)))])
 
     def count_confidence_interval(self):
-        ''' exponential Greenwood: https://www.math.wustl.edu/~sawyer/handouts/greenwood.pdf '''
-        z = ss.norm.ppf(1 - self.alpha / 2)
+        """ Calculated by exponential Greenwood: https://www.math.wustl.edu/~sawyer/handouts/greenwood.pdf """
+        z = norm.ppf(1 - self.alpha / 2)
         cumulative_sq_ = np.sqrt(np.hstack(
             [0.0, np.cumsum(self.hist_cens / (self.cumul_hist_dur * (self.cumul_hist_dur - self.hist_cens)))]))
         np.nan_to_num(cumulative_sq_, copy=False, nan=0)
         v = np.log(self.survival_function)
         np.nan_to_num(v, copy=False, nan=0)
         self.confidence_interval_ = np.vstack([np.exp(v * np.exp(- z * cumulative_sq_ / v)),
                                                np.exp(v * np.exp(+ z * cumulative_sq_ / v))]).T
@@ -62,15 +63,15 @@
         right_censor = right_censor.astype("bool")
         dur_ = np.searchsorted(self.timeline, durations)
 
         self.hist_cens = np.bincount(dur_, weights=right_censor * weights)
         self.cumul_hist_dur = np.cumsum(self.hist_cens[::-1])[::-1]
         self.cumul_hist_dur[self.cumul_hist_dur == 0] = 1e-3  # Any cnt (in sf it becomes zero)
 
-        self.survival_function = np.hstack([1.0, np.cumprod((1.0 - self.hist_cens / (self.cumul_hist_dur)))])
+        self.survival_function = np.hstack([1.0, np.cumprod((1.0 - self.hist_cens / self.cumul_hist_dur))])
 
         N = right_censor.shape[0]
         Ncens = right_censor[~right_censor].shape[0]
         self.survival_function = Ncens / N + (1 - Ncens / N) * self.survival_function
 
 
 class NelsonAalen:
@@ -128,22 +129,23 @@
         # place_bin = np.digitize(times, self.timeline)  # -1
         sf = self.survival_function[np.clip(place_bin, 0, None)]
         sf[times > self.timeline[-1]] = 0
         sf[times < self.timeline[0]] = 1
         return sf
 
 
-
 class BaseLeafModel(NonparamLeafModel):
     survival_class = KaplanMeier
     hazard_class = NelsonAalen
 
+
 class BaseLeafModelOnlySurv(NonparamLeafModel):
     survival_class = KaplanMeier
 
+
 class BaseLeafModelOnlyHazard(NonparamLeafModel):
     hazard_class = NelsonAalen
 
 
 class BaseNormalizedLeafModel(NormalizedLeafModel):
     survival_class = KaplanMeierZeroAfter
     hazard_class = NelsonAalen
@@ -154,14 +156,15 @@
     hazard_class = NelsonAalen
 
 
 class BaseMixLeafModel(MixLeafModel):
     survival_class = KaplanMeierZeroAfter
     hazard_class = NelsonAalen
 
+
 class BaseLeafModeLL(NonparamLeafModel):
     survival_class = KaplanMeierFitter
     hazard_class = NelsonAalenFitter
 
 
 LEAF_NONPARAM_DICT = {
     "base": BaseLeafModel,
```

### Comparing `survivors-1.6.2/survivors/external/parametric.py` & `survivors-1.6.3/survivors/external/parametric.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 AFT_param_grid = PARAM_GRID.copy()
 CoxPH_param_grid = PARAM_GRID.copy()
 
 
 class ParametricLifelinesBase(LeafModel):
     base_model = None
 
-    def __init__(self, except_stop=True, **kwargs):
+    def __init__(self, except_stop=False, **kwargs):
         self.model = None
         self.except_stop = except_stop
         super().__init__(**kwargs)
 
     def prepare_data(self, X):
         if X is None:
             if self.model is None:
@@ -56,17 +56,20 @@
 
     def predict_hazard_at_times(self, X=None, bins=None):
         X = self.prepare_data(X)
         chf = self.model.predict_cumulative_hazard(X, times=bins).to_numpy().T
         return chf
 
     def predict_feature(self, X=None, feature_name=None):
-        X = self.prepare_data(X)
         if feature_name == cnt.TIME_NAME:
-            return self.model.predict_expectation(X).to_numpy()
+            ts = np.linspace(self.model.durations.min(), self.model.durations.max(), 100)
+            sf = self.predict_survival_at_times(X=X, bins=ts)
+            return np.trapz(sf, ts, axis=1)
+            # return self.model.predict_expectation(X).to_numpy()
+        X = self.prepare_data(X)
         return super().predict_feature(X, feature_name)
 
 
 class WeibullAFT(ParametricLifelinesBase):
     base_model = WeibullAFTFitter
```

### Comparing `survivors-1.6.2/survivors/metrics.py` & `survivors-1.6.3/survivors/metrics.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,58 +3,58 @@
 from numba import njit, jit
 from lifelines import KaplanMeierFitter, NelsonAalenFitter
 from lifelines.utils import concordance_index
 
 from .constants import TIME_NAME, CENS_NAME
 
 METRIC_DICT = {
-    "CI": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        concordance_index(y_tst[TIME_NAME], pr_time),
-    "CI_CENS": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        concordance_index(y_tst[TIME_NAME], pr_time, y_tst[CENS_NAME]),
-
-    "IBS": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        ibs(y_tr, y_tst, pr_surv, bins),
-    "BAL_IBS": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        bal_ibs(y_tr, y_tst, pr_surv, bins),
-
-    "IBS_WW": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        ibs_WW(y_tr, y_tst, pr_surv, bins),
-    "BAL_IBS_WW": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        bal_ibs_WW(y_tr, y_tst, pr_surv, bins),
-
-    "IBS_REMAIN": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        ibs_remain(y_tr, y_tst, pr_surv, bins),
-    "BAL_IBS_REMAIN": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        bal_ibs_remain(y_tr, y_tst, pr_surv, bins),
-
-    "IAUC": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        iauc(y_tr, y_tst, pr_haz, bins),
-    "IAUC_WW": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        iauc_WW(y_tr, y_tst, pr_haz, bins),
-    "IAUC_TI": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        iauc_TI(y_tr, y_tst, pr_haz, bins),
-    "IAUC_WW_TI": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        iauc_WW_TI(y_tr, y_tst, pr_haz, bins),
-
-    "AUPRC": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        auprc(y_tr, y_tst, pr_surv, bins),
-    "AUPRC_by_obs": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        auprc(y_tr, y_tst, pr_surv, bins, axis=3),
-    "EVENT_AUPRC": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        event_auprc(y_tr, y_tst, pr_surv, bins),
-    "CENS_AUPRC": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        cens_auprc(y_tr, y_tst, pr_surv, bins),
-    "BAL_AUPRC": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        bal_auprc(y_tr, y_tst, pr_surv, bins),
-
-    "LOGLIKELIHOOD": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        loglikelihood(y_tst[TIME_NAME], y_tst[CENS_NAME], pr_surv, pr_haz, bins),
-    "KL": lambda y_tr, y_tst, pr_time, pr_surv, pr_haz, bins:
-        kl(y_tst[TIME_NAME], y_tst[CENS_NAME], pr_surv, pr_haz, bins)
+    "CI": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        concordance_index(y_tst[TIME_NAME], pred_time),
+    "CI_CENS": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        concordance_index(y_tst[TIME_NAME], pred_time, y_tst[CENS_NAME]),
+
+    "IBS": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        ibs(y_tr, y_tst, pred_sf, bins),
+    "BAL_IBS": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        bal_ibs(y_tr, y_tst, pred_sf, bins),
+
+    "IBS_WW": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        ibs_WW(y_tr, y_tst, pred_sf, bins),
+    "BAL_IBS_WW": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        bal_ibs_WW(y_tr, y_tst, pred_sf, bins),
+
+    "IBS_REMAIN": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        ibs_remain(y_tr, y_tst, pred_sf, bins),
+    "BAL_IBS_REMAIN": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        bal_ibs_remain(y_tr, y_tst, pred_sf, bins),
+
+    "IAUC": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        iauc(y_tr, y_tst, pred_hf, bins),
+    "IAUC_WW": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        iauc_WW(y_tr, y_tst, pred_hf, bins),
+    "IAUC_TI": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        iauc_TI(y_tr, y_tst, pred_hf, bins),
+    "IAUC_WW_TI": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        iauc_WW_TI(y_tr, y_tst, pred_hf, bins),
+
+    "AUPRC": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        auprc(y_tr, y_tst, pred_sf, bins),
+    "AUPRC_by_obs": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        auprc(y_tr, y_tst, pred_sf, bins, axis=3),
+    "EVENT_AUPRC": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        event_auprc(y_tr, y_tst, pred_sf, bins),
+    "CENS_AUPRC": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        cens_auprc(y_tr, y_tst, pred_sf, bins),
+    "BAL_AUPRC": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        bal_auprc(y_tr, y_tst, pred_sf, bins),
+
+    "LOGLIKELIHOOD": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        loglikelihood(y_tst[TIME_NAME], y_tst[CENS_NAME], pred_sf, pred_hf, bins),
+    "KL": lambda y_tr, y_tst, pred_time, pred_sf, pred_hf, bins:
+        kl(y_tst[TIME_NAME], y_tst[CENS_NAME], pred_sf, pred_hf, bins)
 }
 """ dict: Available metrics in library and its realization """
 
 DESCEND_METRICS = ['ibs', 'IBS', 'aic', "AIC", "bic", "BIC", "KL",
                    "BAL_IBS", "IBS_WW", "BAL_IBS_WW", "IBS_REMAIN", "BAL_IBS_REMAIN"]
 """ list: Metrics with decreasing quality improvement """
 
@@ -62,15 +62,15 @@
 def auprc(survival_train, survival_test, estimate, times, axis=-1):
     time = survival_test["time"]
     event = survival_test["cens"]
 
     steps = np.linspace(1e-5, 1 - 1e-5, 100)
     before_time = np.dot(time[:, np.newaxis], steps[np.newaxis, :])
     after_time = np.dot(time[:, np.newaxis], 1 / steps[np.newaxis, :])  # TODO OLD
-    #after_time = time[:, np.newaxis] + np.dot(times[-1] - time[:, np.newaxis], steps[np.newaxis, :])
+
     before_ind = np.clip(np.searchsorted(times, before_time), 0, times.shape[0] - 1)
     after_ind = np.clip(np.searchsorted(times, after_time), 0, times.shape[0] - 1)
 
     est = np.take_along_axis(estimate, before_ind, axis=1)
     est[event] -= np.take_along_axis(estimate[event], after_ind[event], axis=1)
 
     if axis == -1:  # mean for each time and observation
@@ -99,14 +99,15 @@
 
 
 def event_auprc(survival_train, survival_test, estimate, times, axis=-1):
     auprc_event = auprc(survival_train, survival_test[survival_test["cens"]],
                         estimate[survival_test["cens"]], times, axis=axis)
     return auprc_event
 
+
 def cens_auprc(survival_train, survival_test, estimate, times, axis=-1):
     auprc_cens = auprc(survival_train, survival_test[~survival_test["cens"]],
                        estimate[~survival_test["cens"]], times, axis=axis)
     return auprc_cens
 
 
 @njit
@@ -248,18 +249,16 @@
 
     estim_before = np.square(estimate) * test_event[np.newaxis, :].T
     estim_after = np.square(1 - estimate)
     brier_scores = np.array([np.where(test_time < t,
                                       estim_before[:, i],
                                       estim_after[:, i])
                              for i, t in enumerate(times)])
-    N = np.sum(np.array([np.where(test_time < t,
-                                      test_event,
-                                      1)
-                             for i, t in enumerate(times)]), axis=1)
+    N = np.sum(np.array([np.where(test_time < t, test_event, 1)
+                         for i, t in enumerate(times)]), axis=1)
     # ind = np.digitize(test_time, times)
     # n_cens = np.bincount(ind[~test_event], minlength=times.shape[0])
     #
     # N = np.ones(times.shape) * np.sum(test_event)
     # if n_cens.shape[0] > 0:
     #     N += np.cumsum(n_cens[::-1])[::-1]
     time_diff = times[-1] - times[0] if times[-1] > times[0] else 1
@@ -335,19 +334,19 @@
 
     # fit and transform IPCW
     if no_wei:
         ipcw = np.ones(test_time.shape[0])
     else:
         cens = sksurv.metrics.CensoringDistributionEstimator()
         cens.fit(survival_train)
-        Ghat = cens.predict_proba(test_time[test_event])
+        g_hat = cens.predict_proba(test_time[test_event])
         ipcw = np.zeros(test_time.shape[0])
-        Ghat[Ghat == 0] = np.inf
-        if not((Ghat == 0.0).any()):
-            ipcw[test_event] = 1.0 / Ghat
+        g_hat[g_hat == 0] = np.inf
+        if not ((g_hat == 0.0).any()):
+            ipcw[test_event] = 1.0 / g_hat
         else:
             ipcw = np.ones(test_time.shape[0])
 
     # expand arrays to (n_samples, n_times) shape
     test_time = np.broadcast_to(test_time[:, np.newaxis], (n_samples, n_times))
     test_event = np.broadcast_to(test_event[:, np.newaxis], (n_samples, n_times))
     times_2d = np.broadcast_to(times, (n_samples, n_times))
@@ -403,17 +402,19 @@
             return integral / (1.0 - s_times[-1])
     return scores[0]
 
 
 def iauc_WW(s_tr, s_tst, est, times, tied_tol=1e-8):
     return iauc(s_tr, s_tst, est, times, tied_tol=tied_tol, no_wei=True)
 
+
 def iauc_TI(s_tr, s_tst, est, times, tied_tol=1e-8):
     return iauc(s_tr, s_tst, est, times, tied_tol=tied_tol, no_wei=False, time_int=True)
 
+
 def iauc_WW_TI(s_tr, s_tst, est, times, tied_tol=1e-8):
     return iauc(s_tr, s_tst, est, times, tied_tol=tied_tol, no_wei=True, time_int=True)
 
 
 def ipa(survival_train, survival_test, estimate, times, axis=-1):
     """
     Index of Prediction Accuracy: General R^2 for binary outcome and right
@@ -482,15 +483,16 @@
 def aic(num_params, time, cens, sf, cumhf, bins):
     return 2*num_params - 2*loglikelihood(time, cens, sf, cumhf, bins)
 
 
 def bic(k, n, time, cens, sf, cumhf, bins):
     return k*np.log(n) - 2*loglikelihood(time, cens, sf, cumhf, bins)
 
-"""ESTIMATE FUNCTION"""
+
+""" ESTIMATE FUNCTION """
 
 
 def get_survival_func(ddeath, cdeath, bins=None):
     """
     Build Kaplan-Meier Estimate of survival function
 
     Parameters
@@ -507,15 +509,15 @@
     KaplanMeierFitter or array
         If bins is None return kaplan-meier model, 
                    else return values of SF.
 
     """
     kmf = KaplanMeierFitter()
     kmf.fit(ddeath, cdeath)
-    if not(bins is None):
+    if not (bins is None):
         return kmf.survival_function_at_times(bins).to_numpy()
     return kmf
 
 
 def get_hazard_func(ddeath, cdeath, bins=None):
     """
     Build Nelson-Aalen Estimate of Hazard function
@@ -534,50 +536,18 @@
     NelsonAalenFitter or array
         If bins is None return Nelson-Aalen model, 
                    else return values of HF.
 
     """
     naf = NelsonAalenFitter()
     naf.fit(ddeath, cdeath)
-    if not(bins is None):
+    if not (bins is None):
         return naf.cumulative_hazard_at_times(bins).to_numpy()
     return naf
 
-# def get_norm_hist(x, b):
-#     a = np.histogram(x,bins = b)[0]
-#     return a/sum(a)
-
-# def plot_predict_surv(surves, bins, true_time, cens = 1):
-#     """
-#     RUN:
-#         res = ssc.get_score_survival_methods(X_tv, X_tst, new_sign[:-9], bins, True)
-#         plot_predict_surv({i:j[0] for i,j in res.items()}, bins, 150.0, 1)
-#     """
-#     fig, ax = plt.subplots()
-    
-#     for name, surv in surves.items():
-#         ax.plot(bins, surv, 
-#                 label = f"{name}, prob:{round(min(surv[np.where(bins < true_time)]),3)}")
-#     ax.vlines(true_time, 0, 1, 
-#               color = 'k', 
-#               linestyles = ('dashed' if cens else 'solid'),
-#               linewidth = 2)
-#     ax.legend()
-#     plt.ylim(-0.1, 1.1)
-#     plt.show()
-
-# def print_importance(feature, importance):
-#     plt.subplots(figsize=(30, 8))
-#     res = {f:i for f,i in zip(feature, importance)}
-#     res = dict(sorted(res.items(), key = lambda x: x[1]))
-#     print(res)
-#     res = dict(sorted(res.items(), key = lambda x: abs(x[1]))[-15:])
-#     res = dict(sorted(res.items(), key = lambda x: x[1]))
-#     plt.bar(res.keys(), res.values())
-#     plt.show()
 
 IBS_DICT = {
     m.__name__.upper(): m
     for m in [ibs, bal_ibs,
               ibs_WW, bal_ibs_WW,
               ibs_remain, bal_ibs_remain]
-}
+}
```

### Comparing `survivors-1.6.2/survivors/scheme/scheme.py` & `survivors-1.6.3/survivors/scheme/scheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import random
 from .. import metrics as metr
 from .. import criteria as scrit
-from scipy import stats
+from ..criteria import chi2_sf
+# from scipy.stats import chi2
 
 import matplotlib.pyplot as plt
 import seaborn as sns
 sns.set()
 
 
 class Scheme(object):
@@ -77,15 +78,15 @@
         for i1, l1 in enumerate(base.keys()):
             for i2, l2 in enumerate(base.keys()):
                 if i2 > i1:
                     diff_dict[l1 + '#' + l2] = scrit.logrank(base[l1].times, base[l2].times, base[l1].cens,
                                                              base[l2].cens)
         while len(base) > 1:
             max_pair_key, min_stat_val = min(diff_dict.items(), key=lambda x: x[1])
-            max_p_val = stats.chi2.sf(min_stat_val, df=1)
+            max_p_val = chi2_sf(min_stat_val, df=1)
             print('Максимальное P-value:', max_p_val)
             if max_p_val < sign_thres:
                 break
             f_l, s_l = max_pair_key.split('#')
             new_sch = base[f_l].copy().join(base[s_l])
             new_sch_name = new_sch.get_str_rules()
             for k in [f_l, s_l]:
```

### Comparing `survivors-1.6.2/survivors/tree/decision_tree.py` & `survivors-1.6.3/survivors/tree/decision_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import pandas as pd
 import numpy as np
 import os
 import copy
 import tempfile
 
-from graphviz import Digraph
+from graphviz import Digraph, set_jupyter_format
+set_jupyter_format('png')
+
 from sklearn.metrics import roc_auc_score
-from sklearn.preprocessing import OneHotEncoder
-from sksurv.linear_model import CoxPHSurvivalAnalysis
 
 from .node import Node
 from ..scheme import FilledSchemeStrategy
 from .. import constants as cnt
 
 import matplotlib.pyplot as plt
 from imblearn.over_sampling import RandomOverSampler
 
-# import seaborn as sns
-# sns.set()
-
 
 def format_to_pandas(X, columns):
     type_df = type(X)
     if type_df.__name__ == "DataFrame":
         return X[columns].reset_index(drop=True)
     elif type_df.__name__ == "ndarray":
         return pd.DataFrame(X, columns=columns)
@@ -33,17 +30,14 @@
     oversample = RandomOverSampler(sampling_strategy='minority', random_state=42)
     df_over, _ = oversample.fit_resample(df, df[target])
     return df_over
 
 
 """ Functions of prunning """
 
-def ols(a, b):
-    return sum((a - b) ** 2)
-
 
 def find_best_uncut(tree, X, y, target, mode_f, choose_f):
     span_leaf = tree.get_spanning_leaf_numbers()
     d = {}
     for el in span_leaf:
         y_pred = tree.predict(X, target=target, end_list=[el])
         d[el] = round(mode_f(y, y_pred), 4)
@@ -105,40 +99,35 @@
         Available features
     categ : list
         Names of categorical features
     random_state : int
         Fixed seed for building reproducibility
     name : str
         Model's name
-    coxph : CoxPHSurvivalAnalysis
-        Model for hazard prediction
-    ohenc : OneHotEncoder
-        Encoding model from number of Node to indicators
     bins : array-like
         Points of timeline.
     info : dict
         Parameters for building nodes
 
     Methods
     -------
 
     fit : build decision tree with X, y data (iterative splitting node)
-    fit_cox_hazard : fitting Cox model as aggregating model by leaf numbers
     predict : return values of features, rules or schemes
-    predict_cox_hazard : return survival or hazard function from cox model
     predict_at_times : return survival or hazard function
     predict_schemes : return FilledSchemeStrategy or Scheme
     cut_tree : pruning function
 
     visualize : build graphviz Digraph for each node
     translate : Replace rules and features by dictionary
 
     get_leaf_numbers : return leaf numbers from nodes
     get_spanning_leaf_numbers : return pre-leaves numbers from nodes
     delete_leaves_by_span : set up pre-leaves from lists to leaves
+
     """
     def __init__(self, depth=0,
                  random_state=123,
                  features=[],
                  categ=[],
                  cut=False,
                  balance=None,
@@ -148,16 +137,14 @@
         self.balance = balance
         self.nodes = dict()
         self.depth = depth
         self.features = features
         self.categ = categ
         self.random_state = random_state
         self.name = f"CRAID_{self.random_state}"
-        self.coxph = None
-        self.ohenc = None
         self.bins = []
 
     def update_params(self, X_tr):
         if not ("min_samples_leaf" in self.info):
             self.info["min_samples_leaf"] = 0.01
         if isinstance(self.info["min_samples_leaf"], float):
             self.info["min_samples_leaf"] = max(int(self.info["min_samples_leaf"] * X_tr.shape[0]), 1)
@@ -201,45 +188,30 @@
 
         self.nodes[0] = Node(X_tr, features=self.features, categ=self.categ, **self.info)
         stack_nodes = np.array([0], dtype=int)
         while stack_nodes.shape[0] > 0:
             node = self.nodes[stack_nodes[0]]
             stack_nodes = stack_nodes[1:]
             if node.depth >= self.depth:
+                node.set_leaf()
                 continue
             sub_nodes = node.split()
             if sub_nodes.shape[0] > 0:
                 sub_numbers = np.array([len(self.nodes) + i for i in range(sub_nodes.shape[0])])
                 for i in range(sub_nodes.shape[0]):
                     sub_nodes[i].numb = sub_numbers[i]
                 self.nodes.update(dict(zip(sub_numbers, sub_nodes)))
                 node.set_edges(sub_numbers)
                 stack_nodes = np.append(stack_nodes, sub_numbers)
 
         if self.cut:
             self.cut_tree(X_val, cnt.CENS_NAME, mode_f=roc_auc_score, choose_f=max)
 
-        # self.fit_cox_hazard(X, y)
         return
 
-    # def fit_cox_hazard(self, X, y):
-    #     self.coxph = CoxPHSurvivalAnalysis(alpha=0.1)
-    #     self.ohenc = OneHotEncoder(handle_unknown='ignore')
-    #     pred_node = self.predict(X, mode="target", target="numb").reshape(-1, 1)
-    #     ohenc_node = self.ohenc.fit_transform(pred_node).toarray()
-    #     self.coxph.fit(ohenc_node, y)
-
-    # def predict_cox_hazard(self, X, bins):
-    #     bins = np.clip(bins, self.bins.min(), self.bins.max())
-    #     pred_node = self.predict(X, mode="target", target="numb").reshape(-1, 1)
-    #     ohenc_node = self.ohenc.transform(pred_node).toarray()
-    #     hazards = self.coxph.predict_cumulative_hazard_function(ohenc_node)
-    #     pred_haz = np.array(list(map(lambda x: x(bins), hazards)))
-    #     return pred_haz
-
     def predict(self, X, mode="target", target=cnt.TIME_NAME, end_list=[], bins=None):
         """
         Return values by mode & target
 
         Parameters
         ----------
         X : Pandas dataframe
@@ -257,14 +229,15 @@
         bins : array-like, optional
             Points of timeline
 
         Returns
         -------
         res : array-like
             Values by mode & target
+
         """
         X = format_to_pandas(X, self.features)
         num_node_to_key = dict(zip(sorted(self.nodes.keys()), range(len(self.nodes))))
         node_bin = np.zeros((X.shape[0], len(self.nodes)), dtype=bool)
         node_bin[:, 0] = 1
         shape = (X.shape[0])
         if not (bins is None):
@@ -275,16 +248,16 @@
             res = np.full(shape, np.nan, dtype=object)
         else:
             # res = np.full(shape, np.nan, dtype=float)
             res = np.empty(shape, dtype=float)
             res[:] = np.nan
         for i in sorted(self.nodes.keys()):
             ind = node_bin[:, num_node_to_key[i]]
-            X_loc = X[ind]
-            if ind.shape[0] > 0:
+            if np.any(ind):
+                X_loc = X[ind]
                 if self.nodes[i].is_leaf or (i in end_list):
                     if target == "surv" or target == "hazard":
                         res[ind] = self.nodes[i].predict(X_loc, target, bins)
                     elif mode == "target":
                         res[ind] = self.nodes[i].predict(X_loc, target)
                     elif mode == "rules":
                         res[ind] = self.nodes[i].get_full_rule()
@@ -304,26 +277,22 @@
             Contain input features of events.
         bins : array-like
             Points of timeline.
         mode : str, optional
             Type of function. The default is "surv".
             "surv" : send building function in nodes
             "hazard" : send building function in nodes
-            "cox-hazard" : fit CoxPH model on node numbers (input)
-                                          and time/cens (output)
-                       predict cumulative HF from model
 
         Returns
         -------
-        array-like
-            Vector of function values in times (bins).
+        res : array-like
+            Vector of function values in times (bins)
+
         """
         X = format_to_pandas(X, self.features)
-        # if mode == "cox-hazard":
-        #     return self.predict_cox_hazard(X, bins)
         pred = self.predict(X, target=mode, bins=bins)  # Reverse correction
         if self.balance == "balance+correct":
             if mode == "hazard":
                 pred = pred * self.correct_proba
             elif mode == "surv":
                 pred = pred ** self.correct_proba
         return pred
@@ -355,24 +324,22 @@
                             for n_l in np.unique(ret_leaf_numbers) if n_l != np.inf}
         dict_str_fill = {}
         for leaf_list in np.unique(ret_leaf_numbers, axis=0):
             end_leaf = leaf_list[leaf_list != np.inf]
             sch_list = np.vectorize(dict_leaf_scheme.get)(end_leaf)
             dict_str_fill[str(end_leaf)] = FilledSchemeStrategy(sch_list)
 
-        # res = np.array([str(x[x != np.inf]) for x in ret_leaf_numbers]), dtype=object)
-        # res = np.vectorize(dict_str_fill.get)(res)
         res = np.array(list(map(lambda leaf_list: dict_str_fill.get(str(leaf_list[leaf_list != np.inf]), np.nan),
                                 ret_leaf_numbers)), dtype=object)
         return res
 
     def cut_tree(self, X, target, mode_f=roc_auc_score, choose_f=max):
         """
         Method of pruning tree.
-        Find best subtree, which reaches best value of metric "mode_f""
+        Find the best subtree that achieves the best value of the "mode_f" metric".
 
         Parameters
         ----------
         X : Pandas dataframe
             Contain input features of events.
         target : str
             Feature name for metric counting.
@@ -392,15 +359,16 @@
         with tempfile.TemporaryDirectory() as tmp_dir:
             dot = Digraph(node_attr={'shape': 'none'})
             ordered_nodes = sorted(self.nodes.keys())
             for i in ordered_nodes:
                 dot = self.nodes[i].set_dot_node(dot, path_dir=tmp_dir, **kwargs)
             for i in ordered_nodes:
                 dot = self.nodes[i].set_dot_edges(dot)
-            dot.render(os.path.join(path_dir, self.name), view=False, cleanup=True, format="png")
+            dot.render(os.path.join(path_dir, self.name), cleanup=True, format="png")
+        return dot
 
     def translate(self, describe):
         self.features = [describe.get(f, f) for f in self.features]
         self.categ = [describe.get(c, c) for c in self.categ]
         for i in self.nodes.keys():
             self.nodes[i].translate(describe)
```

### Comparing `survivors-1.6.2/survivors/tree/find_split_hist.py` & `survivors-1.6.3/survivors/tree/find_split_hist.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 from numba import njit
 
-from scipy import stats
-# from .stratified_model import KaplanMeier, FullProbKM, NelsonAalen, KaplanMeierZeroAfter
+from ..criteria import chi2_sf
 from ..external import KaplanMeier, NelsonAalen, KaplanMeierZeroAfter, FullProbKM
 from ..metrics import ibs_WW, auprc
 from ..constants import get_y
+# from scipy.stats import chi2
 # import diptest
 
 """ Auxiliary functions """
 
 
 @njit('f4(f4[:], f4[:], f4[:], f4[:], u4, f4[:])', cache=True)
 def lr_hist_statistic(time_hist_1, time_hist_2, cens_hist_1, cens_hist_2,
@@ -68,15 +68,15 @@
 def weight_hist_stat(time_hist_1, time_hist_2, cens_hist_1=None, cens_hist_2=None, weights_hist=None, weightings=""):
     try:
         if cens_hist_1 is None:
             cens_hist_1 = time_hist_1
         if cens_hist_2 is None:
             cens_hist_2 = time_hist_2
         if weights_hist is None:
-            weights_hist = np.ones(time_hist_1.shape[0])
+            weights_hist = np.ones(time_hist_1.shape[0], dtype=np.float32)
         d = {"logrank": 1, "wilcoxon": 2, "tarone-ware": 3, "peto": 4, "weights": 5}
         d.update({"diff": 6, "maxcombo": 7, "symm_peto": 8})
         weightings = d.get(weightings, 1)
 
         logrank = lr_hist_statistic(time_hist_1.astype("float32"),
                                     time_hist_2.astype("float32"),
                                     cens_hist_1.astype("float32"),
@@ -134,45 +134,36 @@
 #                                         left_cens_hist, right_cens_hist,
 #                                         weights_hist, weightings=criterion)
 #     return (max_stat_val, none_to)
 
 
 def optimal_criter_split_hist(left_time_hist, left_cens_hist,
                               right_time_hist, right_cens_hist,
-                              na_time_hist, na_cens_hist, weights_hist, criterion, dis_coef,
-                              apr_t_distr, apr_e_distr, l_reg):
+                              na_time_hist, na_cens_hist, weights_hist, criterion, dis_coef):
     none_to = 0
-    max_stat_val = 1.0
-
     # n1 = np.sum(left_time_hist)
     # n2 = np.sum(right_time_hist)
     # cf = n1 / (n1 + n2)
-    cf = 0.5
+    # cf = 0.5
 
     if na_time_hist.shape[0] > 0:
-        a = weight_hist_stat(left_time_hist + na_time_hist + l_reg * apr_t_distr * cf,
-                             right_time_hist + l_reg * apr_t_distr * (1 - cf),
-                             left_cens_hist + na_cens_hist + l_reg * apr_e_distr * cf,
-                             right_cens_hist + l_reg * apr_e_distr * (1 - cf),
+        a = weight_hist_stat(left_time_hist + na_time_hist, right_time_hist,
+                             left_cens_hist + na_cens_hist, right_cens_hist,
                              weights_hist, weightings=criterion)
-        b = weight_hist_stat(left_time_hist + l_reg * apr_t_distr * cf,
-                             right_time_hist + na_time_hist + l_reg * apr_t_distr * (1 - cf),
-                             left_cens_hist + l_reg * apr_e_distr * cf,
-                             right_cens_hist + na_cens_hist + l_reg * apr_e_distr * (1 - cf),
+        b = weight_hist_stat(left_time_hist, right_time_hist + na_time_hist,
+                             left_cens_hist, right_cens_hist + na_cens_hist,
                              weights_hist, weightings=criterion)
         # Nans move to a leaf with maximal statistical value
         none_to = int(a < b)
         max_stat_val = max(a, b)
     else:
-        max_stat_val = weight_hist_stat(left_time_hist + l_reg * apr_t_distr * cf,
-                                        right_time_hist + l_reg * apr_t_distr * (1 - cf),
-                                        left_cens_hist + l_reg * apr_e_distr * cf,
-                                        right_cens_hist + l_reg * apr_e_distr * (1 - cf),
+        max_stat_val = weight_hist_stat(left_time_hist, right_time_hist,
+                                        left_cens_hist, right_cens_hist,
                                         weights_hist, weightings=criterion)
-    return (max_stat_val, none_to)
+    return max_stat_val, none_to
 
 
 def split_time_to_bins(time, event=None, apr_times=None, apr_events=None):
 #     if apr_times is None:
 #         return np.searchsorted(np.unique(time), time)
 #     return np.searchsorted(np.unique(apr_times), time)
     if apr_times is None:
@@ -187,14 +178,15 @@
 
 #     if apr_times is None:
 #         n = np.clip(time.shape[0] // 2, 2, 100)
 #         return np.searchsorted(np.quantile(time, np.arange(n + 1)/n), time)
 #     n = np.clip(apr_times.shape[0] // 2, 2, 100)
 #     return np.searchsorted(np.quantile(apr_times, np.arange(n + 1)/n), time)
 
+
 def get_attrs(max_stat_val, values, none_to, l_sh, r_sh, nan_sh, stat_diff):
     attrs = dict()
     attrs["stat_val"] = max_stat_val
     attrs["values"] = values
     attrs["stat_diff"] = stat_diff
     if none_to:
         attrs["pos_nan"] = [0, 1]
@@ -241,15 +233,15 @@
     return time_hist, cens_hist
 
 
 def select_best_split_info(attr_dicts, type_attr, bonf=True, descr_woe=None):
     # attr_dicts = sorted(attr_dicts, key=lambda x: abs(x["stat_diff"]), reverse=True)[:max(1, len(attr_dicts)//2)]
     best_attr = max(attr_dicts, key=lambda x: x["stat_val"])
 
-    best_attr["p_value"] = stats.chi2.sf(best_attr["stat_val"], df=1)
+    best_attr["p_value"] = chi2_sf(best_attr["stat_val"], df=1)
     best_attr["sign_split"] = len(attr_dicts)
     if best_attr["sign_split"] > 0:
         if type_attr == "cont":
             best_attr["values"] = [f" <= {best_attr['values']}", f" > {best_attr['values']}"]
         # elif type_attr == "categ":
         #     best_attr["values"] = [f" in {e}" for e in best_attr["values"]]
         elif type_attr == "woe" or type_attr == "categ":
@@ -313,14 +305,57 @@
     d2 = count_sf_diff(time_2, cens_2)
     return min(d1, d2)
 
 
 def hist_best_attr_split(arr, criterion="logrank", type_attr="cont", weights=None, thres_cont_bin_max=100,
                          signif=1.0, signif_stat=0.0, min_samples_leaf=10, bonf=True, verbose=0, balance=False,
                          apr_time=None, apr_event=None, l_reg=0, **kwargs):
+    """
+    Find best split of sample by one feature (histogram realization)
+
+    Parameters
+    ----------
+    arr: numpy ndarray
+        Triplet of two target variables and one splitting feature
+    criterion: str
+        Weighting scheme in log-rank test
+    type_attr: str
+        Type of feature
+        Mode :
+            "cont" -- linear search in continuous values
+            "categ" -- complete search of categorical variable combinations
+            "woe" -- Weight Of Evidence mapping categorical to continuous
+    weights: numpy ndarray
+        Custom weights of observation significance
+    thres_cont_bin_max: int
+        Number of intermediate points
+    signif: float
+        Upper bound of the significance of the partition (p-value)
+    signif_stat: float
+        Lower bound of the significance of the partition (stat value)
+    min_samples_leaf: int
+        Minimum allowed number of observations in a leaf
+    bonf: bool
+        Using bonferroni correction
+    verbose: int
+        Enable verbose output
+    balance: bool
+        Enable balancing in log-rank
+    apr_time: numpy ndarray
+        Source times for log-rank regularization
+    apr_event: numpy ndarray
+        Source event indicator for log-rank regularization
+    l_reg: float
+        Regularization coefficient
+    kwargs: dict
+        Additional parameters
+    Returns
+    -------
+    Dict with the best split of sample by feature
+    """
     best_attr = {"stat_val": signif_stat, "p_value": signif,
                  "sign_split": 0, "values": [], "pos_nan": [1, 0]}
     if arr.shape[1] < 2 * min_samples_leaf:
         return best_attr
     vals = arr[0].astype("float")
     cens = arr[1].astype("uint")
     dur = arr[2].astype("float")
@@ -341,19 +376,20 @@
 
     if apr_time is None:
         dur = split_time_to_bins(dur, cens)
         max_bin = dur.max()
         apr_t_distr = np.zeros(max_bin + 1)
         apr_e_distr = np.zeros(max_bin + 1)
     else:
-        # apr_time_1 = split_time_to_bins(apr_time, apr_time)
         apr_time_1 = split_time_to_bins(apr_time, apr_event, dur, cens)  # , apr_time)
         dur = split_time_to_bins(dur, cens)
         max_bin = apr_time_1.max()
         apr_t_distr, apr_e_distr = get_sa_hists(apr_time_1, apr_event, minlength=max_bin + 1)
+        apr_t_distr = apr_t_distr * l_reg * 0.5
+        apr_e_distr = apr_e_distr * l_reg * 0.5
 
     # dur = split_time_to_bins(dur)
     # max_bin = dur.max()
 
     ind = np.isnan(vals)
 
     # split nan and not-nan
@@ -438,14 +474,27 @@
         weights_hist = (dd - ET)  # **2
         criterion = "weights"
     elif criterion == "kde":
         na = NelsonAalen()
         na.fit(dur, cens, np.ones(len(dur)))
         weights_hist = na.get_smoothed_hazard_at_times(np.unique(dur))
         criterion = "weights"
+    elif criterion == "wilcoxon-pred":
+        if na_time_hist.shape[0] > 0:
+            weights_hist = np.cumsum((r_time_hist + na_time_hist)[::-1])[::-1]
+        else:
+            weights_hist = np.cumsum(r_time_hist[::-1])[::-1]
+        criterion = "weights"
+    elif criterion == "tarone-ware-pred":
+        if na_time_hist.shape[0] > 0:
+            weights_hist = np.sqrt(np.cumsum((r_time_hist + na_time_hist)[::-1])[::-1])
+        else:
+            weights_hist = np.sqrt(np.cumsum(r_time_hist[::-1])[::-1])
+        criterion = "weights"
+
     # elif weights is None:
     #     weights_hist = None
     # else:
     #     weights_hist = np.bincount(dur, weights=weights,  # /sum(weights),
     #                                minlength=max_bin + 1)
     #     weights_hist /= np.bincount(dur, minlength=max_bin + 1)  # np.sqrt()
         # weights_hist = np.cumsum(weights_hist[::-1])[::-1]  # np.sqrt()
@@ -466,21 +515,17 @@
         num_l += curr_n
         num_r -= curr_n
 
         if min(num_l, num_r) <= min_samples_leaf:
             continue
 
         max_stat_val, none_to = optimal_criter_split_hist(
-            l_time_hist, l_cens_hist, r_time_hist, r_cens_hist,
-            na_time_hist, na_cens_hist, weights_hist, criterion, dis_coef,
-            apr_t_distr, apr_e_distr, l_reg)
-
-        # max_stat_val, none_to = optimal_criter_split_hist(
-        #     l_time_hist, l_cens_hist, r_time_hist, r_cens_hist,
-        #     na_time_hist, na_cens_hist, weights_hist, criterion, dis_coef)
+            l_time_hist + apr_t_distr, l_cens_hist + apr_e_distr,
+            r_time_hist + apr_t_distr, r_cens_hist + apr_e_distr,
+            na_time_hist, na_cens_hist, weights_hist, criterion, dis_coef)
 
         if max_stat_val > signif_stat:
             stat_diff = 1
             # if na_time_hist.shape[0] > 0:
             #     stat_diff = stdtest_hist((l_time_hist + (1 - none_to) * na_time_hist),
             #                              (r_time_hist + none_to * na_time_hist))
             # else:
```

### Comparing `survivors-1.6.2/survivors/tree/node.py` & `survivors-1.6.3/survivors/tree/node.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,87 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 
 from joblib import Parallel, delayed
-from scipy import stats
+# from scipy.stats import chi2
+from ..criteria import chi2_isf
 
 from .find_split_hist import hist_best_attr_split
 from .. import constants as cnt
-# from .stratified_model import LEAF_MODEL_DICT, LeafModel
 from ..external import LEAF_MODEL_DICT, LeafModel
 from ..scheme import Scheme
 
-#sns.set()
 custom_params = {"axes.spines.right": False, 'grid.color': 'lightgray', 'axes.grid': True, "axes.spines.top": False}
 sns.set_theme(style="ticks", rc=custom_params)
 # custom_params = {"font.size": 25, "axes.labelsize": 25, "xtick.labelsize": 25, "ytick.labelsize": 25,
 #                  "axes.spines.right": False, 'grid.color': 'lightgray', 'axes.grid': True, "axes.spines.top": False}
-# sns.set_theme(style="ticks", rc=custom_params)
 
-"""" Auxiliary functions """
+""" Auxiliary functions """
 
 
-def join_dict(a, b):
-    return dict(list(a.items()) + list(b.items()))
+class Rule(object):
+    """
+    Node of decision tree.
+    Allow to separate data into 2 child nodes
 
+    Attributes
+    ----------
+    feature : str
+        Name of feature for splitting
+    condition : str
+        Operation for splitting
+    has_nan : bool
+        Flag of the missing values in node
 
-class Rule(object):
+    Methods
+    -------
+    get_feature : Return feature
+    get_condition : Return condition
+    translate: Replace rule by dictionary
+    to_str : Transforming to linear form
+    print : Print all attributes and descriptions
+
+    """
     def __init__(self, feature: str, condition: str, has_nan: int):
         self.feature = feature
         self.condition = condition
         self.has_nan_ = has_nan
 
     def get_feature(self):
         return self.feature
 
     def get_condition(self):
         return self.condition
 
     def has_nan(self):
         return self.has_nan_
 
-    def translate(self, describe):
+    def translate(self, describe: dict):
+        """
+        Rename feature in rule
+        """
         self.feature = describe.get(self.feature, self.feature)
 
     def to_str(self):
         s = f"({self.feature}{self.condition})"
         if self.has_nan_:
-            s = f"({s}| nan)"  # не указано)"
+            s = f"({s}| nan)"
         return s
 
     def print(self):
+        """
+        Print all attributes and descriptions
+        """
         print(f"has_nan: {self.has_nan()}")
         print(f"feature: {self.get_feature()}")
         print(f"condition: {self.get_condition()}")
 
 
-""" Класс вершины дерева решений """
 class Node(object):
-    # __slots__ = ("df", "numb", "full_rule",
-    #              "depth", "edges", "rule_edges", "features", "leaf_model",
-    #              "categ", "woe", "is_leaf", "verbose", "info")
     """
     Node of decision tree.
     Allow to separate data into 2 child nodes
 
     Attributes
     ----------
     df : Pandas DataFrame
@@ -81,29 +99,29 @@
     features : list
         Available features
     categ : list
         Names of categorical features
     woe : boolean
         Mode of categorical preparation
     is_leaf : boolean
-        True if node has no subnodes
+        True if node is terminal (there are no child nodes)
     verbose : int
         Print the best split of the node
     info : dict
         Parameters for finding the best splitting
     leaf_model : LeafModel
         Stratified model by parameter <<leaf_model>> (map with LEAF_MODEL_DICT)
 
     Methods
     -------
     check_params : Fill empty parameters and map max_features to int
     find_best_split : Choose best split of node according to parameters
-    split : Try to create subnodes by best split
+    split : Find best split of df sample and create child nodes
     set_edges: Set number of child nodes from hash table of main tree
-    set_leaf : Delete subnodes and reset data
+    set_leaf : Delete child nodes and set node as terminal
 
     predict : Return statistic values of a data
     predict_scheme : Return all possible outcomes for additional features determination
 
     prepare_df_for_attr : set input values to numpy format (and fill missing features)
     get_edges : defines appropriate child nodes according to input values
     get_full_rule : convert full_rules to a string format
@@ -132,25 +150,24 @@
         self.is_leaf = True
         self.verbose = verbose
         self.info = info
         self.check_params()
 
     def check_params(self):
         self.info.setdefault("bonf", True)
-        self.info.setdefault("n_jobs", 16)
         self.info.setdefault("max_features", 1.0)
         self.info.setdefault("signif", 1.1)
-        self.info.setdefault("signif_stat", stats.chi2.isf(min(self.info["signif"], 1.0), df=1))
+        self.info.setdefault("signif_stat", chi2_isf(min(self.info["signif"], 1.0), df=1))
         self.info.setdefault("thres_cont_bin_max", 100)
         self.info.setdefault("normalize", True)
 
         if self.info["max_features"] == "sqrt":
             self.info["max_features"] = int(np.trunc(np.sqrt(len(self.features))+0.5))
         elif isinstance(self.info["max_features"], float):
-            self.info["max_features"] = int(self.info["max_features"]*len(self.features))
+            self.info["max_features"] = int(self.info["max_features"] * len(self.features))
 
         self.info.setdefault("weights_feature", None)
         if not (self.info["weights_feature"] is None):
             self.info["weights"] = self.df[self.info["weights_feature"]].to_numpy()
 
         leaf_kwargs = {k[5:]: v for k, v in self.info.items() if (k.find("leaf_") != -1) and (k != "leaf_model")}
         self.info.setdefault("leaf_model", "base_zero_after")  # base
@@ -160,90 +177,92 @@
             self.leaf_model = self.info["leaf_model"](**leaf_kwargs)
             if not (isinstance(self.leaf_model, LeafModel)):
                 self.leaf_model = None
         else:
             self.leaf_model = None
         self.size = self.df.shape[0]
 
-        self.leaf_model.fit(self.df)  # , self.info["normalize"])
+        self.leaf_model.fit(self.df)
         # self.ch = np.array(
         #     [np.mean(self.df["time"]), np.std(self.df["time"]), np.sum(self.df["cens"]) / self.df["cens"].shape[0]])
 
     """ GROUP FUNCTIONS: CREATE LEAVES """
     def get_comb_fast(self, features):
-        X = self.df[features + [cnt.CENS_NAME, cnt.TIME_NAME]].to_numpy().T
+        """
+        Create set of all triplets with two target variables and one splitting feature
+        """
+        d_df = dict(zip(self.df.columns, self.df.values.T))
 
-        def create_params_f(v_feature, name):
+        def create_params_f(name):
             d = self.info.copy()
-            d["arr"] = np.vstack((v_feature, X[-2:]))
+            d["arr"] = np.vstack((d_df[name], d_df[cnt.CENS_NAME], d_df[cnt.TIME_NAME]))
             d["type_attr"] = ("woe" if self.woe else "categ") if name in self.categ else "cont"
             return d
 
-        return list(map(create_params_f, X[:-2], features))
-
-    def get_comb(self, features):
-        args = np.array([], dtype=dict)
-        for feat in features:
-            t = self.info.copy()
-            t["type_attr"] = ("woe" if self.woe else "categ") if feat in self.categ else "cont"
-            t["arr"] = self.df.loc[:, [feat, cnt.CENS_NAME, cnt.TIME_NAME]].to_numpy().T
-            args = np.append(args, t)
-        return args
+        return list(map(create_params_f, features))
 
     def find_best_split(self):
+        """
+        Sort through all combinations of splitting the sample by features.
+        Find a split with the highest statistical value.
+        """
         numb_feats = self.info["max_features"]
         numb_feats = np.clip(numb_feats, 1, len(self.features))
-        n_jobs = min(numb_feats, self.info["n_jobs"])
+        n_jobs = self.info.get("n_jobs", 1 if numb_feats < 20 else 5)
 
         selected_feats = list(np.random.choice(self.features, size=numb_feats, replace=False))
-        # args = self.get_comb(selected_feats)
-        args = self.get_comb_fast(selected_feats)
 
+        args = self.get_comb_fast(selected_feats)
         # ml = np.vectorize(lambda x: hist_best_attr_split(**x))(args)
-        with Parallel(n_jobs=n_jobs, verbose=self.verbose, batch_size=10) as parallel:  # prefer="threads"
-           ml = parallel(delayed(hist_best_attr_split)(**a) for a in args)
-        # with Parallel(n_jobs=1, verbose=self.verbose) as parallel:  # prefer="threads"
-        #     ml = parallel(delayed(hist_best_attr_split)(**a) for a in args)  # hist_best_attr_split
+        with Parallel(n_jobs=n_jobs, verbose=self.verbose) as parallel:
+            ml = parallel(delayed(hist_best_attr_split)(**a) for a in args)
+
         attrs = {f: ml[ind] for ind, f in enumerate(selected_feats)}
 
-        # attr = min(attrs, key=lambda x: attrs[x]["p_value"])  # simple p-value
-        attr = max(attrs, key=lambda x: attrs[x]["stat_val"])  # simple stat-val
+        # attr = min(attrs, key=lambda x: attrs[x]["p_value"])  # best by p-value
+        attr = max(attrs, key=lambda x: attrs[x]["stat_val"])  # best by stat-val
         # attrs_gr = dict(filter(lambda x: x[1]["sign_split"] > 0, attrs.items()))
         # if len(attrs_gr) == 0:
         #     attr = min(attrs, key=lambda x: attrs[x]["p_value"])
         # else:
         #     attr = min(attrs_gr, key=lambda x: attrs_gr[x]["p_value"])
         #     if self.info["bonf"]:
         #         attrs[attr]["p_value"] = attrs[attr]["p_value"] / attrs[attr]["sign_split"]
 
         # if attrs[attr]["sign_split"] > 0 and self.info["bonf"]:  # suffix for simple p-value
         #     attrs[attr]["p_value"] = attrs[attr]["p_value"] / attrs[attr]["sign_split"]
         return (attr, attrs[attr])
 
     def ind_for_nodes(self, X_attr, best_split, is_categ):
+        """
+        Map the number of the according child node by rule and sample features.
+        """
         rule_id = best_split["pos_nan"].index(0)
         query = best_split["values"][rule_id]
         if is_categ:
             values = np.isin(X_attr, eval(query[query.find("["):]))
         else:
             values = eval("X_attr" + query)
         return np.where(values, rule_id, 1 - rule_id)
 
     def split(self):
+        """
+        Find best split of df sample and create child nodes
+        """
         node_edges = np.array([], dtype=int)
         self.rule_edges = np.array([], dtype=Rule)
 
         attr, best_split = self.find_best_split()
         # The best split is not significant
         if best_split["sign_split"] == 0:
             if self.verbose > 0:
-                print(f'Конец ветви, незначащее p-value: {best_split["stat_val"]}')
+                print(f'The node is terminal, best p-value: {best_split["stat_val"]}')
             return node_edges
         if self.verbose > 0:
-            print('='*6, best_split["stat_val"], attr)
+            print('='*self.depth, best_split["stat_val"], attr)
 
         branch_ind = self.ind_for_nodes(self.df[attr], best_split, attr in self.categ)
 
         for n_b in np.unique(branch_ind):
             rule = Rule(feature=attr,
                         condition=best_split["values"][n_b],
                         has_nan=best_split["pos_nan"][n_b])
@@ -254,38 +273,25 @@
             node_edges = np.append(node_edges, N)
             self.rule_edges = np.append(self.rule_edges, rule)
 
         if self.rule_edges.shape[0] == 1:
             print(branch_ind, self.df[attr], best_split, attr in self.categ)
             raise ValueError('ERROR: Only one branch created!')
 
-        # for v, p_n in zip(best_split["values"], best_split["pos_nan"]):
-        #     query = attr + v
-        #     if p_n == 1:
-        #         query = "(" + attr + v + ") or (" + attr + " != " + attr + ")"
-        #     rule = Rule(feature=attr, condition=v, has_nan=p_n)
-        #     d_node = self.df.query(query).copy()
-        #     N = Node(df=d_node, full_rule=self.full_rule + [rule],
-        #              features=self.features, categ=self.categ,
-        #              depth=self.depth+1, verbose=self.verbose, **self.info)
-        #     node_edges = np.append(node_edges, N)
-        #     self.rule_edges = np.append(self.rule_edges, rule)
-
+        self.df = None
         return node_edges
 
     def set_edges(self, edges):
         self.edges = edges
         self.is_leaf = False
-        self.df = None
 
     def set_leaf(self):
-        if self.is_leaf:
-            return
         self.edges = np.array([], dtype=int)
         self.is_leaf = True
+        self.df = None
 
     def prepare_df_for_attr(self, X):
         attr = self.rule_edges[0].get_feature()
         if attr not in X.columns:
             X.loc[:, attr] = np.nan
         return X[attr].to_numpy()
 
@@ -310,38 +316,37 @@
         Parameters
         ----------
         X : Pandas dataframe
             Contain input features of events
         target : str or function
             Column name, mode or aggregate function of a leaf sample
             Column name : must be in dataset.columns
-                Return mean of feature
+            - Return mean of feature
             Mode :
-                "surv" return survival function
-                "hazard" return cumulative hazard function
-                attribute_name return attribute value (e.g. depth, numb)
-                feature_name return aggregate statistic value for node
+            - "surv" return survival function
+            - "hazard" return cumulative hazard function
+            - attribute_name return attribute value (e.g. depth, numb)
+            - feature_name return aggregate statistic value for node
         bins : array-like
             Points of timeline
 
         Returns
         -------
         res : array-like
             Values by target
-
         """
         if target == "surv":
-            return self.leaf_model.predict_survival_at_times(X, bins)  # target(X_node=dataset)
+            return self.leaf_model.predict_survival_at_times(X, bins)
         elif target == "hazard":
             return self.leaf_model.predict_hazard_at_times(X, bins)
-        elif target == "ch":
-            return np.repeat(self.ch[np.newaxis, :], X.shape[0], axis=0)
+        # elif target == "ch":
+        #     return np.repeat(self.ch[np.newaxis, :], X.shape[0], axis=0)
         elif target in self.__dict__:
             return np.repeat(getattr(self, target, np.nan), X.shape[0], axis=0)
-        return self.leaf_model.predict_feature(X, target)  # np.mean(dataset[target])
+        return self.leaf_model.predict_feature(X, target)
 
     def predict_scheme(self, X, scheme_feats):
         feat_means = np.array([self.leaf_model.features_predict.get(s_f, np.nan)
                                for s_f in scheme_feats])
         times = self.leaf_model.predict_list_feature(cnt.TIME_NAME)
         cens = self.leaf_model.predict_list_feature(cnt.CENS_NAME)
 
@@ -398,13 +403,11 @@
         if not self.is_leaf:
             for e in range(len(self.rule_edges)):
                 s = self.rule_edges[e].to_str()
                 dot.edge(str(self.numb), str(self.edges[e]), label=s, fontsize='30')
         return dot
 
     def translate(self, describe):
-        if self.is_leaf:
-            self.df = self.df.rename(describe, axis=1)
         self.features = [describe.get(f, f) for f in self.features]
         self.categ = [describe.get(c, c) for c in self.categ]
         for e in range(len(self.rule_edges)):
             self.rule_edges[e].translate(describe)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `survivors-1.6.2/survivors/visualize/comparison.py` & `survivors-1.6.3/survivors/visualize/comparison.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 import numpy as np
 
 custom_params = {"axes.spines.right": False, 'grid.color': 'lightgray', 'axes.grid': True, "axes.spines.top": False}
 sns.set_theme(style="ticks", rc=custom_params)
 
 
 def plot_func_comparison(y_true, y_preds, labels):
+    """
+    Plot multiple functions by method
+
+    Parameters
+    ----------
+    y_true: structured np.ndarray with shape=(n, 2)
+    y_preds: list of np.ndarray with shape=(n, n_bins)
+    labels: list of str
+
+    """
     linestyle = ('solid' if y_true["cens"] else 'dashed')
     fig, ax = plt.subplots(figsize=(8, 5))
 
     for y_pred, label in zip(y_preds, labels):
         ax.plot(y_pred, label=label)
     ax.hlines(1.0, 0, y_true["time"], color='r', linestyle=linestyle)
     ax.hlines(0.0, y_true["time"], len(y_preds[0]), color='r', linestyle=linestyle)
@@ -23,14 +33,26 @@
     plt.title(f'Prediction for {"terminal" if y_true["cens"] else "censured"} event with time={y_true["time"]}')
     plt.xlabel('Time')
     plt.ylabel('Survival probability')
     plt.show()
 
 
 def plot_metric_comparison(y_true, y_preds, labels, bins, metric):
+    """
+    Comparison quality metric in time
+
+    Parameters
+    ----------
+    y_true: structured np.ndarray with shape=(n, 2)
+    y_preds: list of np.ndarray with shape=(n, n_bins)
+    labels: list of str
+    bins: np.ndarray with shape=(n_bins)
+    metric: function of internal metric
+
+    """
     fig, ax = plt.subplots()
     m_name = metric.__name__
 
     for y_pred, label in zip(y_preds, labels):
         m_by_time = metric(y_true[np.newaxis], y_true[np.newaxis], y_pred[np.newaxis], bins, axis=1)
         m_val = metric(y_true[np.newaxis], y_true[np.newaxis], y_pred[np.newaxis], bins, axis=-1)
         ax.plot(m_by_time, label=f"{label} ({m_name}={m_val:.3f})")
```

### Comparing `survivors-1.6.2/survivors.egg-info/PKG-INFO` & `survivors-1.6.3/survivors.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,152 +1,137 @@
 Metadata-Version: 2.1
 Name: survivors
-Version: 1.6.2
+Version: 1.6.3
 Summary: UNKNOWN
 Author: Iulii Vasilev
 Author-email: iuliivasilev@gmail.com
-License: UNKNOWN
+License: BSD 3-Clause License
 Keywords: survival analysis,time-to-event,event data,machine learning
 Platform: UNKNOWN
 Requires-Python: >=3.10
 License-File: LICENSE
 
-|License| |PyPi|_ |DOI|_
+.. -*- mode: rst -*-
 
-===============
+|Price| |License| |PyPi|_ |DOI|_
+
+.. |Price| image:: https://img.shields.io/badge/price-FREE-0098f7.svg
+   :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+
+.. |PyPi| image:: https://img.shields.io/pypi/v/survivors
+.. _PyPi: https://pypi.org/project/survivors/
+
+.. |License| image:: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg
+   :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+
+.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10649986.svg
+.. _DOI: https://zenodo.org/doi/10.5281/zenodo.10649777
+
+=========
 survivors
-===============
+=========
+
+Event analysis has many applications: healthcare, hardware, social science, bioinformatics, and more.вЂЁSurvival analysis allows you to predict not only the time and probability of an event but also how the probability of that event changes over time.
+In particular, there are three functions: the survival function *S(t)*, the density function *f(t)*, and the hazard function *h(t)*:
+
+.. math::
+    S(t)=P(T>t), f(t)=P(T=t), h(t)=P(T=t|T>=t)
 
-`survivors <https://pypi.org/project/survivors/>`_ is a Python library for **survival analysis**.
+The open-source **survivors** library aims to fit accurate data-sensitive tree-based models. 
+These models handle categorical features and deal with missing values,overcoming the limitations of existing `lifelines <https://github.com/lifelines/lifelines?ysclid=lta0m13i2b832399887>`_, `scikit-survival <https://github.com/sebp/scikit-survival>`_, and `pycox <https://github.com/havakv/pycox>`_ models.
+Survivors is a platform for conducting experimental research. The experiment module is compatible with scikit-survival and lifelines models (non-parametric and parametric models have already been embedded into the library).
 
-It allows for building survival models: Survival Tree, Bagging ensemble, Adaptive Boosting ensemble.
+Developed models published in scientific articles [1]_, [2]_, [3]_ and outperformed existing models in terms of accuracy based on open medical data. We invite survival analysis researchers to join the development of survivors, using the library for their projects, reporting any problems, and creating new solutions.
+Documentation is available on https://iuliivasilev.github.io/dev-survivors/
 
-=======================
-About Survival Analysis
-=======================
+Principles
+-----------
 
-The objective in `survival analysis`_ (also referred to as time-to-event or reliability analysis)
-is to establish a connection between covariates and the time of an event.
+Built-in **survivors** models were developed as part of a PhD thesis at Lomonosov Moscow State University. The goal of the library is to analyze existing methods of survival analysis and develop new techniques to overcome these limitations.
 
-Survival analysis is a set of statistical models and methods used for estimating time until the occurrence of an event (or the probability that an event has not occurred). These methods are widely used in demography, e.g. for estimating lifespan or age at the first childbirth, in healthcare, e.g. for estimating the duration of staying in a hospital or survival time after the diagnosis of a disease, in engineering (for reliability analysis), in insurance, economics, and social sciences.
+Existing methods are not suitable for real-world data. Discrete methods use a fixed time scale. Statistical methods are based on strong assumptions, and tree-based methods use the log-rank statistic with low sensitivity.
+**Survivors** has the following features:
 
-Statistical methods need data, but complete data may not be available, i.e. the exact time of the event may be unknown for certain reasons  (the event did not occur before the end of the study or it is unknown whether it occurred). In this case, events are called censored. The data are censored from below (left-censored) when below a given value the exact values of observations are unknown. Right censored data (censored from above) does not have exact observations above a given value. Further in this paper, right censoring is considered.
+1. Continuous Predictions: The timeline is user-friendly and only needs to be set at the prediction stage.
+2. Modified Quality Metrics: Existing metrics are excessively sensitive to data features, such as class imbalance, event distribution, and timeline.
+3. Weighted Survival Tree. For the first time, CRAID uses weighted log-rank criteria. Wilcoxon, Peto, and Tarone-Ware weights increase the significance of events within a certain time interval.
+4. Speed of work. The models are developed from scratch and utilize parallelization, vectorization, and JIT compilation. A new histogram-based method is employed to identify splits in censored data. This method optimizes memory usage and has a high level of operation speed.
+5. Ease of Use. CRAID and ensembles work out-of-the-box. Categorical and missing data are processed within the models.
+6. A Platform for Experiments. The experiments module provides a flexible interface for working with built-in and external survival models, their hyperparameters, and experiment strategies, such as hold-out, cross-validation, grid search with cross-validation and sampling, and time-aware cross-validation.
+
+Installation
+------------
 
-============
 Requirements
-============
+~~~~~~~~~~~~
 
-- Python 3.9 or later
-- joblib
-- pickle-mixin
-- numpy >= 1.22
-- numba >= 0.58.0
-- matplotlib >= 3.5.0
+- Python (>= 3.9)
+- NumPy (>= 1.22)
+- Pandas (>=0.25)
+- Numba (>= 0.58.0)
+- matplotlib (>= 3.5.0)
 - seaborn
-- graphviz >= 2.50.0
-- pandas >=0.25
-- scipy
-- python-dateutil
-- scikit-learn >= 1.0.2
-- lifelines >= 0.27.8
-- scikit-survival >= 0.17.2
+- graphviz (>= 2.50.0)
+- joblib
+- scikit-learn (>= 1.0.2)
 - openpyxl
 
-============
-Installation
-============
+Optional for comprehensive experiments:
 
-The easiest way to install survivors is to use by running::
+- lifelines (>= 0.27.8)
+- scikit-survival (>= 0.17.2)
 
-  pip install survivors
+User Installation
+~~~~~~~~~~~~~~~~~
 
-========
-Examples
-========
+The most convenient and fastest way to install a package is to directly download the library from the Python package catalog (Python Package Index, PyPI).
+The version of the source files in the directory is up-to-date and consistent with the GitHub repository::
 
-The user guides at *doc* and *demonstration* directories provide in-depth information on the key concepts of survivors, an overview of available survival models,
-and hands-on examples in the form of `Jupyter notebooks <https://jupyter.org/>`_.
+  pip install survivors
 
-There are examples of using the library with Jupyter Notebook.
-The example is a variant of solving a multi-stage problem:
+An alternative installation method is based on the use of source files. 
+The first step is to download the source files using Github::
 
-1. Import the library
-2. Loading and preparing data
-3. Model training
-4. Getting a forecast
-5. Visualization of the constructed model
-6. Visualization of true and predicted survival functions
+  git clone command https://github.com/iuliivasilev/dev-survivors.git
 
-==========
-Scenarios
-==========
+Or getting and unpacking the archive of `the latest published version <https://github.com/iuliivasilev/dev-survivors/releases/>`_. Next, use the command line to go to the **dev-survivors** directory. Finally, the manual installation of the library is completed after executing the following command::
 
-The library allows to carry out the following work scenarios:
+  python command setup.py install
 
-1. Collecting data from patient medical histories (hospital tests, medications, treatment) from various medical institutions. The medical history can be presented as a set of tables in csv or xlsx format, or as a hierarchical structure of xml files.
 
-2. Building survival analysis models. There are available the following models: a decision tree, a bagging ensemble, and a boosting ensemble. For each model, there is a wide range of hyperparameters, which provide the flexibility of the model.
+Examples
+------------
 
-3. Predicting the probability and time of the event. Forecasts can be used by the user to solve the problem of classifying or ranking new patients according to the expected severity of the disease.
+The user guides in the *doc* and *demonstration* directories provide detailed information on the key concepts for **survivors**. 
+They also include hands-on examples in the form of `Jupyter notebooks <https://jupyter.org/>`_.
+In particular, the library allows users to carry out a range of scenarios.
+
+1. Loading and preparing 9 open medical datasets: GBSG, PBC, SMARTO, SUPPORT2, WUHAN, ACTG, FLCHAIN, ROTT2, FRAMINGHAM.
+2. Fitting Survival Analysis Models: There are the following models available: a Decision Tree (CRAID), a Bootstrap Ensemble (BootstrapCRAID), and an Adaptive Boosting Ensemble (BoostingCRAID). Each model has a wide range of hyperparameters, providing flexibility for the model.
+3. Predict the probability and timing of the event. Forecasts can help users solve the problem of classifying or ranking new patients based on the expected severity of their disease. 
+4. Predict the individual survival functions and cumulative hazards of patients. Forecasts can be used to support medical decisions and adjust treatments.
+5. Visualizing and interpreting dependencies in data.
 
-4. Predicting the individual survival functions and cumulative hazard of patients. Forecasts can be used to support medical decisions and adjust treatment.
+Help and Support
+----------------
 
-==============
 Communication
-==============
+~~~~~~~~~~~~~
 
-- Mail: iuliivasilev@gmail.com
+- Email: iuliivasilev@gmail.com
 - LinkedIn: https://www.linkedin.com/in/iulii-vasilev
 
-==========
-References
-==========
-
-Please cite the following paper if you are using **survivors**.
-
-    Vasilev I., Petrovskiy M., Mashechkin I. Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria. - 2022.
-
-    Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Sensitivity of Survival Analysis Metrics." Mathematics 11.20 (2023): 4246.
-
-    Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting." International Conference on Pattern Recognition Applications and Methods. Cham: Springer International Publishing, 2021.
-
-.. code::
-
-    @inproceedings{vasilev2022survival,
-        title={Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria.},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor V},
-        booktitle={ICPRAM},
-        pages={132--140},
-        year={2022}
-    }
-
-    @inproceedings{vasilev2023adaptive,
-        title={Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor},
-        booktitle={Pattern Recognition Applications and Methods: 10th International Conference, ICPRAM 2021, and 11th International Conference, ICPRAM 2022, Virtual Event, February 4--6, 2021 and February 3--5, 2022, Revised Selected Papers},
-        pages={98--115},
-        year={2023},
-        organization={Springer}
-    }
-
-    @article{vasilev2023sensitivity,
-        title={Sensitivity of Survival Analysis Metrics},
-        author={Vasilev, Iulii and Petrovskiy, Mikhail and Mashechkin, Igor},
-        journal={Mathematics},
-        volume={11},
-        number={20},
-        pages={4246},
-        year={2023},
-        publisher={MDPI}
-    }
 
-.. _survival analysis: https://en.wikipedia.org/wiki/Survival_analysis
+Citation
+~~~~~~~~~~
 
-.. |PyPi| image:: https://img.shields.io/pypi/v/survivors
-.. _PyPi: https://pypi.org/project/survivors/
+If you use **survivors** in a scientific publication, we would appreciate citations:
 
-.. |License| image:: https://img.shields.io/badge/license-BSD%203--Clause-blue.svg
-  :target: https://github.com/iuliivasilev/dev-survivors/blob/master/LICENSE
+.. [1] Vasilev I., Petrovskiy M., Mashechkin I. Survival Analysis Algorithms based on Decision Trees with Weighted Log-rank Criteria. - 2022.
+
+.. [2] Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Sensitivity of Survival Analysis Metrics." Mathematics 11.20 (2023): 4246.
+
+.. [3] Vasilev, Iulii, Mikhail Petrovskiy, and Igor Mashechkin. "Adaptive Sampling for Weighted Log-Rank Survival Trees Boosting." International Conference on Pattern Recognition Applications and Methods. Cham: Springer International Publishing, 2021.
+
+.. _survival analysis: https://en.wikipedia.org/wiki/Survival_analysis
 
-.. |DOI| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.10649986.svg
-.. _DOI: https://zenodo.org/doi/10.5281/zenodo.10649777
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `survivors-1.6.2/survivors.egg-info/SOURCES.txt` & `survivors-1.6.3/survivors.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.py
+requirements/docs-requirements.txt
 requirements/requirements.txt
 survivors/__init__.py
 survivors/constants.py
 survivors/criteria.py
 survivors/metrics.py
 survivors.egg-info/PKG-INFO
 survivors.egg-info/SOURCES.txt
 survivors.egg-info/dependency_links.txt
 survivors.egg-info/requires.txt
 survivors.egg-info/top_level.txt
 survivors/datasets/__init__.py
 survivors/datasets/backblaze.py
 survivors/datasets/covid.py
+survivors/datasets/new_backblaze.py
 survivors/datasets/onk.py
 survivors/datasets/other.py
 survivors/datasets/data/Framingham.csv
 survivors/datasets/data/GBSG.csv
 survivors/datasets/data/__init__.py
 survivors/datasets/data/actg.csv
 survivors/datasets/data/covid_train.xlsx
 survivors/datasets/data/flchain.csv
 survivors/datasets/data/pbc.csv
 survivors/datasets/data/rott2.csv
 survivors/datasets/data/smarto.csv
 survivors/datasets/data/support2.csv
+survivors/datasets/data/BACKBLAZE/__init__.py
 survivors/datasets/data/COVID/__init__.py
 survivors/datasets/data/ONK/__init__.py
 survivors/ensemble/__init__.py
 survivors/ensemble/base_ensemble.py
 survivors/ensemble/base_ensemble_iter.py
 survivors/ensemble/boosting.py
 survivors/ensemble/bootstrap.py
@@ -46,20 +49,12 @@
 survivors/external/leaf_model.py
 survivors/external/nonparametric.py
 survivors/external/parametric.py
 survivors/scheme/__init__.py
 survivors/scheme/scheme.py
 survivors/tree/__init__.py
 survivors/tree/decision_tree.py
-survivors/tree/find_split(p-value).py
-survivors/tree/find_split.py
 survivors/tree/find_split_hist.py
-survivors/tree/find_split_hist_int.py
 survivors/tree/node.py
-survivors/tree/stratified_model.py
-survivors/tree_pandas/__init__.py
-survivors/tree_pandas/decision_tree.py
-survivors/tree_pandas/find_split.py
-survivors/tree_pandas/node.py
 survivors/visualize/__init__.py
 survivors/visualize/base.py
 survivors/visualize/comparison.py
```

