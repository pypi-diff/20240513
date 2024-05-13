# Comparing `tmp/zeit.nightwatch-1.7.1.tar.gz` & `tmp/zeit_nightwatch-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeit.nightwatch-1.7.1.tar", last modified: Wed Dec 13 09:39:30 2023, max compression
+gzip compressed data, was "zeit_nightwatch-1.8.0.tar", last modified: Mon May 13 08:48:23 2024, max compression
```

## Comparing `zeit.nightwatch-1.7.1.tar` & `zeit_nightwatch-1.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.947535 zeit.nightwatch-1.7.1/
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     1537 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/CHANGES.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     1485 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/LICENSE
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)       78 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/MANIFEST.in
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)    10476 2023-12-13 09:39:30.947819 zeit.nightwatch-1.7.1/PKG-INFO
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     8666 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/README.rst
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)       79 2023-12-13 09:39:30.949075 zeit.nightwatch-1.7.1/setup.cfg
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      867 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/setup.py
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.925118 zeit.nightwatch-1.7.1/src/
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.930967 zeit.nightwatch-1.7.1/src/zeit/
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)       56 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/__init__.py
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.945654 zeit.nightwatch-1.7.1/src/zeit/nightwatch/
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)       92 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/__init__.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     2196 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/jsonreport.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      291 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/playwright.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     2614 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/prometheus.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     3056 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/pytest.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     5876 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/requests.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)     2221 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/src/zeit/nightwatch/selenium.py
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.938873 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)    10476 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/PKG-INFO
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      693 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/SOURCES.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        1 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/dependency_links.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)       52 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/entry_points.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        5 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/namespace_packages.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        1 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/not-zip-safe
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      102 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/requires.txt
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        5 2023-12-13 09:39:30.000000 zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/top_level.txt
-drwxr-xr-x   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)        0 2023-12-13 09:39:30.946735 zeit.nightwatch-1.7.1/tests/
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      556 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/tests/test_basics.py
--rw-r--r--   0 schnerring (1998260604) ZV.ZEIT.DE\Domänen-Benutzer (1553137583)      134 2023-12-13 09:39:29.000000 zeit.nightwatch-1.7.1/tox.ini
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.111441 zeit_nightwatch-1.8.0/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1627 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/CHANGES.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     1485 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/LICENSE
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       78 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/MANIFEST.in
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    10783 2024-05-13 08:48:23.110987 zeit_nightwatch-1.8.0/PKG-INFO
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     8666 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/README.rst
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       79 2024-05-13 08:48:23.112425 zeit_nightwatch-1.8.0/setup.cfg
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      867 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/setup.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.063046 zeit_nightwatch-1.8.0/src/
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.069550 zeit_nightwatch-1.8.0/src/zeit/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       56 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/__init__.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.106926 zeit_nightwatch-1.8.0/src/zeit/nightwatch/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       92 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/__init__.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2196 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/jsonreport.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      291 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/playwright.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2614 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/prometheus.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     3056 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/pytest.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     5908 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/requests.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)     2221 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit/nightwatch/selenium.py
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.110300 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)    10783 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/PKG-INFO
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      693 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)       52 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/entry_points.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        5 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/namespace_packages.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        1 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/not-zip-safe
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      102 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/requires.txt
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)        5 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/top_level.txt
+drwxr-xr-x   0 wolfgang.schnerring   (502) staff       (20)        0 2024-05-13 08:48:23.109751 zeit_nightwatch-1.8.0/tests/
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      556 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/tests/test_basics.py
+-rw-r--r--   0 wolfgang.schnerring   (502) staff       (20)      134 2024-05-13 08:48:22.000000 zeit_nightwatch-1.8.0/tox.ini
```

### Comparing `zeit.nightwatch-1.7.1/CHANGES.txt` & `zeit_nightwatch-1.8.0/CHANGES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 zeit.nightwatch changes
 =======================
 
+1.8.0 (2024-05-13)
+------------------
+
+- Also log HTTP response body, not just headers.
+
+
 1.7.1 (2023-12-13)
 ------------------
 
 - Don't try to json report if no argument was given
 
 
 1.7.0 (2023-12-08)
```

### Comparing `zeit.nightwatch-1.7.1/LICENSE` & `zeit_nightwatch-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/PKG-INFO` & `zeit_nightwatch-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: zeit.nightwatch
-Version: 1.7.1
+Version: 1.8.0
 Summary: pytest helpers for http smoke tests
 Home-page: https://github.com/ZeitOnline/zeit.nightwatch
 Author: Zeit Online
 Author-email: zon-backend@zeit.de
 License: BSD
-Platform: UNKNOWN
 License-File: LICENSE
