# Comparing `tmp/pkscreener-0.44.20240513.364.tar.gz` & `tmp/pkscreener-0.44.20240513.365.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.44.20240513.364.tar", last modified: Mon May 13 13:13:35 2024, max compression
+gzip compressed data, was "pkscreener-0.44.20240513.365.tar", last modified: Mon May 13 14:35:54 2024, max compression
```

## Comparing `pkscreener-0.44.20240513.364.tar` & `pkscreener-0.44.20240513.365.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 13:13:35.583372 pkscreener-0.44.20240513.364/
--rw-rw-rw-   0        0        0     1086 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/LICENSE-Others
--rw-rw-rw-   0        0        0    27795 2024-05-13 13:13:35.583372 pkscreener-0.44.20240513.364/PKG-INFO
--rw-rw-rw-   0        0        0    26856 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 13:13:35.567752 pkscreener-0.44.20240513.364/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:13:35.583372 pkscreener-0.44.20240513.364/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5705 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    29030 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    11236 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    36256 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12370 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23700 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22221 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8158 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18597 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   153935 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    55975 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    83233 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-13 13:13:23.000000 pkscreener-0.44.20240513.364/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   134008 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1024 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    51608 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    30550 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-13 13:13:35.567752 pkscreener-0.44.20240513.364/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27795 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-13 13:13:35.000000 pkscreener-0.44.20240513.364/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-13 13:13:35.583372 pkscreener-0.44.20240513.364/setup.cfg
--rw-rw-rw-   0        0        0     4765 2024-05-13 13:08:07.000000 pkscreener-0.44.20240513.364/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/
+-rw-rw-rw-   0        0        0     1086 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/LICENSE-Others
+-rw-rw-rw-   0        0        0    27795 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/PKG-INFO
+-rw-rw-rw-   0        0        0    26856 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.138474 pkscreener-0.44.20240513.365/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5705 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34185 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    11236 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    36256 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12370 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23700 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22221 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8158 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18597 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   153935 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    55975 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    83233 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-13 14:35:45.000000 pkscreener-0.44.20240513.365/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   134008 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1024 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    51608 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    30550 2024-05-13 14:31:22.000000 pkscreener-0.44.20240513.365/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:35:54.138474 pkscreener-0.44.20240513.365/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27795 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-13 14:35:54.000000 pkscreener-0.44.20240513.365/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-13 14:35:54.154100 pkscreener-0.44.20240513.365/setup.cfg
+-rw-rw-rw-   0        0        0     4765 2024-05-13 14:31:23.000000 pkscreener-0.44.20240513.365/setup.py
```

### Comparing `pkscreener-0.44.20240513.364/LICENSE` & `pkscreener-0.44.20240513.365/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/LICENSE-Others` & `pkscreener-0.44.20240513.365/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/PKG-INFO` & `pkscreener-0.44.20240513.365/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.364
+Version: 0.44.20240513.365
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.364.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.365.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.364/README.md` & `pkscreener-0.44.20240513.365/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -247,19 +247,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.364/pkscreener/__init__.py` & `pkscreener-0.44.20240513.365/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/ArtTexts.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Backtest.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Barometer.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Changelog.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/ConfigManager.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/ConfigManager.py`

 * *Files 13% similar despite different names*

```diff
@@ -209,170 +209,194 @@
             OutputControls().printOutput("")
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] PKScreener User Configuration:"
                 + colorText.END
             )
