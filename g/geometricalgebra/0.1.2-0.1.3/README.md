# Comparing `tmp/geometricalgebra-0.1.2.tar.gz` & `tmp/geometricalgebra-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geometricalgebra-0.1.2.tar", max compression
+gzip compressed data, was "geometricalgebra-0.1.3.tar", max compression
```

## Comparing `geometricalgebra-0.1.2.tar` & `geometricalgebra-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1072 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/LICENSE
--rw-r--r--   0        0        0      837 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/README.md
--rw-r--r--   0        0        0       84 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/__init__.py
--rw-r--r--   0        0        0     8605 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/algebra.py
--rw-r--r--   0        0        0     3110 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cayley.py
--rw-r--r--   0        0        0    39904 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga.py
--rw-r--r--   0        0        0      982 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga2d.py
--rw-r--r--   0        0        0     6061 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga3d.py
--rw-r--r--   0        0        0     1347 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/cga4d.py
--rw-r--r--   0        0        0     2853 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/coherent_point_drift.py
--rw-r--r--   0        0        0      450 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_algebra.py
--rw-r--r--   0        0        0    16229 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_cayley.py
--rw-r--r--   0        0        0     1476 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_coherent_point_drift.py
--rw-r--r--   0        0        0      533 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_gradient.py
--rw-r--r--   0        0        0     1378 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_quaterion_interpolation.py
--rw-r--r--   0        0        0     2189 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_tensorflow.py
--rw-r--r--   0        0        0     7162 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_vector.py
--rw-r--r--   0        0        0    11381 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/tests/test_versor.py
--rw-r--r--   0        0        0      280 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/utils.py
--rw-r--r--   0        0        0    28069 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/vector.py
--rw-r--r--   0        0        0     8139 2024-04-05 09:55:07.346896 geometricalgebra-0.1.2/geometricalgebra/viewer.py
--rw-r--r--   0        0        0     1777 2024-04-05 09:55:07.354896 geometricalgebra-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1647 1970-01-01 00:00:00.000000 geometricalgebra-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-13 09:40:28.020307 geometricalgebra-0.1.3/LICENSE
+-rw-r--r--   0        0        0      837 2024-05-13 09:40:28.020307 geometricalgebra-0.1.3/README.md
+-rw-r--r--   0        0        0       84 2024-05-13 09:40:28.020307 geometricalgebra-0.1.3/geometricalgebra/__init__.py
+-rw-r--r--   0        0        0     8605 2024-05-13 09:40:28.020307 geometricalgebra-0.1.3/geometricalgebra/algebra.py
+-rw-r--r--   0        0        0     3110 2024-05-13 09:40:28.020307 geometricalgebra-0.1.3/geometricalgebra/cayley.py
+-rw-r--r--   0        0        0    39904 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/cga.py
+-rw-r--r--   0        0        0      982 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/cga2d.py
+-rw-r--r--   0        0        0     6061 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/cga3d.py
+-rw-r--r--   0        0        0     1347 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/cga4d.py
+-rw-r--r--   0        0        0     2853 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/coherent_point_drift.py
+-rw-r--r--   0        0        0      450 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_algebra.py
+-rw-r--r--   0        0        0    16229 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_cayley.py
+-rw-r--r--   0        0        0     1476 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_coherent_point_drift.py
+-rw-r--r--   0        0        0      533 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_gradient.py
+-rw-r--r--   0        0        0     1378 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_quaterion_interpolation.py
+-rw-r--r--   0        0        0     2189 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_tensorflow.py
+-rw-r--r--   0        0        0     7162 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_vector.py
+-rw-r--r--   0        0        0    11381 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/tests/test_versor.py
+-rw-r--r--   0        0        0      280 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/utils.py
+-rw-r--r--   0        0        0    28069 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/vector.py
+-rw-r--r--   0        0        0     8139 2024-05-13 09:40:28.024307 geometricalgebra-0.1.3/geometricalgebra/viewer.py
+-rw-r--r--   0        0        0     1806 2024-05-13 09:40:28.028307 geometricalgebra-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1623 1970-01-01 00:00:00.000000 geometricalgebra-0.1.3/PKG-INFO
```

### Comparing `geometricalgebra-0.1.2/LICENSE` & `geometricalgebra-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/README.md` & `geometricalgebra-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/algebra.py` & `geometricalgebra-0.1.3/geometricalgebra/algebra.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/cayley.py` & `geometricalgebra-0.1.3/geometricalgebra/cayley.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/cga.py` & `geometricalgebra-0.1.3/geometricalgebra/cga.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/cga2d.py` & `geometricalgebra-0.1.3/geometricalgebra/cga2d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/cga3d.py` & `geometricalgebra-0.1.3/geometricalgebra/cga3d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/cga4d.py` & `geometricalgebra-0.1.3/geometricalgebra/cga4d.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/coherent_point_drift.py` & `geometricalgebra-0.1.3/geometricalgebra/coherent_point_drift.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_cayley.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_cayley.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_coherent_point_drift.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_coherent_point_drift.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_gradient.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_quaterion_interpolation.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_quaterion_interpolation.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_tensorflow.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_vector.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/tests/test_versor.py` & `geometricalgebra-0.1.3/geometricalgebra/tests/test_versor.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/vector.py` & `geometricalgebra-0.1.3/geometricalgebra/vector.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/geometricalgebra/viewer.py` & `geometricalgebra-0.1.3/geometricalgebra/viewer.py`

 * *Files identical despite different names*

### Comparing `geometricalgebra-0.1.2/pyproject.toml` & `geometricalgebra-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 [tool.poetry]
 name = "geometricalgebra"
