# Comparing `tmp/smadi-1.0.0.tar.gz` & `tmp/smadi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smadi-1.0.0.tar", last modified: Mon Apr 22 22:44:25 2024, max compression
+gzip compressed data, was "smadi-1.0.1.tar", last modified: Mon May 13 10:47:16 2024, max compression
```

## Comparing `smadi-1.0.0.tar` & `smadi-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,53 @@
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/
--rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-1.0.0/.coveragerc
--rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-1.0.0/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-1.0.0/.readthedocs.yml
--rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-1.0.0/AUTHORS.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      128 2024-03-30 14:53:43.000000 smadi-1.0.0/CHANGELOG.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-1.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-1.0.0/LICENSE.txt
--rw-r--r--   0 m294      (1000) m294      (1000)     5297 2024-04-22 22:44:25.770442 smadi-1.0.0/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     3848 2024-04-22 22:42:47.000000 smadi-1.0.0/README.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.742442 smadi-1.0.0/docs/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/Makefile
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.758442 smadi-1.0.0/docs/_static/
--rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/_static/.gitignore
--rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/authors.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/changelog.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 20:04:41.000000 smadi-1.0.0/docs/conf.py
--rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/contributing.rst
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.758442 smadi-1.0.0/docs/examples/
--rw-rw-r--   0 m294      (1000) m294      (1000)     2726 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/Installation.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)     9238 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/Loading_data.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)    43432 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/compute_climatology.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)  1280907 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/detect_the_anomlies.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)   694911 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/plot_climatology.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)   819526 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/examples/workflow.ipynb
--rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/index.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)     2642 2024-04-22 22:42:47.000000 smadi-1.0.0/docs/introduction.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/license.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-1.0.0/docs/readme.rst
--rw-rw-r--   0 m294      (1000) m294      (1000)      231 2024-04-03 20:04:36.000000 smadi-1.0.0/docs/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-1.0.0/pyproject.toml
--rw-rw-r--   0 m294      (1000) m294      (1000)      301 2024-04-03 02:37:06.000000 smadi-1.0.0/requirements.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)     1509 2024-04-22 22:44:25.770442 smadi-1.0.0/setup.cfg
--rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-04-22 22:43:11.000000 smadi-1.0.0/setup.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.686442 smadi-1.0.0/src/
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.762442 smadi-1.0.0/src/smadi/
--rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-1.0.0/src/smadi/__init__.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    22743 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/anomaly_detectors.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    18044 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     7512 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/data_reader.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     9168 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4472 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/map.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2420 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/metadata.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     8206 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/plot.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     9108 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/preprocess.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     4964 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/utils.py
--rw-rw-r--   0 m294      (1000) m294      (1000)    19724 2024-04-22 22:42:47.000000 smadi-1.0.0/src/smadi/workflow.py
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/src/smadi.egg-info/
--rw-r--r--   0 m294      (1000) m294      (1000)     5297 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/PKG-INFO
--rw-rw-r--   0 m294      (1000) m294      (1000)     1149 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/SOURCES.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/dependency_links.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/entry_points.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/not-zip-safe
--rw-rw-r--   0 m294      (1000) m294      (1000)      343 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/requires.txt
--rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-04-22 22:44:25.000000 smadi-1.0.0/src/smadi.egg-info/top_level.txt
-drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-04-22 22:44:25.770442 smadi-1.0.0/tests/
--rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-1.0.0/tests/conftest.py
--rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-1.0.0/tests/data_sample.csv
--rw-rw-r--   0 m294      (1000) m294      (1000)    20040 2024-04-22 22:42:47.000000 smadi-1.0.0/tests/test_climatology.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-1.0.0/tests/test_indicators.py
--rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-1.0.0/tox.ini
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.789512 smadi-1.0.1/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      588 2024-03-30 14:53:43.000000 smadi-1.0.1/.coveragerc
+-rw-rw-r--   0 m294      (1000) m294      (1000)      566 2024-03-30 14:53:43.000000 smadi-1.0.1/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)      530 2024-03-30 14:53:43.000000 smadi-1.0.1/.readthedocs.yml
+-rw-rw-r--   0 m294      (1000) m294      (1000)       85 2024-03-30 14:53:43.000000 smadi-1.0.1/AUTHORS.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      359 2024-04-23 14:00:00.000000 smadi-1.0.1/CHANGELOG.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)    13788 2024-03-30 14:53:43.000000 smadi-1.0.1/CONTRIBUTING.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1079 2024-03-30 14:53:43.000000 smadi-1.0.1/LICENSE.txt
+-rw-r--r--   0 m294      (1000) m294      (1000)     5317 2024-05-13 10:47:16.789512 smadi-1.0.1/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)     3848 2024-04-22 22:42:47.000000 smadi-1.0.1/README.rst
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.737516 smadi-1.0.1/docs/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1154 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/Makefile
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.761515 smadi-1.0.1/docs/_static/
+-rw-rw-r--   0 m294      (1000) m294      (1000)       18 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/_static/.gitignore
+-rw-rw-r--   0 m294      (1000) m294      (1000)       41 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/authors.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       43 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/changelog.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9748 2024-04-03 20:04:41.000000 smadi-1.0.1/docs/conf.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)       33 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/contributing.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2305 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/index.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2642 2024-04-22 22:42:47.000000 smadi-1.0.1/docs/introduction.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       67 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/license.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)       39 2024-03-30 14:53:43.000000 smadi-1.0.1/docs/readme.rst
+-rw-rw-r--   0 m294      (1000) m294      (1000)      231 2024-04-03 20:04:36.000000 smadi-1.0.1/docs/requirements.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)      346 2024-03-30 14:53:43.000000 smadi-1.0.1/pyproject.toml
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1515 2024-05-13 10:47:16.789512 smadi-1.0.1/setup.cfg
+-rw-rw-r--   0 m294      (1000) m294      (1000)      836 2024-05-13 10:38:14.000000 smadi-1.0.1/setup.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.693520 smadi-1.0.1/src/
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.761515 smadi-1.0.1/src/smadi/
+-rw-rw-r--   0 m294      (1000) m294      (1000)      577 2024-03-30 14:53:43.000000 smadi-1.0.1/src/smadi/__init__.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    22743 2024-04-24 10:32:23.000000 smadi-1.0.1/src/smadi/anomaly_detectors.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    18026 2024-05-06 13:03:06.000000 smadi-1.0.1/src/smadi/climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     7512 2024-04-22 22:42:47.000000 smadi-1.0.1/src/smadi/data_reader.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9168 2024-04-22 22:42:47.000000 smadi-1.0.1/src/smadi/indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4876 2024-05-03 16:49:37.000000 smadi-1.0.1/src/smadi/map.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2814 2024-05-05 21:53:43.000000 smadi-1.0.1/src/smadi/metadata.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     8206 2024-04-22 22:42:47.000000 smadi-1.0.1/src/smadi/plot.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     9108 2024-04-22 22:42:47.000000 smadi-1.0.1/src/smadi/preprocess.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     4964 2024-04-22 22:42:47.000000 smadi-1.0.1/src/smadi/utils.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)    19541 2024-05-08 20:25:32.000000 smadi-1.0.1/src/smadi/workflow.py
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.785513 smadi-1.0.1/src/smadi.egg-info/
+-rw-r--r--   0 m294      (1000) m294      (1000)     5317 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/PKG-INFO
+-rw-rw-r--   0 m294      (1000) m294      (1000)      920 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/SOURCES.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/dependency_links.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)       44 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/entry_points.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        1 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/not-zip-safe
+-rw-rw-r--   0 m294      (1000) m294      (1000)      348 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/requires.txt
+-rw-rw-r--   0 m294      (1000) m294      (1000)        6 2024-05-13 10:47:16.000000 smadi-1.0.1/src/smadi.egg-info/top_level.txt
+drwxrwxr-x   0 m294      (1000) m294      (1000)        0 2024-05-13 10:47:16.785513 smadi-1.0.1/tests/
+-rw-rw-r--   0 m294      (1000) m294      (1000)     1117 2024-03-30 15:11:41.000000 smadi-1.0.1/tests/conftest.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)   360610 2024-03-25 13:18:42.000000 smadi-1.0.1/tests/data_sample.csv
+-rw-rw-r--   0 m294      (1000) m294      (1000)    20040 2024-04-22 22:42:47.000000 smadi-1.0.1/tests/test_climatology.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2211 2024-03-30 14:58:43.000000 smadi-1.0.1/tests/test_indicators.py
+-rw-rw-r--   0 m294      (1000) m294      (1000)     2851 2024-03-30 14:53:43.000000 smadi-1.0.1/tox.ini
```

### Comparing `smadi-1.0.0/.coveragerc` & `smadi-1.0.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/.gitignore` & `smadi-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/.readthedocs.yml` & `smadi-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/CONTRIBUTING.rst` & `smadi-1.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/LICENSE.txt` & `smadi-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/PKG-INFO` & `smadi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
@@ -40,14 +40,15 @@
 Requires-Dist: fibgrid
 Requires-Dist: datashader
 Requires-Dist: pycountry
 Requires-Dist: PyQt5
 Requires-Dist: PySide2
 Requires-Dist: mapclassify
 Requires-Dist: standard-precip