-            self.period = input(
-                "[+] Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max\n[+] Enter number of days for which stock data to be downloaded (Days).(Optimal = 280): "
-            )
-            self.daysToLookback = input(
-                "[+] Number of recent trading periods (TimeFrame) to screen for Breakout/Consolidation (Days)(Optimal = 22): "
-            )
-            self.duration = input(
-                "[+] Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo\n[+] Enter Duration of each candle (Days)(Optimal = 1): "
-            )
-            self.minLTP = input(
-                "[+] Minimum Price of Stock to Buy (in RS)(Optimal = 20): "
-            )
-            self.maxLTP = input(
-                "[+] Maximum Price of Stock to Buy (in RS)(Optimal = 50000): "
-            )
-            self.volumeRatio = input(
-                "[+] How many times the volume should be more than average for the breakout? (Number)(Optimal = 2.5): "
-            )
-            self.consolidationPercentage = input(
-                "[+] How many % the price should be in range to consider it as consolidation? (Number)(Optimal = 10): "
-            )
-            self.shuffle = str(
-                input(
-                    "[+] Shuffle stocks rather than screening alphabetically? (Y/N): "
-                )
-            ).lower()
-            self.cacheStockData = str(
-                input(
-                    "[+] Enable High-Performance and Data-Saver mode? (This uses little bit more CPU but performs High Performance Screening) (Y/N): "
-                )
-            ).lower()
-            self.stageTwoPrompt = str(
-                input(
-                    "[+] Screen only for Stage-2 stocks?\n(What are the stages? => https://www.investopedia.com/articles/trading/08/stock-cycle-trend-price.asp)\n(Y/N): "
-                )
-            ).lower()
-            self.useEmaPrompt = str(
-                input(
-                    "[+] Use EMA instead of SMA? (EMA is good for Short-term & SMA for Mid/Long-term trades)[Y/N]: "
-                )
-            ).lower()
-            self.showunknowntrendsPrompt = str(
-                input(
-                    "[+] Show even those results where trends are not known[Y/N] (Recommended Y): "
-                )
-            ).lower()
-            self.logsEnabledPrompt = str(
-                input(
-                    "[+] Enable Viewing logs? You can enable if you are having problems.[Y/N]: "
-                )
-            ).lower()
-            self.enablePortfolioCalculations = str(
-                input(
-                    "[+] Enable calculating portfolio values? [Y/N]: "
-                )
-            ).lower()
-            self.showPastStrategyData = str(
-                input(
-                    "[+] Enable showing past strategy data? [Y/N]: "
-                )
-            ).lower()
-            self.calculatersiintraday = str(
-                input(
-                    "[+] Calculate intraday RSI during trading hours? [Y/N]: "
-                )
-            ).lower()
-            self.generalTimeout = input(
-                "[+] General network timeout (in seconds)(Optimal = 2 for good networks): "
-            )
-            self.longTimeout = input(
-                "[+] Long network timeout for heavier downloads(in seconds)(Optimal = 4 for good networks): "
-            )
-            self.maxNetworkRetryCount = input(
-                "[+] Maximum number of retries in case of network timeout(in seconds)(Optimal = 10 for slow networks): "
-            )
-            self.defaultIndex = input(
-                "[+] Default Index(NSE=12, NASDAQ=15): "
-            )
-            self.backtestPeriod = input(
-                "[+] Number of days in the past for backtesting(in days)(Optimal = 30): "
-            )
-            self.maxBacktestWindow = input(
-                "[+] Number of days to show the results for backtesting(in days)(Optimal = 1 to 30): "
-            )
-            self.morninganalysiscandlenumber = input(
-                "[+] Candle number since the market open time(Optimal = 15 to 60): "
-            )
-            self.morninganalysiscandleduration = input(
-                "[+] Enter Duration of each candle (minutes)(Optimal = 1 to 5): "
-            )
-            self.minVolume = input(
-                "[+] Minimum per day traded volume of any stock (number)(Optimal = 100000): "
-            )
-            self.backtestPeriodFactor = input(
-                "[+] Factor for backtest periods. If you choose 5, 1-Pd would mean 5-Pd returns. (number)(Optimal = 1): "
-            )
-            self.minimumChangePercentage = input(
-                "[+] Minimun change in stock price (in percentage). (number)(Optimal = 0): "
-            )
-            self.atrTrailingStopPeriod = input(
-                "[+] ATR Trailing Stop Periods. (number)(Optimal = 10): "
-            )
-            self.atrTrailingStopSensitivity = input(
-                "[+] ATR Trailing Stop Sensitivity. (number)(Optimal = 1): "
-            )
-            self.atrTrailingStopEMAPeriod = input(
-                "[+] ATR Trailing Stop EMA Period. (number)(Optimal = 1 to 200): "
-            )
-            parser.set("config", "atrtrailingstopemaperiod", self.atrTrailingStopEMAPeriod)
-            parser.set("config", "atrtrailingstopperiod", self.atrTrailingStopPeriod)
-            parser.set("config", "atrtrailingstopsensitivity", self.atrTrailingStopSensitivity)
-            parser.set("config", "backtestPeriod", self.backtestPeriod)
-            parser.set("config", "backtestPeriodFactor", self.backtestPeriodFactor)
-            parser.set("config", "cacheStockData", self.cacheStockData)
-            parser.set("config", "calculatersiintraday", self.calculatersiintraday)
-            parser.set("config", "daysToLookback", self.daysToLookback)
-            parser.set("config", "defaultIndex", self.defaultIndex)
-            parser.set("config", "defaultMonitorOptions", self.defaultMonitorOptions)
-            parser.set("config", "duration", self.duration + "d")
-            parser.set("config", "enablePortfolioCalculations", self.enablePortfolioCalculations)
-            parser.set("config", "generalTimeout", self.generalTimeout)
-            parser.set("config", "logsEnabled", self.logsEnabledPrompt)
-            parser.set("config", "longTimeout", self.longTimeout)
-            parser.set("config", "maxBacktestWindow", self.maxBacktestWindow)
-            parser.set("config", "maxNetworkRetryCount", self.maxNetworkRetryCount)
-            parser.set("config", "maxDashboardWidgetsPerRow", self.maxDashboardWidgetsPerRow)
-            parser.set("config", "maxNumResultRowsInMonitor", self.maxNumResultRowsInMonitor)
-            parser.set("config", "morninganalysiscandleduration", self.morninganalysiscandleduration + "m")
-            parser.set("config", "morninganalysiscandlenumber", self.morninganalysiscandlenumber)
-            parser.set("config", "onlyStageTwoStocks", self.stageTwoPrompt)
-            parser.set("config", "period", self.period + "d")
-            parser.set("config", "showPastStrategyData", self.showPastStrategyData)
-            parser.set("config", "showunknowntrends", self.showunknowntrendsPrompt)
-            parser.set("config", "shuffle", self.shuffle)
-            parser.set("config", "useEMA", self.useEmaPrompt)
+            try:
+                self.period = input(
+                    f"[+] Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max\n[+] Enter number of days for which stock data to be downloaded (Days).(Optimal = 280, Current: {colorText.FAIL}{self.period}{colorText.END}): "
+                ) or self.period
+                self.daysToLookback = input(
+                    f"[+] Number of recent trading periods (TimeFrame) to screen for Breakout/Consolidation (Days)(Optimal = 22, Current: {colorText.FAIL}{self.daysToLookback}{colorText.END}): "
+                ) or self.daysToLookback
+                self.duration = input(
+                    f"[+] Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo\n[+] Enter Duration of each candle (Days)(Optimal = 1, Current: {colorText.FAIL}{self.duration}{colorText.END}): "
+                ) or self.duration
+                self.minLTP = input(
+                    f"[+] Minimum Price of Stock to Buy (in RS)(Optimal = 20, Current: {colorText.FAIL}{self.minLTP}{colorText.END}): "
+                ) or self.minLTP
+                self.maxLTP = input(
+                    f"[+] Maximum Price of Stock to Buy (in RS)(Optimal = 50000, Current: {colorText.FAIL}{self.maxLTP}{colorText.END}): "
+                ) or self.maxLTP
+                self.volumeRatio = input(
+                    f"[+] How many times the volume should be more than average for the breakout? (Number)(Optimal = 2.5, Current: {colorText.FAIL}{self.volumeRatio}{colorText.END}): "
+                ) or self.volumeRatio
+                self.consolidationPercentage = input(
+                    f"[+] How much % the price should be in range, to consider it as consolidation? (Number)(Optimal = 10, Current: {colorText.FAIL}{self.consolidationPercentage}{colorText.END}): "
+                ) or self.consolidationPercentage
+                self.shuffle = str(
+                    input(
+                        f"[+] Shuffle stocks rather than screening alphabetically? (Y/N, Current: {colorText.FAIL}{'y' if self.shuffleEnabled else 'n'}{colorText.END}): "
+                    ) or ('y' if self.shuffleEnabled else 'n')
+                ).lower()
+                self.cacheStockData = str(
+                    input(
+                        f"[+] Enable High-Performance and Data-Saver mode? (This uses little bit more CPU but performs High Performance Screening) (Y/N, Current: {colorText.FAIL}{('y' if self.cacheEnabled else 'n')}{colorText.END}): "
+                    ) or ('y' if self.cacheEnabled else 'n')
+                ).lower()
+                self.stageTwoPrompt = str(
+                    input(
+                        f"[+] Screen only for Stage-2 stocks?\n(What are the stages? => https://www.investopedia.com/articles/trading/08/stock-cycle-trend-price.asp)\n(Y/N, Current: {colorText.FAIL}{'y' if self.stageTwo else 'n'}{colorText.END}): "
+                    ) or ('y' if self.stageTwo else 'n')
+                ).lower()
+                self.useEmaPrompt = str(
+                    input(
+                        f"[+] Use EMA instead of SMA? (EMA is good for Short-term & SMA for Mid/Long-term trades)[Y/N, Current: {colorText.FAIL}{'y' if self.useEMA else 'n'}{colorText.END}]: "
+                    ) or ('y' if self.useEMA else 'n')
+                ).lower()
+                self.showunknowntrendsPrompt = str(
+                    input(
+                        f"[+] Show even those results where trends are not known[Y/N] (Recommended Y, Current: {colorText.FAIL}{'y' if self.showunknowntrends else 'n'}{colorText.END}): "
+                    ) or ('y' if self.showunknowntrends else 'n')
+                ).lower()
+                self.logsEnabledPrompt = str(
+                    input(
+                        f"[+] Enable Viewing logs? You can enable if you are having problems.[Y/N, Current: {colorText.FAIL}{'y' if self.logsEnabled else 'n'}{colorText.END}]: "
+                    ) or ('y' if self.logsEnabled else 'n')
+                ).lower()
+                self.enablePortfolioCalculations = str(
+                    input(
+                        f"[+] Enable calculating portfolio values? [Y/N, Current: {colorText.FAIL}{'y' if self.enablePortfolioCalculations else 'n'}{colorText.END}]: "
+                    ) or ('y' if self.enablePortfolioCalculations else 'n')
+                ).lower()
+                self.showPastStrategyData = str(
+                    input(
+                        f"[+] Enable showing past strategy data? [Y/N, Current: {colorText.FAIL}{'y' if self.showPastStrategyData else 'n'}{colorText.END}]: "
+                    ) or ('y' if self.showPastStrategyData else 'n')
+                ).lower()
+                self.calculatersiintraday = str(
+                    input(
+                        f"[+] Calculate intraday RSI during trading hours? [Y/N, Current: {colorText.FAIL}{'y' if self.calculatersiintraday else 'n'}{colorText.END}]: "
+                    ) or ('y' if self.calculatersiintraday else 'n')
+                ).lower()
+                self.generalTimeout = input(
+                    f"[+] General network timeout (in seconds)(Optimal = 2 for good networks, Current: {colorText.FAIL}{self.generalTimeout}{colorText.END}): "
+                ) or self.generalTimeout
+                self.longTimeout = input(
+                    f"[+] Long network timeout for heavier downloads(in seconds)(Optimal = 4 for good networks, Current: {colorText.FAIL}{self.longTimeout}{colorText.END}): "
+                ) or self.longTimeout
+                self.maxNetworkRetryCount = input(
+                    f"[+] Maximum number of retries in case of network timeout(in seconds)(Optimal = 10 for slow networks, Current: {colorText.FAIL}{self.maxNetworkRetryCount}{colorText.END}): "
+                ) or self.maxNetworkRetryCount
+                self.defaultIndex = input(
+                    f"[+] Default Index(NSE=12, NASDAQ=15, Current: {colorText.FAIL}{self.defaultIndex}{colorText.END}): "
+                ) or self.defaultIndex
+                self.backtestPeriod = input(
+                    f"[+] Number of days in the past for backtesting(in days)(Optimal = 30, Current: {colorText.FAIL}{self.backtestPeriod}{colorText.END}): "
+                ) or self.backtestPeriod
+                self.maxBacktestWindow = input(
+                    f"[+] Number of days to show the results for backtesting(in days)(Optimal = 1 to 30, Current: {colorText.FAIL}{self.maxBacktestWindow}{colorText.END}): "
+                ) or self.maxBacktestWindow
+                self.morninganalysiscandlenumber = input(
+                    f"[+] Candle number since the market open time(Optimal = 15 to 60, Current: {colorText.FAIL}{self.morninganalysiscandlenumber}{colorText.END}): "
+                ) or self.morninganalysiscandlenumber
+                self.morninganalysiscandleduration = input(
+                    f"[+] Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo\n[+] Enter Duration of each candle (minutes)(Optimal = 1 to 5, Current: {colorText.FAIL}{self.morninganalysiscandleduration}{colorText.END}): "
+                ) or self.morninganalysiscandleduration
+                self.minVolume = input(
+                    f"[+] Minimum per day traded volume of any stock (number)(Optimal = 100000, Current: {colorText.FAIL}{self.minVolume}{colorText.END}): "
+                ) or self.minVolume
+                self.backtestPeriodFactor = input(
+                    f"[+] Factor for backtest periods. If you choose 5, 1-Pd would mean 5-Pd returns. (number)(Optimal = 1, Current: {colorText.FAIL}{self.backtestPeriodFactor}{colorText.END}): "
+                ) or self.backtestPeriodFactor
+                self.minimumChangePercentage = input(
+                    f"[+] Minimun change in stock price (in percentage). (number)(Optimal = 0, Current: {colorText.FAIL}{self.minimumChangePercentage}{colorText.END}): "
+                ) or self.minimumChangePercentage
+                self.atrTrailingStopPeriod = input(
+                    f"[+] ATR Trailing Stop Periods. (number)(Optimal = 10, Current: {colorText.FAIL}{self.atrTrailingStopPeriod}{colorText.END}): "
+                ) or self.atrTrailingStopPeriod
+                self.atrTrailingStopSensitivity = input(
+                    f"[+] ATR Trailing Stop Sensitivity. (number)(Optimal = 1, Current: {colorText.FAIL}{self.atrTrailingStopSensitivity}{colorText.END}): "
+                ) or self.atrTrailingStopSensitivity
+                self.atrTrailingStopEMAPeriod = input(
+                    f"[+] ATR Trailing Stop EMA Period. (number)(Optimal = 1 to 200, Current: {colorText.FAIL}{self.atrTrailingStopEMAPeriod}{colorText.END}): "
+                ) or self.atrTrailingStopEMAPeriod
+            except Exception as e:
+                default_logger().debug(e,exc_info=True)
+                from time import sleep
+                OutputControls().printOutput(colorText.FAIL + "Could not save configuration! Please check!" + colorText.END)
+                sleep(3)
+                pass
+            try:
+                parser.set("config", "atrtrailingstopemaperiod", str(self.atrTrailingStopEMAPeriod))
+                parser.set("config", "atrtrailingstopperiod", str(self.atrTrailingStopPeriod))
+                parser.set("config", "atrtrailingstopsensitivity", str(self.atrTrailingStopSensitivity))
+                parser.set("config", "backtestPeriod", str(self.backtestPeriod))
+                parser.set("config", "backtestPeriodFactor", str(self.backtestPeriodFactor))
+                parser.set("config", "cacheStockData", str(self.cacheStockData))
+                parser.set("config", "calculatersiintraday", str(self.calculatersiintraday))
+                parser.set("config", "daysToLookback", str(self.daysToLookback))
+                parser.set("config", "defaultIndex", str(self.defaultIndex))
+                parser.set("config", "defaultMonitorOptions", str(self.defaultMonitorOptions))
+                if self.duration:
+                    endDuration = str(self.duration)[-1].lower()
+                    endDuration = "d" if endDuration not in ["m","h","d","k","o"] else ""
+                parser.set("config", "duration", str(self.duration + endDuration))
+                parser.set("config", "enablePortfolioCalculations", str(self.enablePortfolioCalculations))
+                parser.set("config", "generalTimeout", str(self.generalTimeout))
+                parser.set("config", "logsEnabled", str(self.logsEnabledPrompt))
+                parser.set("config", "longTimeout", str(self.longTimeout))
+                parser.set("config", "maxBacktestWindow", str(self.maxBacktestWindow))
+                parser.set("config", "maxDashboardWidgetsPerRow", str(self.maxDashboardWidgetsPerRow))
+                parser.set("config", "maxNetworkRetryCount", str(self.maxNetworkRetryCount))
+                parser.set("config", "maxNumResultRowsInMonitor", str(self.maxNumResultRowsInMonitor))
+                if self.morninganalysiscandleduration:
+                    endMDuration = str(self.morninganalysiscandleduration)[-1].lower()
+                    endMDuration = "d" if endMDuration not in ["m","h","d","k","o"] else ""
+                parser.set("config", "morninganalysiscandleduration", str(self.morninganalysiscandleduration + endMDuration))
+                parser.set("config", "morninganalysiscandlenumber", str(self.morninganalysiscandlenumber))
+                parser.set("config", "onlyStageTwoStocks", str(self.stageTwoPrompt))
+                if self.period:
+                    endPeriod = str(self.period)[-1].lower()
+                    endPeriod = "d" if endPeriod not in ["d","o","y","x"] else ""
+                parser.set("config", "period", str(self.period + endPeriod))
+                parser.set("config", "showPastStrategyData", str(self.showPastStrategyData))
+                parser.set("config", "showunknowntrends", str(self.showunknowntrendsPrompt))
+                parser.set("config", "shuffle", str(self.shuffle))
+                parser.set("config", "useEMA", str(self.useEmaPrompt))
 