+Requires-Dist: cssselect
+Requires-Dist: lxml
+Requires-Dist: mechanicalsoup
+Requires-Dist: requests
+Requires-Dist: prometheus_client
+Requires-Dist: pytest
+Requires-Dist: pytest-playwright
+Requires-Dist: selenium
+Requires-Dist: setuptools
 
 .. image:: https://github.com/ZeitOnline/zeit.nightwatch/workflows/Run%20tests/badge.svg
    :alt: Test status badge
 
 
 ===============
 zeit.nightwatch
@@ -221,14 +229,20 @@
       "system_log": "11:37:40 INFO  [zeit.nightwatch.requests][MainThread] > POST http://example.com/something\n..."
     }
 
 
 zeit.nightwatch changes
 =======================
 
+1.8.0 (2024-05-13)
+------------------
+
+- Also log HTTP response body, not just headers.
+
+
 1.7.1 (2023-12-13)
 ------------------
 
 - Don't try to json report if no argument was given
 
 
 1.7.0 (2023-12-08)
@@ -314,9 +328,7 @@
 - Declare namespace package properly
 
 
 1.0.0 (2021-02-11)
 ------------------
 
 - Initial release
-
-
```

### Comparing `zeit.nightwatch-1.7.1/README.rst` & `zeit_nightwatch-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/setup.py` & `zeit_nightwatch-1.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='zeit.nightwatch',
-    version='1.7.1',
+    version='1.8.0',
     author='Zeit Online',
     author_email='zon-backend@zeit.de',
     url='https://github.com/ZeitOnline/zeit.nightwatch',
     description='pytest helpers for http smoke tests',
     long_description='\n\n'.join(
         open(x).read() for x in ['README.rst', 'CHANGES.txt']),
     namespace_packages=['zeit'],
```

### Comparing `zeit.nightwatch-1.7.1/src/zeit/nightwatch/jsonreport.py` & `zeit_nightwatch-1.8.0/src/zeit/nightwatch/jsonreport.py`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/src/zeit/nightwatch/prometheus.py` & `zeit_nightwatch-1.8.0/src/zeit/nightwatch/prometheus.py`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/src/zeit/nightwatch/pytest.py` & `zeit_nightwatch-1.8.0/src/zeit/nightwatch/pytest.py`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/src/zeit/nightwatch/requests.py` & `zeit_nightwatch-1.8.0/src/zeit/nightwatch/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,8 +161,9 @@
         lines = ['< %s %s' % (request.method, request.url)]
         lines.extend(['> %s: %s' % x for x in request.headers.items()])
         lines.append('---')
         resp = {'Status': response.status_code}
         resp.update(response.headers)
         lines.extend(['< %s: %s' % x for x in resp.items()])
         log.info('\n'.join(lines))
+        log.info(response.text)
         return response
```

### Comparing `zeit.nightwatch-1.7.1/src/zeit/nightwatch/selenium.py` & `zeit_nightwatch-1.8.0/src/zeit/nightwatch/selenium.py`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/PKG-INFO` & `zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 Metadata-Version: 2.1
 Name: zeit.nightwatch
-Version: 1.7.1
+Version: 1.8.0
 Summary: pytest helpers for http smoke tests
 Home-page: https://github.com/ZeitOnline/zeit.nightwatch
 Author: Zeit Online
 Author-email: zon-backend@zeit.de
 License: BSD
-Platform: UNKNOWN
 License-File: LICENSE
+Requires-Dist: cssselect
+Requires-Dist: lxml
+Requires-Dist: mechanicalsoup
+Requires-Dist: requests
+Requires-Dist: prometheus_client
+Requires-Dist: pytest
+Requires-Dist: pytest-playwright
+Requires-Dist: selenium
+Requires-Dist: setuptools
 
 .. image:: https://github.com/ZeitOnline/zeit.nightwatch/workflows/Run%20tests/badge.svg
    :alt: Test status badge
 
 
 ===============
 zeit.nightwatch
@@ -221,14 +229,20 @@
       "system_log": "11:37:40 INFO  [zeit.nightwatch.requests][MainThread] > POST http://example.com/something\n..."
     }
 
 
 zeit.nightwatch changes
 =======================
 
+1.8.0 (2024-05-13)
+------------------
+
+- Also log HTTP response body, not just headers.
+
+
 1.7.1 (2023-12-13)
 ------------------
 
 - Don't try to json report if no argument was given
 
 
 1.7.0 (2023-12-08)
@@ -314,9 +328,7 @@
 - Declare namespace package properly
 
 
 1.0.0 (2021-02-11)
 ------------------
 
 - Initial release
-
-
```

### Comparing `zeit.nightwatch-1.7.1/src/zeit.nightwatch.egg-info/SOURCES.txt` & `zeit_nightwatch-1.8.0/src/zeit.nightwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zeit.nightwatch-1.7.1/tests/test_basics.py` & `zeit_nightwatch-1.8.0/tests/test_basics.py`

 * *Files identical despite different names*

