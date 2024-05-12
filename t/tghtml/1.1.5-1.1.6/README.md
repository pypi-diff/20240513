# Comparing `tmp/tghtml-1.1.5.tar.gz` & `tmp/tghtml-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tghtml-1.1.5.tar", max compression
+gzip compressed data, was "tghtml-1.1.6.tar", max compression
```

## Comparing `tghtml-1.1.5.tar` & `tghtml-1.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2024-05-12 21:01:53.124555 tghtml-1.1.5/LICENSE
--rw-r--r--   0        0        0      424 2024-05-12 21:46:47.537436 tghtml-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       91 2024-05-12 21:01:53.124555 tghtml-1.1.5/tghtml/__init__.py
--rw-r--r--   0        0        0     5306 2024-05-12 21:46:29.272374 tghtml-1.1.5/tghtml/core.py
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 tghtml-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 21:01:53.124555 tghtml-1.1.6/LICENSE
+-rw-r--r--   0        0        0      477 2024-05-12 22:31:02.265212 tghtml-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-12 22:25:42.459511 tghtml-1.1.6/tghtml/__init__.py
+-rw-r--r--   0        0        0     5306 2024-05-12 21:46:29.272374 tghtml-1.1.6/tghtml/core.py
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 tghtml-1.1.6/PKG-INFO
```

### Comparing `tghtml-1.1.5/LICENSE` & `tghtml-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tghtml-1.1.5/tghtml/core.py` & `tghtml-1.1.6/tghtml/core.py`

 * *Files identical despite different names*

### Comparing `tghtml-1.1.5/PKG-INFO` & `tghtml-1.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tghtml
-Version: 1.1.5
+Version: 1.1.6
 Summary: Simple tool for parse common HTML to Telegram HTML
 License: MIT
 Author: Daniel Zakharov
 Author-email: gzdan734@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: lxml[html-clean] (>=5.2.1,<6.0.0)
 Requires-Dist: readability-lxml (>=0.8.1,<0.9.0)
```

