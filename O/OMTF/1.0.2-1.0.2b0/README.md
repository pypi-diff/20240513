# Comparing `tmp/omtf-1.0.2.tar.gz` & `tmp/omtf-1.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omtf-1.0.2.tar", last modified: Mon May 13 14:12:55 2024, max compression
+gzip compressed data, was "omtf-1.0.2b0.tar", last modified: Mon May 13 14:37:21 2024, max compression
```

## Comparing `omtf-1.0.2.tar` & `omtf-1.0.2b0.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.615536 omtf-1.0.2/
--rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      878 2024-05-13 14:12:55.615536 omtf-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.560538 omtf-1.0.2/omtf/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.565536 omtf-1.0.2/omtf/Brokers/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.2/omtf/Brokers/__init__.py
--rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.2/omtf/Brokers/binance_broker.py
--rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.2/omtf/Brokers/degiro.py
--rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.2/omtf/Brokers/metatrader.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.580539 omtf-1.0.2/omtf/DataProviders/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.2/omtf/DataProviders/__init__.py
--rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.2/omtf/DataProviders/aemet.py
--rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.2/omtf/DataProviders/benzinga.py
--rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.2/omtf/DataProviders/coingecko.py
--rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.2/omtf/DataProviders/coinmarketcap.py
--rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.2/omtf/DataProviders/data.py
--rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.2/omtf/DataProviders/dilutionTracker.py
--rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.2/omtf/DataProviders/expansion.py
--rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.2/omtf/DataProviders/finviz.py
--rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.2/omtf/DataProviders/floatChecker.py
--rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.2/omtf/DataProviders/fmp.py
--rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.2/omtf/DataProviders/fxstreet.py
--rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.2/omtf/DataProviders/geonames.py
--rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.2/omtf/DataProviders/inversis_todo.py
--rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.2/omtf/DataProviders/marketWatch.py
--rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.2/omtf/DataProviders/oecd.py
--rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.2/omtf/DataProviders/openstreetmap.py
--rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.2/omtf/DataProviders/polygon.py
--rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.2/omtf/DataProviders/sec.py
--rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.2/omtf/DataProviders/tradingterminal.py
--rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.2/omtf/DataProviders/worldBank.py
--rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.2/omtf/DataProviders/worldHealthOrg.py
--rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.2/omtf/DataProviders/world_population.py
--rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.2/omtf/DataProviders/yahoo.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.592536 omtf-1.0.2/omtf/MachineLearning/
--rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.2/omtf/MachineLearning/00_models_comparison.py
--rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.2/omtf/MachineLearning/RandomForest.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.2/omtf/MachineLearning/__init__.py
--rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.2/omtf/MachineLearning/decision_trees.py
--rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/genetic_algorithm.py
--rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/gradientboosting.py
--rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.2/omtf/MachineLearning/k_nearest_neighbors.py
--rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.2/omtf/MachineLearning/kmeans_clustering.py
--rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.2/omtf/MachineLearning/linear_regression.py
--rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.2/omtf/MachineLearning/logistic_regression.py
--rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/long_short_term_memory.py
--rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.2/omtf/MachineLearning/naive_bayes.py
--rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.2/omtf/MachineLearning/neural_networks.py
--rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.2/omtf/MachineLearning/principal_component.py
--rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.2/omtf/MachineLearning/random_forest.py
--rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/recurrent_neural_networks.py
--rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.2/omtf/MachineLearning/support_vector.py
--rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.2/omtf/MachineLearning/utils.py
--rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/xgboost_model.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.614536 omtf-1.0.2/omtf/OMTF.egg-info/
--rw-rw-rw-   0        0        0      878 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2340 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.612538 omtf-1.0.2/omtf/Trading/
--rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/Trading/KEYS.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.2/omtf/Trading/__init__.py
--rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.2/omtf/Trading/asset_tradeablitiy.py
--rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.2/omtf/Trading/backtest.py
--rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.2/omtf/Trading/backtest_utils.py
--rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.2/omtf/Trading/config.py
--rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.2/omtf/Trading/continuous_backtest.py
--rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.2/omtf/Trading/discrete_backtest.py
--rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.2/omtf/Trading/execution.py
--rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.2/omtf/Trading/execution_utils.py
--rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.2/omtf/Trading/indicators.py
--rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.2/omtf/Trading/portfolios.py
--rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.2/omtf/Trading/randomWalk.py
--rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.2/omtf/Trading/screeners.py
--rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.2/omtf/Trading/signals.py
--rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.2/omtf/Trading/technical.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.613536 omtf-1.0.2/omtf/sp500Historical/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.2/omtf/sp500Historical/__init__.py
--rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.2/omtf/sp500Historical/sp500_historical.py
--rw-rw-rw-   0        0        0      568 2024-05-13 10:53:01.000000 omtf-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      780 2024-05-13 14:12:55.617537 omtf-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.234284 omtf-1.0.2b0/
+-rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.2b0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.137284 omtf-1.0.2b0/OMTF/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.189285 omtf-1.0.2b0/OMTF/Brokers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.2b0/OMTF/Brokers/__init__.py
+-rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.2b0/OMTF/Brokers/binance_broker.py
+-rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.2b0/OMTF/Brokers/degiro.py
+-rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.2b0/OMTF/Brokers/metatrader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.206284 omtf-1.0.2b0/OMTF/DataProviders/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.2b0/OMTF/DataProviders/__init__.py
+-rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.2b0/OMTF/DataProviders/aemet.py
+-rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.2b0/OMTF/DataProviders/benzinga.py
+-rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.2b0/OMTF/DataProviders/coingecko.py
+-rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.2b0/OMTF/DataProviders/coinmarketcap.py
+-rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.2b0/OMTF/DataProviders/data.py
+-rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.2b0/OMTF/DataProviders/dilutionTracker.py
+-rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.2b0/OMTF/DataProviders/expansion.py
+-rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.2b0/OMTF/DataProviders/finviz.py
+-rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.2b0/OMTF/DataProviders/floatChecker.py
+-rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.2b0/OMTF/DataProviders/fmp.py
+-rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.2b0/OMTF/DataProviders/fxstreet.py
+-rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.2b0/OMTF/DataProviders/geonames.py
+-rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.2b0/OMTF/DataProviders/inversis_todo.py
+-rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.2b0/OMTF/DataProviders/marketWatch.py
+-rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.2b0/OMTF/DataProviders/oecd.py
+-rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.2b0/OMTF/DataProviders/openstreetmap.py
+-rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.2b0/OMTF/DataProviders/polygon.py
+-rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.2b0/OMTF/DataProviders/sec.py
+-rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.2b0/OMTF/DataProviders/tradingterminal.py
+-rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.2b0/OMTF/DataProviders/worldBank.py
+-rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.2b0/OMTF/DataProviders/worldHealthOrg.py
+-rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.2b0/OMTF/DataProviders/world_population.py
+-rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.2b0/OMTF/DataProviders/yahoo.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.220285 omtf-1.0.2b0/OMTF/MachineLearning/
+-rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.2b0/OMTF/MachineLearning/00_models_comparison.py
+-rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.2b0/OMTF/MachineLearning/RandomForest.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.2b0/OMTF/MachineLearning/__init__.py
+-rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.2b0/OMTF/MachineLearning/decision_trees.py
+-rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/gradientboosting.py
+-rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/k_nearest_neighbors.py
+-rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.2b0/OMTF/MachineLearning/kmeans_clustering.py
+-rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.2b0/OMTF/MachineLearning/linear_regression.py
+-rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.2b0/OMTF/MachineLearning/logistic_regression.py
+-rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/long_short_term_memory.py
+-rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.2b0/OMTF/MachineLearning/naive_bayes.py
+-rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.2b0/OMTF/MachineLearning/neural_networks.py
+-rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.2b0/OMTF/MachineLearning/principal_component.py
+-rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.2b0/OMTF/MachineLearning/random_forest.py
+-rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/recurrent_neural_networks.py
+-rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.2b0/OMTF/MachineLearning/support_vector.py
+-rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.2b0/OMTF/MachineLearning/utils.py
+-rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/MachineLearning/xgboost_model.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.231285 omtf-1.0.2b0/OMTF/Trading/
+-rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.2b0/OMTF/Trading/KEYS.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.2b0/OMTF/Trading/__init__.py
+-rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.2b0/OMTF/Trading/asset_tradeablitiy.py
+-rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.2b0/OMTF/Trading/backtest.py
+-rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.2b0/OMTF/Trading/backtest_utils.py
+-rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.2b0/OMTF/Trading/config.py
+-rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.2b0/OMTF/Trading/continuous_backtest.py
+-rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.2b0/OMTF/Trading/discrete_backtest.py
+-rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.2b0/OMTF/Trading/execution.py
+-rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.2b0/OMTF/Trading/execution_utils.py
+-rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.2b0/OMTF/Trading/indicators.py
+-rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.2b0/OMTF/Trading/portfolios.py
+-rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.2b0/OMTF/Trading/randomWalk.py
+-rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.2b0/OMTF/Trading/screeners.py
+-rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.2b0/OMTF/Trading/signals.py
+-rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.2b0/OMTF/Trading/technical.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 14:08:33.000000 omtf-1.0.2b0/OMTF/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.232285 omtf-1.0.2b0/OMTF/sp500Historical/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.2b0/OMTF/sp500Historical/__init__.py
+-rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.2b0/OMTF/sp500Historical/sp500_historical.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.234284 omtf-1.0.2b0/OMTF.egg-info/
+-rw-rw-rw-   0        0        0     1010 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4521 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:37:21.000000 omtf-1.0.2b0/OMTF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1010 2024-05-13 14:37:21.234284 omtf-1.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.2b0/README.md
+-rw-rw-rw-   0        0        0     1321 2024-05-13 14:36:47.000000 omtf-1.0.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2024-05-13 14:37:21.240285 omtf-1.0.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:37:21.233284 omtf-1.0.2b0/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:51:01.000000 omtf-1.0.2b0/tests/__init__.py
```

### Comparing `omtf-1.0.2/LICENSE` & `omtf-1.0.2b0/LICENSE`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/PKG-INFO` & `omtf-1.0.2b0/OMTF.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.2
+Version: 1.0.2b0
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
-Home-page: https://github.com/Daniel-OM/OMTF
+Home-page: https://onemade.es
 Author: Daniel Cano
-Author-email: dcaronm@gmail.com
-Project-URL: Bug Tracker, https://github.com/Daniel-OM/OMTF/-/issues
-Project-URL: repository, https://github.com/Daniel-OM/OMTF
+Author-email: Daniel Cano <dcaronm@gmail.com>
+Maintainer-email: Daniel Cano <dcaronm@gmail.com>
+Project-URL: Homepage, https://onemade.es
+Project-URL: Repository, https://github.com/Daniel-OM/OMTF
+Project-URL: Issues, https://github.com/Daniel-OM/OMTF/issues
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `omtf-1.0.2/omtf/Brokers/binance_broker.py` & `omtf-1.0.2b0/OMTF/Brokers/binance_broker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Brokers/degiro.py` & `omtf-1.0.2b0/OMTF/Brokers/degiro.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Brokers/metatrader.py` & `omtf-1.0.2b0/OMTF/Brokers/metatrader.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/aemet.py` & `omtf-1.0.2b0/OMTF/DataProviders/aemet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/benzinga.py` & `omtf-1.0.2b0/OMTF/DataProviders/benzinga.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/coingecko.py` & `omtf-1.0.2b0/OMTF/DataProviders/coingecko.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/coinmarketcap.py` & `omtf-1.0.2b0/OMTF/DataProviders/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/data.py` & `omtf-1.0.2b0/OMTF/DataProviders/data.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/dilutionTracker.py` & `omtf-1.0.2b0/OMTF/DataProviders/dilutionTracker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/expansion.py` & `omtf-1.0.2b0/OMTF/DataProviders/expansion.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/finviz.py` & `omtf-1.0.2b0/OMTF/DataProviders/finviz.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/floatChecker.py` & `omtf-1.0.2b0/OMTF/DataProviders/floatChecker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/fmp.py` & `omtf-1.0.2b0/OMTF/DataProviders/fmp.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/fxstreet.py` & `omtf-1.0.2b0/OMTF/DataProviders/fxstreet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/geonames.py` & `omtf-1.0.2b0/OMTF/DataProviders/geonames.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/inversis_todo.py` & `omtf-1.0.2b0/OMTF/DataProviders/inversis_todo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/marketWatch.py` & `omtf-1.0.2b0/OMTF/DataProviders/marketWatch.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/oecd.py` & `omtf-1.0.2b0/OMTF/DataProviders/oecd.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/openstreetmap.py` & `omtf-1.0.2b0/OMTF/DataProviders/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/polygon.py` & `omtf-1.0.2b0/OMTF/DataProviders/polygon.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/sec.py` & `omtf-1.0.2b0/OMTF/DataProviders/sec.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/tradingterminal.py` & `omtf-1.0.2b0/OMTF/DataProviders/tradingterminal.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/worldBank.py` & `omtf-1.0.2b0/OMTF/DataProviders/worldBank.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/worldHealthOrg.py` & `omtf-1.0.2b0/OMTF/DataProviders/worldHealthOrg.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/world_population.py` & `omtf-1.0.2b0/OMTF/DataProviders/world_population.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/DataProviders/yahoo.py` & `omtf-1.0.2b0/OMTF/DataProviders/yahoo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/00_models_comparison.py` & `omtf-1.0.2b0/OMTF/MachineLearning/00_models_comparison.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/RandomForest.py` & `omtf-1.0.2b0/OMTF/MachineLearning/RandomForest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/decision_trees.py` & `omtf-1.0.2b0/OMTF/MachineLearning/decision_trees.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/genetic_algorithm.py` & `omtf-1.0.2b0/OMTF/MachineLearning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/gradientboosting.py` & `omtf-1.0.2b0/OMTF/MachineLearning/gradientboosting.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/k_nearest_neighbors.py` & `omtf-1.0.2b0/OMTF/MachineLearning/k_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/kmeans_clustering.py` & `omtf-1.0.2b0/OMTF/MachineLearning/kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/linear_regression.py` & `omtf-1.0.2b0/OMTF/MachineLearning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/logistic_regression.py` & `omtf-1.0.2b0/OMTF/MachineLearning/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/long_short_term_memory.py` & `omtf-1.0.2b0/OMTF/MachineLearning/long_short_term_memory.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/naive_bayes.py` & `omtf-1.0.2b0/OMTF/MachineLearning/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/neural_networks.py` & `omtf-1.0.2b0/OMTF/MachineLearning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/principal_component.py` & `omtf-1.0.2b0/OMTF/MachineLearning/principal_component.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/random_forest.py` & `omtf-1.0.2b0/OMTF/MachineLearning/random_forest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/recurrent_neural_networks.py` & `omtf-1.0.2b0/OMTF/MachineLearning/recurrent_neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/support_vector.py` & `omtf-1.0.2b0/OMTF/MachineLearning/support_vector.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/utils.py` & `omtf-1.0.2b0/OMTF/MachineLearning/utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/MachineLearning/xgboost_model.py` & `omtf-1.0.2b0/OMTF/MachineLearning/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/OMTF.egg-info/PKG-INFO` & `omtf-1.0.2b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.2
+Version: 1.0.2b0
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
-Home-page: https://github.com/Daniel-OM/OMTF
+Home-page: https://onemade.es
 Author: Daniel Cano