-version = '0.1.2'
+version = '0.1.3'
 description = "A package for conformal geometric algebra"
 authors = [
     "Daniel Vorberg <daniel.vorberg@wandelbots.com>",
+    "Patrick Schmager <patrick.schmager@wandelbots.com>",
+    "Christoph Biering <christoph.biering@wandelbots.com>",
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = "^3.9"
 numpy = ">=1.19.0"
 scipy = ">=1.8.0"
-tensorflow = { version = "2.14.0", optional = true, platform = "linux" }
-tensorflow-macos = { version = "2.14.1", optional = true, platform = "darwin"}
+tensorflow = { version = ">=2.16.1", optional = true }
 matplotlib = { version = ">=3.4.2", optional = true }
-jax = { version = "0.4.10", optional = true }
-jaxlib = { version = "0.4.10", optional = true }
+jax = { version = ">=0.4.27", optional = true }
+jaxlib = { version = ">=0.4.27", optional = true }
 
 
 [tool.poetry.extras]
 all = ["matplotlib", "tensorflow", "tensorflow-macos", "jax", "jaxlib"]
 
 [tool.poetry.group.dev.dependencies]
-pytest = "7.4.4"
-pylint = "2.15.4"
+pytest = "^7.4.4"
+pylint = "^2.15.4"
 mypy = "^1.8.0"
-isort = "5.10.1"
-darglint = "1.8.1"
-black = "24.1.1"
-nbval = "0.10.0"
-pytest-cov = "4.1.0"
-pytest-mpl = "0.16.1"
-pdoc = "12.1.0"
+isort = "^5.10.1"
+darglint = "^1.8.1"
+black = "^24.1.1"
+nbval = "^0.11.0"
+pytest-cov = "^4.1.0"
+pytest-mpl = "^0.16.1"
+jupyter = "^1.0.0"
 
 [tool.mypy]
 python_version = "3.9"
 ignore_missing_imports = true
 warn_unreachable = true
 warn_unused_configs = true
 junit_xml = "reports/mypy/mypy.xml"
```

### Comparing `geometricalgebra-0.1.2/PKG-INFO` & `geometricalgebra-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: geometricalgebra
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for conformal geometric algebra
 Author: Daniel Vorberg
 Author-email: daniel.vorberg@wandelbots.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: all
-Requires-Dist: jax (==0.4.10) ; extra == "all"
-Requires-Dist: jaxlib (==0.4.10) ; extra == "all"
+Requires-Dist: jax (>=0.4.27) ; extra == "all"
+Requires-Dist: jaxlib (>=0.4.27) ; extra == "all"
 Requires-Dist: matplotlib (>=3.4.2) ; extra == "all"
 Requires-Dist: numpy (>=1.19.0)
 Requires-Dist: scipy (>=1.8.0)
-Requires-Dist: tensorflow (==2.14.0) ; (sys_platform == "linux") and (extra == "all")
-Requires-Dist: tensorflow-macos (==2.14.1) ; (sys_platform == "darwin") and (extra == "all")
+Requires-Dist: tensorflow (>=2.16.1) ; extra == "all"
 Description-Content-Type: text/markdown
 
 # geometricalgebra
 
 ![badge](https://github.com/wandelbotsgmbh/geometricalgebra/actions/workflows/python-app.yml/badge.svg)
 
 Library implementing conformal geometric algebra.
```