+Requires-Dist: tqdm
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
```

### Comparing `smadi-1.0.0/README.rst` & `smadi-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/docs/Makefile` & `smadi-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/docs/conf.py` & `smadi-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/docs/index.rst` & `smadi-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/docs/introduction.rst` & `smadi-1.0.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/setup.cfg` & `smadi-1.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 	fibgrid
 	datashader
 	pycountry
 	PyQt5
 	PySide2
 	mapclassify
 	standard-precip
+	tqdm
 	importlib-metadata; python_version<"3.8"
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `smadi-1.0.0/setup.py` & `smadi-1.0.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 from setuptools import setup
 
 if __name__ == "__main__":
     try:
         setup(
-            version="1.0.0",
+            version="1.0.1",
             entry_points={
                 "console_scripts": [
                     "run = smadi.workflow:main",
                 ]
             },
         )
```

### Comparing `smadi-1.0.0/src/smadi/__init__.py` & `smadi-1.0.1/src/smadi/__init__.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/anomaly_detectors.py` & `smadi-1.0.1/src/smadi/anomaly_detectors.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/climatology.py` & `smadi-1.0.1/src/smadi/climatology.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
             smooth_window_size,
             timespan,
             agg_metric,
         )
 
     def aggregate(self, **kwargs):
         self.resulted_df[f"{self.var}-{self.agg_metric}"] = self.df[self.var]
