# Comparing `tmp/emhass-0.9.0.tar.gz` & `tmp/emhass-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emhass-0.9.0.tar", last modified: Fri May 10 20:15:36 2024, max compression
+gzip compressed data, was "emhass-0.9.1.tar", last modified: Mon May 13 21:08:01 2024, max compression
```

## Comparing `emhass-0.9.0.tar` & `emhass-0.9.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-05-10 20:15:32.000000 emhass-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-10 20:15:32.000000 emhass-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-10 20:15:32.000000 emhass-0.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-10 20:15:32.000000 emhass-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-10 20:15:32.000000 emhass-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-10 20:15:36.103846 emhass-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    34444 2024-05-10 20:15:32.000000 emhass-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.095846 emhass-0.9.0/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_load_cost_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_load_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_prod_price_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_train_load_clustering.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_train_load_forecast.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-10 20:15:32.000000 emhass-0.9.0/data/data_weather_forecast.csv
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-10 20:15:32.000000 emhass-0.9.0/data/heating_prediction.csv
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_latest.csv
--rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_cost.csv
--rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_profit.csv
--rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-05-10 20:15:32.000000 emhass-0.9.0/data/opt_res_perfect_optim_self-consumption.csv
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_df_final.pkl
--rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_get_data_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_scrapper_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_solarforecast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-10 20:15:32.000000 emhass-0.9.0/data/test_response_solcast_get_method.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-10 20:15:32.000000 emhass-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 20:15:36.103846 emhass-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-10 20:15:32.000000 emhass-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.091846 emhass-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.095846 emhass-0.9.0/src/emhass/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47953 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.099846 emhass-0.9.0/src/emhass/data/
--rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/data/cec_inverters.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/data/cec_modules.pbz2
--rw-r--r--   0 runner    (1001) docker     (127)    47259 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/machine_learning_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    37252 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    21025 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/retrieve_hass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.099846 emhass-0.9.0/src/emhass/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/advanced.html
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/basic.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/emhass_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/emhass_logo_short.svg
--rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/img/feather-sprite.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/script.js
--rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/templates/template.html
--rw-r--r--   0 runner    (1001) docker     (127)    47801 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-05-10 20:15:32.000000 emhass-0.9.0/src/emhass/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/src/emhass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    35602 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 20:15:36.000000 emhass-0.9.0/src/emhass.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 20:15:36.103846 emhass-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    30422 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_command_line_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    31834 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_machine_learning_forecaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_machine_learning_regressor.py
--rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_retrieve_hass.py
--rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-05-10 20:15:32.000000 emhass-0.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.600784 emhass-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    22790 2024-05-13 21:07:58.000000 emhass-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-13 21:07:58.000000 emhass-0.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 21:07:58.000000 emhass-0.9.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-13 21:07:58.000000 emhass-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 21:07:58.000000 emhass-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-05-13 21:08:01.600784 emhass-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    34766 2024-05-13 21:07:58.000000 emhass-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.592784 emhass-0.9.1/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_load_cost_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_load_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_prod_price_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   185427 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_train_load_clustering.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   185431 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_train_load_forecast.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-13 21:07:58.000000 emhass-0.9.1/data/data_weather_forecast.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-13 21:07:58.000000 emhass-0.9.1/data/heating_prediction.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-13 21:07:58.000000 emhass-0.9.1/data/opt_res_latest.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    54568 2024-05-13 21:07:58.000000 emhass-0.9.1/data/opt_res_perfect_optim_cost.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    52501 2024-05-13 21:07:58.000000 emhass-0.9.1/data/opt_res_perfect_optim_profit.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    53838 2024-05-13 21:07:58.000000 emhass-0.9.1/data/opt_res_perfect_optim_self-consumption.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-13 21:07:58.000000 emhass-0.9.1/data/test_df_final.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-05-13 21:07:58.000000 emhass-0.9.1/data/test_response_get_data_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     9515 2024-05-13 21:07:58.000000 emhass-0.9.1/data/test_response_scrapper_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-13 21:07:58.000000 emhass-0.9.1/data/test_response_solarforecast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-13 21:07:58.000000 emhass-0.9.1/data/test_response_solcast_get_method.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 21:07:58.000000 emhass-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:08:01.600784 emhass-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-13 21:07:58.000000 emhass-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.584784 emhass-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.592784 emhass-0.9.1/src/emhass/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47908 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/command_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.592784 emhass-0.9.1/src/emhass/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   168272 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/data/cec_inverters.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)  1655747 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/data/cec_modules.pbz2
+-rw-r--r--   0 runner    (1001) docker     (127)    47076 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10407 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/machine_learning_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37252 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20391 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/retrieve_hass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.596784 emhass-0.9.1/src/emhass/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/advanced.html
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/basic.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.596784 emhass-0.9.1/src/emhass/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    19030 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/img/emhass_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    66736 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/img/emhass_logo_short.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    60319 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/img/feather-sprite.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17332 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/script.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15557 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.596784 emhass-0.9.1/src/emhass/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/templates/template.html
+-rw-r--r--   0 runner    (1001) docker     (127)    47820 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23055 2024-05-13 21:07:58.000000 emhass-0.9.1/src/emhass/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.600784 emhass-0.9.1/src/emhass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    35924 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 21:08:01.000000 emhass-0.9.1/src/emhass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:08:01.600784 emhass-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    30422 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_command_line_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31834 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_machine_learning_forecaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_machine_learning_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_retrieve_hass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15770 2024-05-13 21:07:58.000000 emhass-0.9.1/tests/test_utils.py
```

### Comparing `emhass-0.9.0/CHANGELOG.md` & `emhass-0.9.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 0.9.1 - 2024-05-13
+### Fix
+- Fix patch for issue with paths to modules and inverters database
+- Fixed code formatting, or at least trying to keep a unique format
+
 ## 0.9.0 - 2024-05-10
 ### Improvement
 - On this new version we now have a new method to train a regression model using Scikit-Learn methods. This is the contribution of @gieljnssns. Check the dedicated section the documentation to this new feature: [https://emhass.readthedocs.io/en/latest/mlregressor.html](https://emhass.readthedocs.io/en/latest/mlregressor.html)
 - Again another bunch of nice improvements by @GeoDerp:
   - Added Dictionary var containing EMHASS paths
   - MLForcaster error suppression
   - Add `freq` as runtime parameter
```

### Comparing `emhass-0.9.0/CODE_OF_CONDUCT.md` & `emhass-0.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/CONTRIBUTING.md` & `emhass-0.9.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/LICENSE` & `emhass-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/PKG-INFO` & `emhass-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.9.0
+Version: 0.9.1
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,51 +36,54 @@
 <div align="center">
   <br>
   <img alt="EMHASS" src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/emhass_logo.png" width="300px">
   <h1>Energy Management for Home Assistant</h1>
   <strong></strong>
 </div>
 <br>
+
 <p align="center">
-  <a href="https://github.com/davidusb-geek/emhass/releases">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/releases">
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/davidusb-geek/emhass">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/actions">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/actions">
     <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/davidusb-geek/emhass/python-test.yml?branch=master">
   </a>
-  <a href="https://codecov.io/github/davidusb-geek/emhass" >
+  <a hstyle="text-decoration:none" ref="https://codecov.io/github/davidusb-geek/emhass" >
     <img src="https://codecov.io/github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90"/>
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
     <img alt="GitHub" src="https://img.shields.io/github/license/davidusb-geek/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
-  <a href="https://emhass.readthedocs.io/en/latest/">
+  <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+
 <div align="center">
- <a href="https://emhass.readthedocs.io/en/latest/">
+ <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
   </a>
-   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+   <a style="text-decoration:none" href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/issues">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/issues">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass-add-on">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass-add-on">
      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
   </a>
 </div>
+
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.9.0 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.9.1 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
@@ -14,16 +14,16 @@
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
 skforecast==0.12.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
- _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
-  _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
+ _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_][https://codecov.io/
+  github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
                _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
```

### Comparing `emhass-0.9.0/README.md` & `emhass-0.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 <div align="center">
   <br>
   <img alt="EMHASS" src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/emhass_logo.png" width="300px">
   <h1>Energy Management for Home Assistant</h1>
   <strong></strong>
 </div>
 <br>
+
 <p align="center">
-  <a href="https://github.com/davidusb-geek/emhass/releases">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/releases">
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/davidusb-geek/emhass">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/actions">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/actions">
     <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/davidusb-geek/emhass/python-test.yml?branch=master">
   </a>
-  <a href="https://codecov.io/github/davidusb-geek/emhass" >
+  <a hstyle="text-decoration:none" ref="https://codecov.io/github/davidusb-geek/emhass" >
     <img src="https://codecov.io/github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90"/>
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
     <img alt="GitHub" src="https://img.shields.io/github/license/davidusb-geek/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
-  <a href="https://emhass.readthedocs.io/en/latest/">
+  <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+
 <div align="center">
- <a href="https://emhass.readthedocs.io/en/latest/">
+ <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
   </a>
-   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+   <a style="text-decoration:none" href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/issues">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/issues">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass-add-on">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass-add-on">
      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
   </a>
 </div>
+
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
- _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
-  _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
+ _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_][https://codecov.io/
+  github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
                _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
```

### Comparing `emhass-0.9.0/data/data_load_cost_forecast.csv` & `emhass-0.9.1/data/data_load_cost_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/data_load_forecast.csv` & `emhass-0.9.1/data/data_load_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/data_prod_price_forecast.csv` & `emhass-0.9.1/data/data_prod_price_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/data_train_load_clustering.pkl` & `emhass-0.9.1/data/data_train_load_clustering.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/data_train_load_forecast.pkl` & `emhass-0.9.1/data/data_train_load_forecast.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/data_weather_forecast.csv` & `emhass-0.9.1/data/data_weather_forecast.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/heating_prediction.csv` & `emhass-0.9.1/data/heating_prediction.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/opt_res_latest.csv` & `emhass-0.9.1/data/opt_res_latest.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/opt_res_perfect_optim_cost.csv` & `emhass-0.9.1/data/opt_res_perfect_optim_cost.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/opt_res_perfect_optim_profit.csv` & `emhass-0.9.1/data/opt_res_perfect_optim_profit.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/opt_res_perfect_optim_self-consumption.csv` & `emhass-0.9.1/data/opt_res_perfect_optim_self-consumption.csv`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/test_df_final.pkl` & `emhass-0.9.1/data/test_df_final.pkl`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/test_response_get_data_get_method.pbz2` & `emhass-0.9.1/data/test_response_get_data_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/test_response_scrapper_get_method.pbz2` & `emhass-0.9.1/data/test_response_scrapper_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/test_response_solarforecast_get_method.pbz2` & `emhass-0.9.1/data/test_response_solarforecast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/data/test_response_solcast_get_method.pbz2` & `emhass-0.9.1/data/test_response_solcast_get_method.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/setup.py` & `emhass-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     name='emhass',  # Required
-    version='0.9.0',  # Required
+    version='0.9.1',  # Required
     description='An Energy Management System for Home Assistant',  # Optional
     long_description=long_description,  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/davidusb-geek/emhass',  # Optional
     author='David HERNANDEZ',  # Optional
     author_email='davidusb@gmail.com',  # Optional
     classifiers=[  # Optional
```

### Comparing `emhass-0.9.0/src/emhass/command_line.py` & `emhass-0.9.1/src/emhass/command_line.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 from emhass.forecast import Forecast
 from emhass.machine_learning_forecaster import MLForecaster
 from emhass.optimization import Optimization
 from emhass.machine_learning_regressor import MLRegressor
 from emhass import utils
 
 
-def set_input_data_dict(emhass_conf: dict, costfun: str, 
-    params: str, runtimeparams: str, set_type: str, logger: logging.Logger,
-    get_data_from_file: Optional[bool] = False) -> dict:
+def set_input_data_dict(emhass_conf: dict, costfun: str,
+                        params: str, runtimeparams: str, set_type: str, logger: logging.Logger,
+                        get_data_from_file: Optional[bool] = False) -> dict:
     """
     Set up some of the data needed for the different actions.
-    
+
     :param emhass_conf: Dictionary containing the needed emhass paths
     :type emhass_conf: dict
     :param costfun: The type of cost function to use for optimization problem
     :type costfun: str
     :param params: Configuration parameters passed from data/options.json
     :type params: str
     :param runtimeparams: Runtime optimization parameters passed as a dictionary
@@ -47,173 +47,142 @@
     :return: A dictionnary with multiple data used by the action functions
     :rtype: dict
 
     """
     logger.info("Setting up needed data")
     # Parsing yaml
     retrieve_hass_conf, optim_conf, plant_conf = utils.get_yaml_parse(
-        emhass_conf, use_secrets=not(get_data_from_file), params=params)
+        emhass_conf, use_secrets=not (get_data_from_file), params=params)
     # Treat runtimeparams
     params, retrieve_hass_conf, optim_conf, plant_conf = utils.treat_runtimeparams(
-        runtimeparams,
-        params,
-        retrieve_hass_conf,
-        optim_conf,
-        plant_conf,
-        set_type,
-        logger,
-    )
+        runtimeparams, params, retrieve_hass_conf, optim_conf, plant_conf, set_type, logger)
     # Define main objects
