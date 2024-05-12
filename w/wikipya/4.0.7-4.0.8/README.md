# Comparing `tmp/wikipya-4.0.7.tar.gz` & `tmp/wikipya-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikipya-4.0.7.tar", max compression
+gzip compressed data, was "wikipya-4.0.8.tar", max compression
```

## Comparing `wikipya-4.0.7.tar` & `wikipya-4.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1072 2024-03-09 18:47:12.014745 wikipya-4.0.7/LICENSE
--rw-r--r--   0        0        0     1534 2024-03-09 18:47:12.014745 wikipya-4.0.7/README.md
--rw-r--r--   0        0        0      715 2024-03-09 20:12:49.781540 wikipya-4.0.7/pyproject.toml
--rw-r--r--   0        0        0      184 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/__init__.py
--rw-r--r--   0        0        0      804 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/aiowiki.py
--rw-r--r--   0        0        0     1062 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/clients.py
--rw-r--r--   0        0        0     2797 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/constants.py
--rw-r--r--   0        0        0     1267 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/drivers.py
--rw-r--r--   0        0        0      220 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/exceptions.py
--rw-r--r--   0        0        0      345 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/__init__.py
--rw-r--r--   0        0        0      498 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/get_all.py
--rw-r--r--   0        0        0      275 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/get_page_name.py
--rw-r--r--   0        0        0      500 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/image.py
--rw-r--r--   0        0        0     1766 2024-03-09 19:45:12.283195 wikipya-4.0.7/wikipya/methods/image_legacy.py
--rw-r--r--   0        0        0      374 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/lib.py
--rw-r--r--   0        0        0      398 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/methods/opensearch.py
--rw-r--r--   0        0        0      520 2024-03-09 19:45:36.667099 wikipya-4.0.7/wikipya/methods/page.py
--rw-r--r--   0        0        0      485 2024-03-09 20:06:39.732275 wikipya-4.0.7/wikipya/methods/search.py
--rw-r--r--   0        0        0      863 2024-03-09 20:06:34.036176 wikipya-4.0.7/wikipya/methods/search_with_description.py
--rw-r--r--   0        0        0      293 2024-03-09 19:45:55.575026 wikipya-4.0.7/wikipya/methods/sections.py
--rw-r--r--   0        0        0      241 2024-03-09 19:49:59.142193 wikipya-4.0.7/wikipya/methods/summary.py
--rw-r--r--   0        0        0      513 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/models/__init__.py
--rw-r--r--   0        0        0      166 2024-03-09 19:35:53.006417 wikipya-4.0.7/wikipya/models/image.py
--rw-r--r--   0        0        0       95 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/models/images.py
--rw-r--r--   0        0        0      630 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/models/opensearch.py
--rw-r--r--   0        0        0     1017 2024-03-09 19:37:24.697707 wikipya-4.0.7/wikipya/models/page.py
--rw-r--r--   0        0        0      670 2024-03-09 19:55:52.633885 wikipya-4.0.7/wikipya/models/search.py
--rw-r--r--   0        0        0      246 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/models/section.py
--rw-r--r--   0        0        0      501 2024-03-09 19:37:24.833706 wikipya-4.0.7/wikipya/models/summary.py
--rw-r--r--   0        0        0      549 2024-03-09 18:47:12.018745 wikipya-4.0.7/wikipya/models/url.py
--rw-r--r--   0        0        0     2363 1970-01-01 00:00:00.000000 wikipya-4.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 21:01:45.060544 wikipya-4.0.8/LICENSE
+-rw-r--r--   0        0        0     1534 2024-05-12 21:01:45.060544 wikipya-4.0.8/README.md
+-rw-r--r--   0        0        0      716 2024-05-12 22:09:56.813176 wikipya-4.0.8/pyproject.toml
+-rw-r--r--   0        0        0      184 2024-05-12 21:01:45.060544 wikipya-4.0.8/wikipya/__init__.py
+-rw-r--r--   0        0        0      804 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/aiowiki.py
+-rw-r--r--   0        0        0     1062 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/clients.py
+-rw-r--r--   0        0        0     2797 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/constants.py
+-rw-r--r--   0        0        0     1267 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/drivers.py
+-rw-r--r--   0        0        0      220 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/exceptions.py
+-rw-r--r--   0        0        0      345 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/get_all.py
+-rw-r--r--   0        0        0      275 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/get_page_name.py
+-rw-r--r--   0        0        0      500 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/image.py
+-rw-r--r--   0        0        0     1766 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/image_legacy.py
+-rw-r--r--   0        0        0      374 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/lib.py
+-rw-r--r--   0        0        0      398 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/opensearch.py
+-rw-r--r--   0        0        0      520 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/page.py
+-rw-r--r--   0        0        0      485 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/search.py
+-rw-r--r--   0        0        0      863 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/search_with_description.py
+-rw-r--r--   0        0        0      293 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/sections.py
+-rw-r--r--   0        0        0      241 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/methods/summary.py
+-rw-r--r--   0        0        0      513 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/__init__.py
+-rw-r--r--   0        0        0      166 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/image.py
+-rw-r--r--   0        0        0       95 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/images.py
+-rw-r--r--   0        0        0      630 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/opensearch.py
+-rw-r--r--   0        0        0     1017 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/page.py
+-rw-r--r--   0        0        0      670 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/search.py
+-rw-r--r--   0        0        0      246 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/section.py
+-rw-r--r--   0        0        0      501 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/summary.py
+-rw-r--r--   0        0        0      549 2024-05-12 21:01:45.061544 wikipya-4.0.8/wikipya/models/url.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 wikipya-4.0.8/PKG-INFO
```

### Comparing `wikipya-4.0.7/LICENSE` & `wikipya-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/README.md` & `wikipya-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/pyproject.toml` & `wikipya-4.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "wikipya"
-version = "4.0.7"
+version = "4.0.8"
 description = "A simple async python library for search pages and images in wikis"
 authors = ["Daniel Zakharov <gzdan734@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 repository = "https://github.com/jDan735/wikipya"
 keywords = ["api", "wikipedia", "mediawiki", "asyncio"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.21.2"
 beautifulsoup4 = "^4.10.0"
-tghtml = "1.1.4"
+tghtml = "^1.1.5"
 pydantic = "^2.6.3"
 
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
```

### Comparing `wikipya-4.0.7/wikipya/aiowiki.py` & `wikipya-4.0.8/wikipya/aiowiki.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/clients.py` & `wikipya-4.0.8/wikipya/clients.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/constants.py` & `wikipya-4.0.8/wikipya/constants.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/drivers.py` & `wikipya-4.0.8/wikipya/drivers.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/methods/image_legacy.py` & `wikipya-4.0.8/wikipya/methods/image_legacy.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/methods/page.py` & `wikipya-4.0.8/wikipya/methods/page.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/methods/search_with_description.py` & `wikipya-4.0.8/wikipya/methods/search_with_description.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/models/__init__.py` & `wikipya-4.0.8/wikipya/models/__init__.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/models/opensearch.py` & `wikipya-4.0.8/wikipya/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/models/page.py` & `wikipya-4.0.8/wikipya/models/page.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/models/search.py` & `wikipya-4.0.8/wikipya/models/search.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/wikipya/models/url.py` & `wikipya-4.0.8/wikipya/models/url.py`

 * *Files identical despite different names*

### Comparing `wikipya-4.0.7/PKG-INFO` & `wikipya-4.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wikipya
-Version: 4.0.7
+Version: 4.0.8
 Summary: A simple async python library for search pages and images in wikis
 Home-page: https://github.com/jDan735/wikipya
 License: MIT
 Keywords: api,wikipedia,mediawiki,asyncio
 Author: Daniel Zakharov
 Author-email: gzdan734@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
 Requires-Dist: httpx (>=0.21.2,<0.22.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
-Requires-Dist: tghtml (==1.1.4)
+Requires-Dist: tghtml (>=1.1.5,<2.0.0)
 Project-URL: Repository, https://github.com/jDan735/wikipya
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>📚 wikipya</h1>
   <h3>A simple async python library for search pages and images in wikis</h3>
 </div><br>
```