-        return filter_df(self.resulted_df.drop_duplicates(), **kwargs)
+        return filter_df(self.resulted_df, **kwargs)
 
 
 class Climatology(Aggregator):
     """
     A class for calculating climatology(climate normal) for time series data.
 
     Attributes:
```

### Comparing `smadi-1.0.0/src/smadi/data_reader.py` & `smadi-1.0.1/src/smadi/data_reader.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/indicators.py` & `smadi-1.0.1/src/smadi/indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/map.py` & `smadi-1.0.1/src/smadi/map.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import eomaps
 import pandas as pd
-
+from tqdm import tqdm
 
 from smadi.plot import set_thresholds
 
 
 def set_extent(df, x="lon", y="lat", buffer=2):
     """
     Set the extent for the map based on the provided dataframe and buffer.
@@ -77,41 +77,52 @@
         "y": 0.95,
         "fontsize": 15,
         "ha": "center",
         "va": "center",
         "fontweight": "bold",
     },
     maps_titles=None,
-    maps_titles_kwargs={"pad": 13, "fontsize": 12, "fontweight": "bold"},
+    maps_titles_kwargs={"pad": 11, "fontsize": 10, "fontweight": "bold"},
     add_features=True,
     frame_line_width=1,
+    add_cb=True,
     cb_min_max=["sm_clim", "sm_clim", "abs", "anomaly", "anomaly"],
     cmap="RdYlBu",
     vmin=None,
     vmax=None,
     add_gridlines=False,
     cb_kwargs={
         "pos": 0.4,
         "labelsize": 0.5,
         "tick_lines": "center",
         "show_values": False,
     },
     cb_label=None,
+    save_to=None,
 ):
     m = eomaps.Maps(ax=(ax_rows, ax_cols, 1), figsize=figsize, crs=map_crs)
     figure_title_kwargs["s"] = figure_title
     m.text(**figure_title_kwargs)
 
