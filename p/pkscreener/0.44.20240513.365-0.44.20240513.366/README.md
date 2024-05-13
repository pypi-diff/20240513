# Comparing `tmp/pkscreener-0.44.20240513.365.tar.gz` & `tmp/pkscreener-0.44.20240513.366.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240513.365.tar", last modified: Mon May 13 14:35:54 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240513.366.tar", last modified: Mon May 13 18:56:32 2024, max compression
```

## Comparing `pkscreener-0.44.20240513.365.tar` & `pkscreener-0.44.20240513.366.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/
--rw-rw-rw-   0        0        0     1086 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.138474 pkscreener-0.44.20240513.365/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34185 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    36256 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12370 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   153935 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55975 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-13 14:35:45.000000 pkscreener-0.44.20240513.365/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   134008 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51608 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30550 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.138474 pkscreener-0.44.20240513.365/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-13 14:31:23.000000 pkscreener-0.44.20240513.365/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/
+-rw-rw-rw-   0        0        0     1086 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.450799 pkscreener-0.44.20240513.366/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34185 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    36256 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12370 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-13 18:51:46.000000 pkscreener-0.44.20240513.366/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   153935 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55975 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-13 18:56:24.000000 pkscreener-0.44.20240513.366/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   134008 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51714 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30550 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:56:32.466420 pkscreener-0.44.20240513.366/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-13 18:56:32.000000 pkscreener-0.44.20240513.366/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 18:56:32.482043 pkscreener-0.44.20240513.366/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-13 18:51:47.000000 pkscreener-0.44.20240513.366/setup.py
```

### Comparing `pkscreener-0.44.20240513.365/LICENSE` & `pkscreener-0.44.20240513.366/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/LICENSE-Others` & `pkscreener-0.44.20240513.366/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/PKG-INFO` & `pkscreener-0.44.20240513.366/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.365
+Version: 0.44.20240513.366
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.365.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.366.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.365/README.md` & `pkscreener-0.44.20240513.366/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.365/pkscreener/__init__.py` & `pkscreener-0.44.20240513.366/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/classes/keys.py` & `pkscreener-0.44.20240513.366/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/courbd.ttf` & `pkscreener-0.44.20240513.366/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/globals.py` & `pkscreener-0.44.20240513.366/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240513.366/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240513.366/pkscreener/pkscreenerbot.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,14 +332,16 @@
         inlineMenus.append(
             InlineKeyboardButton(
                 mnu.menuKey, callback_data=str(f"{query.data}_{mnu.menuKey}")
             )
         )
     keyboard = [inlineMenus]
     reply_markup = InlineKeyboardMarkup(keyboard)
+    if query.message.text == menuText:
+        menuText = f"{PKDateUtilities.currentDateTime()}:\n{menuText}"
     await query.edit_message_text(text=menuText, reply_markup=reply_markup)
     return START_ROUTES
 
 
 async def Level2(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     inlineMenus = []
@@ -964,15 +966,15 @@
             sentFrom.append(abs(update.channel_post.chat.id))
             if update.channel_post.chat.username is not None:
                 sentFrom.append(update.channel_post.chat.username)
         if update.channel_post.sender_chat is not None:
             sentFrom.append(abs(update.channel_post.sender_chat.id))
             sentFrom.append(update.channel_post.sender_chat.username)
     if update.edited_channel_post is not None:
-        sentFrom.append(abs(update.edited_channel_post.sender_chat.username))
+        sentFrom.append(abs(update.edited_channel_post.sender_chat.id))
 
     if (
         abs(int(Channel_Id)) in sentFrom
         or abs(int(GROUP_CHAT_ID)) in sentFrom
         or "GroupAnonymousBot" in sentFrom
         or "PKScreener" in sentFrom
         or "PKScreeners" in sentFrom
```

### Comparing `pkscreener-0.44.20240513.365/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240513.366/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240513.366/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.365
+Version: 0.44.20240513.366
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.365.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.366.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.365/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.365/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240513.366/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.365/setup.py` & `pkscreener-0.44.20240513.366/setup.py`

 * *Files identical despite different names*

