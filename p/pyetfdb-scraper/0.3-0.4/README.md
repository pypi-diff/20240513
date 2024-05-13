# Comparing `tmp/pyetfdb_scraper-0.3.tar.gz` & `tmp/pyetfdb_scraper-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyetfdb_scraper-0.3.tar", last modified: Fri Apr  5 10:39:22 2024, max compression
+gzip compressed data, was "pyetfdb_scraper-0.4.tar", last modified: Mon May 13 03:02:59 2024, max compression
```

## Comparing `pyetfdb_scraper-0.3.tar` & `pyetfdb_scraper-0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.756721 pyetfdb_scraper-0.3/
--rw-r--r--   0 lohyikuang   (501) staff       (20)    35148 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/LICENSE
--rw-r--r--   0 lohyikuang   (501) staff       (20)       49 2024-04-05 10:32:32.000000 pyetfdb_scraper-0.3/MANIFEST.in
--rw-r--r--   0 lohyikuang   (501) staff       (20)    22764 2024-04-05 10:39:22.755588 pyetfdb_scraper-0.3/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)    22345 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/README.md
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1040 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/pyproject.toml
--rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2024-04-05 10:39:22.756990 pyetfdb_scraper-0.3/setup.cfg
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1193 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/setup.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.720262 pyetfdb_scraper-0.3/src/
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.726622 pyetfdb_scraper-0.3/src/pyetfdb_scraper/
--rw-r--r--   0 lohyikuang   (501) staff       (20)       19 2024-04-05 10:30:36.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/__init__.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.737279 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/
--rw-r--r--   0 lohyikuang   (501) staff       (20)   567933 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/etfdb.json
--rw-r--r--   0 lohyikuang   (501) staff       (20)   110530 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/user-agents.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)     2010 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     3902 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf_scraper.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.740463 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      120 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      360 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/expense.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1792 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/info.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.751258 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/
--rw-r--r--   0 lohyikuang   (501) staff       (20)      473 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/__init__.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      855 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/dividend.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1669 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/expense.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      939 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holding_analysis.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     5175 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holdings.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)    11489 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/info.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1152 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/performance.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)      544 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/realtime_ratings.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     1408 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/technicals.py
--rw-r--r--   0 lohyikuang   (501) staff       (20)     4800 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper/utils.py
-drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-04-05 10:39:22.752701 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/
--rw-r--r--   0 lohyikuang   (501) staff       (20)    22764 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/PKG-INFO
--rw-r--r--   0 lohyikuang   (501) staff       (20)      928 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/SOURCES.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/dependency_links.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       37 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/requires.txt
--rw-r--r--   0 lohyikuang   (501) staff       (20)       16 2024-04-05 10:39:22.000000 pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/top_level.txt
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.463855 pyetfdb_scraper-0.4/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    35148 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/LICENSE
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       49 2024-04-05 10:32:32.000000 pyetfdb_scraper-0.4/MANIFEST.in
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22642 2024-05-13 03:02:59.463130 pyetfdb_scraper-0.4/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22345 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/README.md
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1040 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/pyproject.toml
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       38 2024-05-13 03:02:59.464015 pyetfdb_scraper-0.4/setup.cfg
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1229 2024-05-10 08:17:54.000000 pyetfdb_scraper-0.4/setup.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.435473 pyetfdb_scraper-0.4/src/
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.439252 pyetfdb_scraper-0.4/src/pyetfdb_scraper/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       20 2024-05-13 03:02:50.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/__init__.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.449159 pyetfdb_scraper-0.4/src/pyetfdb_scraper/data/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)   567933 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/data/etfdb.json
+-rw-r--r--   0 lohyikuang   (501) staff       (20)   110530 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/data/user-agents.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     2010 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/etf.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     3902 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/etf_scraper.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.453326 pyetfdb_scraper-0.4/src/pyetfdb_scraper/models/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      120 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/models/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      360 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/models/expense.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1792 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/models/info.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.461499 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      473 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/__init__.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      855 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/dividend.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1669 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/expense.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      939 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/holding_analysis.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     5175 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/holdings.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    11489 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/info.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1152 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/performance.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      544 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/realtime_ratings.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     1408 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/technicals.py
+-rw-r--r--   0 lohyikuang   (501) staff       (20)     4800 2024-04-05 10:26:56.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper/utils.py
+drwxr-xr-x   0 lohyikuang   (501) staff       (20)        0 2024-05-13 03:02:59.441044 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/
+-rw-r--r--   0 lohyikuang   (501) staff       (20)    22642 2024-05-13 03:02:59.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/PKG-INFO
+-rw-r--r--   0 lohyikuang   (501) staff       (20)      928 2024-05-13 03:02:59.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/SOURCES.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)        1 2024-05-13 03:02:59.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/dependency_links.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       51 2024-05-13 03:02:59.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/requires.txt
+-rw-r--r--   0 lohyikuang   (501) staff       (20)       16 2024-05-13 03:02:59.000000 pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/top_level.txt
```

### Comparing `pyetfdb_scraper-0.3/LICENSE` & `pyetfdb_scraper-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/PKG-INFO` & `pyetfdb_scraper-0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
 Name: pyetfdb_scraper