-    for i, (colm, cb_min_max) in enumerate(zip(df_colms, cb_min_max)):
+    total_iterations = len(df_colms)
+
+    for i, (colm, cb_min_max) in tqdm(
+        enumerate(zip(df_colms, cb_min_max)),
+        total=total_iterations,
+        desc="Processing maps",
+    ):
         ax_index = i + 1
         if i == 0:
             m = m
         else:
             m = m.new_map(ax=(ax_rows, ax_cols, ax_index), figsize=(7, 7), crs=map_crs)
-        m.ax.set_title(maps_titles[i], **maps_titles_kwargs)
+
+        if maps_titles:
+            m.ax.set_title(maps_titles[i], **maps_titles_kwargs)
+
         m.set_shape.rectangles(radius=0.05)
         if add_features:
             m.add_feature.preset.coastline(lw=0.6)
             m.add_feature.preset.countries(lw=0.4, ls="--")
             m.add_feature.preset.ocean()
             m.add_feature.preset.land()
 
@@ -144,23 +155,31 @@
             vmin = -1
             vmax = 1
 
         if colm.split("(")[0] == "smds":
             cmap = cmap + "_r"
 
         m.plot_map(vmin=vmin, vmax=vmax, cmap=cmap, lw=1.5)
-        label = cb_label[i] if cb_label else colm
-        cb = m.add_colorbar(
-            label=label, spacing="uniform", pos=0.4, orientation="vertical"
-        )
-        cb.set_hist_size(0.8)
-        cb.tick_params(rotation=0, labelsize=10, pad=5)
 
-        if cb_min_max == "anomaly":
-            cb.set_bin_labels(
-                bins=bins,
-                names=labels,
-                tick_lines=cb_kwargs["tick_lines"],
-                show_values=cb_kwargs["show_values"],
+        if add_cb:
+            label = cb_label[i] if cb_label else None
+            cb = m.add_colorbar(
+                label=label,
+                spacing="uniform",
+                pos=0.4,
+                orientation="vertical",
+                hist_bins=256,
             )
+            cb.set_hist_size(0.8)
+            cb.tick_params(rotation=0, labelsize=10, pad=5)
+
+            if cb_min_max == "anomaly":
+                cb.set_bin_labels(
+                    bins=bins,
+                    names=labels,
+                    tick_lines=cb_kwargs["tick_lines"],
+                    show_values=cb_kwargs["show_values"],
+                )
 
     m.show()
+    if save_to:
+        m.savefig(save_to)
```

### Comparing `smadi-1.0.0/src/smadi/metadata.py` & `smadi-1.0.1/src/smadi/metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,45 +5,45 @@
         "D-1": (-1.5, -1),
         "NN": (-1, 1),
         "W-1": (1, 1.5),
         "W-2": (1.5, 2),
         "W-3": (2, 3),
     },
     "smapi": {
-        "D-4": (-100, -50),
-        "D-3": (-50, -30),
-        "D-2": (-30, -15),
+        "D-4": (-100, -25),
+        "D-3": (-25, -20),
+        "D-2": (-20, -15),
         "D-1": (-15, -5),
         "NN": (-5, 5),
         "W-1": (5, 15),
-        "W-2": (15, 30),
-        "W-3": (30, 50),
-        "W-4": (50, 100),
+        "W-2": (15, 20),
+        "W-3": (20, 25),
+        "W-4": (25, 100),
     },
     "smdi": {
         "D-4": (-4, -3),
         "D-3": (-3, -2),
         "D-2": (-2, -1),
         "D-1": (-1, -0.5),
         "NN": (-0.5, 0.5),
         "W-1": (0.5, 1),
         "W-2": (1, 2),
         "W-3": (2, 3),
         "W-4": (3, 4),
     },
     "smds": {
-        "W-4": (0, 0.02),
+        # "W-4": (0, 0.02),
         "W-3": (0.02, 0.05),
         "W-2": (0.05, 0.10),
         "W-1": (0.10, 0.20),
         "NN": (0.20, 0.80),
         "D-1": (0.80, 0.90),
         "D-2": (0.90, 0.95),
         "D-3": (0.95, 0.98),
-        "D-4": (0.98, 1),
+        # "D-4": (0.98, 1),
     },
     "smci": {
         "D-4": (0, 0.02),
         "D-3": (0.02, 0.05),
         "D-2": (0.05, 0.10),
         "D-1": (0.10, 0.20),
         "NN": (0.20, 0.80),
@@ -95,9 +95,27 @@
         "D-3": (-3, -2),
         "D-2": (-2, -1.5),
         "D-1": (-1.5, -1),
         "NN": (-1, 1),
         "W-1": (1, 1.5),
         "W-2": (1.5, 2),
         "W-3": (2, 3),
+    },
+    "spi": {
+        "D-3": (-3, -2),
+        "D-2": (-2, -1.5),
+        "D-1": (-1.5, -1),
+        "NN": (-1, 1),
+        "W-1": (1, 1.5),
+        "W-2": (1.5, 2),
+        "W-3": (2, 3),
+    },
+    "sma": {
+        "D-3": (-3, -2),
+        "D-2": (-2, -1.5),
+        "D-1": (-1.5, -1),
+        "NN": (-1, 1),
+        "W-1": (1, 1.5),
+        "W-2": (1.5, 2),
+        "W-3": (2, 3),
     },
 }
