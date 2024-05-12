# Comparing `tmp/schwab_api_wrapper-0.0.2.tar.gz` & `tmp/schwab_api_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_api_wrapper-0.0.2.tar", last modified: Sun Apr 28 01:35:05 2024, max compression
+gzip compressed data, was "schwab_api_wrapper-0.0.3.tar", last modified: Sun May 12 23:10:55 2024, max compression
```

## Comparing `schwab_api_wrapper-0.0.2.tar` & `schwab_api_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.924639 schwab_api_wrapper-0.0.2/
--rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.2/LICENSE
--rw-r--r--   0 owengordon   (501) staff       (20)      549 2024-04-28 01:35:05.924434 schwab_api_wrapper-0.0.2/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)       21 2024-04-28 01:19:10.000000 schwab_api_wrapper-0.0.2/README.md
--rw-r--r--   0 owengordon   (501) staff       (20)      598 2024-04-28 01:35:01.000000 schwab_api_wrapper-0.0.2/pyproject.toml
--rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-04-28 01:35:05.924691 schwab_api_wrapper-0.0.2/setup.cfg
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.918764 schwab_api_wrapper-0.0.2/src/
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.920839 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/
--rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/__main__.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.922465 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/market_hours_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/price_history_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)    10217 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/quotes_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/response_aware_retry.py
--rw-r--r--   0 owengordon   (501) staff       (20)    36504 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/schwab.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.923846 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/
--rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/__init__.py
--rw-r--r--   0 owengordon   (501) staff       (20)     7461 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/accounts_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/errors_schema.py
--rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/orders_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/transactions_schemas.py
--rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/utils.py
-drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-04-28 01:35:05.924196 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/
--rw-r--r--   0 owengordon   (501) staff       (20)      549 2024-04-28 01:35:05.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 owengordon   (501) staff       (20)      930 2024-04-28 01:35:05.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-04-28 01:35:05.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-04-28 01:35:05.000000 schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.187058 schwab_api_wrapper-0.0.3/
+-rw-r--r--   0 owengordon   (501) staff       (20)     1068 2024-04-28 01:20:00.000000 schwab_api_wrapper-0.0.3/LICENSE
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-12 23:10:55.186763 schwab_api_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)       42 2024-04-28 01:37:25.000000 schwab_api_wrapper-0.0.3/README.md
+-rw-r--r--   0 owengordon   (501) staff       (20)      622 2024-05-12 23:09:13.000000 schwab_api_wrapper-0.0.3/pyproject.toml
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.184285 schwab_api_wrapper-0.0.3/schwab_api_wrapper/
+-rw-r--r--   0 owengordon   (501) staff       (20)      125 2024-04-28 01:29:21.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      559 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/__main__.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.185378 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1421 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1181 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/market_hours_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      599 2024-04-28 01:14:10.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/price_history_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    10234 2024-05-12 22:58:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/quotes_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     1920 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/response_aware_retry.py
+-rw-r--r--   0 owengordon   (501) staff       (20)    36520 2024-05-08 01:27:40.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/schwab.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186025 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/
+-rw-r--r--   0 owengordon   (501) staff       (20)        0 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/__init__.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     7461 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/accounts_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)      411 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/errors_schema.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     9122 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/orders_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     5463 2024-04-28 01:14:51.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/transactions_schemas.py
+-rw-r--r--   0 owengordon   (501) staff       (20)     8190 2024-04-28 01:12:54.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper/utils.py
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186392 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/
+-rw-r--r--   0 owengordon   (501) staff       (20)      594 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 owengordon   (501) staff       (20)      879 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)        1 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       19 2024-05-12 23:10:55.000000 schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 owengordon   (501) staff       (20)       38 2024-05-12 23:10:55.187108 schwab_api_wrapper-0.0.3/setup.cfg
+drwxr-xr-x   0 owengordon   (501) staff       (20)        0 2024-05-12 23:10:55.186155 schwab_api_wrapper-0.0.3/tests/
+-rw-r--r--   0 owengordon   (501) staff       (20)    44497 2024-04-28 01:49:49.000000 schwab_api_wrapper-0.0.3/tests/test_schawb_api.py
```

### Comparing `schwab_api_wrapper-0.0.2/LICENSE` & `schwab_api_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/PKG-INFO` & `schwab_api_wrapper-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
-Project-URL: Homepage, https://github.com/OwenGordon/schwab
-Project-URL: Issues, https://github.com/OwenGordon/schwab/issues
+Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
+Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Schwab API Wrapper
+# schwab-api-wrapper
```

### Comparing `schwab_api_wrapper-0.0.2/pyproject.toml` & `schwab_api_wrapper-0.0.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schwab_api_wrapper"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Owen Gordon", email="owengordon330@outlook.com" },
 ]
 description = "A wrapper package around the schwab http api"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.com/OwenGordon/schwab"
