# Comparing `tmp/kappa_maki-1.0.1.tar.gz` & `tmp/kappa_maki-1.0.3.dev1715613122.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kappa_maki-1.0.1.tar", max compression
+gzip compressed data, was "kappa_maki-1.0.3.dev1715613122.tar", max compression
```

## Comparing `kappa_maki-1.0.1.tar` & `kappa_maki-1.0.3.dev1715613122.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2024-04-23 20:10:38.158793 kappa_maki-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1307 2024-04-23 20:10:38.158891 kappa_maki-1.0.1/README.md
--rw-r--r--   0        0        0      594 2024-04-23 20:10:47.131897 kappa_maki-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-23 20:10:38.159244 kappa_maki-1.0.1/src/kappa_maki/__init__.py
--rw-r--r--   0        0        0     8663 2024-04-23 20:10:38.159412 kappa_maki-1.0.1/src/kappa_maki/kappa_maki_formatter.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 kappa_maki-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-13 19:11:31.188915 kappa_maki-1.0.3.dev1715613122/LICENSE.txt
+-rw-r--r--   0        0        0     1307 2024-05-13 19:11:31.189059 kappa_maki-1.0.3.dev1715613122/README.md
+-rw-r--r--   0        0        0      892 2024-05-13 19:12:02.662802 kappa_maki-1.0.3.dev1715613122/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 19:11:31.189537 kappa_maki-1.0.3.dev1715613122/src/kappa_maki/__init__.py
+-rw-r--r--   0        0        0     8663 2024-05-13 19:11:31.189767 kappa_maki-1.0.3.dev1715613122/src/kappa_maki/kappa_maki_formatter.py
+-rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 kappa_maki-1.0.3.dev1715613122/PKG-INFO
```

### Comparing `kappa_maki-1.0.1/LICENSE.txt` & `kappa_maki-1.0.3.dev1715613122/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kappa_maki-1.0.1/README.md` & `kappa_maki-1.0.3.dev1715613122/README.md`

 * *Files identical despite different names*

### Comparing `kappa_maki-1.0.1/src/kappa_maki/kappa_maki_formatter.py` & `kappa_maki-1.0.3.dev1715613122/src/kappa_maki/kappa_maki_formatter.py`

 * *Files identical despite different names*

### Comparing `kappa_maki-1.0.1/PKG-INFO` & `kappa_maki-1.0.3.dev1715613122/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: kappa-maki
-Version: 1.0.1
+Version: 1.0.3.dev1715613122
 Summary: Formatter for generating Cucumber-format JSON test results using the Behave test framework.  Named after a refreshing cucumber sushi cocktail.
 Home-page: https://github.com/TechnologyBrewery/kappa-maki
 License: MIT
 Author: Isaac Becerra Llanos
 Author-email: ibecerrallanos@cpointe-inc.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/TechnologyBrewery/kappa-maki
 Description-Content-Type: text/markdown
 
 [![PyPI](https://img.shields.io/pypi/v/kappa-maki)](https://pypi.org/project/kappa-maki/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kappa-maki)
```