```

### Comparing `smadi-1.0.0/src/smadi/plot.py` & `smadi-1.0.1/src/smadi/plot.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/preprocess.py` & `smadi-1.0.1/src/smadi/preprocess.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/utils.py` & `smadi-1.0.1/src/smadi/utils.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/src/smadi/workflow.py` & `smadi-1.0.1/src/smadi/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 
 from argparse import ArgumentParser, Namespace, ArgumentError
 from typing import List, Tuple, Union, Dict
 from concurrent.futures import ProcessPoolExecutor
 from functools import partial
 import pandas as pd
 import numpy as np
+from tqdm import tqdm
 
 
 from smadi.data_reader import AscatData, read_era5
+from smadi.preprocess import filter_df
 from smadi.utils import (
     create_logger,
     log_exception,
     log_time,
     load_gpis_by_country,
     get_gpis_from_bbox,
 )
@@ -234,14 +236,18 @@
         "save_to": args.save_to,
     }
     return parsed_args
 
 
 # Create a logger
 logger = create_logger("workflow-logger")
+parser = setup_argument_parser()
+args = parse_arguments(parser)
+global ascat_obj
+ascat_obj = AscatData(args["data_path"], args["data_read_bulk"])
 
 
 @log_exception(logger)
 def load_ts(gpi, variable="sm"):
     """
     Load ASCAT time series for a given gpi
     """
@@ -418,19 +424,14 @@
 ):
     """
     Validate and retrieve additional parameters from the anomaly dataframe.
     """
 
     if addi_retrive is not None:
 
-        # if not all(value in ["var", "norm"] for value in addi_retrive):
-        #     raise ValueError(
-        #         "The additional retrieval parameters must be one of the following: 'var', 'norm'"
-        #     )
-
         if "var" in addi_retrive:
             results[f"{variable}-{agg_metric}" + f"({date_str})"] = anomaly[
                 f"{variable}-{agg_metric}"
             ].values
         if "norm" in addi_retrive:
             if "norm-mean" in anomaly.columns:
                 results["norm-mean" + f"({date_str})"] = anomaly["norm-mean"].values
@@ -467,16 +468,14 @@
     dekad: Union[int, List[int]] = None,
     week: Union[int, List[int]] = None,
     bimonth: Union[int, List[int]] = None,
     day: Union[int, List[int]] = None,
     timespan: List[str] = None,
     addi_retrive: list = ["var", "norm"],
     agg_metric: list = "mean",
-    mode: str = "anomaly",
-    era5_path: str = None,
 ) -> Tuple[int, Dict[str, float]]:
     """
     Run the anomaly detection workflow for a single grid point index.
     """
 
     # Load the time series for the given gpi
     global ascat_obj
@@ -511,33 +510,29 @@
         if "-" in method:
             anomaly_params["normal_metrics"] = [method.split("-")[1]]
 
         elif method in ["beta", "gamma"]:
             anomaly_params["dist"] = [method]
 
         try:
-            for date_param in date_params:
-                anomaly = _Detectors[method](**anomaly_params).detect_anomaly(
-                    **date_param
-                )
 
-                # if mode == "anomaly":
+            anomaly = _Detectors[method](**anomaly_params).detect_anomaly()
+            for date_param in date_params:
+                anomaly_df = filter_df(anomaly, **date_param)
                 date_str = f"-".join(str(value) for value in date_param.values())
