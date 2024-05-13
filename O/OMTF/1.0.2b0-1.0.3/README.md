# Comparing `tmp/omtf-1.0.2b0.tar.gz` & `tmp/omtf-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omtf-1.0.2b0.tar", last modified: Mon May 13 14:37:21 2024, max compression
+gzip compressed data, was "omtf-1.0.3.tar", last modified: Mon May 13 14:54:39 2024, max compression
```

## Comparing `omtf-1.0.2b0.tar` & `omtf-1.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.234284 omtf-1.0.2b0/
--rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.2b0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.137284 omtf-1.0.2b0/OMTF/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.189285 omtf-1.0.2b0/OMTF/Brokers/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.2b0/OMTF/Brokers/__init__.py
--rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.2b0/OMTF/Brokers/binance_broker.py
--rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.2b0/OMTF/Brokers/degiro.py
--rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.2b0/OMTF/Brokers/metatrader.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.206284 omtf-1.0.2b0/OMTF/DataProviders/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.2b0/OMTF/DataProviders/__init__.py
--rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.2b0/OMTF/DataProviders/aemet.py
--rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.2b0/OMTF/DataProviders/benzinga.py
--rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.2b0/OMTF/DataProviders/coingecko.py
--rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.2b0/OMTF/DataProviders/coinmarketcap.py
--rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.2b0/OMTF/DataProviders/data.py
--rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.2b0/OMTF/DataProviders/dilutionTracker.py
--rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.2b0/OMTF/DataProviders/expansion.py
--rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.2b0/OMTF/DataProviders/finviz.py
--rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.2b0/OMTF/DataProviders/floatChecker.py
--rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.2b0/OMTF/DataProviders/fmp.py
--rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.2b0/OMTF/DataProviders/fxstreet.py
--rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.2b0/OMTF/DataProviders/geonames.py
--rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.2b0/OMTF/DataProviders/inversis_todo.py
--rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.2b0/OMTF/DataProviders/marketWatch.py
--rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.2b0/OMTF/DataProviders/oecd.py
--rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.2b0/OMTF/DataProviders/openstreetmap.py
--rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.2b0/OMTF/DataProviders/polygon.py
--rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.2b0/OMTF/DataProviders/sec.py
--rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.2b0/OMTF/DataProviders/tradingterminal.py
--rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.2b0/OMTF/DataProviders/worldBank.py
--rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.2b0/OMTF/DataProviders/worldHealthOrg.py
--rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.2b0/OMTF/DataProviders/world_population.py
--rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.2b0/OMTF/DataProviders/yahoo.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.220285 omtf-1.0.2b0/OMTF/MachineLearning/
--rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.2b0/OMTF/MachineLearning/00_models_comparison.py
--rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.2b0/OMTF/MachineLearning/RandomForest.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.2b0/OMTF/MachineLearning/__init__.py
--rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.2b0/OMTF/MachineLearning/decision_trees.py
--rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/genetic_algorithm.py
--rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/gradientboosting.py
--rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/k_nearest_neighbors.py
--rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.2b0/OMTF/MachineLearning/kmeans_clustering.py
--rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.2b0/OMTF/MachineLearning/linear_regression.py
--rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.2b0/OMTF/MachineLearning/logistic_regression.py
--rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/long_short_term_memory.py
--rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.2b0/OMTF/MachineLearning/naive_bayes.py
--rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.2b0/OMTF/MachineLearning/neural_networks.py
--rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.2b0/OMTF/MachineLearning/principal_component.py
--rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.2b0/OMTF/MachineLearning/random_forest.py
--rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/recurrent_neural_networks.py
--rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.2b0/OMTF/MachineLearning/support_vector.py
--rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.2b0/OMTF/MachineLearning/utils.py
--rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/xgboost_model.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.231285 omtf-1.0.2b0/OMTF/Trading/
--rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/Trading/KEYS.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.2b0/OMTF/Trading/__init__.py
--rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.2b0/OMTF/Trading/asset_tradeablitiy.py
--rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.2b0/OMTF/Trading/backtest.py
--rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.2b0/OMTF/Trading/backtest_utils.py
--rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.2b0/OMTF/Trading/config.py
--rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.2b0/OMTF/Trading/continuous_backtest.py
--rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.2b0/OMTF/Trading/discrete_backtest.py
--rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.2b0/OMTF/Trading/execution.py
--rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.2b0/OMTF/Trading/execution_utils.py
--rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.2b0/OMTF/Trading/indicators.py
--rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.2b0/OMTF/Trading/portfolios.py
--rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.2b0/OMTF/Trading/randomWalk.py
--rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.2b0/OMTF/Trading/screeners.py
--rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.2b0/OMTF/Trading/signals.py
--rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.2b0/OMTF/Trading/technical.py
--rw-rw-rw-   0        0        0        0 2024-05-13 14:08:33.000000 omtf-1.0.2b0/OMTF/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.232285 omtf-1.0.2b0/OMTF/sp500Historical/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.2b0/OMTF/sp500Historical/__init__.py
--rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.2b0/OMTF/sp500Historical/sp500_historical.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.234284 omtf-1.0.2b0/OMTF.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4521 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1010 2024-05-13 14:37:21.234284 omtf-1.0.2b0/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.2b0/README.md
--rw-rw-rw-   0        0        0     1321 2024-05-13 14:36:47.000000 omtf-1.0.2b0/pyproject.toml
--rw-rw-rw-   0        0        0      730 2024-05-13 14:37:21.240285 omtf-1.0.2b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.233284 omtf-1.0.2b0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:51:01.000000 omtf-1.0.2b0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.697068 omtf-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:38.223976 omtf-1.0.3/OMTF/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.638070 omtf-1.0.3/OMTF/Brokers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Brokers/__init__.py
+-rw-rw-rw-   0        0        0    25562 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Brokers/binance_broker.py
+-rw-rw-rw-   0        0        0    47308 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Brokers/degiro.py
+-rw-rw-rw-   0        0        0    19726 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Brokers/metatrader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.656068 omtf-1.0.3/OMTF/DataProviders/
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/__init__.py
+-rw-rw-rw-   0        0        0     8382 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/aemet.py
+-rw-rw-rw-   0        0        0    35813 2024-05-13 14:51:12.000000 omtf-1.0.3/OMTF/DataProviders/benzinga.py
+-rw-rw-rw-   0        0        0     3043 2024-05-13 14:51:19.000000 omtf-1.0.3/OMTF/DataProviders/coingecko.py
+-rw-rw-rw-   0        0        0     3057 2024-05-13 14:51:25.000000 omtf-1.0.3/OMTF/DataProviders/coinmarketcap.py
+-rw-rw-rw-   0        0        0     9297 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/data.py
+-rw-rw-rw-   0        0        0     8939 2024-05-13 14:51:34.000000 omtf-1.0.3/OMTF/DataProviders/dilutionTracker.py
+-rw-rw-rw-   0        0        0    12959 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/expansion.py
+-rw-rw-rw-   0        0        0    23250 2024-05-13 14:51:49.000000 omtf-1.0.3/OMTF/DataProviders/finviz.py
+-rw-rw-rw-   0        0        0     3007 2024-05-13 14:51:55.000000 omtf-1.0.3/OMTF/DataProviders/floatChecker.py
+-rw-rw-rw-   0        0        0     2644 2024-05-13 14:51:59.000000 omtf-1.0.3/OMTF/DataProviders/fmp.py
+-rw-rw-rw-   0        0        0     9110 2024-05-13 14:52:04.000000 omtf-1.0.3/OMTF/DataProviders/fxstreet.py
+-rw-rw-rw-   0        0        0     3528 2024-05-13 14:52:13.000000 omtf-1.0.3/OMTF/DataProviders/geonames.py
+-rw-rw-rw-   0        0        0     2033 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/inversis_todo.py
+-rw-rw-rw-   0        0        0     8327 2024-05-13 14:52:21.000000 omtf-1.0.3/OMTF/DataProviders/marketWatch.py
+-rw-rw-rw-   0        0        0     2446 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/oecd.py
+-rw-rw-rw-   0        0        0     1980 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/openstreetmap.py
+-rw-rw-rw-   0        0        0    22944 2024-05-13 14:52:35.000000 omtf-1.0.3/OMTF/DataProviders/polygon.py
+-rw-rw-rw-   0        0        0    10057 2024-05-13 14:52:39.000000 omtf-1.0.3/OMTF/DataProviders/sec.py
+-rw-rw-rw-   0        0        0    11939 2024-05-13 14:52:44.000000 omtf-1.0.3/OMTF/DataProviders/tradingterminal.py
+-rw-rw-rw-   0        0        0     5178 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/worldBank.py
+-rw-rw-rw-   0        0        0     4373 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/worldHealthOrg.py
+-rw-rw-rw-   0        0        0     2455 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/DataProviders/world_population.py
+-rw-rw-rw-   0        0        0    19768 2024-05-13 14:52:55.000000 omtf-1.0.3/OMTF/DataProviders/yahoo.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.672068 omtf-1.0.3/OMTF/MachineLearning/
+-rw-rw-rw-   0        0        0    20084 2024-05-13 14:49:05.000000 omtf-1.0.3/OMTF/MachineLearning/00_models_comparison.py
+-rw-rw-rw-   0        0        0    12096 2024-05-13 14:50:36.000000 omtf-1.0.3/OMTF/MachineLearning/RandomForest.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/__init__.py
+-rw-rw-rw-   0        0        0    17758 2024-05-13 14:49:13.000000 omtf-1.0.3/OMTF/MachineLearning/decision_trees.py
+-rw-rw-rw-   0        0        0     9212 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    16219 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/gradientboosting.py
+-rw-rw-rw-   0        0        0     7553 2024-05-13 14:49:25.000000 omtf-1.0.3/OMTF/MachineLearning/k_nearest_neighbors.py
+-rw-rw-rw-   0        0        0     5869 2024-05-13 14:49:32.000000 omtf-1.0.3/OMTF/MachineLearning/kmeans_clustering.py
+-rw-rw-rw-   0        0        0    18425 2024-05-13 14:49:40.000000 omtf-1.0.3/OMTF/MachineLearning/linear_regression.py
+-rw-rw-rw-   0        0        0    16063 2024-05-13 14:49:47.000000 omtf-1.0.3/OMTF/MachineLearning/logistic_regression.py
+-rw-rw-rw-   0        0        0    23342 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/long_short_term_memory.py
+-rw-rw-rw-   0        0        0     9887 2024-05-13 14:49:56.000000 omtf-1.0.3/OMTF/MachineLearning/naive_bayes.py
+-rw-rw-rw-   0        0        0    33248 2024-05-13 14:50:02.000000 omtf-1.0.3/OMTF/MachineLearning/neural_networks.py
+-rw-rw-rw-   0        0        0     8495 2024-05-13 14:50:09.000000 omtf-1.0.3/OMTF/MachineLearning/principal_component.py
+-rw-rw-rw-   0        0        0     9422 2024-05-13 14:50:28.000000 omtf-1.0.3/OMTF/MachineLearning/random_forest.py
+-rw-rw-rw-   0        0        0    18154 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/recurrent_neural_networks.py
+-rw-rw-rw-   0        0        0    11905 2024-05-13 14:50:44.000000 omtf-1.0.3/OMTF/MachineLearning/support_vector.py
+-rw-rw-rw-   0        0        0    20912 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/MachineLearning/utils.py
+-rw-rw-rw-   0        0        0    13406 2024-05-13 14:50:54.000000 omtf-1.0.3/OMTF/MachineLearning/xgboost_model.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.692066 omtf-1.0.3/OMTF/Trading/
+-rw-rw-rw-   0        0        0      102 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/KEYS.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/__init__.py
+-rw-rw-rw-   0        0        0     2767 2024-05-13 14:41:53.000000 omtf-1.0.3/OMTF/Trading/asset_tradeablitiy.py
+-rw-rw-rw-   0        0        0    68761 2024-05-13 14:42:09.000000 omtf-1.0.3/OMTF/Trading/backtest.py
+-rw-rw-rw-   0        0        0    26961 2024-05-13 14:42:04.000000 omtf-1.0.3/OMTF/Trading/backtest_utils.py
+-rw-rw-rw-   0        0        0     9694 2024-05-13 14:42:16.000000 omtf-1.0.3/OMTF/Trading/config.py
+-rw-rw-rw-   0        0        0    37263 2024-05-13 14:42:26.000000 omtf-1.0.3/OMTF/Trading/continuous_backtest.py
+-rw-rw-rw-   0        0        0    44572 2024-05-13 14:43:04.000000 omtf-1.0.3/OMTF/Trading/discrete_backtest.py
+-rw-rw-rw-   0        0        0    51840 2024-05-13 14:43:20.000000 omtf-1.0.3/OMTF/Trading/execution.py
+-rw-rw-rw-   0        0        0    74814 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/execution_utils.py
+-rw-rw-rw-   0        0        0   136092 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/indicators.py
+-rw-rw-rw-   0        0        0    16776 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/portfolios.py
+-rw-rw-rw-   0        0        0    16607 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/randomWalk.py
+-rw-rw-rw-   0        0        0    17910 2024-05-13 14:43:45.000000 omtf-1.0.3/OMTF/Trading/screeners.py
+-rw-rw-rw-   0        0        0   231069 2024-05-13 14:43:44.000000 omtf-1.0.3/OMTF/Trading/signals.py
+-rw-rw-rw-   0        0        0    49172 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/Trading/technical.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.694067 omtf-1.0.3/OMTF/sp500Historical/
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/sp500Historical/__init__.py
+-rw-rw-rw-   0        0        0     9782 2024-05-13 14:39:40.000000 omtf-1.0.3/OMTF/sp500Historical/sp500_historical.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.696068 omtf-1.0.3/OMTF.egg-info/
+-rw-rw-rw-   0        0        0     1008 2024-05-13 14:54:38.000000 omtf-1.0.3/OMTF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-05-13 14:54:38.000000 omtf-1.0.3/OMTF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:54:38.000000 omtf-1.0.3/OMTF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:54:38.000000 omtf-1.0.3/OMTF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1008 2024-05-13 14:54:39.696068 omtf-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1320 2024-05-13 14:54:09.000000 omtf-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2024-05-13 14:54:39.698066 omtf-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:39.695069 omtf-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:51:01.000000 omtf-1.0.3/tests/__init__.py
```

### Comparing `omtf-1.0.2b0/LICENSE` & `omtf-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Brokers/binance_broker.py` & `omtf-1.0.3/OMTF/Brokers/binance_broker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Brokers/degiro.py` & `omtf-1.0.3/OMTF/Brokers/degiro.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Brokers/metatrader.py` & `omtf-1.0.3/OMTF/Brokers/metatrader.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/aemet.py` & `omtf-1.0.3/OMTF/DataProviders/aemet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/benzinga.py` & `omtf-1.0.3/OMTF/DataProviders/benzinga.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import certifi
 import numpy as np
 import pandas as pd
 import requests
 import urllib3
 from bs4 import BeautifulSoup
 
-from data import DataProvider
+from .data import DataProvider
 
 
 class ERROR(Exception):
     
     '''
     Class to raise custom errors.
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/coingecko.py` & `omtf-1.0.3/OMTF/DataProviders/coingecko.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import time
 import requests
 
 import pandas as pd
 
-from data import DataProvider
+from .data import DataProvider
 
 class CoinGecko(DataProvider):
 
     headers: dict = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                                     'Chrome/108.0.0.0 Safari/537.36',
     }
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/coinmarketcap.py` & `omtf-1.0.3/OMTF/DataProviders/coinmarketcap.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import json as JSON
 
 import certifi
 import urllib3
 from bs4 import BeautifulSoup
 
-from data import DataProvider
+from .data import DataProvider
 
 
 class CoinMarketCap(DataProvider):
 
     headers: dict = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) ' \
                                     'Chrome/108.0.0.0 Safari/537.36',
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/data.py` & `omtf-1.0.3/OMTF/DataProviders/data.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/dilutionTracker.py` & `omtf-1.0.3/OMTF/DataProviders/dilutionTracker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime as dt
 from random import choice
 
 import numpy as np
 import pandas as pd
 import requests
 
-from data import DataProvider
+from .data import DataProvider
 
 
 class DilutionTracker(DataProvider):
 
     headers: dict = {
         'Accept': 'application/json',
         'Origin': 'https://dilutiontracker.com',
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/expansion.py` & `omtf-1.0.3/OMTF/DataProviders/expansion.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/finviz.py` & `omtf-1.0.3/OMTF/DataProviders/finviz.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import certifi
 import numpy as np
 import pandas as pd
 import urllib3
 from bs4 import BeautifulSoup
 
-from data import DataProvider
+from .data import DataProvider
 
 class Finviz(DataProvider):
 
     '''
     Class used for webscraping Finviz.
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/floatChecker.py` & `omtf-1.0.3/OMTF/DataProviders/floatChecker.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime as dt
 
 import certifi
 import pandas as pd
 import urllib3
 from bs4 import BeautifulSoup
 
