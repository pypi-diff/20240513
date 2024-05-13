# Comparing `tmp/mkt-retv-1.422.tar.gz` & `tmp/mkt-retv-1.423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkt-retv-1.422.tar", last modified: Mon May  6 15:01:39 2024, max compression
+gzip compressed data, was "mkt-retv-1.423.tar", last modified: Mon May 13 14:51:52 2024, max compression
```

## Comparing `mkt-retv-1.422.tar` & `mkt-retv-1.423.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.612087 mkt-retv-1.422/
--rw-rw-rw-   0        0        0      697 2024-05-06 15:01:39.612087 mkt-retv-1.422/PKG-INFO
--rw-rw-rw-   0        0        0     1633 2024-05-06 09:02:26.000000 mkt-retv-1.422/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.040593 mkt-retv-1.422/market_research/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.422/market_research/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.150742 mkt-retv-1.422/market_research/analysis/
--rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.422/market_research/analysis/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.422/market_research/analysis/_analysis_scheme.py
--rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.422/market_research/analysis/imgemanger.py
--rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.422/market_research/analysis/sentimentmanager.py
--rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.422/market_research/analysis/textmanager.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.213798 mkt-retv-1.422/market_research/scraper/
--rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.422/market_research/scraper/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.422/market_research/scraper/_scaper_scheme.py
--rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.422/market_research/scraper/_visualizer_scheme.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.230278 mkt-retv-1.422/market_research/scraper/models/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.422/market_research/scraper/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.230278 mkt-retv-1.422/market_research/scraper/models/lge/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.422/market_research/scraper/models/lge/__init__.py
--rw-rw-rw-   0        0        0    13027 2024-05-06 15:01:23.000000 mkt-retv-1.422/market_research/scraper/models/lge/spec_l.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.245419 mkt-retv-1.422/market_research/scraper/models/pana/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.422/market_research/scraper/models/pana/__init__.py
--rw-rw-rw-   0        0        0     6924 2024-05-06 15:01:23.000000 mkt-retv-1.422/market_research/scraper/models/pana/spec_p.py
--rw-rw-rw-   0        0        0    12990 2024-05-06 15:01:23.000000 mkt-retv-1.422/market_research/scraper/models/pana/spec_pjp.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.308372 mkt-retv-1.422/market_research/scraper/models/sony/
--rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.422/market_research/scraper/models/sony/__init__.py
--rw-rw-rw-   0        0        0     5356 2024-05-06 08:36:11.000000 mkt-retv-1.422/market_research/scraper/models/sony/cleanup_s.py
--rw-rw-rw-   0        0        0    10665 2024-05-06 15:01:23.000000 mkt-retv-1.422/market_research/scraper/models/sony/sepc_sjp.py
--rw-rw-rw-   0        0        0    12584 2024-05-06 15:01:23.000000 mkt-retv-1.422/market_research/scraper/models/sony/spec_s.py
--rw-rw-rw-   0        0        0     4392 2024-05-06 09:01:29.000000 mkt-retv-1.422/market_research/scraper/models/sony/visualizer_s.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.392574 mkt-retv-1.422/market_research/scraper/rtings/
--rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.422/market_research/scraper/rtings/__init__.py
--rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.422/market_research/scraper/rtings/rtings.py
--rw-rw-rw-   0        0        0     6309 2023-11-26 10:28:52.000000 mkt-retv-1.422/market_research/scraper/rtings/rurlsearcher.py
--rw-rw-rw-   0        0        0    13793 2023-11-23 12:05:59.000000 mkt-retv-1.422/market_research/scraper/rtings/rvisualizer.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.517805 mkt-retv-1.422/market_research/tools/
--rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.422/market_research/tools/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.422/market_research/tools/aimanager.py
--rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.422/market_research/tools/filemanager.py
--rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.422/market_research/tools/installer.py
--rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.422/market_research/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-06 15:01:39.596426 mkt-retv-1.422/mkt_retv.egg-info/
--rw-rw-rw-   0        0        0      697 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 15:01:38.000000 mkt-retv-1.422/mkt_retv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 15:01:39.612087 mkt-retv-1.422/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-06 15:01:34.000000 mkt-retv-1.422/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.364982 mkt-retv-1.423/
+-rw-rw-rw-   0        0        0      697 2024-05-13 14:51:52.364384 mkt-retv-1.423/PKG-INFO
+-rw-rw-rw-   0        0        0     1633 2024-05-06 09:02:26.000000 mkt-retv-1.423/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.249167 mkt-retv-1.423/market_research/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.423/market_research/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.268282 mkt-retv-1.423/market_research/analysis/
+-rw-rw-rw-   0        0        0      167 2024-01-28 14:21:17.000000 mkt-retv-1.423/market_research/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-11-23 12:49:10.000000 mkt-retv-1.423/market_research/analysis/_analysis_scheme.py
+-rw-rw-rw-   0        0        0    10414 2024-01-30 11:22:46.000000 mkt-retv-1.423/market_research/analysis/imgemanger.py
+-rw-rw-rw-   0        0        0    11047 2023-12-02 10:26:16.000000 mkt-retv-1.423/market_research/analysis/sentimentmanager.py
+-rw-rw-rw-   0        0        0     6080 2024-04-27 23:25:08.000000 mkt-retv-1.423/market_research/analysis/textmanager.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.268282 mkt-retv-1.423/market_research/scraper/
+-rw-rw-rw-   0        0        0      538 2024-05-05 09:44:35.000000 mkt-retv-1.423/market_research/scraper/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-11-21 13:39:46.000000 mkt-retv-1.423/market_research/scraper/_scaper_scheme.py
+-rw-rw-rw-   0        0        0      497 2023-11-21 16:22:41.000000 mkt-retv-1.423/market_research/scraper/_visualizer_scheme.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.268282 mkt-retv-1.423/market_research/scraper/models/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.423/market_research/scraper/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.280825 mkt-retv-1.423/market_research/scraper/models/lge/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.423/market_research/scraper/models/lge/__init__.py
+-rw-rw-rw-   0        0        0    13027 2024-05-06 15:01:23.000000 mkt-retv-1.423/market_research/scraper/models/lge/spec_l.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.280825 mkt-retv-1.423/market_research/scraper/models/pana/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.423/market_research/scraper/models/pana/__init__.py
+-rw-rw-rw-   0        0        0     6924 2024-05-06 15:01:23.000000 mkt-retv-1.423/market_research/scraper/models/pana/spec_p.py
+-rw-rw-rw-   0        0        0    12990 2024-05-06 15:01:23.000000 mkt-retv-1.423/market_research/scraper/models/pana/spec_pjp.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.295099 mkt-retv-1.423/market_research/scraper/models/sony/
+-rw-rw-rw-   0        0        0        0 2024-05-05 10:36:43.000000 mkt-retv-1.423/market_research/scraper/models/sony/__init__.py
+-rw-rw-rw-   0        0        0     5356 2024-05-06 08:36:11.000000 mkt-retv-1.423/market_research/scraper/models/sony/cleanup_s.py
+-rw-rw-rw-   0        0        0    10665 2024-05-06 15:01:23.000000 mkt-retv-1.423/market_research/scraper/models/sony/sepc_sjp.py
+-rw-rw-rw-   0        0        0    12584 2024-05-06 15:01:23.000000 mkt-retv-1.423/market_research/scraper/models/sony/spec_s.py
+-rw-rw-rw-   0        0        0     4392 2024-05-06 09:01:29.000000 mkt-retv-1.423/market_research/scraper/models/sony/visualizer_s.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.300059 mkt-retv-1.423/market_research/scraper/rtings/
+-rw-rw-rw-   0        0        0      106 2023-11-19 08:24:51.000000 mkt-retv-1.423/market_research/scraper/rtings/__init__.py
+-rw-rw-rw-   0        0        0    10290 2023-11-23 09:57:43.000000 mkt-retv-1.423/market_research/scraper/rtings/rtings.py
+-rw-rw-rw-   0        0        0     5636 2024-05-13 14:42:54.000000 mkt-retv-1.423/market_research/scraper/rtings/rurlsearcher.py
+-rw-rw-rw-   0        0        0    15786 2024-05-13 14:46:31.000000 mkt-retv-1.423/market_research/scraper/rtings/rvisualizer.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.309537 mkt-retv-1.423/market_research/tools/
+-rw-rw-rw-   0        0        0      206 2023-11-16 08:38:53.000000 mkt-retv-1.423/market_research/tools/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-11-18 14:03:46.000000 mkt-retv-1.423/market_research/tools/aimanager.py
+-rw-rw-rw-   0        0        0     3371 2023-11-19 12:13:44.000000 mkt-retv-1.423/market_research/tools/filemanager.py
+-rw-rw-rw-   0        0        0     3818 2023-11-14 14:05:22.000000 mkt-retv-1.423/market_research/tools/installer.py
+-rw-rw-rw-   0        0        0     5509 2023-11-15 11:16:47.000000 mkt-retv-1.423/market_research/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:51:52.360659 mkt-retv-1.423/mkt_retv.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      129 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 14:51:52.000000 mkt-retv-1.423/mkt_retv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:51:52.364982 mkt-retv-1.423/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-13 14:50:36.000000 mkt-retv-1.423/setup.py
```

### Comparing `mkt-retv-1.422/PKG-INFO` & `mkt-retv-1.423/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.422
+Version: 1.423
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.422/README.md` & `mkt-retv-1.423/README.md`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/analysis/_analysis_scheme.py` & `mkt-retv-1.423/market_research/analysis/_analysis_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/analysis/imgemanger.py` & `mkt-retv-1.423/market_research/analysis/imgemanger.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/analysis/sentimentmanager.py` & `mkt-retv-1.423/market_research/analysis/sentimentmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/analysis/textmanager.py` & `mkt-retv-1.423/market_research/analysis/textmanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/__init__.py` & `mkt-retv-1.423/market_research/scraper/__init__.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/_scaper_scheme.py` & `mkt-retv-1.423/market_research/scraper/_scaper_scheme.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/lge/spec_l.py` & `mkt-retv-1.423/market_research/scraper/models/lge/spec_l.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/pana/spec_p.py` & `mkt-retv-1.423/market_research/scraper/models/pana/spec_p.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/pana/spec_pjp.py` & `mkt-retv-1.423/market_research/scraper/models/pana/spec_pjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/sony/cleanup_s.py` & `mkt-retv-1.423/market_research/scraper/models/sony/cleanup_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/sony/sepc_sjp.py` & `mkt-retv-1.423/market_research/scraper/models/sony/sepc_sjp.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/sony/spec_s.py` & `mkt-retv-1.423/market_research/scraper/models/sony/spec_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/models/sony/visualizer_s.py` & `mkt-retv-1.423/market_research/scraper/models/sony/visualizer_s.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/rtings/rtings.py` & `mkt-retv-1.423/market_research/scraper/rtings/rtings.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/scraper/rtings/rurlsearcher.py` & `mkt-retv-1.423/market_research/scraper/rtings/rurlsearcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,104 +1,103 @@
 import time
 from selenium.webdriver.common.keys import Keys
 from bs4 import BeautifulSoup
 import pandas as pd
 from tqdm import tqdm
 from market_research.scraper._scaper_scheme import Scraper
 
+
 class Rurlsearcher(Scraper):
     def __init__(self, enable_headless=True):
         super().__init__(enable_headless=enable_headless)
-        self.wait_time=2
-        self.model_dictionary = {"sony":{
-                                        "oled": [
-                                            'XR-77A95L', 'XR-65A75L', 'XR-65A95K', 'XR-65A90J', 'XR-65A80CL',
-                                            'XR-77A80CL', 'XR-77A80K', 'XR-65A80CK', 'XR-42A90K', 'XR-55A80CL',
-                                            'XR-83A80CL', 'XR-55A80CK', 'XR-65A80K', 'XR-83A90J', 'XR-48A90K',
-                                            'XR-77A80L', 'XR-55A95K', 'XR-77A80CK', 'XR-55A80L', 'XR-55A80K',
-                                            'XR-55A95L', 'XR-65A95L', 'XR-55A75L', 'XR-65A80L', 'XR-83A80L',
-                                            'XR-55A90J'
-                                        ],
-                                        "mini_led": [
-                                            'XR-65X93CL', 'XR-75X93CL', 'XR-75X93L', 'XR-85X93L', 'XR-85X95L',
-                                            'XR-65X93L'
-                                        ],
-                                        "lcd":['XR-55X90CK', 'XR-65X90CK', 'XR-75X90CK', 'XR-85X90CK',
-                                               'KD-55X80CK', 'KD-65X80CK', 'KD-75X80CK', 'KD-85X80CK',
-                                               'KD-43X85K', 'KD-50X85K', 'KD-55X85K', 'KD-65X85K', 'KD-75X85K',
-                                               'KD-85X85K', 'XR-55X90CL', 'XR-65X90CL', 'XR-75X90CL',
-                                               'XR-85X90CL', 'XR-65X95K', 'XR-75X95K', 'XR-85X95K', 'XR-55X90K',
-                                               'XR-65X90K', 'XR-75X90K', 'XR-85X90K', 'XR-55X90L', 'XR-65X90L',
-                                               'XR-75X90L', 'XR-85X90L', 'XR-98X90L', 'KD-43X80K', 'KD-50X80K',
-                                               'KD-55X80K', 'KD-65X80K', 'KD-75X80K', 'KD-85X80K', 'XR-75Z9K',
-                                               'XR-85Z9K', 'KD-32W830K', 'KD-55X77CL', 'KD-65X77CL', 'KD-75X77CL',
-                                               'KD-85X77CL', 'KD-43X77L', 'KD-50X77L', 'KD-55X77L', 'KD-65X77L',
-                                               'KD-75X77L', 'KD-85X77L']
-                                    }
+        self.wait_time = 2
+        self.model_dictionary = {"sony": {
+            "oled": [
+                'XR-77A95L', 'XR-65A75L', 'XR-65A95K', 'XR-65A90J', 'XR-65A80CL',
+                'XR-77A80CL', 'XR-77A80K', 'XR-65A80CK', 'XR-42A90K', 'XR-55A80CL',
+                'XR-83A80CL', 'XR-55A80CK', 'XR-65A80K', 'XR-83A90J', 'XR-48A90K',
+                'XR-77A80L', 'XR-55A95K', 'XR-77A80CK', 'XR-55A80L', 'XR-55A80K',
+                'XR-55A95L', 'XR-65A95L', 'XR-55A75L', 'XR-65A80L', 'XR-83A80L',
+                'XR-55A90J'
+            ],
+            "mini_led": [
+                'XR-65X93CL', 'XR-75X93CL', 'XR-75X93L', 'XR-85X93L', 'XR-85X95L',
+                'XR-65X93L'
+            ],
+            "lcd": ['XR-55X90CK', 'XR-65X90CK', 'XR-75X90CK', 'XR-85X90CK',
+                    'KD-55X80CK', 'KD-65X80CK', 'KD-75X80CK', 'KD-85X80CK',
+                    'KD-43X85K', 'KD-50X85K', 'KD-55X85K', 'KD-65X85K', 'KD-75X85K',
+                    'KD-85X85K', 'XR-55X90CL', 'XR-65X90CL', 'XR-75X90CL',
+                    'XR-85X90CL', 'XR-65X95K', 'XR-75X95K', 'XR-85X95K', 'XR-55X90K',
+                    'XR-65X90K', 'XR-75X90K', 'XR-85X90K', 'XR-55X90L', 'XR-65X90L',
+                    'XR-75X90L', 'XR-85X90L', 'XR-98X90L', 'KD-43X80K', 'KD-50X80K',
+                    'KD-55X80K', 'KD-65X80K', 'KD-75X80K', 'KD-85X80K', 'XR-75Z9K',
+                    'XR-85Z9K', 'KD-32W830K', 'KD-55X77CL', 'KD-65X77CL', 'KD-75X77CL',
+                    'KD-85X77CL', 'KD-43X77L', 'KD-50X77L', 'KD-55X77L', 'KD-65X77L',
+                    'KD-75X77L', 'KD-85X77L']
+        }
         }
 
         self.model_url_preset = {"sony":
             {
                 "oled": [
                     'https://www.rtings.com/tv/reviews/sony/a90k-oled',
-                     'https://www.rtings.com/tv/reviews/sony/a80l-a80cl-oled',
-                     'https://www.rtings.com/tv/reviews/sony/a90j-oled',
-                     'https://www.rtings.com/tv/reviews/sony/a95k-oled',
-                     'https://www.rtings.com/tv/reviews/sony/a95l-oled',
-                     'https://www.rtings.com/tv/reviews/lg/g3-oled',
-                     'https://www.rtings.com/tv/reviews/sony/a80k-a80ck-oled'
-                         ],
+                    'https://www.rtings.com/tv/reviews/sony/a80l-a80cl-oled',
+                    'https://www.rtings.com/tv/reviews/sony/a90j-oled',
+                    'https://www.rtings.com/tv/reviews/sony/a95k-oled',
+                    'https://www.rtings.com/tv/reviews/sony/a95l-oled',
+                    'https://www.rtings.com/tv/reviews/lg/g3-oled',
+                    'https://www.rtings.com/tv/reviews/sony/a80k-a80ck-oled'
+                ],
                 "mini_led": [
                     'https://www.rtings.com/tv/reviews/sony/x95l',
                     'https://www.rtings.com/tv/reviews/sony/x93l-x93cl'
                 ],
-                "lcd":[
+                "lcd": [
                     'https://www.rtings.com/tv/reviews/sony/x90l-x90cl',
-                     'https://www.rtings.com/tv/reviews/sony/x77l-x77cl',
-                     'https://www.rtings.com/tv/reviews/sony/x85k',
-                     'https://www.rtings.com/tv/reviews/sony/a95l-oled',
-                     'https://www.rtings.com/tv/reviews/sony/x90k-x90ck',
-                     'https://www.rtings.com/tv/reviews/sony/x95k',
-                     'https://www.rtings.com/tv/reviews/sony/x80k-x80ck'
+                    'https://www.rtings.com/tv/reviews/sony/x77l-x77cl',
+                    'https://www.rtings.com/tv/reviews/sony/x85k',
+                    'https://www.rtings.com/tv/reviews/sony/a95l-oled',
+                    'https://www.rtings.com/tv/reviews/sony/x90k-x90ck',
+                    'https://www.rtings.com/tv/reviews/sony/x95k',
+                    'https://www.rtings.com/tv/reviews/sony/x80k-x80ck'
                 ]
             }
         }
 
-
-    def get_model_from_dictionary(self, maker:str="sony", key_mode=False):
+    def get_model_from_dictionary(self, maker: str = "sony", key_mode=False):
         if key_mode:
             return self.model_dictionary.keys()
         return self.model_dictionary.get(maker.lower())
 
-    def get_url_from_model_preset(self, maker:str="sony", key_mode=False):
+    def get_url_from_model_preset(self, maker: str = "sony", key_mode=False):
         if key_mode:
             return self.model_dictionary.keys()
         return self.model_dictionary.get(maker.lower())
 
-    def get_urls_from_web(self, keywords:list[str,] = None)->list:
-        urls_set = set()  
+    def get_urls_from_web(self, keywords: list[str,] = None) -> list:
+        urls_set = set()
         for keyword in tqdm(keywords):
             url = self._search_and_extract_url(search_query=keyword)
             if url is not None:
                 urls_set.add(url)
         return list(urls_set)
 
-    def get_urls_from_inputpath(self, intput_folder_path:str)->list:
+    def get_urls_from_inputpath(self, intput_folder_path: str) -> list:
         self.set_data_path(intput_folder_path=intput_folder_path)
 
         urls = []
         file_list = self.intput_folder.glob('*')
         excel_files = [file for file in file_list if file.suffix in {'.xlsx', '.xls'}]
         for excel_file in excel_files:
             df = pd.read_excel(excel_file)
             urls.extend(df["urls"])
         return urls
 
-
-    def _search_and_extract_url(self, search_query:str, base_url = "https://www.rtings.com"):
+    def _search_and_extract_url(self, search_query: str, base_url="https://www.rtings.com"):
         driver = self.web_driver.get_chrome()
         try:
             driver.get(base_url)
             search_input = driver.find_element("class name", "searchbar-input")
             search_input.send_keys(search_query)
             search_input.send_keys(Keys.RETURN)
             time.sleep(self.wait_time)
@@ -113,8 +112,7 @@
                     split_url = url.split('/')
                     if len(split_url) == 5:
                         return base_url + url
         finally:
             # 브라우저 종료
             driver.quit()
         return None
-
```

