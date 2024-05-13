# Comparing `tmp/omtf-1.0.1.tar.gz` & `tmp/omtf-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omtf-1.0.1.tar", last modified: Mon May 13 14:01:59 2024, max compression
+gzip compressed data, was "omtf-1.0.2.tar", last modified: Mon May 13 14:12:55 2024, max compression
```

## Comparing `omtf-1.0.1.tar` & `omtf-1.0.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.890715 omtf-1.0.1/
--rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      878 2024-05-13 14:01:59.890715 omtf-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.835715 omtf-1.0.1/omtf/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.840715 omtf-1.0.1/omtf/Brokers/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.1/omtf/Brokers/__init__.py
--rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.1/omtf/Brokers/binance_broker.py
--rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.1/omtf/Brokers/degiro.py
--rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.1/omtf/Brokers/metatrader.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.856719 omtf-1.0.1/omtf/DataProviders/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.1/omtf/DataProviders/__init__.py
--rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.1/omtf/DataProviders/aemet.py
--rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.1/omtf/DataProviders/benzinga.py
--rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.1/omtf/DataProviders/coingecko.py
--rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.1/omtf/DataProviders/coinmarketcap.py
--rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.1/omtf/DataProviders/data.py
--rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.1/omtf/DataProviders/dilutionTracker.py
--rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.1/omtf/DataProviders/expansion.py
--rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.1/omtf/DataProviders/finviz.py
--rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.1/omtf/DataProviders/floatChecker.py
--rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.1/omtf/DataProviders/fmp.py
--rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.1/omtf/DataProviders/fxstreet.py
--rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.1/omtf/DataProviders/geonames.py
--rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.1/omtf/DataProviders/inversis_todo.py
--rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.1/omtf/DataProviders/marketWatch.py
--rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.1/omtf/DataProviders/oecd.py
--rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.1/omtf/DataProviders/openstreetmap.py
--rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.1/omtf/DataProviders/polygon.py
--rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.1/omtf/DataProviders/sec.py
--rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.1/omtf/DataProviders/tradingterminal.py
--rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.1/omtf/DataProviders/worldBank.py
--rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.1/omtf/DataProviders/worldHealthOrg.py
--rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.1/omtf/DataProviders/world_population.py
--rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.1/omtf/DataProviders/yahoo.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.868716 omtf-1.0.1/omtf/MachineLearning/
--rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.1/omtf/MachineLearning/00_models_comparison.py
--rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.1/omtf/MachineLearning/RandomForest.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.1/omtf/MachineLearning/__init__.py
--rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.1/omtf/MachineLearning/decision_trees.py
--rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/genetic_algorithm.py
--rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/gradientboosting.py
--rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.1/omtf/MachineLearning/k_nearest_neighbors.py
--rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.1/omtf/MachineLearning/kmeans_clustering.py
--rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.1/omtf/MachineLearning/linear_regression.py
--rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.1/omtf/MachineLearning/logistic_regression.py
--rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/long_short_term_memory.py
--rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.1/omtf/MachineLearning/naive_bayes.py
--rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.1/omtf/MachineLearning/neural_networks.py
--rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.1/omtf/MachineLearning/principal_component.py
--rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.1/omtf/MachineLearning/random_forest.py
--rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/recurrent_neural_networks.py
--rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.1/omtf/MachineLearning/support_vector.py
--rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.1/omtf/MachineLearning/utils.py
--rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/MachineLearning/xgboost_model.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.890715 omtf-1.0.1/omtf/OMTF.egg-info/
--rw-rw-rw-   0        0        0      878 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2340 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-13 14:01:59.000000 omtf-1.0.1/omtf/OMTF.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.887718 omtf-1.0.1/omtf/Trading/
--rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.1/omtf/Trading/KEYS.py
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.1/omtf/Trading/__init__.py
--rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.1/omtf/Trading/asset_tradeablitiy.py
--rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.1/omtf/Trading/backtest.py
--rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.1/omtf/Trading/backtest_utils.py
--rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.1/omtf/Trading/config.py
--rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.1/omtf/Trading/continuous_backtest.py
--rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.1/omtf/Trading/discrete_backtest.py
--rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.1/omtf/Trading/execution.py
--rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.1/omtf/Trading/execution_utils.py
--rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.1/omtf/Trading/indicators.py
--rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.1/omtf/Trading/portfolios.py
--rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.1/omtf/Trading/randomWalk.py
--rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.1/omtf/Trading/screeners.py
--rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.1/omtf/Trading/signals.py
--rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.1/omtf/Trading/technical.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:01:59.889715 omtf-1.0.1/omtf/sp500Historical/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.1/omtf/sp500Historical/__init__.py
--rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.1/omtf/sp500Historical/sp500_historical.py
--rw-rw-rw-   0        0        0      568 2024-05-13 10:53:01.000000 omtf-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      780 2024-05-13 14:01:59.892719 omtf-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.615536 omtf-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2024-05-13 10:23:42.000000 omtf-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      878 2024-05-13 14:12:55.615536 omtf-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      239 2024-05-13 10:01:20.000000 omtf-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.560538 omtf-1.0.2/omtf/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.565536 omtf-1.0.2/omtf/Brokers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:34.000000 omtf-1.0.2/omtf/Brokers/__init__.py
+-rw-rw-rw-   0        0        0    25562 2024-04-23 07:26:55.000000 omtf-1.0.2/omtf/Brokers/binance_broker.py
+-rw-rw-rw-   0        0        0    47308 2024-02-19 17:23:47.000000 omtf-1.0.2/omtf/Brokers/degiro.py
+-rw-rw-rw-   0        0        0    19726 2024-01-15 19:10:15.000000 omtf-1.0.2/omtf/Brokers/metatrader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.580539 omtf-1.0.2/omtf/DataProviders/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:21.000000 omtf-1.0.2/omtf/DataProviders/__init__.py
+-rw-rw-rw-   0        0        0     8382 2024-04-19 14:38:56.000000 omtf-1.0.2/omtf/DataProviders/aemet.py
+-rw-rw-rw-   0        0        0    35812 2024-05-13 09:59:43.000000 omtf-1.0.2/omtf/DataProviders/benzinga.py
+-rw-rw-rw-   0        0        0     3042 2024-05-13 10:01:15.000000 omtf-1.0.2/omtf/DataProviders/coingecko.py
+-rw-rw-rw-   0        0        0     3056 2024-05-13 10:01:16.000000 omtf-1.0.2/omtf/DataProviders/coinmarketcap.py
+-rw-rw-rw-   0        0        0     9297 2024-02-23 16:02:54.000000 omtf-1.0.2/omtf/DataProviders/data.py
+-rw-rw-rw-   0        0        0     8938 2024-05-13 10:01:12.000000 omtf-1.0.2/omtf/DataProviders/dilutionTracker.py
+-rw-rw-rw-   0        0        0    12959 2024-04-23 07:26:55.000000 omtf-1.0.2/omtf/DataProviders/expansion.py
+-rw-rw-rw-   0        0        0    23249 2024-05-13 10:01:11.000000 omtf-1.0.2/omtf/DataProviders/finviz.py
+-rw-rw-rw-   0        0        0     3006 2024-05-13 10:01:10.000000 omtf-1.0.2/omtf/DataProviders/floatChecker.py
+-rw-rw-rw-   0        0        0     2643 2024-05-13 13:55:30.000000 omtf-1.0.2/omtf/DataProviders/fmp.py
+-rw-rw-rw-   0        0        0     9109 2024-05-13 10:01:02.000000 omtf-1.0.2/omtf/DataProviders/fxstreet.py
+-rw-rw-rw-   0        0        0     3551 2024-05-13 07:26:11.000000 omtf-1.0.2/omtf/DataProviders/geonames.py
+-rw-rw-rw-   0        0        0     2033 2024-02-29 08:10:37.000000 omtf-1.0.2/omtf/DataProviders/inversis_todo.py
+-rw-rw-rw-   0        0        0     8326 2024-05-13 10:00:57.000000 omtf-1.0.2/omtf/DataProviders/marketWatch.py
+-rw-rw-rw-   0        0        0     2446 2024-03-01 15:37:47.000000 omtf-1.0.2/omtf/DataProviders/oecd.py
+-rw-rw-rw-   0        0        0     1980 2024-03-19 12:42:31.000000 omtf-1.0.2/omtf/DataProviders/openstreetmap.py
+-rw-rw-rw-   0        0        0    22943 2024-05-13 10:00:57.000000 omtf-1.0.2/omtf/DataProviders/polygon.py
+-rw-rw-rw-   0        0        0    10056 2024-05-13 10:00:56.000000 omtf-1.0.2/omtf/DataProviders/sec.py
+-rw-rw-rw-   0        0        0    11938 2024-05-13 10:00:55.000000 omtf-1.0.2/omtf/DataProviders/tradingterminal.py
+-rw-rw-rw-   0        0        0     5178 2024-03-01 15:35:37.000000 omtf-1.0.2/omtf/DataProviders/worldBank.py
+-rw-rw-rw-   0        0        0     4373 2024-03-01 15:40:01.000000 omtf-1.0.2/omtf/DataProviders/worldHealthOrg.py
+-rw-rw-rw-   0        0        0     2455 2024-03-19 21:36:21.000000 omtf-1.0.2/omtf/DataProviders/world_population.py
+-rw-rw-rw-   0        0        0    19767 2024-05-13 10:00:55.000000 omtf-1.0.2/omtf/DataProviders/yahoo.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.592536 omtf-1.0.2/omtf/MachineLearning/
+-rw-rw-rw-   0        0        0    20066 2024-05-13 10:00:54.000000 omtf-1.0.2/omtf/MachineLearning/00_models_comparison.py
+-rw-rw-rw-   0        0        0    12095 2024-05-13 10:02:40.000000 omtf-1.0.2/omtf/MachineLearning/RandomForest.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:16.000000 omtf-1.0.2/omtf/MachineLearning/__init__.py
+-rw-rw-rw-   0        0        0    17751 2024-05-13 10:01:40.000000 omtf-1.0.2/omtf/MachineLearning/decision_trees.py
+-rw-rw-rw-   0        0        0     9212 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/genetic_algorithm.py
+-rw-rw-rw-   0        0        0    16219 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/gradientboosting.py
+-rw-rw-rw-   0        0        0     7546 2024-05-13 10:01:49.000000 omtf-1.0.2/omtf/MachineLearning/k_nearest_neighbors.py
+-rw-rw-rw-   0        0        0     5862 2024-05-13 10:01:53.000000 omtf-1.0.2/omtf/MachineLearning/kmeans_clustering.py
+-rw-rw-rw-   0        0        0    18418 2024-05-13 10:01:58.000000 omtf-1.0.2/omtf/MachineLearning/linear_regression.py
+-rw-rw-rw-   0        0        0    16056 2024-05-13 10:02:01.000000 omtf-1.0.2/omtf/MachineLearning/logistic_regression.py
+-rw-rw-rw-   0        0        0    23342 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/long_short_term_memory.py
+-rw-rw-rw-   0        0        0     9880 2024-05-13 10:02:08.000000 omtf-1.0.2/omtf/MachineLearning/naive_bayes.py
+-rw-rw-rw-   0        0        0    33241 2024-05-13 10:02:12.000000 omtf-1.0.2/omtf/MachineLearning/neural_networks.py
+-rw-rw-rw-   0        0        0     8488 2024-05-13 10:02:16.000000 omtf-1.0.2/omtf/MachineLearning/principal_component.py
+-rw-rw-rw-   0        0        0     9422 2024-05-13 10:02:25.000000 omtf-1.0.2/omtf/MachineLearning/random_forest.py
+-rw-rw-rw-   0        0        0    18154 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/recurrent_neural_networks.py
+-rw-rw-rw-   0        0        0    11898 2024-05-13 10:02:58.000000 omtf-1.0.2/omtf/MachineLearning/support_vector.py
+-rw-rw-rw-   0        0        0    20912 2024-05-13 10:04:44.000000 omtf-1.0.2/omtf/MachineLearning/utils.py
+-rw-rw-rw-   0        0        0    13443 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/MachineLearning/xgboost_model.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.614536 omtf-1.0.2/omtf/OMTF.egg-info/
+-rw-rw-rw-   0        0        0      878 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2340 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-13 14:12:55.000000 omtf-1.0.2/omtf/OMTF.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.612538 omtf-1.0.2/omtf/Trading/
+-rw-rw-rw-   0        0        0      102 2024-01-04 16:12:49.000000 omtf-1.0.2/omtf/Trading/KEYS.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:03.000000 omtf-1.0.2/omtf/Trading/__init__.py
+-rw-rw-rw-   0        0        0     2766 2024-03-09 10:22:31.000000 omtf-1.0.2/omtf/Trading/asset_tradeablitiy.py
+-rw-rw-rw-   0        0        0    68759 2024-05-13 10:08:47.000000 omtf-1.0.2/omtf/Trading/backtest.py
+-rw-rw-rw-   0        0        0    26961 2024-05-13 10:07:25.000000 omtf-1.0.2/omtf/Trading/backtest_utils.py
+-rw-rw-rw-   0        0        0     9693 2024-05-13 10:08:58.000000 omtf-1.0.2/omtf/Trading/config.py
+-rw-rw-rw-   0        0        0    37259 2024-05-13 10:09:06.000000 omtf-1.0.2/omtf/Trading/continuous_backtest.py
+-rw-rw-rw-   0        0        0    44568 2024-05-13 10:09:12.000000 omtf-1.0.2/omtf/Trading/discrete_backtest.py
+-rw-rw-rw-   0        0        0    51835 2024-05-13 10:18:32.000000 omtf-1.0.2/omtf/Trading/execution.py
+-rw-rw-rw-   0        0        0    74814 2024-05-13 10:09:18.000000 omtf-1.0.2/omtf/Trading/execution_utils.py
+-rw-rw-rw-   0        0        0   136092 2024-05-13 10:05:58.000000 omtf-1.0.2/omtf/Trading/indicators.py
+-rw-rw-rw-   0        0        0    16776 2024-03-12 19:59:06.000000 omtf-1.0.2/omtf/Trading/portfolios.py
+-rw-rw-rw-   0        0        0    16607 2024-05-13 10:18:57.000000 omtf-1.0.2/omtf/Trading/randomWalk.py
+-rw-rw-rw-   0        0        0    17909 2024-05-13 10:19:58.000000 omtf-1.0.2/omtf/Trading/screeners.py
+-rw-rw-rw-   0        0        0   231068 2024-05-13 10:19:53.000000 omtf-1.0.2/omtf/Trading/signals.py
+-rw-rw-rw-   0        0        0    49172 2024-05-13 10:20:30.000000 omtf-1.0.2/omtf/Trading/technical.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:12:55.613536 omtf-1.0.2/omtf/sp500Historical/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:49:10.000000 omtf-1.0.2/omtf/sp500Historical/__init__.py
+-rw-rw-rw-   0        0        0     9782 2024-04-02 06:42:24.000000 omtf-1.0.2/omtf/sp500Historical/sp500_historical.py
+-rw-rw-rw-   0        0        0      568 2024-05-13 10:53:01.000000 omtf-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      780 2024-05-13 14:12:55.617537 omtf-1.0.2/setup.cfg
```

### Comparing `omtf-1.0.1/LICENSE` & `omtf-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/PKG-INFO` & `omtf-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.1
+Version: 1.0.2
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
 Home-page: https://github.com/Daniel-OM/OMTF
 Author: Daniel Cano
 Author-email: dcaronm@gmail.com
 Project-URL: Bug Tracker, https://github.com/Daniel-OM/OMTF/-/issues
 Project-URL: repository, https://github.com/Daniel-OM/OMTF
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omtf-1.0.1/omtf/Brokers/binance_broker.py` & `omtf-1.0.2/omtf/Brokers/binance_broker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Brokers/degiro.py` & `omtf-1.0.2/omtf/Brokers/degiro.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Brokers/metatrader.py` & `omtf-1.0.2/omtf/Brokers/metatrader.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/aemet.py` & `omtf-1.0.2/omtf/DataProviders/aemet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/benzinga.py` & `omtf-1.0.2/omtf/DataProviders/benzinga.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/coingecko.py` & `omtf-1.0.2/omtf/DataProviders/coingecko.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/coinmarketcap.py` & `omtf-1.0.2/omtf/DataProviders/coinmarketcap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/data.py` & `omtf-1.0.2/omtf/DataProviders/data.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/dilutionTracker.py` & `omtf-1.0.2/omtf/DataProviders/dilutionTracker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/expansion.py` & `omtf-1.0.2/omtf/DataProviders/expansion.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/finviz.py` & `omtf-1.0.2/omtf/DataProviders/finviz.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/floatChecker.py` & `omtf-1.0.2/omtf/DataProviders/floatChecker.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/fmp.py` & `omtf-1.0.2/omtf/DataProviders/fmp.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/fxstreet.py` & `omtf-1.0.2/omtf/DataProviders/fxstreet.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/geonames.py` & `omtf-1.0.2/omtf/DataProviders/geonames.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/inversis_todo.py` & `omtf-1.0.2/omtf/DataProviders/inversis_todo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/marketWatch.py` & `omtf-1.0.2/omtf/DataProviders/marketWatch.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/oecd.py` & `omtf-1.0.2/omtf/DataProviders/oecd.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/openstreetmap.py` & `omtf-1.0.2/omtf/DataProviders/openstreetmap.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/polygon.py` & `omtf-1.0.2/omtf/DataProviders/polygon.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/sec.py` & `omtf-1.0.2/omtf/DataProviders/sec.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/tradingterminal.py` & `omtf-1.0.2/omtf/DataProviders/tradingterminal.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/worldBank.py` & `omtf-1.0.2/omtf/DataProviders/worldBank.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/worldHealthOrg.py` & `omtf-1.0.2/omtf/DataProviders/worldHealthOrg.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/world_population.py` & `omtf-1.0.2/omtf/DataProviders/world_population.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/DataProviders/yahoo.py` & `omtf-1.0.2/omtf/DataProviders/yahoo.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/00_models_comparison.py` & `omtf-1.0.2/omtf/MachineLearning/00_models_comparison.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/RandomForest.py` & `omtf-1.0.2/omtf/MachineLearning/RandomForest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/decision_trees.py` & `omtf-1.0.2/omtf/MachineLearning/decision_trees.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/genetic_algorithm.py` & `omtf-1.0.2/omtf/MachineLearning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/gradientboosting.py` & `omtf-1.0.2/omtf/MachineLearning/gradientboosting.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/k_nearest_neighbors.py` & `omtf-1.0.2/omtf/MachineLearning/k_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/kmeans_clustering.py` & `omtf-1.0.2/omtf/MachineLearning/kmeans_clustering.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/linear_regression.py` & `omtf-1.0.2/omtf/MachineLearning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/logistic_regression.py` & `omtf-1.0.2/omtf/MachineLearning/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/long_short_term_memory.py` & `omtf-1.0.2/omtf/MachineLearning/long_short_term_memory.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/naive_bayes.py` & `omtf-1.0.2/omtf/MachineLearning/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/neural_networks.py` & `omtf-1.0.2/omtf/MachineLearning/neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/principal_component.py` & `omtf-1.0.2/omtf/MachineLearning/principal_component.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/random_forest.py` & `omtf-1.0.2/omtf/MachineLearning/random_forest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/recurrent_neural_networks.py` & `omtf-1.0.2/omtf/MachineLearning/recurrent_neural_networks.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/support_vector.py` & `omtf-1.0.2/omtf/MachineLearning/support_vector.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/utils.py` & `omtf-1.0.2/omtf/MachineLearning/utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/MachineLearning/xgboost_model.py` & `omtf-1.0.2/omtf/MachineLearning/xgboost_model.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/OMTF.egg-info/PKG-INFO` & `omtf-1.0.2/omtf/OMTF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OMTF
-Version: 1.0.1
+Version: 1.0.2
 Summary: OM Trading Framework is the framework I use to test my strategies and carry out the portfolio management.
 Home-page: https://github.com/Daniel-OM/OMTF
 Author: Daniel Cano
 Author-email: dcaronm@gmail.com
 Project-URL: Bug Tracker, https://github.com/Daniel-OM/OMTF/-/issues
 Project-URL: repository, https://github.com/Daniel-OM/OMTF
 Classifier: Programming Language :: Python :: 3