-Author-email: dcaronm@gmail.com
-Project-URL: Bug Tracker, https://github.com/Daniel-OM/OMTF/-/issues
-Project-URL: repository, https://github.com/Daniel-OM/OMTF
+Author-email: Daniel Cano <dcaronm@gmail.com>
+Maintainer-email: Daniel Cano <dcaronm@gmail.com>
+Project-URL: Homepage, https://onemade.es
+Project-URL: Repository, https://github.com/Daniel-OM/OMTF
+Project-URL: Issues, https://github.com/Daniel-OM/OMTF/issues
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `omtf-1.0.2/omtf/Trading/asset_tradeablitiy.py` & `omtf-1.0.2b0/OMTF/Trading/asset_tradeablitiy.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/backtest.py` & `omtf-1.0.2b0/OMTF/Trading/backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/backtest_utils.py` & `omtf-1.0.2b0/OMTF/Trading/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/config.py` & `omtf-1.0.2b0/OMTF/Trading/config.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/continuous_backtest.py` & `omtf-1.0.2b0/OMTF/Trading/continuous_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/discrete_backtest.py` & `omtf-1.0.2b0/OMTF/Trading/discrete_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/execution.py` & `omtf-1.0.2b0/OMTF/Trading/execution.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/execution_utils.py` & `omtf-1.0.2b0/OMTF/Trading/execution_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/indicators.py` & `omtf-1.0.2b0/OMTF/Trading/indicators.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/portfolios.py` & `omtf-1.0.2b0/OMTF/Trading/portfolios.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/randomWalk.py` & `omtf-1.0.2b0/OMTF/Trading/randomWalk.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/screeners.py` & `omtf-1.0.2b0/OMTF/Trading/screeners.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/signals.py` & `omtf-1.0.2b0/OMTF/Trading/signals.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/Trading/technical.py` & `omtf-1.0.2b0/OMTF/Trading/technical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/omtf/sp500Historical/sp500_historical.py` & `omtf-1.0.2b0/OMTF/sp500Historical/sp500_historical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.2/setup.cfg` & `omtf-1.0.2b0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -14,36 +14,33 @@
 000000d0: 6e61 6765 6d65 6e74 2e0d 0a6c 6f6e 675f  nagement...long_
 000000e0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000f0: 6c65 3a20 5245 4144 4d45 2e6d 642c 204c  le: README.md, L
 00000100: 4943 454e 5345 2e74 7874 0d0a 6c6f 6e67  ICENSE.txt..long
 00000110: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
 00000120: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
 00000130: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-00000140: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000150: 636f 6d2f 4461 6e69 656c 2d4f 4d2f 4f4d  com/Daniel-OM/OM
-00000160: 5446 0d0a 7072 6f6a 6563 745f 7572 6c73  TF..project_urls
-00000170: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-00000180: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000190: 7562 2e63 6f6d 2f44 616e 6965 6c2d 4f4d  ub.com/Daniel-OM
-000001a0: 2f4f 4d54 462f 2d2f 6973 7375 6573 0d0a  /OMTF/-/issues..
-000001b0: 0972 6570 6f73 6974 6f72 7920 3d20 6874  .repository = ht
-000001c0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000001d0: 2f44 616e 6965 6c2d 4f4d 2f4f 4d54 460d  /Daniel-OM/OMTF.
-000001e0: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-000001f0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000200: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000210: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
-00000220: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000230: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000240: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000250: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
-00000260: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
-00000270: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000280: 0d0a 093d 206f 6d74 660d 0a70 6163 6b61  ...= omtf..packa
-00000290: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-000002a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-000002b0: 3d33 2e31 300d 0a0d 0a5b 6f70 7469 6f6e  =3.10....[option
-000002c0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-000002d0: 0d0a 7768 6572 6520 3d20 6f6d 7466 0d0a  ..where = omtf..
-000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
-000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
-00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
+00000140: 2068 7474 7073 3a2f 2f6f 6e65 6d61 6465   https://onemade
+00000150: 2e65 730d 0a70 726f 6a65 6374 5f75 726c  .es..project_url
+00000160: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+00000170: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+00000180: 6875 622e 636f 6d2f 4461 6e69 656c 2d4f  hub.com/Daniel-O
+00000190: 4d2f 4f4d 5446 2f69 7373 7565 730d 0a09  M/OMTF/issues...
+000001a0: 7265 706f 7369 746f 7279 203d 2068 7474  repository = htt
+000001b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000001c0: 4461 6e69 656c 2d4f 4d2f 4f4d 5446 0d0a  Daniel-OM/OMTF..
+000001d0: 636c 6173 7369 6669 6572 7320 3d20 0d0a  classifiers = ..
+000001e0: 0944 6576 656c 6f70 6d65 6e74 2053 7461  .Development Sta
+000001f0: 7475 7320 3a3a 2034 202d 2042 6574 610d  tus :: 4 - Beta.
+00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000220: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
+00000230: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
+00000240: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
+00000250: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+00000260: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+00000270: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
+00000280: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000290: 643a 0d0a 7079 7468 6f6e 5f72 6571 7569  d:..python_requi
+000002a0: 7265 7320 3d20 3e3d 332e 3130 0d0a 0d0a  res = >=3.10....
+000002b0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+000002c0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+000002d0: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

