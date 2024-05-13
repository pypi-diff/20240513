# Comparing `tmp/fundus-0.3.0.tar.gz` & `tmp/fundus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fundus-0.3.0.tar", last modified: Sun Apr 21 19:42:17 2024, max compression
+gzip compressed data, was "fundus-0.3.1.tar", last modified: Mon May 13 11:28:40 2024, max compression
```

## Comparing `fundus-0.3.0.tar` & `fundus-0.3.1.tar`

### file list

```diff
@@ -1,105 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-21 19:42:13.000000 fundus-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-21 19:42:13.000000 fundus-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-21 19:42:17.625123 fundus-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-21 19:42:13.000000 fundus-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-21 19:42:13.000000 fundus-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:42:17.625123 fundus-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.609123 fundus-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.609123 fundus-0.3.0/src/fundus/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12059 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/parser/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/at/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/at/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/at/orf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8394 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/base_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.613123 fundus-0.3.0/src/fundus/publishers/ch/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/ch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/ch/srf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/de/
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/berliner_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/bild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/braunschweiger_zeitung.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/business_insider_de.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/die_welt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/die_zeit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/dw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/faz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/focus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/mdr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/merkur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/ndr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/ntv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/rheinische_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/spon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/stern.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/sz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/tagesschau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/taz.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/de/waz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/fr/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/fr/le_monde.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/lt/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/lt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/lt/lrt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/na/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/na/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/na/the_namibian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.617123 fundus-0.3.0/src/fundus/publishers/uk/
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/i_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_guardian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/uk/the_telegraph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/publishers/us/
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/ap_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/business_insider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/cnbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/fox_news.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/free_beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/la_times.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/occupy_democrats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/reuters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_gateway_pundit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_intercept.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_nation_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/the_new_yorker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/washington_times_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/publishers/us/world_truth.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/scraping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/article.py
--rw-r--r--   0 runner    (1001) docker     (127)    18725 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/scraper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/scraping/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.621123 fundus-0.3.0/src/fundus/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-21 19:42:13.000000 fundus-0.3.0/src/fundus/utils/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/src/fundus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9082 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 19:42:17.000000 fundus-0.3.0/src/fundus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:42:17.625123 fundus-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9663 2024-04-21 19:42:13.000000 fundus-0.3.0/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.565196 fundus-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 11:28:36.000000 fundus-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 11:28:36.000000 fundus-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-13 11:28:40.565196 fundus-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-13 11:28:36.000000 fundus-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-13 11:28:36.000000 fundus-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:28:40.565196 fundus-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.541196 fundus-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/parser/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/parser/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/publishers/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/publishers/at/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/at/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/at/derstandard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/at/orf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/publishers/au/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/au/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/au/nine_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/base_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/publishers/ch/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/ch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/ch/srf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.545196 fundus-0.3.1/src/fundus/publishers/cn/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/cn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/cn/people.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.553196 fundus-0.3.1/src/fundus/publishers/de/
+-rw-r--r--   0 runner    (1001) docker     (127)    18504 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/berliner_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/bild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/boersenzeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/br.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/braunschweiger_zeitung.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/business_insider_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/die_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/die_zeit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/dw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/faz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/focus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/frankfurter_rundschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/freiepresse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/gamestar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/hamburger_abendblatt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/hessenschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/junge_welt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/kicker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/mdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/merkur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/morgenpost_berlin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/motorsport_magazin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/mz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/ndr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/netzpolitik_org.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/ntv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/postillon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/rbb24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/rheinische_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/rn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/spon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/sportschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/stern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/sz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/tagesschau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/tagesspiegel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/taz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/vogue_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/waz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/wdr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/winfuture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/de/zdf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.553196 fundus-0.3.1/src/fundus/publishers/fr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/fr/le_figaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/fr/le_monde.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.553196 fundus-0.3.1/src/fundus/publishers/lt/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/lt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/lt/lrt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.557196 fundus-0.3.1/src/fundus/publishers/my/
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/my/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/my/malay_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.557196 fundus-0.3.1/src/fundus/publishers/na/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/na/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/na/the_namibian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.557196 fundus-0.3.1/src/fundus/publishers/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/shared/euronews.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.557196 fundus-0.3.1/src/fundus/publishers/tr/
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/tr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/tr/haberturk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/tr/ntvtr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.557196 fundus-0.3.1/src/fundus/publishers/uk/
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/daily_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/daily_star.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/evening_standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/i_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/the_guardian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/the_independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/the_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/the_sun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/uk/the_telegraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.561196 fundus-0.3.1/src/fundus/publishers/us/
+-rw-r--r--   0 runner    (1001) docker     (127)     8304 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/ap_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/business_insider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/cnbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/fox_news.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/free_beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/la_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/occupy_democrats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/reuters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/rolling_stone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/techcrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/the_gateway_pundit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/the_intercept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/the_nation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/the_new_yorker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/voice_of_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/washington_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/washington_times_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/wired.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/publishers/us/world_truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.561196 fundus-0.3.1/src/fundus/scraping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19097 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/scraper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/scraping/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.561196 fundus-0.3.1/src/fundus/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-13 11:28:36.000000 fundus-0.3.1/src/fundus/utils/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.565196 fundus-0.3.1/src/fundus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9075 2024-05-13 11:28:40.000000 fundus-0.3.1/src/fundus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-13 11:28:40.000000 fundus-0.3.1/src/fundus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:28:40.000000 fundus-0.3.1/src/fundus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-13 11:28:40.000000 fundus-0.3.1/src/fundus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 11:28:40.000000 fundus-0.3.1/src/fundus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:28:40.565196 fundus-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-13 11:28:36.000000 fundus-0.3.1/tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 11:28:36.000000 fundus-0.3.1/tests/test_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-13 11:28:36.000000 fundus-0.3.1/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-13 11:28:36.000000 fundus-0.3.1/tests/test_parser.py
```

### Comparing `fundus-0.3.0/LICENSE` & `fundus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/PKG-INFO` & `fundus-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: more-itertools<10,>=9.1
 Requires-Dist: cssselect<2,>=1.1
 Requires-Dist: feedparser<7,>=6.0
 Requires-Dist: colorama<1,>=0.4
 Requires-Dist: typing-extensions<5,>=4.6
 Requires-Dist: langdetect<2,>=1.0
-Requires-Dist: validators!=0.23,<1,>=0.20
+Requires-Dist: validators<1,>=0.24
 Requires-Dist: requests<3,>=2.28
 Requires-Dist: tqdm<5,>=4.66
 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2
 Requires-Dist: dill<1,>=0.3
 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev"
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.3.0 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.3.1 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9 Requires-Dist: more-itertools<10,>=9.1 Requires-
 Dist: cssselect<2,>=1.1 Requires-Dist: feedparser<7,>=6.0 Requires-Dist:
 colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.6 Requires-Dist:
-langdetect<2,>=1.0 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
+langdetect<2,>=1.0 Requires-Dist: validators<1,>=0.24 Requires-Dist:
 requests<3,>=2.28 Requires-Dist: tqdm<5,>=4.66 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2 Requires-Dist: dill<1,>=0.3 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.9.0; extra
 == "dev" Requires-Dist: isort==5.12.0; extra == "dev" Requires-Dist:
 black==23.1.0; extra == "dev" Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev" Requires-Dist:
 types-requests<3,>=2.28; extra == "dev" Requires-Dist: types-colorama<1,>=0.4;
