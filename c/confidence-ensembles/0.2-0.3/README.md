# Comparing `tmp/confidence_ensembles-0.2.tar.gz` & `tmp/confidence_ensembles-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidence_ensembles-0.2.tar", last modified: Mon May 13 12:22:33 2024, max compression
+gzip compressed data, was "confidence_ensembles-0.3.tar", last modified: Mon May 13 15:46:36 2024, max compression
```

## Comparing `confidence_ensembles-0.2.tar` & `confidence_ensembles-0.3.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.147713 confidence_ensembles-0.2/
--rw-rw-rw-   0        0        0     1082 2023-12-12 15:23:45.000000 confidence_ensembles-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     5917 2024-05-13 12:22:33.145653 confidence_ensembles-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5397 2023-12-13 09:26:00.000000 confidence_ensembles-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.143669 confidence_ensembles-0.2/confidence_ensembles.egg-info/
--rw-rw-rw-   0        0        0     5917 2024-05-13 12:22:32.000000 confidence_ensembles-0.2/confidence_ensembles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2024-05-13 12:22:32.000000 confidence_ensembles-0.2/confidence_ensembles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:22:32.000000 confidence_ensembles-0.2/confidence_ensembles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-13 12:22:32.000000 confidence_ensembles-0.2/confidence_ensembles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-12-12 15:22:43.000000 confidence_ensembles-0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 12:22:33.147713 confidence_ensembles-0.2/setup.cfg
--rw-rw-rw-   0        0        0      804 2024-05-13 12:19:36.000000 confidence_ensembles-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.020151 confidence_ensembles-0.2/src/
--rw-rw-rw-   0        0        0      145 2023-12-12 15:37:26.000000 confidence_ensembles-0.2/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.091121 confidence_ensembles-0.2/src/classifiers/
--rw-rw-rw-   0        0        0    10790 2023-12-13 11:15:20.000000 confidence_ensembles-0.2/src/classifiers/Classifier.py
--rw-rw-rw-   0        0        0     8114 2024-01-31 17:03:17.000000 confidence_ensembles-0.2/src/classifiers/ConfidenceBagging.py
--rw-rw-rw-   0        0        0     8855 2024-01-31 17:02:44.000000 confidence_ensembles-0.2/src/classifiers/ConfidenceBaggingParallel.py
--rw-rw-rw-   0        0        0    10057 2023-12-13 12:12:53.000000 confidence_ensembles-0.2/src/classifiers/ConfidenceBoosting.py
--rw-rw-rw-   0        0        0       15 2024-05-13 12:18:03.000000 confidence_ensembles-0.2/src/classifiers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.134146 confidence_ensembles-0.2/src/metrics/
--rw-rw-rw-   0        0        0     5040 2023-02-08 11:01:44.000000 confidence_ensembles-0.2/src/metrics/DiversityMetric.py
--rw-rw-rw-   0        0        0     4912 2023-12-12 15:11:21.000000 confidence_ensembles-0.2/src/metrics/EnsembleMetric.py
--rw-rw-rw-   0        0        0       15 2024-05-13 12:18:03.000000 confidence_ensembles-0.2/src/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:22:33.141364 confidence_ensembles-0.2/src/utils/
--rw-rw-rw-   0        0        0       15 2024-05-13 12:18:03.000000 confidence_ensembles-0.2/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3918 2023-11-22 13:17:21.000000 confidence_ensembles-0.2/src/utils/general_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.398405 confidence_ensembles-0.3/
+-rw-rw-rw-   0        0        0     1082 2023-12-12 15:23:45.000000 confidence_ensembles-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     5917 2024-05-13 15:46:36.396410 confidence_ensembles-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5397 2023-12-13 09:26:00.000000 confidence_ensembles-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.190589 confidence_ensembles-0.3/confidence-ensembles/
+-rw-rw-rw-   0        0        0      171 2024-05-13 15:46:07.000000 confidence_ensembles-0.3/confidence-ensembles/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.250605 confidence_ensembles-0.3/confidence-ensembles/classifiers/
+-rw-rw-rw-   0        0        0    10790 2023-12-13 11:15:20.000000 confidence_ensembles-0.3/confidence-ensembles/classifiers/Classifier.py
+-rw-rw-rw-   0        0        0     8114 2024-01-31 17:03:17.000000 confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBagging.py
+-rw-rw-rw-   0        0        0     8855 2024-01-31 17:02:44.000000 confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBaggingParallel.py
+-rw-rw-rw-   0        0        0    10057 2023-12-13 12:12:53.000000 confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBoosting.py
+-rw-rw-rw-   0        0        0       80 2024-05-13 15:43:35.000000 confidence_ensembles-0.3/confidence-ensembles/classifiers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.280666 confidence_ensembles-0.3/confidence-ensembles/metrics/
+-rw-rw-rw-   0        0        0     5040 2023-02-08 11:01:44.000000 confidence_ensembles-0.3/confidence-ensembles/metrics/DiversityMetric.py
+-rw-rw-rw-   0        0        0     4912 2023-12-12 15:11:21.000000 confidence_ensembles-0.3/confidence-ensembles/metrics/EnsembleMetric.py
+-rw-rw-rw-   0        0        0       45 2024-05-13 15:43:48.000000 confidence_ensembles-0.3/confidence-ensembles/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.339861 confidence_ensembles-0.3/confidence-ensembles/tests/
+-rw-rw-rw-   0        0        0       15 2024-05-13 15:45:42.000000 confidence_ensembles-0.3/confidence-ensembles/tests/__init__.py
+-rw-rw-rw-   0        0        0     2598 2023-12-13 13:54:57.000000 confidence_ensembles-0.3/confidence-ensembles/tests/example_supervised.py
+-rw-rw-rw-   0        0        0     2818 2023-12-12 15:11:21.000000 confidence_ensembles-0.3/confidence-ensembles/tests/example_unsupervised.py
+-rw-rw-rw-   0        0        0    12939 2024-01-31 16:02:33.000000 confidence_ensembles-0.3/confidence-ensembles/tests/rq1-2.py
+-rw-rw-rw-   0        0        0    16307 2024-01-31 16:02:33.000000 confidence_ensembles-0.3/confidence-ensembles/tests/rq3.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.358301 confidence_ensembles-0.3/confidence-ensembles/utils/
+-rw-rw-rw-   0        0        0       27 2024-05-13 15:43:57.000000 confidence_ensembles-0.3/confidence-ensembles/utils/__init__.py
+-rw-rw-rw-   0        0        0     3918 2023-11-22 13:17:21.000000 confidence_ensembles-0.3/confidence-ensembles/utils/general_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:46:36.393410 confidence_ensembles-0.3/confidence_ensembles.egg-info/
+-rw-rw-rw-   0        0        0     5917 2024-05-13 15:46:36.000000 confidence_ensembles-0.3/confidence_ensembles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      945 2024-05-13 15:46:36.000000 confidence_ensembles-0.3/confidence_ensembles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:46:36.000000 confidence_ensembles-0.3/confidence_ensembles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 15:46:36.000000 confidence_ensembles-0.3/confidence_ensembles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-12-12 15:22:43.000000 confidence_ensembles-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:46:36.398405 confidence_ensembles-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      804 2024-05-13 15:43:28.000000 confidence_ensembles-0.3/setup.py
```

### Comparing `confidence_ensembles-0.2/LICENSE.txt` & `confidence_ensembles-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/PKG-INFO` & `confidence_ensembles-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidence-ensembles
-Version: 0.2
+Version: 0.3
 Summary: Confidence Ensembles to Improve Classification
 Home-page: https://github.com/tommyippoz/confidence-ensembles
 Author: Tommaso Zoppi
 Author-email: tommaso.zoppi@unitn.it
 Keywords: machine learning,confidence,safety,ensamble
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `confidence_ensembles-0.2/README.md` & `confidence_ensembles-0.3/README.md`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/confidence_ensembles.egg-info/PKG-INFO` & `confidence_ensembles-0.3/confidence_ensembles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidence-ensembles
-Version: 0.2
+Version: 0.3
 Summary: Confidence Ensembles to Improve Classification
 Home-page: https://github.com/tommyippoz/confidence-ensembles
 Author: Tommaso Zoppi
 Author-email: tommaso.zoppi@unitn.it
 Keywords: machine learning,confidence,safety,ensamble
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `confidence_ensembles-0.2/setup.py` & `confidence_ensembles-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='confidence-ensembles',
-     version='0.2',
+     version='0.3',
      scripts=[],
      author="Tommaso Zoppi",
      author_email="tommaso.zoppi@unitn.it",
      description="Confidence Ensembles to Improve Classification",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/tommyippoz/confidence-ensembles",
```

### Comparing `confidence_ensembles-0.2/src/classifiers/Classifier.py` & `confidence_ensembles-0.3/confidence-ensembles/classifiers/Classifier.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/classifiers/ConfidenceBagging.py` & `confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBagging.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/classifiers/ConfidenceBaggingParallel.py` & `confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBaggingParallel.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/classifiers/ConfidenceBoosting.py` & `confidence_ensembles-0.3/confidence-ensembles/classifiers/ConfidenceBoosting.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/metrics/DiversityMetric.py` & `confidence_ensembles-0.3/confidence-ensembles/metrics/DiversityMetric.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/metrics/EnsembleMetric.py` & `confidence_ensembles-0.3/confidence-ensembles/metrics/EnsembleMetric.py`

 * *Files identical despite different names*

### Comparing `confidence_ensembles-0.2/src/utils/general_utils.py` & `confidence_ensembles-0.3/confidence-ensembles/utils/general_utils.py`

 * *Files identical despite different names*