-            parser.set("filters", "consolidationPercentage", self.consolidationPercentage)
-            parser.set("filters", "maxPrice", self.maxLTP)
-            parser.set("filters", "minimumChangePercentage", self.minimumChangePercentage)
-            parser.set("filters", "minimumVolume", self.minVolume)
-            parser.set("filters", "minPrice", self.minLTP)
-            parser.set("filters", "volumeRatio", self.volumeRatio)
+                parser.set("filters", "consolidationPercentage", str(self.consolidationPercentage))
+                parser.set("filters", "maxPrice", str(self.maxLTP))
+                parser.set("filters", "minimumChangePercentage", str(self.minimumChangePercentage))
+                parser.set("filters", "minimumVolume", str(self.minVolume))
+                parser.set("filters", "minPrice", str(self.minLTP))
+                parser.set("filters", "volumeRatio", str(self.volumeRatio))
+            except Exception as e:
+                default_logger().debug(e,exc_info=True)
+                from time import sleep
+                OutputControls().printOutput(colorText.FAIL + "Could not save configuration! Please check!" + colorText.END)
+                sleep(3)
+                pass
 
             # delete stock data due to config change
             self.deleteFileWithPattern()
             OutputControls().printOutput(
                 colorText.BOLD
                 + colorText.FAIL
                 + "[+] Cached Stock Data Deleted."
                 + colorText.END
             )
 
             try:
                 fp = open("pkscreener.ini", "w")
                 parser.write(fp)
                 fp.close()
+                self.getConfig(parser=parser)
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + "[+] User configuration saved."
                     + colorText.END
                 )
                 input("Press <Enter> to continue...")
```

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Fetcher.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/MarketStatus.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/MenuOptions.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKScheduler.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PKTask.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Pktalib.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Portfolio.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/StockScreener.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/Utility.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/classes/keys.py` & `pkscreener-0.44.20240513.365/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/courbd.ttf` & `pkscreener-0.44.20240513.365/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/globals.py` & `pkscreener-0.44.20240513.365/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/pkscreener.ini` & `pkscreener-0.44.20240513.365/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/pkscreenerbot.py` & `pkscreener-0.44.20240513.365/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener/pkscreenercli.py` & `pkscreener-0.44.20240513.365/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.44.20240513.365/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.44.20240513.364
+Version: 0.44.20240513.365
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.364.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.44.20240513.365.zip
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
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240512.363/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.44.20240513.364/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.44.20240513.364/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.44.20240513.365/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.44.20240513.364/setup.py` & `pkscreener-0.44.20240513.365/setup.py`

 * *Files identical despite different names*