```

### Comparing `omtf-1.0.1/omtf/OMTF.egg-info/SOURCES.txt` & `omtf-1.0.2/omtf/OMTF.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/asset_tradeablitiy.py` & `omtf-1.0.2/omtf/Trading/asset_tradeablitiy.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/backtest.py` & `omtf-1.0.2/omtf/Trading/backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/backtest_utils.py` & `omtf-1.0.2/omtf/Trading/backtest_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/config.py` & `omtf-1.0.2/omtf/Trading/config.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/continuous_backtest.py` & `omtf-1.0.2/omtf/Trading/continuous_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/discrete_backtest.py` & `omtf-1.0.2/omtf/Trading/discrete_backtest.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/execution.py` & `omtf-1.0.2/omtf/Trading/execution.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/execution_utils.py` & `omtf-1.0.2/omtf/Trading/execution_utils.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/indicators.py` & `omtf-1.0.2/omtf/Trading/indicators.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/portfolios.py` & `omtf-1.0.2/omtf/Trading/portfolios.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/randomWalk.py` & `omtf-1.0.2/omtf/Trading/randomWalk.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/screeners.py` & `omtf-1.0.2/omtf/Trading/screeners.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/signals.py` & `omtf-1.0.2/omtf/Trading/signals.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/Trading/technical.py` & `omtf-1.0.2/omtf/Trading/technical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/omtf/sp500Historical/sp500_historical.py` & `omtf-1.0.2/omtf/sp500Historical/sp500_historical.py`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/pyproject.toml` & `omtf-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `omtf-1.0.1/setup.cfg` & `omtf-1.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204f 4d54 460d 0a76 6572 7369 6f6e   = OMTF..version
-00000020: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
+00000020: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
 00000030: 203d 2044 616e 6965 6c20 4361 6e6f 0d0a   = Daniel Cano..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2064  author_email = d
 00000050: 6361 726f 6e6d 4067 6d61 696c 2e63 6f6d  caronm@gmail.com
 00000060: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000070: 4f4d 2054 7261 6469 6e67 2046 7261 6d65  OM Trading Frame
 00000080: 776f 726b 2069 7320 7468 6520 6672 616d  work is the fram
 00000090: 6577 6f72 6b20 4920 7573 6520 746f 2074  ework I use to t
```

