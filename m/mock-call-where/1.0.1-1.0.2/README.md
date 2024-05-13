# Comparing `tmp/mock_call_where-1.0.1.tar.gz` & `tmp/mock_call_where-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mock_call_where-1.0.1.tar", last modified: Sun May 12 16:41:29 2024, max compression
+gzip compressed data, was "mock_call_where-1.0.2.tar", last modified: Mon May 13 21:00:58 2024, max compression
```

## Comparing `mock_call_where-1.0.1.tar` & `mock_call_where-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.936206 mock_call_where-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.940206 mock_call_where-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13918 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.936206 mock_call_where-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/src/mock_call_where/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/src/mock_call_where/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/src/mock_call_where/override.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/src/mock_call_where/pytest_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/src/mock_call_where.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-12 16:41:29.000000 mock_call_where-1.0.1/src/mock_call_where.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:41:29.944206 mock_call_where-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/tests/test_it_works.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-12 16:40:55.000000 mock_call_where-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.078295 mock_call_where-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.070295 mock_call_where-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.074295 mock_call_where-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13918 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-13 21:00:58.078295 mock_call_where-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.074295 mock_call_where-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.074295 mock_call_where-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-13 21:00:58.078295 mock_call_where-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.070295 mock_call_where-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.074295 mock_call_where-1.0.2/src/mock_call_where/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/src/mock_call_where/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/src/mock_call_where/override.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/src/mock_call_where/pytest_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.078295 mock_call_where-1.0.2/src/mock_call_where.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:00:57.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 21:00:58.000000 mock_call_where-1.0.2/src/mock_call_where.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:00:58.078295 mock_call_where-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/tests/test_it_works.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-13 21:00:27.000000 mock_call_where-1.0.2/tox.ini
```

### Comparing `mock_call_where-1.0.1/.coveragerc` & `mock_call_where-1.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/.github/workflows/ci.yml` & `mock_call_where-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/.gitignore` & `mock_call_where-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/.pre-commit-config.yaml` & `mock_call_where-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/.readthedocs.yml` & `mock_call_where-1.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/CONTRIBUTING.rst` & `mock_call_where-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/LICENSE.txt` & `mock_call_where-1.0.2/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2024 Collin Sage
+Copyright (c) 2024 MrCocoDev
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mock_call_where-1.0.1/PKG-INFO` & `mock_call_where-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mock-call-where
-Version: 1.0.1
+Version: 1.0.2
 Summary: A short little plugin to find where a mock was called!
-Home-page: https://github.com/MrSage/mock-call-where
-Author: Collin Sage
-Author-email: 3229549+MrSage@users.noreply.github.com
+Home-page: https://github.com/MrCocoDev/mock-call-where
+Author: MrCocoDev
+Author-email: 3229549+MrCocoDev@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -47,17 +47,17 @@
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 .. image:: https://img.shields.io/pypi/v/mock-call-where.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/mock-call-where/
-.. image:: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml/badge.svg
+.. image:: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml/badge.svg
     :alt: GitHub Test CI
-    :target: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml
+    :target: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml
 .. image:: https://pepy.tech/badge/mock-call-where/month
     :alt: Monthly Downloads
     :target: https://pepy.tech/project/mock-call-where
 
 |
 
 ===============
```

### Comparing `mock_call_where-1.0.1/README.rst` & `mock_call_where-1.0.2/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 .. image:: https://img.shields.io/pypi/v/mock-call-where.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/mock-call-where/
-.. image:: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml/badge.svg
+.. image:: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml/badge.svg
     :alt: GitHub Test CI
-    :target: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml
+    :target: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml
 .. image:: https://pepy.tech/badge/mock-call-where/month
     :alt: Monthly Downloads
     :target: https://pepy.tech/project/mock-call-where
 
 |
 
 ===============
```

### Comparing `mock_call_where-1.0.1/docs/Makefile` & `mock_call_where-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/docs/conf.py` & `mock_call_where-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/docs/index.rst` & `mock_call_where-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/setup.cfg` & `mock_call_where-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = mock-call-where
 description = A short little plugin to find where a mock was called!
-author = Collin Sage
-author_email = 3229549+MrSage@users.noreply.github.com
+author = MrCocoDev
+author_email = 3229549+MrCocoDev@users.noreply.github.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
-url = https://github.com/MrSage/mock-call-where
+url = https://github.com/MrCocoDev/mock-call-where
 project_urls = 
 	Documentation = https://pyscaffold.org/
 platforms = any
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Framework :: Pytest
 	Intended Audience :: Developers
```

### Comparing `mock_call_where-1.0.1/setup.py` & `mock_call_where-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/src/mock_call_where/__init__.py` & `mock_call_where-1.0.2/src/mock_call_where/__init__.py`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/src/mock_call_where/override.py` & `mock_call_where-1.0.2/src/mock_call_where/override.py`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/src/mock_call_where.egg-info/PKG-INFO` & `mock_call_where-1.0.2/src/mock_call_where.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: mock-call-where
-Version: 1.0.1
+Version: 1.0.2
 Summary: A short little plugin to find where a mock was called!
-Home-page: https://github.com/MrSage/mock-call-where
-Author: Collin Sage
-Author-email: 3229549+MrSage@users.noreply.github.com
+Home-page: https://github.com/MrCocoDev/mock-call-where
+Author: MrCocoDev
+Author-email: 3229549+MrCocoDev@users.noreply.github.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -47,17 +47,17 @@
 
 .. image:: https://img.shields.io/badge/-PyScaffold-005CA0?logo=pyscaffold
     :alt: Project generated with PyScaffold
     :target: https://pyscaffold.org/
 .. image:: https://img.shields.io/pypi/v/mock-call-where.svg
     :alt: PyPI-Server
     :target: https://pypi.org/project/mock-call-where/
-.. image:: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml/badge.svg
+.. image:: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml/badge.svg
     :alt: GitHub Test CI
-    :target: https://github.com/MrSage/mock-call-where/actions/workflows/ci.yml
+    :target: https://github.com/MrCocoDev/mock-call-where/actions/workflows/ci.yml
 .. image:: https://pepy.tech/badge/mock-call-where/month
     :alt: Monthly Downloads
     :target: https://pepy.tech/project/mock-call-where
 
 |
 
 ===============
```

### Comparing `mock_call_where-1.0.1/src/mock_call_where.egg-info/SOURCES.txt` & `mock_call_where-1.0.2/src/mock_call_where.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/tests/test_it_works.py` & `mock_call_where-1.0.2/tests/test_it_works.py`

 * *Files identical despite different names*

### Comparing `mock_call_where-1.0.1/tox.ini` & `mock_call_where-1.0.2/tox.ini`

 * *Files identical despite different names*

