# Comparing `tmp/aiocmcapi-0.6.tar.gz` & `tmp/aiocmcapi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocmcapi-0.6.tar", last modified: Mon May 13 02:27:31 2024, max compression
+gzip compressed data, was "aiocmcapi-0.6.1.tar", last modified: Mon May 13 02:31:26 2024, max compression
```

## Comparing `aiocmcapi-0.6.tar` & `aiocmcapi-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:27:31.872820 aiocmcapi-0.6/
--rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6/LICENSE
--rw-rw-rw-   0        0        0     2045 2024-05-13 02:27:31.871821 aiocmcapi-0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 02:27:31.871821 aiocmcapi-0.6/aiocmcapi.egg-info/
--rw-rw-rw-   0        0        0     2045 2024-05-13 02:27:31.000000 aiocmcapi-0.6/aiocmcapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-13 02:27:31.000000 aiocmcapi-0.6/aiocmcapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:27:31.000000 aiocmcapi-0.6/aiocmcapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-05-13 02:27:31.000000 aiocmcapi-0.6/aiocmcapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-13 02:27:31.000000 aiocmcapi-0.6/aiocmcapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      410 2024-05-13 02:27:22.000000 aiocmcapi-0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 02:27:31.872820 aiocmcapi-0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 02:31:26.559199 aiocmcapi-0.6.1/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 19:33:44.000000 aiocmcapi-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     2047 2024-05-13 02:31:26.558200 aiocmcapi-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1777 2024-05-11 21:20:54.000000 aiocmcapi-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 02:31:26.558200 aiocmcapi-0.6.1/aiocmcapi.egg-info/
+-rw-rw-rw-   0        0        0     2047 2024-05-13 02:31:26.000000 aiocmcapi-0.6.1/aiocmcapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-05-13 02:31:26.000000 aiocmcapi-0.6.1/aiocmcapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:31:26.000000 aiocmcapi-0.6.1/aiocmcapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-13 02:31:26.000000 aiocmcapi-0.6.1/aiocmcapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 02:31:26.000000 aiocmcapi-0.6.1/aiocmcapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      412 2024-05-13 02:31:02.000000 aiocmcapi-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:31:26.559199 aiocmcapi-0.6.1/setup.cfg
```

### Comparing `aiocmcapi-0.6/LICENSE` & `aiocmcapi-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.6/PKG-INFO` & `aiocmcapi-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.6
+Version: 0.6.1
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

### Comparing `aiocmcapi-0.6/README.md` & `aiocmcapi-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `aiocmcapi-0.6/aiocmcapi.egg-info/PKG-INFO` & `aiocmcapi-0.6.1/aiocmcapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocmcapi
-Version: 0.6
+Version: 0.6.1
 Summary: Async wrapper for CoinMarketCap API
 Author-email: alobuzy <amozebus@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp>=3.9.5
```

