# Comparing `tmp/PKNSETools-0.1.20240512.105.tar.gz` & `tmp/PKNSETools-0.1.20240513.106.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PKNSETools-0.1.20240512.105.tar", last modified: Sun May 12 14:07:12 2024, max compression
+gzip compressed data, was "PKNSETools-0.1.20240513.106.tar", last modified: Mon May 13 21:56:18 2024, max compression
```

## Comparing `PKNSETools-0.1.20240512.105.tar` & `PKNSETools-0.1.20240513.106.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/
--rw-rw-rw-   0        0        0     2663 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKNSETools/
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKNSETools/Benny/
--rw-rw-rw-   0        0        0    34274 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/Benny/NSE.py
--rw-rw-rw-   0        0        0     1198 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/Benny/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKNSETools/Nasdaq/
--rw-rw-rw-   0        0        0     3386 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/Nasdaq/PKNasdaqIndex.py
--rw-rw-rw-   0        0        0     1225 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/Nasdaq/__init__.py
--rw-rw-rw-   0        0        0     4806 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKAllStocks.py
--rw-rw-rw-   0        0        0    10770 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKCompanyGeneral.py
--rw-rw-rw-   0        0        0     3303 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKCompanyStock.py
--rw-rw-rw-   0        0        0     2635 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKConstants.py
--rw-rw-rw-   0        0        0    10388 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKIntraDay.py
--rw-rw-rw-   0        0        0    13763 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/PKNSEStockDataFetcher.py
--rw-rw-rw-   0        0        0       31 2024-05-12 14:07:07.000000 PKNSETools-0.1.20240512.105/PKNSETools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/
--rw-rw-rw-   0        0        0     1830 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockDB.py
--rw-rw-rw-   0        0        0     1848 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockFairValueDB.py
--rw-rw-rw-   0        0        0     1836 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockMFIDB.py
--rw-rw-rw-   0        0        0    61961 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
--rw-rw-rw-   0        0        0     1378 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/error.py
--rw-rw-rw-   0        0        0    40060 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/funds.py
--rw-rw-rw-   0        0        0    22038 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/search.py
--rw-rw-rw-   0        0        0    13495 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/security.py
--rw-rw-rw-   0        0        0    29916 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/stock.py
--rw-rw-rw-   0        0        0    23246 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 14:07:12.703636 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/
--rw-rw-rw-   0        0        0     2663 2024-05-12 14:07:12.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2024-05-12 14:07:12.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 14:07:12.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-12 14:07:06.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       79 2024-05-12 14:07:12.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-12 14:07:12.000000 PKNSETools-0.1.20240512.105/PKNSETools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1884 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/README.md
--rw-rw-rw-   0        0        0       86 2024-05-12 14:07:12.719262 PKNSETools-0.1.20240512.105/setup.cfg
--rw-rw-rw-   0        0        0     3832 2024-05-12 14:05:58.000000 PKNSETools-0.1.20240512.105/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/
+-rw-rw-rw-   0        0        0     2663 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools/
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools/Benny/
+-rw-rw-rw-   0        0        0    34274 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Benny/NSE.py
+-rw-rw-rw-   0        0        0     1198 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Benny/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/
+-rw-rw-rw-   0        0        0     3386 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/PKNasdaqIndex.py
+-rw-rw-rw-   0        0        0     1225 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/__init__.py
+-rw-rw-rw-   0        0        0     4806 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKAllStocks.py
+-rw-rw-rw-   0        0        0    10770 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyGeneral.py
+-rw-rw-rw-   0        0        0     3303 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyStock.py
+-rw-rw-rw-   0        0        0     2635 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKConstants.py
+-rw-rw-rw-   0        0        0    10388 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKIntraDay.py
+-rw-rw-rw-   0        0        0    13849 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/PKNSEStockDataFetcher.py
+-rw-rw-rw-   0        0        0       31 2024-05-13 21:56:14.000000 PKNSETools-0.1.20240513.106/PKNSETools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/
+-rw-rw-rw-   0        0        0     1830 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockDB.py
+-rw-rw-rw-   0        0        0     1848 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockFairValueDB.py
+-rw-rw-rw-   0        0        0     1836 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockMFIDB.py
+-rw-rw-rw-   0        0        0    61961 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/PKMorningstarDataFetcher.py
+-rw-rw-rw-   0        0        0     1378 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/error.py
+-rw-rw-rw-   0        0        0    40060 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/funds.py
+-rw-rw-rw-   0        0        0    22038 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/search.py
+-rw-rw-rw-   0        0        0    13495 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/security.py
+-rw-rw-rw-   0        0        0    29916 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/stock.py
+-rw-rw-rw-   0        0        0    23246 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 21:56:18.808617 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/
+-rw-rw-rw-   0        0        0     2663 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-13 21:56:12.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       79 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 21:56:18.000000 PKNSETools-0.1.20240513.106/PKNSETools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1884 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-13 21:56:18.824237 PKNSETools-0.1.20240513.106/setup.cfg
+-rw-rw-rw-   0        0        0     3832 2024-05-13 21:55:01.000000 PKNSETools-0.1.20240513.106/setup.py
```

### Comparing `PKNSETools-0.1.20240512.105/PKG-INFO` & `PKNSETools-0.1.20240513.106/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240512.105
+Version: 0.1.20240513.106
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240512.105.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240513.106.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/Benny/NSE.py` & `PKNSETools-0.1.20240513.106/PKNSETools/Benny/NSE.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/Benny/__init__.py` & `PKNSETools-0.1.20240513.106/PKNSETools/Benny/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/Nasdaq/PKNasdaqIndex.py` & `PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/PKNasdaqIndex.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/Nasdaq/__init__.py` & `PKNSETools-0.1.20240513.106/PKNSETools/Nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKAllStocks.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKAllStocks.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKCompanyGeneral.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyGeneral.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKCompanyStock.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKCompanyStock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKConstants.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKConstants.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKIntraDay.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKIntraDay.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/PKNSEStockDataFetcher.py` & `PKNSETools-0.1.20240513.106/PKNSETools/PKNSEStockDataFetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
             11: "https://archives.nseindia.com/content/indices/ind_niftymidcap150list.csv",
             14: "https://archives.nseindia.com/content/fo/fo_mktlots.csv",
         }
 
         url = tickerMapping.get(tickerOption)
 
         try:
