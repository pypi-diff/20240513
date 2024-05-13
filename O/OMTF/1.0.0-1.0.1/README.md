# Comparing `tmp/omtf-1.0.0.tar.gz` & `tmp/omtf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omtf-1.0.0.tar", last modified: Mon May 13 10:54:27 2024, max compression
+gzip compressed data, was "omtf-1.0.1.tar", last modified: Mon May 13 14:01:59 2024, max compression
```

## Comparing `omtf-1.0.0.tar` & `omtf-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.878573 omtf-1.0.0/
--rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:27.000000 omtf-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1994 2024-05-13 10:54:27.877574 omtf-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.0/README.md
--rw-rw-rw-   0        0        0      568 2024-05-13 10:53:01.000000 omtf-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      778 2024-05-13 10:54:27.879574 omtf-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.823574 omtf-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.828575 omtf-1.0.0/src/Brokers/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.0/src/Brokers/__init__.py
--rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.0/src/Brokers/binance_broker.py
--rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.0/src/Brokers/degiro.py
--rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.0/src/Brokers/metatrader.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.842576 omtf-1.0.0/src/DataProviders/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.0/src/DataProviders/__init__.py
--rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.0/src/DataProviders/aemet.py
--rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.0/src/DataProviders/benzinga.py
--rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.0/src/DataProviders/coingecko.py
--rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.0/src/DataProviders/coinmarketcap.py
--rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.0/src/DataProviders/data.py
--rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.0/src/DataProviders/dilutionTracker.py
--rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.0/src/DataProviders/expansion.py
--rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.0/src/DataProviders/finviz.py
--rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.0/src/DataProviders/floatChecker.py
--rw-rw-rw-   0        0        0     2663 2024-05-13 10:01:06.000000 omtf-1.0.0/src/DataProviders/fmp.py
--rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.0/src/DataProviders/fxstreet.py
--rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.0/src/DataProviders/geonames.py
--rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.0/src/DataProviders/inversis_todo.py
--rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.0/src/DataProviders/marketWatch.py
--rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.0/src/DataProviders/oecd.py
--rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.0/src/DataProviders/openstreetmap.py
--rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.0/src/DataProviders/polygon.py
--rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.0/src/DataProviders/sec.py
--rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.0/src/DataProviders/tradingterminal.py
--rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.0/src/DataProviders/worldBank.py
--rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.0/src/DataProviders/worldHealthOrg.py
--rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.0/src/DataProviders/world_population.py
--rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.0/src/DataProviders/yahoo.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.854573 omtf-1.0.0/src/MachineLearning/
--rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.0/src/MachineLearning/00_models_comparison.py
--rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.0/src/MachineLearning/RandomForest.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.0/src/MachineLearning/__init__.py
--rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.0/src/MachineLearning/decision_trees.py
--rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.0/src/MachineLearning/genetic_algorithm.py
--rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.0/src/MachineLearning/gradientboosting.py
--rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.0/src/MachineLearning/k_nearest_neighbors.py
--rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.0/src/MachineLearning/kmeans_clustering.py
--rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.0/src/MachineLearning/linear_regression.py
--rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.0/src/MachineLearning/logistic_regression.py
--rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.0/src/MachineLearning/long_short_term_memory.py
--rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.0/src/MachineLearning/naive_bayes.py
--rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.0/src/MachineLearning/neural_networks.py
--rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.0/src/MachineLearning/principal_component.py
--rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.0/src/MachineLearning/random_forest.py
--rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.0/src/MachineLearning/recurrent_neural_networks.py
--rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.0/src/MachineLearning/support_vector.py
--rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.0/src/MachineLearning/utils.py
--rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.0/src/MachineLearning/xgboost_model.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.877574 omtf-1.0.0/src/OMTF.egg-info/
--rw-rw-rw-   0        0        0     1994 2024-05-13 10:54:27.000000 omtf-1.0.0/src/OMTF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2283 2024-05-13 10:54:27.000000 omtf-1.0.0/src/OMTF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 10:54:27.000000 omtf-1.0.0/src/OMTF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-13 10:54:27.000000 omtf-1.0.0/src/OMTF.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.875575 omtf-1.0.0/src/Trading/
--rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.0/src/Trading/KEYS.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.0/src/Trading/__init__.py
--rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.0/src/Trading/asset_tradeablitiy.py
--rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.0/src/Trading/backtest.py
--rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.0/src/Trading/backtest_utils.py
--rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.0/src/Trading/config.py
--rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.0/src/Trading/continuous_backtest.py
--rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.0/src/Trading/discrete_backtest.py
--rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.0/src/Trading/execution.py
--rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.0/src/Trading/execution_utils.py
--rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.0/src/Trading/indicators.py
--rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.0/src/Trading/portfolios.py
--rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.0/src/Trading/randomWalk.py
--rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.0/src/Trading/screeners.py
--rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.0/src/Trading/signals.py
--rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.0/src/Trading/technical.py
-drwxrwxrwx   0        0        0        0 2024-05-13 10:54:27.876575 omtf-1.0.0/src/sp500Historical/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.0/src/sp500Historical/__init__.py
--rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.0/src/sp500Historical/sp500_historical.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.890715 omtf-1.0.1/
+-rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      878 2024-05-13 14:01:59.890715 omtf-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.835715 omtf-1.0.1/omtf/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.840715 omtf-1.0.1/omtf/Brokers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.1/omtf/Brokers/__init__.py
+-rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.1/omtf/Brokers/binance_broker.py
+-rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.1/omtf/Brokers/degiro.py
+-rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.1/omtf/Brokers/metatrader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.856719 omtf-1.0.1/omtf/DataProviders/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.1/omtf/DataProviders/__init__.py
+-rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.1/omtf/DataProviders/aemet.py
+-rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.1/omtf/DataProviders/benzinga.py
+-rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.1/omtf/DataProviders/coingecko.py
+-rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.1/omtf/DataProviders/coinmarketcap.py
+-rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.1/omtf/DataProviders/data.py
+-rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.1/omtf/DataProviders/dilutionTracker.py
+-rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.1/omtf/DataProviders/expansion.py
+-rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.1/omtf/DataProviders/finviz.py
+-rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.1/omtf/DataProviders/floatChecker.py
+-rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.1/omtf/DataProviders/fmp.py
+-rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.1/omtf/DataProviders/fxstreet.py
+-rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.1/omtf/DataProviders/geonames.py
+-rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.1/omtf/DataProviders/inversis_todo.py
+-rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.1/omtf/DataProviders/marketWatch.py
+-rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.1/omtf/DataProviders/oecd.py
+-rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.1/omtf/DataProviders/openstreetmap.py
+-rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.1/omtf/DataProviders/polygon.py
+-rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.1/omtf/DataProviders/sec.py
+-rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.1/omtf/DataProviders/tradingterminal.py
+-rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.1/omtf/DataProviders/worldBank.py
+-rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.1/omtf/DataProviders/worldHealthOrg.py
+-rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.1/omtf/DataProviders/world_population.py
+-rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.1/omtf/DataProviders/yahoo.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.868716 omtf-1.0.1/omtf/MachineLearning/
+-rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.1/omtf/MachineLearning/00_models_comparison.py
+-rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.1/omtf/MachineLearning/RandomForest.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.1/omtf/MachineLearning/__init__.py
+-rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.1/omtf/MachineLearning/decision_trees.py
+-rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/gradientboosting.py
+-rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.1/omtf/MachineLearning/k_nearest_neighbors.py
+-rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.1/omtf/MachineLearning/kmeans_clustering.py
+-rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.1/omtf/MachineLearning/linear_regression.py
+-rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.1/omtf/MachineLearning/logistic_regression.py
+-rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/long_short_term_memory.py
+-rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.1/omtf/MachineLearning/naive_bayes.py
+-rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.1/omtf/MachineLearning/neural_networks.py
+-rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.1/omtf/MachineLearning/principal_component.py
+-rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.1/omtf/MachineLearning/random_forest.py
+-rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/recurrent_neural_networks.py
+-rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.1/omtf/MachineLearning/support_vector.py
+-rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.1/omtf/MachineLearning/utils.py
+-rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/xgboost_model.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.890715 omtf-1.0.1/omtf/OMTF.egg-info/
+-rw-rw-rw-   0        0        0      878 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2340 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.887718 omtf-1.0.1/omtf/Trading/
+-rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/Trading/KEYS.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.1/omtf/Trading/__init__.py
+-rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.1/omtf/Trading/asset_tradeablitiy.py
+-rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.1/omtf/Trading/backtest.py
+-rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.1/omtf/Trading/backtest_utils.py
+-rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.1/omtf/Trading/config.py
+-rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.1/omtf/Trading/continuous_backtest.py
+-rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.1/omtf/Trading/discrete_backtest.py
+-rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.1/omtf/Trading/execution.py
+-rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.1/omtf/Trading/execution_utils.py
+-rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.1/omtf/Trading/indicators.py
+-rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.1/omtf/Trading/portfolios.py
+-rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.1/omtf/Trading/randomWalk.py
+-rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.1/omtf/Trading/screeners.py
+-rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.1/omtf/Trading/signals.py
+-rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.1/omtf/Trading/technical.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.889715 omtf-1.0.1/omtf/sp500Historical/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.1/omtf/sp500Historical/__init__.py
+-rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.1/omtf/sp500Historical/sp500_historical.py
+-rw-rw-rw-   0        0        0      568 2024-05-13 10:53:01.000000 omtf-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      780 2024-05-13 14:01:59.892719 omtf-1.0.1/setup.cfg
```

### Comparing `omtf-1.0.0/LICENSE` & `omtf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/pyproject.toml` & `omtf-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/setup.cfg` & `omtf-1.0.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204f 4d54 460d 0a76 6572 7369 6f6e   = OMTF..version
-00000020: 203d 2031 2e30 2e30 0d0a 6175 7468 6f72   = 1.0.0..author
+00000020: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
 00000030: 203d 2044 616e 6965 6c20 4361 6e6f 0d0a   = Daniel Cano..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
 00000050: 6361 726f 6e6d 4067 6d61 696c 2e63 6f6d  caronm@gmail.com
 00000060: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000070: 4f4d 2054 7261 6469 6e67 2046 7261 6d65  OM Trading Frame
 00000080: 776f 726b 2069 7320 7468 6520 6672 616d  work is the fram
 00000090: 6577 6f72 6b20 4920 7573 6520 746f 2074  ework I use to t
