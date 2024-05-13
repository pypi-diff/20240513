# Comparing `tmp/polyssifier-1.0.8.tar.gz` & `tmp/polyssifier-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyssifier-1.0.8.tar", last modified: Tue Feb 20 01:40:30 2024, max compression
+gzip compressed data, was "polyssifier-1.0.9.tar", last modified: Tue Feb 20 01:52:30 2024, max compression
```

## Comparing `polyssifier-1.0.8.tar` & `polyssifier-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:40:30.748247 polyssifier-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-20 01:40:30.000000 polyssifier-1.0.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-02-20 01:40:30.000000 polyssifier-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-20 01:40:30.748247 polyssifier-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-20 01:40:30.000000 polyssifier-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:40:30.748247 polyssifier-1.0.8/polyssifier/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier/poly_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier/polyssifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:40:30.748247 polyssifier-1.0.8/polyssifier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-20 01:40:30.000000 polyssifier-1.0.8/polyssifier.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-20 01:40:30.748247 polyssifier-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-20 01:40:30.000000 polyssifier-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:40:30.748247 polyssifier-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-02-20 01:40:30.000000 polyssifier-1.0.8/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-20 01:40:30.000000 polyssifier-1.0.8/tests/test_multiclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-20 01:40:30.000000 polyssifier-1.0.8/tests/test_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-20 01:40:30.000000 polyssifier-1.0.8/tests/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:52:30.506574 polyssifier-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-20 01:52:30.000000 polyssifier-1.0.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18027 2024-02-20 01:52:30.000000 polyssifier-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-20 01:52:30.506574 polyssifier-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-02-20 01:52:30.000000 polyssifier-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:52:30.502575 polyssifier-1.0.9/polyssifier/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier/poly_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21837 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier/polyssifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:52:30.506574 polyssifier-1.0.9/polyssifier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-20 01:52:30.000000 polyssifier-1.0.9/polyssifier.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-20 01:52:30.506574 polyssifier-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-02-20 01:52:30.000000 polyssifier-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 01:52:30.506574 polyssifier-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-02-20 01:52:30.000000 polyssifier-1.0.9/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-20 01:52:30.000000 polyssifier-1.0.9/tests/test_multiclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-20 01:52:30.000000 polyssifier-1.0.9/tests/test_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-02-20 01:52:30.000000 polyssifier-1.0.9/tests/test_regression.py
```

### Comparing `polyssifier-1.0.8/LICENSE` & `polyssifier-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/PKG-INFO` & `polyssifier-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyssifier
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data exploration tool for assessing optimal classification methods
 Home-page: https://github.com/alvarouc/polyssifier
 Author: Alvaro Ulloa
 Author-email: alvarouc@gmail.com
 License: GPLv3
 Keywords: classification machine learning data science
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polyssifier-1.0.8/README.md` & `polyssifier-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/polyssifier/logger.py` & `polyssifier-1.0.9/polyssifier/logger.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/polyssifier/poly_utils.py` & `polyssifier-1.0.9/polyssifier/poly_utils.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/polyssifier/polyssifier.py` & `polyssifier-1.0.9/polyssifier/polyssifier.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/polyssifier/report.py` & `polyssifier-1.0.9/polyssifier/report.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/polyssifier.egg-info/PKG-INFO` & `polyssifier-1.0.9/polyssifier.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyssifier
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data exploration tool for assessing optimal classification methods
 Home-page: https://github.com/alvarouc/polyssifier
 Author: Alvaro Ulloa
 Author-email: alvarouc@gmail.com
 License: GPLv3
 Keywords: classification machine learning data science
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `polyssifier-1.0.8/setup.py` & `polyssifier-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/tests/test_classification.py` & `polyssifier-1.0.9/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/tests/test_multiclass.py` & `polyssifier-1.0.9/tests/test_multiclass.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/tests/test_polynomial.py` & `polyssifier-1.0.9/tests/test_polynomial.py`

 * *Files identical despite different names*

### Comparing `polyssifier-1.0.8/tests/test_regression.py` & `polyssifier-1.0.9/tests/test_regression.py`

 * *Files identical despite different names*