-            res = self.fetchURL(url)
+            headers = {"user-agent": random_user_agent()}
+            res = self.fetchURL(url,headers=headers,timeout=10)
             if res is None or res.status_code != 200:
                 return listStockCodes
             cr = csv.reader(res.text.strip().split("\n"))
 
             if tickerOption == 14:
                 for i in range(5):
                     next(cr)  # skipping first line
```

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockDB.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockFairValueDB.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockFairValueDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/NSEStockMFIDB.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/NSEStockMFIDB.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/PKMorningstarDataFetcher.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/PKMorningstarDataFetcher.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/__init__.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/__init__.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/error.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/error.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/funds.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/funds.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/search.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/search.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/security.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/security.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/stock.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/stock.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools/morningstartools/utils.py` & `PKNSETools-0.1.20240513.106/PKNSETools/morningstartools/utils.py`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools.egg-info/PKG-INFO` & `PKNSETools-0.1.20240513.106/PKNSETools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: PKNSETools
-Version: 0.1.20240512.105
+Version: 0.1.20240513.106
 Summary: A Python-based data downloader for NSE, India
 Home-page: https://github.com/pkjmesra/PKNSETools
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240512.105.zip
+Download-URL: https://github.com/pkjmesra/PKNSETools/archive/v0.1.20240513.106.zip
 Keywords: NSE,Stocks,Data Download
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
```

### Comparing `PKNSETools-0.1.20240512.105/PKNSETools.egg-info/SOURCES.txt` & `PKNSETools-0.1.20240513.106/PKNSETools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/README.md` & `PKNSETools-0.1.20240513.106/README.md`

 * *Files identical despite different names*

### Comparing `PKNSETools-0.1.20240512.105/setup.py` & `PKNSETools-0.1.20240513.106/setup.py`

 * *Files identical despite different names*