### Comparing `mkt-retv-1.422/market_research/scraper/rtings/rvisualizer.py` & `mkt-retv-1.423/market_research/scraper/rtings/rvisualizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,50 +176,96 @@
 
         if save_plot_name is None:
             file_name = re.sub(r'\([^)]*\)', '', sup_title)
             save_plot_name = f"plot_for_{file_name}.png"
         plt.savefig(self.output_folder / save_plot_name, bbox_inches='tight')
         plt.show()
 
+    import matplotlib.pyplot as plt
+
     def plot_lines(self, column, swap_mode=True, ylims: list = None,
-                   yticks: list = None, save_plot_name:str=None):
+                   yticks: list = None, save_plot_name: str = None):
 
         df = self._get_data(column)
         mode_dict = self._plot_mode(column, swap_mode)
         col_y = mode_dict.get("col_y")
         col_x = mode_dict.get("col_x")
         col_color = mode_dict.get("col_facet")
 
         suffix = self.title_units_dict.get(col_y)
-        
+
         if suffix is not None:
             sup_title = f"{col_y} ({suffix}) by {col_x}"
         else:
             sup_title = f"{col_y} by {col_x}"
 
+        fig, ax = plt.subplots(figsize=(10, 5))
+
         if col_color is not None:
-            fig = px.line(df, x=col_x, y=col_y, color=col_color, title=sup_title, line_shape='linear',
-                          color_discrete_sequence=px.colors.qualitative.Vivid)
+            colors = plt.cm.viridis(np.linspace(0, 1, len(df[col_color].unique())))
+            for i, (group, data) in enumerate(df.groupby(col_color)):
+                ax.plot(data[col_x], data[col_y], label=group, color=colors[i])
+                for x, y, val in zip(data[col_x], data[col_y], data[col_y]):
+                    ax.annotate(f'{val}', (x, y), textcoords="offset points", xytext=(0, 10), ha='center')
         else:
-            fig = px.line(df, x=col_x, y=col_y, title=None, line_shape='linear',
-                          color_discrete_sequence=px.colors.qualitative.Vivid)
+            ax.plot(df[col_x], df[col_y])
+            for x, y, val in zip(df[col_x], df[col_y], df[col_y]):
+                ax.annotate(f'{val}', (x, y), textcoords="offset points", xytext=(0, 10), ha='center')
+
+        ax.set_title(sup_title)
+        ax.set_xlabel(col_x)
+        ax.set_ylabel(col_y)
 
-        fig.update_layout(width=1000, height=500, template='plotly_white', margin=dict(l=10, r=10, b=10, t=40))
         if yticks is not None:
-            tickvals = [float(y_tick) for y_tick in yticks]
-            ticktext = [str(y_tick) for y_tick in yticks]
-            fig.update_yaxes(tickvals=tickvals, ticktext=ticktext)
+            ax.set_yticks(yticks)
         if ylims is not None:
-            fig.update_yaxes(range=ylims)
+            ax.set_ylim(ylims)
 
         if save_plot_name is None:
             file_name = re.sub(r'\([^)]*\)', '', sup_title)
             save_plot_name = f"plot_for_{file_name}.png"
-        # fig.write_image(save_plot_name)
-        fig.show()
+        plt.savefig(save_plot_name)
+        plt.show()
+
+    # def plot_lines(self, column, swap_mode=True, ylims: list = None,
+    #                yticks: list = None, save_plot_name:str=None):
+    #
+    #     df = self._get_data(column)
+    #     mode_dict = self._plot_mode(column, swap_mode)
+    #     col_y = mode_dict.get("col_y")
+    #     col_x = mode_dict.get("col_x")
+    #     col_color = mode_dict.get("col_facet")
+    #
+    #     suffix = self.title_units_dict.get(col_y)
+    #
+    #     if suffix is not None:
+    #         sup_title = f"{col_y} ({suffix}) by {col_x}"
+    #     else:
+    #         sup_title = f"{col_y} by {col_x}"
+    #
+    #     if col_color is not None:
+    #         fig = px.line(df, x=col_x, y=col_y, color=col_color, title=sup_title, line_shape='linear',
+    #                       color_discrete_sequence=px.colors.qualitative.Vivid)
+    #     else:
+    #         fig = px.line(df, x=col_x, y=col_y, title=None, line_shape='linear',
+    #                       color_discrete_sequence=px.colors.qualitative.Vivid)
+    #
+    #     fig.update_layout(width=1000, height=500, template='plotly_white', margin=dict(l=10, r=10, b=10, t=40))
+    #     if yticks is not None:
+    #         tickvals = [float(y_tick) for y_tick in yticks]
+    #         ticktext = [str(y_tick) for y_tick in yticks]
+    #         fig.update_yaxes(tickvals=tickvals, ticktext=ticktext)
+    #     if ylims is not None:
+    #         fig.update_yaxes(range=ylims)
+    #
+    #     if save_plot_name is None:
+    #         file_name = re.sub(r'\([^)]*\)', '', sup_title)
+    #         save_plot_name = f"plot_for_{file_name}.png"
+    #     # fig.write_image(save_plot_name)
+    #     fig.show()
 
 
     def _plot_mode(self, column, swap_mode):
         col_y = column
         col_x = "model"
         col_facet = "label"
 