-    rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'], 
-                      retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'], 
+    rh = RetrieveHass(retrieve_hass_conf['hass_url'], retrieve_hass_conf['long_lived_token'],
+                      retrieve_hass_conf['freq'], retrieve_hass_conf['time_zone'],
                       params, emhass_conf, logger, get_data_from_file=get_data_from_file)
     fcst = Forecast(retrieve_hass_conf, optim_conf, plant_conf,
                     params, emhass_conf, logger, get_data_from_file=get_data_from_file)
-    opt = Optimization(retrieve_hass_conf, optim_conf, plant_conf, 
-                       fcst.var_load_cost, fcst.var_prod_price, 
+    opt = Optimization(retrieve_hass_conf, optim_conf, plant_conf,
+                       fcst.var_load_cost, fcst.var_prod_price,
                        costfun, emhass_conf, logger)
     # Perform setup based on type of action
     if set_type == "perfect-optim":
         # Retrieve data from hass
         if get_data_from_file:
             with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
             retrieve_hass_conf['var_load'] = str(var_list[0])
             retrieve_hass_conf['var_PV'] = str(var_list[1])
-            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
-            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
-        else:
-            days_list = utils.get_days_list(retrieve_hass_conf["days_to_retrieve"])
-            var_list = [retrieve_hass_conf["var_load"], retrieve_hass_conf["var_PV"]]
-            if not rh.get_data(
-                days_list,
-                var_list,
-                minimal_response=False,
-                significant_changes_only=False,
-            ):
+            retrieve_hass_conf['var_interp'] = [
+                retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [
+                retrieve_hass_conf['var_PV']]
+        else:
+            days_list = utils.get_days_list(
+                retrieve_hass_conf["days_to_retrieve"])
+            var_list = [retrieve_hass_conf["var_load"],
+                        retrieve_hass_conf["var_PV"]]
+            if not rh.get_data(days_list, var_list, minimal_response=False, significant_changes_only=False):
                 return False
-        if not rh.prepare_data(
-            retrieve_hass_conf["var_load"],
-            load_negative=retrieve_hass_conf["load_negative"],
-            set_zero_min=retrieve_hass_conf["set_zero_min"],
-            var_replace_zero=retrieve_hass_conf["var_replace_zero"],
-            var_interp=retrieve_hass_conf["var_interp"],
-        ):
+        if not rh.prepare_data(retrieve_hass_conf["var_load"],
+                               load_negative=retrieve_hass_conf["load_negative"],
+                               set_zero_min=retrieve_hass_conf["set_zero_min"],
+                               var_replace_zero=retrieve_hass_conf["var_replace_zero"],
+                               var_interp=retrieve_hass_conf["var_interp"]):
             return False
         df_input_data = rh.df_final.copy()
         # What we don't need for this type of action
         P_PV_forecast, P_load_forecast, df_input_data_dayahead = None, None, None
     elif set_type == "dayahead-optim":
         # Get PV and load forecasts
         df_weather = fcst.get_weather_forecast(
-            method=optim_conf["weather_forecast_method"]
-        )
+            method=optim_conf["weather_forecast_method"])
         P_PV_forecast = fcst.get_power_from_weather(df_weather)
-        P_load_forecast = fcst.get_load_forecast(method=optim_conf['load_forecast_method'])
-        if isinstance(P_load_forecast,bool) and not P_load_forecast:
-            logger.error("Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
+        P_load_forecast = fcst.get_load_forecast(
+            method=optim_conf['load_forecast_method'])
+        if isinstance(P_load_forecast, bool) and not P_load_forecast:
+            logger.error(
+                "Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
             return False
-        df_input_data_dayahead = pd.DataFrame(
-            np.transpose(np.vstack([P_PV_forecast.values, P_load_forecast.values])),
-            index=P_PV_forecast.index,
-            columns=["P_PV_forecast", "P_load_forecast"],
-        )
+        df_input_data_dayahead = pd.DataFrame(np.transpose(np.vstack(
+            [P_PV_forecast.values, P_load_forecast.values])), index=P_PV_forecast.index,
+            columns=["P_PV_forecast", "P_load_forecast"])
         df_input_data_dayahead = utils.set_df_index_freq(df_input_data_dayahead)
         params = json.loads(params)
-        if (
-            "prediction_horizon" in params["passed_data"]
-            and params["passed_data"]["prediction_horizon"] is not None
-        ):
+        if ("prediction_horizon" in params["passed_data"] and params["passed_data"]["prediction_horizon"] is not None):
             prediction_horizon = params["passed_data"]["prediction_horizon"]
             df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[
-                df_input_data_dayahead.index[0] : df_input_data_dayahead.index[
-                    prediction_horizon - 1
-                ]
-            ]
+                df_input_data_dayahead.index[0]: df_input_data_dayahead.index[prediction_horizon - 1]]
         # What we don't need for this type of action
         df_input_data, days_list = None, None
     elif set_type == "naive-mpc-optim":
         # Retrieve data from hass
         if get_data_from_file:
             with open(emhass_conf['data_path'] / 'test_df_final.pkl', 'rb') as inp:
                 rh.df_final, days_list, var_list = pickle.load(inp)
             retrieve_hass_conf['var_load'] = str(var_list[0])
             retrieve_hass_conf['var_PV'] = str(var_list[1])
-            retrieve_hass_conf['var_interp'] = [retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
-            retrieve_hass_conf['var_replace_zero'] = [retrieve_hass_conf['var_PV']]
+            retrieve_hass_conf['var_interp'] = [
+                retrieve_hass_conf['var_PV'], retrieve_hass_conf['var_load']]
+            retrieve_hass_conf['var_replace_zero'] = [
+                retrieve_hass_conf['var_PV']]
         else:
             days_list = utils.get_days_list(1)
-            var_list = [retrieve_hass_conf["var_load"], retrieve_hass_conf["var_PV"]]
-            if not rh.get_data(
-                days_list,
-                var_list,
-                minimal_response=False,
-                significant_changes_only=False,
-            ):
+            var_list = [retrieve_hass_conf["var_load"],
+                        retrieve_hass_conf["var_PV"]]
+            if not rh.get_data(days_list, var_list, minimal_response=False, significant_changes_only=False):
                 return False
-        if not rh.prepare_data(
-            retrieve_hass_conf["var_load"],
-            load_negative=retrieve_hass_conf["load_negative"],
-            set_zero_min=retrieve_hass_conf["set_zero_min"],
-            var_replace_zero=retrieve_hass_conf["var_replace_zero"],
-            var_interp=retrieve_hass_conf["var_interp"],
-        ):
+        if not rh.prepare_data(retrieve_hass_conf["var_load"],
+                               load_negative=retrieve_hass_conf["load_negative"],
+                               set_zero_min=retrieve_hass_conf["set_zero_min"],
+                               var_replace_zero=retrieve_hass_conf["var_replace_zero"],
+                               var_interp=retrieve_hass_conf["var_interp"]):
             return False
         df_input_data = rh.df_final.copy()
         # Get PV and load forecasts
-        df_weather = fcst.get_weather_forecast(method=optim_conf['weather_forecast_method'])
-        P_PV_forecast = fcst.get_power_from_weather(df_weather, set_mix_forecast=True, df_now=df_input_data)
-        P_load_forecast = fcst.get_load_forecast(method=optim_conf['load_forecast_method'], set_mix_forecast=True, df_now=df_input_data)
-        if isinstance(P_load_forecast,bool) and not P_load_forecast:
-            logger.error("Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
+        df_weather = fcst.get_weather_forecast(
+            method=optim_conf['weather_forecast_method'])
+        P_PV_forecast = fcst.get_power_from_weather(
+            df_weather, set_mix_forecast=True, df_now=df_input_data)
+        P_load_forecast = fcst.get_load_forecast(
+            method=optim_conf['load_forecast_method'], set_mix_forecast=True, df_now=df_input_data)
+        if isinstance(P_load_forecast, bool) and not P_load_forecast:
+            logger.error(
+                "Unable to get sensor power photovoltaics, or sensor power load no var loads. Check HA sensors and their daily data")
             return False
         df_input_data_dayahead = pd.concat([P_PV_forecast, P_load_forecast], axis=1)
         df_input_data_dayahead = utils.set_df_index_freq(df_input_data_dayahead)
         df_input_data_dayahead.columns = ["P_PV_forecast", "P_load_forecast"]
         params = json.loads(params)
-        if (
-            "prediction_horizon" in params["passed_data"]
-            and params["passed_data"]["prediction_horizon"] is not None
-        ):
+        if ("prediction_horizon" in params["passed_data"] and params["passed_data"]["prediction_horizon"] is not None):
             prediction_horizon = params["passed_data"]["prediction_horizon"]
             df_input_data_dayahead = copy.deepcopy(df_input_data_dayahead)[
-                df_input_data_dayahead.index[0] : df_input_data_dayahead.index[
-                    prediction_horizon - 1
-                ]
-            ]
-    elif (
-        set_type == "forecast-model-fit"
-        or set_type == "forecast-model-predict"
-        or set_type == "forecast-model-tune"
-    ):
+                df_input_data_dayahead.index[0]: df_input_data_dayahead.index[prediction_horizon - 1]]
+    elif (set_type == "forecast-model-fit" or set_type == "forecast-model-predict" or set_type == "forecast-model-tune"):
         df_input_data_dayahead = None
         P_PV_forecast, P_load_forecast = None, None
         params = json.loads(params)
         # Retrieve data from hass
         days_to_retrieve = params["passed_data"]["days_to_retrieve"]
         model_type = params["passed_data"]["model_type"]
         var_model = params["passed_data"]["var_model"]
         if get_data_from_file:
             days_list = None
             filename = 'data_train_'+model_type+'.pkl'
             filename_path = emhass_conf['data_path'] / filename
             with open(filename_path, 'rb') as inp:
                 df_input_data, _ = pickle.load(inp)
-            df_input_data = df_input_data[
-                df_input_data.index[-1] - pd.offsets.Day(days_to_retrieve) :
-            ]
+            df_input_data = df_input_data[df_input_data.index[-1] - pd.offsets.Day(days_to_retrieve):]
         else:
             days_list = utils.get_days_list(days_to_retrieve)
             var_list = [var_model]
             if not rh.get_data(days_list, var_list):
                 return False
             df_input_data = rh.df_final.copy()
-
     elif set_type == "regressor-model-fit" or set_type == "regressor-model-predict":
-
         df_input_data, df_input_data_dayahead = None, None
         P_PV_forecast, P_load_forecast = None, None
         params = json.loads(params)
         days_list = None
         csv_file = params["passed_data"].get("csv_file", None)
         if "features" in params["passed_data"]:
             features = params["passed_data"]["features"]
@@ -221,52 +190,45 @@
             target = params["passed_data"]["target"]
         if "timestamp" in params["passed_data"]:
             timestamp = params["passed_data"]["timestamp"]
         if csv_file:
             if get_data_from_file:
                 base_path = emhass_conf["data_path"]  # + "/data"
                 filename_path = pathlib.Path(base_path) / csv_file
-
             else:
                 filename_path = emhass_conf["data_path"] / csv_file
-
             if filename_path.is_file():
                 df_input_data = pd.read_csv(filename_path, parse_dates=True)
-
             else:
-                logger.error("The CSV file " + csv_file + " was not found in path: " + str(emhass_conf["data_path"]))
+                logger.error("The CSV file " + csv_file +
+                             " was not found in path: " + str(emhass_conf["data_path"]))
                 return False
-                #raise ValueError("The CSV file " + csv_file + " was not found.")
+                # raise ValueError("The CSV file " + csv_file + " was not found.")
             required_columns = []
             required_columns.extend(features)
             required_columns.append(target)
             if timestamp is not None:
                 required_columns.append(timestamp)
-
             if not set(required_columns).issubset(df_input_data.columns):
-                logger.error("The cvs file does not contain the required columns.")
+                logger.error(
+                    "The cvs file does not contain the required columns.")
                 msg = f"CSV file should contain the following columns: {', '.join(required_columns)}"
                 logger.error(msg)
                 return False
-                #raise ValueError(
-                #    msg,
-                #)
-
     elif set_type == "publish-data":
         df_input_data, df_input_data_dayahead = None, None
         P_PV_forecast, P_load_forecast = None, None
         days_list = None
     else:
         logger.error(
             "The passed action argument and hence the set_type parameter for setup is not valid",
         )
         df_input_data, df_input_data_dayahead = None, None
         P_PV_forecast, P_load_forecast = None, None
         days_list = None
-
     # The input data dictionary to return
     input_data_dict = {
         'emhass_conf': emhass_conf,
         'retrieve_hass_conf': retrieve_hass_conf,
         'rh': rh,
         'opt': opt,
         'fcst': fcst,
@@ -277,20 +239,17 @@
         'costfun': costfun,
         'params': params,
         'days_list': days_list
     }
     return input_data_dict
 
 
-def perfect_forecast_optim(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    save_data_to_file: Optional[bool] = True,
-    debug: Optional[bool] = False,
-) -> pd.DataFrame:
+def perfect_forecast_optim(input_data_dict: dict, logger: logging.Logger,
+                           save_data_to_file: Optional[bool] = True, 
+                           debug: Optional[bool] = False) -> pd.DataFrame:
     """
     Perform a call to the perfect forecast optimization routine.
 
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
@@ -301,41 +260,41 @@
     :return: The output data of the optimization
     :rtype: pd.DataFrame
 
     """
     logger.info("Performing perfect forecast optimization")
     # Load cost and prod price forecast
     df_input_data = input_data_dict['fcst'].get_load_cost_forecast(
-        input_data_dict['df_input_data'], 
+        input_data_dict['df_input_data'],
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'],
         list_and_perfect=True)
-    if isinstance(df_input_data,bool) and not df_input_data:
+    if isinstance(df_input_data, bool) and not df_input_data:
         return False
     df_input_data = input_data_dict['fcst'].get_prod_price_forecast(
         df_input_data, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'],
         list_and_perfect=True)
-    if isinstance(df_input_data,bool) and not df_input_data:
-        return False 
-    opt_res = input_data_dict['opt'].perform_perfect_forecast_optim(df_input_data, input_data_dict['days_list'])
+    if isinstance(df_input_data, bool) and not df_input_data:
+        return False
+    opt_res = input_data_dict['opt'].perform_perfect_forecast_optim(
+        df_input_data, input_data_dict['days_list'])
     # Save CSV file for analysis
     if save_data_to_file:
-        filename = "opt_res_perfect_optim_" + input_data_dict["costfun"] + ".csv"
+        filename = "opt_res_perfect_optim_" + \
+            input_data_dict["costfun"] + ".csv"
     else:  # Just save the latest optimization results
         filename = "opt_res_latest.csv"
     if not debug:
-        opt_res.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
+        opt_res.to_csv(
+            input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res
 
 
-def dayahead_forecast_optim(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False,
-    debug: Optional[bool] = False,
-) -> pd.DataFrame:
+def dayahead_forecast_optim(input_data_dict: dict, logger: logging.Logger, 
+                            save_data_to_file: Optional[bool] = False, 
+                            debug: Optional[bool] = False) -> pd.DataFrame:
     """
     Perform a call to the day-ahead optimization routine.
 
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
@@ -348,42 +307,40 @@
 
     """
     logger.info("Performing day-ahead forecast optimization")
     # Load cost and prod price forecast
     df_input_data_dayahead = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data_dayahead'],
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'])
-    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
-        return False 
+    if isinstance(df_input_data_dayahead, bool) and not df_input_data_dayahead:
+        return False
     df_input_data_dayahead = input_data_dict['fcst'].get_prod_price_forecast(
-        df_input_data_dayahead, 
+        df_input_data_dayahead,
         method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'])
-    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
-        return False 
+    if isinstance(df_input_data_dayahead, bool) and not df_input_data_dayahead:
+        return False
     opt_res_dayahead = input_data_dict['opt'].perform_dayahead_forecast_optim(
         df_input_data_dayahead, input_data_dict['P_PV_forecast'], input_data_dict['P_load_forecast'])
     # Save CSV file for publish_data
     if save_data_to_file:
         today = datetime.now(timezone.utc).replace(
             hour=0, minute=0, second=0, microsecond=0
         )
         filename = "opt_res_dayahead_" + today.strftime("%Y_%m_%d") + ".csv"
     else:  # Just save the latest optimization results
         filename = "opt_res_latest.csv"
     if not debug:
-        opt_res_dayahead.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
+        opt_res_dayahead.to_csv(
+            input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res_dayahead
 
 
-def naive_mpc_optim(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False,
-    debug: Optional[bool] = False,
-) -> pd.DataFrame:
+def naive_mpc_optim(input_data_dict: dict, logger: logging.Logger, 
+                    save_data_to_file: Optional[bool] = False, 
+                    debug: Optional[bool] = False) -> pd.DataFrame:
     """
     Perform a call to the naive Model Predictive Controller optimization routine.
 
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
@@ -396,54 +353,47 @@
 
     """
     logger.info("Performing naive MPC optimization")
     # Load cost and prod price forecast
     df_input_data_dayahead = input_data_dict['fcst'].get_load_cost_forecast(
         input_data_dict['df_input_data_dayahead'],
         method=input_data_dict['fcst'].optim_conf['load_cost_forecast_method'])
-    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
-        return False 
+    if isinstance(df_input_data_dayahead, bool) and not df_input_data_dayahead:
+        return False
     df_input_data_dayahead = input_data_dict['fcst'].get_prod_price_forecast(
         df_input_data_dayahead, method=input_data_dict['fcst'].optim_conf['prod_price_forecast_method'])
-    if isinstance(df_input_data_dayahead,bool) and not df_input_data_dayahead:
-        return False 
+    if isinstance(df_input_data_dayahead, bool) and not df_input_data_dayahead:
+        return False
     # The specifics params for the MPC at runtime
     prediction_horizon = input_data_dict["params"]["passed_data"]["prediction_horizon"]
     soc_init = input_data_dict["params"]["passed_data"]["soc_init"]
     soc_final = input_data_dict["params"]["passed_data"]["soc_final"]
     def_total_hours = input_data_dict["params"]["passed_data"]["def_total_hours"]
     def_start_timestep = input_data_dict["params"]["passed_data"]["def_start_timestep"]
     def_end_timestep = input_data_dict["params"]["passed_data"]["def_end_timestep"]
     opt_res_naive_mpc = input_data_dict["opt"].perform_naive_mpc_optim(
-        df_input_data_dayahead,
-        input_data_dict["P_PV_forecast"],
-        input_data_dict["P_load_forecast"],
-        prediction_horizon,
-        soc_init,
-        soc_final,
-        def_total_hours,
-        def_start_timestep,
-        def_end_timestep,
-    )
+        df_input_data_dayahead, input_data_dict["P_PV_forecast"], input_data_dict["P_load_forecast"],
+        prediction_horizon, soc_init, soc_final, def_total_hours,
+        def_start_timestep, def_end_timestep)
     # Save CSV file for publish_data
     if save_data_to_file:
         today = datetime.now(timezone.utc).replace(
             hour=0, minute=0, second=0, microsecond=0
         )
         filename = "opt_res_naive_mpc_" + today.strftime("%Y_%m_%d") + ".csv"
     else:  # Just save the latest optimization results
         filename = "opt_res_latest.csv"
     if not debug:
-        opt_res_naive_mpc.to_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
+        opt_res_naive_mpc.to_csv(
+            input_data_dict['emhass_conf']['data_path'] / filename, index_label='timestamp')
     return opt_res_naive_mpc
 
 
-def forecast_model_fit(
-    input_data_dict: dict, logger: logging.Logger, debug: Optional[bool] = False
-) -> Tuple[pd.DataFrame, pd.DataFrame, MLForecaster]:
+def forecast_model_fit(input_data_dict: dict, logger: logging.Logger, 
+                       debug: Optional[bool] = False) -> Tuple[pd.DataFrame, pd.DataFrame, MLForecaster]:
     """Perform a forecast model fit from training data retrieved from Home Assistant.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
@@ -455,35 +405,33 @@
     model_type = input_data_dict['params']['passed_data']['model_type']
     var_model = input_data_dict['params']['passed_data']['var_model']
     sklearn_model = input_data_dict['params']['passed_data']['sklearn_model']
     num_lags = input_data_dict['params']['passed_data']['num_lags']
     split_date_delta = input_data_dict['params']['passed_data']['split_date_delta']
     perform_backtest = input_data_dict['params']['passed_data']['perform_backtest']
     # The ML forecaster object
-    mlf = MLForecaster(data, model_type, var_model, sklearn_model, num_lags, input_data_dict['emhass_conf'], logger)
+    mlf = MLForecaster(data, model_type, var_model, sklearn_model,
+                       num_lags, input_data_dict['emhass_conf'], logger)
     # Fit the ML model
     df_pred, df_pred_backtest = mlf.fit(
         split_date_delta=split_date_delta, perform_backtest=perform_backtest
     )
     # Save model
     if not debug:
         filename = model_type+'_mlf.pkl'
         filename_path = input_data_dict['emhass_conf']['data_path'] / filename
         with open(filename_path, 'wb') as outp:
             pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)
     return df_pred, df_pred_backtest, mlf
 
 
-def forecast_model_predict(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    use_last_window: Optional[bool] = True,
-    debug: Optional[bool] = False,
-    mlf: Optional[MLForecaster] = None,
-) -> pd.DataFrame:
+def forecast_model_predict(input_data_dict: dict, logger: logging.Logger, 
+                           use_last_window: Optional[bool] = True, 
+                           debug: Optional[bool] = False, mlf: Optional[MLForecaster] = None
+                           ) -> pd.DataFrame:
     r"""Perform a forecast model predict using a previously trained skforecast model.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param use_last_window: True if the 'last_window' option should be used for the \
@@ -535,48 +483,32 @@
     publish_prefix = input_data_dict["params"]["passed_data"]["publish_prefix"]
     if model_predict_publish is True:
         # Estimate the current index
         now_precise = datetime.now(
             input_data_dict["retrieve_hass_conf"]["time_zone"]
         ).replace(second=0, microsecond=0)
         if input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "nearest":
-            idx_closest = predictions.index.get_indexer(
-                [now_precise], method="nearest"
-            )[0]
+            idx_closest = predictions.index.get_indexer([now_precise], method="nearest")[0]
         elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "first":
-            idx_closest = predictions.index.get_indexer([now_precise], method="ffill")[
-                0
-            ]
+            idx_closest = predictions.index.get_indexer([now_precise], method="ffill")[0]
         elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "last":
-            idx_closest = predictions.index.get_indexer([now_precise], method="bfill")[
-                0
-            ]
+            idx_closest = predictions.index.get_indexer([now_precise], method="bfill")[0]
         if idx_closest == -1:
-            idx_closest = predictions.index.get_indexer(
-                [now_precise], method="nearest"
-            )[0]
+            idx_closest = predictions.index.get_indexer([now_precise], method="nearest")[0]
         # Publish Load forecast
         input_data_dict["rh"].post_data(
-            predictions,
-            idx_closest,
-            model_predict_entity_id,
-            model_predict_unit_of_measurement,
-            model_predict_friendly_name,
-            type_var="mlforecaster",
-            publish_prefix=publish_prefix,
-        )
+            predictions, idx_closest, model_predict_entity_id,
+            model_predict_unit_of_measurement, model_predict_friendly_name,
+            type_var="mlforecaster", publish_prefix=publish_prefix)
     return predictions
 
 
-def forecast_model_tune(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    debug: Optional[bool] = False,
-    mlf: Optional[MLForecaster] = None,
-) -> Tuple[pd.DataFrame, MLForecaster]:
+def forecast_model_tune(input_data_dict: dict, logger: logging.Logger, 
+                        debug: Optional[bool] = False, mlf: Optional[MLForecaster] = None
+                        ) -> Tuple[pd.DataFrame, MLForecaster]:
     """Tune a forecast model hyperparameters using bayesian optimization.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
@@ -603,23 +535,20 @@
     # Tune the model
     df_pred_optim = mlf.tune(debug=debug)
     # Save model
     if not debug:
         filename = model_type+'_mlf.pkl'
         filename_path = input_data_dict['emhass_conf']['data_path'] / filename
         with open(filename_path, 'wb') as outp:
-            pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)       
+            pickle.dump(mlf, outp, pickle.HIGHEST_PROTOCOL)
     return df_pred_optim, mlf
 
 
-def regressor_model_fit(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    debug: Optional[bool] = False,
-) -> None:
+def regressor_model_fit(input_data_dict: dict, logger: logging.Logger, 
+                        debug: Optional[bool] = False) -> MLRegressor:
     """Perform a forecast model fit from training data retrieved from Home Assistant.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
@@ -636,114 +565,96 @@
     else:
         logger.error("parameter: 'regression_model' not passed")
         return False
     if "features" in input_data_dict["params"]["passed_data"]:
         features = input_data_dict["params"]["passed_data"]["features"]
     else:
         logger.error("parameter: 'features' not passed")
-        return False    
+        return False
     if "target" in input_data_dict["params"]["passed_data"]:
         target = input_data_dict["params"]["passed_data"]["target"]
     else:
         logger.error("parameter: 'target' not passed")
-        return False        
+        return False
     if "timestamp" in input_data_dict["params"]["passed_data"]:
         timestamp = input_data_dict["params"]["passed_data"]["timestamp"]
     else:
         logger.error("parameter: 'timestamp' not passed")
-        return False       
+        return False
     if "date_features" in input_data_dict["params"]["passed_data"]:
         date_features = input_data_dict["params"]["passed_data"]["date_features"]
     else:
         logger.error("parameter: 'date_features' not passed")
-        return False           
-
+        return False
     # The MLRegressor object
-    mlr = MLRegressor(
-        data,
-        model_type,
-        regression_model,
-        features,
-        target,
-        timestamp,
-        logger,
-    )
+    mlr = MLRegressor(data, model_type, regression_model, features, target, timestamp, logger)
     # Fit the ML model
     mlr.fit(date_features=date_features)
     # Save model
     if not debug:
         filename = model_type + "_mlr.pkl"
         filename_path = input_data_dict["emhass_conf"]["data_path"] / filename
         with open(filename_path, "wb") as outp:
             pickle.dump(mlr, outp, pickle.HIGHEST_PROTOCOL)
     return mlr
 
 
-def regressor_model_predict(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    debug: Optional[bool] = False,
-    mlr: Optional[MLRegressor] = None,
-) -> None:
+def regressor_model_predict(input_data_dict: dict, logger: logging.Logger, 
+                            debug: Optional[bool] = False, mlr: Optional[MLRegressor] = None
+                            ) -> np.ndarray:
     """Perform a prediction from csv file.
 
     :param input_data_dict: A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging.Logger
     :param debug: True to debug, useful for unit testing, defaults to False
     :type debug: Optional[bool], optional
     """
     if "model_type" in input_data_dict["params"]["passed_data"]:
         model_type = input_data_dict["params"]["passed_data"]["model_type"]
     else:
         logger.error("parameter: 'model_type' not passed")
-        return False   
+        return False
     filename = model_type + "_mlr.pkl"
     filename_path = input_data_dict["emhass_conf"]["data_path"] / filename
     if not debug:
         if filename_path.is_file():
             with open(filename_path, "rb") as inp:
                 mlr = pickle.load(inp)
         else:
             logger.error(
                 "The ML forecaster file was not found, please run a model fit method before this predict method",
             )
             return False
-    if "new_values" in input_data_dict["params"]["passed_data"]:    
+    if "new_values" in input_data_dict["params"]["passed_data"]:
         new_values = input_data_dict["params"]["passed_data"]["new_values"]
     else:
         logger.error("parameter: 'new_values' not passed")
-        return False         
+        return False
     # Predict from csv file
     prediction = mlr.predict(new_values)
-    
-    mlr_predict_entity_id = input_data_dict["params"]["passed_data"].get("mlr_predict_entity_id","sensor.mlr_predict")
-    mlr_predict_unit_of_measurement = input_data_dict["params"]["passed_data"].get("mlr_predict_unit_of_measurement","h")
-    mlr_predict_friendly_name = input_data_dict["params"]["passed_data"].get("mlr_predict_friendly_name","mlr predictor")
+    mlr_predict_entity_id = input_data_dict["params"]["passed_data"].get(
+        "mlr_predict_entity_id", "sensor.mlr_predict")
+    mlr_predict_unit_of_measurement = input_data_dict["params"]["passed_data"].get(
+        "mlr_predict_unit_of_measurement", "h")
+    mlr_predict_friendly_name = input_data_dict["params"]["passed_data"].get(
+        "mlr_predict_friendly_name", "mlr predictor")
     # Publish prediction
     idx = 0
     if not debug:
-        input_data_dict["rh"].post_data(
-            prediction,
-            idx,
-            mlr_predict_entity_id,
-            mlr_predict_unit_of_measurement,
-            mlr_predict_friendly_name,
-            type_var="mlregressor",
-        )
+        input_data_dict["rh"].post_data(prediction, idx, mlr_predict_entity_id,
+            mlr_predict_unit_of_measurement, mlr_predict_friendly_name,
+            type_var="mlregressor")
     return prediction
 
 
-def publish_data(
-    input_data_dict: dict,
-    logger: logging.Logger,
-    save_data_to_file: Optional[bool] = False,
-    opt_res_latest: Optional[pd.DataFrame] = None,
-) -> pd.DataFrame:
+def publish_data(input_data_dict: dict, logger: logging.Logger, 
+                 save_data_to_file: Optional[bool] = False, 
+                 opt_res_latest: Optional[pd.DataFrame] = None) -> pd.DataFrame:
     """
     Publish the data obtained from the optimization results.
 
     :param input_data_dict:  A dictionnary with multiple data used by the action functions
     :type input_data_dict: dict
     :param logger: The passed logger object
     :type logger: logging object
@@ -760,36 +671,36 @@
             hour=0, minute=0, second=0, microsecond=0
         )
         filename = "opt_res_dayahead_" + today.strftime("%Y_%m_%d") + ".csv"
     else:
         filename = "opt_res_latest.csv"
     if opt_res_latest is None:
         if not os.path.isfile(input_data_dict['emhass_conf']['data_path'] / filename):
-            logger.error("File not found error, run an optimization task first.")
+            logger.error(
+                "File not found error, run an optimization task first.")
             return
         else:
-            opt_res_latest = pd.read_csv(input_data_dict['emhass_conf']['data_path'] / filename, index_col='timestamp')
+            opt_res_latest = pd.read_csv(
+                input_data_dict['emhass_conf']['data_path'] / filename, index_col='timestamp')
             opt_res_latest.index = pd.to_datetime(opt_res_latest.index)
             opt_res_latest.index.freq = input_data_dict["retrieve_hass_conf"]["freq"]
     # Estimate the current index
     now_precise = datetime.now(
         input_data_dict["retrieve_hass_conf"]["time_zone"]
     ).replace(second=0, microsecond=0)
     if input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "nearest":
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[
-            0
-        ]
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[0]
     elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "first":
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="ffill")[0]
+        idx_closest = opt_res_latest.index.get_indexer(
+            [now_precise], method="ffill")[0]
     elif input_data_dict["retrieve_hass_conf"]["method_ts_round"] == "last":
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="bfill")[0]
+        idx_closest = opt_res_latest.index.get_indexer(
+            [now_precise], method="bfill")[0]
     if idx_closest == -1:
-        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[
-            0
-        ]
+        idx_closest = opt_res_latest.index.get_indexer([now_precise], method="nearest")[0]
     # Publish the data
     params = json.loads(input_data_dict["params"])
     publish_prefix = params["passed_data"]["publish_prefix"]
     # Publish PV forecast
     custom_pv_forecast_id = params["passed_data"]["custom_pv_forecast_id"]
     input_data_dict["rh"].post_data(
         opt_res_latest["P_PV"],
@@ -926,15 +837,16 @@
         custom_unit_prod_price_id["unit_of_measurement"],
         custom_unit_prod_price_id["friendly_name"],
         type_var="unit_prod_price",
         publish_prefix=publish_prefix,
     )
     cols_published = cols_published + ["unit_prod_price"]
     # Create a DF resuming what has been published
-    opt_res = opt_res_latest[cols_published].loc[[opt_res_latest.index[idx_closest]]]
+    opt_res = opt_res_latest[cols_published].loc[[
+        opt_res_latest.index[idx_closest]]]
     return opt_res
 
 
 def main():
     r"""Define the main command line entry function.
 
     This function may take several arguments as inputs. You can type `emhass --help` to see the list of options:
@@ -955,127 +867,120 @@
     - debug: Use True for testing purposes
 
     """
     # Parsing arguments
     parser = argparse.ArgumentParser()
     parser.add_argument('--action', type=str, help='Set the desired action, options are: perfect-optim, dayahead-optim,\
         naive-mpc-optim, publish-data, forecast-model-fit, forecast-model-predict, forecast-model-tune')
-    parser.add_argument('--config', type=str, help='Define path to the config.yaml file')
-    parser.add_argument('--data', type=str, help='Define path to the Data files (.csv & .pkl)')
+    parser.add_argument('--config', type=str,
+                        help='Define path to the config.yaml file')
+    parser.add_argument('--data', type=str,
+                        help='Define path to the Data files (.csv & .pkl)')
     parser.add_argument('--root', type=str, help='Define path emhass root')
-    parser.add_argument('--costfun', type=str, default='profit', help='Define the type of cost function, options are: profit, cost, self-consumption')
-    parser.add_argument('--log2file', type=strtobool, default='False', help='Define if we should log to a file or not')
-    parser.add_argument('--params', type=str, default=None, help='Configuration parameters passed from data/options.json')
-    parser.add_argument('--runtimeparams', type=str, default=None, help='Pass runtime optimization parameters as dictionnary')
-    parser.add_argument('--debug', type=strtobool, default='False', help='Use True for testing purposes')
+    parser.add_argument('--costfun', type=str, default='profit',
+                        help='Define the type of cost function, options are: profit, cost, self-consumption')
+    parser.add_argument('--log2file', type=strtobool, default='False',
+                        help='Define if we should log to a file or not')
+    parser.add_argument('--params', type=str, default=None,
+                        help='Configuration parameters passed from data/options.json')
+    parser.add_argument('--runtimeparams', type=str, default=None,
+                        help='Pass runtime optimization parameters as dictionnary')
+    parser.add_argument('--debug', type=strtobool,
+                        default='False', help='Use True for testing purposes')
     args = parser.parse_args()
     # The path to the configuration files
-    
     if args.config is not None:
         config_path = pathlib.Path(args.config)
     else:
-        config_path = pathlib.Path(str(utils.get_root(__file__, num_parent=2) / 'config_emhass.yaml' ))
-
+        config_path = pathlib.Path(
+            str(utils.get_root(__file__, num_parent=2) / 'config_emhass.yaml'))
     if args.data is not None:
         data_path = pathlib.Path(args.data)
     else:
         data_path = (config_path.parent / 'data/')
-
     if args.root is not None:
         root_path = pathlib.Path(args.root)
     else:
         root_path = config_path.parent
-    
     emhass_conf = {}
     emhass_conf['config_path'] = config_path
     emhass_conf['data_path'] = data_path
     emhass_conf['root_path'] = root_path
     # create logger
-    logger, ch = utils.get_logger(__name__, emhass_conf, save_to_file=bool(args.log2file))
-    
+    logger, ch = utils.get_logger(
+        __name__, emhass_conf, save_to_file=bool(args.log2file))
     logger.debug("config path: " + str(config_path))
     logger.debug("data path: " + str(data_path))
     logger.debug("root path: " + str(root_path))
-
-
     if not config_path.exists():
-        logger.error("Could not find config_emhass.yaml file in: " + str(config_path))
-        logger.error("Try setting config file path with --config" )
+        logger.error(
+            "Could not find config_emhass.yaml file in: " + str(config_path))
+        logger.error("Try setting config file path with --config")
         return False
-
     if not os.path.isdir(data_path):
         logger.error("Could not find data foulder in: " + str(data_path))
-        logger.error("Try setting data path with --data" )
+        logger.error("Try setting data path with --data")
         return False
-
     if not os.path.isdir(root_path / 'src'):
         logger.error("Could not find emhass/src foulder in: " + str(root_path))
-        logger.error("Try setting emhass root path with --root" )
+        logger.error("Try setting emhass root path with --root")
         return False
-
     # Additionnal argument
     try:
         parser.add_argument(
             "--version",
             action="version",
             version="%(prog)s " + version("emhass"),
         )
         args = parser.parse_args()
     except Exception:
         logger.info(
             "Version not found for emhass package. Or importlib exited with PackageNotFoundError.",
         )
     # Setup parameters
-    input_data_dict = set_input_data_dict(emhass_conf, 
-                                          args.costfun, args.params, args.runtimeparams, args.action, 
+    input_data_dict = set_input_data_dict(emhass_conf,
+                                          args.costfun, args.params, args.runtimeparams, args.action,
                                           logger, args.debug)
     # Perform selected action
     if args.action == "perfect-optim":
-        opt_res = perfect_forecast_optim(input_data_dict, logger, debug=args.debug)
+        opt_res = perfect_forecast_optim(
+            input_data_dict, logger, debug=args.debug)
     elif args.action == "dayahead-optim":
-        opt_res = dayahead_forecast_optim(input_data_dict, logger, debug=args.debug)
+        opt_res = dayahead_forecast_optim(
+            input_data_dict, logger, debug=args.debug)
     elif args.action == "naive-mpc-optim":
         opt_res = naive_mpc_optim(input_data_dict, logger, debug=args.debug)
     elif args.action == "forecast-model-fit":
         df_fit_pred, df_fit_pred_backtest, mlf = forecast_model_fit(
             input_data_dict, logger, debug=args.debug
         )
         opt_res = None
     elif args.action == "forecast-model-predict":
         if args.debug:
             _, _, mlf = forecast_model_fit(input_data_dict, logger, debug=args.debug)
         else:
             mlf = None
-        df_pred = forecast_model_predict(
-            input_data_dict, logger, debug=args.debug, mlf=mlf
-        )
+        df_pred = forecast_model_predict(input_data_dict, logger, debug=args.debug, mlf=mlf)
         opt_res = None
     elif args.action == "forecast-model-tune":
         if args.debug:
             _, _, mlf = forecast_model_fit(input_data_dict, logger, debug=args.debug)
         else:
             mlf = None
-        df_pred_optim, mlf = forecast_model_tune(
-            input_data_dict, logger, debug=args.debug, mlf=mlf
-        )
+        df_pred_optim, mlf = forecast_model_tune(input_data_dict, logger, debug=args.debug, mlf=mlf)
         opt_res = None
     elif args.action == "regressor-model-fit":
         mlr = regressor_model_fit(input_data_dict, logger, debug=args.debug)
         opt_res = None
     elif args.action == "regressor-model-predict":
         if args.debug:
             mlr = regressor_model_fit(input_data_dict, logger, debug=args.debug)
         else:
             mlr = None
-        prediction = regressor_model_predict(
-            input_data_dict,
-            logger,
-            debug=args.debug,
-            mlr=mlr,
-        )
+        prediction = regressor_model_predict(input_data_dict, logger, debug=args.debug,mlr=mlr)
         opt_res = None
     elif args.action == "publish-data":
         opt_res = publish_data(input_data_dict, logger)
     else:
         logger.error("The passed action argument is not valid")
         logger.error("Try setting --action: perfect-optim, dayahead-optim, naive-mpc-optim, forecast-model-fit, forecast-model-predict, forecast-model-tune or publish-data")
         opt_res = None
@@ -1096,13 +1001,13 @@
         return df_pred
     elif args.action == "regressor-model-fit":
         return mlr
     elif args.action == "regressor-model-predict":
         return prediction
     elif args.action == "forecast-model-tune":
         return df_pred_optim, mlf
-    else: 
+    else:
         return opt_res
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `emhass-0.9.0/src/emhass/data/cec_inverters.pbz2` & `emhass-0.9.1/src/emhass/data/cec_inverters.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/data/cec_modules.pbz2` & `emhass-0.9.1/src/emhass/data/cec_modules.pbz2`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/forecast.py` & `emhass-0.9.1/src/emhass/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,17 +413,17 @@
                 P_PV_forecast = df_weather['yhat']
                 P_PV_forecast.name = None
             else: # We will transform the weather data into electrical power
                 # Transform to power (Watts)
                 # Setting the main parameters of the PV plant
                 location = Location(latitude=self.lat, longitude=self.lon)
                 temp_params = TEMPERATURE_MODEL_PARAMETERS['sapm']['close_mount_glass_glass']
-                cec_modules = bz2.BZ2File(self.emhass_conf['root_path'] / 'src/emhass/data/cec_modules.pbz2', "rb")
+                cec_modules =  bz2.BZ2File(pathlib.Path(__file__).parent / 'data/cec_modules.pbz2', "rb")
                 cec_modules = cPickle.load(cec_modules)
-                cec_inverters = bz2.BZ2File(self.emhass_conf['root_path'] / 'src/emhass/data/cec_inverters.pbz2', "rb")
+                cec_inverters = bz2.BZ2File(pathlib.Path(__file__).parent / 'data/cec_inverters.pbz2', "rb")
                 cec_inverters = cPickle.load(cec_inverters)
                 if type(self.plant_conf['module_model']) == list:
                     P_PV_forecast = pd.Series(0, index=df_weather.index)
                     for i in range(len(self.plant_conf['module_model'])):
                         # Selecting correct module and inverter
                         module = cec_modules[self.plant_conf['module_model'][i]]
                         inverter = cec_inverters[self.plant_conf['inverter_model'][i]]
@@ -635,18 +635,18 @@
                     var_interp = [var_list[0]]
                     self.var_list = [var_list[0]]
                     self.var_load_new = self.var_load+'_positive'
             else:
                 days_list = get_days_list(days_min_load_forecast) 
                 if not rh.get_data(days_list, var_list):
                     return False
-            if  not rh.prepare_data(self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
-                            set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
-                            var_replace_zero = var_replace_zero, 
-                            var_interp = var_interp):
+            if  not rh.prepare_data(
+                self.retrieve_hass_conf['var_load'], load_negative = self.retrieve_hass_conf['load_negative'],
+                set_zero_min = self.retrieve_hass_conf['set_zero_min'], 
+                var_replace_zero = var_replace_zero, var_interp = var_interp):
                 return False
             df = rh.df_final.copy()[[self.var_load_new]]
         if method == 'naive': # using a naive approach
             mask_forecast_out = (df.index > days_list[-1] - self.optim_conf['delta_forecast'])
             forecast_out = df.copy().loc[mask_forecast_out]
             forecast_out = forecast_out.rename(columns={self.var_load_new: 'yhat'})
             # Force forecast_out length to avoid mismatches
@@ -743,15 +743,14 @@
         :type csv_path: str, optional
         :return: The input DataFrame with one additionnal column appended containing
             the load cost for each time observation.
         :rtype: pd.DataFrame
 
         """
         csv_path  = self.emhass_conf['data_path'] / csv_path
-
         if method == 'hp_hc_periods':
             df_final[self.var_load_cost] = self.optim_conf['load_cost_hc']
             list_df_hp = []
             for key, period_hp in self.optim_conf['list_hp_periods'].items():
                 list_df_hp.append(df_final[self.var_load_cost].between_time(
                     period_hp[0]['start'], period_hp[1]['end']))
             for df_hp in list_df_hp:
@@ -776,20 +775,19 @@
                 forecast_out = self.get_forecast_out_from_csv_or_list(
                     df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_load_cost] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
             return False
-            
         return df_final
     
     def get_prod_price_forecast(self, df_final: pd.DataFrame, method: Optional[str] = 'constant',
-                               csv_path: Optional[str] = "data_prod_price_forecast.csv", 
-                               list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
+                                csv_path: Optional[str] = "data_prod_price_forecast.csv", 
+                                list_and_perfect: Optional[bool] = False) -> pd.DataFrame:
 
         r"""
         Get the unit power production price for the energy injected to the grid.\
         This is the price of the energy injected to the utility in a vector \
         sampled at the fixed freq value.
         
         :param df_input_data: The DataFrame containing all the input data retrieved
@@ -803,24 +801,21 @@
             defaults to "/data/data_load_cost_forecast.csv"
         :type csv_path: str, optional
         :return: The input DataFrame with one additionnal column appended containing
             the power production price for each time observation.
         :rtype: pd.DataFrame
 
         """
-
         csv_path  = self.emhass_conf['data_path'] / csv_path
-
         if method == 'constant':
             df_final[self.var_prod_price] = self.optim_conf['prod_sell_price']
         elif method == 'csv':
             forecast_dates_csv = self.get_forecast_days_csv(timedelta_days=0)
-            forecast_out = self.get_forecast_out_from_csv_or_list(df_final,
-                                                          forecast_dates_csv,
-                                                          csv_path)
+            forecast_out = self.get_forecast_out_from_csv_or_list(
+                df_final, forecast_dates_csv, csv_path)
             df_final[self.var_prod_price] = forecast_out
         elif method == 'list': # reading a list of values
             # Loading data from passed list
             data_list = self.params['passed_data']['prod_price_forecast']
             # Check if the passed data has the correct length
             if len(data_list) < len(self.forecast_dates) and self.params['passed_data']['prediction_horizon'] is None:
                 self.logger.error("Passed data from passed list is not long enough")
@@ -833,10 +828,9 @@
                 forecast_out = self.get_forecast_out_from_csv_or_list(
                     df_final, forecast_dates_csv, None, data_list=data_list, list_and_perfect=list_and_perfect)
                 # Fill the final DF
                 df_final[self.var_prod_price] = forecast_out
         else:
             self.logger.error("Passed method is not valid")
             return False
-            
         return df_final
```

### Comparing `emhass-0.9.0/src/emhass/machine_learning_forecaster.py` & `emhass-0.9.1/src/emhass/machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/machine_learning_regressor.py` & `emhass-0.9.1/src/emhass/machine_learning_regressor.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,24 +72,16 @@
 
     - `fit`: to train a model with the passed data.
 
     - `predict`: to obtain a forecast from a pre-trained model.
 
     """
 
-    def __init__(  # noqa: PLR0913
-        self: MLRegressor,
-        data: pd.DataFrame,
-        model_type: str,
-        regression_model: str,
-        features: list,
-        target: str,
-        timestamp: str,
-        logger: logging.Logger,
-    ) -> None:
+    def __init__(self: MLRegressor, data: pd.DataFrame, model_type: str, regression_model: str,
+                 features: list, target: str, timestamp: str, logger: logging.Logger) -> None:
         r"""Define constructor for the forecast class.
 
         :param data: The data that will be used for train/test
         :type data: pd.DataFrame
         :param model_type: A unique name defining this model and useful to identify \
             for what it will be used for.
         :type model_type: str
@@ -120,19 +112,15 @@
         self.data = self.data[~self.data.index.duplicated(keep="first")]
         self.data_exo = None
         self.steps = None
         self.model = None
         self.grid_search = None
 
     @staticmethod
-    def add_date_features(
-        data: pd.DataFrame,
-        date_features: list,
-        timestamp: str,
-    ) -> pd.DataFrame:
+    def add_date_features(data: pd.DataFrame, date_features: list, timestamp: str) -> pd.DataFrame:
         """Add date features from the input DataFrame timestamp.
 
         :param data: The input DataFrame
         :type data: pd.DataFrame
         :param timestamp: The column containing the timestamp
         :type timestamp: str
         :return: The DataFrame with the added features
@@ -148,31 +136,26 @@
             df["day_of_week"] = [i.dayofweek for i in df["timestamp"]]
         if "day_of_year" in date_features:
             df["day_of_year"] = [i.dayofyear for i in df["timestamp"]]
         if "day" in date_features:
             df["day"] = [i.day for i in df["timestamp"]]
         if "hour" in date_features:
             df["hour"] = [i.day for i in df["timestamp"]]
-
         return df
 
     def get_regression_model(self: MLRegressor) -> tuple[str, str]:
-        """Get the base model and parameter grid for the specified regression model.
-
+        r"""
+        Get the base model and parameter grid for the specified regression model.
         Returns a tuple containing the base model and parameter grid corresponding to \
             the specified regression model.
 
-        Args:
-        ----
-            self: The instance of the MLRegressor class.
-
-        Returns:
-        -------
-            A tuple containing the base model and parameter grid.
-
+        :param self: The instance of the MLRegressor class.
+        :type self: MLRegressor
+        :return: A tuple containing the base model and parameter grid.
+        :rtype: tuple[str, str]
         """
         if self.regression_model == "LinearRegression":
             base_model = REGRESSION_METHODS["LinearRegression"]["model"]
             param_grid = REGRESSION_METHODS["LinearRegression"]["param_grid"]
         elif self.regression_model == "RidgeRegression":
             base_model = REGRESSION_METHODS["RidgeRegression"]["model"]
             param_grid = REGRESSION_METHODS["RidgeRegression"]["param_grid"]
@@ -193,15 +176,15 @@
                 "Passed model %s is not valid",
                 self.regression_model,
             )
             return None
         return base_model, param_grid
 
     def fit(self: MLRegressor, date_features: list | None = None) -> None:
-        """Fit the model using the provided data.
+        r"""Fit the model using the provided data.
 
         :param date_features: A list of 'date_features' to take into account when \
             fitting the model.
         :type data: list
         """
         self.logger.info("Performing a MLRegressor fit for %s", self.model_type)
         self.data_exo = pd.DataFrame(self.data)
@@ -222,53 +205,32 @@
                     self.timestamp,
                 )
             else:
                 self.logger.error(
                     "If no timestamp provided, you can't use date_features, going \
                     further without date_features.",
                 )
-
         y = self.data_exo[self.target]
         self.data_exo = self.data_exo.drop(self.target, axis=1)
         if self.timestamp is not None:
             self.data_exo = self.data_exo.drop(self.timestamp, axis=1)
-        X = self.data_exo  # noqa: N806
-
-        X_train, X_test, y_train, y_test = train_test_split(  # noqa: N806
-            X,
-            y,
-            test_size=0.2,
-            random_state=42,
-        )
-
+        X = self.data_exo 
+        X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)
         self.steps = len(X_test)
-
         base_model, param_grid = self.get_regression_model()
-
         self.model = make_pipeline(StandardScaler(), base_model)
-
         # Create a grid search object
-        self.grid_search = GridSearchCV(
-            self.model,
-            param_grid,
-            cv=5,
-            scoring="neg_mean_squared_error",
-            refit=True,
-            verbose=0,
-            n_jobs=-1,
-        )
-
+        self.grid_search = GridSearchCV(self.model, param_grid, cv=5, scoring="neg_mean_squared_error",
+                                        refit=True, verbose=0, n_jobs=-1)
         # Fit the grid search object to the data
         self.logger.info("Training a %s model", self.regression_model)
         start_time = time.time()
         self.grid_search.fit(X_train.values, y_train.values)
         self.logger.info("Elapsed time for model fit: %s", time.time() - start_time)
-
         self.model = self.grid_search.best_estimator_
-
         # Make predictions
         predictions = self.model.predict(X_test.values)
         predictions = pd.Series(predictions, index=X_test.index)
         pred_metric = r2_score(y_test, predictions)
         self.logger.info(
             "Prediction R2 score of fitted model on test data: %s",
             pred_metric,
@@ -282,9 +244,8 @@
             Example: [2.24, 5.68].
         :type new_values: list
         :return: The np.ndarray containing the predicted value.
         :rtype: np.ndarray
         """
         self.logger.info("Performing a prediction for %s", self.model_type)
         new_values = np.array([new_values])
-
         return self.model.predict(new_values)
```

### Comparing `emhass-0.9.0/src/emhass/optimization.py` & `emhass-0.9.1/src/emhass/optimization.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/retrieve_hass.py` & `emhass-0.9.1/src/emhass/retrieve_hass.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,22 +61,17 @@
         self.freq = freq
         self.time_zone = time_zone
         self.params = params
         # self.emhass_conf = emhass_conf
         self.logger = logger
         self.get_data_from_file = get_data_from_file
 
-    def get_data(
-        self,
-        days_list: pd.date_range,
-        var_list: list,
-        minimal_response: Optional[bool] = False,
-        significant_changes_only: Optional[bool] = False,
-        test_url: Optional[str] = "empty",
-    ) -> None:
+    def get_data(self, days_list: pd.date_range, var_list: list, 
+                 minimal_response: Optional[bool] = False, significant_changes_only: Optional[bool] = False,
+                 test_url: Optional[str] = "empty") -> None:
         r"""
         Retrieve the actual data from hass.
         
         :param days_list: A list of days to retrieve. The ISO format should be used \
             and the timezone is UTC. The frequency of the data_range should be freq='D'
         :type days_list: pandas.date_range
         :param var_list: The list of variables to retrive from hass. These should \
@@ -96,17 +91,15 @@
             are experimental
         """
         self.logger.info("Retrieve hass get data method initiated...")
         self.df_final = pd.DataFrame()
         x = 0  # iterate based on days
         # Looping on each day from days list
         for day in days_list:
-
             for i, var in enumerate(var_list):
-
                 if test_url == "empty":
                     if (
                         self.hass_url == "http://supervisor/core/api"
                     ):  # If we are using the supervisor API
                         url = (
                             self.hass_url
                             + "/history/period/"
@@ -285,23 +278,16 @@
         if self.time_zone is not None:
             self.df_final.index = self.df_final.index.tz_convert(self.time_zone)
         # Drop datetimeindex duplicates on final DF
         self.df_final = self.df_final[~self.df_final.index.duplicated(keep="first")]
         return True
 
     @staticmethod
-    def get_attr_data_dict(
-        data_df: pd.DataFrame,
-        idx: int,
-        entity_id: str,
-        unit_of_measurement: str,
-        friendly_name: str,
-        list_name: str,
-        state: float,
-    ) -> dict:
+    def get_attr_data_dict(data_df: pd.DataFrame, idx: int, entity_id: str, unit_of_measurement: str,
+                           friendly_name: str, list_name: str, state: float) -> dict:
         list_df = copy.deepcopy(data_df).loc[data_df.index[idx] :].reset_index()
         list_df.columns = ["timestamps", entity_id]
         ts_list = [str(i) for i in list_df["timestamps"].tolist()]
         vals_list = [str(np.round(i, 2)) for i in list_df[entity_id].tolist()]
         forecast_list = []
         for i, ts in enumerate(ts_list):
             datum = {}
@@ -314,25 +300,17 @@
                 "unit_of_measurement": unit_of_measurement,
                 "friendly_name": friendly_name,
                 list_name: forecast_list,
             },
         }
         return data
 
-    def post_data(
-        self,
-        data_df: pd.DataFrame,
-        idx: int,
-        entity_id: str,
-        unit_of_measurement: str,
-        friendly_name: str,
-        type_var: str,
-        from_mlforecaster: Optional[bool] = False,
-        publish_prefix: Optional[str] = "",
-    ) -> None:
+    def post_data(self, data_df: pd.DataFrame, idx: int, entity_id: str, unit_of_measurement: str,
+                  friendly_name: str, type_var: str, from_mlforecaster: Optional[bool] = False,
+                  publish_prefix: Optional[str] = "") -> None:
         r"""
         Post passed data to hass.
         
         :param data_df: The DataFrame containing the data that will be posted \
             to hass. This should be a one columns DF or a series.
         :type data_df: pd.DataFrame
         :param idx: The int index of the location of the data within the passed \
@@ -371,83 +349,34 @@
         elif type_var == "optim_status":
             state = data_df.loc[data_df.index[idx]]
         elif type_var == "mlregressor":
             state = data_df[idx]
         else:
             state = np.round(data_df.loc[data_df.index[idx]], 2)
         if type_var == "power":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "forecasts",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "forecasts", state)
         elif type_var == "deferrable":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "deferrables_schedule",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "deferrables_schedule", state)
         elif type_var == "batt":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "battery_scheduled_power",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "battery_scheduled_power", state)
         elif type_var == "SOC":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "battery_scheduled_soc",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "battery_scheduled_soc", state)
         elif type_var == "unit_load_cost":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "unit_load_cost_forecasts",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement, 
+                                                   friendly_name, "unit_load_cost_forecasts", state)
         elif type_var == "unit_prod_price":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "unit_prod_price_forecasts",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "unit_prod_price_forecasts", state)
         elif type_var == "mlforecaster":
-            data = RetrieveHass.get_attr_data_dict(
-                data_df,
-                idx,
-                entity_id,
-                unit_of_measurement,
-                friendly_name,
-                "scheduled_forecast",
-                state,
-            )
+            data = RetrieveHass.get_attr_data_dict(data_df, idx, entity_id, unit_of_measurement,
+                                                   friendly_name, "scheduled_forecast", state)
         elif type_var == "optim_status":
             data = {
                 "state": state,
                 "attributes": {
                     "unit_of_measurement": unit_of_measurement,
                     "friendly_name": friendly_name,
                 },
@@ -466,18 +395,16 @@
                 "attributes": {
                     "unit_of_measurement": unit_of_measurement,
                     "friendly_name": friendly_name,
                 },
             }
         # Actually post the data
         if self.get_data_from_file:
-
             class response:
                 pass
-
             response.status_code = 200
             response.ok = True
         else:
             response = post(url, headers=headers, data=json.dumps(data))
         # Treating the response status and posting them on the logger
         if response.ok:
             self.logger.info("Successfully posted to " + entity_id + " = " + str(state))
```

### Comparing `emhass-0.9.0/src/emhass/static/advanced.html` & `emhass-0.9.1/src/emhass/static/advanced.html`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/basic.html` & `emhass-0.9.1/src/emhass/static/basic.html`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/img/emhass_icon.png` & `emhass-0.9.1/src/emhass/static/img/emhass_icon.png`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/img/emhass_logo_short.svg` & `emhass-0.9.1/src/emhass/static/img/emhass_logo_short.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/img/feather-sprite.svg` & `emhass-0.9.1/src/emhass/static/img/feather-sprite.svg`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/script.js` & `emhass-0.9.1/src/emhass/static/script.js`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/static/style.css` & `emhass-0.9.1/src/emhass/static/style.css`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/templates/index.html` & `emhass-0.9.1/src/emhass/templates/index.html`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass/utils.py` & `emhass-0.9.1/src/emhass/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         root = pathlib.Path(file).resolve().parent.parent
     elif num_parent == 1:
         root = pathlib.Path(file).resolve().parent
     else:
         raise ValueError("num_parent value not valid, must be between 1 and 3")
     return root
 
+
 def get_logger(fun_name: str, emhass_conf: dict, save_to_file: Optional[bool] = True,
                logging_level: Optional[str] = "DEBUG") -> Tuple[logging.Logger, logging.StreamHandler]:
     """
     Create a simple logger object.
 
     :param fun_name: The Python function object name where the logger will be used
     :type fun_name: str
@@ -84,17 +85,16 @@
     )
     ch.setFormatter(formatter)
     logger.addHandler(ch)
 
     return logger, ch
 
 
-def get_forecast_dates(
-    freq: int, delta_forecast: int, timedelta_days: Optional[int] = 0
-) -> pd.core.indexes.datetimes.DatetimeIndex:
+def get_forecast_dates(freq: int, delta_forecast: int, timedelta_days: Optional[int] = 0
+                       ) -> pd.core.indexes.datetimes.DatetimeIndex:
     """
     Get the date_range list of the needed future dates using the delta_forecast parameter.
 
     :param freq: Optimization time step.
     :type freq: int
     :param delta_forecast: Number of days to forecast in the future to be used for the optimization.
     :type delta_forecast: int
@@ -109,23 +109,17 @@
     end_forecast = (start_forecast + pd.Timedelta(days=delta_forecast)).replace(microsecond=0)
     forecast_dates = pd.date_range(start=start_forecast, 
         end=end_forecast+timedelta(days=timedelta_days)-freq, 
         freq=freq).round(freq, ambiguous='infer', nonexistent='shift_forward')
     return forecast_dates
 
 
-def treat_runtimeparams(
-    runtimeparams: str,
-    params: str,
-    retrieve_hass_conf: dict,
-    optim_conf: dict,
-    plant_conf: dict,
-    set_type: str,
-    logger: logging.Logger,
-) -> Tuple[str, dict]:
+def treat_runtimeparams(runtimeparams: str, params: str, retrieve_hass_conf: dict, optim_conf: dict,
+                        plant_conf: dict, set_type: str, logger: logging.Logger
+                        ) -> Tuple[str, dict]:
     """
     Treat the passed optimization runtime parameters.
 
     :param runtimeparams: Json string containing the runtime parameters dict.
     :type runtimeparams: str
     :param params: Configuration parameters passed from data/options.json
     :type params: str
@@ -499,14 +493,15 @@
         else:
             publish_prefix = runtimeparams["publish_prefix"]
         params["passed_data"]["publish_prefix"] = publish_prefix
     # Serialize the final params
     params = json.dumps(params)
     return params, retrieve_hass_conf, optim_conf, plant_conf
 
+
 def get_yaml_parse(emhass_conf: dict, use_secrets: Optional[bool] = True,
                    params: Optional[str] = None) -> Tuple[dict, dict, dict]:
     """
     Perform parsing of the config.yaml file.
     
     :param emhass_conf: Dictionary containing the needed emhass paths
     :type emhass_conf: dict
@@ -651,17 +646,15 @@
     injection_dict["subsubtitle2"] = (
         "<h4>Summary table for latest optimization results</h4>"
     )
     injection_dict["table2"] = table2
     return injection_dict
 
 
-def get_injection_dict_forecast_model_fit(
-    df_fit_pred: pd.DataFrame, mlf: MLForecaster
-) -> dict:
+def get_injection_dict_forecast_model_fit(df_fit_pred: pd.DataFrame, mlf: MLForecaster) -> dict:
     """
     Build a dictionary with graphs and tables for the webui for special MLF fit case.
 
     :param df_fit_pred: The fit result DataFrame
     :type df_fit_pred: pd.DataFrame
     :param mlf: The MLForecaster object
     :type mlf: MLForecaster
@@ -682,17 +675,15 @@
     injection_dict["subsubtitle0"] = (
         "<h4>Forecasting variable " + mlf.var_model + "</h4>"
     )
     injection_dict["figure_0"] = image_path_0
     return injection_dict
 
 
-def get_injection_dict_forecast_model_tune(
-    df_pred_optim: pd.DataFrame, mlf: MLForecaster
-) -> dict:
+def get_injection_dict_forecast_model_tune(df_pred_optim: pd.DataFrame, mlf: MLForecaster) -> dict:
     """
     Build a dictionary with graphs and tables for the webui for special MLF tune case.
 
     :param df_pred_optim: The tune result DataFrame
     :type df_pred_optim: pd.DataFrame
     :param mlf: The MLForecaster object
     :type mlf: MLForecaster
@@ -715,21 +706,16 @@
     injection_dict["subsubtitle0"] = (
         "<h4>Forecasting variable " + mlf.var_model + "</h4>"
     )
     injection_dict["figure_0"] = image_path_0
     return injection_dict
 
 
-def build_params(
-    params: dict,
-    params_secrets: dict,
-    options: dict,
-    addon: int,
-    logger: logging.Logger,
-) -> dict:
+def build_params(params: dict, params_secrets: dict, options: dict, addon: int,
+                 logger: logging.Logger) -> dict:
     """
     Build the main params dictionary from the loaded options.json when using the add-on.
 
     :param params: The main params dictionary
     :type params: dict
     :param params_secrets: The dictionary containing the secret protected variables
     :type params_secrets: dict
@@ -963,15 +949,14 @@
     :return: The list of days
     :rtype: pd.date_range
 
     """
     today = datetime.now(timezone.utc).replace(minute=0, second=0, microsecond=0)
     d = (today - timedelta(days=days_to_retrieve)).isoformat()
     days_list = pd.date_range(start=d, end=today.isoformat(), freq="D")
-
     return days_list
 
 
 def set_df_index_freq(df: pd.DataFrame) -> pd.DataFrame:
     """
     Set the freq of a DataFrame DateTimeIndex.
```

### Comparing `emhass-0.9.0/src/emhass/web_server.py` & `emhass-0.9.1/src/emhass/web_server.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/src/emhass.egg-info/PKG-INFO` & `emhass-0.9.1/src/emhass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emhass
-Version: 0.9.0
+Version: 0.9.1
 Summary: An Energy Management System for Home Assistant
 Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ
 Author-email: davidusb@gmail.com
 Keywords: energy,management,optimization,hass
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -36,51 +36,54 @@
 <div align="center">
   <br>
   <img alt="EMHASS" src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/emhass_logo.png" width="300px">
   <h1>Energy Management for Home Assistant</h1>
   <strong></strong>
 </div>
 <br>
+
 <p align="center">
-  <a href="https://github.com/davidusb-geek/emhass/releases">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/releases">
     <img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/davidusb-geek/emhass">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/actions">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/actions">
     <img alt="GitHub Workflow Status" src="https://img.shields.io/github/actions/workflow/status/davidusb-geek/emhass/python-test.yml?branch=master">
   </a>
-  <a href="https://codecov.io/github/davidusb-geek/emhass" >
+  <a hstyle="text-decoration:none" ref="https://codecov.io/github/davidusb-geek/emhass" >
     <img src="https://codecov.io/github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90"/>
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/blob/master/LICENSE">
     <img alt="GitHub" src="https://img.shields.io/github/license/davidusb-geek/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/emhass">
   </a>
-  <a href="https://pypi.org/project/emhass/">
+  <a style="text-decoration:none" href="https://pypi.org/project/emhass/">
     <img alt="PyPI - Status" src="https://img.shields.io/pypi/status/emhass">
   </a>
-  <a href="https://emhass.readthedocs.io/en/latest/">
+  <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
     <img alt="Read the Docs" src="https://img.shields.io/readthedocs/emhass">
   </a>
 </p>
+
 <div align="center">
- <a href="https://emhass.readthedocs.io/en/latest/">
+ <a style="text-decoration:none" href="https://emhass.readthedocs.io/en/latest/">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Documentation_button.svg" alt="Documentation">
   </a>
-   <a href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
+   <a style="text-decoration:none" href="https://community.home-assistant.io/t/emhass-an-energy-management-for-home-assistant/338126">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Community_button.svg" alt="Community">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass/issues">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass/issues">
       <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/Issues_button.svg" alt="Issues">
   </a>
-  <a href="https://github.com/davidusb-geek/emhass-add-on">
+  <a style="text-decoration:none" href="https://github.com/davidusb-geek/emhass-add-on">
      <img src="https://raw.githubusercontent.com/davidusb-geek/emhass/master/docs/images/EMHASS_Add_on_button.svg" alt="EMHASS Add-on">
   </a>
 </div>
+
 <br>
 <p align="center">
 If you like this work please consider buying a coffee ;-) 
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/davidusbgeek" target="_blank">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" >
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: emhass Version: 0.9.0 Summary: An Energy Management
+Metadata-Version: 2.1 Name: emhass Version: 0.9.1 Summary: An Energy Management
 System for Home Assistant Home-page: https://github.com/davidusb-geek/emhass
 Author: David HERNANDEZ Author-email: davidusb@gmail.com Keywords:
 energy,management,optimization,hass Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier: Topic
 :: Software Development :: Build Tools Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.11 Classifier:
 Operating System :: OS Independent Requires-Python: >=3.10, <3.12 Description-