-Version: 0.3
+Version: 0.4
 Summary: Scrape ETFs from ETFDB
 Home-page: https://github.com/lvxhnat/pyetf-scraper
 Author: Yi Kuang
 Author-email: yikuang5@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: bs4
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
+License-File: LICENSE
 
 # pyetfdb_scraper: Free ETF data at your fingertips
 ```pyetfdb_scraper``` is a Python library for extracting ETF data directly from [ETFDB](https://etfdb.com/), a website providing one of the largest ETF Databases containing ETFs from a vast range of asset classes, industries, issuers, and investment styles.
 
 ## Quick Start
 Install with ```pip``` as a package pip. See the pip package here https://pypi.org/project/pyetfdb-scraper/.
```

### Comparing `pyetfdb_scraper-0.3/README.md` & `pyetfdb_scraper-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/pyproject.toml` & `pyetfdb_scraper-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/setup.py` & `pyetfdb_scraper-0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,12 +32,14 @@
     long_description_content_type="text/markdown",
     url="https://github.com/lvxhnat/pyetf-scraper",
     package_dir={"": "src"},
     packages=find_packages("src", exclude=["*tests"]),
     package_data={name: ["data/etfdb.json", "data/user-agents.txt"]},
     python_requires=">=3.7",
     install_requires=[
+        "pydantic",
         "requests",
         "bs4",
+        "lxml",
     ],
     extras_require={"dev": list(dev_requirements)},
 )
```

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/etfdb.json` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/data/etfdb.json`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/data/user-agents.txt` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/data/user-agents.txt`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/etf.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/etf_scraper.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/etf_scraper.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/models/info.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/models/info.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/dividend.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/dividend.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/expense.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/expense.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holding_analysis.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/holding_analysis.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/holdings.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/holdings.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/info.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/info.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/performance.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/performance.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/realtime_ratings.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/realtime_ratings.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/tabs/technicals.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/tabs/technicals.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper/utils.py` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/PKG-INFO` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 Metadata-Version: 2.1
-Name: pyetfdb_scraper
-Version: 0.3
+Name: pyetfdb-scraper
+Version: 0.4
 Summary: Scrape ETFs from ETFDB
 Home-page: https://github.com/lvxhnat/pyetf-scraper
 Author: Yi Kuang
 Author-email: yikuang5@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: bs4
 Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
+License-File: LICENSE
 
 # pyetfdb_scraper: Free ETF data at your fingertips
 ```pyetfdb_scraper``` is a Python library for extracting ETF data directly from [ETFDB](https://etfdb.com/), a website providing one of the largest ETF Databases containing ETFs from a vast range of asset classes, industries, issuers, and investment styles.
 
 ## Quick Start
 Install with ```pip``` as a package pip. See the pip package here https://pypi.org/project/pyetfdb-scraper/.
```

### Comparing `pyetfdb_scraper-0.3/src/pyetfdb_scraper.egg-info/SOURCES.txt` & `pyetfdb_scraper-0.4/src/pyetfdb_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