@@ -240,15 +286,16 @@
 
     def heatmap_scores(self, cmap="cividis", cbar=True, annot=True, save_plot_name:str=None , figsize=(8,10)):
         col_socres = ["maker", "product", "category", "header", "score"]
         data_df = self.df[col_socres].drop_duplicates().replace("", np.nan).dropna()
         data_df["score"] = data_df["score"].map(lambda x: float(x))
         data_df["product"] = data_df["product"].map(lambda x: x.replace("-oled", ""))
         data_df = data_df.pivot(index=["maker", "product"], columns=["category", "header"], values='score')
-        data_df = data_df.T.reset_index().sort_index(axis=1).drop("category", axis=1).set_index("header")
+        # data_df = data_df.T.reset_index().sort_index(axis=1).drop("category", axis=1).set_index("header")
+        data_df = data_df.T.reset_index().sort_index(axis=1, level=0).drop("category", axis=1).set_index("header")
         data_df = data_df.sort_index(axis=1, level=[0, 1])  # Sort the index levels
         plt.figure(figsize=figsize)
         sns.heatmap(data_df, annot=annot, cmap=cmap, cbar=cbar, vmin=0, vmax=10, yticklabels=data_df.index)
         title = "Rtings Score heatmap"
         plt.title(title)
         if save_plot_name is None:
             save_plot_name = f"plot_for_{title}.png"
```

### Comparing `mkt-retv-1.422/market_research/tools/aimanager.py` & `mkt-retv-1.423/market_research/tools/aimanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/tools/filemanager.py` & `mkt-retv-1.423/market_research/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/tools/installer.py` & `mkt-retv-1.423/market_research/tools/installer.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/market_research/tools/webdriver.py` & `mkt-retv-1.423/market_research/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/mkt_retv.egg-info/PKG-INFO` & `mkt-retv-1.423/mkt_retv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkt-retv
-Version: 1.422
+Version: 1.423
 Summary: market research TV 
 Home-page: https://github.com/xikest/research_market_tv
 Author: xikest
 Project-URL: Source, https://github.com/xikest/research_market_tv
 Project-URL: Bug Tracker, https://github.com/xikest/research_market_tv/issues
 Requires-Python: >=3.7
 Requires-Dist: numpy
```

### Comparing `mkt-retv-1.422/mkt_retv.egg-info/SOURCES.txt` & `mkt-retv-1.423/mkt_retv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkt-retv-1.422/setup.py` & `mkt-retv-1.423/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkt-retv',
-    version='1.422',
+    version='1.423',
     author='xikest',
     description='market research TV ',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy', 'pandas',
         'selenium','beautifulsoup4','requests',
```