@@ -14,16 +14,16 @@
 Requires-Dist: pyyaml>=5.4.1 Requires-Dist: tables<=3.9.1 Requires-Dist:
 skforecast==0.12.0 Requires-Dist: flask>=2.0.3 Requires-Dist: waitress>=2.1.1
 Requires-Dist: plotly>=5.6.0
 
                                    [EMHASS]
               ************ EEnneerrggyy MMaannaaggeemmeenntt ffoorr HHoommee AAssssiissttaanntt ************
 
- _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/
-  _g_i_t_h_u_b_/_d_a_v_i_d_u_s_b_-_g_e_e_k_/_e_m_h_a_s_s_/_b_r_a_n_c_h_/_m_a_s_t_e_r_/_g_r_a_p_h_/_b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_B_W_7_K_S_C_H_N_9_0_]
+ _[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _W_o_r_k_f_l_o_w_ _S_t_a_t_u_s_][https://codecov.io/
+  github/davidusb-geek/emhass/branch/master/graph/badge.svg?token=BW7KSCHN90]
          _[_G_i_t_H_u_b_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _S_t_a_t_u_s_]_[_R_e_a_d_ _t_h_e_ _D_o_c_s_]
                _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_C_o_m_m_u_n_i_t_y_]_[_I_s_s_u_e_s_]_[_E_M_H_A_S_S_ _A_d_d_-_o_n_]
 
            If you like this work please consider buying a coffee ;-)
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 EHMASS is a Python module designed to optimize your home energy interfacing
 with Home Assistant. ## Introduction EMHASS (Energy Management for Home
```

### Comparing `emhass-0.9.0/src/emhass.egg-info/SOURCES.txt` & `emhass-0.9.1/src/emhass.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_command_line_utils.py` & `emhass-0.9.1/tests/test_command_line_utils.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_forecast.py` & `emhass-0.9.1/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_machine_learning_forecaster.py` & `emhass-0.9.1/tests/test_machine_learning_forecaster.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_machine_learning_regressor.py` & `emhass-0.9.1/tests/test_machine_learning_regressor.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_optimization.py` & `emhass-0.9.1/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_retrieve_hass.py` & `emhass-0.9.1/tests/test_retrieve_hass.py`

 * *Files identical despite different names*

### Comparing `emhass-0.9.0/tests/test_utils.py` & `emhass-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