```

### Comparing `fundus-0.3.0/README.md` & `fundus-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/pyproject.toml` & `fundus-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fundus"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "Max Dallabetta", email = "max.dallabetta@googlemail.com" },
 ]
 description = "A very simple news crawler"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -27,15 +27,15 @@
     "lxml>=4.9, <5",
     "more-itertools>=9.1, <10",
     "cssselect>=1.1, <2",
     "feedparser>=6.0, <7",
     "colorama>=0.4, <1",
     "typing-extensions>=4.6, <5",
     "langdetect>=1.0, <2",
-    "validators>=0.20, <1, !=0.23",
+    "validators>=0.24, <1",
     "requests>=2.28, <3",
     "tqdm>=4.66, <5",
     "fastwarc>=0.14, <1",
     "chardet>=5.2, <6",
     "dill>=0.3, <1"
 ]
```

### Comparing `fundus-0.3.0/src/fundus/parser/base_parser.py` & `fundus-0.3.1/src/fundus/parser/base_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,17 @@
         elif other.priority is None:
             return True
         else:
             return self.priority < other.priority
 
     def __repr__(self):
         if instance := self.__self__:
-            return f"bound {type(self).__name__} of {instance}: {self.__wrapped__} --> '{self.__name__}'"
+            return f"bound {type(self).__name__} of {instance}: {self.__wrapped__} --> {self.__name__!r}"
         else:
-            return f"registered {type(self).__name__}: {self.__wrapped__} --> '{self.__name__}'"
+            return f"registered {type(self).__name__}: {self.__wrapped__} --> {self.__name__!r}"
 
 
 class Attribute(RegisteredFunction):
     def __init__(self, func: Callable[[object], Any], priority: Optional[int], validate: bool):
         self.validate = validate
         super(Attribute, self).__init__(func=func, priority=priority)
 
@@ -211,15 +211,15 @@
                     parsed_data[attribute_name] = func()
                 except Exception as err:
                     if error_handling == "catch":
                         parsed_data[attribute_name] = err
                     elif error_handling == "suppress" or error_handling == "raise":
                         raise err
                     else:
-                        raise ValueError(f"Invalid value '{error_handling}' for parameter <error_handling>")
+                        raise ValueError(f"Invalid value {error_handling!r} for parameter <error_handling>")
 
             else:
                 raise TypeError(f"Invalid type for {func}. Only subclasses of 'RegisteredFunction' are allowed")
 
         return parsed_data
 
     def share(self, **kwargs):
@@ -270,16 +270,16 @@
             )
 
         mapping: Dict[date, _ParserCache] = {}
         for versioned_parser in sorted(included_parsers, key=lambda parser: parser.VALID_UNTIL):
             validation_date: date
             if prev := mapping.get(validation_date := versioned_parser.VALID_UNTIL):  # type: ignore
                 raise ValueError(
-                    f"Found versions '{prev.factory.__name__}' and '{versioned_parser.__name__}' of "
-                    f"'{self}' with same validation date.\nMake sure you use class attribute VALID_UNTIL "
+                    f"Found versions {prev.factory.__name__!r} and {versioned_parser.__name__!r} of "
+                    f"{str(self)!r} with same validation date.\nMake sure you use class attribute VALID_UNTIL "
                     f"of <class {BaseParser.__name__}> to set validation dates for legacy versions."
                 )
             mapping[validation_date] = _ParserCache(versioned_parser)
         self._parser_mapping = mapping
 
     def __call__(self, crawl_date: Optional[Union[datetime, date]] = None) -> BaseParser:
         if crawl_date is None:
@@ -311,15 +311,16 @@
         return bool(self._parser_mapping)
 
     def __str__(self) -> str:
         return f"<{ParserProxy.__name__} {type(self).__name__}>"
 
     def __repr__(self) -> str:
         return (
-            f"{type(self).__name__} including versions '{', '.join([cache.factory.__name__ for cache in self._parser_mapping.values()])}'"
+            f"{type(self).__name__} including versions "
+            f"{', '.join([cache.factory.__name__ for cache in self._parser_mapping.values()])!r}"
             if self._parser_mapping
             else f"Empty {type(self).__name__}"
         )
 
     @property
     def attribute_mapping(self) -> Dict[Type[BaseParser], AttributeCollection]:
         return {versioned_parser: versioned_parser.attributes() for versioned_parser in self}
```

### Comparing `fundus-0.3.0/src/fundus/parser/data.py` & `fundus-0.3.1/src/fundus/parser/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
         if result == _sentinel:
             return default
 
         return result
 
     def __repr__(self):
-        return f"LD containing '{', '.join(content)}'" if (content := self.__dict__.keys()) else "Empty LD"
+        return f"LD containing {', '.join(content)!r}" if (content := self.__dict__.keys()) else "Empty LD"
 
 
 class TextSequence(Sequence[str]):
     def __init__(self, texts: Iterable[str]):
         self._data: Tuple[str, ...] = tuple(texts)
 
     @overload
@@ -240,14 +240,17 @@
             "paragraphs": list(self.paragraphs),
         }
 
     @classmethod
     def deserialize(cls, serialized: Dict[str, Any]) -> Self:
         return cls(headline=TextSequence(serialized["headline"]), paragraphs=TextSequence(serialized["paragraphs"]))
 
+    def __bool__(self):
+        return bool(self.paragraphs)
+
 
 @dataclass
 class ArticleBody(TextSequenceTree):
     summary: TextSequence
     sections: List[ArticleSection]
 
     def serialize(self) -> Dict[str, Any]:
@@ -258,7 +261,10 @@
 
     @classmethod
     def deserialize(cls, serialized: Dict[str, Any]) -> Self:
         return cls(
             summary=TextSequence(serialized["summary"]),
             sections=[ArticleSection.deserialize(section) for section in serialized["sections"]],
         )
+
+    def __bool__(self):
+        return any(bool(section) for section in self.sections)
```

### Comparing `fundus-0.3.0/src/fundus/parser/utility.py` & `fundus-0.3.1/src/fundus/parser/utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
     def __hash__(self) -> int:
         return hash(self.position)
 
     def __str__(self) -> str:
         return self.text_content()
 
+    def __repr__(self):
+        return f"{type(self).__name__}: {self.text_content()}"
+
     def __bool__(self):
         return bool(normalize_whitespace(self.text_content()))
 
 
 class SummaryNode(Node):
     pass
 
@@ -113,14 +116,18 @@
         # return empty body if no text is present
         return ArticleBody(TextSequence([]), [])
 
     instructions = more_itertools.split_when(nodes, pred=lambda x, y: type(x) != type(y))
 
     if not summary_nodes:
         instructions = more_itertools.prepend([], instructions)
