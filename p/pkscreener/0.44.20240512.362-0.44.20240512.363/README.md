# Comparing `tmp/pkscreener-0.44.20240512.362.tar.gz` & `tmp/pkscreener-0.44.20240512.363.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240512.362.tar", last modified: Sun May 12 14:41:45 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240512.363.tar", last modified: Sun May 12 15:17:22 2024, max compression
```

## Comparing `pkscreener-0.44.20240512.362.tar` & `pkscreener-0.44.20240512.363.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/
--rw-rw-rw-   0        0        0     1086 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.652561 pkscreener-0.44.20240512.362/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    28414 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    30922 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    11667 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   128056 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55925 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-12 14:41:40.000000 pkscreener-0.44.20240512.362/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   131494 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/globals.py
--rw-rw-rw-   0        0        0      929 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51608 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30222 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:41:45.652561 pkscreener-0.44.20240512.362/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-12 14:41:45.000000 pkscreener-0.44.20240512.362/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-12 14:41:45.668179 pkscreener-0.44.20240512.362/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-12 14:38:37.000000 pkscreener-0.44.20240512.362/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:17:22.955569 pkscreener-0.44.20240512.363/
+-rw-rw-rw-   0        0        0     1086 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-12 15:17:22.955569 pkscreener-0.44.20240512.363/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 15:17:22.949547 pkscreener-0.44.20240512.363/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:17:22.955569 pkscreener-0.44.20240512.363/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    28414 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    30922 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    11667 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   128056 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55925 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-12 15:17:13.000000 pkscreener-0.44.20240512.363/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   131494 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/globals.py
+-rw-rw-rw-   0        0        0      929 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51608 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30383 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-12 15:17:22.949547 pkscreener-0.44.20240512.363/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-12 15:17:22.000000 pkscreener-0.44.20240512.363/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-12 15:17:22.955569 pkscreener-0.44.20240512.363/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-12 15:12:14.000000 pkscreener-0.44.20240512.363/setup.py
```

### Comparing `pkscreener-0.44.20240512.362/LICENSE` & `pkscreener-0.44.20240512.363/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/LICENSE-Others` & `pkscreener-0.44.20240512.363/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/PKG-INFO` & `pkscreener-0.44.20240512.363/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240512.362
+Version: 0.44.20240512.363
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.362.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.363.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.362/README.md` & `pkscreener-0.44.20240512.363/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.362/pkscreener/__init__.py` & `pkscreener-0.44.20240512.363/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/classes/keys.py` & `pkscreener-0.44.20240512.363/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/courbd.ttf` & `pkscreener-0.44.20240512.363/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/globals.py` & `pkscreener-0.44.20240512.363/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240512.363/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240512.363/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240512.363/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,14 +322,16 @@
 
 def runApplication():
     from pkscreener.globals import main, sendQuickScanResult,sendMessageToTelegramChannel, sendGlobalMarketBarometer, updateMenuChoiceHierarchy, isInterrupted, refreshStockData, closeWorkersAndExit
     # From a previous call to main with args, it may have been mutated.
     # Let's stock to the original args passed by user
     argsv = argParser.parse_known_args()
     args = argsv[0]
+    if args.options is not None:
+        args.options = args.options.replace("::",":")
     if args.runintradayanalysis:
         from pkscreener.classes.MenuOptions import menus
         runOptions = menus.allMenus(topLevel="C", index=12)
         optionalFinalOutcome_df = None
         import pkscreener.classes.Utility as Utility
         import pandas as pd
         # Delete any existing data from the previous run.
@@ -577,17 +579,19 @@
         pkscreenerbot.runpkscreenerbot()
         return
     
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
-    if args.options is not None and str(args.options) == "0":
-        # Must be from unit tests to be able to break out of loops via eventing
-        args.options = None
+    if args.options is not None:
+        if str(args.options) == "0":
+            # Must be from unit tests to be able to break out of loops via eventing
+            args.options = None
+        args.options = args.options.replace("::",":")
     
     if args.maxprice:
         configManager.maxLTP = args.maxprice
         configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
     if args.minprice:
         configManager.minLTP = args.minprice
         configManager.setConfig(ConfigManager.parser, default=True, showFileCreatedText=False)
```

### Comparing `pkscreener-0.44.20240512.362/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240512.363/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240512.362
+Version: 0.44.20240512.363
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.362.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240512.363.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -269,19 +269,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.361/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.362/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240512.362/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240512.363/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240512.362/setup.py` & `pkscreener-0.44.20240512.363/setup.py`

 * *Files identical despite different names*