@@ -34,16 +34,16 @@
 00000210: 203a 3a20 330d 0a09 4c69 6365 6e73 6520   :: 3...License 
 00000220: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
 00000230: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
 00000240: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
 00000250: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
 00000260: 656e 740d 0a0d 0a5b 6f70 7469 6f6e 735d  ent....[options]
 00000270: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
-00000280: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
-00000290: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000002a0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-000002b0: 332e 3130 0d0a 0d0a 5b6f 7074 696f 6e73  3.10....[options
-000002c0: 2e70 6163 6b61 6765 732e 6669 6e64 5d0d  .packages.find].
-000002d0: 0a77 6865 7265 203d 2073 7263 0d0a 0d0a  .where = src....
-000002e0: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
-000002f0: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
-00000300: 7465 203d 2030 0d0a 0d0a                 te = 0....
+00000280: 0d0a 093d 206f 6d74 660d 0a70 6163 6b61  ...= omtf..packa
+00000290: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
+000002a0: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
+000002b0: 3d33 2e31 300d 0a0d 0a5b 6f70 7469 6f6e  =3.10....[option
+000002c0: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+000002d0: 0d0a 7768 6572 6520 3d20 6f6d 7466 0d0a  ..where = omtf..
+000002e0: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+000002f0: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000300: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

### Comparing `omtf-1.0.0/src/Brokers/binance_broker.py` & `omtf-1.0.1/omtf/Brokers/binance_broker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Brokers/degiro.py` & `omtf-1.0.1/omtf/Brokers/degiro.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Brokers/metatrader.py` & `omtf-1.0.1/omtf/Brokers/metatrader.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/aemet.py` & `omtf-1.0.1/omtf/DataProviders/aemet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/benzinga.py` & `omtf-1.0.1/omtf/DataProviders/benzinga.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/coingecko.py` & `omtf-1.0.1/omtf/DataProviders/coingecko.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/coinmarketcap.py` & `omtf-1.0.1/omtf/DataProviders/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/data.py` & `omtf-1.0.1/omtf/DataProviders/data.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/dilutionTracker.py` & `omtf-1.0.1/omtf/DataProviders/dilutionTracker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/expansion.py` & `omtf-1.0.1/omtf/DataProviders/expansion.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/finviz.py` & `omtf-1.0.1/omtf/DataProviders/finviz.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/floatChecker.py` & `omtf-1.0.1/omtf/DataProviders/floatChecker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/fmp.py` & `omtf-1.0.1/omtf/DataProviders/fmp.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,9 +57,9 @@
         return self._request(url, params)
 
 
 
 
 if __name__ == '__main__':
 
-    fmp = FinancialModellingProp(api_key='aba9a750dd340f1afcb8fd2d959706de')
-    fmp.stocksList()
+    fmp = FinancialModellingProp(api_key='your-token')
+    fmp.stocksList()
```

### Comparing `omtf-1.0.0/src/DataProviders/fxstreet.py` & `omtf-1.0.1/omtf/DataProviders/fxstreet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/geonames.py` & `omtf-1.0.1/omtf/DataProviders/geonames.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/inversis_todo.py` & `omtf-1.0.1/omtf/DataProviders/inversis_todo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/marketWatch.py` & `omtf-1.0.1/omtf/DataProviders/marketWatch.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/oecd.py` & `omtf-1.0.1/omtf/DataProviders/oecd.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/openstreetmap.py` & `omtf-1.0.1/omtf/DataProviders/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/polygon.py` & `omtf-1.0.1/omtf/DataProviders/polygon.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/sec.py` & `omtf-1.0.1/omtf/DataProviders/sec.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/tradingterminal.py` & `omtf-1.0.1/omtf/DataProviders/tradingterminal.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/worldBank.py` & `omtf-1.0.1/omtf/DataProviders/worldBank.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/worldHealthOrg.py` & `omtf-1.0.1/omtf/DataProviders/worldHealthOrg.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/world_population.py` & `omtf-1.0.1/omtf/DataProviders/world_population.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/DataProviders/yahoo.py` & `omtf-1.0.1/omtf/DataProviders/yahoo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/00_models_comparison.py` & `omtf-1.0.1/omtf/MachineLearning/00_models_comparison.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/RandomForest.py` & `omtf-1.0.1/omtf/MachineLearning/RandomForest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/decision_trees.py` & `omtf-1.0.1/omtf/MachineLearning/decision_trees.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/genetic_algorithm.py` & `omtf-1.0.1/omtf/MachineLearning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/gradientboosting.py` & `omtf-1.0.1/omtf/MachineLearning/gradientboosting.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/k_nearest_neighbors.py` & `omtf-1.0.1/omtf/MachineLearning/k_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/kmeans_clustering.py` & `omtf-1.0.1/omtf/MachineLearning/kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/linear_regression.py` & `omtf-1.0.1/omtf/MachineLearning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/logistic_regression.py` & `omtf-1.0.1/omtf/MachineLearning/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/long_short_term_memory.py` & `omtf-1.0.1/omtf/MachineLearning/long_short_term_memory.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/naive_bayes.py` & `omtf-1.0.1/omtf/MachineLearning/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/neural_networks.py` & `omtf-1.0.1/omtf/MachineLearning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/principal_component.py` & `omtf-1.0.1/omtf/MachineLearning/principal_component.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/random_forest.py` & `omtf-1.0.1/omtf/MachineLearning/random_forest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/recurrent_neural_networks.py` & `omtf-1.0.1/omtf/MachineLearning/recurrent_neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/support_vector.py` & `omtf-1.0.1/omtf/MachineLearning/support_vector.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/utils.py` & `omtf-1.0.1/omtf/MachineLearning/utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/MachineLearning/xgboost_model.py` & `omtf-1.0.1/omtf/MachineLearning/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/asset_tradeablitiy.py` & `omtf-1.0.1/omtf/Trading/asset_tradeablitiy.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/backtest.py` & `omtf-1.0.1/omtf/Trading/backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/backtest_utils.py` & `omtf-1.0.1/omtf/Trading/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/config.py` & `omtf-1.0.1/omtf/Trading/config.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/continuous_backtest.py` & `omtf-1.0.1/omtf/Trading/continuous_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/discrete_backtest.py` & `omtf-1.0.1/omtf/Trading/discrete_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/execution.py` & `omtf-1.0.1/omtf/Trading/execution.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/execution_utils.py` & `omtf-1.0.1/omtf/Trading/execution_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/indicators.py` & `omtf-1.0.1/omtf/Trading/indicators.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/portfolios.py` & `omtf-1.0.1/omtf/Trading/portfolios.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/randomWalk.py` & `omtf-1.0.1/omtf/Trading/randomWalk.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/screeners.py` & `omtf-1.0.1/omtf/Trading/screeners.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/signals.py` & `omtf-1.0.1/omtf/Trading/signals.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/Trading/technical.py` & `omtf-1.0.1/omtf/Trading/technical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.0/src/sp500Historical/sp500_historical.py` & `omtf-1.0.1/omtf/sp500Historical/sp500_historical.py`

 * *Files identical despite different names*