-from data import DataProvider
+from .data import DataProvider
 
 
 class FloatChecker(DataProvider):
 
     # Urls and device to connect
     headers: dict = {
         'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/fmp.py` & `omtf-1.0.3/OMTF/DataProviders/fmp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 import requests
 
-from data import DataProvider
+from .data import DataProvider
 
 class FinancialModellingProp(DataProvider):
 
     '''
     https://site.financialmodelingprep.com/developer/docs/#Stock-Screener
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/fxstreet.py` & `omtf-1.0.3/OMTF/DataProviders/fxstreet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import enum
 import datetime as dt
 import requests
 import pandas as pd
 
-from data import DataProvider
+from .data import DataProvider
 
 class FXStreet(DataProvider):
 
     class Volatility(enum.Enum):
         NONE: str = 'NONE'
         LOW: str = 'LOW'
         MEDIUM: str = 'MEDIUM'
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/geonames.py` & `omtf-1.0.3/OMTF/DataProviders/geonames.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 import enum
 import requests
 import pandas as pd
 
-import pandas as pd
-
 class PoblationStyle(enum.Enum):
     
     SHORT: str = 'SHORT'
     MEDIUM: str = 'MEDIUM'
     LONG: str = 'LONG'
     FULL: str = 'FULL'
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/inversis_todo.py` & `omtf-1.0.3/OMTF/DataProviders/inversis_todo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/marketWatch.py` & `omtf-1.0.3/OMTF/DataProviders/marketWatch.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,520 +2,520 @@
 00000010: 6520 6173 2064 740d 0a69 6d70 6f72 7420  e as dt..import 
 00000020: 6a73 6f6e 0d0a 6672 6f6d 2072 616e 646f  json..from rando
 00000030: 6d20 696d 706f 7274 2063 686f 6963 650d  m import choice.
 00000040: 0a0d 0a69 6d70 6f72 7420 7061 6e64 6173  ...import pandas
 00000050: 2061 7320 7064 0d0a 696d 706f 7274 2072   as pd..import r
 00000060: 6571 7565 7374 730d 0a66 726f 6d20 6273  equests..from bs
 00000070: 3420 696d 706f 7274 2042 6561 7574 6966  4 import Beautif
-00000080: 756c 536f 7570 0d0a 0d0a 6672 6f6d 2064  ulSoup....from d
-00000090: 6174 6120 696d 706f 7274 2044 6174 6150  ata import DataP
-000000a0: 726f 7669 6465 720d 0a0d 0a0d 0a63 6c61  rovider......cla
-000000b0: 7373 204d 6172 6b65 7457 6174 6368 2844  ss MarketWatch(D
-000000c0: 6174 6150 726f 7669 6465 7229 3a0d 0a0d  ataProvider):...
-000000d0: 0a20 2020 2070 6179 6c6f 6164 3a20 6469  .    payload: di
-000000e0: 6374 203d 207b 0d0a 2020 2020 2020 2020  ct = {..        
-000000f0: 2253 7465 7022 3a20 2250 3144 222c 0d0a  "Step": "P1D",..
-00000100: 2020 2020 2020 2020 2254 696d 6546 7261          "TimeFra
-00000110: 6d65 223a 2250 3159 222c 200d 0a20 2020  me":"P1Y", ..   
-00000120: 2020 2020 2022 5374 6172 7444 6174 6522       "StartDate"
-00000130: 3a31 3635 3034 3132 3830 3030 3030 2c0d  :1650412800000,.
-00000140: 0a20 2020 2020 2020 2022 456e 6444 6174  .        "EndDat
-00000150: 6522 3a31 3638 3139 3438 3830 3030 3030  e":1681948800000
-00000160: 2c0d 0a20 2020 2020 2020 2022 456e 7469  ,..        "Enti
-00000170: 746c 656d 656e 7454 6f6b 656e 223a 2022  tlementToken": "
-00000180: 6365 6363 3432 3637 6130 3139 3461 6638  cecc4267a0194af8
-00000190: 3963 6133 3433 3830 3561 3365 3537 6166  9ca343805a3e57af
-000001a0: 222c 0d0a 2020 2020 2020 2020 2249 6e63  ",..        "Inc
-000001b0: 6c75 6465 4d6f 636b 5469 636b 223a 2054  ludeMockTick": T
-000001c0: 7275 652c 0d0a 2020 2020 2020 2020 2246  rue,..        "F
-000001d0: 696c 7465 724e 756c 6c53 6c6f 7473 223a  ilterNullSlots":
-000001e0: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-000001f0: 2022 4669 6c74 6572 436c 6f73 6564 506f   "FilterClosedPo
-00000200: 696e 7473 223a 2054 7275 652c 0d0a 2020  ints": True,..  
-00000210: 2020 2020 2020 2249 6e63 6c75 6465 436c        "IncludeCl
-00000220: 6f73 6564 536c 6f74 7322 3a20 4661 6c73  osedSlots": Fals
-00000230: 652c 0d0a 2020 2020 2020 2020 2249 6e63  e,..        "Inc
-00000240: 6c75 6465 4f66 6669 6369 616c 436c 6f73  ludeOfficialClos
-00000250: 6522 3a20 5472 7565 2c0d 0a20 2020 2020  e": True,..     
-00000260: 2020 2022 496e 6a65 6374 4f70 656e 223a     "InjectOpen":
-00000270: 2046 616c 7365 2c0d 0a20 2020 2020 2020   False,..       
-00000280: 2022 5368 6f77 5072 654d 6172 6b65 7422   "ShowPreMarket"
-00000290: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
-000002a0: 2020 2253 686f 7741 6674 6572 486f 7572    "ShowAfterHour
-000002b0: 7322 3a20 4661 6c73 652c 0d0a 2020 2020  s": False,..    
-000002c0: 2020 2020 2255 7365 4578 7465 6e64 6564      "UseExtended
-000002d0: 5469 6d65 4672 616d 6522 3a20 5472 7565  TimeFrame": True
-000002e0: 2c0d 0a20 2020 2020 2020 2022 5761 6e74  ,..        "Want
-000002f0: 5072 696f 7243 6c6f 7365 223a 2046 616c  PriorClose": Fal
-00000300: 7365 2c0d 0a20 2020 2020 2020 2022 496e  se,..        "In
-00000310: 636c 7564 6543 7572 7265 6e74 5175 6f74  cludeCurrentQuot
-00000320: 6573 223a 2046 616c 7365 2c0d 0a20 2020  es": False,..   
-00000330: 2020 2020 2022 5265 7365 7454 6f64 6179       "ResetToday
-00000340: 7341 6674 6572 486f 7572 7350 6572 6365  sAfterHoursPerce
-00000350: 6e74 4368 616e 6765 223a 2046 616c 7365  ntChange": False
-00000360: 2c0d 0a20 2020 2020 2020 2022 5365 7269  ,..        "Seri
-00000370: 6573 223a 205b 0d0a 2020 2020 2020 2020  es": [..        
-00000380: 2020 2020 7b0d 0a20 2020 2020 2020 2020      {..         
-00000390: 2020 2020 2020 2022 4b65 7922 3a20 2253         "Key": "S
-000003a0: 544f 434b 2f55 532f 584e 4153 2f43 4a4a  TOCK/US/XNAS/CJJ
-000003b0: 4422 2c20 2320 584e 5953 0d0a 2020 2020  D", # XNYS..    
-000003c0: 2020 2020 2020 2020 2020 2020 2244 6961              "Dia
-000003d0: 6c65 6374 223a 2243 6861 7274 696e 6722  lect":"Charting"
-000003e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000003f0: 2020 2022 4b69 6e64 223a 2254 6963 6b65     "Kind":"Ticke
-00000400: 7222 2c0d 0a20 2020 2020 2020 2020 2020  r",..           
-00000410: 2020 2020 2022 5365 7269 6573 4964 223a       "SeriesId":
-00000420: 2273 3122 2c0d 0a20 2020 2020 2020 2020  "s1",..         
-00000430: 2020 2020 2020 2022 4461 7461 5479 7065         "DataType
-00000440: 7322 3a20 5b22 4f70 656e 222c 2248 6967  s": ["Open","Hig
-00000450: 6822 2c22 4c6f 7722 2c22 4c61 7374 225d  h","Low","Last"]
-00000460: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000470: 2020 2022 496e 6469 6361 746f 7273 223a     "Indicators":
-00000480: 205b 0d0a 2020 2020 2020 2020 2020 2020   [..            
-00000490: 2020 2020 2020 2020 7b0d 0a20 2020 2020          {..     
+00000080: 756c 536f 7570 0d0a 0d0a 6672 6f6d 202e  ulSoup....from .
+00000090: 6461 7461 2069 6d70 6f72 7420 4461 7461  data import Data
+000000a0: 5072 6f76 6964 6572 0d0a 0d0a 0d0a 636c  Provider......cl
+000000b0: 6173 7320 4d61 726b 6574 5761 7463 6828  ass MarketWatch(
+000000c0: 4461 7461 5072 6f76 6964 6572 293a 0d0a  DataProvider):..
+000000d0: 0d0a 2020 2020 7061 796c 6f61 643a 2064  ..    payload: d
+000000e0: 6963 7420 3d20 7b0d 0a20 2020 2020 2020  ict = {..       
+000000f0: 2022 5374 6570 223a 2022 5031 4422 2c0d   "Step": "P1D",.
+00000100: 0a20 2020 2020 2020 2022 5469 6d65 4672  .        "TimeFr
+00000110: 616d 6522 3a22 5031 5922 2c20 0d0a 2020  ame":"P1Y", ..  
+00000120: 2020 2020 2020 2253 7461 7274 4461 7465        "StartDate
+00000130: 223a 3136 3530 3431 3238 3030 3030 302c  ":1650412800000,
+00000140: 0d0a 2020 2020 2020 2020 2245 6e64 4461  ..        "EndDa
+00000150: 7465 223a 3136 3831 3934 3838 3030 3030  te":168194880000
+00000160: 302c 0d0a 2020 2020 2020 2020 2245 6e74  0,..        "Ent
+00000170: 6974 6c65 6d65 6e74 546f 6b65 6e22 3a20  itlementToken": 
+00000180: 2263 6563 6334 3236 3761 3031 3934 6166  "cecc4267a0194af
+00000190: 3839 6361 3334 3338 3035 6133 6535 3761  89ca343805a3e57a
+000001a0: 6622 2c0d 0a20 2020 2020 2020 2022 496e  f",..        "In
+000001b0: 636c 7564 654d 6f63 6b54 6963 6b22 3a20  cludeMockTick": 
+000001c0: 5472 7565 2c0d 0a20 2020 2020 2020 2022  True,..        "
+000001d0: 4669 6c74 6572 4e75 6c6c 536c 6f74 7322  FilterNullSlots"
+000001e0: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+000001f0: 2020 2246 696c 7465 7243 6c6f 7365 6450    "FilterClosedP
+00000200: 6f69 6e74 7322 3a20 5472 7565 2c0d 0a20  oints": True,.. 
+00000210: 2020 2020 2020 2022 496e 636c 7564 6543         "IncludeC
+00000220: 6c6f 7365 6453 6c6f 7473 223a 2046 616c  losedSlots": Fal
+00000230: 7365 2c0d 0a20 2020 2020 2020 2022 496e  se,..        "In
+00000240: 636c 7564 654f 6666 6963 6961 6c43 6c6f  cludeOfficialClo
+00000250: 7365 223a 2054 7275 652c 0d0a 2020 2020  se": True,..    
+00000260: 2020 2020 2249 6e6a 6563 744f 7065 6e22      "InjectOpen"
+00000270: 3a20 4661 6c73 652c 0d0a 2020 2020 2020  : False,..      
+00000280: 2020 2253 686f 7750 7265 4d61 726b 6574    "ShowPreMarket
+00000290: 223a 2046 616c 7365 2c0d 0a20 2020 2020  ": False,..     
+000002a0: 2020 2022 5368 6f77 4166 7465 7248 6f75     "ShowAfterHou
+000002b0: 7273 223a 2046 616c 7365 2c0d 0a20 2020  rs": False,..   
+000002c0: 2020 2020 2022 5573 6545 7874 656e 6465       "UseExtende
+000002d0: 6454 696d 6546 7261 6d65 223a 2054 7275  dTimeFrame": Tru
+000002e0: 652c 0d0a 2020 2020 2020 2020 2257 616e  e,..        "Wan
+000002f0: 7450 7269 6f72 436c 6f73 6522 3a20 4661  tPriorClose": Fa
+00000300: 6c73 652c 0d0a 2020 2020 2020 2020 2249  lse,..        "I
+00000310: 6e63 6c75 6465 4375 7272 656e 7451 756f  ncludeCurrentQuo
+00000320: 7465 7322 3a20 4661 6c73 652c 0d0a 2020  tes": False,..  
+00000330: 2020 2020 2020 2252 6573 6574 546f 6461        "ResetToda
+00000340: 7973 4166 7465 7248 6f75 7273 5065 7263  ysAfterHoursPerc
+00000350: 656e 7443 6861 6e67 6522 3a20 4661 6c73  entChange": Fals
+00000360: 652c 0d0a 2020 2020 2020 2020 2253 6572  e,..        "Ser
+00000370: 6965 7322 3a20 5b0d 0a20 2020 2020 2020  ies": [..       
+00000380: 2020 2020 207b 0d0a 2020 2020 2020 2020       {..        
+00000390: 2020 2020 2020 2020 224b 6579 223a 2022          "Key": "
+000003a0: 5354 4f43 4b2f 5553 2f58 4e41 532f 434a  STOCK/US/XNAS/CJ
+000003b0: 4a44 222c 2023 2058 4e59 530d 0a20 2020  JD", # XNYS..   
+000003c0: 2020 2020 2020 2020 2020 2020 2022 4469               "Di
+000003d0: 616c 6563 7422 3a22 4368 6172 7469 6e67  alect":"Charting
+000003e0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+000003f0: 2020 2020 224b 696e 6422 3a22 5469 636b      "Kind":"Tick
+00000400: 6572 222c 0d0a 2020 2020 2020 2020 2020  er",..          
+00000410: 2020 2020 2020 2253 6572 6965 7349 6422        "SeriesId"
+00000420: 3a22 7331 222c 0d0a 2020 2020 2020 2020  :"s1",..        
+00000430: 2020 2020 2020 2020 2244 6174 6154 7970          "DataTyp
+00000440: 6573 223a 205b 224f 7065 6e22 2c22 4869  es": ["Open","Hi
+00000450: 6768 222c 224c 6f77 222c 224c 6173 7422  gh","Low","Last"
+00000460: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000470: 2020 2020 2249 6e64 6963 6174 6f72 7322      "Indicators"
+00000480: 3a20 5b0d 0a20 2020 2020 2020 2020 2020  : [..           
+00000490: 2020 2020 2020 2020 207b 0d0a 2020 2020           {..    
 000004a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004b0: 2020 2022 5061 7261 6d65 7465 7273 223a     "Parameters":
-000004c0: 205b 5d2c 0d0a 2020 2020 2020 2020 2020   [],..          
-000004d0: 2020 2020 2020 2020 2020 2020 2020 224b                "K
-000004e0: 696e 6422 3a20 2256 6f6c 756d 6522 2c0d  ind": "Volume",.
-000004f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000500: 2020 2020 2020 2020 2022 5365 7269 6573           "Series
-00000510: 4964 223a 2022 6932 220d 0a20 2020 2020  Id": "i2"..     
-00000520: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000530: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000540: 2020 2020 2020 2023 207b 0d0a 2020 2020         # {..    
+000004b0: 2020 2020 2250 6172 616d 6574 6572 7322      "Parameters"
+000004c0: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000004e0: 4b69 6e64 223a 2022 566f 6c75 6d65 222c  Kind": "Volume",
+000004f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000500: 2020 2020 2020 2020 2020 2253 6572 6965            "Serie
+00000510: 7349 6422 3a20 2269 3222 0d0a 2020 2020  sId": "i2"..    
+00000520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000530: 7d2c 0d0a 2020 2020 2020 2020 2020 2020  },..            
+00000540: 2020 2020 2020 2020 2320 7b0d 0a20 2020          # {..   
 00000550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000560: 2320 2020 2020 2250 6172 616d 6574 6572  #     "Parameter
-00000570: 7322 3a20 5b0d 0a20 2020 2020 2020 2020  s": [..         
-00000580: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00000590: 2020 2020 207b 224e 616d 6522 3a22 5065       {"Name":"Pe
-000005a0: 7269 6f64 222c 2256 616c 7565 223a 2235  riod","Value":"5
-000005b0: 3022 7d0d 0a20 2020 2020 2020 2020 2020  0"}..           
-000005c0: 2020 2020 2020 2020 2023 2020 2020 205d           #     ]
-000005d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000005e0: 2020 2020 2020 2023 2020 2020 2022 4b69         #     "Ki
-000005f0: 6e64 223a 2253 696d 706c 654d 6f76 696e  nd":"SimpleMovin
-00000600: 6741 7665 7261 6765 222c 0d0a 2020 2020  gAverage",..    
+00000560: 2023 2020 2020 2022 5061 7261 6d65 7465   #     "Paramete
+00000570: 7273 223a 205b 0d0a 2020 2020 2020 2020  rs": [..        
+00000580: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00000590: 2020 2020 2020 7b22 4e61 6d65 223a 2250        {"Name":"P
+000005a0: 6572 696f 6422 2c22 5661 6c75 6522 3a22  eriod","Value":"
+000005b0: 3530 227d 0d0a 2020 2020 2020 2020 2020  50"}..          
+000005c0: 2020 2020 2020 2020 2020 2320 2020 2020            #     
+000005d0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+000005e0: 2020 2020 2020 2020 2320 2020 2020 224b          #     "K
+000005f0: 696e 6422 3a22 5369 6d70 6c65 4d6f 7669  ind":"SimpleMovi
+00000600: 6e67 4176 6572 6167 6522 2c0d 0a20 2020  ngAverage",..   
 00000610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000620: 2320 2253 6572 6965 7349 6422 3a22 6933  # "SeriesId":"i3
-00000630: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00000640: 2020 2020 2020 2023 207d 2c0d 0a20 2020         # },..   
+00000620: 2023 2022 5365 7269 6573 4964 223a 2269   # "SeriesId":"i
+00000630: 3322 0d0a 2020 2020 2020 2020 2020 2020  3"..            
+00000640: 2020 2020 2020 2020 2320 7d2c 0d0a 2020          # },..  
 00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 2023 207b 0d0a 2020 2020 2020 2020 2020   # {..          
-00000670: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00000680: 2250 6172 616d 6574 6572 7322 3a20 5b0d  "Parameters": [.
-00000690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000006a0: 2020 2020 2023 2020 2020 2020 2020 207b       #         {
-000006b0: 224e 616d 6522 3a22 454d 4131 222c 2256  "Name":"EMA1","V
-000006c0: 616c 7565 223a 3132 7d2c 0d0a 2020 2020  alue":12},..    
+00000660: 2020 2320 7b0d 0a20 2020 2020 2020 2020    # {..         
+00000670: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00000680: 2022 5061 7261 6d65 7465 7273 223a 205b   "Parameters": [
+00000690: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000006a0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
+000006b0: 7b22 4e61 6d65 223a 2245 4d41 3122 2c22  {"Name":"EMA1","
+000006c0: 5661 6c75 6522 3a31 327d 2c0d 0a20 2020  Value":12},..   
 000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2320 2020 2020 2020 2020 7b22 4e61 6d65  #         {"Name
-000006f0: 223a 2245 4d41 3222 2c22 5661 6c75 6522  ":"EMA2","Value"
-00000700: 3a32 367d 2c0d 0a20 2020 2020 2020 2020  :26},..         
-00000710: 2020 2020 2020 2020 2020 2023 2020 2020             #    
-00000720: 2020 2020 207b 224e 616d 6522 3a22 5369       {"Name":"Si
-00000730: 676e 616c 4c69 6e65 222c 2256 616c 7565  gnalLine","Value
-00000740: 223a 397d 0d0a 2020 2020 2020 2020 2020  ":9}..          
-00000750: 2020 2020 2020 2020 2020 2320 2020 2020            #     
-00000760: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00000770: 2020 2020 2020 2020 2320 2020 2020 224b          #     "K
-00000780: 696e 6422 3a20 224d 6f76 696e 6741 7665  ind": "MovingAve
-00000790: 7261 6765 436f 6e76 6572 6765 6e63 6544  rageConvergenceD
-000007a0: 6976 6572 6765 6e63 6522 2c0d 0a20 2020  ivergence",..   
+000006e0: 2023 2020 2020 2020 2020 207b 224e 616d   #         {"Nam
+000006f0: 6522 3a22 454d 4132 222c 2256 616c 7565  e":"EMA2","Value
+00000700: 223a 3236 7d2c 0d0a 2020 2020 2020 2020  ":26},..        
+00000710: 2020 2020 2020 2020 2020 2020 2320 2020              #   
+00000720: 2020 2020 2020 7b22 4e61 6d65 223a 2253        {"Name":"S
+00000730: 6967 6e61 6c4c 696e 6522 2c22 5661 6c75  ignalLine","Valu
+00000740: 6522 3a39 7d0d 0a20 2020 2020 2020 2020  e":9}..         
+00000750: 2020 2020 2020 2020 2020 2023 2020 2020             #    
+00000760: 205d 2c0d 0a20 2020 2020 2020 2020 2020   ],..           
+00000770: 2020 2020 2020 2020 2023 2020 2020 2022           #     "
+00000780: 4b69 6e64 223a 2022 4d6f 7669 6e67 4176  Kind": "MovingAv
+00000790: 6572 6167 6543 6f6e 7665 7267 656e 6365  erageConvergence
+000007a0: 4469 7665 7267 656e 6365 222c 0d0a 2020  Divergence",..  
 000007b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007c0: 2023 2020 2020 2022 5365 7269 6573 4964   #     "SeriesId
-000007d0: 223a 2269 3422 0d0a 2020 2020 2020 2020  ":"i4"..        
-000007e0: 2020 2020 2020 2020 2020 2020 2320 7d2c              # },
-000007f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000800: 2020 2020 2020 7b0d 0a20 2020 2020 2020        {..       
+000007c0: 2020 2320 2020 2020 2253 6572 6965 7349    #     "SeriesI
+000007d0: 6422 3a22 6934 220d 0a20 2020 2020 2020  d":"i4"..       
+000007e0: 2020 2020 2020 2020 2020 2020 2023 207d               # }
+000007f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000800: 2020 2020 2020 207b 0d0a 2020 2020 2020         {..      
 00000810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000820: 2022 5061 7261 6d65 7465 7273 223a 205b   "Parameters": [
-00000830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000840: 2020 2020 2020 2020 2020 2020 2020 7b22                {"
-00000850: 4e61 6d65 223a 2259 6561 724f 7665 7259  Name":"YearOverY
-00000860: 6561 7222 7d0d 0a20 2020 2020 2020 2020  ear"}..         
-00000870: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000880: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000890: 2020 2020 2020 2020 2020 2022 4b69 6e64             "Kind
-000008a0: 223a 2022 4561 726e 696e 6773 4576 656e  ": "EarningsEven
-000008b0: 7473 222c 200d 0a20 2020 2020 2020 2020  ts", ..         
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000008d0: 5365 7269 6573 4964 223a 2269 3522 0d0a  SeriesId":"i5"..
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008f0: 2020 2020 7d2c 0d0a 2020 2020 2020 2020      },..        
-00000900: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
+00000820: 2020 2250 6172 616d 6574 6572 7322 3a20    "Parameters": 
+00000830: 5b0d 0a20 2020 2020 2020 2020 2020 2020  [..             
+00000840: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00000850: 224e 616d 6522 3a22 5965 6172 4f76 6572  "Name":"YearOver
+00000860: 5965 6172 227d 0d0a 2020 2020 2020 2020  Year"}..        
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000890: 2020 2020 2020 2020 2020 2020 224b 696e              "Kin
+000008a0: 6422 3a20 2245 6172 6e69 6e67 7345 7665  d": "EarningsEve
+000008b0: 6e74 7322 2c20 0d0a 2020 2020 2020 2020  nts", ..        
+000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008d0: 2253 6572 6965 7349 6422 3a22 6935 220d  "SeriesId":"i5".
+000008e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000008f0: 2020 2020 207d 2c0d 0a20 2020 2020 2020       },..       
+00000900: 2020 2020 2020 2020 2020 2020 207b 0d0a               {..
 00000910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000920: 2020 2020 2020 2022 5061 7261 6d65 7465         "Paramete
-00000930: 7273 223a 205b 5d2c 0d0a 2020 2020 2020  rs": [],..      
+00000920: 2020 2020 2020 2020 2250 6172 616d 6574          "Paramet
+00000930: 6572 7322 3a20 5b5d 2c0d 0a20 2020 2020  ers": [],..     
 00000940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000950: 2020 224b 696e 6422 3a22 4469 7669 6465    "Kind":"Divide
-00000960: 6e64 4576 656e 7473 222c 0d0a 2020 2020  ndEvents",..    
+00000950: 2020 2022 4b69 6e64 223a 2244 6976 6964     "Kind":"Divid
+00000960: 656e 6445 7665 6e74 7322 2c0d 0a20 2020  endEvents",..   
 00000970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000980: 2020 2020 2253 6572 6965 7349 6422 3a22      "SeriesId":"
-00000990: 6936 220d 0a20 2020 2020 2020 2020 2020  i6"..           
-000009a0: 2020 2020 2020 2020 207d 2c0d 0a20 2020           },..   
+00000980: 2020 2020 2022 5365 7269 6573 4964 223a       "SeriesId":
+00000990: 2269 3622 0d0a 2020 2020 2020 2020 2020  "i6"..          
+000009a0: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
 000009b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009c0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
-000009d0: 2020 2020 2020 2020 2020 2020 2250 6172              "Par
-000009e0: 616d 6574 6572 7322 3a5b 5d2c 0d0a 2020  ameters":[],..  
+000009c0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+000009d0: 2020 2020 2020 2020 2020 2020 2022 5061               "Pa
+000009e0: 7261 6d65 7465 7273 223a 5b5d 2c0d 0a20  rameters":[],.. 
 000009f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a00: 2020 2020 2020 224b 696e 6422 3a22 5370        "Kind":"Sp
-00000a10: 6c69 7445 7665 6e74 7322 2c0d 0a20 2020  litEvents",..   
+00000a00: 2020 2020 2020 2022 4b69 6e64 223a 2253         "Kind":"S
+00000a10: 706c 6974 4576 656e 7473 222c 0d0a 2020  plitEvents",..  
 00000a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a30: 2020 2020 2022 5365 7269 6573 4964 223a       "SeriesId":
-00000a40: 2269 3722 0d0a 2020 2020 2020 2020 2020  "i7"..          
-00000a50: 2020 2020 2020 2020 2020 7d2c 0d0a 2020            },..  
+00000a30: 2020 2020 2020 2253 6572 6965 7349 6422        "SeriesId"
+00000a40: 3a22 6937 220d 0a20 2020 2020 2020 2020  :"i7"..         
+00000a50: 2020 2020 2020 2020 2020 207d 2c0d 0a20             },.. 
 00000a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a70: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
-00000a80: 2020 2020 2020 2020 2020 2020 2022 5061               "Pa
-00000a90: 7261 6d65 7465 7273 223a 205b 0d0a 2020  rameters": [..  
+00000a70: 2020 207b 0d0a 2020 2020 2020 2020 2020     {..          
+00000a80: 2020 2020 2020 2020 2020 2020 2020 2250                "P
+00000a90: 6172 616d 6574 6572 7322 3a20 5b0d 0a20  arameters": [.. 
 00000aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ab0: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000ac0: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000ad0: 6c75 6522 3a22 3130 3222 7d2c 0d0a 2020  lue":"102"},..  
+00000ab0: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000ac0: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000ad0: 616c 7565 223a 2231 3032 227d 2c0d 0a20  alue":"102"},.. 
 00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000af0: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000b00: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000b10: 6c75 6522 3a22 3130 3322 7d2c 0d0a 2020  lue":"103"},..  
+00000af0: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000b00: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000b10: 616c 7565 223a 2231 3033 227d 2c0d 0a20  alue":"103"},.. 
 00000b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b30: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000b40: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000b50: 6c75 6522 3a22 3131 3522 7d2c 0d0a 2020  lue":"115"},..  
+00000b30: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000b40: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000b50: 616c 7565 223a 2231 3135 227d 2c0d 0a20  alue":"115"},.. 
 00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b70: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000b80: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000b90: 6c75 6522 3a22 3432 3422 7d2c 0d0a 2020  lue":"424"},..  
+00000b70: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000b80: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000b90: 616c 7565 223a 2234 3234 227d 2c0d 0a20  alue":"424"},.. 
 00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bb0: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000bc0: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000bd0: 6c75 6522 3a22 3432 3522 7d2c 0d0a 2020  lue":"425"},..  
+00000bb0: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000bc0: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000bd0: 616c 7565 223a 2234 3235 227d 2c0d 0a20  alue":"425"},.. 
 00000be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000bf0: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000c00: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000c10: 6c75 6522 3a22 3432 3622 7d2c 0d0a 2020  lue":"426"},..  
+00000bf0: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000c00: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000c10: 616c 7565 223a 2234 3236 227d 2c0d 0a20  alue":"426"},.. 
 00000c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c30: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000c40: 223a 2244 6f63 5479 7065 7322 2c22 5661  ":"DocTypes","Va
-00000c50: 6c75 6522 3a22 3432 3722 7d2c 0d0a 2020  lue":"427"},..  
+00000c30: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000c40: 6522 3a22 446f 6354 7970 6573 222c 2256  e":"DocTypes","V
+00000c50: 616c 7565 223a 2234 3237 227d 2c0d 0a20  alue":"427"},.. 
 00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c70: 2020 2020 2020 2020 2020 7b22 4e61 6d65            {"Name
-00000c80: 223a 2253 6967 6e69 6669 6361 6e63 6520  ":"Significance 
-00000c90: 466c 6167 222c 2256 616c 7565 223a 224e  Flag","Value":"N
-00000ca0: 6f6e 6522 7d0d 0a20 2020 2020 2020 2020  one"}..         
-00000cb0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00000cc0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00000cd0: 2020 2020 2020 2020 2020 2022 4b69 6e64             "Kind
-00000ce0: 223a 224e 6577 7344 656e 7369 7479 222c  ":"NewsDensity",
-00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d00: 2020 2020 2020 2020 2020 2253 6572 6965            "Serie
-00000d10: 7349 6422 3a22 6938 220d 0a20 2020 2020  sId":"i8"..     
-00000d20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00000d30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000d40: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
-00000d50: 207d 0d0a 2020 2020 2020 2020 5d0d 0a20   }..        ].. 
-00000d60: 2020 207d 0d0a 0d0a 2020 2020 6465 6620     }....    def 
-00000d70: 5f72 6571 7565 7374 2873 656c 662c 2075  _request(self, u
-00000d80: 726c 3a73 7472 2c20 6865 6164 6572 733a  rl:str, headers:
-00000d90: 6469 6374 3d4e 6f6e 652c 2070 6172 616d  dict=None, param
-00000da0: 733a 6469 6374 3d4e 6f6e 652c 206a 736f  s:dict=None, jso
-00000db0: 6e3a 626f 6f6c 3d54 7275 650d 0a20 2020  n:bool=True..   
-00000dc0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-00000dd0: 2d3e 2028 6c69 7374 207c 2064 6963 7420  -> (list | dict 
-00000de0: 7c20 7265 7175 6573 7473 2e52 6573 706f  | requests.Respo
-00000df0: 6e73 6529 3a0d 0a0d 0a20 2020 2020 2020  nse):....       
-00000e00: 2069 6620 6865 6164 6572 7320 213d 204e   if headers != N
-00000e10: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00000e20: 2020 6865 6164 6572 733a 2064 6963 7420    headers: dict 
-00000e30: 3d20 7b2a 2a68 6561 6465 7273 2c20 2a2a  = {**headers, **
-00000e40: 7365 6c66 2e5f 7261 6e64 6f6d 5f68 6561  self._random_hea
-00000e50: 6465 7228 297d 0d0a 2020 2020 2020 2020  der()}..        
-00000e60: 0d0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-00000e70: 3a20 7265 7175 6573 7473 2e52 6573 706f  : requests.Respo
-00000e80: 6e73 6520 3d20 7265 7175 6573 7473 2e67  nse = requests.g
-00000e90: 6574 2875 726c 2c20 6865 6164 6572 733d  et(url, headers=
-00000ea0: 6865 6164 6572 732c 7061 7261 6d73 3d70  headers,params=p
-00000eb0: 6172 616d 7329 0d0a 0d0a 2020 2020 2020  arams)....      
-00000ec0: 2020 7265 7475 726e 2073 656c 662e 722e    return self.r.
-00000ed0: 6a73 6f6e 2829 2069 6620 6a73 6f6e 2065  json() if json e
-00000ee0: 6c73 6520 7365 6c66 2e72 0d0a 2020 2020  lse self.r..    
-00000ef0: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
-00000f00: 7444 6174 6128 7365 6c66 2c20 7379 6d62  tData(self, symb
-00000f10: 6f6c 3a73 7472 2c20 7374 6570 3a73 7472  ol:str, step:str
-00000f20: 3d27 5031 4427 2c20 7469 6d65 6672 616d  ='P1D', timefram
-00000f30: 653a 7374 723d 2750 3159 272c 0d0a 2020  e:str='P1Y',..  
-00000f40: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00000f50: 6172 743a 7374 723d 4e6f 6e65 2c20 656e  art:str=None, en
-00000f60: 643a 7374 723d 4e6f 6e65 2c20 7072 656d  d:str=None, prem
-00000f70: 6172 6b65 743a 626f 6f6c 3d54 7275 652c  arket:bool=True,
-00000f80: 2061 6674 6572 686f 7572 733a 626f 6f6c   afterhours:bool
-00000f90: 3d54 7275 652c 0d0a 2020 2020 2020 2020  =True,..        
-00000fa0: 2020 2020 2020 2020 636b 6579 3a73 7472          ckey:str
-00000fb0: 3d27 6365 6363 3432 3637 6130 2729 202d  ='cecc4267a0') -
-00000fc0: 3e20 2864 6963 7420 7c20 7064 2e44 6174  > (dict | pd.Dat
-00000fd0: 6146 7261 6d65 293a 0d0a 2020 2020 2020  aFrame):..      
-00000fe0: 2020 0d0a 2020 2020 2020 2020 7061 796c    ..        payl
-00000ff0: 6f61 6420 3d20 7365 6c66 2e70 6179 6c6f  oad = self.paylo
-00001000: 6164 2e63 6f70 7928 290d 0a20 2020 2020  ad.copy()..     
-00001010: 2020 2069 6620 7374 6172 7420 213d 204e     if start != N
-00001020: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00001030: 2020 7061 796c 6f61 645b 2753 7461 7274    payload['Start
-00001040: 4461 7465 275d 203d 2064 742e 6461 7465  Date'] = dt.date
-00001050: 7469 6d65 2e74 696d 6573 7461 6d70 2864  time.timestamp(d
-00001060: 742e 6461 7465 7469 6d65 2e73 7472 7074  t.datetime.strpt
-00001070: 696d 6528 7374 6172 7429 290d 0a20 2020  ime(start))..   
-00001080: 2020 2020 2069 6620 656e 6420 213d 204e       if end != N
-00001090: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-000010a0: 2020 7061 796c 6f61 645b 2745 6e64 4461    payload['EndDa
-000010b0: 7465 275d 203d 2064 742e 6461 7465 7469  te'] = dt.dateti
-000010c0: 6d65 2e74 696d 6573 7461 6d70 2864 742e  me.timestamp(dt.
-000010d0: 6461 7465 7469 6d65 2e73 7472 7074 696d  datetime.strptim
-000010e0: 6528 7374 6172 7429 290d 0a0d 0a20 2020  e(start))....   
-000010f0: 2020 2020 2068 6561 6465 7273 3a20 6469       headers: di
-00001100: 6374 203d 207b 0d0a 2020 2020 2020 2020  ct = {..        
-00001110: 2020 2020 2741 6363 6570 7427 3a20 2761      'Accept': 'a
-00001120: 7070 6c69 6361 7469 6f6e 2f6a 736f 6e2c  pplication/json,
-00001130: 2074 6578 742f 6a61 7661 7363 7269 7074   text/javascript
-00001140: 2c20 2a2f 2a3b 2071 3d30 2e30 3127 2c0d  , */*; q=0.01',.
-00001150: 0a20 2020 2020 2020 2020 2020 2027 4163  .            'Ac
-00001160: 6365 7074 2d45 6e63 6f64 696e 6727 3a20  cept-Encoding': 
-00001170: 2767 7a69 702c 2064 6566 6c61 7465 2c20  'gzip, deflate, 
-00001180: 6272 272c 0d0a 2020 2020 2020 2020 2020  br',..          
-00001190: 2020 2741 6363 6570 742d 4c61 6e67 7561    'Accept-Langua
-000011a0: 6765 273a 2027 6573 2d45 532c 6573 3b71  ge': 'es-ES,es;q
-000011b0: 3d30 2e39 2c65 6e3b 713d 302e 3827 2c0d  =0.9,en;q=0.8',.
-000011c0: 0a20 2020 2020 2020 2020 2020 2027 436f  .            'Co
-000011d0: 6e6e 6563 7469 6f6e 273a 2027 6b65 6570  nnection': 'keep
-000011e0: 2d61 6c69 7665 272c 0d0a 2020 2020 2020  -alive',..      
-000011f0: 2020 2020 2020 2744 796c 616e 3230 3130        'Dylan2010
-00001200: 2e45 6e74 6974 6c65 6d65 6e74 546f 6b65  .EntitlementToke
-00001210: 6e27 3a20 2763 6563 6334 3236 3761 3031  n': 'cecc4267a01
-00001220: 3934 6166 3839 6361 3334 3338 3035 6133  94af89ca343805a3
-00001230: 6535 3761 6627 2c0d 0a20 2020 2020 2020  e57af',..       
-00001240: 2020 2020 2027 486f 7374 273a 2027 6170       'Host': 'ap
-00001250: 692d 7365 6375 7265 2e77 736a 2e6e 6574  i-secure.wsj.net
-00001260: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
-00001270: 274f 7269 6769 6e27 3a20 2768 7474 7073  'Origin': 'https
-00001280: 3a2f 2f77 7777 2e6d 6172 6b65 7477 6174  ://www.marketwat
-00001290: 6368 2e63 6f6d 272c 0d0a 2020 2020 2020  ch.com',..      
-000012a0: 2020 2020 2020 2752 6566 6572 6572 273a        'Referer':
-000012b0: 2066 2768 7474 7073 3a2f 2f77 7777 2e6d   f'https://www.m
-000012c0: 6172 6b65 7477 6174 6368 2e63 6f6d 2f69  arketwatch.com/i
-000012d0: 6e76 6573 7469 6e67 2f73 746f 636b 2f7b  nvesting/stock/{
-000012e0: 7379 6d62 6f6c 7d27 2c0d 0a20 2020 2020  symbol}',..     
-000012f0: 2020 207d 0d0a 0d0a 2020 2020 2020 2020     }....        
-00001300: 7572 6c3a 2073 7472 203d 2027 6874 7470  url: str = 'http
-00001310: 733a 2f2f 6170 692d 7365 6375 7265 2e77  s://api-secure.w
-00001320: 736a 2e6e 6574 2f61 7069 2f6d 6963 6865  sj.net/api/miche
-00001330: 6c61 6e67 656c 6f2f 7469 6d65 7365 7269  langelo/timeseri
-00001340: 6573 2f68 6973 746f 7279 270d 0a20 2020  es/history'..   
-00001350: 2020 2020 200d 0a20 2020 2020 2020 2064       ..        d
-00001360: 6174 6120 3d20 7365 6c66 2e5f 7265 7175  ata = self._requ
-00001370: 6573 7428 7572 6c3d 7572 6c2c 2068 6561  est(url=url, hea
-00001380: 6465 7273 3d68 6561 6465 7273 2c20 0d0a  ders=headers, ..
-00001390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013a0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-000013b0: 616d 733d 7b27 6a73 6f6e 273a 206a 736f  ams={'json': jso
-000013c0: 6e2e 6475 6d70 7328 7061 796c 6f61 642c  n.dumps(payload,
-000013d0: 2065 6e73 7572 655f 6173 6369 693d 4661   ensure_ascii=Fa
-000013e0: 6c73 6529 2e65 6e63 6f64 6528 2775 7466  lse).encode('utf
-000013f0: 2d38 2729 2c20 0d0a 2020 2020 2020 2020  -8'), ..        
+00000c70: 2020 2020 2020 2020 2020 207b 224e 616d             {"Nam
+00000c80: 6522 3a22 5369 676e 6966 6963 616e 6365  e":"Significance
+00000c90: 2046 6c61 6722 2c22 5661 6c75 6522 3a22   Flag","Value":"
+00000ca0: 4e6f 6e65 227d 0d0a 2020 2020 2020 2020  None"}..        
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00000cd0: 2020 2020 2020 2020 2020 2020 224b 696e              "Kin
+00000ce0: 6422 3a22 4e65 7773 4465 6e73 6974 7922  d":"NewsDensity"
+00000cf0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00000d00: 2020 2020 2020 2020 2020 2022 5365 7269             "Seri
+00000d10: 6573 4964 223a 2269 3822 0d0a 2020 2020  esId":"i8"..    
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d30: 7d0d 0a20 2020 2020 2020 2020 2020 2020  }..             
+00000d40: 2020 205d 0d0a 2020 2020 2020 2020 2020     ]..          
+00000d50: 2020 7d0d 0a20 2020 2020 2020 205d 0d0a    }..        ]..
+00000d60: 2020 2020 7d0d 0a0d 0a20 2020 2064 6566      }....    def
+00000d70: 205f 7265 7175 6573 7428 7365 6c66 2c20   _request(self, 
+00000d80: 7572 6c3a 7374 722c 2068 6561 6465 7273  url:str, headers
+00000d90: 3a64 6963 743d 4e6f 6e65 2c20 7061 7261  :dict=None, para
+00000da0: 6d73 3a64 6963 743d 4e6f 6e65 2c20 6a73  ms:dict=None, js
+00000db0: 6f6e 3a62 6f6f 6c3d 5472 7565 0d0a 2020  on:bool=True..  
+00000dc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00000dd0: 202d 3e20 286c 6973 7420 7c20 6469 6374   -> (list | dict
+00000de0: 207c 2072 6571 7565 7374 732e 5265 7370   | requests.Resp
+00000df0: 6f6e 7365 293a 0d0a 0d0a 2020 2020 2020  onse):....      
+00000e00: 2020 6966 2068 6561 6465 7273 2021 3d20    if headers != 
+00000e10: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00000e20: 2020 2068 6561 6465 7273 3a20 6469 6374     headers: dict
+00000e30: 203d 207b 2a2a 6865 6164 6572 732c 202a   = {**headers, *
+00000e40: 2a73 656c 662e 5f72 616e 646f 6d5f 6865  *self._random_he
+00000e50: 6164 6572 2829 7d0d 0a20 2020 2020 2020  ader()}..       
+00000e60: 200d 0a20 2020 2020 2020 2073 656c 662e   ..        self.
+00000e70: 723a 2072 6571 7565 7374 732e 5265 7370  r: requests.Resp
+00000e80: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
+00000e90: 6765 7428 7572 6c2c 2068 6561 6465 7273  get(url, headers
+00000ea0: 3d68 6561 6465 7273 2c70 6172 616d 733d  =headers,params=
+00000eb0: 7061 7261 6d73 290d 0a0d 0a20 2020 2020  params)....     
+00000ec0: 2020 2072 6574 7572 6e20 7365 6c66 2e72     return self.r
+00000ed0: 2e6a 736f 6e28 2920 6966 206a 736f 6e20  .json() if json 
+00000ee0: 656c 7365 2073 656c 662e 720d 0a20 2020  else self.r..   
+00000ef0: 2020 2020 200d 0a20 2020 2064 6566 2067       ..    def g
+00000f00: 6574 4461 7461 2873 656c 662c 2073 796d  etData(self, sym
+00000f10: 626f 6c3a 7374 722c 2073 7465 703a 7374  bol:str, step:st
+00000f20: 723d 2750 3144 272c 2074 696d 6566 7261  r='P1D', timefra
+00000f30: 6d65 3a73 7472 3d27 5031 5927 2c0d 0a20  me:str='P1Y',.. 
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00000f50: 7461 7274 3a73 7472 3d4e 6f6e 652c 2065  tart:str=None, e
+00000f60: 6e64 3a73 7472 3d4e 6f6e 652c 2070 7265  nd:str=None, pre
+00000f70: 6d61 726b 6574 3a62 6f6f 6c3d 5472 7565  market:bool=True
+00000f80: 2c20 6166 7465 7268 6f75 7273 3a62 6f6f  , afterhours:boo
+00000f90: 6c3d 5472 7565 2c0d 0a20 2020 2020 2020  l=True,..       
+00000fa0: 2020 2020 2020 2020 2063 6b65 793a 7374           ckey:st
+00000fb0: 723d 2763 6563 6334 3236 3761 3027 2920  r='cecc4267a0') 
+00000fc0: 2d3e 2028 6469 6374 207c 2070 642e 4461  -> (dict | pd.Da
+00000fd0: 7461 4672 616d 6529 3a0d 0a20 2020 2020  taFrame):..     
+00000fe0: 2020 200d 0a20 2020 2020 2020 2070 6179     ..        pay
+00000ff0: 6c6f 6164 203d 2073 656c 662e 7061 796c  load = self.payl
+00001000: 6f61 642e 636f 7079 2829 0d0a 2020 2020  oad.copy()..    
+00001010: 2020 2020 6966 2073 7461 7274 2021 3d20      if start != 
+00001020: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+00001030: 2020 2070 6179 6c6f 6164 5b27 5374 6172     payload['Star
+00001040: 7444 6174 6527 5d20 3d20 6474 2e64 6174  tDate'] = dt.dat
+00001050: 6574 696d 652e 7469 6d65 7374 616d 7028  etime.timestamp(
+00001060: 6474 2e64 6174 6574 696d 652e 7374 7270  dt.datetime.strp
+00001070: 7469 6d65 2873 7461 7274 2929 0d0a 2020  time(start))..  
+00001080: 2020 2020 2020 6966 2065 6e64 2021 3d20        if end != 
+00001090: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
+000010a0: 2020 2070 6179 6c6f 6164 5b27 456e 6444     payload['EndD
+000010b0: 6174 6527 5d20 3d20 6474 2e64 6174 6574  ate'] = dt.datet
+000010c0: 696d 652e 7469 6d65 7374 616d 7028 6474  ime.timestamp(dt
+000010d0: 2e64 6174 6574 696d 652e 7374 7270 7469  .datetime.strpti
+000010e0: 6d65 2873 7461 7274 2929 0d0a 0d0a 2020  me(start))....  
+000010f0: 2020 2020 2020 6865 6164 6572 733a 2064        headers: d
+00001100: 6963 7420 3d20 7b0d 0a20 2020 2020 2020  ict = {..       
+00001110: 2020 2020 2027 4163 6365 7074 273a 2027       'Accept': '
+00001120: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
+00001130: 2c20 7465 7874 2f6a 6176 6173 6372 6970  , text/javascrip
+00001140: 742c 202a 2f2a 3b20 713d 302e 3031 272c  t, */*; q=0.01',
+00001150: 0d0a 2020 2020 2020 2020 2020 2020 2741  ..            'A
+00001160: 6363 6570 742d 456e 636f 6469 6e67 273a  ccept-Encoding':
+00001170: 2027 677a 6970 2c20 6465 666c 6174 652c   'gzip, deflate,
+00001180: 2062 7227 2c0d 0a20 2020 2020 2020 2020   br',..         
+00001190: 2020 2027 4163 6365 7074 2d4c 616e 6775     'Accept-Langu
+000011a0: 6167 6527 3a20 2765 732d 4553 2c65 733b  age': 'es-ES,es;
+000011b0: 713d 302e 392c 656e 3b71 3d30 2e38 272c  q=0.9,en;q=0.8',
+000011c0: 0d0a 2020 2020 2020 2020 2020 2020 2743  ..            'C
+000011d0: 6f6e 6e65 6374 696f 6e27 3a20 276b 6565  onnection': 'kee
+000011e0: 702d 616c 6976 6527 2c0d 0a20 2020 2020  p-alive',..     
+000011f0: 2020 2020 2020 2027 4479 6c61 6e32 3031         'Dylan201
+00001200: 302e 456e 7469 746c 656d 656e 7454 6f6b  0.EntitlementTok
+00001210: 656e 273a 2027 6365 6363 3432 3637 6130  en': 'cecc4267a0
+00001220: 3139 3461 6638 3963 6133 3433 3830 3561  194af89ca343805a
+00001230: 3365 3537 6166 272c 0d0a 2020 2020 2020  3e57af',..      
+00001240: 2020 2020 2020 2748 6f73 7427 3a20 2761        'Host': 'a
+00001250: 7069 2d73 6563 7572 652e 7773 6a2e 6e65  pi-secure.wsj.ne
+00001260: 7427 2c0d 0a20 2020 2020 2020 2020 2020  t',..           
+00001270: 2027 4f72 6967 696e 273a 2027 6874 7470   'Origin': 'http
+00001280: 733a 2f2f 7777 772e 6d61 726b 6574 7761  s://www.marketwa
+00001290: 7463 682e 636f 6d27 2c0d 0a20 2020 2020  tch.com',..     
+000012a0: 2020 2020 2020 2027 5265 6665 7265 7227         'Referer'
+000012b0: 3a20 6627 6874 7470 733a 2f2f 7777 772e  : f'https://www.
+000012c0: 6d61 726b 6574 7761 7463 682e 636f 6d2f  marketwatch.com/
+000012d0: 696e 7665 7374 696e 672f 7374 6f63 6b2f  investing/stock/
+000012e0: 7b73 796d 626f 6c7d 272c 0d0a 2020 2020  {symbol}',..    
+000012f0: 2020 2020 7d0d 0a0d 0a20 2020 2020 2020      }....       
+00001300: 2075 726c 3a20 7374 7220 3d20 2768 7474   url: str = 'htt
+00001310: 7073 3a2f 2f61 7069 2d73 6563 7572 652e  ps://api-secure.
+00001320: 7773 6a2e 6e65 742f 6170 692f 6d69 6368  wsj.net/api/mich
+00001330: 656c 616e 6765 6c6f 2f74 696d 6573 6572  elangelo/timeser
+00001340: 6965 732f 6869 7374 6f72 7927 0d0a 2020  ies/history'..  
+00001350: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00001360: 6461 7461 203d 2073 656c 662e 5f72 6571  data = self._req
+00001370: 7565 7374 2875 726c 3d75 726c 2c20 6865  uest(url=url, he
+00001380: 6164 6572 733d 6865 6164 6572 732c 200d  aders=headers, .
+00001390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000013a0: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+000013b0: 7261 6d73 3d7b 276a 736f 6e27 3a20 6a73  rams={'json': js
+000013c0: 6f6e 2e64 756d 7073 2870 6179 6c6f 6164  on.dumps(payload
+000013d0: 2c20 656e 7375 7265 5f61 7363 6969 3d46  , ensure_ascii=F
+000013e0: 616c 7365 292e 656e 636f 6465 2827 7574  alse).encode('ut
+000013f0: 662d 3827 292c 200d 0a20 2020 2020 2020  f-8'), ..       
 00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001410: 2020 2020 2020 2020 2763 6b65 7927 3a20          'ckey': 
-00001420: 636b 6579 7d29 0d0a 2020 2020 2020 2020  ckey})..        
-00001430: 7072 696e 7428 6461 7461 290d 0a20 2020  print(data)..   
-00001440: 2020 2020 2064 663a 2070 642e 4461 7461       df: pd.Data
-00001450: 4672 616d 6520 3d20 7064 2e44 6174 6146  Frame = pd.DataF
-00001460: 7261 6d65 2829 0d0a 2020 2020 2020 2020  rame()..        
-00001470: 6466 5b27 5469 6d65 275d 203d 2064 6174  df['Time'] = dat
-00001480: 615b 2754 696d 6549 6e66 6f27 5d5b 2754  a['TimeInfo']['T
-00001490: 6963 6b73 275d 0d0a 2020 2020 2020 2020  icks']..        
-000014a0: 6466 5b27 4461 7465 5469 6d65 275d 203d  df['DateTime'] =
-000014b0: 2070 642e 746f 5f64 6174 6574 696d 6528   pd.to_datetime(
-000014c0: 6466 5b27 5469 6d65 275d 2c20 756e 6974  df['Time'], unit
-000014d0: 3d27 6d73 2729 0d0a 2020 2020 2020 2020  ='ms')..        
-000014e0: 6466 2e73 6574 5f69 6e64 6578 286b 6579  df.set_index(key
-000014f0: 733d 2744 6174 6554 696d 6527 2c20 696e  s='DateTime', in
-00001500: 706c 6163 653d 5472 7565 290d 0a20 2020  place=True)..   
-00001510: 2020 2020 2064 663a 2070 642e 4461 7461       df: pd.Data
-00001520: 4672 616d 6520 3d20 6466 2e74 7a5f 6c6f  Frame = df.tz_lo
-00001530: 6361 6c69 7a65 2874 7a3d 2755 5443 2729  calize(tz='UTC')
-00001540: 2364 742e 6461 7465 7469 6d65 2e6e 6f77  #dt.datetime.now
-00001550: 2864 742e 7469 6d65 7a6f 6e65 2e75 7463  (dt.timezone.utc
-00001560: 292e 6173 7469 6d65 7a6f 6e65 2829 2e74  ).astimezone().t
-00001570: 7a69 6e66 6f29 0d0a 2020 2020 2020 2020  zinfo)..        
-00001580: 6466 3a20 7064 2e44 6174 6146 7261 6d65  df: pd.DataFrame
-00001590: 203d 2064 662e 747a 5f63 6f6e 7665 7274   = df.tz_convert
-000015a0: 2827 416d 6572 6963 612f 4e65 775f 596f  ('America/New_Yo
-000015b0: 726b 2729 0d0a 2020 2020 2020 2020 666f  rk')..        fo
-000015c0: 7220 7320 696e 2064 6174 615b 2753 6572  r s in data['Ser
-000015d0: 6965 7327 5d3a 0d0a 2020 2020 2020 2020  ies']:..        
-000015e0: 2020 2020 6466 5b73 5b27 4465 7369 7265      df[s['Desire
-000015f0: 6444 6174 6150 6f69 6e74 7327 5d5d 203d  dDataPoints']] =
-00001600: 2073 5b27 4461 7461 506f 696e 7473 275d   s['DataPoints']
-00001610: 0d0a 2020 2020 2020 2020 6466 2e72 656e  ..        df.ren
-00001620: 616d 6528 636f 6c75 6d6e 733d 7b27 4c61  ame(columns={'La
-00001630: 7374 273a 2743 6c6f 7365 277d 2c20 696e  st':'Close'}, in
-00001640: 706c 6163 653d 5472 7565 290d 0a0d 0a20  place=True).... 
-00001650: 2020 2020 2020 2069 6620 7072 656d 6172         if premar
-00001660: 6b65 7420 6f72 2061 6674 6572 686f 7572  ket or afterhour
-00001670: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-00001680: 6461 7461 3a20 6469 6374 203d 207b 2754  data: dict = {'T
-00001690: 6f74 616c 273a 6466 7d0d 0a20 2020 2020  otal':df}..     
-000016a0: 2020 2020 2020 2069 6620 7072 656d 6172         if premar
-000016b0: 6b65 743a 0d0a 2020 2020 2020 2020 2020  ket:..          
-000016c0: 2020 2020 2020 6461 7461 5b27 504d 275d        data['PM']
-000016d0: 203d 2064 662e 6265 7477 6565 6e5f 7469   = df.between_ti
-000016e0: 6d65 2827 3030 3a30 3027 2c20 2730 393a  me('00:00', '09:
-000016f0: 3330 2729 0d0a 2020 2020 2020 2020 2020  30')..          
-00001700: 2020 6966 2061 6674 6572 686f 7572 733a    if afterhours:
-00001710: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001720: 2020 6461 7461 5b27 4148 275d 203d 2064    data['AH'] = d
-00001730: 662e 6265 7477 6565 6e5f 7469 6d65 2827  f.between_time('
-00001740: 3136 3a30 3027 2c20 2732 333a 3539 2729  16:00', '23:59')
-00001750: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00001760: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001770: 6120 3d20 6466 2e63 6f70 7928 290d 0a0d  a = df.copy()...
-00001780: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001790: 6461 7461 0d0a 0d0a 0d0a 2020 2020 6465  data......    de
-000017a0: 6620 6765 7451 756f 7465 2873 656c 662c  f getQuote(self,
-000017b0: 2073 796d 626f 6c73 3a6c 6973 7429 3a0d   symbols:list):.
-000017c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000017d0: 2020 2070 6172 616d 733a 2064 6963 7420     params: dict 
-000017e0: 3d20 7b0d 0a20 2020 2020 2020 2020 2020  = {..           
-000017f0: 2027 6469 616c 6563 7427 3a20 276f 6666   'dialect': 'off
-00001800: 6963 6961 6c27 2c0d 0a20 2020 2020 2020  icial',..       
-00001810: 2020 2020 2027 6e65 6564 6564 273a 2027       'needed': '
-00001820: 436f 6d70 6f73 6974 6554 7261 6469 6e67  CompositeTrading
-00001830: 7c42 6c75 6567 7261 7373 4368 616e 6e65  |BluegrassChanne
-00001840: 6c73 272c 0d0a 2020 2020 2020 2020 2020  ls',..          
-00001850: 2020 274d 6178 496e 7374 7275 6d65 6e74    'MaxInstrument
-00001860: 4d61 7463 6865 7327 3a20 2731 272c 0d0a  Matches': '1',..
-00001870: 2020 2020 2020 2020 2020 2020 2761 6363              'acc
-00001880: 6570 7427 3a20 2761 7070 6c69 6361 7469  ept': 'applicati
-00001890: 6f6e 2f6a 736f 6e27 2c0d 0a20 2020 2020  on/json',..     
-000018a0: 2020 2020 2020 2027 456e 7469 746c 656d         'Entitlem
-000018b0: 656e 7454 6f6b 656e 273a 2027 6365 6363  entToken': 'cecc
-000018c0: 3432 3637 6130 3139 3461 6638 3963 6133  4267a0194af89ca3
-000018d0: 3433 3830 3561 3365 3537 6166 272c 0d0a  43805a3e57af',..
-000018e0: 2020 2020 2020 2020 2020 2020 2763 6b65              'cke
-000018f0: 7927 3a20 2763 6563 6334 3236 3761 3027  y': 'cecc4267a0'
-00001900: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00001910: 6469 616c 6563 7473 273a 2027 4368 6172  dialects': 'Char
-00001920: 7469 6e67 272c 0d0a 2020 2020 2020 2020  ting',..        
-00001930: 2020 2020 2769 6427 3a20 272c 272e 6a6f      'id': ','.jo
-00001940: 696e 285b 6627 5374 6f63 6b2d 5553 2d7b  in([f'Stock-US-{
-00001950: 737d 2720 666f 7220 7320 696e 2073 796d  s}' for s in sym
-00001960: 626f 6c73 5d29 0d0a 2020 2020 2020 2020  bols])..        
-00001970: 7d0d 0a20 2020 2020 2020 200d 0a20 2020  }..        ..   
-00001980: 2020 2020 2068 6561 6465 7273 3a20 6469       headers: di
-00001990: 6374 203d 207b 0d0a 2020 2020 2020 2020  ct = {..        
-000019a0: 2020 2020 2741 6363 6570 7427 3a20 272a      'Accept': '*
-000019b0: 2f2a 272c 0d0a 2020 2020 2020 2020 2020  /*',..          
-000019c0: 2020 2741 6363 6570 742d 456e 636f 6469    'Accept-Encodi
-000019d0: 6e67 273a 2027 677a 6970 2c20 6465 666c  ng': 'gzip, defl
-000019e0: 6174 652c 2062 7227 2c0d 0a20 2020 2020  ate, br',..     
-000019f0: 2020 2020 2020 2027 4163 6365 7074 2d4c         'Accept-L
-00001a00: 616e 6775 6167 6527 3a20 2765 732d 4553  anguage': 'es-ES
-00001a10: 2c65 733b 713d 302e 392c 656e 3b71 3d30  ,es;q=0.9,en;q=0
-00001a20: 2e38 272c 0d0a 2020 2020 2020 2020 2020  .8',..          
-00001a30: 2020 2743 6f6e 6e65 6374 696f 6e27 3a20    'Connection': 
-00001a40: 276b 6565 702d 616c 6976 6527 2c0d 0a20  'keep-alive',.. 
-00001a50: 2020 2020 2020 2020 2020 2027 486f 7374             'Host
-00001a60: 273a 2027 6170 692e 7773 6a2e 6e65 7427  ': 'api.wsj.net'
-00001a70: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00001a80: 4f72 6967 696e 273a 2027 6874 7470 733a  Origin': 'https:
-00001a90: 2f2f 7777 772e 6d61 726b 6574 7761 7463  //www.marketwatc
-00001aa0: 682e 636f 6d27 2c0d 0a20 2020 2020 2020  h.com',..       
-00001ab0: 2020 2020 2027 5265 6665 7265 7227 3a20       'Referer': 
-00001ac0: 6627 6874 7470 733a 2f2f 7777 772e 6d61  f'https://www.ma
-00001ad0: 726b 6574 7761 7463 682e 636f 6d2f 696e  rketwatch.com/in
-00001ae0: 7665 7374 696e 672f 7374 6f63 6b2f 7b73  vesting/stock/{s
-00001af0: 796d 626f 6c73 5b30 5d7d 272c 0d0a 2020  ymbols[0]}',..  
-00001b00: 2020 2020 2020 7d0d 0a0d 0a20 2020 2020        }....     
-00001b10: 2020 2075 726c 3a20 7374 7220 3d20 2768     url: str = 'h
-00001b20: 7474 7073 3a2f 2f61 7069 2e77 736a 2e6e  ttps://api.wsj.n
-00001b30: 6574 2f61 7069 2f64 796c 616e 2f71 756f  et/api/dylan/quo
-00001b40: 7465 732f 7632 2f63 6f6d 702f 7175 6f74  tes/v2/comp/quot
-00001b50: 6542 7944 6961 6c65 6374 270d 0a20 2020  eByDialect'..   
-00001b60: 2020 2020 200d 0a20 2020 2020 2020 2071       ..        q
-00001b70: 756f 7465 203d 2073 656c 662e 5f72 6571  uote = self._req
-00001b80: 7565 7374 2875 726c 3d75 726c 2c20 6865  uest(url=url, he
-00001b90: 6164 6572 733d 6865 6164 6572 732c 2070  aders=headers, p
-00001ba0: 6172 616d 733d 7061 7261 6d73 290d 0a20  arams=params).. 
-00001bb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00001bc0: 2072 6574 7572 6e20 7175 6f74 650d 0a0d   return quote...
-00001bd0: 0a20 2020 2064 6566 2067 6574 5072 656d  .    def getPrem
-00001be0: 6172 6b65 7428 7365 6c66 2920 2d3e 2064  arket(self) -> d
-00001bf0: 6963 743a 0d0a 0d0a 2020 2020 2020 2020  ict:....        
-00001c00: 6865 6164 6572 733a 2064 6963 7420 3d20  headers: dict = 
-00001c10: 7b0d 0a20 2020 2020 2020 2020 2020 2027  {..            '
-00001c20: 4f72 6967 696e 273a 2027 6874 7470 733a  Origin': 'https:
-00001c30: 2f2f 7777 772e 6d61 726b 6574 7761 7463  //www.marketwatc
-00001c40: 682e 636f 6d27 2c0d 0a20 2020 2020 2020  h.com',..       
-00001c50: 207d 0d0a 2020 2020 2020 2020 7572 6c3a   }..        url:
-00001c60: 2073 7472 203d 2027 6874 7470 733a 2f2f   str = 'https://
-00001c70: 7777 772e 6d61 726b 6574 7761 7463 682e  www.marketwatch.
-00001c80: 636f 6d2f 746f 6f6c 732f 7363 7265 656e  com/tools/screen
-00001c90: 6572 2f70 7265 6d61 726b 6574 270d 0a0d  er/premarket'...
-00001ca0: 0a20 2020 2020 2020 2072 3a20 7265 7175  .        r: requ
-00001cb0: 6573 7473 2e52 6573 706f 6e73 6520 3d20  ests.Response = 
-00001cc0: 7365 6c66 2e5f 7265 7175 6573 7428 7572  self._request(ur
-00001cd0: 6c3d 7572 6c2c 2068 6561 6465 7273 3d68  l=url, headers=h
-00001ce0: 6561 6465 7273 2c20 6a73 6f6e 3d46 616c  eaders, json=Fal
-00001cf0: 7365 290d 0a20 2020 2020 2020 2068 746d  se)..        htm
-00001d00: 6c3a 2042 6561 7574 6966 756c 536f 7570  l: BeautifulSoup
-00001d10: 203d 2042 6561 7574 6966 756c 536f 7570   = BeautifulSoup
-00001d20: 2872 2e74 6578 742c 2027 6874 6d6c 2e70  (r.text, 'html.p
-00001d30: 6172 7365 7227 290d 0a0d 0a20 2020 2020  arser')....     
-00001d40: 2020 2074 6162 6c65 733a 2073 6574 203d     tables: set =
-00001d50: 2068 746d 6c2e 6669 6e64 5f61 6c6c 2827   html.find_all('
-00001d60: 7461 626c 6527 202c 7b27 636c 6173 7327  table' ,{'class'
-00001d70: 3a27 7461 626c 6520 7461 626c 652d 2d6f  :'table table--o
-00001d80: 7665 7266 6c6f 7720 616c 6967 6e2d 2d72  verflow align--r
-00001d90: 6967 6874 277d 290d 0a0d 0a20 2020 2020  ight'})....     
-00001da0: 2020 2064 6673 3a20 6c69 7374 203d 205b     dfs: list = [
-00001db0: 5d0d 0a20 2020 2020 2020 2066 6f72 2074  ]..        for t
-00001dc0: 6162 6c65 2069 6e20 7461 626c 6573 3a0d  able in tables:.
-00001dd0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-00001de0: 756d 6e73 3a20 6c69 7374 203d 205b 5b63  umns: list = [[c
-00001df0: 2066 6f72 2063 2069 6e20 692e 636f 6e74   for c in i.cont
-00001e00: 656e 7473 2069 6620 6320 213d 2027 5c6e  ents if c != '\n
-00001e10: 275d 5b30 5d2e 6765 745f 7465 7874 2829  '][0].get_text()
-00001e20: 2066 6f72 2069 2069 6e20 7461 626c 652e   for i in table.
-00001e30: 6669 6e64 5f61 6c6c 2827 7468 2729 5d0d  find_all('th')].
-00001e40: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
-00001e50: 613a 206c 6973 7420 3d20 5b5b 6365 6c6c  a: list = [[cell
-00001e60: 2e67 6574 5f74 6578 7428 292e 7265 706c  .get_text().repl
-00001e70: 6163 6528 275c 6e27 2c20 2727 2920 666f  ace('\n', '') fo
-00001e80: 7220 6365 6c6c 2069 6e20 726f 772e 6669  r cell in row.fi
-00001e90: 6e64 5f61 6c6c 2827 7464 2729 5d20 5c0d  nd_all('td')] \.
-00001ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001eb0: 2020 2020 2066 6f72 2072 6f77 2069 6e20       for row in 
-00001ec0: 7461 626c 652e 6669 6e64 5f61 6c6c 2827  table.find_all('
-00001ed0: 7472 2729 5d5b 313a 5d0d 0a20 2020 2020  tr')][1:]..     
-00001ee0: 2020 2020 2020 2064 663a 2070 642e 4461         df: pd.Da
-00001ef0: 7461 4672 616d 6520 3d20 7064 2e44 6174  taFrame = pd.Dat
-00001f00: 6146 7261 6d65 2863 6f6c 756d 6e73 3d63  aFrame(columns=c
-00001f10: 6f6c 756d 6e73 2c20 6461 7461 3d64 6174  olumns, data=dat
-00001f20: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
-00001f30: 6466 5b27 5379 6d62 6f6c 275d 203d 2064  df['Symbol'] = d
-00001f40: 665b 2753 796d 626f 6c27 5d2e 6170 706c  f['Symbol'].appl
-00001f50: 7928 6c61 6d62 6461 2078 3a20 785b 3a69  y(lambda x: x[:i
-00001f60: 6e74 286c 656e 2878 292f 3229 5d29 0d0a  nt(len(x)/2)])..
-00001f70: 2020 2020 2020 2020 2020 2020 6466 732e              dfs.
-00001f80: 6170 7065 6e64 2864 6629 0d0a 2020 2020  append(df)..    
-00001f90: 2020 2020 6466 733a 2064 6963 7420 3d20      dfs: dict = 
-00001fa0: 7b0d 0a20 2020 2020 2020 2020 2020 2027  {..            '
-00001fb0: 4761 696e 6572 7327 3a20 6466 735b 305d  Gainers': dfs[0]
-00001fc0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
-00001fd0: 4c6f 7365 7273 273a 2064 6673 5b31 5d2c  Losers': dfs[1],
-00001fe0: 0d0a 2020 2020 2020 2020 2020 2020 2741  ..            'A
-00001ff0: 6374 6976 6527 3a20 6466 735b 325d 0d0a  ctive': dfs[2]..
-00002000: 2020 2020 2020 2020 7d0d 0a0d 0a20 2020          }....   
-00002010: 2020 2020 2072 6574 7572 6e20 6466 730d       return dfs.
-00002020: 0a20 2020 200d 0a20 2020 200d 0a0d 0a69  .    ..    ....i
-00002030: 6620 5f5f 6e61 6d65 5f5f 203d 3d20 275f  f __name__ == '_
-00002040: 5f6d 6169 6e5f 5f27 3a0d 0a0d 0a20 2020  _main__':....   
-00002050: 206d 7720 3d20 4d61 726b 6574 5761 7463   mw = MarketWatc
-00002060: 6828 290d 0a20 2020 2070 7265 6d61 726b  h()..    premark
-00002070: 6574 203d 206d 772e 6765 7450 7265 6d61  et = mw.getPrema
-00002080: 726b 6574 2829                           rket()
+00001410: 2020 2020 2020 2020 2027 636b 6579 273a           'ckey':
+00001420: 2063 6b65 797d 290d 0a20 2020 2020 2020   ckey})..       
+00001430: 2070 7269 6e74 2864 6174 6129 0d0a 2020   print(data)..  
+00001440: 2020 2020 2020 6466 3a20 7064 2e44 6174        df: pd.Dat
+00001450: 6146 7261 6d65 203d 2070 642e 4461 7461  aFrame = pd.Data
+00001460: 4672 616d 6528 290d 0a20 2020 2020 2020  Frame()..       
+00001470: 2064 665b 2754 696d 6527 5d20 3d20 6461   df['Time'] = da
+00001480: 7461 5b27 5469 6d65 496e 666f 275d 5b27  ta['TimeInfo']['
+00001490: 5469 636b 7327 5d0d 0a20 2020 2020 2020  Ticks']..       
+000014a0: 2064 665b 2744 6174 6554 696d 6527 5d20   df['DateTime'] 
+000014b0: 3d20 7064 2e74 6f5f 6461 7465 7469 6d65  = pd.to_datetime
+000014c0: 2864 665b 2754 696d 6527 5d2c 2075 6e69  (df['Time'], uni
+000014d0: 743d 276d 7327 290d 0a20 2020 2020 2020  t='ms')..       
+000014e0: 2064 662e 7365 745f 696e 6465 7828 6b65   df.set_index(ke
+000014f0: 7973 3d27 4461 7465 5469 6d65 272c 2069  ys='DateTime', i
+00001500: 6e70 6c61 6365 3d54 7275 6529 0d0a 2020  nplace=True)..  
+00001510: 2020 2020 2020 6466 3a20 7064 2e44 6174        df: pd.Dat
+00001520: 6146 7261 6d65 203d 2064 662e 747a 5f6c  aFrame = df.tz_l
+00001530: 6f63 616c 697a 6528 747a 3d27 5554 4327  ocalize(tz='UTC'
+00001540: 2923 6474 2e64 6174 6574 696d 652e 6e6f  )#dt.datetime.no
+00001550: 7728 6474 2e74 696d 657a 6f6e 652e 7574  w(dt.timezone.ut
+00001560: 6329 2e61 7374 696d 657a 6f6e 6528 292e  c).astimezone().
+00001570: 747a 696e 666f 290d 0a20 2020 2020 2020  tzinfo)..       
+00001580: 2064 663a 2070 642e 4461 7461 4672 616d   df: pd.DataFram
+00001590: 6520 3d20 6466 2e74 7a5f 636f 6e76 6572  e = df.tz_conver
+000015a0: 7428 2741 6d65 7269 6361 2f4e 6577 5f59  t('America/New_Y
+000015b0: 6f72 6b27 290d 0a20 2020 2020 2020 2066  ork')..        f
+000015c0: 6f72 2073 2069 6e20 6461 7461 5b27 5365  or s in data['Se
+000015d0: 7269 6573 275d 3a0d 0a20 2020 2020 2020  ries']:..       
+000015e0: 2020 2020 2064 665b 735b 2744 6573 6972       df[s['Desir
+000015f0: 6564 4461 7461 506f 696e 7473 275d 5d20  edDataPoints']] 
+00001600: 3d20 735b 2744 6174 6150 6f69 6e74 7327  = s['DataPoints'
+00001610: 5d0d 0a20 2020 2020 2020 2064 662e 7265  ]..        df.re
+00001620: 6e61 6d65 2863 6f6c 756d 6e73 3d7b 274c  name(columns={'L
+00001630: 6173 7427 3a27 436c 6f73 6527 7d2c 2069  ast':'Close'}, i
+00001640: 6e70 6c61 6365 3d54 7275 6529 0d0a 0d0a  nplace=True)....
+00001650: 2020 2020 2020 2020 6966 2070 7265 6d61          if prema
+00001660: 726b 6574 206f 7220 6166 7465 7268 6f75  rket or afterhou
+00001670: 7273 3a0d 0a20 2020 2020 2020 2020 2020  rs:..           
+00001680: 2064 6174 613a 2064 6963 7420 3d20 7b27   data: dict = {'
+00001690: 546f 7461 6c27 3a64 667d 0d0a 2020 2020  Total':df}..    
+000016a0: 2020 2020 2020 2020 6966 2070 7265 6d61          if prema
+000016b0: 726b 6574 3a0d 0a20 2020 2020 2020 2020  rket:..         
+000016c0: 2020 2020 2020 2064 6174 615b 2750 4d27         data['PM'
+000016d0: 5d20 3d20 6466 2e62 6574 7765 656e 5f74  ] = df.between_t
+000016e0: 696d 6528 2730 303a 3030 272c 2027 3039  ime('00:00', '09
+000016f0: 3a33 3027 290d 0a20 2020 2020 2020 2020  :30')..         
+00001700: 2020 2069 6620 6166 7465 7268 6f75 7273     if afterhours
+00001710: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00001720: 2020 2064 6174 615b 2741 4827 5d20 3d20     data['AH'] = 
+00001730: 6466 2e62 6574 7765 656e 5f74 696d 6528  df.between_time(
+00001740: 2731 363a 3030 272c 2027 3233 3a35 3927  '16:00', '23:59'
+00001750: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00001760: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00001770: 7461 203d 2064 662e 636f 7079 2829 0d0a  ta = df.copy()..
+00001780: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001790: 2064 6174 610d 0a0d 0a0d 0a20 2020 2064   data......    d
+000017a0: 6566 2067 6574 5175 6f74 6528 7365 6c66  ef getQuote(self
+000017b0: 2c20 7379 6d62 6f6c 733a 6c69 7374 293a  , symbols:list):
+000017c0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+000017d0: 2020 2020 7061 7261 6d73 3a20 6469 6374      params: dict
+000017e0: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+000017f0: 2020 2764 6961 6c65 6374 273a 2027 6f66    'dialect': 'of
+00001800: 6669 6369 616c 272c 0d0a 2020 2020 2020  ficial',..      
+00001810: 2020 2020 2020 276e 6565 6465 6427 3a20        'needed': 
+00001820: 2743 6f6d 706f 7369 7465 5472 6164 696e  'CompositeTradin
+00001830: 677c 426c 7565 6772 6173 7343 6861 6e6e  g|BluegrassChann
+00001840: 656c 7327 2c0d 0a20 2020 2020 2020 2020  els',..         
+00001850: 2020 2027 4d61 7849 6e73 7472 756d 656e     'MaxInstrumen
+00001860: 744d 6174 6368 6573 273a 2027 3127 2c0d  tMatches': '1',.
+00001870: 0a20 2020 2020 2020 2020 2020 2027 6163  .            'ac
+00001880: 6365 7074 273a 2027 6170 706c 6963 6174  cept': 'applicat
+00001890: 696f 6e2f 6a73 6f6e 272c 0d0a 2020 2020  ion/json',..    
+000018a0: 2020 2020 2020 2020 2745 6e74 6974 6c65          'Entitle
+000018b0: 6d65 6e74 546f 6b65 6e27 3a20 2763 6563  mentToken': 'cec
+000018c0: 6334 3236 3761 3031 3934 6166 3839 6361  c4267a0194af89ca
+000018d0: 3334 3338 3035 6133 6535 3761 6627 2c0d  343805a3e57af',.
+000018e0: 0a20 2020 2020 2020 2020 2020 2027 636b  .            'ck
+000018f0: 6579 273a 2027 6365 6363 3432 3637 6130  ey': 'cecc4267a0
+00001900: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001910: 2764 6961 6c65 6374 7327 3a20 2743 6861  'dialects': 'Cha
+00001920: 7274 696e 6727 2c0d 0a20 2020 2020 2020  rting',..       
+00001930: 2020 2020 2027 6964 273a 2027 2c27 2e6a       'id': ','.j
+00001940: 6f69 6e28 5b66 2753 746f 636b 2d55 532d  oin([f'Stock-US-
+00001950: 7b73 7d27 2066 6f72 2073 2069 6e20 7379  {s}' for s in sy
+00001960: 6d62 6f6c 735d 290d 0a20 2020 2020 2020  mbols])..       
+00001970: 207d 0d0a 2020 2020 2020 2020 0d0a 2020   }..        ..  
+00001980: 2020 2020 2020 6865 6164 6572 733a 2064        headers: d
+00001990: 6963 7420 3d20 7b0d 0a20 2020 2020 2020  ict = {..       
+000019a0: 2020 2020 2027 4163 6365 7074 273a 2027       'Accept': '
+000019b0: 2a2f 2a27 2c0d 0a20 2020 2020 2020 2020  */*',..         
+000019c0: 2020 2027 4163 6365 7074 2d45 6e63 6f64     'Accept-Encod
+000019d0: 696e 6727 3a20 2767 7a69 702c 2064 6566  ing': 'gzip, def
+000019e0: 6c61 7465 2c20 6272 272c 0d0a 2020 2020  late, br',..    
+000019f0: 2020 2020 2020 2020 2741 6363 6570 742d          'Accept-
+00001a00: 4c61 6e67 7561 6765 273a 2027 6573 2d45  Language': 'es-E
+00001a10: 532c 6573 3b71 3d30 2e39 2c65 6e3b 713d  S,es;q=0.9,en;q=
+00001a20: 302e 3827 2c0d 0a20 2020 2020 2020 2020  0.8',..         
+00001a30: 2020 2027 436f 6e6e 6563 7469 6f6e 273a     'Connection':
+00001a40: 2027 6b65 6570 2d61 6c69 7665 272c 0d0a   'keep-alive',..
+00001a50: 2020 2020 2020 2020 2020 2020 2748 6f73              'Hos
+00001a60: 7427 3a20 2761 7069 2e77 736a 2e6e 6574  t': 'api.wsj.net
+00001a70: 272c 0d0a 2020 2020 2020 2020 2020 2020  ',..            
+00001a80: 274f 7269 6769 6e27 3a20 2768 7474 7073  'Origin': 'https
+00001a90: 3a2f 2f77 7777 2e6d 6172 6b65 7477 6174  ://www.marketwat
+00001aa0: 6368 2e63 6f6d 272c 0d0a 2020 2020 2020  ch.com',..      
+00001ab0: 2020 2020 2020 2752 6566 6572 6572 273a        'Referer':
+00001ac0: 2066 2768 7474 7073 3a2f 2f77 7777 2e6d   f'https://www.m
+00001ad0: 6172 6b65 7477 6174 6368 2e63 6f6d 2f69  arketwatch.com/i
+00001ae0: 6e76 6573 7469 6e67 2f73 746f 636b 2f7b  nvesting/stock/{
+00001af0: 7379 6d62 6f6c 735b 305d 7d27 2c0d 0a20  symbols[0]}',.. 
+00001b00: 2020 2020 2020 207d 0d0a 0d0a 2020 2020         }....    
+00001b10: 2020 2020 7572 6c3a 2073 7472 203d 2027      url: str = '
+00001b20: 6874 7470 733a 2f2f 6170 692e 7773 6a2e  https://api.wsj.
+00001b30: 6e65 742f 6170 692f 6479 6c61 6e2f 7175  net/api/dylan/qu
+00001b40: 6f74 6573 2f76 322f 636f 6d70 2f71 756f  otes/v2/comp/quo
+00001b50: 7465 4279 4469 616c 6563 7427 0d0a 2020  teByDialect'..  
+00001b60: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00001b70: 7175 6f74 6520 3d20 7365 6c66 2e5f 7265  quote = self._re
+00001b80: 7175 6573 7428 7572 6c3d 7572 6c2c 2068  quest(url=url, h
+00001b90: 6561 6465 7273 3d68 6561 6465 7273 2c20  eaders=headers, 
+00001ba0: 7061 7261 6d73 3d70 6172 616d 7329 0d0a  params=params)..
+00001bb0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00001bc0: 2020 7265 7475 726e 2071 756f 7465 0d0a    return quote..
+00001bd0: 0d0a 2020 2020 6465 6620 6765 7450 7265  ..    def getPre
+00001be0: 6d61 726b 6574 2873 656c 6629 202d 3e20  market(self) -> 
+00001bf0: 6469 6374 3a0d 0a0d 0a20 2020 2020 2020  dict:....       
+00001c00: 2068 6561 6465 7273 3a20 6469 6374 203d   headers: dict =
+00001c10: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001c20: 274f 7269 6769 6e27 3a20 2768 7474 7073  'Origin': 'https
+00001c30: 3a2f 2f77 7777 2e6d 6172 6b65 7477 6174  ://www.marketwat
+00001c40: 6368 2e63 6f6d 272c 0d0a 2020 2020 2020  ch.com',..      
+00001c50: 2020 7d0d 0a20 2020 2020 2020 2075 726c    }..        url
+00001c60: 3a20 7374 7220 3d20 2768 7474 7073 3a2f  : str = 'https:/
+00001c70: 2f77 7777 2e6d 6172 6b65 7477 6174 6368  /www.marketwatch
+00001c80: 2e63 6f6d 2f74 6f6f 6c73 2f73 6372 6565  .com/tools/scree
+00001c90: 6e65 722f 7072 656d 6172 6b65 7427 0d0a  ner/premarket'..
+00001ca0: 0d0a 2020 2020 2020 2020 723a 2072 6571  ..        r: req
+00001cb0: 7565 7374 732e 5265 7370 6f6e 7365 203d  uests.Response =
+00001cc0: 2073 656c 662e 5f72 6571 7565 7374 2875   self._request(u
+00001cd0: 726c 3d75 726c 2c20 6865 6164 6572 733d  rl=url, headers=
+00001ce0: 6865 6164 6572 732c 206a 736f 6e3d 4661  headers, json=Fa
+00001cf0: 6c73 6529 0d0a 2020 2020 2020 2020 6874  lse)..        ht
+00001d00: 6d6c 3a20 4265 6175 7469 6675 6c53 6f75  ml: BeautifulSou
+00001d10: 7020 3d20 4265 6175 7469 6675 6c53 6f75  p = BeautifulSou
+00001d20: 7028 722e 7465 7874 2c20 2768 746d 6c2e  p(r.text, 'html.
+00001d30: 7061 7273 6572 2729 0d0a 0d0a 2020 2020  parser')....    
+00001d40: 2020 2020 7461 626c 6573 3a20 7365 7420      tables: set 
+00001d50: 3d20 6874 6d6c 2e66 696e 645f 616c 6c28  = html.find_all(
+00001d60: 2774 6162 6c65 2720 2c7b 2763 6c61 7373  'table' ,{'class
+00001d70: 273a 2774 6162 6c65 2074 6162 6c65 2d2d  ':'table table--
+00001d80: 6f76 6572 666c 6f77 2061 6c69 676e 2d2d  overflow align--
+00001d90: 7269 6768 7427 7d29 0d0a 0d0a 2020 2020  right'})....    
+00001da0: 2020 2020 6466 733a 206c 6973 7420 3d20      dfs: list = 
+00001db0: 5b5d 0d0a 2020 2020 2020 2020 666f 7220  []..        for 
+00001dc0: 7461 626c 6520 696e 2074 6162 6c65 733a  table in tables:
+00001dd0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+00001de0: 6c75 6d6e 733a 206c 6973 7420 3d20 5b5b  lumns: list = [[
+00001df0: 6320 666f 7220 6320 696e 2069 2e63 6f6e  c for c in i.con
+00001e00: 7465 6e74 7320 6966 2063 2021 3d20 275c  tents if c != '\
+00001e10: 6e27 5d5b 305d 2e67 6574 5f74 6578 7428  n'][0].get_text(
+00001e20: 2920 666f 7220 6920 696e 2074 6162 6c65  ) for i in table
+00001e30: 2e66 696e 645f 616c 6c28 2774 6827 295d  .find_all('th')]
+00001e40: 0d0a 2020 2020 2020 2020 2020 2020 6461  ..            da
+00001e50: 7461 3a20 6c69 7374 203d 205b 5b63 656c  ta: list = [[cel
+00001e60: 6c2e 6765 745f 7465 7874 2829 2e72 6570  l.get_text().rep
+00001e70: 6c61 6365 2827 5c6e 272c 2027 2729 2066  lace('\n', '') f
+00001e80: 6f72 2063 656c 6c20 696e 2072 6f77 2e66  or cell in row.f
+00001e90: 696e 645f 616c 6c28 2774 6427 295d 205c  ind_all('td')] \
+00001ea0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001eb0: 2020 2020 2020 666f 7220 726f 7720 696e        for row in
+00001ec0: 2074 6162 6c65 2e66 696e 645f 616c 6c28   table.find_all(
+00001ed0: 2774 7227 295d 5b31 3a5d 0d0a 2020 2020  'tr')][1:]..    
+00001ee0: 2020 2020 2020 2020 6466 3a20 7064 2e44          df: pd.D
+00001ef0: 6174 6146 7261 6d65 203d 2070 642e 4461  ataFrame = pd.Da
+00001f00: 7461 4672 616d 6528 636f 6c75 6d6e 733d  taFrame(columns=
+00001f10: 636f 6c75 6d6e 732c 2064 6174 613d 6461  columns, data=da
+00001f20: 7461 290d 0a20 2020 2020 2020 2020 2020  ta)..           
+00001f30: 2064 665b 2753 796d 626f 6c27 5d20 3d20   df['Symbol'] = 
+00001f40: 6466 5b27 5379 6d62 6f6c 275d 2e61 7070  df['Symbol'].app
+00001f50: 6c79 286c 616d 6264 6120 783a 2078 5b3a  ly(lambda x: x[:
+00001f60: 696e 7428 6c65 6e28 7829 2f32 295d 290d  int(len(x)/2)]).
+00001f70: 0a20 2020 2020 2020 2020 2020 2064 6673  .            dfs
+00001f80: 2e61 7070 656e 6428 6466 290d 0a20 2020  .append(df)..   
+00001f90: 2020 2020 2064 6673 3a20 6469 6374 203d       dfs: dict =
+00001fa0: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00001fb0: 2747 6169 6e65 7273 273a 2064 6673 5b30  'Gainers': dfs[0
+00001fc0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00001fd0: 274c 6f73 6572 7327 3a20 6466 735b 315d  'Losers': dfs[1]
+00001fe0: 2c0d 0a20 2020 2020 2020 2020 2020 2027  ,..            '
+00001ff0: 4163 7469 7665 273a 2064 6673 5b32 5d0d  Active': dfs[2].
+00002000: 0a20 2020 2020 2020 207d 0d0a 0d0a 2020  .        }....  
+00002010: 2020 2020 2020 7265 7475 726e 2064 6673        return dfs
+00002020: 0d0a 2020 2020 0d0a 2020 2020 0d0a 0d0a  ..    ..    ....
+00002030: 6966 205f 5f6e 616d 655f 5f20 3d3d 2027  if __name__ == '
+00002040: 5f5f 6d61 696e 5f5f 273a 0d0a 0d0a 2020  __main__':....  
+00002050: 2020 6d77 203d 204d 6172 6b65 7457 6174    mw = MarketWat
+00002060: 6368 2829 0d0a 2020 2020 7072 656d 6172  ch()..    premar
+00002070: 6b65 7420 3d20 6d77 2e67 6574 5072 656d  ket = mw.getPrem
+00002080: 6172 6b65 7428 29                        arket()
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/oecd.py` & `omtf-1.0.3/OMTF/DataProviders/oecd.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/openstreetmap.py` & `omtf-1.0.3/OMTF/DataProviders/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/polygon.py` & `omtf-1.0.3/OMTF/DataProviders/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import time
 import requests
 import pandas as pd
 
-from data import DataProvider
+from .data import DataProvider
 
 class Polygon(DataProvider):
 
     BASE_URL: str = 'https://api.polygon.io'
 
     def __init__(self,api_key:str='cUlHULSDVdLm9Up1TsKxF3RU2dEKm3nq', 
                  free:bool=False) -> None:
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/sec.py` & `omtf-1.0.3/OMTF/DataProviders/sec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os
 import requests
 import time
 import pandas as pd
 
-from data import DataProvider
+from .data import DataProvider
 
 
 class SEC(DataProvider):
 
     BASE_URL: str = 'https://www.sec.gov'
     DATA_URL: str = 'https://data.sec.gov'
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/tradingterminal.py` & `omtf-1.0.3/OMTF/DataProviders/tradingterminal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import numpy as np
 import pandas as pd
 
 import requests
 
-from data import DataProvider
+from .data import DataProvider
 
 url = 'https://api.tradingterminal.com/v1/overview/marketSummary?stock=SPY,QQQ,DIA,IWM&crypto=BTCUSD' # Close data
 url = 'https://api.tradingterminal.com/v1/overview/callratio?exchanges=AMEX,NYSE,NASDAQ,CBOE' # Pull/Call ratio
 
 url = 'https://api.tradingterminal.com/v1/fmp/CompanyQuote?ticker=AAPL,CLUSD,BZUSD,NGUSD,GCUSD,SIUSD,PLUSD,HGUSD,LBUSD,EURUSD' # Quote
 url = 'https://api.tradingterminal.com/v1/fmp/HolidaysAndTradingHours' # Calendar
 url = 'https://api.tradingterminal.com/v1/fmp/EarningsCalendarConfirmed?startDate=2023-04-30&endDate=2023-05-06' # Earnings calendar
```

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/worldBank.py` & `omtf-1.0.3/OMTF/DataProviders/worldBank.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/worldHealthOrg.py` & `omtf-1.0.3/OMTF/DataProviders/worldHealthOrg.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/world_population.py` & `omtf-1.0.3/OMTF/DataProviders/world_population.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/DataProviders/yahoo.py` & `omtf-1.0.3/OMTF/DataProviders/yahoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import enum
 
 import requests
 from bs4 import BeautifulSoup
 
-from data import DataProvider
+from .data import DataProvider
 
 class YahooFinance(DataProvider):
 
     class Method(enum.Enum):
         GET: str = 'GET'
         POST: str = 'POST'
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/00_models_comparison.py` & `omtf-1.0.3/OMTF/MachineLearning/00_models_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 
 import math
 import numpy as np
 import pandas as pd
 
-import utils
-from linear_regression import LinearRegression
-from logistic_regression import LogisticRegression
-from kmeans_clustering import Kmeans
-from decision_trees import DecisionTreeClassifier
-from random_forest import RandomForest
-from k_nearest_neighbors import KNN
-from principal_component import PCA
-from support_vector import SupportVectorMachine
-from naive_bayes import NaiveBayes
-from neural_networks import NeuralNetwork
-from long_short_term_memory import LSTM
+from . import utils
+from .linear_regression import LinearRegression
+from .logistic_regression import LogisticRegression
+from .kmeans_clustering import Kmeans
+from .decision_trees import DecisionTreeClassifier
+from .random_forest import RandomForest
+from .k_nearest_neighbors import KNN
+from .principal_component import PCA
+from .support_vector import SupportVectorMachine
+from .naive_bayes import NaiveBayes
+from .neural_networks import NeuralNetwork
+from .long_short_term_memory import LSTM
 
 import yfinance as yf
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
 def getData(ticker:str) -> pd.DataFrame:
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/RandomForest.py` & `omtf-1.0.3/OMTF/MachineLearning/RandomForest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import math
 import numpy as np
 
-from gradientboosting import DecisionTree, RegressionTree
+from .gradientboosting import DecisionTree, RegressionTree
 
 class RandomForest:
 
     """    Random forest common class.    """
 
     def __init__(self, trees:list[(DecisionTree | RegressionTree)], n_trees:int,
                  prediction_aggrigation_calculation, max_feature:int=None) -> None:
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/decision_trees.py` & `omtf-1.0.3/OMTF/MachineLearning/decision_trees.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 
 class Node():
     
     #From: https://www.kaggle.com/code/fareselmenshawii/decision-tree-from-scratch?scriptVersionId=130941860
     
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/genetic_algorithm.py` & `omtf-1.0.3/OMTF/MachineLearning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/gradientboosting.py` & `omtf-1.0.3/OMTF/MachineLearning/gradientboosting.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/k_nearest_neighbors.py` & `omtf-1.0.3/OMTF/MachineLearning/k_nearest_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 class KNN:
     
     # From: https://www.kaggle.com/code/fareselmenshawii/knn-from-scratch
     
     """
     K-Nearest Neighbors (KNN) classification algorithm
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/kmeans_clustering.py` & `omtf-1.0.3/OMTF/MachineLearning/kmeans_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 class Kmeans:
 
     # From: https://www.kaggle.com/code/fareselmenshawii/kmeans-from-scratch
 
     """
     K-Means clustering algorithm implementation.
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/linear_regression.py` & `omtf-1.0.3/OMTF/MachineLearning/linear_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
-import utils
+from . import utils
 
 
 class LinearRegression:
     
     # From: https://www.kaggle.com/code/fareselmenshawii/linear-regression-from-scratch
 
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/logistic_regression.py` & `omtf-1.0.3/OMTF/MachineLearning/logistic_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,1004 +1,1004 @@
 00000000: 0d0a 696d 706f 7274 2070 6963 6b6c 650d  ..import pickle.
 00000010: 0a69 6d70 6f72 7420 6e75 6d70 7920 6173  .import numpy as
 00000020: 206e 700d 0a69 6d70 6f72 7420 7061 6e64   np..import pand
 00000030: 6173 2061 7320 7064 0d0a 696d 706f 7274  as as pd..import
 00000040: 2070 6c6f 746c 792e 6578 7072 6573 7320   plotly.express 
-00000050: 6173 2070 780d 0a0d 0a69 6d70 6f72 7420  as px....import 
-00000060: 7574 696c 730d 0a0d 0a63 6c61 7373 204c  utils....class L
-00000070: 6f67 6973 7469 6352 6567 7265 7373 696f  ogisticRegressio
-00000080: 6e3a 0d0a 2020 2020 0d0a 2020 2020 2320  n:..    ..    # 
-00000090: 4672 6f6d 3a20 6874 7470 733a 2f2f 7777  From: https://ww
-000000a0: 772e 6b61 6767 6c65 2e63 6f6d 2f63 6f64  w.kaggle.com/cod
-000000b0: 652f 6661 7265 7365 6c6d 656e 7368 6177  e/fareselmenshaw
-000000c0: 6969 2f6c 6f67 6973 7469 632d 7265 6772  ii/logistic-regr
-000000d0: 6573 7369 6f6e 2d66 726f 6d2d 7363 7261  ession-from-scra
-000000e0: 7463 680d 0a20 2020 200d 0a20 2020 2027  tch..    ..    '
-000000f0: 2727 0d0a 2020 2020 4c6f 6769 7374 6963  ''..    Logistic
-00000100: 2052 6567 7265 7373 696f 6e20 6d6f 6465   Regression mode
-00000110: 6c2e 0d0a 2020 2020 0d0a 2020 2020 4c6f  l...    ..    Lo
-00000120: 6769 7374 6963 2072 6567 7265 7373 696f  gistic regressio
-00000130: 6e20 6973 2061 2077 6964 656c 7920 7573  n is a widely us
-00000140: 6564 206d 6f64 656c 2069 6e20 6d61 6368  ed model in mach
-00000150: 696e 6520 6c65 6172 6e69 6e67 2066 6f72  ine learning for
-00000160: 2062 696e 6172 7920 0d0a 2020 2020 636c   binary ..    cl
-00000170: 6173 7369 6669 6361 7469 6f6e 2074 6173  assification tas
-00000180: 6b73 2e20 4974 206d 6f64 656c 7320 7468  ks. It models th
-00000190: 6520 7072 6f62 6162 696c 6974 7920 7468  e probability th
-000001a0: 6174 2061 2067 6976 656e 2069 6e70 7574  at a given input
-000001b0: 2062 656c 6f6e 6773 200d 0a20 2020 2074   belongs ..    t
-000001c0: 6f20 6120 7061 7274 6963 756c 6172 2063  o a particular c
-000001d0: 6c61 7373 2e20 0d0a 0d0a 2020 2020 5061  lass. ....    Pa
-000001e0: 7261 6d65 7465 7273 0d0a 2020 2020 2d2d  rameters..    --
-000001f0: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 6c65  --------..    le
-00000200: 6172 6e69 6e67 5f72 6174 653a 2066 6c6f  arning_rate: flo
-00000210: 6174 0d0a 2020 2020 2020 2020 4c65 6172  at..        Lear
-00000220: 6e69 6e67 2072 6174 6520 666f 7220 7468  ning rate for th
-00000230: 6520 6d6f 6465 6c2e 0d0a 0d0a 2020 2020  e model.....    
-00000240: 4d65 7468 6f64 730d 0a20 2020 202d 2d2d  Methods..    ---
-00000250: 2d2d 2d2d 0d0a 2020 2020 696e 6974 6961  ----..    initia
-00000260: 6c69 7a65 5f70 6172 616d 6574 6572 2829  lize_parameter()
-00000270: 3a20 496e 6974 6961 6c69 7a65 7320 7468  : Initializes th
-00000280: 6520 7061 7261 6d65 7465 7273 206f 6620  e parameters of 
-00000290: 7468 6520 6d6f 6465 6c2e 0d0a 2020 2020  the model...    
-000002a0: 7369 676d 6f69 6428 7a29 3a20 436f 6d70  sigmoid(z): Comp
-000002b0: 7574 6573 2074 6865 2073 6967 6d6f 6964  utes the sigmoid
-000002c0: 2061 6374 6976 6174 696f 6e20 6675 6e63   activation func
-000002d0: 7469 6f6e 2066 6f72 2067 6976 656e 2069  tion for given i
-000002e0: 6e70 7574 207a 2e0d 0a20 2020 2066 6f72  nput z...    for
-000002f0: 7761 7264 2858 293a 2043 6f6d 7075 7465  ward(X): Compute
-00000300: 7320 666f 7277 6172 6420 7072 6f70 6167  s forward propag
-00000310: 6174 696f 6e20 666f 7220 6769 7665 6e20  ation for given 
-00000320: 696e 7075 7420 582e 0d0a 2020 2020 636f  input X...    co
-00000330: 6d70 7574 655f 636f 7374 2870 7265 6469  mpute_cost(predi
-00000340: 6374 696f 6e73 293a 2043 6f6d 7075 7465  ctions): Compute
-00000350: 7320 7468 6520 636f 7374 2066 756e 6374  s the cost funct
-00000360: 696f 6e20 666f 7220 6769 7665 6e20 7072  ion for given pr
-00000370: 6564 6963 7469 6f6e 732e 0d0a 2020 2020  edictions...    
-00000380: 636f 6d70 7574 655f 6772 6164 6965 6e74  compute_gradient
-00000390: 2870 7265 6469 6374 696f 6e73 293a 2043  (predictions): C
-000003a0: 6f6d 7075 7465 7320 7468 6520 6772 6164  omputes the grad
-000003b0: 6965 6e74 7320 666f 7220 7468 6520 6d6f  ients for the mo
-000003c0: 6465 6c20 7573 696e 6720 6769 7665 6e20  del using given 
-000003d0: 7072 6564 6963 7469 6f6e 732e 0d0a 2020  predictions...  
-000003e0: 2020 6669 7428 582c 2079 2c20 6974 6572    fit(X, y, iter
-000003f0: 6174 696f 6e73 2c20 706c 6f74 5f63 6f73  ations, plot_cos
-00000400: 7429 3a20 5472 6169 6e73 2074 6865 206d  t): Trains the m
-00000410: 6f64 656c 206f 6e20 6769 7665 6e20 696e  odel on given in
-00000420: 7075 7420 5820 616e 6420 6c61 6265 6c73  put X and labels
-00000430: 2079 2066 6f72 2073 7065 6369 6669 6564   y for specified
-00000440: 2069 7465 7261 7469 6f6e 732e 0d0a 2020   iterations...  
-00000450: 2020 7072 6564 6963 7428 5829 3a20 5072    predict(X): Pr
-00000460: 6564 6963 7473 2074 6865 206c 6162 656c  edicts the label
-00000470: 7320 666f 7220 6769 7665 6e20 696e 7075  s for given inpu
-00000480: 7420 582e 0d0a 2020 2020 2727 270d 0a0d  t X...    '''...
-00000490: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-000004a0: 5f28 7365 6c66 2c20 6c65 6172 6e69 6e67  _(self, learning
-000004b0: 5f72 6174 653a 666c 6f61 743d 302e 3030  _rate:float=0.00
-000004c0: 3031 2c20 636f 6e76 6572 6765 6e63 655f  01, convergence_
-000004d0: 746f 6c3a 666c 6f61 743d 302e 3030 3030  tol:float=0.0000
-000004e0: 3030 3030 3030 3129 202d 3e20 4e6f 6e65  0000001) -> None
-000004f0: 3a0d 0a20 2020 2020 2020 200d 0a20 2020  :..        ..   
-00000500: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-00000510: 2020 436f 6e73 7472 7563 746f 7220 6d65    Constructor me
-00000520: 7468 6f64 2074 6861 7420 696e 6974 6961  thod that initia
-00000530: 6c69 7a65 7320 7468 6520 4c6f 6769 7374  lizes the Logist
-00000540: 6963 5265 6772 6573 7369 6f6e 206f 626a  icRegression obj
-00000550: 6563 742e 0d0a 0d0a 2020 2020 2020 2020  ect.....        
-00000560: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00000570: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00000580: 2020 2020 2020 2020 6c65 6172 6e69 6e67          learning
-00000590: 5f72 6174 6520 3a20 666c 6f61 740d 0a20  _rate : float.. 
-000005a0: 2020 2020 2020 2020 2020 2054 6865 206c             The l
-000005b0: 6561 726e 696e 6720 7261 7465 2075 7365  earning rate use
-000005c0: 6420 696e 2067 7261 6469 656e 7420 6465  d in gradient de
-000005d0: 7363 656e 742e 2044 6566 756c 7473 2074  scent. Defults t
-000005e0: 6f20 302e 3030 3031 2e0d 0a20 2020 2020  o 0.0001...     
-000005f0: 2020 2063 6f6e 7665 7267 656e 6365 5f74     convergence_t
-00000600: 6f6c 3a20 666c 6f61 740d 0a20 2020 2020  ol: float..     
-00000610: 2020 2020 2020 2054 6865 2074 6f6c 6572         The toler
-00000620: 616e 6365 2066 6f72 2063 6f6e 7665 7267  ance for converg
-00000630: 656e 6365 2028 7374 6f70 7069 6e67 2063  ence (stopping c
-00000640: 7269 7465 7269 6f6e 292e 2044 6566 6175  riterion). Defau
-00000650: 6c74 7320 746f 2030 2e30 3030 3030 3030  lts to 0.0000000
-00000660: 3030 3031 2e0d 0a20 2020 2020 2020 2027  0001...        '
-00000670: 2727 0d0a 2020 2020 2020 2020 0d0a 2020  ''..        ..  
-00000680: 2020 2020 2020 6e70 2e72 616e 646f 6d2e        np.random.
-00000690: 7365 6564 2831 290d 0a20 2020 2020 2020  seed(1)..       
-000006a0: 2073 656c 662e 6c65 6172 6e69 6e67 5f72   self.learning_r
-000006b0: 6174 6520 3d20 6c65 6172 6e69 6e67 5f72  ate = learning_r
-000006c0: 6174 650d 0a20 2020 2020 2020 2073 656c  ate..        sel
-000006d0: 662e 636f 6e76 6572 6765 6e63 655f 746f  f.convergence_to
-000006e0: 6c20 3d20 636f 6e76 6572 6765 6e63 655f  l = convergence_
-000006f0: 746f 6c0d 0a0d 0a20 2020 2064 6566 2069  tol....    def i
-00000700: 6e69 7469 616c 697a 655f 7061 7261 6d65  nitialize_parame
-00000710: 7465 7228 7365 6c66 2920 2d3e 204e 6f6e  ter(self) -> Non
-00000720: 653a 0d0a 2020 2020 2020 2020 0d0a 2020  e:..        ..  
-00000730: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-00000740: 2020 2049 6e69 7469 616c 697a 6573 2074     Initializes t
-00000750: 6865 2070 6172 616d 6574 6572 7320 6f66  he parameters of
-00000760: 2074 6865 206d 6f64 656c 2e0d 0a20 2020   the model...   
-00000770: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
-00000780: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
-00000790: 2e57 203d 206e 702e 7a65 726f 7328 7365  .W = np.zeros(se
-000007a0: 6c66 2e58 2e73 6861 7065 5b31 5d29 0d0a  lf.X.shape[1])..
-000007b0: 2020 2020 2020 2020 7365 6c66 2e62 203d          self.b =
-000007c0: 2030 2e30 0d0a 0d0a 2020 2020 6465 6620   0.0....    def 
-000007d0: 666f 7277 6172 6428 7365 6c66 2c20 583a  forward(self, X:
-000007e0: 6e70 2e6e 6461 7272 6179 2920 2d3e 2028  np.ndarray) -> (
-000007f0: 6e70 2e6e 6461 7272 6179 293a 0d0a 0d0a  np.ndarray):....
-00000800: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-00000810: 2020 2020 2043 6f6d 7075 7465 2074 6865       Compute the
-00000820: 2066 6f72 7761 7264 2070 726f 7061 6761   forward propaga
-00000830: 7469 6f6e 2066 6f72 2067 6976 656e 2069  tion for given i
-00000840: 6e70 7574 2058 2e0d 0a0d 0a20 2020 2020  nput X.....     
-00000850: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
-00000860: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
-00000870: 2d0d 0a20 2020 2020 2020 2058 3a20 6e70  -..        X: np
-00000880: 2e6e 6461 7272 6179 0d0a 2020 2020 2020  .ndarray..      
-00000890: 2020 2020 2020 496e 7075 7420 6461 7461        Input data
-000008a0: 206f 6620 7368 6170 6520 286d 2c20 6e5f   of shape (m, n_
-000008b0: 6665 6174 7572 6573 292e 0d0a 0d0a 2020  features).....  
-000008c0: 2020 2020 2020 5265 7475 726e 730d 0a20        Returns.. 
-000008d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0d0a         -------..
-000008e0: 2020 2020 2020 2020 7265 7475 726e 3a20          return: 
-000008f0: 6e70 2e6e 6461 7272 6179 0d0a 2020 2020  np.ndarray..    
-00000900: 2020 2020 2020 2020 4f75 7470 7574 2064          Output d
-00000910: 6174 6120 6f66 2073 6861 7065 2028 6d2c  ata of shape (m,
-00000920: 292e 0d0a 2020 2020 2020 2020 2727 270d  )...        '''.
-00000930: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-00000940: 2020 2023 2070 7269 6e74 2858 2e73 6861     # print(X.sha
-00000950: 7065 2c20 7365 6c66 2e57 2e73 6861 7065  pe, self.W.shape
-00000960: 290d 0a20 2020 2020 2020 205a 203d 206e  )..        Z = n
-00000970: 702e 6d61 746d 756c 2858 2c20 7365 6c66  p.matmul(X, self
-00000980: 2e57 2920 2b20 7365 6c66 2e62 0d0a 2020  .W) + self.b..  
-00000990: 2020 2020 2020 412c 2063 6163 6865 203d        A, cache =
-000009a0: 2075 7469 6c73 2e73 6967 6d6f 6964 285a   utils.sigmoid(Z
-000009b0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-000009c0: 2020 2020 2072 6574 7572 6e20 410d 0a0d       return A...
-000009d0: 0a20 2020 2064 6566 2063 6f6d 7075 7465  .    def compute
-000009e0: 5f63 6f73 7428 7365 6c66 2c20 7072 6564  _cost(self, pred
-000009f0: 6963 7469 6f6e 733a 6e70 2e6e 6461 7272  ictions:np.ndarr
-00000a00: 6179 2920 2d3e 2066 6c6f 6174 3a0d 0a20  ay) -> float:.. 
-00000a10: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00000a20: 2027 2727 0d0a 2020 2020 2020 2020 436f   '''..        Co
-00000a30: 6d70 7574 6573 2074 6865 2063 6f73 7420  mputes the cost 
-00000a40: 6675 6e63 7469 6f6e 2066 6f72 2067 6976  function for giv
-00000a50: 656e 2070 7265 6469 6374 696f 6e73 2e0d  en predictions..
-00000a60: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-00000a70: 6574 6572 730d 0a20 2020 2020 2020 202d  eters..        -
-00000a80: 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020  ---------..     
-00000a90: 2020 2070 7265 6469 6374 696f 6e73 3a20     predictions: 
-00000aa0: 6e70 2e6e 6461 7272 6179 0d0a 2020 2020  np.ndarray..    
-00000ab0: 2020 2020 2020 2020 5072 6564 6963 7469          Predicti
-00000ac0: 6f6e 7320 6f66 2073 6861 7065 2028 6d2c  ons of shape (m,
-00000ad0: 292e 0d0a 0d0a 2020 2020 2020 2020 5265  ).....        Re
-00000ae0: 7475 726e 730d 0a20 2020 2020 2020 202d  turns..        -
-00000af0: 2d2d 2d2d 2d2d 0d0a 2020 2020 2020 2020  ------..        
-00000b00: 7265 7475 726e 3a20 666c 6f61 740d 0a20  return: float.. 
-00000b10: 2020 2020 2020 2020 2020 2043 6f73 7420             Cost 
-00000b20: 6f66 2074 6865 206d 6f64 656c 2e0d 0a20  of the model... 
-00000b30: 2020 2020 2020 2027 2727 0d0a 2020 2020         '''..    
-00000b40: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
-00000b50: 636f 6d70 7574 6520 7468 6520 636f 7374  compute the cost
-00000b60: 0d0a 2020 2020 2020 2020 636f 7374 203d  ..        cost =
-00000b70: 206e 702e 7375 6d28 282d 6e70 2e6c 6f67   np.sum((-np.log
-00000b80: 2870 7265 6469 6374 696f 6e73 202b 2031  (predictions + 1
-00000b90: 652d 3829 202a 2073 656c 662e 7929 202b  e-8) * self.y) +
-00000ba0: 2028 2d6e 702e 6c6f 6728 3120 2d20 7072   (-np.log(1 - pr
-00000bb0: 6564 6963 7469 6f6e 7320 2b20 3165 2d38  edictions + 1e-8
-00000bc0: 2929 202a 205c 0d0a 2020 2020 2020 2020  )) * \..        
+00000050: 6173 2070 780d 0a0d 0a66 726f 6d20 2e20  as px....from . 
+00000060: 696d 706f 7274 2075 7469 6c73 0d0a 0d0a  import utils....
+00000070: 636c 6173 7320 4c6f 6769 7374 6963 5265  class LogisticRe
+00000080: 6772 6573 7369 6f6e 3a0d 0a20 2020 200d  gression:..    .
+00000090: 0a20 2020 2023 2046 726f 6d3a 2068 7474  .    # From: htt
+000000a0: 7073 3a2f 2f77 7777 2e6b 6167 676c 652e  ps://www.kaggle.
+000000b0: 636f 6d2f 636f 6465 2f66 6172 6573 656c  com/code/faresel
+000000c0: 6d65 6e73 6861 7769 692f 6c6f 6769 7374  menshawii/logist
+000000d0: 6963 2d72 6567 7265 7373 696f 6e2d 6672  ic-regression-fr
+000000e0: 6f6d 2d73 6372 6174 6368 0d0a 2020 2020  om-scratch..    
+000000f0: 0d0a 2020 2020 2727 270d 0a20 2020 204c  ..    '''..    L
+00000100: 6f67 6973 7469 6320 5265 6772 6573 7369  ogistic Regressi
+00000110: 6f6e 206d 6f64 656c 2e0d 0a20 2020 200d  on model...    .
+00000120: 0a20 2020 204c 6f67 6973 7469 6320 7265  .    Logistic re
+00000130: 6772 6573 7369 6f6e 2069 7320 6120 7769  gression is a wi
+00000140: 6465 6c79 2075 7365 6420 6d6f 6465 6c20  dely used model 
+00000150: 696e 206d 6163 6869 6e65 206c 6561 726e  in machine learn
+00000160: 696e 6720 666f 7220 6269 6e61 7279 200d  ing for binary .
+00000170: 0a20 2020 2063 6c61 7373 6966 6963 6174  .    classificat
+00000180: 696f 6e20 7461 736b 732e 2049 7420 6d6f  ion tasks. It mo
+00000190: 6465 6c73 2074 6865 2070 726f 6261 6269  dels the probabi
+000001a0: 6c69 7479 2074 6861 7420 6120 6769 7665  lity that a give
+000001b0: 6e20 696e 7075 7420 6265 6c6f 6e67 7320  n input belongs 
+000001c0: 0d0a 2020 2020 746f 2061 2070 6172 7469  ..    to a parti
+000001d0: 6375 6c61 7220 636c 6173 732e 200d 0a0d  cular class. ...
+000001e0: 0a20 2020 2050 6172 616d 6574 6572 730d  .    Parameters.
+000001f0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d  .    ----------.
+00000200: 0a20 2020 206c 6561 726e 696e 675f 7261  .    learning_ra
+00000210: 7465 3a20 666c 6f61 740d 0a20 2020 2020  te: float..     
+00000220: 2020 204c 6561 726e 696e 6720 7261 7465     Learning rate
+00000230: 2066 6f72 2074 6865 206d 6f64 656c 2e0d   for the model..
+00000240: 0a0d 0a20 2020 204d 6574 686f 6473 0d0a  ...    Methods..
+00000250: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00000260: 2069 6e69 7469 616c 697a 655f 7061 7261   initialize_para
+00000270: 6d65 7465 7228 293a 2049 6e69 7469 616c  meter(): Initial
+00000280: 697a 6573 2074 6865 2070 6172 616d 6574  izes the paramet
+00000290: 6572 7320 6f66 2074 6865 206d 6f64 656c  ers of the model
+000002a0: 2e0d 0a20 2020 2073 6967 6d6f 6964 287a  ...    sigmoid(z
+000002b0: 293a 2043 6f6d 7075 7465 7320 7468 6520  ): Computes the 
+000002c0: 7369 676d 6f69 6420 6163 7469 7661 7469  sigmoid activati
+000002d0: 6f6e 2066 756e 6374 696f 6e20 666f 7220  on function for 
+000002e0: 6769 7665 6e20 696e 7075 7420 7a2e 0d0a  given input z...
+000002f0: 2020 2020 666f 7277 6172 6428 5829 3a20      forward(X): 
+00000300: 436f 6d70 7574 6573 2066 6f72 7761 7264  Computes forward
+00000310: 2070 726f 7061 6761 7469 6f6e 2066 6f72   propagation for
+00000320: 2067 6976 656e 2069 6e70 7574 2058 2e0d   given input X..
+00000330: 0a20 2020 2063 6f6d 7075 7465 5f63 6f73  .    compute_cos
+00000340: 7428 7072 6564 6963 7469 6f6e 7329 3a20  t(predictions): 
+00000350: 436f 6d70 7574 6573 2074 6865 2063 6f73  Computes the cos
+00000360: 7420 6675 6e63 7469 6f6e 2066 6f72 2067  t function for g
+00000370: 6976 656e 2070 7265 6469 6374 696f 6e73  iven predictions
+00000380: 2e0d 0a20 2020 2063 6f6d 7075 7465 5f67  ...    compute_g
+00000390: 7261 6469 656e 7428 7072 6564 6963 7469  radient(predicti
+000003a0: 6f6e 7329 3a20 436f 6d70 7574 6573 2074  ons): Computes t
+000003b0: 6865 2067 7261 6469 656e 7473 2066 6f72  he gradients for
+000003c0: 2074 6865 206d 6f64 656c 2075 7369 6e67   the model using
+000003d0: 2067 6976 656e 2070 7265 6469 6374 696f   given predictio
+000003e0: 6e73 2e0d 0a20 2020 2066 6974 2858 2c20  ns...    fit(X, 
+000003f0: 792c 2069 7465 7261 7469 6f6e 732c 2070  y, iterations, p
+00000400: 6c6f 745f 636f 7374 293a 2054 7261 696e  lot_cost): Train
+00000410: 7320 7468 6520 6d6f 6465 6c20 6f6e 2067  s the model on g
+00000420: 6976 656e 2069 6e70 7574 2058 2061 6e64  iven input X and
+00000430: 206c 6162 656c 7320 7920 666f 7220 7370   labels y for sp
+00000440: 6563 6966 6965 6420 6974 6572 6174 696f  ecified iteratio
+00000450: 6e73 2e0d 0a20 2020 2070 7265 6469 6374  ns...    predict
+00000460: 2858 293a 2050 7265 6469 6374 7320 7468  (X): Predicts th
+00000470: 6520 6c61 6265 6c73 2066 6f72 2067 6976  e labels for giv
+00000480: 656e 2069 6e70 7574 2058 2e0d 0a20 2020  en input X...   
+00000490: 2027 2727 0d0a 0d0a 2020 2020 6465 6620   '''....    def 
+000004a0: 5f5f 696e 6974 5f5f 2873 656c 662c 206c  __init__(self, l
+000004b0: 6561 726e 696e 675f 7261 7465 3a66 6c6f  earning_rate:flo
+000004c0: 6174 3d30 2e30 3030 312c 2063 6f6e 7665  at=0.0001, conve
+000004d0: 7267 656e 6365 5f74 6f6c 3a66 6c6f 6174  rgence_tol:float
+000004e0: 3d30 2e30 3030 3030 3030 3030 3031 2920  =0.00000000001) 
+000004f0: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
+00000500: 2020 0d0a 2020 2020 2020 2020 2727 270d    ..        '''.
+00000510: 0a20 2020 2020 2020 2043 6f6e 7374 7275  .        Constru
+00000520: 6374 6f72 206d 6574 686f 6420 7468 6174  ctor method that
+00000530: 2069 6e69 7469 616c 697a 6573 2074 6865   initializes the
+00000540: 204c 6f67 6973 7469 6352 6567 7265 7373   LogisticRegress
+00000550: 696f 6e20 6f62 6a65 6374 2e0d 0a0d 0a20  ion object..... 
+00000560: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00000570: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00000580: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 206c  -----..        l
+00000590: 6561 726e 696e 675f 7261 7465 203a 2066  earning_rate : f
+000005a0: 6c6f 6174 0d0a 2020 2020 2020 2020 2020  loat..          
+000005b0: 2020 5468 6520 6c65 6172 6e69 6e67 2072    The learning r
+000005c0: 6174 6520 7573 6564 2069 6e20 6772 6164  ate used in grad
+000005d0: 6965 6e74 2064 6573 6365 6e74 2e20 4465  ient descent. De
+000005e0: 6675 6c74 7320 746f 2030 2e30 3030 312e  fults to 0.0001.
+000005f0: 0d0a 2020 2020 2020 2020 636f 6e76 6572  ..        conver
+00000600: 6765 6e63 655f 746f 6c3a 2066 6c6f 6174  gence_tol: float
+00000610: 0d0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
+00000620: 6520 746f 6c65 7261 6e63 6520 666f 7220  e tolerance for 
+00000630: 636f 6e76 6572 6765 6e63 6520 2873 746f  convergence (sto
+00000640: 7070 696e 6720 6372 6974 6572 696f 6e29  pping criterion)
+00000650: 2e20 4465 6661 756c 7473 2074 6f20 302e  . Defaults to 0.
+00000660: 3030 3030 3030 3030 3030 312e 0d0a 2020  00000000001...  
+00000670: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+00000680: 2020 200d 0a20 2020 2020 2020 206e 702e     ..        np.
+00000690: 7261 6e64 6f6d 2e73 6565 6428 3129 0d0a  random.seed(1)..
+000006a0: 2020 2020 2020 2020 7365 6c66 2e6c 6561          self.lea
+000006b0: 726e 696e 675f 7261 7465 203d 206c 6561  rning_rate = lea
+000006c0: 726e 696e 675f 7261 7465 0d0a 2020 2020  rning_rate..    
+000006d0: 2020 2020 7365 6c66 2e63 6f6e 7665 7267      self.converg
+000006e0: 656e 6365 5f74 6f6c 203d 2063 6f6e 7665  ence_tol = conve
+000006f0: 7267 656e 6365 5f74 6f6c 0d0a 0d0a 2020  rgence_tol....  
+00000700: 2020 6465 6620 696e 6974 6961 6c69 7a65    def initialize
+00000710: 5f70 6172 616d 6574 6572 2873 656c 6629  _parameter(self)
+00000720: 202d 3e20 4e6f 6e65 3a0d 0a20 2020 2020   -> None:..     
+00000730: 2020 200d 0a20 2020 2020 2020 2027 2727     ..        '''
+00000740: 0d0a 2020 2020 2020 2020 496e 6974 6961  ..        Initia
+00000750: 6c69 7a65 7320 7468 6520 7061 7261 6d65  lizes the parame
+00000760: 7465 7273 206f 6620 7468 6520 6d6f 6465  ters of the mode
+00000770: 6c2e 0d0a 2020 2020 2020 2020 2727 270d  l...        '''.
+00000780: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00000790: 2020 2073 656c 662e 5720 3d20 6e70 2e7a     self.W = np.z
+000007a0: 6572 6f73 2873 656c 662e 582e 7368 6170  eros(self.X.shap
+000007b0: 655b 315d 290d 0a20 2020 2020 2020 2073  e[1])..        s
+000007c0: 656c 662e 6220 3d20 302e 300d 0a0d 0a20  elf.b = 0.0.... 
+000007d0: 2020 2064 6566 2066 6f72 7761 7264 2873     def forward(s
+000007e0: 656c 662c 2058 3a6e 702e 6e64 6172 7261  elf, X:np.ndarra
+000007f0: 7929 202d 3e20 286e 702e 6e64 6172 7261  y) -> (np.ndarra
+00000800: 7929 3a0d 0a0d 0a20 2020 2020 2020 2027  y):....        '
+00000810: 2727 0d0a 2020 2020 2020 2020 436f 6d70  ''..        Comp
+00000820: 7574 6520 7468 6520 666f 7277 6172 6420  ute the forward 
+00000830: 7072 6f70 6167 6174 696f 6e20 666f 7220  propagation for 
+00000840: 6769 7665 6e20 696e 7075 7420 582e 0d0a  given input X...
+00000850: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00000860: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
+00000870: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
+00000880: 2020 583a 206e 702e 6e64 6172 7261 790d    X: np.ndarray.
+00000890: 0a20 2020 2020 2020 2020 2020 2049 6e70  .            Inp
+000008a0: 7574 2064 6174 6120 6f66 2073 6861 7065  ut data of shape
+000008b0: 2028 6d2c 206e 5f66 6561 7475 7265 7329   (m, n_features)
+000008c0: 2e0d 0a0d 0a20 2020 2020 2020 2052 6574  .....        Ret
+000008d0: 7572 6e73 0d0a 2020 2020 2020 2020 2d2d  urns..        --
+000008e0: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2072  -----..        r
+000008f0: 6574 7572 6e3a 206e 702e 6e64 6172 7261  eturn: np.ndarra
+00000900: 790d 0a20 2020 2020 2020 2020 2020 204f  y..            O
+00000910: 7574 7075 7420 6461 7461 206f 6620 7368  utput data of sh
+00000920: 6170 6520 286d 2c29 2e0d 0a20 2020 2020  ape (m,)...     
+00000930: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00000940: 0d0a 2020 2020 2020 2020 2320 7072 696e  ..        # prin
+00000950: 7428 582e 7368 6170 652c 2073 656c 662e  t(X.shape, self.
+00000960: 572e 7368 6170 6529 0d0a 2020 2020 2020  W.shape)..      
+00000970: 2020 5a20 3d20 6e70 2e6d 6174 6d75 6c28    Z = np.matmul(
+00000980: 582c 2073 656c 662e 5729 202b 2073 656c  X, self.W) + sel
+00000990: 662e 620d 0a20 2020 2020 2020 2041 2c20  f.b..        A, 
+000009a0: 6361 6368 6520 3d20 7574 696c 732e 7369  cache = utils.si
+000009b0: 676d 6f69 6428 5a29 0d0a 2020 2020 2020  gmoid(Z)..      
+000009c0: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+000009d0: 726e 2041 0d0a 0d0a 2020 2020 6465 6620  rn A....    def 
+000009e0: 636f 6d70 7574 655f 636f 7374 2873 656c  compute_cost(sel
+000009f0: 662c 2070 7265 6469 6374 696f 6e73 3a6e  f, predictions:n
+00000a00: 702e 6e64 6172 7261 7929 202d 3e20 666c  p.ndarray) -> fl
+00000a10: 6f61 743a 0d0a 2020 2020 2020 2020 0d0a  oat:..        ..
+00000a20: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
+00000a30: 2020 2020 2043 6f6d 7075 7465 7320 7468       Computes th
+00000a40: 6520 636f 7374 2066 756e 6374 696f 6e20  e cost function 
+00000a50: 666f 7220 6769 7665 6e20 7072 6564 6963  for given predic
+00000a60: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+00000a70: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
+00000a80: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
+00000a90: 0d0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
+00000aa0: 7469 6f6e 733a 206e 702e 6e64 6172 7261  tions: np.ndarra
+00000ab0: 790d 0a20 2020 2020 2020 2020 2020 2050  y..            P
+00000ac0: 7265 6469 6374 696f 6e73 206f 6620 7368  redictions of sh
+00000ad0: 6170 6520 286d 2c29 2e0d 0a0d 0a20 2020  ape (m,).....   
+00000ae0: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
+00000af0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
+00000b00: 2020 2020 2020 2072 6574 7572 6e3a 2066         return: f
+00000b10: 6c6f 6174 0d0a 2020 2020 2020 2020 2020  loat..          
+00000b20: 2020 436f 7374 206f 6620 7468 6520 6d6f    Cost of the mo
+00000b30: 6465 6c2e 0d0a 2020 2020 2020 2020 2727  del...        ''
+00000b40: 270d 0a20 2020 2020 2020 200d 0a20 2020  '..        ..   
+00000b50: 2020 2020 2023 2063 6f6d 7075 7465 2074       # compute t
+00000b60: 6865 2063 6f73 740d 0a20 2020 2020 2020  he cost..       
+00000b70: 2063 6f73 7420 3d20 6e70 2e73 756d 2828   cost = np.sum((
+00000b80: 2d6e 702e 6c6f 6728 7072 6564 6963 7469  -np.log(predicti
+00000b90: 6f6e 7320 2b20 3165 2d38 2920 2a20 7365  ons + 1e-8) * se
+00000ba0: 6c66 2e79 2920 2b20 282d 6e70 2e6c 6f67  lf.y) + (-np.log
+00000bb0: 2831 202d 2070 7265 6469 6374 696f 6e73  (1 - predictions
+00000bc0: 202b 2031 652d 3829 2920 2a20 5c0d 0a20   + 1e-8)) * \.. 
 00000bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000be0: 2831 202d 2073 656c 662e 7929 2920 2023  (1 - self.y))  #
-00000bf0: 2077 6520 6172 6520 6164 6469 6e67 2073   we are adding s
-00000c00: 6d61 6c6c 2076 616c 7565 2065 7073 696c  mall value epsil
-00000c10: 6f6e 2074 6f20 6176 6f69 6420 6c6f 6720  on to avoid log 
-00000c20: 6f66 2030 0d0a 2020 2020 2020 2020 0d0a  of 0..        ..
-00000c30: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00000c40: 6f73 7420 2f20 7365 6c66 2e58 2e73 6861  ost / self.X.sha
-00000c50: 7065 5b30 5d0d 0a0d 0a20 2020 2064 6566  pe[0]....    def
-00000c60: 2063 6f6d 7075 7465 5f67 7261 6469 656e   compute_gradien
-00000c70: 7428 7365 6c66 2c20 7072 6564 6963 7469  t(self, predicti
-00000c80: 6f6e 733a 6e70 2e6e 6461 7272 6179 2920  ons:np.ndarray) 
-00000c90: 2d3e 204e 6f6e 653a 0d0a 2020 2020 2020  -> None:..      
-00000ca0: 2020 0d0a 2020 2020 2020 2020 2727 270d    ..        '''.
-00000cb0: 0a20 2020 2020 2020 2043 6f6d 7075 7465  .        Compute
-00000cc0: 7320 7468 6520 6772 6164 6965 6e74 7320  s the gradients 
-00000cd0: 666f 7220 7468 6520 6d6f 6465 6c20 7573  for the model us
-00000ce0: 696e 6720 6769 7665 6e20 7072 6564 6963  ing given predic
-00000cf0: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
-00000d00: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00000d10: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00000d20: 0d0a 2020 2020 2020 2020 7072 6564 6963  ..        predic
-00000d30: 7469 6f6e 733a 206e 702e 6e64 6172 7261  tions: np.ndarra
-00000d40: 790d 0a20 2020 2020 2020 2020 2020 2050  y..            P
-00000d50: 7265 6469 6374 696f 6e73 206f 6620 7468  redictions of th
-00000d60: 6520 6d6f 6465 6c2e 0d0a 2020 2020 2020  e model...      
-00000d70: 2020 2727 270d 0a20 2020 2020 2020 200d    '''..        .
-00000d80: 0a20 2020 2020 2020 2023 2067 6574 2074  .        # get t
-00000d90: 7261 696e 696e 6720 7368 6170 650d 0a20  raining shape.. 
-00000da0: 2020 2020 2020 206d 203d 2073 656c 662e         m = self.
-00000db0: 582e 7368 6170 655b 305d 0d0a 0d0a 2020  X.shape[0]....  
-00000dc0: 2020 2020 2020 2320 636f 6d70 7574 6520        # compute 
-00000dd0: 6772 6164 6965 6e74 7320 616e 6420 7363  gradients and sc
-00000de0: 616c 6520 7468 656d 0d0a 2020 2020 2020  ale them..      
-00000df0: 2020 7365 6c66 2e64 5720 3d20 6e70 2e61    self.dW = np.a
-00000e00: 7272 6179 285b 6e70 2e6d 6561 6e28 6772  rray([np.mean(gr
-00000e10: 6164 2920 666f 7220 6772 6164 2069 6e20  ad) for grad in 
-00000e20: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-00000e30: 2020 2020 2020 206e 702e 6d61 746d 756c         np.matmul
-00000e40: 2873 656c 662e 582e 542c 2028 7072 6564  (self.X.T, (pred
-00000e50: 6963 7469 6f6e 7320 2d20 7365 6c66 2e79  ictions - self.y
-00000e60: 2929 205d 2920 2a20 312f 6d0d 0a20 2020  )) ]) * 1/m..   
-00000e70: 2020 2020 2073 656c 662e 6462 203d 206e       self.db = n
-00000e80: 702e 7375 6d28 6e70 2e73 7562 7472 6163  p.sum(np.subtrac
-00000e90: 7428 7072 6564 6963 7469 6f6e 732c 2073  t(predictions, s
-00000ea0: 656c 662e 7929 2920 2a20 312f 6d0d 0a0d  elf.y)) * 1/m...
-00000eb0: 0a20 2020 2064 6566 2066 6974 2873 656c  .    def fit(sel
-00000ec0: 662c 2058 3a6e 702e 6e64 6172 7261 792c  f, X:np.ndarray,
-00000ed0: 2079 3a6e 702e 6e64 6172 7261 792c 2069   y:np.ndarray, i
-00000ee0: 7465 7261 7469 6f6e 733a 696e 743d 3130  terations:int=10
-00000ef0: 3030 3030 302c 200d 0a20 2020 2020 2020  00000, ..       
-00000f00: 2020 2020 2070 6c6f 745f 636f 7374 3a62       plot_cost:b
-00000f10: 6f6f 6c3d 5472 7565 2c20 7665 7262 6f73  ool=True, verbos
-00000f20: 653a 626f 6f6c 3d54 7275 6529 202d 3e20  e:bool=True) -> 
-00000f30: 4e6f 6e65 3a0d 0a0d 0a20 2020 2020 2020  None:....       
-00000f40: 2027 2727 0d0a 2020 2020 2020 2020 5472   '''..        Tr
-00000f50: 6169 6e73 2074 6865 206d 6f64 656c 206f  ains the model o
-00000f60: 6e20 6769 7665 6e20 696e 7075 7420 5820  n given input X 
-00000f70: 616e 6420 6c61 6265 6c73 2079 2066 6f72  and labels y for
-00000f80: 2073 7065 6369 6669 6564 2069 7465 7261   specified itera
-00000f90: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
-00000fa0: 2020 5061 7261 6d65 7465 7273 0d0a 2020    Parameters..  
-00000fb0: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00000fc0: 0d0a 2020 2020 2020 2020 583a 206e 702e  ..        X: np.
-00000fd0: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
-00000fe0: 2020 2020 2054 7261 696e 696e 6720 696e       Training in
-00000ff0: 7075 7420 6461 7461 206f 6620 7368 6170  put data of shap
-00001000: 6520 286d 2c20 6e5f 6665 6174 7572 6573  e (m, n_features
-00001010: 292e 0d0a 2020 2020 2020 2020 793a 206e  )...        y: n
-00001020: 702e 6e64 6172 7261 790d 0a20 2020 2020  p.ndarray..     
-00001030: 2020 2020 2020 2054 7261 696e 696e 6720         Training 
-00001040: 6c61 6265 6c73 206f 6620 7368 6170 6520  labels of shape 
-00001050: 286d 2c29 2e0d 0a20 2020 2020 2020 2069  (m,)...        i
-00001060: 7465 7261 7469 6f6e 733a 2069 6e74 0d0a  terations: int..
-00001070: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00001080: 6e75 6d62 6572 206f 6620 6974 6572 6174  number of iterat
-00001090: 696f 6e73 2066 6f72 2067 7261 6469 656e  ions for gradien
-000010a0: 7420 6465 7363 656e 742e 2041 6c73 6f20  t descent. Also 
-000010b0: 6e61 6d65 6420 6570 6f63 6873 2e0d 0a20  named epochs... 
-000010c0: 2020 2020 2020 2070 6c6f 745f 636f 7374         plot_cost
-000010d0: 3a20 626f 6f6c 0d0a 2020 2020 2020 2020  : bool..        
-000010e0: 2020 2020 5768 6574 6865 7220 746f 2070      Whether to p
-000010f0: 6c6f 7420 7468 6520 636f 7374 2064 7572  lot the cost dur
-00001100: 696e 6720 7472 6169 6e69 6e67 2e20 4465  ing training. De
-00001110: 6661 756c 7473 2074 6f20 5472 7565 2e0d  faults to True..
-00001120: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
-00001130: 3a20 626f 6f6c 0d0a 2020 2020 2020 2020  : bool..        
-00001140: 2020 2020 5472 7565 2074 6f20 7072 696e      True to prin
-00001150: 7420 7472 6169 6e69 6e67 2072 6573 756c  t training resul
-00001160: 7473 2e0d 0a0d 0a20 2020 2020 2020 2052  ts.....        R
-00001170: 6169 7365 730d 0a20 2020 2020 2020 202d  aises..        -
-00001180: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2041  -----..        A
-00001190: 7373 6572 7469 6f6e 4572 726f 723a 2049  ssertionError: I
-000011a0: 6620 696e 7075 7420 6461 7461 2061 6e64  f input data and
-000011b0: 206c 6162 656c 7320 6172 6520 6e6f 7420   labels are not 
-000011c0: 4e75 6d50 7920 6172 7261 7973 206f 7220  NumPy arrays or 
-000011d0: 6861 7665 206d 6973 6d61 7463 6865 6420  have mismatched 
-000011e0: 7368 6170 6573 2e0d 0a0d 0a20 2020 2020  shapes.....     
-000011f0: 2020 2050 6c6f 7473 0d0a 2020 2020 2020     Plots..      
-00001200: 2020 2d2d 2d2d 2d0d 0a20 2020 2020 2020    -----..       
-00001210: 2050 6c6f 746c 7920 6c69 6e65 2063 6861   Plotly line cha
-00001220: 7274 2073 686f 7769 6e67 2063 6f73 7420  rt showing cost 
-00001230: 7673 2e20 6974 6572 6174 696f 6e20 2869  vs. iteration (i
-00001240: 6620 706c 6f74 5f63 6f73 7420 6973 2054  f plot_cost is T
-00001250: 7275 6529 2e0d 0a20 2020 2020 2020 2027  rue)...        '
-00001260: 2727 0d0a 2020 2020 2020 2020 0d0a 2020  ''..        ..  
-00001270: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00001280: 6e73 7461 6e63 6528 582c 206e 702e 6e64  nstance(X, np.nd
-00001290: 6172 7261 7929 2c20 2258 206d 7573 7420  array), "X must 
-000012a0: 6265 2061 204e 756d 5079 2061 7272 6179  be a NumPy array
-000012b0: 220d 0a20 2020 2020 2020 2061 7373 6572  "..        asser
-000012c0: 7420 6973 696e 7374 616e 6365 2879 2c20  t isinstance(y, 
-000012d0: 6e70 2e6e 6461 7272 6179 292c 2022 7920  np.ndarray), "y 
-000012e0: 6d75 7374 2062 6520 6120 4e75 6d50 7920  must be a NumPy 
-000012f0: 6172 7261 7922 0d0a 2020 2020 2020 2020  array"..        
-00001300: 6173 7365 7274 2058 2e73 6861 7065 5b30  assert X.shape[0
-00001310: 5d20 3d3d 2079 2e73 6861 7065 5b30 5d2c  ] == y.shape[0],
-00001320: 2022 5820 616e 6420 7920 6d75 7374 2068   "X and y must h
-00001330: 6176 6520 7468 6520 7361 6d65 206e 756d  ave the same num
-00001340: 6265 7220 6f66 2073 616d 706c 6573 220d  ber of samples".
-00001350: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00001360: 6974 6572 6174 696f 6e73 203e 2030 2c20  iterations > 0, 
-00001370: 2249 7465 7261 7469 6f6e 7320 6d75 7374  "Iterations must
-00001380: 2062 6520 6772 6561 7465 7220 7468 616e   be greater than
-00001390: 2030 220d 0a20 2020 2020 2020 200d 0a20   0"..        .. 
-000013a0: 2020 2020 2020 2058 203d 2058 2069 6620         X = X if 
-000013b0: 726f 756e 6428 6e70 2e6d 6561 6e28 5829  round(np.mean(X)
-000013c0: 2920 3d3d 2030 2061 6e64 2072 6f75 6e64  ) == 0 and round
-000013d0: 286e 702e 7374 6428 5829 2920 3d3d 2031  (np.std(X)) == 1
-000013e0: 2065 6c73 6520 7574 696c 732e 7363 616c   else utils.scal
-000013f0: 6528 5829 0d0a 2020 2020 2020 2020 7365  e(X)..        se
-00001400: 6c66 2e58 203d 2058 0d0a 2020 2020 2020  lf.X = X..      
-00001410: 2020 7365 6c66 2e79 203d 2079 0d0a 2020    self.y = y..  
-00001420: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
-00001430: 616c 697a 655f 7061 7261 6d65 7465 7228  alize_parameter(
-00001440: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00001450: 2020 2020 2073 656c 662e 6457 5f68 6973       self.dW_his
-00001460: 742c 2073 656c 662e 6462 5f68 6973 742c  t, self.db_hist,
-00001470: 2073 656c 662e 575f 6869 7374 2c20 7365   self.W_hist, se
-00001480: 6c66 2e62 5f68 6973 742c 2073 656c 662e  lf.b_hist, self.
-00001490: 636f 7374 7320 3d20 5b5d 2c20 5b5d 2c20  costs = [], [], 
-000014a0: 5b5d 2c20 5b5d 2c20 5b5d 0d0a 0d0a 2020  [], [], []....  
-000014b0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-000014c0: 616e 6765 2869 7465 7261 7469 6f6e 7329  ange(iterations)
-000014d0: 3a0d 0a20 2020 2020 2020 2020 2020 2023  :..            #
-000014e0: 2066 6f72 7761 7264 2070 726f 7061 6761   forward propaga
-000014f0: 7469 6f6e 0d0a 2020 2020 2020 2020 2020  tion..          
-00001500: 2020 7072 6564 6963 7469 6f6e 7320 3d20    predictions = 
-00001510: 7365 6c66 2e66 6f72 7761 7264 2873 656c  self.forward(sel
-00001520: 662e 5829 0d0a 0d0a 2020 2020 2020 2020  f.X)....        
-00001530: 2020 2020 2320 636f 6d70 7574 6520 636f      # compute co
-00001540: 7374 0d0a 2020 2020 2020 2020 2020 2020  st..            
-00001550: 7365 6c66 2e63 6f73 7420 3d20 7365 6c66  self.cost = self
-00001560: 2e63 6f6d 7075 7465 5f63 6f73 7428 7072  .compute_cost(pr
-00001570: 6564 6963 7469 6f6e 7329 0d0a 0d0a 2020  edictions)....  
-00001580: 2020 2020 2020 2020 2020 2320 636f 6d70            # comp
-00001590: 7574 6520 6772 6164 6965 6e74 730d 0a20  ute gradients.. 
-000015a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000015b0: 636f 6d70 7574 655f 6772 6164 6965 6e74  compute_gradient
-000015c0: 2870 7265 6469 6374 696f 6e73 290d 0a0d  (predictions)...
-000015d0: 0a20 2020 2020 2020 2020 2020 2023 2075  .            # u
-000015e0: 7064 6174 6520 7061 7261 6d65 7465 7273  pdate parameters
-000015f0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-00001600: 6c66 2e57 203d 2073 656c 662e 5720 2d20  lf.W = self.W - 
-00001610: 7365 6c66 2e6c 6561 726e 696e 675f 7261  self.learning_ra
-00001620: 7465 202a 2073 656c 662e 6457 0d0a 2020  te * self.dW..  
-00001630: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00001640: 203d 2073 656c 662e 6220 2d20 7365 6c66   = self.b - self
-00001650: 2e6c 6561 726e 696e 675f 7261 7465 202a  .learning_rate *
-00001660: 2073 656c 662e 6462 0d0a 2020 2020 2020   self.db..      
-00001670: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00001680: 2020 2020 7365 6c66 2e63 6f73 7473 2e61      self.costs.a
-00001690: 7070 656e 6428 7365 6c66 2e63 6f73 7429  ppend(self.cost)
-000016a0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-000016b0: 6c66 2e64 575f 6869 7374 2e61 7070 656e  lf.dW_hist.appen
-000016c0: 6428 7365 6c66 2e64 5729 0d0a 2020 2020  d(self.dW)..    
-000016d0: 2020 2020 2020 2020 7365 6c66 2e64 625f          self.db_
-000016e0: 6869 7374 2e61 7070 656e 6428 7365 6c66  hist.append(self
-000016f0: 2e64 6229 0d0a 2020 2020 2020 2020 2020  .db)..          
-00001700: 2020 7365 6c66 2e57 5f68 6973 742e 6170    self.W_hist.ap
-00001710: 7065 6e64 2873 656c 662e 5729 0d0a 2020  pend(self.W)..  
-00001720: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00001730: 5f68 6973 742e 6170 7065 6e64 2873 656c  _hist.append(sel
-00001740: 662e 6229 0d0a 0d0a 2020 2020 2020 2020  f.b)....        
-00001750: 2020 2020 2320 7072 696e 7420 636f 7374      # print cost
-00001760: 2065 7665 7279 2031 3030 2069 7465 7261   every 100 itera
-00001770: 7469 6f6e 730d 0a20 2020 2020 2020 2020  tions..         
-00001780: 2020 2069 6620 6920 2520 3130 3030 3020     if i % 10000 
-00001790: 3d3d 2030 2061 6e64 2076 6572 626f 7365  == 0 and verbose
-000017a0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000017b0: 2020 2070 7269 6e74 2866 2743 6f73 7420     print(f'Cost 
-000017c0: 6166 7465 7220 6974 6572 6174 696f 6e20  after iteration 
-000017d0: 7b69 7d3a 207b 7365 6c66 2e63 6f73 747d  {i}: {self.cost}
-000017e0: 2729 0d0a 0d0a 2020 2020 2020 2020 2020  ')....          
-000017f0: 2020 6966 2069 203e 2030 2061 6e64 2061    if i > 0 and a
-00001800: 6273 2873 656c 662e 636f 7374 735b 2d31  bs(self.costs[-1
-00001810: 5d20 2d20 7365 6c66 2e63 6f73 7473 5b2d  ] - self.costs[-
-00001820: 325d 2920 3c20 7365 6c66 2e63 6f6e 7665  2]) < self.conve
-00001830: 7267 656e 6365 5f74 6f6c 3a0d 0a20 2020  rgence_tol:..   
-00001840: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00001850: 6e74 2866 2743 6f6e 7665 7267 6564 2061  nt(f'Converged a
-00001860: 6674 6572 207b 697d 2069 7465 7261 7469  fter {i} iterati
-00001870: 6f6e 732e 2729 0d0a 2020 2020 2020 2020  ons.')..        
-00001880: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
-00001890: 0a20 2020 2020 2020 2069 6620 706c 6f74  .        if plot
-000018a0: 5f63 6f73 743a 0d0a 2020 2020 2020 2020  _cost:..        
-000018b0: 2020 2020 7365 6c66 2e70 6c6f 7443 6f73      self.plotCos
-000018c0: 7473 2829 0d0a 2020 2020 2020 2020 2020  ts()..          
-000018d0: 2020 0d0a 2020 2020 6465 6620 706c 6f74    ..    def plot
-000018e0: 436f 7374 7328 7365 6c66 2c20 7465 6d70  Costs(self, temp
-000018f0: 6c61 7465 3a73 7472 3d27 706c 6f74 6c79  late:str='plotly
-00001900: 5f64 6172 6b27 2c20 636f 6c6f 723a 7374  _dark', color:st
-00001910: 723d 2723 3431 4245 4539 2729 202d 3e20  r='#41BEE9') -> 
-00001920: 4e6f 6e65 3a0d 0a20 2020 2020 2020 200d  None:..        .
-00001930: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-00001940: 2020 2020 2020 506c 6f74 6c79 206c 696e        Plotly lin
-00001950: 6520 6368 6172 7420 7368 6f77 696e 6720  e chart showing 
-00001960: 636f 7374 2076 732e 2069 7465 7261 7469  cost vs. iterati
-00001970: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 2050  on.....        P
-00001980: 6172 616d 6574 6572 730d 0a20 2020 2020  arameters..     
-00001990: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20     ----------.. 
-000019a0: 2020 2020 2020 2074 656d 706c 6174 653a         template:
-000019b0: 2073 7472 0d0a 2020 2020 2020 2020 2020   str..          
-000019c0: 2020 5465 6d70 6c61 7465 2066 726f 6d20    Template from 
-000019d0: 7468 6520 6c69 7374 2061 7661 696c 6162  the list availab
-000019e0: 6c65 3a20 5b27 6767 706c 6f74 3227 2c20  le: ['ggplot2', 
-000019f0: 2773 6561 626f 726e 272c 2027 7369 6d70  'seaborn', 'simp
-00001a00: 6c65 5f77 6869 7465 272c 2027 706c 6f74  le_white', 'plot
-00001a10: 6c79 272c 0d0a 2020 2020 2020 2020 2020  ly',..          
-00001a20: 2020 2770 6c6f 746c 795f 7768 6974 6527    'plotly_white'
-00001a30: 2c20 2770 6c6f 746c 795f 6461 726b 272c  , 'plotly_dark',
-00001a40: 2027 7072 6573 656e 7461 7469 6f6e 272c   'presentation',
-00001a50: 2027 7867 7269 646f 6666 272c 0d0a 2020   'xgridoff',..  
-00001a60: 2020 2020 2020 2020 2020 2779 6772 6964            'ygrid
-00001a70: 6f66 6627 2c20 2767 7269 646f 6e27 2c20  off', 'gridon', 
-00001a80: 276e 6f6e 6527 5d2e 2044 6566 6175 6c74  'none']. Default
-00001a90: 7320 746f 2027 706c 6f74 6c79 5f64 6172  s to 'plotly_dar
-00001aa0: 6b27 2e0d 0a20 2020 2020 2020 2063 6f6c  k'...        col
-00001ab0: 6f72 3a20 7374 720d 0a20 2020 2020 2020  or: str..       
-00001ac0: 2020 2020 2048 6578 6167 6573 696d 616c       Hexagesimal
-00001ad0: 2063 6f6c 6f72 2e0d 0a0d 0a20 2020 2020   color.....     
-00001ae0: 2020 2050 6c6f 7473 0d0a 2020 2020 2020     Plots..      
-00001af0: 2020 2d2d 2d2d 2d0d 0a20 2020 2020 2020    -----..       
-00001b00: 2050 6c6f 746c 7920 6c69 6e65 2063 6861   Plotly line cha
-00001b10: 7274 2073 686f 7769 6e67 2063 6f73 7420  rt showing cost 
-00001b20: 7673 2e20 6974 6572 6174 696f 6e2e 0d0a  vs. iteration...
-00001b30: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
-00001b40: 2020 2020 200d 0a20 2020 2020 2020 2066       ..        f
-00001b50: 6967 203d 2070 782e 6c69 6e65 2879 3d73  ig = px.line(y=s
-00001b60: 656c 662e 636f 7374 732c 2074 6974 6c65  elf.costs, title
-00001b70: 3d22 436f 7374 2076 7320 4974 6572 6174  ="Cost vs Iterat
-00001b80: 696f 6e22 2c20 7465 6d70 6c61 7465 3d74  ion", template=t
-00001b90: 656d 706c 6174 6529 0d0a 2020 2020 2020  emplate)..      
-00001ba0: 2020 6669 672e 7570 6461 7465 5f6c 6179    fig.update_lay
-00001bb0: 6f75 7428 0d0a 2020 2020 2020 2020 2020  out(..          
-00001bc0: 2020 7469 746c 655f 666f 6e74 5f63 6f6c    title_font_col
-00001bd0: 6f72 3d63 6f6c 6f72 2c0d 0a20 2020 2020  or=color,..     
-00001be0: 2020 2020 2020 2078 6178 6973 3d64 6963         xaxis=dic
-00001bf0: 7428 636f 6c6f 723d 636f 6c6f 722c 2074  t(color=color, t
-00001c00: 6974 6c65 3d22 4974 6572 6174 696f 6e73  itle="Iterations
-00001c10: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-00001c20: 2079 6178 6973 3d64 6963 7428 636f 6c6f   yaxis=dict(colo
-00001c30: 723d 636f 6c6f 722c 2074 6974 6c65 3d22  r=color, title="
-00001c40: 436f 7374 2229 0d0a 2020 2020 2020 2020  Cost")..        
-00001c50: 290d 0a20 2020 2020 2020 2066 6967 2e73  )..        fig.s
-00001c60: 686f 7728 290d 0a0d 0a20 2020 2064 6566  how()....    def
-00001c70: 2070 7265 6469 6374 2873 656c 662c 2058   predict(self, X
-00001c80: 3a6e 702e 6e64 6172 7261 7929 202d 3e20  :np.ndarray) -> 
-00001c90: 6e70 2e6e 6461 7272 6179 3a0d 0a0d 0a20  np.ndarray:.... 
-00001ca0: 2020 2020 2020 2027 2727 0d0a 2020 2020         '''..    
-00001cb0: 2020 2020 5072 6564 6963 7420 7461 7267      Predict targ
-00001cc0: 6574 2076 616c 7565 7320 666f 7220 6e65  et values for ne
-00001cd0: 7720 696e 7075 7420 6461 7461 2e0d 0a0d  w input data....
-00001ce0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00001cf0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
-00001d00: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
-00001d10: 2058 3a20 6e70 2e6e 6461 7272 6179 0d0a   X: np.ndarray..
-00001d20: 2020 2020 2020 2020 2020 2020 496e 7075              Inpu
-00001d30: 7420 6461 7461 206f 6620 7368 6170 6520  t data of shape 
-00001d40: 286d 2c20 6e5f 6665 6174 7572 6573 292e  (m, n_features).
-00001d50: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
-00001d60: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
-00001d70: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7265  ----..        re
-00001d80: 7475 726e 3a20 6e70 2e6e 6461 7272 6179  turn: np.ndarray
-00001d90: 0d0a 2020 2020 2020 2020 2020 2020 5072  ..            Pr
-00001da0: 6564 6963 7465 6420 7461 7267 6574 2076  edicted target v
-00001db0: 616c 7565 7320 6f66 2073 6861 7065 2028  alues of shape (
-00001dc0: 6d2c 292e 0d0a 2020 2020 2020 2020 2727  m,)...        ''
-00001dd0: 270d 0a20 2020 2020 2020 200d 0a20 2020  '..        ..   
-00001de0: 2020 2020 2058 203d 2058 2069 6620 726f       X = X if ro
-00001df0: 756e 6428 6e70 2e6d 6561 6e28 5829 2920  und(np.mean(X)) 
-00001e00: 3d3d 2030 2061 6e64 2072 6f75 6e64 286e  == 0 and round(n
-00001e10: 702e 7374 6428 5829 2920 3d3d 2031 2065  p.std(X)) == 1 e
-00001e20: 6c73 6520 7574 696c 732e 7363 616c 6528  lse utils.scale(
-00001e30: 5829 0d0a 2020 2020 2020 2020 7365 6c66  X)..        self
-00001e40: 2e58 203d 2058 0d0a 2020 2020 2020 2020  .X = X..        
-00001e50: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00001e60: 206e 702e 726f 756e 6428 7365 6c66 2e66   np.round(self.f
-00001e70: 6f72 7761 7264 2858 2929 0d0a 2020 2020  orward(X))..    
-00001e80: 0d0a 2020 2020 6465 6620 6765 7457 6569  ..    def getWei
-00001e90: 6768 7473 2873 656c 662c 2066 6561 7475  ghts(self, featu
-00001ea0: 7265 733a 6c69 7374 2920 2d3e 2070 642e  res:list) -> pd.
-00001eb0: 4461 7461 4672 616d 653a 0d0a 0d0a 2020  DataFrame:....  
-00001ec0: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
-00001ed0: 2020 2047 6574 2074 6865 2077 6569 6768     Get the weigh
-00001ee0: 7473 2066 726f 6d20 7468 6520 6c61 7374  ts from the last
-00001ef0: 2074 7261 696e 696e 672e 0d0a 0d0a 2020   training.....  
-00001f00: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00001f10: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
-00001f20: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6665  ----..        fe
-00001f30: 6174 7572 6573 3a20 6c69 7374 0d0a 2020  atures: list..  
-00001f40: 2020 2020 2020 2020 2020 4c69 7374 206f            List o
-00001f50: 6620 7468 6520 6665 6174 7572 6573 206e  f the features n
-00001f60: 616d 6573 2061 7373 6f63 6961 7465 6420  ames associated 
-00001f70: 746f 2074 6865 2077 6569 6768 7473 2e0d  to the weights..
-00001f80: 0a0d 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00001f90: 6e73 0d0a 2020 2020 2020 2020 2d2d 2d2d  ns..        ----
-00001fa0: 2d2d 2d0d 0a20 2020 2020 2020 2072 6574  ---..        ret
-00001fb0: 7572 6e3a 2070 642e 4461 7461 4672 616d  urn: pd.DataFram
-00001fc0: 650d 0a20 2020 2020 2020 2020 2020 2044  e..            D
-00001fd0: 6174 6146 7261 6d65 2063 6f6e 7461 696e  ataFrame contain
-00001fe0: 696e 6720 7468 6520 7765 6967 6874 7320  ing the weights 
-00001ff0: 7261 6e6b 6564 2e0d 0a20 2020 2020 2020  ranked...       
-00002000: 2027 2727 0d0a 2020 2020 2020 2020 0d0a   '''..        ..
-00002010: 2020 2020 2020 2020 7265 7475 726e 2070          return p
-00002020: 642e 4461 7461 4672 616d 6528 7b27 5765  d.DataFrame({'We
-00002030: 6967 6874 7327 3a73 656c 662e 577d 2c20  ights':self.W}, 
-00002040: 696e 6465 783d 6665 6174 7572 6573 2920  index=features) 
-00002050: 5c0d 0a20 2020 2020 2020 2020 2020 2020  \..             
-00002060: 2020 202e 736f 7274 5f76 616c 7565 7328     .sort_values(
-00002070: 6279 3d27 5765 6967 6874 7327 2c20 6173  by='Weights', as
-00002080: 6365 6e64 696e 673d 4661 6c73 6529 0d0a  cending=False)..
-00002090: 2020 2020 0d0a 2020 2020 6465 6620 7361      ..    def sa
-000020a0: 7665 5f6d 6f64 656c 2873 656c 662c 2066  ve_model(self, f
-000020b0: 696c 656e 616d 653a 7374 723d 276c 6173  ilename:str='las
-000020c0: 745f 4c6f 6752 6567 5f6d 6f64 656c 2e70  t_LogReg_model.p
-000020d0: 6b6c 2729 202d 3e20 4e6f 6e65 3a0d 0a0d  kl') -> None:...
-000020e0: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-000020f0: 2020 2020 2020 5361 7665 2074 6865 2074        Save the t
-00002100: 7261 696e 6564 206d 6f64 656c 2074 6f20  rained model to 
-00002110: 6120 6669 6c65 2075 7369 6e67 2070 6963  a file using pic
-00002120: 6b6c 652e 0d0a 0d0a 2020 2020 2020 2020  kle.....        
-00002130: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
-00002140: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
-00002150: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00002160: 3a20 7374 720d 0a20 2020 2020 2020 2020  : str..         
-00002170: 2020 2054 6865 206e 616d 6520 6f66 2074     The name of t
-00002180: 6865 2066 696c 6520 746f 2073 6176 6520  he file to save 
-00002190: 7468 6520 6d6f 6465 6c20 746f 2e0d 0a20  the model to... 
-000021a0: 2020 2020 2020 2027 2727 0d0a 0d0a 2020         '''....  
-000021b0: 2020 2020 2020 6d6f 6465 6c5f 6461 7461        model_data
-000021c0: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
-000021d0: 2020 276c 6561 726e 696e 675f 7261 7465    'learning_rate
-000021e0: 273a 2073 656c 662e 6c65 6172 6e69 6e67  ': self.learning
-000021f0: 5f72 6174 652c 0d0a 2020 2020 2020 2020  _rate,..        
-00002200: 2020 2020 2763 6f6e 7665 7267 656e 6365      'convergence
-00002210: 5f74 6f6c 273a 2073 656c 662e 636f 6e76  _tol': self.conv
-00002220: 6572 6765 6e63 655f 746f 6c2c 0d0a 2020  ergence_tol,..  
-00002230: 2020 2020 2020 2020 2020 2757 273a 2073            'W': s
-00002240: 656c 662e 572c 0d0a 2020 2020 2020 2020  elf.W,..        
-00002250: 2020 2020 2762 273a 2073 656c 662e 620d      'b': self.b.
-00002260: 0a20 2020 2020 2020 207d 0d0a 0d0a 2020  .        }....  
-00002270: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00002280: 6669 6c65 6e61 6d65 2c20 2777 6227 2920  filename, 'wb') 
-00002290: 6173 2066 696c 653a 0d0a 2020 2020 2020  as file:..      
-000022a0: 2020 2020 2020 7069 636b 6c65 2e64 756d        pickle.dum
-000022b0: 7028 6d6f 6465 6c5f 6461 7461 2c20 6669  p(model_data, fi
-000022c0: 6c65 290d 0a0d 0a20 2020 2040 636c 6173  le)....    @clas
-000022d0: 736d 6574 686f 640d 0a20 2020 2064 6566  smethod..    def
-000022e0: 206c 6f61 645f 6d6f 6465 6c28 636c 732c   load_model(cls,
-000022f0: 2066 696c 656e 616d 653a 7374 723d 276c   filename:str='l
-00002300: 6173 745f 4c6f 6752 6567 5f6d 6f64 656c  ast_LogReg_model
-00002310: 2e70 6b6c 2729 3a0d 0a0d 0a20 2020 2020  .pkl'):....     
-00002320: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
-00002330: 4c6f 6164 2061 2074 7261 696e 6564 206d  Load a trained m
-00002340: 6f64 656c 2066 726f 6d20 6120 6669 6c65  odel from a file
-00002350: 2075 7369 6e67 2070 6963 6b6c 652e 0d0a   using pickle...
-00002360: 0d0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00002370: 7465 7273 0d0a 2020 2020 2020 2020 2d2d  ters..        --
-00002380: 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020  --------..      
-00002390: 2020 6669 6c65 6e61 6d65 3a20 7374 720d    filename: str.
-000023a0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-000023b0: 206e 616d 6520 6f66 2074 6865 2066 696c   name of the fil
-000023c0: 6520 746f 206c 6f61 6420 7468 6520 6d6f  e to load the mo
-000023d0: 6465 6c20 6672 6f6d 2e0d 0a0d 0a20 2020  del from.....   
-000023e0: 2020 2020 2052 6574 7572 6e73 0d0a 2020       Returns..  
-000023f0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20        -------.. 
-00002400: 2020 2020 2020 206c 6f61 6465 645f 6d6f         loaded_mo
-00002410: 6465 6c3a 204c 6f67 6973 7469 6352 6567  del: LogisticReg
-00002420: 7265 7373 696f 6e0d 0a20 2020 2020 2020  ression..       
-00002430: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
-00002440: 206f 6620 7468 6520 4c6f 6769 7374 6963   of the Logistic
-00002450: 5265 6772 6573 7369 6f6e 2063 6c61 7373  Regression class
-00002460: 2077 6974 6820 6c6f 6164 6564 2070 6172   with loaded par
-00002470: 616d 6574 6572 732e 0d0a 2020 2020 2020  ameters...      
-00002480: 2020 2727 270d 0a0d 0a20 2020 2020 2020    '''....       
-00002490: 2077 6974 6820 6f70 656e 2866 696c 656e   with open(filen
-000024a0: 616d 652c 2027 7262 2729 2061 7320 6669  ame, 'rb') as fi
-000024b0: 6c65 3a0d 0a20 2020 2020 2020 2020 2020  le:..           
-000024c0: 206d 6f64 656c 5f64 6174 6120 3d20 7069   model_data = pi
-000024d0: 636b 6c65 2e6c 6f61 6428 6669 6c65 290d  ckle.load(file).
-000024e0: 0a0d 0a20 2020 2020 2020 2023 2043 7265  ...        # Cre
-000024f0: 6174 6520 6120 6e65 7720 696e 7374 616e  ate a new instan
-00002500: 6365 206f 6620 7468 6520 636c 6173 7320  ce of the class 
-00002510: 616e 6420 696e 6974 6961 6c69 7a65 2069  and initialize i
-00002520: 7420 7769 7468 2074 6865 206c 6f61 6465  t with the loade
-00002530: 6420 7061 7261 6d65 7465 7273 0d0a 2020  d parameters..  
-00002540: 2020 2020 2020 6c6f 6164 6564 5f6d 6f64        loaded_mod
-00002550: 656c 203d 2063 6c73 286d 6f64 656c 5f64  el = cls(model_d
-00002560: 6174 615b 276c 6561 726e 696e 675f 7261  ata['learning_ra
-00002570: 7465 275d 2c20 6d6f 6465 6c5f 6461 7461  te'], model_data
-00002580: 5b27 636f 6e76 6572 6765 6e63 655f 746f  ['convergence_to
-00002590: 6c27 5d29 0d0a 2020 2020 2020 2020 6c6f  l'])..        lo
-000025a0: 6164 6564 5f6d 6f64 656c 2e57 203d 206d  aded_model.W = m
-000025b0: 6f64 656c 5f64 6174 615b 2757 275d 0d0a  odel_data['W']..
-000025c0: 2020 2020 2020 2020 6c6f 6164 6564 5f6d          loaded_m
-000025d0: 6f64 656c 2e62 203d 206d 6f64 656c 5f64  odel.b = model_d
-000025e0: 6174 615b 2762 275d 0d0a 0d0a 2020 2020  ata['b']....    
-000025f0: 2020 2020 7265 7475 726e 206c 6f61 6465      return loade
-00002600: 645f 6d6f 6465 6c0d 0a0d 0a20 2020 2064  d_model....    d
-00002610: 6566 2070 6c6f 7450 7265 6469 6374 696f  ef plotPredictio
-00002620: 6e28 7365 6c66 2c20 583a 6e70 2e6e 6461  n(self, X:np.nda
-00002630: 7272 6179 3d4e 6f6e 652c 2079 3a6e 702e  rray=None, y:np.
-00002640: 6e64 6172 7261 793d 4e6f 6e65 2920 2d3e  ndarray=None) ->
-00002650: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002660: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00002670: 2020 2020 2020 2050 6c6f 746c 7920 6368         Plotly ch
-00002680: 6172 7420 636f 6e74 6169 6e69 6e67 2074  art containing t
-00002690: 6865 2072 6561 6c20 6461 7461 2061 6e64  he real data and
-000026a0: 2074 6865 2070 7265 6469 6374 696f 6e2e   the prediction.
-000026b0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
-000026c0: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
-000026d0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
-000026e0: 2020 2020 583a 206e 702e 6e64 6172 7261      X: np.ndarra
-000026f0: 790d 0a20 2020 2020 2020 2020 2020 2049  y..            I
-00002700: 6e70 7574 2064 6174 6120 6f66 2073 6861  nput data of sha
-00002710: 7065 2028 6d2c 206e 5f66 6561 7475 7265  pe (m, n_feature
-00002720: 7329 2e0d 0a20 2020 2020 2020 2079 3a20  s)...        y: 
-00002730: 6e70 2e6e 6461 7272 6179 0d0a 2020 2020  np.ndarray..    
-00002740: 2020 2020 2020 2020 4461 7461 2074 6f20          Data to 
-00002750: 7072 6564 6963 7420 6f66 2073 6861 7065  predict of shape
-00002760: 2028 6d2c 2029 2e0d 0a0d 0a20 2020 2020   (m, ).....     
-00002770: 2020 2050 6c6f 7473 0d0a 2020 2020 2020     Plots..      
-00002780: 2020 2d2d 2d2d 2d0d 0a20 2020 2020 2020    -----..       
-00002790: 2050 6c6f 746c 7920 6368 6172 7420 636f   Plotly chart co
-000027a0: 6e74 6169 6e69 6e67 2074 6865 2072 6561  ntaining the rea
-000027b0: 6c20 6461 7461 2061 6e64 2074 6865 2070  l data and the p
-000027c0: 7265 6469 6374 696f 6e2e 0d0a 2020 2020  rediction...    
-000027d0: 2020 2020 2727 270d 0a0d 0a20 2020 2020      '''....     
-000027e0: 2020 2058 203d 2073 656c 662e 5820 6966     X = self.X if
-000027f0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00002800: 582c 206e 702e 6e64 6172 7261 7929 2065  X, np.ndarray) e
-00002810: 6c73 6520 580d 0a20 2020 2020 2020 2079  lse X..        y
-00002820: 203d 2073 656c 662e 7920 6966 206e 6f74   = self.y if not
-00002830: 2069 7369 6e73 7461 6e63 6528 792c 206e   isinstance(y, n
-00002840: 702e 6e64 6172 7261 7929 2065 6c73 6520  p.ndarray) else 
-00002850: 790d 0a20 2020 2020 2020 200d 0a20 2020  y..        ..   
-00002860: 2020 2020 2069 6d70 6f72 7420 706c 6f74       import plot
-00002870: 6c79 2e67 7261 7068 5f6f 626a 7320 6173  ly.graph_objs as
-00002880: 2067 6f0d 0a20 2020 2020 2020 2066 6967   go..        fig
-00002890: 203d 2067 6f2e 4669 6775 7265 285b 0d0a   = go.Figure([..
-000028a0: 2020 2020 2020 2020 2020 2020 676f 2e53              go.S
-000028b0: 6361 7474 6572 280d 0a20 2020 2020 2020  catter(..       
-000028c0: 2020 2020 2020 2020 206e 616d 653d 2744           name='D
-000028d0: 6174 6127 2c0d 0a20 2020 2020 2020 2020  ata',..         
-000028e0: 2020 2020 2020 2079 3d79 2c0d 0a20 2020         y=y,..   
-000028f0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00002900: 653d 276d 6172 6b65 7273 272c 0d0a 2020  e='markers',..  
-00002910: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00002920: 726b 6572 3d64 6963 7428 636f 6c6f 723d  rker=dict(color=
-00002930: 2772 6564 272c 2073 697a 653d 3229 2c0d  'red', size=2),.
-00002940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002950: 2073 686f 776c 6567 656e 643d 5472 7565   showlegend=True
-00002960: 0d0a 2020 2020 2020 2020 2020 2020 292c  ..            ),
-00002970: 0d0a 2020 2020 2020 2020 2020 2020 676f  ..            go
-00002980: 2e53 6361 7474 6572 280d 0a20 2020 2020  .Scatter(..     
-00002990: 2020 2020 2020 2020 2020 206e 616d 653d             name=
-000029a0: 2750 7265 6469 6374 696f 6e27 2c0d 0a20  'Prediction',.. 
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2079                 y
-000029c0: 3d73 656c 662e 7072 6564 6963 7428 5829  =self.predict(X)
-000029d0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000029e0: 2020 206d 6f64 653d 276c 696e 6573 272c     mode='lines',
-000029f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002a00: 2020 6d61 726b 6572 3d64 6963 7428 636f    marker=dict(co
-00002a10: 6c6f 723d 2223 3434 3422 292c 0d0a 2020  lor="#444"),..  
-00002a20: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00002a30: 6e65 3d64 6963 7428 7769 6474 683d 3129  ne=dict(width=1)
-00002a40: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002a50: 2020 2073 686f 776c 6567 656e 643d 5472     showlegend=Tr
-00002a60: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00002a70: 290d 0a20 2020 2020 2020 205d 290d 0a20  )..        ]).. 
-00002a80: 2020 2020 2020 2066 6967 2e75 7064 6174         fig.updat
-00002a90: 655f 6c61 796f 7574 280d 0a20 2020 2020  e_layout(..     
-00002aa0: 2020 2020 2020 2078 6178 6973 5f74 6974         xaxis_tit
-00002ab0: 6c65 3d27 5827 2c0d 0a20 2020 2020 2020  le='X',..       
-00002ac0: 2020 2020 2079 6178 6973 5f74 6974 6c65       yaxis_title
-00002ad0: 3d27 5927 2c0d 0a20 2020 2020 2020 2020  ='Y',..         
-00002ae0: 2020 2074 6974 6c65 3d27 5072 6564 6963     title='Predic
-00002af0: 7469 6f6e 2076 732e 2074 6172 6765 7427  tion vs. target'
-00002b00: 2c0d 0a20 2020 2020 2020 2020 2020 2068  ,..            h
-00002b10: 6f76 6572 6d6f 6465 3d22 7822 0d0a 2020  overmode="x"..  
-00002b20: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-00002b30: 2066 6967 2e73 686f 7728 290d 0a20 2020   fig.show()..   
-00002b40: 2020 2020 200d 0a20 2020 2064 6566 2067       ..    def g
-00002b50: 6574 4d65 7472 6963 7328 7365 6c66 2c20  etMetrics(self, 
-00002b60: 795f 7265 616c 3a6e 702e 6e64 6172 7261  y_real:np.ndarra
-00002b70: 792c 2079 5f70 7265 643a 6e70 2e6e 6461  y, y_pred:np.nda
-00002b80: 7272 6179 2c20 7368 6f77 3a62 6f6f 6c3d  rray, show:bool=
-00002b90: 5472 7565 2920 2d3e 2064 6963 743a 0d0a  True) -> dict:..
-00002ba0: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
-00002bb0: 2020 2020 2020 2047 6574 206d 6f64 656c         Get model
-00002bc0: 206d 6574 7269 6373 2e0d 0a0d 0a20 2020   metrics.....   
-00002bd0: 2020 2020 2050 6172 616d 6574 6572 730d       Parameters.
-00002be0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00002bf0: 2d2d 2d0d 0a20 2020 2020 2020 2079 5f72  ---..        y_r
-00002c00: 6561 6c3a 206e 702e 6e64 6172 7261 790d  eal: np.ndarray.
-00002c10: 0a20 2020 2020 2020 2020 2020 2041 7272  .            Arr
-00002c20: 6179 2063 6f6e 7461 696e 6967 2074 6865  ay containig the
-00002c30: 2072 6561 6c20 6461 7461 2074 6f20 6265   real data to be
-00002c40: 2070 7265 6469 6374 6564 2e0d 0a20 2020   predicted...   
-00002c50: 2020 2020 2079 5f70 7265 643a 206e 702e       y_pred: np.
-00002c60: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
-00002c70: 2020 2020 2041 7272 6179 2063 6f6e 7461       Array conta
-00002c80: 696e 6967 2074 6865 2070 7265 6469 6374  inig the predict
-00002c90: 6564 2064 6174 612e 0d0a 2020 2020 2020  ed data...      
-00002ca0: 2020 7368 6f77 3a20 626f 6f6c 0d0a 2020    show: bool..  
-00002cb0: 2020 2020 2020 2020 2020 5472 7565 2074            True t
-00002cc0: 6f20 7072 696e 7420 7468 6520 6d65 7472  o print the metr
-00002cd0: 6963 732e 0d0a 0d0a 2020 2020 2020 2020  ics.....        
-00002ce0: 5265 7475 726e 730d 0a20 2020 2020 2020  Returns..       
-00002cf0: 202d 2d2d 2d2d 2d2d 0d0a 2020 2020 2020   -------..      
-00002d00: 2020 7265 7475 726e 3a20 6469 6374 0d0a    return: dict..
-00002d10: 2020 2020 2020 2020 2020 2020 4469 6374              Dict
-00002d20: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-00002d30: 6720 2761 6363 7572 6163 7927 2c20 2770  g 'accuracy', 'p
-00002d40: 7265 6369 7369 6f6e 272c 2027 7265 6361  recision', 'reca
-00002d50: 6c6c 2720 616e 6420 0d0a 2020 2020 2020  ll' and ..      
-00002d60: 2020 2020 2020 2766 315f 7363 6f72 6527        'f1_score'
-00002d70: 2066 6f72 2074 6865 206d 6f64 656c 2e0d   for the model..
-00002d80: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
-00002d90: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00002da0: 6163 6375 7261 6379 203d 2075 7469 6c73  accuracy = utils
-00002db0: 2e43 6c61 7373 6966 6963 6174 696f 6e4d  .ClassificationM
-00002dc0: 6574 7269 6373 2e61 6363 7572 6163 7928  etrics.accuracy(
-00002dd0: 795f 7265 616c 2c20 795f 7072 6564 290d  y_real, y_pred).
-00002de0: 0a20 2020 2020 2020 2070 7265 6369 7369  .        precisi
-00002df0: 6f6e 203d 2075 7469 6c73 2e43 6c61 7373  on = utils.Class
-00002e00: 6966 6963 6174 696f 6e4d 6574 7269 6373  ificationMetrics
-00002e10: 2e70 7265 6369 7369 6f6e 2879 5f72 6561  .precision(y_rea
-00002e20: 6c2c 2079 5f70 7265 6429 0d0a 2020 2020  l, y_pred)..    
-00002e30: 2020 2020 7265 6361 6c6c 203d 2075 7469      recall = uti
-00002e40: 6c73 2e43 6c61 7373 6966 6963 6174 696f  ls.Classificatio
-00002e50: 6e4d 6574 7269 6373 2e72 6563 616c 6c28  nMetrics.recall(
-00002e60: 795f 7265 616c 2c20 795f 7072 6564 290d  y_real, y_pred).
-00002e70: 0a20 2020 2020 2020 2066 315f 7363 6f72  .        f1_scor
-00002e80: 6520 3d20 7574 696c 732e 436c 6173 7369  e = utils.Classi
-00002e90: 6669 6361 7469 6f6e 4d65 7472 6963 732e  ficationMetrics.
-00002ea0: 6631 5f73 636f 7265 2879 5f72 6561 6c2c  f1_score(y_real,
-00002eb0: 2079 5f70 7265 6429 0d0a 2020 2020 2020   y_pred)..      
-00002ec0: 2020 0d0a 2020 2020 2020 2020 6966 2073    ..        if s
-00002ed0: 686f 773a 0d0a 2020 2020 2020 2020 2020  how:..          
-00002ee0: 2020 7072 696e 7428 6622 4163 6375 7261    print(f"Accura
-00002ef0: 6379 3a20 7b61 6363 7572 6163 793a 2e32  cy: {accuracy:.2
-00002f00: 257d 2229 0d0a 2020 2020 2020 2020 2020  %}")..          
-00002f10: 2020 7072 696e 7428 6622 5072 6563 6973    print(f"Precis
-00002f20: 696f 6e3a 207b 7072 6563 6973 696f 6e3a  ion: {precision:
-00002f30: 2e32 257d 2229 0d0a 2020 2020 2020 2020  .2%}")..        
-00002f40: 2020 2020 7072 696e 7428 6622 5265 6361      print(f"Reca
-00002f50: 6c6c 3a20 7b72 6563 616c 6c3a 2e32 257d  ll: {recall:.2%}
-00002f60: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00002f70: 7072 696e 7428 6622 4631 2d53 636f 7265  print(f"F1-Score
-00002f80: 3a20 7b66 315f 7363 6f72 653a 2e32 257d  : {f1_score:.2%}
-00002f90: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-00002fa0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002fb0: 207b 2761 6363 7572 6163 7927 3a61 6363   {'accuracy':acc
-00002fc0: 7572 6163 792c 2027 7072 6563 6973 696f  uracy, 'precisio
-00002fd0: 6e27 3a70 7265 6369 7369 6f6e 2c20 0d0a  n':precision, ..
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2772 6563 616c 6c27 3a72 6563 616c 6c2c  'recall':recall,
-00003000: 2027 6631 5f73 636f 7265 273a 6631 5f73   'f1_score':f1_s
-00003010: 636f 7265 7d0d 0a0d 0a20 2020 2020 2020  core}....       
-00003020: 200d 0a69 6620 5f5f 6e61 6d65 5f5f 203d   ..if __name__ =
-00003030: 3d20 275f 5f6d 6169 6e5f 5f27 3a0d 0a0d  = '__main__':...
-00003040: 0a20 2020 2069 6d70 6f72 7420 7966 696e  .    import yfin
-00003050: 616e 6365 2061 7320 7966 0d0a 2020 2020  ance as yf..    
-00003060: 6672 6f6d 2070 7269 6e63 6970 616c 5f63  from principal_c
-00003070: 6f6d 706f 6e65 6e74 2069 6d70 6f72 7420  omponent import 
-00003080: 5043 410d 0a20 2020 200d 0a20 2020 2070  PCA..    ..    p
-00003090: 6361 5f61 7070 6c79 203d 2046 616c 7365  ca_apply = False
-000030a0: 0d0a 2020 2020 6a75 7374 5f73 6964 6520  ..    just_side 
-000030b0: 3d20 4661 6c73 650d 0a0d 0a20 2020 2064  = False....    d
-000030c0: 6174 6120 3d20 7966 2e54 6963 6b65 7228  ata = yf.Ticker(
-000030d0: 2754 534c 4127 292e 6869 7374 6f72 7928  'TSLA').history(
-000030e0: 7065 7269 6f64 3d27 3579 272c 2069 6e74  period='5y', int
-000030f0: 6572 7661 6c3d 2731 6427 290d 0a20 2020  erval='1d')..   
-00003100: 2064 6174 612e 636f 6c75 6d6e 7320 3d20   data.columns = 
-00003110: 5b63 2e6c 6f77 6572 2829 2066 6f72 2063  [c.lower() for c
-00003120: 2069 6e20 6461 7461 2e63 6f6c 756d 6e73   in data.columns
-00003130: 5d0d 0a20 2020 2064 6174 615b 2764 6174  ]..    data['dat
-00003140: 6527 5d20 3d20 6461 7461 2e69 6e64 6578  e'] = data.index
-00003150: 0d0a 2020 2020 6461 7461 5b27 7072 6576  ..    data['prev
-00003160: 5f63 6c6f 7365 275d 203d 2064 6174 615b  _close'] = data[
-00003170: 2763 6c6f 7365 275d 2e73 6869 6674 2831  'close'].shift(1
-00003180: 290d 0a20 2020 2064 6174 615b 276f 7574  )..    data['out
-00003190: 6c69 6572 5f70 7527 5d20 3d20 6461 7461  lier_pu'] = data
-000031a0: 5b27 6f70 656e 275d 2f64 6174 615b 276f  ['open']/data['o
-000031b0: 7065 6e27 5d2e 726f 6c6c 696e 6728 3530  pen'].rolling(50
-000031c0: 292e 6d65 616e 2829 202d 2031 0d0a 2020  ).mean() - 1..  
-000031d0: 2020 6461 7461 5b27 7261 6e67 6527 5d20    data['range'] 
-000031e0: 3d20 2864 6174 615b 2768 6967 6827 5d20  = (data['high'] 
-000031f0: 2d20 6461 7461 5b27 6c6f 7727 5d29 2e73  - data['low']).s
-00003200: 6869 6674 2831 290d 0a20 2020 2064 6174  hift(1)..    dat
-00003210: 615b 2772 616e 6765 5f70 7527 5d20 3d20  a['range_pu'] = 
-00003220: 6461 7461 5b27 7261 6e67 6527 5d2f 6461  data['range']/da
-00003230: 7461 5b27 6f70 656e 275d 0d0a 2020 2020  ta['open']..    
-00003240: 6461 7461 5b27 6f70 656e 5f74 6f5f 636c  data['open_to_cl
-00003250: 6f73 6527 5d20 3d20 2864 6174 615b 2763  ose'] = (data['c
-00003260: 6c6f 7365 275d 202d 2064 6174 615b 276f  lose'] - data['o
-00003270: 7065 6e27 5d29 2e73 6869 6674 2831 290d  pen']).shift(1).
-00003280: 0a20 2020 2064 6174 615b 276f 7065 6e5f  .    data['open_
-00003290: 746f 5f63 6c6f 7365 5f70 7527 5d20 3d20  to_close_pu'] = 
-000032a0: 6461 7461 5b27 7261 6e67 6527 5d2f 6461  data['range']/da
-000032b0: 7461 5b27 6f70 656e 275d 0d0a 2020 2020  ta['open']..    
-000032c0: 6461 7461 5b27 6761 7027 5d20 3d20 6461  data['gap'] = da
-000032d0: 7461 5b27 6f70 656e 275d 202d 2064 6174  ta['open'] - dat
-000032e0: 615b 2763 6c6f 7365 275d 2e73 6869 6674  a['close'].shift
-000032f0: 2831 290d 0a20 2020 2064 6174 615b 2767  (1)..    data['g
-00003300: 6170 5f70 7527 5d20 3d20 6461 7461 5b27  ap_pu'] = data['
-00003310: 6761 7027 5d20 2f20 6461 7461 5b27 636c  gap'] / data['cl
-00003320: 6f73 6527 5d2e 7368 6966 7428 3129 0d0a  ose'].shift(1)..
-00003330: 2020 2020 0d0a 2020 2020 6461 7461 5b27      ..    data['
-00003340: 6461 7927 5d20 3d20 6461 7461 5b27 6461  day'] = data['da
-00003350: 7465 275d 2e64 742e 7965 6172 0d0a 2020  te'].dt.year..  
-00003360: 2020 6461 7461 5b27 6d6f 6e74 6827 5d20    data['month'] 
-00003370: 3d20 6461 7461 5b27 6461 7465 275d 2e64  = data['date'].d
-00003380: 742e 6d6f 6e74 680d 0a20 2020 2064 6174  t.month..    dat
-00003390: 615b 2779 6561 7227 5d20 3d20 6461 7461  a['year'] = data
-000033a0: 5b27 6461 7465 275d 2e64 742e 6461 790d  ['date'].dt.day.
-000033b0: 0a20 2020 2064 6174 615b 2777 6565 6b5f  .    data['week_
-000033c0: 6461 7927 5d20 3d20 6461 7461 5b27 6461  day'] = data['da
-000033d0: 7465 275d 2e64 742e 6461 796f 6677 6565  te'].dt.dayofwee
-000033e0: 6b0d 0a20 2020 2064 6174 615b 2769 735f  k..    data['is_
-000033f0: 7175 6172 7465 725f 656e 6427 5d20 3d20  quarter_end'] = 
-00003400: 6e70 2e77 6865 7265 2864 6174 615b 276d  np.where(data['m
-00003410: 6f6e 7468 275d 2533 203d 3d20 302c 2031  onth']%3 == 0, 1
-00003420: 2c20 3029 0d0a 2020 2020 2020 2020 0d0a  , 0)..        ..
-00003430: 2020 2020 6461 7461 5b27 7461 7267 6574      data['target
-00003440: 275d 203d 206e 702e 7768 6572 6528 6461  '] = np.where(da
-00003450: 7461 5b27 6f70 656e 275d 203c 2064 6174  ta['open'] < dat
-00003460: 615b 2763 6c6f 7365 275d 2c20 312c 2030  a['close'], 1, 0
-00003470: 290d 0a20 2020 2064 6174 612e 6472 6f70  )..    data.drop
-00003480: 6e61 2869 6e70 6c61 6365 3d54 7275 6529  na(inplace=True)
-00003490: 0d0a 2020 2020 0d0a 2020 2020 6665 6174  ..    ..    feat
-000034a0: 7572 6573 203d 205b 2772 616e 6765 5f70  ures = ['range_p
-000034b0: 7527 2c20 276f 7065 6e5f 746f 5f63 6c6f  u', 'open_to_clo
-000034c0: 7365 5f70 7527 2c20 2767 6170 5f70 7527  se_pu', 'gap_pu'
-000034d0: 2c20 276f 7574 6c69 6572 5f70 7527 2c20  , 'outlier_pu', 
-000034e0: 2764 6179 272c 2027 6d6f 6e74 6827 2c20  'day', 'month', 
-000034f0: 2777 6565 6b5f 6461 7927 2c20 2769 735f  'week_day', 'is_
-00003500: 7175 6172 7465 725f 656e 6427 5d0d 0a0d  quarter_end']...
-00003510: 0a20 2020 2058 5f74 7261 696e 2c20 585f  .    X_train, X_
-00003520: 7465 7374 2c20 795f 7472 6169 6e2c 2079  test, y_train, y
-00003530: 5f74 6573 7420 3d20 7574 696c 732e 7472  _test = utils.tr
-00003540: 6169 6e5f 7465 7374 5f73 706c 6974 2864  ain_test_split(d
-00003550: 6174 615b 6665 6174 7572 6573 5d2c 2064  ata[features], d
-00003560: 6174 615b 2774 6172 6765 7427 5d2c 200d  ata['target'], .
-00003570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000be0: 2020 2020 2020 2028 3120 2d20 7365 6c66         (1 - self
+00000bf0: 2e79 2929 2020 2320 7765 2061 7265 2061  .y))  # we are a
+00000c00: 6464 696e 6720 736d 616c 6c20 7661 6c75  dding small valu
+00000c10: 6520 6570 7369 6c6f 6e20 746f 2061 766f  e epsilon to avo
+00000c20: 6964 206c 6f67 206f 6620 300d 0a20 2020  id log of 0..   
+00000c30: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+00000c40: 6574 7572 6e20 636f 7374 202f 2073 656c  eturn cost / sel
+00000c50: 662e 582e 7368 6170 655b 305d 0d0a 0d0a  f.X.shape[0]....
+00000c60: 2020 2020 6465 6620 636f 6d70 7574 655f      def compute_
+00000c70: 6772 6164 6965 6e74 2873 656c 662c 2070  gradient(self, p
+00000c80: 7265 6469 6374 696f 6e73 3a6e 702e 6e64  redictions:np.nd
+00000c90: 6172 7261 7929 202d 3e20 4e6f 6e65 3a0d  array) -> None:.
+00000ca0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00000cb0: 2020 2027 2727 0d0a 2020 2020 2020 2020     '''..        
+00000cc0: 436f 6d70 7574 6573 2074 6865 2067 7261  Computes the gra
+00000cd0: 6469 656e 7473 2066 6f72 2074 6865 206d  dients for the m
+00000ce0: 6f64 656c 2075 7369 6e67 2067 6976 656e  odel using given
+00000cf0: 2070 7265 6469 6374 696f 6e73 2e0d 0a0d   predictions....
+00000d00: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000d10: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+00000d20: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00000d30: 2070 7265 6469 6374 696f 6e73 3a20 6e70   predictions: np
+00000d40: 2e6e 6461 7272 6179 0d0a 2020 2020 2020  .ndarray..      
+00000d50: 2020 2020 2020 5072 6564 6963 7469 6f6e        Prediction
+00000d60: 7320 6f66 2074 6865 206d 6f64 656c 2e0d  s of the model..
+00000d70: 0a20 2020 2020 2020 2027 2727 0d0a 2020  .        '''..  
+00000d80: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000d90: 2320 6765 7420 7472 6169 6e69 6e67 2073  # get training s
+00000da0: 6861 7065 0d0a 2020 2020 2020 2020 6d20  hape..        m 
+00000db0: 3d20 7365 6c66 2e58 2e73 6861 7065 5b30  = self.X.shape[0
+00000dc0: 5d0d 0a0d 0a20 2020 2020 2020 2023 2063  ]....        # c
+00000dd0: 6f6d 7075 7465 2067 7261 6469 656e 7473  ompute gradients
+00000de0: 2061 6e64 2073 6361 6c65 2074 6865 6d0d   and scale them.
+00000df0: 0a20 2020 2020 2020 2073 656c 662e 6457  .        self.dW
+00000e00: 203d 206e 702e 6172 7261 7928 5b6e 702e   = np.array([np.
+00000e10: 6d65 616e 2867 7261 6429 2066 6f72 2067  mean(grad) for g
+00000e20: 7261 6420 696e 205c 0d0a 2020 2020 2020  rad in \..      
+00000e30: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00000e40: 2e6d 6174 6d75 6c28 7365 6c66 2e58 2e54  .matmul(self.X.T
+00000e50: 2c20 2870 7265 6469 6374 696f 6e73 202d  , (predictions -
+00000e60: 2073 656c 662e 7929 2920 5d29 202a 2031   self.y)) ]) * 1
+00000e70: 2f6d 0d0a 2020 2020 2020 2020 7365 6c66  /m..        self
+00000e80: 2e64 6220 3d20 6e70 2e73 756d 286e 702e  .db = np.sum(np.
+00000e90: 7375 6274 7261 6374 2870 7265 6469 6374  subtract(predict
+00000ea0: 696f 6e73 2c20 7365 6c66 2e79 2929 202a  ions, self.y)) *
+00000eb0: 2031 2f6d 0d0a 0d0a 2020 2020 6465 6620   1/m....    def 
+00000ec0: 6669 7428 7365 6c66 2c20 583a 6e70 2e6e  fit(self, X:np.n
+00000ed0: 6461 7272 6179 2c20 793a 6e70 2e6e 6461  darray, y:np.nda
+00000ee0: 7272 6179 2c20 6974 6572 6174 696f 6e73  rray, iterations
+00000ef0: 3a69 6e74 3d31 3030 3030 3030 2c20 0d0a  :int=1000000, ..
+00000f00: 2020 2020 2020 2020 2020 2020 706c 6f74              plot
+00000f10: 5f63 6f73 743a 626f 6f6c 3d54 7275 652c  _cost:bool=True,
+00000f20: 2076 6572 626f 7365 3a62 6f6f 6c3d 5472   verbose:bool=Tr
+00000f30: 7565 2920 2d3e 204e 6f6e 653a 0d0a 0d0a  ue) -> None:....
+00000f40: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
+00000f50: 2020 2020 2054 7261 696e 7320 7468 6520       Trains the 
+00000f60: 6d6f 6465 6c20 6f6e 2067 6976 656e 2069  model on given i
+00000f70: 6e70 7574 2058 2061 6e64 206c 6162 656c  nput X and label
+00000f80: 7320 7920 666f 7220 7370 6563 6966 6965  s y for specifie
+00000f90: 6420 6974 6572 6174 696f 6e73 2e0d 0a0d  d iterations....
+00000fa0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00000fb0: 6572 730d 0a20 2020 2020 2020 202d 2d2d  ers..        ---
+00000fc0: 2d2d 2d2d 2d2d 2d0d 0a20 2020 2020 2020  -------..       
+00000fd0: 2058 3a20 6e70 2e6e 6461 7272 6179 0d0a   X: np.ndarray..
+00000fe0: 2020 2020 2020 2020 2020 2020 5472 6169              Trai
+00000ff0: 6e69 6e67 2069 6e70 7574 2064 6174 6120  ning input data 
+00001000: 6f66 2073 6861 7065 2028 6d2c 206e 5f66  of shape (m, n_f
+00001010: 6561 7475 7265 7329 2e0d 0a20 2020 2020  eatures)...     
+00001020: 2020 2079 3a20 6e70 2e6e 6461 7272 6179     y: np.ndarray
+00001030: 0d0a 2020 2020 2020 2020 2020 2020 5472  ..            Tr
+00001040: 6169 6e69 6e67 206c 6162 656c 7320 6f66  aining labels of
+00001050: 2073 6861 7065 2028 6d2c 292e 0d0a 2020   shape (m,)...  
+00001060: 2020 2020 2020 6974 6572 6174 696f 6e73        iterations
+00001070: 3a20 696e 740d 0a20 2020 2020 2020 2020  : int..         
+00001080: 2020 2054 6865 206e 756d 6265 7220 6f66     The number of
+00001090: 2069 7465 7261 7469 6f6e 7320 666f 7220   iterations for 
+000010a0: 6772 6164 6965 6e74 2064 6573 6365 6e74  gradient descent
+000010b0: 2e20 416c 736f 206e 616d 6564 2065 706f  . Also named epo
+000010c0: 6368 732e 0d0a 2020 2020 2020 2020 706c  chs...        pl
+000010d0: 6f74 5f63 6f73 743a 2062 6f6f 6c0d 0a20  ot_cost: bool.. 
+000010e0: 2020 2020 2020 2020 2020 2057 6865 7468             Wheth
+000010f0: 6572 2074 6f20 706c 6f74 2074 6865 2063  er to plot the c
+00001100: 6f73 7420 6475 7269 6e67 2074 7261 696e  ost during train
+00001110: 696e 672e 2044 6566 6175 6c74 7320 746f  ing. Defaults to
+00001120: 2054 7275 652e 0d0a 2020 2020 2020 2020   True...        
+00001130: 7665 7262 6f73 653a 2062 6f6f 6c0d 0a20  verbose: bool.. 
+00001140: 2020 2020 2020 2020 2020 2054 7275 6520             True 
+00001150: 746f 2070 7269 6e74 2074 7261 696e 696e  to print trainin
+00001160: 6720 7265 7375 6c74 732e 0d0a 0d0a 2020  g results.....  
+00001170: 2020 2020 2020 5261 6973 6573 0d0a 2020        Raises..  
+00001180: 2020 2020 2020 2d2d 2d2d 2d2d 0d0a 2020        ------..  
+00001190: 2020 2020 2020 4173 7365 7274 696f 6e45        AssertionE
+000011a0: 7272 6f72 3a20 4966 2069 6e70 7574 2064  rror: If input d
+000011b0: 6174 6120 616e 6420 6c61 6265 6c73 2061  ata and labels a
+000011c0: 7265 206e 6f74 204e 756d 5079 2061 7272  re not NumPy arr
+000011d0: 6179 7320 6f72 2068 6176 6520 6d69 736d  ays or have mism
+000011e0: 6174 6368 6564 2073 6861 7065 732e 0d0a  atched shapes...
+000011f0: 0d0a 2020 2020 2020 2020 506c 6f74 730d  ..        Plots.
+00001200: 0a20 2020 2020 2020 202d 2d2d 2d2d 0d0a  .        -----..
+00001210: 2020 2020 2020 2020 506c 6f74 6c79 206c          Plotly l
+00001220: 696e 6520 6368 6172 7420 7368 6f77 696e  ine chart showin
+00001230: 6720 636f 7374 2076 732e 2069 7465 7261  g cost vs. itera
+00001240: 7469 6f6e 2028 6966 2070 6c6f 745f 636f  tion (if plot_co
+00001250: 7374 2069 7320 5472 7565 292e 0d0a 2020  st is True)...  
+00001260: 2020 2020 2020 2727 270d 0a20 2020 2020        '''..     
+00001270: 2020 200d 0a20 2020 2020 2020 2061 7373     ..        ass
+00001280: 6572 7420 6973 696e 7374 616e 6365 2858  ert isinstance(X
+00001290: 2c20 6e70 2e6e 6461 7272 6179 292c 2022  , np.ndarray), "
+000012a0: 5820 6d75 7374 2062 6520 6120 4e75 6d50  X must be a NumP
+000012b0: 7920 6172 7261 7922 0d0a 2020 2020 2020  y array"..      
+000012c0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+000012d0: 6e63 6528 792c 206e 702e 6e64 6172 7261  nce(y, np.ndarra
+000012e0: 7929 2c20 2279 206d 7573 7420 6265 2061  y), "y must be a
+000012f0: 204e 756d 5079 2061 7272 6179 220d 0a20   NumPy array".. 
+00001300: 2020 2020 2020 2061 7373 6572 7420 582e         assert X.
+00001310: 7368 6170 655b 305d 203d 3d20 792e 7368  shape[0] == y.sh
+00001320: 6170 655b 305d 2c20 2258 2061 6e64 2079  ape[0], "X and y
+00001330: 206d 7573 7420 6861 7665 2074 6865 2073   must have the s
+00001340: 616d 6520 6e75 6d62 6572 206f 6620 7361  ame number of sa
+00001350: 6d70 6c65 7322 0d0a 2020 2020 2020 2020  mples"..        
+00001360: 6173 7365 7274 2069 7465 7261 7469 6f6e  assert iteration
+00001370: 7320 3e20 302c 2022 4974 6572 6174 696f  s > 0, "Iteratio
+00001380: 6e73 206d 7573 7420 6265 2067 7265 6174  ns must be great
+00001390: 6572 2074 6861 6e20 3022 0d0a 2020 2020  er than 0"..    
+000013a0: 2020 2020 0d0a 2020 2020 2020 2020 5820      ..        X 
+000013b0: 3d20 5820 6966 2072 6f75 6e64 286e 702e  = X if round(np.
+000013c0: 6d65 616e 2858 2929 203d 3d20 3020 616e  mean(X)) == 0 an
+000013d0: 6420 726f 756e 6428 6e70 2e73 7464 2858  d round(np.std(X
+000013e0: 2929 203d 3d20 3120 656c 7365 2075 7469  )) == 1 else uti
+000013f0: 6c73 2e73 6361 6c65 2858 290d 0a20 2020  ls.scale(X)..   
+00001400: 2020 2020 2073 656c 662e 5820 3d20 580d       self.X = X.
+00001410: 0a20 2020 2020 2020 2073 656c 662e 7920  .        self.y 
+00001420: 3d20 790d 0a20 2020 2020 2020 2073 656c  = y..        sel
+00001430: 662e 696e 6974 6961 6c69 7a65 5f70 6172  f.initialize_par
+00001440: 616d 6574 6572 2829 0d0a 2020 2020 2020  ameter()..      
+00001450: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00001460: 2e64 575f 6869 7374 2c20 7365 6c66 2e64  .dW_hist, self.d
+00001470: 625f 6869 7374 2c20 7365 6c66 2e57 5f68  b_hist, self.W_h
+00001480: 6973 742c 2073 656c 662e 625f 6869 7374  ist, self.b_hist
+00001490: 2c20 7365 6c66 2e63 6f73 7473 203d 205b  , self.costs = [
+000014a0: 5d2c 205b 5d2c 205b 5d2c 205b 5d2c 205b  ], [], [], [], [
+000014b0: 5d0d 0a0d 0a20 2020 2020 2020 2066 6f72  ]....        for
+000014c0: 2069 2069 6e20 7261 6e67 6528 6974 6572   i in range(iter
+000014d0: 6174 696f 6e73 293a 0d0a 2020 2020 2020  ations):..      
+000014e0: 2020 2020 2020 2320 666f 7277 6172 6420        # forward 
+000014f0: 7072 6f70 6167 6174 696f 6e0d 0a20 2020  propagation..   
+00001500: 2020 2020 2020 2020 2070 7265 6469 6374           predict
+00001510: 696f 6e73 203d 2073 656c 662e 666f 7277  ions = self.forw
+00001520: 6172 6428 7365 6c66 2e58 290d 0a0d 0a20  ard(self.X).... 
+00001530: 2020 2020 2020 2020 2020 2023 2063 6f6d             # com
+00001540: 7075 7465 2063 6f73 740d 0a20 2020 2020  pute cost..     
+00001550: 2020 2020 2020 2073 656c 662e 636f 7374         self.cost
+00001560: 203d 2073 656c 662e 636f 6d70 7574 655f   = self.compute_
+00001570: 636f 7374 2870 7265 6469 6374 696f 6e73  cost(predictions
+00001580: 290d 0a0d 0a20 2020 2020 2020 2020 2020  )....           
+00001590: 2023 2063 6f6d 7075 7465 2067 7261 6469   # compute gradi
+000015a0: 656e 7473 0d0a 2020 2020 2020 2020 2020  ents..          
+000015b0: 2020 7365 6c66 2e63 6f6d 7075 7465 5f67    self.compute_g
+000015c0: 7261 6469 656e 7428 7072 6564 6963 7469  radient(predicti
+000015d0: 6f6e 7329 0d0a 0d0a 2020 2020 2020 2020  ons)....        
+000015e0: 2020 2020 2320 7570 6461 7465 2070 6172      # update par
+000015f0: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+00001600: 2020 2020 2073 656c 662e 5720 3d20 7365       self.W = se
+00001610: 6c66 2e57 202d 2073 656c 662e 6c65 6172  lf.W - self.lear
+00001620: 6e69 6e67 5f72 6174 6520 2a20 7365 6c66  ning_rate * self
+00001630: 2e64 570d 0a20 2020 2020 2020 2020 2020  .dW..           
+00001640: 2073 656c 662e 6220 3d20 7365 6c66 2e62   self.b = self.b
+00001650: 202d 2073 656c 662e 6c65 6172 6e69 6e67   - self.learning
+00001660: 5f72 6174 6520 2a20 7365 6c66 2e64 620d  _rate * self.db.
+00001670: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00001680: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001690: 636f 7374 732e 6170 7065 6e64 2873 656c  costs.append(sel
+000016a0: 662e 636f 7374 290d 0a20 2020 2020 2020  f.cost)..       
+000016b0: 2020 2020 2073 656c 662e 6457 5f68 6973       self.dW_his
+000016c0: 742e 6170 7065 6e64 2873 656c 662e 6457  t.append(self.dW
+000016d0: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
+000016e0: 656c 662e 6462 5f68 6973 742e 6170 7065  elf.db_hist.appe
+000016f0: 6e64 2873 656c 662e 6462 290d 0a20 2020  nd(self.db)..   
+00001700: 2020 2020 2020 2020 2073 656c 662e 575f           self.W_
+00001710: 6869 7374 2e61 7070 656e 6428 7365 6c66  hist.append(self
+00001720: 2e57 290d 0a20 2020 2020 2020 2020 2020  .W)..           
+00001730: 2073 656c 662e 625f 6869 7374 2e61 7070   self.b_hist.app
+00001740: 656e 6428 7365 6c66 2e62 290d 0a0d 0a20  end(self.b).... 
+00001750: 2020 2020 2020 2020 2020 2023 2070 7269             # pri
+00001760: 6e74 2063 6f73 7420 6576 6572 7920 3130  nt cost every 10
+00001770: 3020 6974 6572 6174 696f 6e73 0d0a 2020  0 iterations..  
+00001780: 2020 2020 2020 2020 2020 6966 2069 2025            if i %
+00001790: 2031 3030 3030 203d 3d20 3020 616e 6420   10000 == 0 and 
+000017a0: 7665 7262 6f73 653a 0d0a 2020 2020 2020  verbose:..      
+000017b0: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+000017c0: 6627 436f 7374 2061 6674 6572 2069 7465  f'Cost after ite
+000017d0: 7261 7469 6f6e 207b 697d 3a20 7b73 656c  ration {i}: {sel
+000017e0: 662e 636f 7374 7d27 290d 0a0d 0a20 2020  f.cost}')....   
+000017f0: 2020 2020 2020 2020 2069 6620 6920 3e20           if i > 
+00001800: 3020 616e 6420 6162 7328 7365 6c66 2e63  0 and abs(self.c
+00001810: 6f73 7473 5b2d 315d 202d 2073 656c 662e  osts[-1] - self.
+00001820: 636f 7374 735b 2d32 5d29 203c 2073 656c  costs[-2]) < sel
+00001830: 662e 636f 6e76 6572 6765 6e63 655f 746f  f.convergence_to
+00001840: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
+00001850: 2020 2020 7072 696e 7428 6627 436f 6e76      print(f'Conv
+00001860: 6572 6765 6420 6166 7465 7220 7b69 7d20  erged after {i} 
+00001870: 6974 6572 6174 696f 6e73 2e27 290d 0a20  iterations.').. 
+00001880: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00001890: 7265 616b 0d0a 0d0a 2020 2020 2020 2020  reak....        
+000018a0: 6966 2070 6c6f 745f 636f 7374 3a0d 0a20  if plot_cost:.. 
+000018b0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000018c0: 706c 6f74 436f 7374 7328 290d 0a20 2020  plotCosts()..   
+000018d0: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+000018e0: 6566 2070 6c6f 7443 6f73 7473 2873 656c  ef plotCosts(sel
+000018f0: 662c 2074 656d 706c 6174 653a 7374 723d  f, template:str=
+00001900: 2770 6c6f 746c 795f 6461 726b 272c 2063  'plotly_dark', c
+00001910: 6f6c 6f72 3a73 7472 3d27 2334 3142 4545  olor:str='#41BEE
+00001920: 3927 2920 2d3e 204e 6f6e 653a 0d0a 2020  9') -> None:..  
+00001930: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00001940: 2727 270d 0a20 2020 2020 2020 2050 6c6f  '''..        Plo
+00001950: 746c 7920 6c69 6e65 2063 6861 7274 2073  tly line chart s
+00001960: 686f 7769 6e67 2063 6f73 7420 7673 2e20  howing cost vs. 
+00001970: 6974 6572 6174 696f 6e2e 0d0a 0d0a 2020  iteration.....  
+00001980: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00001990: 0d0a 2020 2020 2020 2020 2d2d 2d2d 2d2d  ..        ------
+000019a0: 2d2d 2d2d 0d0a 2020 2020 2020 2020 7465  ----..        te
+000019b0: 6d70 6c61 7465 3a20 7374 720d 0a20 2020  mplate: str..   
+000019c0: 2020 2020 2020 2020 2054 656d 706c 6174           Templat
+000019d0: 6520 6672 6f6d 2074 6865 206c 6973 7420  e from the list 
+000019e0: 6176 6169 6c61 626c 653a 205b 2767 6770  available: ['ggp
+000019f0: 6c6f 7432 272c 2027 7365 6162 6f72 6e27  lot2', 'seaborn'
+00001a00: 2c20 2773 696d 706c 655f 7768 6974 6527  , 'simple_white'
+00001a10: 2c20 2770 6c6f 746c 7927 2c0d 0a20 2020  , 'plotly',..   
+00001a20: 2020 2020 2020 2020 2027 706c 6f74 6c79           'plotly
+00001a30: 5f77 6869 7465 272c 2027 706c 6f74 6c79  _white', 'plotly
+00001a40: 5f64 6172 6b27 2c20 2770 7265 7365 6e74  _dark', 'present
+00001a50: 6174 696f 6e27 2c20 2778 6772 6964 6f66  ation', 'xgridof
+00001a60: 6627 2c0d 0a20 2020 2020 2020 2020 2020  f',..           
+00001a70: 2027 7967 7269 646f 6666 272c 2027 6772   'ygridoff', 'gr
+00001a80: 6964 6f6e 272c 2027 6e6f 6e65 275d 2e20  idon', 'none']. 
+00001a90: 4465 6661 756c 7473 2074 6f20 2770 6c6f  Defaults to 'plo
+00001aa0: 746c 795f 6461 726b 272e 0d0a 2020 2020  tly_dark'...    
+00001ab0: 2020 2020 636f 6c6f 723a 2073 7472 0d0a      color: str..
+00001ac0: 2020 2020 2020 2020 2020 2020 4865 7861              Hexa
+00001ad0: 6765 7369 6d61 6c20 636f 6c6f 722e 0d0a  gesimal color...
+00001ae0: 0d0a 2020 2020 2020 2020 506c 6f74 730d  ..        Plots.
+00001af0: 0a20 2020 2020 2020 202d 2d2d 2d2d 0d0a  .        -----..
+00001b00: 2020 2020 2020 2020 506c 6f74 6c79 206c          Plotly l
+00001b10: 696e 6520 6368 6172 7420 7368 6f77 696e  ine chart showin
+00001b20: 6720 636f 7374 2076 732e 2069 7465 7261  g cost vs. itera
+00001b30: 7469 6f6e 2e0d 0a20 2020 2020 2020 2027  tion...        '
+00001b40: 2727 0d0a 2020 2020 2020 2020 0d0a 2020  ''..        ..  
+00001b50: 2020 2020 2020 6669 6720 3d20 7078 2e6c        fig = px.l
+00001b60: 696e 6528 793d 7365 6c66 2e63 6f73 7473  ine(y=self.costs
+00001b70: 2c20 7469 746c 653d 2243 6f73 7420 7673  , title="Cost vs
+00001b80: 2049 7465 7261 7469 6f6e 222c 2074 656d   Iteration", tem
+00001b90: 706c 6174 653d 7465 6d70 6c61 7465 290d  plate=template).
+00001ba0: 0a20 2020 2020 2020 2066 6967 2e75 7064  .        fig.upd
+00001bb0: 6174 655f 6c61 796f 7574 280d 0a20 2020  ate_layout(..   
+00001bc0: 2020 2020 2020 2020 2074 6974 6c65 5f66           title_f
+00001bd0: 6f6e 745f 636f 6c6f 723d 636f 6c6f 722c  ont_color=color,
+00001be0: 0d0a 2020 2020 2020 2020 2020 2020 7861  ..            xa
+00001bf0: 7869 733d 6469 6374 2863 6f6c 6f72 3d63  xis=dict(color=c
+00001c00: 6f6c 6f72 2c20 7469 746c 653d 2249 7465  olor, title="Ite
+00001c10: 7261 7469 6f6e 7322 292c 0d0a 2020 2020  rations"),..    
+00001c20: 2020 2020 2020 2020 7961 7869 733d 6469          yaxis=di
+00001c30: 6374 2863 6f6c 6f72 3d63 6f6c 6f72 2c20  ct(color=color, 
+00001c40: 7469 746c 653d 2243 6f73 7422 290d 0a20  title="Cost").. 
+00001c50: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00001c60: 2020 6669 672e 7368 6f77 2829 0d0a 0d0a    fig.show()....
+00001c70: 2020 2020 6465 6620 7072 6564 6963 7428      def predict(
+00001c80: 7365 6c66 2c20 583a 6e70 2e6e 6461 7272  self, X:np.ndarr
+00001c90: 6179 2920 2d3e 206e 702e 6e64 6172 7261  ay) -> np.ndarra
+00001ca0: 793a 0d0a 0d0a 2020 2020 2020 2020 2727  y:....        ''
+00001cb0: 270d 0a20 2020 2020 2020 2050 7265 6469  '..        Predi
+00001cc0: 6374 2074 6172 6765 7420 7661 6c75 6573  ct target values
+00001cd0: 2066 6f72 206e 6577 2069 6e70 7574 2064   for new input d
+00001ce0: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
+00001cf0: 5061 7261 6d65 7465 7273 0d0a 2020 2020  Parameters..    
+00001d00: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a      ----------..
+00001d10: 2020 2020 2020 2020 583a 206e 702e 6e64          X: np.nd
+00001d20: 6172 7261 790d 0a20 2020 2020 2020 2020  array..         
+00001d30: 2020 2049 6e70 7574 2064 6174 6120 6f66     Input data of
+00001d40: 2073 6861 7065 2028 6d2c 206e 5f66 6561   shape (m, n_fea
+00001d50: 7475 7265 7329 2e0d 0a0d 0a20 2020 2020  tures).....     
+00001d60: 2020 2052 6574 7572 6e73 0d0a 2020 2020     Returns..    
+00001d70: 2020 2020 2d2d 2d2d 2d2d 2d0d 0a20 2020      -------..   
+00001d80: 2020 2020 2072 6574 7572 6e3a 206e 702e       return: np.
+00001d90: 6e64 6172 7261 790d 0a20 2020 2020 2020  ndarray..       
+00001da0: 2020 2020 2050 7265 6469 6374 6564 2074       Predicted t
+00001db0: 6172 6765 7420 7661 6c75 6573 206f 6620  arget values of 
+00001dc0: 7368 6170 6520 286d 2c29 2e0d 0a20 2020  shape (m,)...   
+00001dd0: 2020 2020 2027 2727 0d0a 2020 2020 2020       '''..      
+00001de0: 2020 0d0a 2020 2020 2020 2020 5820 3d20    ..        X = 
+00001df0: 5820 6966 2072 6f75 6e64 286e 702e 6d65  X if round(np.me
+00001e00: 616e 2858 2929 203d 3d20 3020 616e 6420  an(X)) == 0 and 
+00001e10: 726f 756e 6428 6e70 2e73 7464 2858 2929  round(np.std(X))
+00001e20: 203d 3d20 3120 656c 7365 2075 7469 6c73   == 1 else utils
+00001e30: 2e73 6361 6c65 2858 290d 0a20 2020 2020  .scale(X)..     
+00001e40: 2020 2073 656c 662e 5820 3d20 580d 0a20     self.X = X.. 
+00001e50: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00001e60: 2072 6574 7572 6e20 6e70 2e72 6f75 6e64   return np.round
+00001e70: 2873 656c 662e 666f 7277 6172 6428 5829  (self.forward(X)
+00001e80: 290d 0a20 2020 200d 0a20 2020 2064 6566  )..    ..    def
+00001e90: 2067 6574 5765 6967 6874 7328 7365 6c66   getWeights(self
+00001ea0: 2c20 6665 6174 7572 6573 3a6c 6973 7429  , features:list)
+00001eb0: 202d 3e20 7064 2e44 6174 6146 7261 6d65   -> pd.DataFrame
+00001ec0: 3a0d 0a0d 0a20 2020 2020 2020 2027 2727  :....        '''
+00001ed0: 0d0a 2020 2020 2020 2020 4765 7420 7468  ..        Get th
+00001ee0: 6520 7765 6967 6874 7320 6672 6f6d 2074  e weights from t
+00001ef0: 6865 206c 6173 7420 7472 6169 6e69 6e67  he last training
+00001f00: 2e0d 0a0d 0a20 2020 2020 2020 2050 6172  .....        Par
+00001f10: 616d 6574 6572 730d 0a20 2020 2020 2020  ameters..       
+00001f20: 202d 2d2d 2d2d 2d2d 2d2d 2d0d 0a20 2020   ----------..   
+00001f30: 2020 2020 2066 6561 7475 7265 733a 206c       features: l
+00001f40: 6973 740d 0a20 2020 2020 2020 2020 2020  ist..           
+00001f50: 204c 6973 7420 6f66 2074 6865 2066 6561   List of the fea
+00001f60: 7475 7265 7320 6e61 6d65 7320 6173 736f  tures names asso
+00001f70: 6369 6174 6564 2074 6f20 7468 6520 7765  ciated to the we
+00001f80: 6967 6874 732e 0d0a 0d0a 2020 2020 2020  ights.....      
+00001f90: 2020 5265 7475 726e 730d 0a20 2020 2020    Returns..     
+00001fa0: 2020 202d 2d2d 2d2d 2d2d 0d0a 2020 2020     -------..    
+00001fb0: 2020 2020 7265 7475 726e 3a20 7064 2e44      return: pd.D
+00001fc0: 6174 6146 7261 6d65 0d0a 2020 2020 2020  ataFrame..      
+00001fd0: 2020 2020 2020 4461 7461 4672 616d 6520        DataFrame 
+00001fe0: 636f 6e74 6169 6e69 6e67 2074 6865 2077  containing the w
+00001ff0: 6569 6768 7473 2072 616e 6b65 642e 0d0a  eights ranked...
+00002000: 2020 2020 2020 2020 2727 270d 0a20 2020          '''..   
+00002010: 2020 2020 200d 0a20 2020 2020 2020 2072       ..        r
+00002020: 6574 7572 6e20 7064 2e44 6174 6146 7261  eturn pd.DataFra
+00002030: 6d65 287b 2757 6569 6768 7473 273a 7365  me({'Weights':se
+00002040: 6c66 2e57 7d2c 2069 6e64 6578 3d66 6561  lf.W}, index=fea
+00002050: 7475 7265 7329 205c 0d0a 2020 2020 2020  tures) \..      
+00002060: 2020 2020 2020 2020 2020 2e73 6f72 745f            .sort_
+00002070: 7661 6c75 6573 2862 793d 2757 6569 6768  values(by='Weigh
+00002080: 7473 272c 2061 7363 656e 6469 6e67 3d46  ts', ascending=F
+00002090: 616c 7365 290d 0a20 2020 200d 0a20 2020  alse)..    ..   
+000020a0: 2064 6566 2073 6176 655f 6d6f 6465 6c28   def save_model(
+000020b0: 7365 6c66 2c20 6669 6c65 6e61 6d65 3a73  self, filename:s
+000020c0: 7472 3d27 6c61 7374 5f4c 6f67 5265 675f  tr='last_LogReg_
+000020d0: 6d6f 6465 6c2e 706b 6c27 2920 2d3e 204e  model.pkl') -> N
+000020e0: 6f6e 653a 0d0a 0d0a 2020 2020 2020 2020  one:....        
+000020f0: 2727 270d 0a20 2020 2020 2020 2053 6176  '''..        Sav
+00002100: 6520 7468 6520 7472 6169 6e65 6420 6d6f  e the trained mo
+00002110: 6465 6c20 746f 2061 2066 696c 6520 7573  del to a file us
+00002120: 696e 6720 7069 636b 6c65 2e0d 0a0d 0a20  ing pickle..... 
+00002130: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00002140: 730d 0a20 2020 2020 2020 202d 2d2d 2d2d  s..        -----
+00002150: 2d2d 2d2d 2d0d 0a20 2020 2020 2020 2066  -----..        f
+00002160: 696c 656e 616d 653a 2073 7472 0d0a 2020  ilename: str..  
+00002170: 2020 2020 2020 2020 2020 5468 6520 6e61            The na
+00002180: 6d65 206f 6620 7468 6520 6669 6c65 2074  me of the file t
+00002190: 6f20 7361 7665 2074 6865 206d 6f64 656c  o save the model
+000021a0: 2074 6f2e 0d0a 2020 2020 2020 2020 2727   to...        ''
+000021b0: 270d 0a0d 0a20 2020 2020 2020 206d 6f64  '....        mod
+000021c0: 656c 5f64 6174 6120 3d20 7b0d 0a20 2020  el_data = {..   
+000021d0: 2020 2020 2020 2020 2027 6c65 6172 6e69           'learni
+000021e0: 6e67 5f72 6174 6527 3a20 7365 6c66 2e6c  ng_rate': self.l
+000021f0: 6561 726e 696e 675f 7261 7465 2c0d 0a20  earning_rate,.. 
+00002200: 2020 2020 2020 2020 2020 2027 636f 6e76             'conv
+00002210: 6572 6765 6e63 655f 746f 6c27 3a20 7365  ergence_tol': se
+00002220: 6c66 2e63 6f6e 7665 7267 656e 6365 5f74  lf.convergence_t
+00002230: 6f6c 2c0d 0a20 2020 2020 2020 2020 2020  ol,..           
+00002240: 2027 5727 3a20 7365 6c66 2e57 2c0d 0a20   'W': self.W,.. 
+00002250: 2020 2020 2020 2020 2020 2027 6227 3a20             'b': 
+00002260: 7365 6c66 2e62 0d0a 2020 2020 2020 2020  self.b..        
+00002270: 7d0d 0a0d 0a20 2020 2020 2020 2077 6974  }....        wit
+00002280: 6820 6f70 656e 2866 696c 656e 616d 652c  h open(filename,
+00002290: 2027 7762 2729 2061 7320 6669 6c65 3a0d   'wb') as file:.
+000022a0: 0a20 2020 2020 2020 2020 2020 2070 6963  .            pic
+000022b0: 6b6c 652e 6475 6d70 286d 6f64 656c 5f64  kle.dump(model_d
+000022c0: 6174 612c 2066 696c 6529 0d0a 0d0a 2020  ata, file)....  
+000022d0: 2020 4063 6c61 7373 6d65 7468 6f64 0d0a    @classmethod..
+000022e0: 2020 2020 6465 6620 6c6f 6164 5f6d 6f64      def load_mod
+000022f0: 656c 2863 6c73 2c20 6669 6c65 6e61 6d65  el(cls, filename
+00002300: 3a73 7472 3d27 6c61 7374 5f4c 6f67 5265  :str='last_LogRe
+00002310: 675f 6d6f 6465 6c2e 706b 6c27 293a 0d0a  g_model.pkl'):..
+00002320: 0d0a 2020 2020 2020 2020 2727 270d 0a20  ..        '''.. 
+00002330: 2020 2020 2020 204c 6f61 6420 6120 7472         Load a tr
+00002340: 6169 6e65 6420 6d6f 6465 6c20 6672 6f6d  ained model from
+00002350: 2061 2066 696c 6520 7573 696e 6720 7069   a file using pi
+00002360: 636b 6c65 2e0d 0a0d 0a20 2020 2020 2020  ckle.....       
+00002370: 2050 6172 616d 6574 6572 730d 0a20 2020   Parameters..   
+00002380: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0d       ----------.
+00002390: 0a20 2020 2020 2020 2066 696c 656e 616d  .        filenam
+000023a0: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
+000023b0: 2020 2020 5468 6520 6e61 6d65 206f 6620      The name of 
+000023c0: 7468 6520 6669 6c65 2074 6f20 6c6f 6164  the file to load
+000023d0: 2074 6865 206d 6f64 656c 2066 726f 6d2e   the model from.
+000023e0: 0d0a 0d0a 2020 2020 2020 2020 5265 7475  ....        Retu
+000023f0: 726e 730d 0a20 2020 2020 2020 202d 2d2d  rns..        ---
+00002400: 2d2d 2d2d 0d0a 2020 2020 2020 2020 6c6f  ----..        lo
+00002410: 6164 6564 5f6d 6f64 656c 3a20 4c6f 6769  aded_model: Logi
+00002420: 7374 6963 5265 6772 6573 7369 6f6e 0d0a  sticRegression..
+00002430: 2020 2020 2020 2020 2020 2020 416e 2069              An i
+00002440: 6e73 7461 6e63 6520 6f66 2074 6865 204c  nstance of the L
+00002450: 6f67 6973 7469 6352 6567 7265 7373 696f  ogisticRegressio
+00002460: 6e20 636c 6173 7320 7769 7468 206c 6f61  n class with loa
+00002470: 6465 6420 7061 7261 6d65 7465 7273 2e0d  ded parameters..
+00002480: 0a20 2020 2020 2020 2027 2727 0d0a 0d0a  .        '''....
+00002490: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
+000024a0: 6e28 6669 6c65 6e61 6d65 2c20 2772 6227  n(filename, 'rb'
+000024b0: 2920 6173 2066 696c 653a 0d0a 2020 2020  ) as file:..    
+000024c0: 2020 2020 2020 2020 6d6f 6465 6c5f 6461          model_da
+000024d0: 7461 203d 2070 6963 6b6c 652e 6c6f 6164  ta = pickle.load
+000024e0: 2866 696c 6529 0d0a 0d0a 2020 2020 2020  (file)....      
+000024f0: 2020 2320 4372 6561 7465 2061 206e 6577    # Create a new
+00002500: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+00002510: 2063 6c61 7373 2061 6e64 2069 6e69 7469   class and initi
+00002520: 616c 697a 6520 6974 2077 6974 6820 7468  alize it with th
+00002530: 6520 6c6f 6164 6564 2070 6172 616d 6574  e loaded paramet
+00002540: 6572 730d 0a20 2020 2020 2020 206c 6f61  ers..        loa
+00002550: 6465 645f 6d6f 6465 6c20 3d20 636c 7328  ded_model = cls(
+00002560: 6d6f 6465 6c5f 6461 7461 5b27 6c65 6172  model_data['lear
+00002570: 6e69 6e67 5f72 6174 6527 5d2c 206d 6f64  ning_rate'], mod
+00002580: 656c 5f64 6174 615b 2763 6f6e 7665 7267  el_data['converg
+00002590: 656e 6365 5f74 6f6c 275d 290d 0a20 2020  ence_tol'])..   
+000025a0: 2020 2020 206c 6f61 6465 645f 6d6f 6465       loaded_mode
+000025b0: 6c2e 5720 3d20 6d6f 6465 6c5f 6461 7461  l.W = model_data
+000025c0: 5b27 5727 5d0d 0a20 2020 2020 2020 206c  ['W']..        l
+000025d0: 6f61 6465 645f 6d6f 6465 6c2e 6220 3d20  oaded_model.b = 
+000025e0: 6d6f 6465 6c5f 6461 7461 5b27 6227 5d0d  model_data['b'].
+000025f0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+00002600: 6e20 6c6f 6164 6564 5f6d 6f64 656c 0d0a  n loaded_model..
+00002610: 0d0a 2020 2020 6465 6620 706c 6f74 5072  ..    def plotPr
+00002620: 6564 6963 7469 6f6e 2873 656c 662c 2058  ediction(self, X
+00002630: 3a6e 702e 6e64 6172 7261 793d 4e6f 6e65  :np.ndarray=None
+00002640: 2c20 793a 6e70 2e6e 6461 7272 6179 3d4e  , y:np.ndarray=N
+00002650: 6f6e 6529 202d 3e20 4e6f 6e65 3a0d 0a20  one) -> None:.. 
+00002660: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002670: 2027 2727 0d0a 2020 2020 2020 2020 506c   '''..        Pl
+00002680: 6f74 6c79 2063 6861 7274 2063 6f6e 7461  otly chart conta
+00002690: 696e 696e 6720 7468 6520 7265 616c 2064  ining the real d
+000026a0: 6174 6120 616e 6420 7468 6520 7072 6564  ata and the pred
+000026b0: 6963 7469 6f6e 2e0d 0a0d 0a20 2020 2020  iction.....     
+000026c0: 2020 2050 6172 616d 6574 6572 730d 0a20     Parameters.. 
+000026d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000026e0: 2d0d 0a20 2020 2020 2020 2058 3a20 6e70  -..        X: np
+000026f0: 2e6e 6461 7272 6179 0d0a 2020 2020 2020  .ndarray..      
+00002700: 2020 2020 2020 496e 7075 7420 6461 7461        Input data
+00002710: 206f 6620 7368 6170 6520 286d 2c20 6e5f   of shape (m, n_
+00002720: 6665 6174 7572 6573 292e 0d0a 2020 2020  features)...    
+00002730: 2020 2020 793a 206e 702e 6e64 6172 7261      y: np.ndarra
+00002740: 790d 0a20 2020 2020 2020 2020 2020 2044  y..            D
+00002750: 6174 6120 746f 2070 7265 6469 6374 206f  ata to predict o
+00002760: 6620 7368 6170 6520 286d 2c20 292e 0d0a  f shape (m, )...
+00002770: 0d0a 2020 2020 2020 2020 506c 6f74 730d  ..        Plots.
+00002780: 0a20 2020 2020 2020 202d 2d2d 2d2d 0d0a  .        -----..
+00002790: 2020 2020 2020 2020 506c 6f74 6c79 2063          Plotly c
+000027a0: 6861 7274 2063 6f6e 7461 696e 696e 6720  hart containing 
+000027b0: 7468 6520 7265 616c 2064 6174 6120 616e  the real data an
+000027c0: 6420 7468 6520 7072 6564 6963 7469 6f6e  d the prediction
+000027d0: 2e0d 0a20 2020 2020 2020 2027 2727 0d0a  ...        '''..
+000027e0: 0d0a 2020 2020 2020 2020 5820 3d20 7365  ..        X = se
+000027f0: 6c66 2e58 2069 6620 6e6f 7420 6973 696e  lf.X if not isin
+00002800: 7374 616e 6365 2858 2c20 6e70 2e6e 6461  stance(X, np.nda
+00002810: 7272 6179 2920 656c 7365 2058 0d0a 2020  rray) else X..  
+00002820: 2020 2020 2020 7920 3d20 7365 6c66 2e79        y = self.y
+00002830: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00002840: 6365 2879 2c20 6e70 2e6e 6461 7272 6179  ce(y, np.ndarray
+00002850: 2920 656c 7365 2079 0d0a 2020 2020 2020  ) else y..      
+00002860: 2020 0d0a 2020 2020 2020 2020 696d 706f    ..        impo
+00002870: 7274 2070 6c6f 746c 792e 6772 6170 685f  rt plotly.graph_
+00002880: 6f62 6a73 2061 7320 676f 0d0a 2020 2020  objs as go..    
+00002890: 2020 2020 6669 6720 3d20 676f 2e46 6967      fig = go.Fig
+000028a0: 7572 6528 5b0d 0a20 2020 2020 2020 2020  ure([..         
+000028b0: 2020 2067 6f2e 5363 6174 7465 7228 0d0a     go.Scatter(..
+000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028d0: 6e61 6d65 3d27 4461 7461 272c 0d0a 2020  name='Data',..  
+000028e0: 2020 2020 2020 2020 2020 2020 2020 793d                y=
+000028f0: 792c 0d0a 2020 2020 2020 2020 2020 2020  y,..            
+00002900: 2020 2020 6d6f 6465 3d27 6d61 726b 6572      mode='marker
+00002910: 7327 2c0d 0a20 2020 2020 2020 2020 2020  s',..           
+00002920: 2020 2020 206d 6172 6b65 723d 6469 6374       marker=dict
+00002930: 2863 6f6c 6f72 3d27 7265 6427 2c20 7369  (color='red', si
+00002940: 7a65 3d32 292c 0d0a 2020 2020 2020 2020  ze=2),..        
+00002950: 2020 2020 2020 2020 7368 6f77 6c65 6765          showlege
+00002960: 6e64 3d54 7275 650d 0a20 2020 2020 2020  nd=True..       
+00002970: 2020 2020 2029 2c0d 0a20 2020 2020 2020       ),..       
+00002980: 2020 2020 2067 6f2e 5363 6174 7465 7228       go.Scatter(
+00002990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000029a0: 2020 6e61 6d65 3d27 5072 6564 6963 7469    name='Predicti
+000029b0: 6f6e 272c 0d0a 2020 2020 2020 2020 2020  on',..          
+000029c0: 2020 2020 2020 793d 7365 6c66 2e70 7265        y=self.pre
+000029d0: 6469 6374 2858 292c 0d0a 2020 2020 2020  dict(X),..      
+000029e0: 2020 2020 2020 2020 2020 6d6f 6465 3d27            mode='
+000029f0: 6c69 6e65 7327 2c0d 0a20 2020 2020 2020  lines',..       
+00002a00: 2020 2020 2020 2020 206d 6172 6b65 723d           marker=
+00002a10: 6469 6374 2863 6f6c 6f72 3d22 2334 3434  dict(color="#444
+00002a20: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
+00002a30: 2020 2020 206c 696e 653d 6469 6374 2877       line=dict(w
+00002a40: 6964 7468 3d31 292c 0d0a 2020 2020 2020  idth=1),..      
+00002a50: 2020 2020 2020 2020 2020 7368 6f77 6c65            showle
+00002a60: 6765 6e64 3d54 7275 650d 0a20 2020 2020  gend=True..     
+00002a70: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+00002a80: 2020 5d29 0d0a 2020 2020 2020 2020 6669    ])..        fi
+00002a90: 672e 7570 6461 7465 5f6c 6179 6f75 7428  g.update_layout(
+00002aa0: 0d0a 2020 2020 2020 2020 2020 2020 7861  ..            xa
+00002ab0: 7869 735f 7469 746c 653d 2758 272c 0d0a  xis_title='X',..
+00002ac0: 2020 2020 2020 2020 2020 2020 7961 7869              yaxi
+00002ad0: 735f 7469 746c 653d 2759 272c 0d0a 2020  s_title='Y',..  
+00002ae0: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+00002af0: 2750 7265 6469 6374 696f 6e20 7673 2e20  'Prediction vs. 
+00002b00: 7461 7267 6574 272c 0d0a 2020 2020 2020  target',..      
+00002b10: 2020 2020 2020 686f 7665 726d 6f64 653d        hovermode=
+00002b20: 2278 220d 0a20 2020 2020 2020 2029 0d0a  "x"..        )..
+00002b30: 2020 2020 2020 2020 6669 672e 7368 6f77          fig.show
+00002b40: 2829 0d0a 2020 2020 2020 2020 0d0a 2020  ()..        ..  
+00002b50: 2020 6465 6620 6765 744d 6574 7269 6373    def getMetrics
+00002b60: 2873 656c 662c 2079 5f72 6561 6c3a 6e70  (self, y_real:np
+00002b70: 2e6e 6461 7272 6179 2c20 795f 7072 6564  .ndarray, y_pred
+00002b80: 3a6e 702e 6e64 6172 7261 792c 2073 686f  :np.ndarray, sho
+00002b90: 773a 626f 6f6c 3d54 7275 6529 202d 3e20  w:bool=True) -> 
+00002ba0: 6469 6374 3a0d 0a0d 0a20 2020 2020 2020  dict:....       
+00002bb0: 2027 2727 0d0a 2020 2020 2020 2020 4765   '''..        Ge
+00002bc0: 7420 6d6f 6465 6c20 6d65 7472 6963 732e  t model metrics.
+00002bd0: 0d0a 0d0a 2020 2020 2020 2020 5061 7261  ....        Para
+00002be0: 6d65 7465 7273 0d0a 2020 2020 2020 2020  meters..        
+00002bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 0d0a 2020 2020  ----------..    
+00002c00: 2020 2020 795f 7265 616c 3a20 6e70 2e6e      y_real: np.n
+00002c10: 6461 7272 6179 0d0a 2020 2020 2020 2020  darray..        
+00002c20: 2020 2020 4172 7261 7920 636f 6e74 6169      Array contai
+00002c30: 6e69 6720 7468 6520 7265 616c 2064 6174  nig the real dat
+00002c40: 6120 746f 2062 6520 7072 6564 6963 7465  a to be predicte
+00002c50: 642e 0d0a 2020 2020 2020 2020 795f 7072  d...        y_pr
+00002c60: 6564 3a20 6e70 2e6e 6461 7272 6179 0d0a  ed: np.ndarray..
+00002c70: 2020 2020 2020 2020 2020 2020 4172 7261              Arra
+00002c80: 7920 636f 6e74 6169 6e69 6720 7468 6520  y containig the 
+00002c90: 7072 6564 6963 7465 6420 6461 7461 2e0d  predicted data..
+00002ca0: 0a20 2020 2020 2020 2073 686f 773a 2062  .        show: b
+00002cb0: 6f6f 6c0d 0a20 2020 2020 2020 2020 2020  ool..           
+00002cc0: 2054 7275 6520 746f 2070 7269 6e74 2074   True to print t
+00002cd0: 6865 206d 6574 7269 6373 2e0d 0a0d 0a20  he metrics..... 
+00002ce0: 2020 2020 2020 2052 6574 7572 6e73 0d0a         Returns..
+00002cf0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0d          -------.
+00002d00: 0a20 2020 2020 2020 2072 6574 7572 6e3a  .        return:
+00002d10: 2064 6963 740d 0a20 2020 2020 2020 2020   dict..         
+00002d20: 2020 2044 6963 7469 6f6e 6172 7920 636f     Dictionary co
+00002d30: 6e74 6169 6e69 6e67 2027 6163 6375 7261  ntaining 'accura
+00002d40: 6379 272c 2027 7072 6563 6973 696f 6e27  cy', 'precision'
+00002d50: 2c20 2772 6563 616c 6c27 2061 6e64 200d  , 'recall' and .
+00002d60: 0a20 2020 2020 2020 2020 2020 2027 6631  .            'f1
+00002d70: 5f73 636f 7265 2720 666f 7220 7468 6520  _score' for the 
+00002d80: 6d6f 6465 6c2e 0d0a 2020 2020 2020 2020  model...        
+00002d90: 2727 270d 0a20 2020 2020 2020 200d 0a20  '''..        .. 
+00002da0: 2020 2020 2020 2061 6363 7572 6163 7920         accuracy 
+00002db0: 3d20 7574 696c 732e 436c 6173 7369 6669  = utils.Classifi
+00002dc0: 6361 7469 6f6e 4d65 7472 6963 732e 6163  cationMetrics.ac
+00002dd0: 6375 7261 6379 2879 5f72 6561 6c2c 2079  curacy(y_real, y
+00002de0: 5f70 7265 6429 0d0a 2020 2020 2020 2020  _pred)..        
+00002df0: 7072 6563 6973 696f 6e20 3d20 7574 696c  precision = util
+00002e00: 732e 436c 6173 7369 6669 6361 7469 6f6e  s.Classification
+00002e10: 4d65 7472 6963 732e 7072 6563 6973 696f  Metrics.precisio
+00002e20: 6e28 795f 7265 616c 2c20 795f 7072 6564  n(y_real, y_pred
+00002e30: 290d 0a20 2020 2020 2020 2072 6563 616c  )..        recal
+00002e40: 6c20 3d20 7574 696c 732e 436c 6173 7369  l = utils.Classi
+00002e50: 6669 6361 7469 6f6e 4d65 7472 6963 732e  ficationMetrics.
+00002e60: 7265 6361 6c6c 2879 5f72 6561 6c2c 2079  recall(y_real, y
+00002e70: 5f70 7265 6429 0d0a 2020 2020 2020 2020  _pred)..        
+00002e80: 6631 5f73 636f 7265 203d 2075 7469 6c73  f1_score = utils
+00002e90: 2e43 6c61 7373 6966 6963 6174 696f 6e4d  .ClassificationM
+00002ea0: 6574 7269 6373 2e66 315f 7363 6f72 6528  etrics.f1_score(
+00002eb0: 795f 7265 616c 2c20 795f 7072 6564 290d  y_real, y_pred).
+00002ec0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00002ed0: 2020 2069 6620 7368 6f77 3a0d 0a20 2020     if show:..   
+00002ee0: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00002ef0: 2241 6363 7572 6163 793a 207b 6163 6375  "Accuracy: {accu
+00002f00: 7261 6379 3a2e 3225 7d22 290d 0a20 2020  racy:.2%}")..   
+00002f10: 2020 2020 2020 2020 2070 7269 6e74 2866           print(f
+00002f20: 2250 7265 6369 7369 6f6e 3a20 7b70 7265  "Precision: {pre
+00002f30: 6369 7369 6f6e 3a2e 3225 7d22 290d 0a20  cision:.2%}").. 
+00002f40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00002f50: 2866 2252 6563 616c 6c3a 207b 7265 6361  (f"Recall: {reca
+00002f60: 6c6c 3a2e 3225 7d22 290d 0a20 2020 2020  ll:.2%}")..     
+00002f70: 2020 2020 2020 2070 7269 6e74 2866 2246         print(f"F
+00002f80: 312d 5363 6f72 653a 207b 6631 5f73 636f  1-Score: {f1_sco
+00002f90: 7265 3a2e 3225 7d22 290d 0a20 2020 2020  re:.2%}")..     
+00002fa0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002fb0: 2072 6574 7572 6e20 7b27 6163 6375 7261   return {'accura
+00002fc0: 6379 273a 6163 6375 7261 6379 2c20 2770  cy':accuracy, 'p
+00002fd0: 7265 6369 7369 6f6e 273a 7072 6563 6973  recision':precis
+00002fe0: 696f 6e2c 200d 0a20 2020 2020 2020 2020  ion, ..         
+00002ff0: 2020 2020 2020 2027 7265 6361 6c6c 273a         'recall':
+00003000: 7265 6361 6c6c 2c20 2766 315f 7363 6f72  recall, 'f1_scor
+00003010: 6527 3a66 315f 7363 6f72 657d 0d0a 0d0a  e':f1_score}....
+00003020: 2020 2020 2020 2020 0d0a 6966 205f 5f6e          ..if __n
+00003030: 616d 655f 5f20 3d3d 2027 5f5f 6d61 696e  ame__ == '__main
+00003040: 5f5f 273a 0d0a 0d0a 2020 2020 696d 706f  __':....    impo
+00003050: 7274 2079 6669 6e61 6e63 6520 6173 2079  rt yfinance as y
+00003060: 660d 0a20 2020 2066 726f 6d20 7072 696e  f..    from prin
+00003070: 6369 7061 6c5f 636f 6d70 6f6e 656e 7420  cipal_component 
+00003080: 696d 706f 7274 2050 4341 0d0a 2020 2020  import PCA..    
+00003090: 0d0a 2020 2020 7063 615f 6170 706c 7920  ..    pca_apply 
+000030a0: 3d20 4661 6c73 650d 0a20 2020 206a 7573  = False..    jus
+000030b0: 745f 7369 6465 203d 2046 616c 7365 0d0a  t_side = False..
+000030c0: 0d0a 2020 2020 6461 7461 203d 2079 662e  ..    data = yf.
+000030d0: 5469 636b 6572 2827 5453 4c41 2729 2e68  Ticker('TSLA').h
+000030e0: 6973 746f 7279 2870 6572 696f 643d 2735  istory(period='5
+000030f0: 7927 2c20 696e 7465 7276 616c 3d27 3164  y', interval='1d
+00003100: 2729 0d0a 2020 2020 6461 7461 2e63 6f6c  ')..    data.col
+00003110: 756d 6e73 203d 205b 632e 6c6f 7765 7228  umns = [c.lower(
+00003120: 2920 666f 7220 6320 696e 2064 6174 612e  ) for c in data.
+00003130: 636f 6c75 6d6e 735d 0d0a 2020 2020 6461  columns]..    da
+00003140: 7461 5b27 6461 7465 275d 203d 2064 6174  ta['date'] = dat
+00003150: 612e 696e 6465 780d 0a20 2020 2064 6174  a.index..    dat
+00003160: 615b 2770 7265 765f 636c 6f73 6527 5d20  a['prev_close'] 
+00003170: 3d20 6461 7461 5b27 636c 6f73 6527 5d2e  = data['close'].
+00003180: 7368 6966 7428 3129 0d0a 2020 2020 6461  shift(1)..    da
+00003190: 7461 5b27 6f75 746c 6965 725f 7075 275d  ta['outlier_pu']
+000031a0: 203d 2064 6174 615b 276f 7065 6e27 5d2f   = data['open']/
+000031b0: 6461 7461 5b27 6f70 656e 275d 2e72 6f6c  data['open'].rol
+000031c0: 6c69 6e67 2835 3029 2e6d 6561 6e28 2920  ling(50).mean() 
+000031d0: 2d20 310d 0a20 2020 2064 6174 615b 2772  - 1..    data['r
+000031e0: 616e 6765 275d 203d 2028 6461 7461 5b27  ange'] = (data['
+000031f0: 6869 6768 275d 202d 2064 6174 615b 276c  high'] - data['l
+00003200: 6f77 275d 292e 7368 6966 7428 3129 0d0a  ow']).shift(1)..
+00003210: 2020 2020 6461 7461 5b27 7261 6e67 655f      data['range_
+00003220: 7075 275d 203d 2064 6174 615b 2772 616e  pu'] = data['ran
+00003230: 6765 275d 2f64 6174 615b 276f 7065 6e27  ge']/data['open'
+00003240: 5d0d 0a20 2020 2064 6174 615b 276f 7065  ]..    data['ope
+00003250: 6e5f 746f 5f63 6c6f 7365 275d 203d 2028  n_to_close'] = (
+00003260: 6461 7461 5b27 636c 6f73 6527 5d20 2d20  data['close'] - 
+00003270: 6461 7461 5b27 6f70 656e 275d 292e 7368  data['open']).sh
+00003280: 6966 7428 3129 0d0a 2020 2020 6461 7461  ift(1)..    data
+00003290: 5b27 6f70 656e 5f74 6f5f 636c 6f73 655f  ['open_to_close_
+000032a0: 7075 275d 203d 2064 6174 615b 2772 616e  pu'] = data['ran
+000032b0: 6765 275d 2f64 6174 615b 276f 7065 6e27  ge']/data['open'
+000032c0: 5d0d 0a20 2020 2064 6174 615b 2767 6170  ]..    data['gap
+000032d0: 275d 203d 2064 6174 615b 276f 7065 6e27  '] = data['open'
+000032e0: 5d20 2d20 6461 7461 5b27 636c 6f73 6527  ] - data['close'
+000032f0: 5d2e 7368 6966 7428 3129 0d0a 2020 2020  ].shift(1)..    
+00003300: 6461 7461 5b27 6761 705f 7075 275d 203d  data['gap_pu'] =
+00003310: 2064 6174 615b 2767 6170 275d 202f 2064   data['gap'] / d
+00003320: 6174 615b 2763 6c6f 7365 275d 2e73 6869  ata['close'].shi
+00003330: 6674 2831 290d 0a20 2020 200d 0a20 2020  ft(1)..    ..   
+00003340: 2064 6174 615b 2764 6179 275d 203d 2064   data['day'] = d
+00003350: 6174 615b 2764 6174 6527 5d2e 6474 2e79  ata['date'].dt.y
+00003360: 6561 720d 0a20 2020 2064 6174 615b 276d  ear..    data['m
+00003370: 6f6e 7468 275d 203d 2064 6174 615b 2764  onth'] = data['d
+00003380: 6174 6527 5d2e 6474 2e6d 6f6e 7468 0d0a  ate'].dt.month..
+00003390: 2020 2020 6461 7461 5b27 7965 6172 275d      data['year']
+000033a0: 203d 2064 6174 615b 2764 6174 6527 5d2e   = data['date'].
+000033b0: 6474 2e64 6179 0d0a 2020 2020 6461 7461  dt.day..    data
+000033c0: 5b27 7765 656b 5f64 6179 275d 203d 2064  ['week_day'] = d
+000033d0: 6174 615b 2764 6174 6527 5d2e 6474 2e64  ata['date'].dt.d
+000033e0: 6179 6f66 7765 656b 0d0a 2020 2020 6461  ayofweek..    da
+000033f0: 7461 5b27 6973 5f71 7561 7274 6572 5f65  ta['is_quarter_e
+00003400: 6e64 275d 203d 206e 702e 7768 6572 6528  nd'] = np.where(
+00003410: 6461 7461 5b27 6d6f 6e74 6827 5d25 3320  data['month']%3 
+00003420: 3d3d 2030 2c20 312c 2030 290d 0a20 2020  == 0, 1, 0)..   
+00003430: 2020 2020 200d 0a20 2020 2064 6174 615b       ..    data[
+00003440: 2774 6172 6765 7427 5d20 3d20 6e70 2e77  'target'] = np.w
+00003450: 6865 7265 2864 6174 615b 276f 7065 6e27  here(data['open'
+00003460: 5d20 3c20 6461 7461 5b27 636c 6f73 6527  ] < data['close'
+00003470: 5d2c 2031 2c20 3029 0d0a 2020 2020 6461  ], 1, 0)..    da
+00003480: 7461 2e64 726f 706e 6128 696e 706c 6163  ta.dropna(inplac
+00003490: 653d 5472 7565 290d 0a20 2020 200d 0a20  e=True)..    .. 
+000034a0: 2020 2066 6561 7475 7265 7320 3d20 5b27     features = ['
+000034b0: 7261 6e67 655f 7075 272c 2027 6f70 656e  range_pu', 'open
+000034c0: 5f74 6f5f 636c 6f73 655f 7075 272c 2027  _to_close_pu', '
+000034d0: 6761 705f 7075 272c 2027 6f75 746c 6965  gap_pu', 'outlie
+000034e0: 725f 7075 272c 2027 6461 7927 2c20 276d  r_pu', 'day', 'm
+000034f0: 6f6e 7468 272c 2027 7765 656b 5f64 6179  onth', 'week_day
+00003500: 272c 2027 6973 5f71 7561 7274 6572 5f65  ', 'is_quarter_e
+00003510: 6e64 275d 0d0a 0d0a 2020 2020 585f 7472  nd']....    X_tr
+00003520: 6169 6e2c 2058 5f74 6573 742c 2079 5f74  ain, X_test, y_t
+00003530: 7261 696e 2c20 795f 7465 7374 203d 2075  rain, y_test = u
+00003540: 7469 6c73 2e74 7261 696e 5f74 6573 745f  tils.train_test_
+00003550: 7370 6c69 7428 6461 7461 5b66 6561 7475  split(data[featu
+00003560: 7265 735d 2c20 6461 7461 5b27 7461 7267  res], data['targ
+00003570: 6574 275d 2c20 0d0a 2020 2020 2020 2020  et'], ..        
 00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000035b0: 616e 646f 6d5f 7374 6174 653d 3431 2c20  andom_state=41, 
-000035c0: 7465 7374 5f73 697a 653d 302e 3229 0d0a  test_size=0.2)..
-000035d0: 2020 2020 585f 7472 6169 6e5f 7374 616e      X_train_stan
-000035e0: 642c 2058 5f74 6573 745f 7374 616e 6420  d, X_test_stand 
-000035f0: 3d20 7574 696c 732e 7374 616e 6461 7264  = utils.standard
-00003600: 697a 655f 6461 7461 2858 5f74 7261 696e  ize_data(X_train
-00003610: 2c20 585f 7465 7374 290d 0a20 2020 200d  , X_test)..    .
-00003620: 0a20 2020 2069 6620 7063 615f 6170 706c  .    if pca_appl
-00003630: 793a 0d0a 2020 2020 2020 2020 7063 6120  y:..        pca 
-00003640: 3d20 5043 4128 6c65 6e28 6665 6174 7572  = PCA(len(featur
-00003650: 6573 292f 3229 0d0a 2020 2020 2020 2020  es)/2)..        
-00003660: 7063 612e 6669 7428 585f 7472 6169 6e5f  pca.fit(X_train_
-00003670: 7374 616e 6429 0d0a 2020 2020 2020 2020  stand)..        
-00003680: 585f 7472 6169 6e5f 7374 616e 6420 3d20  X_train_stand = 
-00003690: 7063 612e 7472 616e 7366 6f72 6d28 585f  pca.transform(X_
-000036a0: 7472 6169 6e5f 7374 616e 6429 0d0a 2020  train_stand)..  
-000036b0: 2020 2020 2020 585f 7465 7374 5f73 7461        X_test_sta
-000036c0: 6e64 203d 2070 6361 2e74 7261 6e73 666f  nd = pca.transfo
-000036d0: 726d 2858 5f74 6573 745f 7374 616e 6429  rm(X_test_stand)
-000036e0: 0d0a 2020 2020 2020 2020 7063 612e 706c  ..        pca.pl
-000036f0: 6f74 436f 6d70 6f6e 656e 7473 2858 5f74  otComponents(X_t
-00003700: 7261 696e 5f73 7461 6e64 290d 0a20 2020  rain_stand)..   
-00003710: 2020 2020 2070 6361 2e63 756d 756c 6174       pca.cumulat
-00003720: 6976 655f 7661 7269 616e 6365 5f72 6174  ive_variance_rat
-00003730: 696f 0d0a 2020 2020 2020 2020 0d0a 2020  io..        ..  
-00003740: 2020 2020 2020 6665 6174 7572 6573 203d        features =
-00003750: 205b 6627 5043 7b69 7d27 2066 6f72 2069   [f'PC{i}' for i
-00003760: 2069 6e20 7261 6e67 6528 585f 7472 6169   in range(X_trai
-00003770: 6e5f 7374 616e 642e 7368 6170 655b 2d31  n_stand.shape[-1
-00003780: 5d29 5d0d 0a0d 0a20 2020 206d 6f64 656c  ])]....    model
-00003790: 203d 204c 6f67 6973 7469 6352 6567 7265   = LogisticRegre
-000037a0: 7373 696f 6e28 6c65 6172 6e69 6e67 5f72  ssion(learning_r
-000037b0: 6174 653d 302e 3030 3031 290d 0a20 2020  ate=0.0001)..   
-000037c0: 206d 6f64 656c 2e66 6974 2858 5f74 7261   model.fit(X_tra
-000037d0: 696e 5f73 7461 6e64 2c20 795f 7472 6169  in_stand, y_trai
-000037e0: 6e2c 2031 3030 3030 3030 2c20 7665 7262  n, 1000000, verb
-000037f0: 6f73 653d 4661 6c73 6529 0d0a 2020 2020  ose=False)..    
-00003800: 0d0a 2020 2020 795f 7472 6169 6e5f 7072  ..    y_train_pr
-00003810: 6564 203d 206d 6f64 656c 2e70 7265 6469  ed = model.predi
-00003820: 6374 2858 5f74 7261 696e 5f73 7461 6e64  ct(X_train_stand
-00003830: 290d 0a20 2020 2079 5f74 6573 745f 7072  )..    y_test_pr
-00003840: 6564 203d 206d 6f64 656c 2e70 7265 6469  ed = model.predi
-00003850: 6374 2858 5f74 6573 745f 7374 616e 6429  ct(X_test_stand)
-00003860: 0d0a 2020 2020 0d0a 2020 2020 2320 5368  ..    ..    # Sh
-00003870: 6f77 206d 6574 7269 6373 0d0a 2020 2020  ow metrics..    
-00003880: 7465 7374 7320 3d20 7b27 7472 6169 6e27  tests = {'train'
-00003890: 3a20 5b79 5f74 7261 696e 2c20 795f 7472  : [y_train, y_tr
-000038a0: 6169 6e5f 7072 6564 5d2c 2027 7465 7374  ain_pred], 'test
-000038b0: 273a 5b79 5f74 6573 742c 2079 5f74 6573  ':[y_test, y_tes
-000038c0: 745f 7072 6564 5d7d 0d0a 2020 2020 666f  t_pred]}..    fo
-000038d0: 7220 6b20 696e 2074 6573 7473 3a0d 0a20  r k in tests:.. 
-000038e0: 2020 2020 2020 2079 5f74 6573 742c 2079         y_test, y
-000038f0: 5f70 7265 6420 3d20 7465 7374 735b 6b5d  _pred = tests[k]
-00003900: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
-00003910: 2020 2020 7072 696e 7428 6627 5c6e 4d45      print(f'\nME
-00003920: 5452 4943 5320 464f 5220 5448 4520 7b6b  TRICS FOR THE {k
-00003930: 2e75 7070 6572 2829 7d20 2d2d 2d2d 2d2d  .upper()} ------
-00003940: 2d2d 2d2d 2d2d 2d2d 2d2d 2729 0d0a 2020  ----------')..  
-00003950: 2020 2020 2020 6d6f 6465 6c2e 6765 744d        model.getM
-00003960: 6574 7269 6373 2879 5f74 6573 742c 2079  etrics(y_test, y
-00003970: 5f70 7265 642c 2073 686f 773d 5472 7565  _pred, show=True
-00003980: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00003990: 2020 2020 2079 5f64 6620 3d20 7064 2e44       y_df = pd.D
-000039a0: 6174 6146 7261 6d65 287b 274f 7065 6e27  ataFrame({'Open'
-000039b0: 3a64 6174 615b 276f 7065 6e27 5d2e 696c  :data['open'].il
-000039c0: 6f63 5b2d 6c65 6e28 795f 7465 7374 293a  oc[-len(y_test):
-000039d0: 5d2c 200d 0a20 2020 2020 2020 2020 2020  ], ..           
+000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000035b0: 2020 2020 2020 7261 6e64 6f6d 5f73 7461        random_sta
+000035c0: 7465 3d34 312c 2074 6573 745f 7369 7a65  te=41, test_size
+000035d0: 3d30 2e32 290d 0a20 2020 2058 5f74 7261  =0.2)..    X_tra
+000035e0: 696e 5f73 7461 6e64 2c20 585f 7465 7374  in_stand, X_test
+000035f0: 5f73 7461 6e64 203d 2075 7469 6c73 2e73  _stand = utils.s
+00003600: 7461 6e64 6172 6469 7a65 5f64 6174 6128  tandardize_data(
+00003610: 585f 7472 6169 6e2c 2058 5f74 6573 7429  X_train, X_test)
+00003620: 0d0a 2020 2020 0d0a 2020 2020 6966 2070  ..    ..    if p
+00003630: 6361 5f61 7070 6c79 3a0d 0a20 2020 2020  ca_apply:..     
+00003640: 2020 2070 6361 203d 2050 4341 286c 656e     pca = PCA(len
+00003650: 2866 6561 7475 7265 7329 2f32 290d 0a20  (features)/2).. 
+00003660: 2020 2020 2020 2070 6361 2e66 6974 2858         pca.fit(X
+00003670: 5f74 7261 696e 5f73 7461 6e64 290d 0a20  _train_stand).. 
+00003680: 2020 2020 2020 2058 5f74 7261 696e 5f73         X_train_s
+00003690: 7461 6e64 203d 2070 6361 2e74 7261 6e73  tand = pca.trans
+000036a0: 666f 726d 2858 5f74 7261 696e 5f73 7461  form(X_train_sta
+000036b0: 6e64 290d 0a20 2020 2020 2020 2058 5f74  nd)..        X_t
+000036c0: 6573 745f 7374 616e 6420 3d20 7063 612e  est_stand = pca.
+000036d0: 7472 616e 7366 6f72 6d28 585f 7465 7374  transform(X_test
+000036e0: 5f73 7461 6e64 290d 0a20 2020 2020 2020  _stand)..       
+000036f0: 2070 6361 2e70 6c6f 7443 6f6d 706f 6e65   pca.plotCompone
+00003700: 6e74 7328 585f 7472 6169 6e5f 7374 616e  nts(X_train_stan
+00003710: 6429 0d0a 2020 2020 2020 2020 7063 612e  d)..        pca.
+00003720: 6375 6d75 6c61 7469 7665 5f76 6172 6961  cumulative_varia
+00003730: 6e63 655f 7261 7469 6f0d 0a20 2020 2020  nce_ratio..     
+00003740: 2020 200d 0a20 2020 2020 2020 2066 6561     ..        fea
+00003750: 7475 7265 7320 3d20 5b66 2750 437b 697d  tures = [f'PC{i}
+00003760: 2720 666f 7220 6920 696e 2072 616e 6765  ' for i in range
+00003770: 2858 5f74 7261 696e 5f73 7461 6e64 2e73  (X_train_stand.s
+00003780: 6861 7065 5b2d 315d 295d 0d0a 0d0a 2020  hape[-1])]....  
+00003790: 2020 6d6f 6465 6c20 3d20 4c6f 6769 7374    model = Logist
+000037a0: 6963 5265 6772 6573 7369 6f6e 286c 6561  icRegression(lea
+000037b0: 726e 696e 675f 7261 7465 3d30 2e30 3030  rning_rate=0.000
+000037c0: 3129 0d0a 2020 2020 6d6f 6465 6c2e 6669  1)..    model.fi
+000037d0: 7428 585f 7472 6169 6e5f 7374 616e 642c  t(X_train_stand,
+000037e0: 2079 5f74 7261 696e 2c20 3130 3030 3030   y_train, 100000
+000037f0: 302c 2076 6572 626f 7365 3d46 616c 7365  0, verbose=False
+00003800: 290d 0a20 2020 200d 0a20 2020 2079 5f74  )..    ..    y_t
+00003810: 7261 696e 5f70 7265 6420 3d20 6d6f 6465  rain_pred = mode
+00003820: 6c2e 7072 6564 6963 7428 585f 7472 6169  l.predict(X_trai
+00003830: 6e5f 7374 616e 6429 0d0a 2020 2020 795f  n_stand)..    y_
+00003840: 7465 7374 5f70 7265 6420 3d20 6d6f 6465  test_pred = mode
+00003850: 6c2e 7072 6564 6963 7428 585f 7465 7374  l.predict(X_test
+00003860: 5f73 7461 6e64 290d 0a20 2020 200d 0a20  _stand)..    .. 
+00003870: 2020 2023 2053 686f 7720 6d65 7472 6963     # Show metric
+00003880: 730d 0a20 2020 2074 6573 7473 203d 207b  s..    tests = {
+00003890: 2774 7261 696e 273a 205b 795f 7472 6169  'train': [y_trai
+000038a0: 6e2c 2079 5f74 7261 696e 5f70 7265 645d  n, y_train_pred]
+000038b0: 2c20 2774 6573 7427 3a5b 795f 7465 7374  , 'test':[y_test
+000038c0: 2c20 795f 7465 7374 5f70 7265 645d 7d0d  , y_test_pred]}.
+000038d0: 0a20 2020 2066 6f72 206b 2069 6e20 7465  .    for k in te
+000038e0: 7374 733a 0d0a 2020 2020 2020 2020 795f  sts:..        y_
+000038f0: 7465 7374 2c20 795f 7072 6564 203d 2074  test, y_pred = t
+00003900: 6573 7473 5b6b 5d0d 0a20 2020 2020 2020  ests[k]..       
+00003910: 200d 0a20 2020 2020 2020 2070 7269 6e74   ..        print
+00003920: 2866 275c 6e4d 4554 5249 4353 2046 4f52  (f'\nMETRICS FOR
+00003930: 2054 4845 207b 6b2e 7570 7065 7228 297d   THE {k.upper()}
+00003940: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+00003950: 2d27 290d 0a20 2020 2020 2020 206d 6f64  -')..        mod
+00003960: 656c 2e67 6574 4d65 7472 6963 7328 795f  el.getMetrics(y_
+00003970: 7465 7374 2c20 795f 7072 6564 2c20 7368  test, y_pred, sh
+00003980: 6f77 3d54 7275 6529 0d0a 2020 2020 2020  ow=True)..      
+00003990: 2020 0d0a 2020 2020 2020 2020 795f 6466    ..        y_df
+000039a0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+000039b0: 7b27 4f70 656e 273a 6461 7461 5b27 6f70  {'Open':data['op
+000039c0: 656e 275d 2e69 6c6f 635b 2d6c 656e 2879  en'].iloc[-len(y
+000039d0: 5f74 6573 7429 3a5d 2c20 0d0a 2020 2020  _test):], ..    
 000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039f0: 2027 436c 6f73 6527 3a64 6174 615b 2763   'Close':data['c
-00003a00: 6c6f 7365 275d 2e69 6c6f 635b 2d6c 656e  lose'].iloc[-len
-00003a10: 2879 5f74 6573 7429 3a5d 2c0d 0a20 2020  (y_test):],..   
-00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a30: 2020 2020 2020 2020 2027 4f72 6967 273a           'Orig':
-00003a40: 2079 5f74 6573 742c 2027 5072 6564 273a   y_test, 'Pred':
-00003a50: 2079 5f70 7265 647d 290d 0a20 2020 2020   y_pred})..     
-00003a60: 2020 2079 5f64 665b 2752 616e 6765 275d     y_df['Range']
-00003a70: 203d 2079 5f64 665b 2743 6c6f 7365 275d   = y_df['Close']
-00003a80: 202d 2079 5f64 665b 274f 7065 6e27 5d0d   - y_df['Open'].
-00003a90: 0a20 2020 2020 2020 2069 6620 6a75 7374  .        if just
-00003aa0: 5f73 6964 653a 0d0a 2020 2020 2020 2020  _side:..        
-00003ab0: 2020 2020 795f 6466 5b27 4f72 6967 5f73      y_df['Orig_s
-00003ac0: 6964 6527 5d20 3d20 6e70 2e77 6865 7265  ide'] = np.where
-00003ad0: 2879 5f64 665b 274f 7269 6727 5d20 3e20  (y_df['Orig'] > 
-00003ae0: 795f 6466 5b27 4f72 6967 275d 2e73 6869  y_df['Orig'].shi
-00003af0: 6674 2831 292c 2031 2c20 0d0a 2020 2020  ft(1), 1, ..    
-00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b10: 2020 2020 2020 2020 2020 2020 6e70 2e77              np.w
-00003b20: 6865 7265 2879 5f64 665b 274f 7269 6727  here(y_df['Orig'
-00003b30: 5d20 3c20 795f 6466 5b27 4f72 6967 275d  ] < y_df['Orig']
-00003b40: 2e73 6869 6674 2831 292c 202d 312c 2030  .shift(1), -1, 0
-00003b50: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
-00003b60: 795f 6466 5b27 5072 6564 5f73 6964 6527  y_df['Pred_side'
-00003b70: 5d20 3d20 6e70 2e77 6865 7265 2879 5f64  ] = np.where(y_d
-00003b80: 665b 2750 7265 6427 5d20 3e20 795f 6466  f['Pred'] > y_df
-00003b90: 5b27 5072 6564 275d 2e73 6869 6674 2831  ['Pred'].shift(1
-00003ba0: 292c 2031 2c20 0d0a 2020 2020 2020 2020  ), 1, ..        
+000039f0: 2020 2020 2020 2020 2743 6c6f 7365 273a          'Close':
+00003a00: 6461 7461 5b27 636c 6f73 6527 5d2e 696c  data['close'].il
+00003a10: 6f63 5b2d 6c65 6e28 795f 7465 7374 293a  oc[-len(y_test):
+00003a20: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
+00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a40: 274f 7269 6727 3a20 795f 7465 7374 2c20  'Orig': y_test, 
+00003a50: 2750 7265 6427 3a20 795f 7072 6564 7d29  'Pred': y_pred})
+00003a60: 0d0a 2020 2020 2020 2020 795f 6466 5b27  ..        y_df['
+00003a70: 5261 6e67 6527 5d20 3d20 795f 6466 5b27  Range'] = y_df['
+00003a80: 436c 6f73 6527 5d20 2d20 795f 6466 5b27  Close'] - y_df['
+00003a90: 4f70 656e 275d 0d0a 2020 2020 2020 2020  Open']..        
+00003aa0: 6966 206a 7573 745f 7369 6465 3a0d 0a20  if just_side:.. 
+00003ab0: 2020 2020 2020 2020 2020 2079 5f64 665b             y_df[
+00003ac0: 274f 7269 675f 7369 6465 275d 203d 206e  'Orig_side'] = n
+00003ad0: 702e 7768 6572 6528 795f 6466 5b27 4f72  p.where(y_df['Or
+00003ae0: 6967 275d 203e 2079 5f64 665b 274f 7269  ig'] > y_df['Ori
+00003af0: 6727 5d2e 7368 6966 7428 3129 2c20 312c  g'].shift(1), 1,
+00003b00: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 206e 702e 7768 6572 6528 795f 6466     np.where(y_df
+00003b30: 5b27 4f72 6967 275d 203c 2079 5f64 665b  ['Orig'] < y_df[
+00003b40: 274f 7269 6727 5d2e 7368 6966 7428 3129  'Orig'].shift(1)
+00003b50: 2c20 2d31 2c20 3029 290d 0a20 2020 2020  , -1, 0))..     
+00003b60: 2020 2020 2020 2079 5f64 665b 2750 7265         y_df['Pre
+00003b70: 645f 7369 6465 275d 203d 206e 702e 7768  d_side'] = np.wh
+00003b80: 6572 6528 795f 6466 5b27 5072 6564 275d  ere(y_df['Pred']
+00003b90: 203e 2079 5f64 665b 2750 7265 6427 5d2e   > y_df['Pred'].
+00003ba0: 7368 6966 7428 3129 2c20 312c 200d 0a20  shift(1), 1, .. 
 00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bc0: 2020 2020 2020 2020 6e70 2e77 6865 7265          np.where
-00003bd0: 2879 5f64 665b 2750 7265 6427 5d20 3c20  (y_df['Pred'] < 
-00003be0: 795f 6466 5b27 5072 6564 275d 2e73 6869  y_df['Pred'].shi
-00003bf0: 6674 2831 292c 202d 312c 2030 2929 0d0a  ft(1), -1, 0))..
-00003c00: 2020 2020 2020 2020 2020 2020 7375 6363              succ
-00003c10: 6573 7320 3d20 795f 6466 5b79 5f64 665b  ess = y_df[y_df[
-00003c20: 2750 7265 645f 7369 6465 275d 203d 3d20  'Pred_side'] == 
-00003c30: 795f 6466 5b27 4f72 6967 5f73 6964 6527  y_df['Orig_side'
-00003c40: 5d5d 0d0a 2020 2020 2020 2020 2020 2020  ]]..            
-00003c50: 6572 726f 7220 3d20 795f 6466 5b79 5f64  error = y_df[y_d
-00003c60: 665b 2750 7265 645f 7369 6465 275d 2021  f['Pred_side'] !
-00003c70: 3d20 795f 6466 5b27 4f72 6967 5f73 6964  = y_df['Orig_sid
-00003c80: 6527 5d5d 0d0a 2020 2020 2020 2020 656c  e']]..        el
-00003c90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-00003ca0: 2073 7563 6365 7373 203d 2079 5f64 665b   success = y_df[
-00003cb0: 795f 6466 5b27 5072 6564 275d 203d 3d20  y_df['Pred'] == 
-00003cc0: 795f 6466 5b27 4f72 6967 275d 5d0d 0a20  y_df['Orig']].. 
-00003cd0: 2020 2020 2020 2020 2020 2065 7272 6f72             error
-00003ce0: 203d 2079 5f64 665b 795f 6466 5b27 5072   = y_df[y_df['Pr
-00003cf0: 6564 275d 2021 3d20 795f 6466 5b27 4f72  ed'] != y_df['Or
-00003d00: 6967 275d 5d0d 0a20 2020 2020 2020 200d  ig']]..        .
-00003d10: 0a20 2020 2020 2020 2077 7220 3d20 6c65  .        wr = le
-00003d20: 6e28 7375 6363 6573 7329 2f6c 656e 2879  n(success)/len(y
-00003d30: 5f64 6629 0d0a 2020 2020 2020 2020 7272  _df)..        rr
-00003d40: 203d 2028 7375 6363 6573 735b 2752 616e   = (success['Ran
-00003d50: 6765 275d 2e61 6273 2829 2e6d 6561 6e28  ge'].abs().mean(
-00003d60: 2929 2f28 6572 726f 725b 2752 616e 6765  ))/(error['Range
-00003d70: 275d 2e61 6273 2829 2e6d 6561 6e28 2929  '].abs().mean())
-00003d80: 0d0a 2020 2020 2020 2020 7072 696e 7428  ..        print(
-00003d90: 6627 5369 6465 2053 7563 6365 7373 3a20  f'Side Success: 
-00003da0: 7b77 723a 2e32 257d 2729 0d0a 2020 2020  {wr:.2%}')..    
-00003db0: 2020 2020 7072 696e 7428 6627 5269 736b      print(f'Risk
-00003dc0: 2052 6577 6172 643a 207b 7272 3a2e 327d   Reward: {rr:.2}
-00003dd0: 2052 2729 0d0a 2020 2020 2020 2020 7072   R')..        pr
-00003de0: 696e 7428 6622 5370 6563 7461 6e63 793a  int(f"Spectancy:
-00003df0: 207b 2877 7220 2a20 7375 6363 6573 735b   {(wr * success[
-00003e00: 2752 616e 6765 275d 2e61 6273 2829 2e6d  'Range'].abs().m
-00003e10: 6561 6e28 2920 2d20 2831 2d77 7229 202a  ean() - (1-wr) *
-00003e20: 2065 7272 6f72 5b27 5261 6e67 6527 5d2e   error['Range'].
-00003e30: 6162 7328 292e 6d65 616e 2829 293a 2e32  abs().mean()):.2
-00003e40: 257d 2229 0d0a 0d0a 2020 2020 2320 506c  %}")....    # Pl
-00003e50: 6f74 2070 7265 6469 6374 696f 6e0d 0a20  ot prediction.. 
-00003e60: 2020 206d 6f64 656c 2e70 6c6f 7450 7265     model.plotPre
-00003e70: 6469 6374 696f 6e28 583d 585f 7465 7374  diction(X=X_test
-00003e80: 5f73 7461 6e64 2c20 793d 795f 7465 7374  _stand, y=y_test
-00003e90: 290d 0a20 2020 2070 7269 6e74 286d 6f64  )..    print(mod
-00003ea0: 656c 2e67 6574 5765 6967 6874 7328 6665  el.getWeights(fe
-00003eb0: 6174 7572 6573 2929                      atures))
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00003bd0: 702e 7768 6572 6528 795f 6466 5b27 5072  p.where(y_df['Pr
+00003be0: 6564 275d 203c 2079 5f64 665b 2750 7265  ed'] < y_df['Pre
+00003bf0: 6427 5d2e 7368 6966 7428 3129 2c20 2d31  d'].shift(1), -1
+00003c00: 2c20 3029 290d 0a20 2020 2020 2020 2020  , 0))..         
+00003c10: 2020 2073 7563 6365 7373 203d 2079 5f64     success = y_d
+00003c20: 665b 795f 6466 5b27 5072 6564 5f73 6964  f[y_df['Pred_sid
+00003c30: 6527 5d20 3d3d 2079 5f64 665b 274f 7269  e'] == y_df['Ori
+00003c40: 675f 7369 6465 275d 5d0d 0a20 2020 2020  g_side']]..     
+00003c50: 2020 2020 2020 2065 7272 6f72 203d 2079         error = y
+00003c60: 5f64 665b 795f 6466 5b27 5072 6564 5f73  _df[y_df['Pred_s
+00003c70: 6964 6527 5d20 213d 2079 5f64 665b 274f  ide'] != y_df['O
+00003c80: 7269 675f 7369 6465 275d 5d0d 0a20 2020  rig_side']]..   
+00003c90: 2020 2020 2065 6c73 653a 0d0a 2020 2020       else:..    
+00003ca0: 2020 2020 2020 2020 7375 6363 6573 7320          success 
+00003cb0: 3d20 795f 6466 5b79 5f64 665b 2750 7265  = y_df[y_df['Pre
+00003cc0: 6427 5d20 3d3d 2079 5f64 665b 274f 7269  d'] == y_df['Ori
+00003cd0: 6727 5d5d 0d0a 2020 2020 2020 2020 2020  g']]..          
+00003ce0: 2020 6572 726f 7220 3d20 795f 6466 5b79    error = y_df[y
+00003cf0: 5f64 665b 2750 7265 6427 5d20 213d 2079  _df['Pred'] != y
+00003d00: 5f64 665b 274f 7269 6727 5d5d 0d0a 2020  _df['Orig']]..  
+00003d10: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003d20: 7772 203d 206c 656e 2873 7563 6365 7373  wr = len(success
+00003d30: 292f 6c65 6e28 795f 6466 290d 0a20 2020  )/len(y_df)..   
+00003d40: 2020 2020 2072 7220 3d20 2873 7563 6365       rr = (succe
+00003d50: 7373 5b27 5261 6e67 6527 5d2e 6162 7328  ss['Range'].abs(
+00003d60: 292e 6d65 616e 2829 292f 2865 7272 6f72  ).mean())/(error
+00003d70: 5b27 5261 6e67 6527 5d2e 6162 7328 292e  ['Range'].abs().
+00003d80: 6d65 616e 2829 290d 0a20 2020 2020 2020  mean())..       
+00003d90: 2070 7269 6e74 2866 2753 6964 6520 5375   print(f'Side Su
+00003da0: 6363 6573 733a 207b 7772 3a2e 3225 7d27  ccess: {wr:.2%}'
+00003db0: 290d 0a20 2020 2020 2020 2070 7269 6e74  )..        print
+00003dc0: 2866 2752 6973 6b20 5265 7761 7264 3a20  (f'Risk Reward: 
+00003dd0: 7b72 723a 2e32 7d20 5227 290d 0a20 2020  {rr:.2} R')..   
+00003de0: 2020 2020 2070 7269 6e74 2866 2253 7065       print(f"Spe
+00003df0: 6374 616e 6379 3a20 7b28 7772 202a 2073  ctancy: {(wr * s
+00003e00: 7563 6365 7373 5b27 5261 6e67 6527 5d2e  uccess['Range'].
+00003e10: 6162 7328 292e 6d65 616e 2829 202d 2028  abs().mean() - (
+00003e20: 312d 7772 2920 2a20 6572 726f 725b 2752  1-wr) * error['R
+00003e30: 616e 6765 275d 2e61 6273 2829 2e6d 6561  ange'].abs().mea
+00003e40: 6e28 2929 3a2e 3225 7d22 290d 0a0d 0a20  n()):.2%}").... 
+00003e50: 2020 2023 2050 6c6f 7420 7072 6564 6963     # Plot predic
+00003e60: 7469 6f6e 0d0a 2020 2020 6d6f 6465 6c2e  tion..    model.
+00003e70: 706c 6f74 5072 6564 6963 7469 6f6e 2858  plotPrediction(X
+00003e80: 3d58 5f74 6573 745f 7374 616e 642c 2079  =X_test_stand, y
+00003e90: 3d79 5f74 6573 7429 0d0a 2020 2020 7072  =y_test)..    pr
+00003ea0: 696e 7428 6d6f 6465 6c2e 6765 7457 6569  int(model.getWei
+00003eb0: 6768 7473 2866 6561 7475 7265 7329 29    ghts(features))
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/long_short_term_memory.py` & `omtf-1.0.3/OMTF/MachineLearning/long_short_term_memory.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/naive_bayes.py` & `omtf-1.0.3/OMTF/MachineLearning/naive_bayes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 class NaiveBayes:
     
     '''
     Naive Bayes classifier implementation using Gaussian distribution assumption.
     
     Tries to maximize the probability of something happening assuming something has
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/neural_networks.py` & `omtf-1.0.3/OMTF/MachineLearning/neural_networks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
-import utils
+from . import utils
 
 class NeuralNetwork:
 
     '''
     Initialize Parameters: We start by initializing the weights and biases of the model. 
     For each layer l in the network, we initialize  W[l] to be a matrix with dimensions 
     (n[l],n[l−1]), where  n[l] is the number of units in layer  l and  n[l−1] is the number
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/principal_component.py` & `omtf-1.0.3/OMTF/MachineLearning/principal_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 class PCA:
     
     # From: https://www.kaggle.com/code/fareselmenshawii/pca-from-scratch/notebook?scriptVersionId=121402593
     
     '''
     Principal Component Analysis (PCA) class for dimensionality reduction.
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/random_forest.py` & `omtf-1.0.3/OMTF/MachineLearning/random_forest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
-import decision_trees
+from . import utils, decision_trees
 
 class RandomForest:
     
     # From: https://www.kaggle.com/code/fareselmenshawii/random-forest-from-scratch?scriptVersionId=138025147
     
     '''
     A random forest classifier.
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/recurrent_neural_networks.py` & `omtf-1.0.3/OMTF/MachineLearning/recurrent_neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/support_vector.py` & `omtf-1.0.3/OMTF/MachineLearning/support_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import math
 import pickle
 import numpy as np
 import pandas as pd
 
-import utils
+from . import utils
 
 class SupportVectorMachine:
     
     '''
     A Support Vector Machine (SVM) implementation using gradient descent.
     
     The goal is to find a hyperplane that separates the data into 2
```

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/utils.py` & `omtf-1.0.3/OMTF/MachineLearning/utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/MachineLearning/xgboost_model.py` & `omtf-1.0.3/OMTF/MachineLearning/xgboost_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
 import math
 import numpy as np 
 import pandas as pd
-from collections import defaultdict
 
 class XGBoost():
     
     '''
     XGBoost from Scratch
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/asset_tradeablitiy.py` & `omtf-1.0.3/OMTF/Trading/asset_tradeablitiy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 import numpy as np
 import pandas as pd
 
-from execution_utils import AssetConfig
+from .execution_utils import AssetConfig
 
 class AssetTradeable:
     
     def __init__(self, asset:AssetConfig, prices:pd.DataFrame, trades:pd.DataFrame, 
                  asset_column:str='Ticker') -> None:
         self.asset: AssetConfig = asset
         self.prices: pd.DataFrame = prices
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/backtest.py` & `omtf-1.0.3/OMTF/Trading/backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pytz
 import numpy as np
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from signals import ContinuousSignals, DiscreteSignals
-from indicators import OHLC, Indicators
+from .signals import ContinuousSignals, DiscreteSignals
+from .indicators import OHLC, Indicators
 #from google_sheets.google_sheets import GoogleSheets
 
 
 
 class Commissions:
 
     def __init__(self, ctype:str='percentage', commission:float=5.0,
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/backtest_utils.py` & `omtf-1.0.3/OMTF/Trading/backtest_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 import enum
 import numpy as np
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from indicators import OHLC
-
-from execution_utils import (typeToDict, Commissions, Trade, OrderType, StrategyConfig, 
+from .indicators import OHLC
+from .execution_utils import (typeToDict, Commissions, Trade, OrderType, StrategyConfig, 
     AssetConfig, TradeSide, CloseMethod, SignalsSide)
 
 class ReturnsType(enum.Enum):
     SIMPLE = 'SIMPLE'
     COMPOUND = 'COMPOUND'
 
 class CapitalType(enum.Enum):
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/config.py` & `omtf-1.0.3/OMTF/Trading/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 import datetime as dt
-from execution_utils import AssetConfig, Commissions, StrategyConfig, TypeOperative
+from .execution_utils import AssetConfig, Commissions, StrategyConfig, TypeOperative
 
 
 BASE_CURRENCY = 'EUR'
 TYPE_OPERATIVE = TypeOperative.DISCRETE
 EXECUTION_PATH = 'execution' # Directory where to store the files with the trades
 OPEN_POSITIONS_FILE = 'trades_orders.csv' # Name of the file containing the orders
 OPEN_TRADES_FILE = 'open_trades.csv' # Name of the file containing the open trades
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/continuous_backtest.py` & `omtf-1.0.3/OMTF/Trading/continuous_backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import datetime as dt
 import numpy as np
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from signals import ContinuousSignals
-from indicators import OHLC, Indicators
-from backtest_utils import (CapitalType, Commissions, BtConfig, 
+from .signals import ContinuousSignals
+from .indicators import OHLC, Indicators
+from .backtest_utils import (CapitalType, Commissions, BtConfig, 
     Backtest, ReturnsType)
-from execution_utils import (TradeSide, OrderType, CloseMethod, 
+from .execution_utils import (TradeSide, OrderType, CloseMethod, 
     DrawDownMitigation, RiskCalculation, AssetConfig, StrategyConfig,
     Trade, KPIs, Leverage, Metrics, Transitions, SignalsSide, Execution,
     JSON)
 #from google_sheets.google_sheets import GoogleSheets
 
 class ContinuousBackTest(Backtest):
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/discrete_backtest.py` & `omtf-1.0.3/OMTF/Trading/discrete_backtest.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import enum
 import numpy as np
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from signals import DiscreteSignals
-from indicators import OHLC, Indicators
-from backtest_utils import CapitalType, Commissions, BtConfig, Backtest
-from execution_utils import (TradeSide, OrderType, CloseMethod, 
+from .signals import DiscreteSignals
+from .indicators import OHLC, Indicators
+from .backtest_utils import CapitalType, Commissions, BtConfig, Backtest
+from .execution_utils import (TradeSide, OrderType, CloseMethod, 
     DrawDownMitigation, RiskCalculation, AssetConfig, StrategyConfig,
     Trade, KPIs, Leverage, Metrics, SignalsSide, Execution)
 #from google_sheets.google_sheets import GoogleSheets
 
 class DiscreteBackTest(Backtest):
 
     '''
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/execution.py` & `omtf-1.0.3/OMTF/Trading/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 import enum
 import numpy as np
 import pandas as pd
 
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
-from signals import ContinuousSignals, DiscreteSignals
-from indicators import Indicators
-from backtest_utils import (Commissions, BtConfig, TradeSide, OrderType, CloseMethod, 
+from .signals import ContinuousSignals, DiscreteSignals
+from .indicators import Indicators
+from .backtest_utils import (Commissions, BtConfig, TradeSide, OrderType, CloseMethod, 
     AssetConfig, StrategyConfig, Trade, SignalsSide)
-from execution_utils import (DrawDownMitigation, RiskCalculation,
+from .execution_utils import (DrawDownMitigation, RiskCalculation,
     KPIs, Leverage, Metrics, Transitions, Execution,
     JSON)
-from backtest_utils import Backtest, ReturnsType
+from .backtest_utils import Backtest, ReturnsType
 
 #from google_sheets.google_sheets import GoogleSheets
 
 class ExecutionType(enum.Enum):
     BACKTEST: str = 'BACKTEST'
     PAPER: str = 'PAPER'
     REAL: str = 'REAL'
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/execution_utils.py` & `omtf-1.0.3/OMTF/Trading/execution_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Trading/indicators.py` & `omtf-1.0.3/OMTF/Trading/indicators.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Trading/portfolios.py` & `omtf-1.0.3/OMTF/Trading/portfolios.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Trading/randomWalk.py` & `omtf-1.0.3/OMTF/Trading/randomWalk.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/Trading/screeners.py` & `omtf-1.0.3/OMTF/Trading/screeners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import enum
 import numpy as np
 import pandas as pd
 
-from portfolios import CustomPortfolioWeighting, Markowitz, VolatType
+from .portfolios import CustomPortfolioWeighting, Markowitz, VolatType
 
     
 class Frequency(enum.Enum):
     YEARLY: str = 'yearly'
     MONTHLY: str = 'monthly'
     WEEKLY: str = 'weekly'
     DAILY: str = 'daily'
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/signals.py` & `omtf-1.0.3/OMTF/Trading/signals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import enum
 
 import numpy as np
 import pandas as pd
 
-from indicators import OHLC, Indicators
+from .indicators import OHLC, Indicators
 
     
 # def checkStrategyConfig(self, strat_name):
 
 #     from config import strategies
 
 #     if strat_name not in list(strategies.keys()):
```

### Comparing `omtf-1.0.2b0/OMTF/Trading/technical.py` & `omtf-1.0.3/OMTF/Trading/technical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF/sp500Historical/sp500_historical.py` & `omtf-1.0.3/OMTF/sp500Historical/sp500_historical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/OMTF.egg-info/PKG-INFO` & `omtf-1.0.3/OMTF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.2b0
+Version: 1.0.3
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
 Home-page: https://onemade.es
 Author: Daniel Cano
 Author-email: Daniel Cano <dcaronm@gmail.com>
 Maintainer-email: Daniel Cano <dcaronm@gmail.com>
 Project-URL: Homepage, https://onemade.es
 Project-URL: Repository, https://github.com/Daniel-OM/OMTF
```

### Comparing `omtf-1.0.2b0/OMTF.egg-info/SOURCES.txt` & `omtf-1.0.3/OMTF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2b0/PKG-INFO` & `omtf-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.2b0
+Version: 1.0.3
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
 Home-page: https://onemade.es
 Author: Daniel Cano
 Author-email: Daniel Cano <dcaronm@gmail.com>
 Maintainer-email: Daniel Cano <dcaronm@gmail.com>
 Project-URL: Homepage, https://onemade.es
 Project-URL: Repository, https://github.com/Daniel-OM/OMTF
```

### Comparing `omtf-1.0.2b0/pyproject.toml` & `omtf-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "OMTF"
-version = "1.0.2b"
+version = "1.0.3"
 authors = [
   { name="Daniel Cano", email="dcaronm@gmail.com" },
 ]
 maintainers = [
   { name="Daniel Cano", email="dcaronm@gmail.com" },
 ]
 description = "OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management."
```

### Comparing `omtf-1.0.2b0/setup.cfg` & `omtf-1.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204f 4d54 460d 0a76 6572 7369 6f6e   = OMTF..version
-00000020: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
+00000020: 203d 2031 2e30 2e33 0d0a 6175 7468 6f72   = 1.0.3..author
 00000030: 203d 2044 616e 6965 6c20 4361 6e6f 0d0a   = Daniel Cano..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
 00000050: 6361 726f 6e6d 4067 6d61 696c 2e63 6f6d  caronm@gmail.com
 00000060: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000070: 4f4d 2054 7261 6469 6e67 2046 7261 6d65  OM Trading Frame
 00000080: 776f 726b 2069 7320 7468 6520 6672 616d  work is the fram
 00000090: 6577 6f72 6b20 4920 7573 6520 746f 2074  ework I use to t
```

