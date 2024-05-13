# Comparing `tmp/sportswrangler-0.1.0.tar.gz` & `tmp/sportswrangler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportswrangler-0.1.0.tar", max compression
+gzip compressed data, was "sportswrangler-0.1.1.tar", max compression
```

## Comparing `sportswrangler-0.1.0.tar` & `sportswrangler-0.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      454 2024-04-23 02:09:58.022221 sportswrangler-0.1.0/README.md
--rw-r--r--   0        0        0      422 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      102 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/generic/__init__.py
--rw-r--r--   0        0        0     2065 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/generic/wrangler.py
--rw-r--r--   0        0        0      154 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/global_configs.py
--rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/__init__.py
--rw-r--r--   0        0        0      206 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/__init__.py
--rw-r--r--   0        0        0     3732 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/classes.py
--rw-r--r--   0        0        0      238 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/constants.py
--rw-r--r--   0        0        0     4739 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/enums.py
--rw-r--r--   0        0        0      252 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/__init__.py
--rw-r--r--   0        0        0    20124 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/base.py
--rw-r--r--   0        0        0     2044 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/epl.py
--rw-r--r--   0        0        0     2079 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/mlb.py
--rw-r--r--   0        0        0     1949 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nba.py
--rw-r--r--   0        0        0     2276 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nfl.py
--rw-r--r--   0        0        0     1352 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nhl.py
--rw-r--r--   0        0        0       51 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/sports/__init__.py
--rw-r--r--   0        0        0       40 2024-04-23 02:09:58.026221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/__init__.py
--rw-r--r--   0        0        0   531535 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/players.csv
--rw-r--r--   0        0        0     5204 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
--rw-r--r--   0        0        0   144790 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/players.csv
--rw-r--r--   0        0        0     3101 2024-04-23 02:09:58.030221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
--rw-r--r--   0        0        0   774056 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/players.csv
--rw-r--r--   0        0        0     8878 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
--rw-r--r--   0        0        0   293594 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/players.csv
--rw-r--r--   0        0        0     3313 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
--rw-r--r--   0        0        0    12392 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/sports/data_feeds/wrangler.py
--rw-r--r--   0        0        0        0 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/__init__.py
--rw-r--r--   0        0        0      250 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/enums.py
--rw-r--r--   0        0        0      142 2024-04-23 02:09:58.034221 sportswrangler-0.1.0/sportswrangler/utils/helpers.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      454 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/README.md
+-rw-r--r--   0        0        0      422 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      169 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/generic/__init__.py
+-rw-r--r--   0        0        0     2065 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/generic/wrangler.py
+-rw-r--r--   0        0        0      154 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/global_configs.py
+-rw-r--r--   0        0        0       28 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/__init__.py
+-rw-r--r--   0        0        0     3732 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/classes.py
+-rw-r--r--   0        0        0      238 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/constants.py
+-rw-r--r--   0        0        0     4739 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/enums.py
+-rw-r--r--   0        0        0      252 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/__init__.py
+-rw-r--r--   0        0        0    20124 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/base.py
+-rw-r--r--   0        0        0     2044 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/epl.py
+-rw-r--r--   0        0        0     2079 2024-05-13 20:45:53.063984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/mlb.py
+-rw-r--r--   0        0        0     1949 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nba.py
+-rw-r--r--   0        0        0     2276 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nfl.py
+-rw-r--r--   0        0        0     1352 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nhl.py
+-rw-r--r--   0        0        0       51 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/__init__.py
+-rw-r--r--   0        0        0       40 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/__init__.py
+-rw-r--r--   0        0        0   531535 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/MLB/players.csv
+-rw-r--r--   0        0        0     5204 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/MLB/teams.csv
+-rw-r--r--   0        0        0   144790 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NBA/players.csv
+-rw-r--r--   0        0        0     3101 2024-05-13 20:45:53.067984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NBA/teams.csv
+-rw-r--r--   0        0        0   774056 2024-05-13 20:45:53.071984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NFL/players.csv
+-rw-r--r--   0        0        0     8878 2024-05-13 20:45:53.071984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NFL/teams.csv
+-rw-r--r--   0        0        0   293594 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NHL/players.csv
+-rw-r--r--   0        0        0     3313 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NHL/teams.csv
+-rw-r--r--   0        0        0    12392 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/sports/data_feeds/wrangler.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/utils/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/utils/enums.py
+-rw-r--r--   0        0        0      142 2024-05-13 20:45:53.075984 sportswrangler-0.1.1/sportswrangler/utils/helpers.py
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 sportswrangler-0.1.1/PKG-INFO
```

### Comparing `sportswrangler-0.1.0/sportswrangler/generic/wrangler.py` & `sportswrangler-0.1.1/sportswrangler/generic/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/classes.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/classes.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/utils/enums.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/utils/enums.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/base.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/base.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/epl.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/epl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/mlb.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/mlb.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nba.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nba.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nfl.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nfl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/odds/the_odds_api/wranglers/nhl.py` & `sportswrangler-0.1.1/sportswrangler/odds/the_odds_api/wranglers/nhl.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/players.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/MLB/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/MLB/teams.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/MLB/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/players.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NBA/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NBA/teams.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NBA/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/players.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NFL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NFL/teams.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NFL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/players.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NHL/players.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/assets/NHL/teams.csv` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/assets/NHL/teams.csv`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/sportswrangler/sports/data_feeds/wrangler.py` & `sportswrangler-0.1.1/sportswrangler/sports/data_feeds/wrangler.py`

 * *Files identical despite different names*

### Comparing `sportswrangler-0.1.0/PKG-INFO` & `sportswrangler-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sportswrangler
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for wranglin' sports and sports odds data
 Author: Dejon
 Author-email: dejon.wright@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

