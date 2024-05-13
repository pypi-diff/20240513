# Comparing `tmp/pymc_bart-0.5.6.tar.gz` & `tmp/pymc_bart-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymc_bart-0.5.6.tar", last modified: Sat Dec 23 23:59:33 2023, max compression
+gzip compressed data, was "pymc_bart-0.5.7.tar", last modified: Fri Dec 29 16:15:25 2023, max compression
```

## Comparing `pymc_bart-0.5.6.tar` & `pymc_bart-0.5.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11720 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/pymc_bart/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    24188 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/pgbart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/split_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12048 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    30259 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pymc_bart/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/pymc_bart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-23 23:59:33.000000 pymc_bart-0.5.6/pymc_bart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-23 23:59:33.000000 pymc_bart-0.5.6/pymc_bart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 23:59:33.000000 pymc_bart-0.5.6/pymc_bart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-23 23:59:33.000000 pymc_bart-0.5.6/pymc_bart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-23 23:59:33.000000 pymc_bart-0.5.6/pymc_bart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 23:59:33.504013 pymc_bart-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/tests/test_bart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/tests/test_pgbart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/tests/test_split_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-23 23:59:26.000000 pymc_bart-0.5.6/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 16:15:25.739348 pymc_bart-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11720 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-29 16:15:25.739348 pymc_bart-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 16:15:25.735348 pymc_bart-0.5.7/pymc_bart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24205 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12048 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30259 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pymc_bart/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 16:15:25.735348 pymc_bart-0.5.7/pymc_bart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2023-12-29 16:15:25.000000 pymc_bart-0.5.7/pymc_bart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2023-12-29 16:15:25.000000 pymc_bart-0.5.7/pymc_bart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 16:15:25.000000 pymc_bart-0.5.7/pymc_bart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-29 16:15:25.000000 pymc_bart-0.5.7/pymc_bart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-29 16:15:25.000000 pymc_bart-0.5.7/pymc_bart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 16:15:25.739348 pymc_bart-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 16:15:25.735348 pymc_bart-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/tests/test_bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/tests/test_pgbart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/tests/test_split_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-12-29 16:15:18.000000 pymc_bart-0.5.7/tests/test_tree.py
```

### Comparing `pymc_bart-0.5.6/CODE_OF_CONDUCT.md` & `pymc_bart-0.5.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/CONTRIBUTING.md` & `pymc_bart-0.5.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/LICENSE` & `pymc_bart-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/PKG-INFO` & `pymc_bart-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc_bart
-Version: 0.5.6
+Version: 0.5.7
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `pymc_bart-0.5.6/README.md` & `pymc_bart-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/pymc_bart/__init__.py` & `pymc_bart-0.5.7/pymc_bart/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,11 +21,11 @@
     plot_pdp,
     plot_ice,
     plot_dependence,
     plot_variable_importance,
 )
 
 __all__ = ["BART", "PGBART"]
-__version__ = "0.5.6"
+__version__ = "0.5.7"
 
 
 pm.STEP_METHODS = list(pm.STEP_METHODS) + [PGBART]
```

### Comparing `pymc_bart-0.5.6/pymc_bart/bart.py` & `pymc_bart-0.5.7/pymc_bart/bart.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/pymc_bart/pgbart.py` & `pymc_bart-0.5.7/pymc_bart/pgbart.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         if self.bart.split_rules:
             self.split_rules = self.bart.split_rules
         else:
             self.split_rules = [ContinuousSplitRule] * self.X.shape[1]
 
         for idx, rule in enumerate(self.split_rules):
             if rule is ContinuousSplitRule:
-                self.X[:, idx] = jitter_duplicated(self.X[:, idx], np.std(self.X[:, idx]))
+                self.X[:, idx] = jitter_duplicated(self.X[:, idx], np.nanstd(self.X[:, idx]))
 
         init_mean = self.bart.Y.mean()
         self.num_observations = self.X.shape[0]
         self.num_variates = self.X.shape[1]
         self.available_predictors = list(range(self.num_variates))
 
         # if data is binary
@@ -696,27 +696,26 @@
 def jitter_duplicated(array: npt.NDArray[np.float_], std: float) -> npt.NDArray[np.float_]:
     """
     Jitter duplicated values.
     """
     if are_whole_number(array):
         seen = []
         for idx, num in enumerate(array):
-            if num in seen:
+            if num in seen and not np.isnan(num):
                 array[idx] = num + np.random.normal(0, std / 12)
             else:
                 seen.append(num)
 
     return array
 
 
 @njit
 def are_whole_number(array: npt.NDArray[np.float_]) -> np.bool_:
     """Check if all values in array are whole numbers"""
-    new_array = np.mod(array, 1)
-    return np.all(new_array == 0)
+    return np.all(np.mod(array[~np.isnan(array)], 1) == 0)
 
 
 def logp(point, out_vars, vars, shared):  # pylint: disable=redefined-builtin
     """Compile PyTensor function of the model and the input and output variables.
 
     Parameters
     ----------
```

### Comparing `pymc_bart-0.5.6/pymc_bart/split_rules.py` & `pymc_bart-0.5.7/pymc_bart/split_rules.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/pymc_bart/tree.py` & `pymc_bart-0.5.7/pymc_bart/tree.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/pymc_bart/utils.py` & `pymc_bart-0.5.7/pymc_bart/utils.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/pymc_bart.egg-info/PKG-INFO` & `pymc_bart-0.5.7/pymc_bart.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc_bart
-Version: 0.5.6
+Version: 0.5.7
 Summary: Bayesian Additive Regression Trees for Probabilistic programming with PyMC
 Home-page: http://github.com/pymc-devs/pymc-bart
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `pymc_bart-0.5.6/pymc_bart.egg-info/SOURCES.txt` & `pymc_bart-0.5.7/pymc_bart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/setup.py` & `pymc_bart-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/tests/__init__.py` & `pymc_bart-0.5.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/tests/test_bart.py` & `pymc_bart-0.5.7/tests/test_bart.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/tests/test_pgbart.py` & `pymc_bart-0.5.7/tests/test_pgbart.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/tests/test_split_rules.py` & `pymc_bart-0.5.7/tests/test_split_rules.py`

 * *Files identical despite different names*

### Comparing `pymc_bart-0.5.6/tests/test_tree.py` & `pymc_bart-0.5.7/tests/test_tree.py`

 * *Files identical despite different names*