-                results[method + f"({date_str})"] = anomaly[method].values
+                results[method + f"({date_str})"] = anomaly_df[method].values
 
                 results = addi_retrival(
                     addi_retrive=addi_retrive,
                     results=results,
-                    anomaly=anomaly,
+                    anomaly=anomaly_df,
                     variable=variable,
                     date_str=date_str,
                     agg_metric=agg_metric,
                 )
-                # elif mode == "spi":
-                #     era5_df = read_era5(era5_path, loc=(lon, lat))
 
         except AttributeError as e:
             return None
 
     return (gpi, results)
 
 
@@ -582,14 +577,17 @@
     logger.info(f"Loading grid points for {aoi}....")
 
     if isinstance(aoi, str):
         pointlist = load_gpis_by_country(aoi)
     else:
         pointlist = get_gpis_from_bbox(aoi)
 
+    pointlist = pointlist.drop(2933)
+    pointlist = pointlist.drop(3210)
+    pointlist = pointlist.drop(812)
     logger.info(f"Grid points loaded successfully for {aoi}\n")
     logger.info(f"\n\n{pointlist.head()}")
     pre_compute = partial(
         single_po_run,
         methods=methods,
         variable=variable,
         time_step=time_step,
@@ -624,30 +622,26 @@
         "Day": day,
     }
     for param, value in date_parameters.items():
         if value:
             logger.info(f"     {param}: {value}")
 
     with ProcessPoolExecutor(workers) as executor:
-        results = executor.map(pre_compute, pointlist["point"])
+        results = list(
+            tqdm(executor.map(pre_compute, pointlist["point"]), total=len(pointlist))
+        )
+        # results = executor.map(pre_compute, pointlist["point"])
         for result in results:
             pointlist = _finalize(result, pointlist)
 
         return pointlist
 
 
 def main():
 
-    parser = setup_argument_parser()
-    args = parse_arguments(parser)
-
-    # Create an instance of the AscatData class
-    global ascat_obj
-    ascat_obj = AscatData(args["data_path"], args["data_read_bulk"])
-
     try:
         validate_anomaly_method(args["methods"])
         validate_date_params(
             args["time_step"],
             args["year"],
             args["month"],
             args["dekad"],
```

### Comparing `smadi-1.0.0/src/smadi.egg-info/PKG-INFO` & `smadi-1.0.1/src/smadi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smadi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Add a short description here!
 Home-page: https://github.com/MuhammedM294/smadi
 Author: MuhammedM294
 Author-email: muhammedaabdelaal@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Project-URL: Source, https://github.com/MuhammedM294/smadi
@@ -40,14 +40,15 @@
 Requires-Dist: fibgrid
 Requires-Dist: datashader
 Requires-Dist: pycountry
 Requires-Dist: PyQt5
 Requires-Dist: PySide2
 Requires-Dist: mapclassify
 Requires-Dist: standard-precip
+Requires-Dist: tqdm
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
```

### Comparing `smadi-1.0.0/src/smadi.egg-info/SOURCES.txt` & `smadi-1.0.1/src/smadi.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -3,35 +3,28 @@
 .readthedocs.yml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE.txt
 README.rst
 pyproject.toml
-requirements.txt
 setup.cfg
 setup.py
 tox.ini
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/introduction.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
-docs/examples/Installation.ipynb
-docs/examples/Loading_data.ipynb
-docs/examples/compute_climatology.ipynb
-docs/examples/detect_the_anomlies.ipynb
-docs/examples/plot_climatology.ipynb
-docs/examples/workflow.ipynb
 src/smadi/__init__.py
 src/smadi/anomaly_detectors.py
 src/smadi/climatology.py
 src/smadi/data_reader.py
 src/smadi/indicators.py
 src/smadi/map.py
 src/smadi/metadata.py
```

### Comparing `smadi-1.0.0/tests/conftest.py` & `smadi-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/tests/data_sample.csv` & `smadi-1.0.1/tests/data_sample.csv`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/tests/test_climatology.py` & `smadi-1.0.1/tests/test_climatology.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/tests/test_indicators.py` & `smadi-1.0.1/tests/test_indicators.py`

 * *Files identical despite different names*

### Comparing `smadi-1.0.0/tox.ini` & `smadi-1.0.1/tox.ini`

 * *Files identical despite different names*