+    elif not nodes[: len(summary_nodes)] == summary_nodes:
+        raise ValueError(
+            f"The summary should be at the beginning of the article, but extracted article starts with '{nodes[0]!r}'"
+        )
 
     if not subhead_nodes or (paragraph_nodes and subhead_nodes[0] > paragraph_nodes[0]):
         first = next(instructions)
         instructions = itertools.chain([first, []], instructions)
 
     summary = TextSequence(
         map(lambda x: normalize_whitespace(x.text_content(excluded_tags=["script"])), next(instructions))
@@ -188,37 +195,53 @@
         value:      An input value representing author(s) which get parsed based on type
         split_on:   Only relevant for type(<value>) = str. If set, split <value> on <split_on>,
             else (default) split <value> on common delimiters
 
     Returns:
         A parsed and striped list of authors
     """
+
+    def parse_author_dict(author_dict: Dict[str, str]) -> Optional[str]:
+        if (author_name := author_dict.get("name")) is not None:
+            return author_name
+
+        given_name = author_dict.get("givenName", "")
+        additional_name = author_dict.get("additionalName", "")
+        family_name = author_dict.get("familyName", "")
+        if given_name and family_name:
+            return " ".join(filter(bool, [given_name, additional_name, family_name]))
+        else:
+            return None
+
     if not value:
         return []
 
     parameter_type_error: TypeError = TypeError(
         f"<value> '{value}' has an unsupported type {type(value)}. "
         f"Supported types are 'Optional[str], Dict[str, str], List[str], List[Dict[str, str]],'"
     )
 
     if isinstance(value, str):
         common_delimiters = [",", ";", " und ", " and "]
         authors = list(filter(bool, re.split(r"|".join(split_on or common_delimiters), value)))
 
     elif isinstance(value, dict):
-        authors = [name] if (name := value.get("name")) else []
+        if author := parse_author_dict(value):
+            return [author]
+        else:
+            return []
 
     elif isinstance(value, list):
         if isinstance(value[0], str):
             value = cast(List[str], value)
             authors = value
 
         elif isinstance(value[0], dict):
             value = cast(List[Dict[str, str]], value)
-            authors = [name for author in value if (name := author.get("name"))]
+            authors = [name for author in value if (name := parse_author_dict(author))]
 
         else:
             raise parameter_type_error
 
     else:
         raise parameter_type_error
 
@@ -229,20 +252,20 @@
 
 def generic_text_extraction_with_css(doc, selector: XPath) -> Optional[str]:
     nodes = selector(doc)
     return strip_nodes_to_text(nodes)
 
 
 def generic_topic_parsing(keywords: Optional[Union[str, List[str]]], delimiter: str = ",") -> List[str]:
-    if isinstance(keywords, str):
-        return [keyword.strip() for keyword in keywords.split(delimiter)]
+    if not keywords:
+        return []
+    elif isinstance(keywords, str):
+        return [cleaned for keyword in keywords.split(delimiter) if (cleaned := keyword.strip())]
     elif isinstance(keywords, list) and all(isinstance(s, str) for s in keywords):
         return keywords
-    elif keywords is None:
-        return []
     else:
         raise TypeError(f"Encountered unexpected type {type(keywords)} as keyword parameter")
 
 
 _tz_infos = {"CET": 3600, "CEST": 7200}
```

### Comparing `fundus-0.3.0/src/fundus/publishers/__init__.py` & `fundus-0.3.1/src/fundus/publishers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from fundus.publishers.at import AT
+from fundus.publishers.au import AU
 from fundus.publishers.base_objects import PublisherCollectionMeta
 from fundus.publishers.ch import CH
+from fundus.publishers.cn import CN
 from fundus.publishers.de import DE
 from fundus.publishers.fr import FR
 from fundus.publishers.lt import LT
+from fundus.publishers.my import MY
 from fundus.publishers.na import NA
+from fundus.publishers.tr import TR
 from fundus.publishers.uk import UK
 from fundus.publishers.us import US
 
 
 class PublisherCollection(metaclass=PublisherCollectionMeta):
     na = NA
     de = DE
     at = AT
+    au = AU
     us = US
     uk = UK
     fr = FR
     ch = CH
     lt = LT
+    cn = CN
+    tr = TR
+    my = MY
```

### Comparing `fundus-0.3.0/src/fundus/publishers/at/orf.py` & `fundus-0.3.1/src/fundus/publishers/at/orf.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/base_objects.py` & `fundus-0.3.1/src/fundus/publishers/base_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,32 +55,32 @@
             NewsMap: [],
             Sitemap: [],
         }
 
         for url_source in spec.sources:
             if not isinstance(url_source, URLSource):
                 raise TypeError(
-                    f"Unexpected type '{type(url_source).__name__}' as source for {self.name}. "
-                    f"Allowed are '{', '.join(cls.__name__ for cls in iterate_all_subclasses(URLSource))}'"
+                    f"Unexpected type {type(url_source).__name__!r} as source for {self!r}. "
+                    f"Allowed are {', '.join(repr(cls.__name__) for cls in iterate_all_subclasses(URLSource))}"
                 )
             source_mapping[type(url_source)].append(url_source)
 
         self.source_mapping = source_mapping
 
     def __str__(self) -> str:
         return f"{self.publisher_name}"
 
     def supports(self, source_types: List[Type[URLSource]]) -> bool:
         if not source_types:
             raise ValueError(f"Got empty value '{source_types}' for parameter <source_types>.")
         for source_type in source_types:
             if not inspect.isclass(source_type) or not issubclass(source_type, URLSource):
                 raise TypeError(
-                    f"Got unexpected type '{source_type}'. "
-                    f"Allowed are '{', '.join(cls.__name__ for cls in iterate_all_subclasses(URLSource))}'"
+                    f"Got unexpected type {source_type!r}. "
+                    f"Allowed are {', '.join(repr(cls.__name__) for cls in iterate_all_subclasses(URLSource))}"
                 )
         return all(bool(self.source_mapping.get(source_type)) for source_type in source_types)
 
     @classmethod
     def search(
         cls, attributes: Optional[List[str]] = None, source_types: Optional[List[Type[URLSource]]] = None
     ) -> List["PublisherEnum"]:
@@ -133,15 +133,15 @@
     def __new__(mcs, name, bases, attrs):
         included_enums: List[EnumMeta] = [value for value in attrs.values() if mcs._is_publisher_enum(value)]
         publisher_mapping: Dict[str, PublisherEnum] = {}
         for country_enum in included_enums:
             for publisher_enum in country_enum:  # type: ignore
                 if existing := publisher_mapping.get(publisher_enum.name):
                     raise AttributeError(
-                        f"Found duplicate publisher names in same collection '{name}'. "
+                        f"Found duplicate publisher names in same collection {name!r}: "
                         f"{type(existing).__name__} -> {existing.name} and "
                         f"{type(publisher_enum).__name__} -> {publisher_enum.name}"
                     )
                 publisher_mapping[publisher_enum.name] = publisher_enum
         return super().__new__(mcs, name, bases, attrs)
 
     def get_publisher_enum_mapping(cls) -> Dict[str, EnumMeta]:
@@ -190,15 +190,15 @@
         Returns:
             PublisherEnum: The corresponding publisher.
 
         """
         for publisher_enum in self:
             if publisher_enum.name == name:
                 return publisher_enum
-        raise KeyError(f"Publisher '{name}' not present in {self.__name__}")
+        raise KeyError(f"Publisher {name!r} not present in {self.__name__}")
 
     def __len__(cls) -> int:
         """The number of publishers included in the collection.
 
         Returns:
             int: The number of publishers.
         """
```

### Comparing `fundus-0.3.0/src/fundus/publishers/ch/__init__.py` & `fundus-0.3.1/src/fundus/publishers/ch/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/ch/srf.py` & `fundus-0.3.1/src/fundus/publishers/ch/srf.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/berliner_zeitung.py` & `fundus-0.3.1/src/fundus/publishers/de/berliner_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/bild.py` & `fundus-0.3.1/src/fundus/publishers/de/bild.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/braunschweiger_zeitung.py` & `fundus-0.3.1/src/fundus/publishers/de/braunschweiger_zeitung.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/business_insider_de.py` & `fundus-0.3.1/src/fundus/publishers/de/business_insider_de.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/die_welt.py` & `fundus-0.3.1/src/fundus/publishers/de/die_welt.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/die_zeit.py` & `fundus-0.3.1/src/fundus/publishers/de/die_zeit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/dw.py` & `fundus-0.3.1/src/fundus/publishers/de/dw.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/faz.py` & `fundus-0.3.1/src/fundus/publishers/de/faz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/focus.py` & `fundus-0.3.1/src/fundus/publishers/de/focus.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/mdr.py` & `fundus-0.3.1/src/fundus/publishers/de/mdr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/merkur.py` & `fundus-0.3.1/src/fundus/publishers/de/merkur.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/ndr.py` & `fundus-0.3.1/src/fundus/publishers/de/ndr.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/ntv.py` & `fundus-0.3.1/src/fundus/publishers/de/ntv.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/rheinische_post.py` & `fundus-0.3.1/src/fundus/publishers/de/rheinische_post.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/spon.py` & `fundus-0.3.1/src/fundus/publishers/de/spon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/stern.py` & `fundus-0.3.1/src/fundus/publishers/de/stern.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/sz.py` & `fundus-0.3.1/src/fundus/publishers/de/sz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/tagesschau.py` & `fundus-0.3.1/src/fundus/publishers/de/tagesschau.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/taz.py` & `fundus-0.3.1/src/fundus/publishers/de/taz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/de/waz.py` & `fundus-0.3.1/src/fundus/publishers/de/waz.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/fr/le_monde.py` & `fundus-0.3.1/src/fundus/publishers/fr/le_monde.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/lt/lrt.py` & `fundus-0.3.1/src/fundus/publishers/lt/lrt.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/na/__init__.py` & `fundus-0.3.1/src/fundus/publishers/na/__init__.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/na/the_namibian.py` & `fundus-0.3.1/src/fundus/publishers/na/the_namibian.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/uk/i_news.py` & `fundus-0.3.1/src/fundus/publishers/uk/i_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/uk/the_guardian.py` & `fundus-0.3.1/src/fundus/publishers/uk/the_guardian.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/uk/the_independent.py` & `fundus-0.3.1/src/fundus/publishers/uk/the_independent.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/uk/the_telegraph.py` & `fundus-0.3.1/src/fundus/publishers/uk/the_telegraph.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/__init__.py` & `fundus-0.3.1/src/fundus/publishers/us/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from fundus.publishers.base_objects import PublisherEnum, PublisherSpec
-from fundus.scraping.filter import inverse, regex_filter
+from fundus.scraping.filter import inverse, lor, regex_filter
 from fundus.scraping.url import NewsMap, RSSFeed, Sitemap
 
 from .ap_news import APNewsParser
 from .business_insider import BusinessInsiderParser
 from .cnbc import CNBCParser
 from .fox_news import FoxNewsParser
 from .free_beacon import FreeBeaconParser
 from .la_times import LATimesParser
 from .occupy_democrats import OccupyDemocratsParser
 from .reuters import ReutersParser
+from .rolling_stone import RollingStoneParser
+from .techcrunch import TechCrunchParser
 from .the_gateway_pundit import TheGatewayPunditParser
 from .the_intercept import TheInterceptParser
 from .the_nation_parser import TheNationParser
 from .the_new_yorker import TheNewYorkerParser
+from .voice_of_america import VOAParser
+from .washington_post import WashingtonPostParser
 from .washington_times_parser import WashingtonTimesParser
+from .wired import WiredParser
 from .world_truth import WorldTruthParser
 
 
 class US(PublisherEnum):
     APNews = PublisherSpec(
         name="Associated Press News",
         domain="https://apnews.com/",
@@ -36,14 +41,28 @@
     CNBC = PublisherSpec(
         name="CNBC",
         domain="https://www.cnbc.com/",
         sources=[Sitemap("https://www.cnbc.com/sitemapAll.xml"), NewsMap("https://www.cnbc.com/sitemap_news.xml")],
         parser=CNBCParser,
     )
 
+    TechCrunch = PublisherSpec(
+        name="TechCrunch",
+        domain="https://techcrunch.com/",
+        sources=[
+            Sitemap(
+                "https://techcrunch.com/sitemap_index.xml",
+                sitemap_filter=inverse(regex_filter("post-sitemap")),
+                reverse=True,
+            ),
+            NewsMap("https://techcrunch.com/news-sitemap.xml"),
+        ],
+        parser=TechCrunchParser,
+    )
+
     TheIntercept = PublisherSpec(
         name="The Intercept",
         domain="https://theintercept.com/",
         sources=[
             RSSFeed("https://theintercept.com/feed/?lang=en"),
             Sitemap(
                 "https://theintercept.com/sitemap_index.xml",
@@ -113,14 +132,28 @@
             RSSFeed("https://www.washingtontimes.com/rss/headlines/news/politics/"),
             Sitemap("https://www.washingtontimes.com/sitemap-stories.xml"),
             Sitemap("https://www.washingtontimes.com/sitemap-entries.xml"),
         ],
         parser=WashingtonTimesParser,
     )
 
+    WashingtonPost = PublisherSpec(
+        name="Washington Post",
+        domain="https://www.washingtonpost.com/",
+        sources=[
+            Sitemap("https://www.washingtonpost.com/sitemaps/sitemap.xml.gz"),
+            NewsMap("https://www.washingtonpost.com/sitemaps/news-sitemap.xml.gz"),
+            RSSFeed("https://feeds.washingtonpost.com/rss/world"),
+            RSSFeed("https://feeds.washingtonpost.com/rss/national"),
+        ],
+        parser=WashingtonPostParser,
+        # Adds a URL-filter to ignore incomplete URLs
+        url_filter=regex_filter("washingtonpost.com(\/)?$"),
+    )
+
     TheNewYorker = PublisherSpec(
         name="The New Yorker",
         domain="https://www.newyorker.com/",
         sources=[
             Sitemap("https://www.newyorker.com/sitemap.xml"),
             NewsMap("https://www.newyorker.com/feed/google-news-sitemap-feed/sitemap-google-news"),
         ],
@@ -160,7 +193,44 @@
         domain="https://www.businessinsider.com/",
         sources=[
             NewsMap("https://www.businessinsider.com/sitemap/google-news.xml"),
             Sitemap("https://www.businessinsider.com/sitemap/2024-01.xml"),
         ],
         parser=BusinessInsiderParser,
     )
+
+    RollingStone = PublisherSpec(
+        name="Rolling Stone",
+        domain="https://www.rollingstone.com/",
+        sources=[
+            NewsMap("https://www.rollingstone.com/news-sitemap.xml"),
+            Sitemap(
+                "https://www.rollingstone.com/sitemap_index.xml",
+                sitemap_filter=inverse(lor(regex_filter("/pmc_list-sitemap"), regex_filter("/post-sitemap"))),
+            ),
+        ],
+        parser=RollingStoneParser,
+    )
+
+    VoiceOfAmerica = PublisherSpec(
+        name="Voice Of America",
+        domain="https://www.voanews.com/",
+        sources=[
+            NewsMap("https://www.voanews.com/sitemap_415_news.xml.gz"),
+            Sitemap(
+                "https://www.voanews.com/sitemap.xml", sitemap_filter=inverse(regex_filter(r"sitemap_[\d_]*\.xml\.gz"))
+            ),
+        ],
+        parser=VOAParser,
+    )
+
+    Wired = PublisherSpec(
+        name="Wired",
+        domain="https://www.wired.com",
+        sources=[
+            RSSFeed("https://www.wired.com/feed/rss"),
+            NewsMap("https://www.wired.com/feed/google-latest-news/sitemap-google-news"),
+            Sitemap("https://www.wired.com/sitemap.xml"),
+            Sitemap("https://www.wired.com/sitemap-archive-1.xml"),
+        ],
+        parser=WiredParser,
+    )
```

### Comparing `fundus-0.3.0/src/fundus/publishers/us/ap_news.py` & `fundus-0.3.1/src/fundus/publishers/us/ap_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/business_insider.py` & `fundus-0.3.1/src/fundus/publishers/us/business_insider.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/cnbc.py` & `fundus-0.3.1/src/fundus/publishers/us/cnbc.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/fox_news.py` & `fundus-0.3.1/src/fundus/publishers/us/fox_news.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/free_beacon.py` & `fundus-0.3.1/src/fundus/publishers/us/free_beacon.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/la_times.py` & `fundus-0.3.1/src/fundus/publishers/us/la_times.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/occupy_democrats.py` & `fundus-0.3.1/src/fundus/publishers/us/occupy_democrats.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/reuters.py` & `fundus-0.3.1/src/fundus/publishers/us/reuters.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/the_gateway_pundit.py` & `fundus-0.3.1/src/fundus/publishers/us/the_gateway_pundit.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/the_intercept.py` & `fundus-0.3.1/src/fundus/publishers/us/the_intercept.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/the_nation_parser.py` & `fundus-0.3.1/src/fundus/publishers/us/the_nation_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/the_new_yorker.py` & `fundus-0.3.1/src/fundus/publishers/us/the_new_yorker.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/washington_times_parser.py` & `fundus-0.3.1/src/fundus/publishers/us/washington_times_parser.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/publishers/us/world_truth.py` & `fundus-0.3.1/src/fundus/publishers/us/world_truth.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/scraping/article.py` & `fundus-0.3.1/src/fundus/scraping/article.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
 
 import langdetect
 import lxml.html
 import more_itertools
 from colorama import Fore, Style
 
-from fundus.logging.logger import basic_logger
+from fundus.logging import create_logger
 from fundus.parser import ArticleBody
 from fundus.scraping.html import HTML
 
+logger = create_logger(__name__)
+
 
 @dataclass(frozen=True)
 class Article:
     html: HTML
     exception: Optional[Exception] = None
 
     # supported (validated) attributes as defined in the guidelines
@@ -50,26 +52,26 @@
     def lang(self) -> Optional[str]:
         language: Optional[str] = None
 
         if self.plaintext:
             try:
                 language = langdetect.detect(self.plaintext)
             except langdetect.LangDetectException:
-                basic_logger.debug(f"Unable to detect language for article '{self.html.responded_url}'")
+                logger.debug(f"Unable to detect language for article {self.html.responded_url!r}")
 
         # use @lang attribute of <html> tag as fallback
         if not language or language == langdetect.detector_factory.Detector.UNKNOWN_LANG:
             language = lxml.html.fromstring(self.html.content).get("lang")
             if language and "-" in language:
                 language = language.split("-")[0]
 
         return language
 
     def __getattr__(self, item: object) -> Any:
-        raise AttributeError(f"'{type(self).__name__}' object has no attribute '{item}'")
+        raise AttributeError(f"{type(self).__name__!r} object has no attribute {str(item)!r}")
 
     def __str__(self):
         # the subsequent indent here is a bit wacky, but textwrapper.dedent won't work with tabs, so we have to use
         # whitespaces instead.
         title_wrapper = TextWrapper(width=80, max_lines=1, initial_indent="")
         text_wrapper = TextWrapper(width=80, max_lines=2, initial_indent="", subsequent_indent="          ")
         wrapped_title = title_wrapper.fill(
```

### Comparing `fundus-0.3.0/src/fundus/scraping/crawler.py` & `fundus-0.3.1/src/fundus/scraping/crawler.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,36 @@
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
+from urllib.parse import urljoin, urlparse
 
 import dill
 import more_itertools
 import requests
 from dateutil.rrule import MONTHLY, rrule
 from more_itertools import roundrobin
 from tqdm import tqdm
 from typing_extensions import ParamSpec, TypeAlias
 
-from fundus.logging import basic_logger
+from fundus.logging import create_logger
 from fundus.publishers.base_objects import PublisherCollectionMeta, PublisherEnum
 from fundus.scraping.article import Article
 from fundus.scraping.delay import Delay
 from fundus.scraping.filter import ExtractionFilter, Requires, RequiresAll, URLFilter
 from fundus.scraping.html import CCNewsSource
 from fundus.scraping.scraper import CCNewsScraper, WebScraper
 from fundus.scraping.session import session_handler
 from fundus.scraping.url import URLSource
 
+logger = create_logger(__name__)
+
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 
 Publisher: TypeAlias = Union[PublisherEnum, Type[PublisherEnum], PublisherCollectionMeta]
 
 
 # noinspection PyPep8Naming
@@ -111,14 +114,20 @@
             try:
                 handle.get(timeout=0.1)
             except TimeoutError:
                 continue
             return
 
 
+def remove_query_parameters_from_url(url: str) -> str:
+    if any(parameter_indicator in url for parameter_indicator in ("?", "#")):
+        return urljoin(url, urlparse(url).path)
+    return url
+
+
 class CrawlerBase(ABC):
     def __init__(self, *publishers: Publisher):
         if not publishers:
             raise ValueError("param <publishers> of <Crawler.__init__> has to be non empty")
 
         self.publishers: List[PublisherEnum] = list(set(more_itertools.collapse(publishers)))
 
@@ -186,36 +195,37 @@
             for publisher in self.publishers:
                 supported_attributes = set(
                     more_itertools.flatten(
                         collection.names for collection in publisher.parser.attribute_mapping.values()
                     )
                 )
                 if missing_attributes := extraction_filter.required_attributes - supported_attributes:
-                    basic_logger.warning(
+                    logger.warning(
                         f"The required attribute(s) `{', '.join(missing_attributes)}` "
                         f"is(are) not supported by {publisher.publisher_name}. Skipping publisher"
                     )
                 else:
                     fitting_publishers.append(publisher)
 
             if not fitting_publishers:
-                basic_logger.error(
+                logger.error(
                     f"Could not find any fitting publishers for required attributes  "
                     f"`{', '.join(extraction_filter.required_attributes)}`"
                 )
                 return
         else:
             fitting_publishers = self.publishers
 
         article_count = 0
         for article in self._build_article_iterator(
             tuple(fitting_publishers), error_handling, build_extraction_filter(), url_filter
         ):
-            if not only_unique or article.html.responded_url not in response_cache:
-                response_cache.add(article.html.responded_url)
+            url_without_query_parameters = remove_query_parameters_from_url(article.html.responded_url)
+            if not only_unique or url_without_query_parameters not in response_cache:
+                response_cache.add(url_without_query_parameters)
                 article_count += 1
                 yield article
             if article_count == max_articles:
                 break
 
         session_handler.close_current_session()
```

### Comparing `fundus-0.3.0/src/fundus/scraping/delay.py` & `fundus-0.3.1/src/fundus/scraping/delay.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/src/fundus/scraping/filter.py` & `fundus-0.3.1/src/fundus/scraping/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,17 +160,17 @@
             if not self._eval(value := extraction.get(attribute)) or isinstance(value, Exception)
         ]
         return FilterResultWithMissingAttributes(*missing_attributes)
 
 
 class RequiresAll(Requires):
     def __init__(self, eval_booleans: bool = False) -> None:
-        """Name wrap for Requires()
+        """Name wrap for Requires(eval_booleans=False)
 
         This is for readability only. By default, it requires all non-boolean attributes of the extraction
-        to evaluate to True. Set `skip_boolean=False` to alter this behaviour.
+        to evaluate to True. Set `eval_booleans=True` to include boolean values in the evaluation as well.
         See class:Requires docstring for more information.
 
         Args:
             eval_booleans: See Requires docstring for more information. Defaults to False.
         """
         super().__init__(eval_booleans=eval_booleans)
```

### Comparing `fundus-0.3.0/src/fundus/scraping/html.py` & `fundus-0.3.1/src/fundus/scraping/html.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,65 @@
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Dict, Iterable, Iterator, List, Optional, Protocol
 from urllib.parse import urlparse
 
 import chardet
+import lxml.html
 import requests
 import validators
 from fastwarc import ArchiveIterator, WarcRecord, WarcRecordType
+from lxml.cssselect import CSSSelector
 from requests import ConnectionError, HTTPError
 
-from fundus.logging import basic_logger
+from fundus.logging import create_logger
 from fundus.publishers.base_objects import PublisherEnum
 from fundus.scraping.delay import Delay
 from fundus.scraping.filter import URLFilter
-from fundus.scraping.session import _default_header
+from fundus.scraping.session import _default_header, session_handler
+from fundus.scraping.url import URLSource
 
 __all__ = [
     "HTML",
     "SourceInfo",
     "WarcSourceInfo",
     "WebSourceInfo",
     "HTMLSource",
     "WebSource",
     "CCNewsSource",
 ]
 
-from fundus.scraping.session import session_handler
-from fundus.scraping.url import URLSource
+logger = create_logger(__name__)
+
+# unfortunately lxml does not support case-insensitive CSSSelectors
+_content_type_selector = CSSSelector("meta[http-equiv='Content-Type'], meta[http-equiv='content-type']")
+
+
+def _detect_charset_from_response(response: requests.Response) -> str:
+    """Detects HTML encoding based on meta tag <http-equiv='Content-Type'>
+
+    Args:
+        response: Response to detect encoding for
+
+    Returns:
+        str: detected encoding or response.apparent_encoding
+    """
+    # see https://github.com/flairNLP/fundus/issues/446
+    # use response fallback to decode HTML in a first guess
+    guessed_text = response.content.decode(response.encoding or "utf-8")
+    charset = None
+    if (content_type_nodes := _content_type_selector(lxml.html.document_fromstring(guessed_text))) and len(
+        content_type_nodes
+    ) == 1:
+        content_type_node = content_type_nodes.pop()
+        for field in content_type_node.attrib.get("content", "").split(";"):
+            if "charset" in field:
+                charset = field.replace("charset=", "").strip()
+    return charset or response.apparent_encoding
 
 
 @dataclass(frozen=True)
 class HTML:
     requested_url: str
     responded_url: str
     content: str
@@ -93,48 +121,53 @@
 
         for url in self.url_source:
             if self.delay:
                 time.sleep(max(0.0, self.delay() - time.time() + timestamp))
                 timestamp = time.time()
 
             if not validators.url(url):
-                basic_logger.debug(f"Skipped requested URL '{url}' because the URL is malformed")
+                logger.debug(f"Skipped requested URL {url!r} because the URL is malformed")
                 continue
 
             if filter_url(url):
-                basic_logger.debug(f"Skipped requested URL '{url}' because of URL filter")
+                logger.debug(f"Skipped requested URL {url!r} because of URL filter")
                 continue
 
             session = session_handler.get_session()
             for key, value in self.query_parameters.items():
                 if "?" in url:
                     url += "&" + key + "=" + value
                 else:
                     url += "?" + key + "=" + value
             try:
                 response = session.get(url, headers=self.request_header)
 
             except (HTTPError, ConnectionError) as error:
-                basic_logger.info(f"Skipped requested URL '{url}' because of '{error}'")
+                logger.info(f"Skipped requested URL {url!r} because of {error!r}")
                 if isinstance(error, HTTPError) and error.response.status_code >= 500:
-                    basic_logger.info(f"Skipped {self.publisher} due to server errors: '{error}'")
+                    logger.info(f"Skipped {self.publisher!r} due to server errors: {error!r}")
                 continue
 
             except Exception as error:
-                basic_logger.warning(f"Warning! Skipped  requested URL '{url}' because of an unexpected error {error}")
+                logger.warning(f"Warning! Skipped  requested URL {url!r} because of an unexpected error {error!r}")
                 continue
 
             else:
+                if "charset" not in response.headers["content-type"]:
+                    # That's actually the only place requests checks to detect encoding, so if charset
+                    # is not set, requests falls back to default encodings (latin-1/utf-8)
+                    response.encoding = _detect_charset_from_response(response)
+
                 if filter_url(str(response.url)):
-                    basic_logger.debug(f"Skipped responded URL '{str(response.url)}' because of URL filter")
+                    logger.debug(f"Skipped responded URL {str(response.url)!r} because of URL filter")
                     continue
                 html = response.text
 
                 if response.history:
-                    basic_logger.info(f"Got redirected {len(response.history)} time(s) from {url} -> {response.url}")
+                    logger.info(f"Got redirected {len(response.history)} time(s) from {url!r} -> {response.url!r}")
 
                 source_info = (
                     WebSourceInfo(self.publisher, type(self.url_source).__name__, self.url_source.url)
                     if isinstance(self.url_source, URLSource)
                     else SourceInfo(self.publisher)
                 )
 
@@ -163,53 +196,53 @@
 
             try:
                 return str(warc_body, encoding=record.http_charset)
             except (UnicodeDecodeError, TypeError):
                 encoding: Optional[str] = chardet.detect(warc_body)["encoding"]
 
                 if encoding is not None:
-                    basic_logger.debug(
+                    logger.debug(
                         f"Trying to decode record {record.record_id!r} from {target_url!r} "
                         f"using detected encoding {encoding}."
                     )
 
                     try:
                         return str(warc_body, encoding=encoding)
                     except UnicodeDecodeError:
-                        basic_logger.warning(
+                        logger.warning(
                             f"Couldn't decode record {record.record_id!r} from {target_url!r} with "
                             f"original charset {record.http_charset!r} using detected charset {encoding!r}."
                         )
                 else:
-                    basic_logger.warning(
+                    logger.warning(
                         f"Couldn't detect charset for record {record.record_id!r} from {target_url!r} "
                         f"with invalid original charset {record.http_charset!r}."
                     )
 
             return None
 
         with requests.Session() as session:
             stream = session.get(self.warc_path, stream=True, headers=self.headers).raw
 
             for warc_record in ArchiveIterator(stream, record_types=WarcRecordType.response, verify_digests=True):
                 target_url = str(warc_record.headers["WARC-Target-URI"])
 
                 if url_filter is not None and url_filter(target_url):
-                    basic_logger.debug(f"Skipped WARC record with target URI {target_url!r} because of URL filter")
+                    logger.debug(f"Skipped WARC record with target URI {target_url!r} because of URL filter")
                     continue
 
                 publisher_domain: str = urlparse(target_url).netloc
 
                 if publisher_domain not in self._publisher_mapping:
                     continue
 
                 publisher = self._publisher_mapping[publisher_domain]
 
                 if publisher.url_filter is not None and publisher.url_filter(target_url):
-                    basic_logger.debug(
+                    logger.debug(
                         f"Skipped WARC record with target URI {target_url!r} because of "
                         f"publisher specific URL filter"
                     )
                     continue
 
                 if (content := extract_content(warc_record)) is None:
                     continue
```

### Comparing `fundus-0.3.0/src/fundus/scraping/scraper.py` & `fundus-0.3.1/src/fundus/scraping/scraper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Dict, Iterator, List, Literal, Optional, Type
 
 import more_itertools
 
-from fundus.logging import basic_logger
+from fundus.logging import create_logger
 from fundus.parser import ParserProxy
 from fundus.publishers.base_objects import PublisherEnum
 from fundus.scraping.article import Article
 from fundus.scraping.delay import Delay
 from fundus.scraping.filter import (
     ExtractionFilter,
     FilterResultWithMissingAttributes,
     URLFilter,
 )
 from fundus.scraping.html import CCNewsSource, HTMLSource, WebSource
 from fundus.scraping.url import URLSource
 
+logger = create_logger(__name__)
+
 
 class BaseScraper:
     def __init__(self, *sources: HTMLSource, parser_mapping: Dict[str, ParserProxy]):
         self.sources = sources
         self.parser_mapping = parser_mapping
 
     def scrape(
@@ -30,38 +32,36 @@
         for source in self.sources:
             for html in source.fetch(url_filter=url_filter):
                 parser = self.parser_mapping[html.source_info.publisher]
 
                 try:
                     extraction = parser(html.crawl_date).parse(html.content, error_handling)
 
-                except Exception as err:
+                except Exception as error:
                     if error_handling == "raise":
-                        error_message = f"Run into an error processing article '{html.requested_url}'"
-                        basic_logger.error(error_message)
-                        err.args = (str(err) + "\n\n" + error_message,)
-                        raise err
+                        error_message = f"Run into an error processing article {html.requested_url!r}"
+                        logger.error(error_message)
+                        error.args = (str(error) + "\n\n" + error_message,)
+                        raise error
                     elif error_handling == "catch":
-                        yield Article(html=html, exception=err)
+                        yield Article(html=html, exception=error)
                     elif error_handling == "suppress":
-                        basic_logger.info(f"Skipped article at '{html.requested_url}' because of: {err!r}")
+                        logger.info(f"Skipped article at {html.requested_url!r} because of: {error!r}")
                     else:
-                        raise ValueError(f"Unknown value '{error_handling}' for parameter <error_handling>'")
+                        raise ValueError(f"Unknown value {error_handling!r} for parameter <error_handling>'")
 
                 else:
                     if extraction_filter and (filter_result := extraction_filter(extraction)):
                         if isinstance(filter_result, FilterResultWithMissingAttributes):
-                            basic_logger.debug(
-                                f"Skipped article at '{html.requested_url}' because attribute(s) "
+                            logger.debug(
+                                f"Skipped article at {html.requested_url!r} because attribute(s) "
                                 f"{', '.join(filter_result.missing_attributes)!r} is(are) missing"
                             )
                         else:
-                            basic_logger.debug(
-                                f"Skipped article at '{html.requested_url}' because of extraction filter"
-                            )
+                            logger.debug(f"Skipped article at {html.requested_url!r} because of extraction filter")
                     else:
                         article = Article.from_extracted(html=html, extracted=extraction)
                         yield article
 
 
 class WebScraper(BaseScraper):
     def __init__(
@@ -79,14 +79,15 @@
 
         html_sources = [
             WebSource(
                 url_source=url_source,
                 publisher=publisher.publisher_name,
                 request_header=publisher.request_header,
                 delay=delay,
+                url_filter=publisher.url_filter,
                 query_parameters=publisher.query_parameter,
             )
             for url_source in url_sources
         ]
         parser_mapping: Dict[str, ParserProxy] = {publisher.publisher_name: publisher.parser}
         super().__init__(*html_sources, parser_mapping=parser_mapping)
```

### Comparing `fundus-0.3.0/src/fundus/scraping/session.py` & `fundus-0.3.1/src/fundus/scraping/session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import threading
 from contextlib import contextmanager
 from typing import Iterator, Optional
 
 import requests.adapters
 from typing_extensions import Self
 
-from fundus.logging import basic_logger
+from fundus.logging import create_logger
+
+logger = create_logger(__name__)
 
 _default_header = {"user-agent": "Fundus"}
 
 
 class SessionHandler:
     """Object for handling project global request.Session
 
@@ -36,22 +38,22 @@
         - pool_maxsize: <self.pool_maxsize>
         - hooks: (1) Hook to raise an `HTTPError` if one occurred. (2) Hook to log the request responses.
 
         Returns:
             A new requests.Session
         """
 
-        basic_logger.debug("Creating new session")
+        logger.debug("Creating new session")
         session = requests.Session()
 
         def _response_log(response: requests.Response, *args, **kwargs) -> None:
             history = response.history
             previous_status_codes = [f"({response.status_code})" for response in history] if history else []
             status_code_chain = " -> ".join(previous_status_codes + [f"({response.status_code})"])
-            basic_logger.debug(
+            logger.debug(
                 f"{status_code_chain} <{response.request.method} {response.url!r}> "
                 f"took {response.elapsed.total_seconds()} second(s)"
             )
 
         # hooks
         response_hooks = [lambda response, *args, **kwargs: response.raise_for_status(), _response_log]
         session.hooks["response"].extend(response_hooks)
@@ -88,15 +90,15 @@
         """Tears down the current build session
 
         Returns:
             None
         """
         if self.session is not None:
             session = self.get_session()
-            basic_logger.debug(f"Close session {session}")
+            logger.debug(f"Close session {session}")
             session.close()
             self.session = None
 
     @contextmanager
     def context(self, pool_connections: int, pool_maxsize: int) -> Iterator[Self]:
         """Context manager to temporarily overwrite parameter and build a new session.
```

### Comparing `fundus-0.3.0/src/fundus/scraping/url.py` & `fundus-0.3.1/src/fundus/scraping/url.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,27 @@
 import feedparser
 import lxml.html
 import validators
 from lxml.cssselect import CSSSelector
 from lxml.etree import XPath
 from requests import ConnectionError, HTTPError
 
-from fundus.logging import basic_logger
+from fundus.logging import create_logger
 from fundus.scraping.filter import URLFilter, inverse
 from fundus.scraping.session import _default_header, session_handler
 
+logger = create_logger(__name__)
+
 
 class _ArchiveDecompressor:
     def __init__(self):
-        self.archive_mapping: Dict[str, Callable[[bytes], bytes]] = {"application/x-gzip": self._decompress_gzip}
+        self.archive_mapping: Dict[str, Callable[[bytes], bytes]] = {
+            "application/x-gzip": self._decompress_gzip,
+            "gzip": self._decompress_gzip,
+        }
 
     @staticmethod
     def _decompress_gzip(compressed_content: bytes) -> bytes:
         decompressed_content = gzip.decompress(compressed_content)
         return decompressed_content
 
     def decompress(self, content: bytes, file_format: "str") -> bytes:
@@ -41,15 +46,15 @@
 
     _request_header: Dict[str, str] = field(default_factory=dict)
 
     def __post_init__(self):
         if not self._request_header:
             self._request_header = _default_header
         if not validators.url(self.url, strict_query=False):
-            basic_logger.error(f"{type(self).__name__} initialized with invalid URL {self.url}")
+            logger.error(f"{type(self).__name__} initialized with invalid URL {self.url}")
 
     def set_header(self, request_header: Dict[str, str]) -> None:
         self._request_header = request_header
 
     @abstractmethod
     def __iter__(self) -> Iterator[str]:
         raise NotImplemented
@@ -70,19 +75,23 @@
         return itertools.islice(self, max_urls)
 
 
 @dataclass
 class RSSFeed(URLSource):
     def __iter__(self) -> Iterator[str]:
         session = session_handler.get_session()
-        response = session.get(self.url, headers=self._request_header)
+        try:
+            response = session.get(self.url, headers=self._request_header)
+        except HTTPError as err:
+            logger.warning(f"Warning! Couldn't parse rss feed {self.url!r} because of {err}")
+            return
         html = response.text
         rss_feed = feedparser.parse(html)
         if exception := rss_feed.get("bozo_exception"):
-            basic_logger.warning(f"Warning! Couldn't parse rss feed '{self.url}' because of {exception}")
+            logger.warning(f"Warning! Couldn't parse rss feed {self.url!r} because of {exception}")
             return
         else:
             for url in (entry["link"] for entry in rss_feed["entries"]):
                 yield url
 
 
 @dataclass
@@ -95,25 +104,25 @@
     _sitemap_selector: ClassVar[XPath] = CSSSelector("sitemap > loc")
     _url_selector: ClassVar[XPath] = CSSSelector("url > loc")
 
     def __iter__(self) -> Iterator[str]:
         def yield_recursive(sitemap_url: str) -> Iterator[str]:
             session = session_handler.get_session()
             if not validators.url(sitemap_url):
-                basic_logger.info(f"Skipped sitemap '{sitemap_url}' because the URL is malformed")
+                logger.info(f"Skipped sitemap {sitemap_url!r} because the URL is malformed")
             try:
                 response = session.get(url=sitemap_url, headers=self._request_header)
             except (HTTPError, ConnectionError) as error:
-                basic_logger.warning(f"Warning! Couldn't reach sitemap '{sitemap_url}' because of {error}")
+                logger.warning(f"Warning! Couldn't reach sitemap {sitemap_url!r} because of {error!r}")
                 return
             content = response.content
             if (content_type := response.headers.get("content-type")) in self._decompressor.supported_file_formats:
                 content = self._decompressor.decompress(content, content_type)
             if not content:
-                basic_logger.warning(f"Warning! Empty sitemap at '{sitemap_url}'")
+                logger.warning(f"Warning! Empty sitemap at {sitemap_url!r}")
                 return
             tree = lxml.html.fromstring(content)
             urls = [node.text_content() for node in self._url_selector(tree)]
             if urls:
                 for new_url in reversed(urls) if self.reverse else urls:
                     yield new_url
             elif self.recursive:
```

### Comparing `fundus-0.3.0/src/fundus.egg-info/PKG-INFO` & `fundus-0.3.1/src/fundus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fundus
-Version: 0.3.0
+Version: 0.3.1
 Summary: A very simple news crawler
 Author-email: Max Dallabetta <max.dallabetta@googlemail.com>
 License: MIT
 Project-URL: Repository, https://github.com/flairNLP/fundus
 Keywords: web scraping, web crawling
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 Requires-Dist: lxml<5,>=4.9
 Requires-Dist: more-itertools<10,>=9.1
 Requires-Dist: cssselect<2,>=1.1
 Requires-Dist: feedparser<7,>=6.0
 Requires-Dist: colorama<1,>=0.4
 Requires-Dist: typing-extensions<5,>=4.6
 Requires-Dist: langdetect<2,>=1.0
-Requires-Dist: validators!=0.23,<1,>=0.20
+Requires-Dist: validators<1,>=0.24
 Requires-Dist: requests<3,>=2.28
 Requires-Dist: tqdm<5,>=4.66
 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2
 Requires-Dist: dill<1,>=0.3
 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev"
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fundus Version: 0.3.0 Summary: A very simple news
+Metadata-Version: 2.1 Name: fundus Version: 0.3.1 Summary: A very simple news
 crawler Author-email: Max Dallabetta
 googlemail.com> License: MIT Project-URL: Repository, https://github.com/
 flairNLP/fundus Keywords: web scraping, web crawling Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Requires-Python: >=3.8 Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: python-dateutil<3,>=2.8
 Requires-Dist: lxml<5,>=4.9 Requires-Dist: more-itertools<10,>=9.1 Requires-
 Dist: cssselect<2,>=1.1 Requires-Dist: feedparser<7,>=6.0 Requires-Dist:
 colorama<1,>=0.4 Requires-Dist: typing-extensions<5,>=4.6 Requires-Dist:
-langdetect<2,>=1.0 Requires-Dist: validators!=0.23,<1,>=0.20 Requires-Dist:
+langdetect<2,>=1.0 Requires-Dist: validators<1,>=0.24 Requires-Dist:
 requests<3,>=2.28 Requires-Dist: tqdm<5,>=4.66 Requires-Dist: fastwarc<1,>=0.14
 Requires-Dist: chardet<6,>=5.2 Requires-Dist: dill<1,>=0.3 Provides-Extra: dev
 Requires-Dist: pytest~=7.2.2; extra == "dev" Requires-Dist: mypy==1.9.0; extra
 == "dev" Requires-Dist: isort==5.12.0; extra == "dev" Requires-Dist:
 black==23.1.0; extra == "dev" Requires-Dist: types-lxml; extra == "dev"
 Requires-Dist: types-python-dateutil<3,>=2.8; extra == "dev" Requires-Dist:
 types-requests<3,>=2.28; extra == "dev" Requires-Dist: types-colorama<1,>=0.4;
```

### Comparing `fundus-0.3.0/tests/test_collection.py` & `fundus-0.3.1/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/tests/test_crawler.py` & `fundus-0.3.1/tests/test_crawler.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/tests/test_filter.py` & `fundus-0.3.1/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `fundus-0.3.0/tests/test_parser.py` & `fundus-0.3.1/tests/test_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,45 +126,50 @@
         assert attrs1.names != attrs2.names
 
 
 # enforce test coverage for test parsing
 # because this is also used for the generate_parser_test_files script we export it here
 attributes_required_to_cover = {"title", "authors", "topics", "publishing_date", "body"}
 
+attributes_parsers_are_required_to_cover = {"body"}
+
 
 @pytest.mark.parametrize(
     "publisher", list(PublisherCollection), ids=[publisher.name for publisher in PublisherCollection]
 )
 class TestParser:
     def test_annotations(self, publisher: PublisherEnum) -> None:
         parser_proxy = publisher.parser
         for versioned_parser in parser_proxy:
+            assert attributes_parsers_are_required_to_cover.issubset(
+                set(versioned_parser.attributes().validated.names)
+            ), f"{versioned_parser.__name__!r} should implement at least {attributes_parsers_are_required_to_cover!r}"
             for attr in versioned_parser.attributes().validated:
                 if annotation := attribute_annotations_mapping[attr.__name__]:
                     assert (
                         attr.__annotations__.get("return") == annotation
-                    ), f"Attribute {attr.__name__} for {versioned_parser.__name__} failed"
+                    ), f"Attribute {attr.__name__!r} for {versioned_parser.__name__!r} failed"
                 else:
-                    raise KeyError(f"Unsupported attribute '{attr.__name__}'")
+                    raise KeyError(f"Unsupported attribute {attr.__name__!r}")
 
     def test_parsing(self, publisher: PublisherEnum) -> None:
         comparative_data = load_test_case_data(publisher)
         html_mapping = load_html_test_file_mapping(publisher)
 
         for versioned_parser in publisher.parser:
             # validate json
             version_name = versioned_parser.__name__
             assert (
                 version_data := comparative_data.get(version_name)
-            ), f"Missing test data for parser version '{version_name}'"
+            ), f"Missing test data for parser version {version_name!r}"
 
             for key, value in version_data.items():
                 if not value:
                     raise ValueError(
-                        f"There is no value set for key '{key}' in the test JSON. "
+                        f"There is no value set for key {key!r} in the test JSON. "
                         f"Only complete articles should be used as test cases"
                     )
 
             # test coverage
             supported_attrs = set(versioned_parser.attributes().names)
             missing_attrs = attributes_required_to_cover & supported_attrs - set(version_data.keys())
             assert (
@@ -181,15 +186,15 @@
             for key, value in version_data.items():
                 assert value == extraction[key]
 
     def test_reserved_attribute_names(self, publisher: PublisherEnum):
         parser = publisher.parser
         for attr in attribute_annotations_mapping.keys():
             if value := getattr(parser, attr, None):
-                assert isinstance(value, Attribute), f"The name '{attr}' is reserved for attributes only."
+                assert isinstance(value, Attribute), f"The name {attr!r} is reserved for attributes only."
 
 
 class TestUtility:
     def test_generic_author_parsing(self):
         # type None
         assert generic_author_parsing(None) == []
```