-Issues = "https://github.com/OwenGordon/schwab/issues"
+Homepage = "https://github.com/OwenGordon/schwab-api-wrapper"
+Issues = "https://github.com/OwenGordon/schwab-api-wrapper/issues"
```

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/__main__.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/__main__.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/errors_schema.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/errors_schema.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/market_hours_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/market_hours_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/price_history_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/price_history_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/market_data/quotes_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/market_data/quotes_schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
     askTime: int  # Last ask time in milliseconds since Epoch
     bidMICId: str  # bid MIC code
     bidPrice: float  # Current Best Bid Price
     bidSize: int  # Number of shares for bid
     bidTime: int  # last bid tim in milliseconds since Epoch
     closePrice: float  # Previous day's closing price
     highPrice: float  # Day's high trade price
-    lastMICId: str  # Last MIC code
+    lastMICId: Optional[str] = None  # Last MIC code
     lastPrice: float  # TODO documentation missing on site
     lastSize: int  # Number of sahres traded with last trade
     lowPrice: float  # Day's low trade price
     mark: float  # Mark price
     markChange: float  # Mark Price change
     markPercentChange: float  # Mark Price percent change
     netChange: float  # Current Last-Prev Close
```

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/response_aware_retry.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/response_aware_retry.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/schwab.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/schwab.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,18 +68,18 @@
         )
 
         if (
             not renew_refresh_token
             and datetime.now(timezone.utc) >= self.refresh_token_valid_until
         ):
             logging.getLogger(__name__).fatal(
-                "The API OAuth Refresh token has expired. Please renew this token by running `python3 -m schwab_api [parameters.json]`"
+                "The API OAuth Refresh token has expired. Please renew this token by running `python3 -m schwab_api_wrapper [parameters.json]`"
             )
             print(
-                "The API OAuth Refresh token has expired. Please renew this token by running `python3 -m schwab_api [parameters.json]`"
+                "The API OAuth Refresh token has expired. Please renew this token by running `python3 -m schwab_api_wrapper [parameters.json]`"
             )
             exit(1)
 
         self.retry_strategy = ResponseAwareRetry(
             total=3,
             backoff_factor=1,
             status_forcelist=[429, 500, 501, 502, 503],
```

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/accounts_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/accounts_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/orders_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/orders_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/trader_api/transactions_schemas.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/trader_api/transactions_schemas.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper/utils.py` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/PKG-INFO` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: schwab_api_wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper package around the schwab http api
 Author-email: Owen Gordon <owengordon330@outlook.com>
-Project-URL: Homepage, https://github.com/OwenGordon/schwab
-Project-URL: Issues, https://github.com/OwenGordon/schwab/issues
+Project-URL: Homepage, https://github.com/OwenGordon/schwab-api-wrapper
+Project-URL: Issues, https://github.com/OwenGordon/schwab-api-wrapper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Schwab API Wrapper
+# schwab-api-wrapper
```

### Comparing `schwab_api_wrapper-0.0.2/src/schwab_api_wrapper.egg-info/SOURCES.txt` & `schwab_api_wrapper-0.0.3/schwab_api_wrapper.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
-src/schwab_api_wrapper/__init__.py
-src/schwab_api_wrapper/__main__.py
-src/schwab_api_wrapper/response_aware_retry.py
-src/schwab_api_wrapper/schwab.py
-src/schwab_api_wrapper/utils.py
-src/schwab_api_wrapper.egg-info/PKG-INFO
-src/schwab_api_wrapper.egg-info/SOURCES.txt
-src/schwab_api_wrapper.egg-info/dependency_links.txt
-src/schwab_api_wrapper.egg-info/top_level.txt
-src/schwab_api_wrapper/market_data/__init__.py
-src/schwab_api_wrapper/market_data/errors_schema.py
-src/schwab_api_wrapper/market_data/market_hours_schemas.py
-src/schwab_api_wrapper/market_data/price_history_schemas.py
-src/schwab_api_wrapper/market_data/quotes_schemas.py
-src/schwab_api_wrapper/trader_api/__init__.py
-src/schwab_api_wrapper/trader_api/accounts_schemas.py
-src/schwab_api_wrapper/trader_api/errors_schema.py
-src/schwab_api_wrapper/trader_api/orders_schemas.py
-src/schwab_api_wrapper/trader_api/transactions_schemas.py
+schwab_api_wrapper/__init__.py
+schwab_api_wrapper/__main__.py
+schwab_api_wrapper/response_aware_retry.py
+schwab_api_wrapper/schwab.py
+schwab_api_wrapper/utils.py
+schwab_api_wrapper.egg-info/PKG-INFO
+schwab_api_wrapper.egg-info/SOURCES.txt
+schwab_api_wrapper.egg-info/dependency_links.txt
+schwab_api_wrapper.egg-info/top_level.txt
+schwab_api_wrapper/market_data/__init__.py
+schwab_api_wrapper/market_data/errors_schema.py
+schwab_api_wrapper/market_data/market_hours_schemas.py
+schwab_api_wrapper/market_data/price_history_schemas.py
+schwab_api_wrapper/market_data/quotes_schemas.py
+schwab_api_wrapper/trader_api/__init__.py
+schwab_api_wrapper/trader_api/accounts_schemas.py
+schwab_api_wrapper/trader_api/errors_schema.py
+schwab_api_wrapper/trader_api/orders_schemas.py
+schwab_api_wrapper/trader_api/transactions_schemas.py
+tests/test_schawb_api.py
```

