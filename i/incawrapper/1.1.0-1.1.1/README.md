# Comparing `tmp/incawrapper-1.1.0.tar.gz` & `tmp/incawrapper-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incawrapper-1.1.0.tar", last modified: Thu Feb  8 10:33:48 2024, max compression
+gzip compressed data, was "incawrapper-1.1.1.tar", last modified: Mon May 13 12:40:45 2024, max compression
```

## Comparing `incawrapper-1.1.0.tar` & `incawrapper-1.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.555705 incawrapper-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-08 10:33:34.000000 incawrapper-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-02-08 10:33:48.555705 incawrapper-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-02-08 10:33:34.000000 incawrapper-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.547706 incawrapper-1.1.0/incawrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.551705 incawrapper-1.1.0/incawrapper/core/
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAFitData.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAMonteCarloResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAScript.py
--rw-r--r--   0 runner    (1001) docker     (127)    33880 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCAScript_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/INCASimulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/dataschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/load_matlab_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/core/run_inca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.551705 incawrapper-1.1.0/incawrapper/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/utils/chemical_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/utils/merge_reversible_reactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/utils/schema_overview.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.551705 incawrapper-1.1.0/incawrapper/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/visualization/diagnositics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-02-08 10:33:34.000000 incawrapper-1.1.0/incawrapper/visualization/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.555705 incawrapper-1.1.0/incawrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-02-08 10:33:48.000000 incawrapper-1.1.0/incawrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-08 10:33:48.000000 incawrapper-1.1.0/incawrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 10:33:48.000000 incawrapper-1.1.0/incawrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-08 10:33:48.000000 incawrapper-1.1.0/incawrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-08 10:33:48.000000 incawrapper-1.1.0/incawrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-08 10:33:34.000000 incawrapper-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-08 10:33:48.555705 incawrapper-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 10:33:34.000000 incawrapper-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 10:33:48.551705 incawrapper-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAFitData.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAMonteCarloResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAResults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAScript.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_INCAScript_writing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_dataschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_linting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_utils_chemical_formula.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-08 10:33:34.000000 incawrapper-1.1.0/tests/test_utils_merge_reversible_reactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.709079 incawrapper-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 12:40:40.000000 incawrapper-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-13 12:40:45.709079 incawrapper-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-13 12:40:40.000000 incawrapper-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.701079 incawrapper-1.1.1/incawrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.705079 incawrapper-1.1.1/incawrapper/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAFitData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAMonteCarloResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4037 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33880 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCAScript_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/INCASimulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/dataschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/load_matlab_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/core/run_inca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.705079 incawrapper-1.1.1/incawrapper/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/utils/chemical_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/utils/merge_reversible_reactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/utils/schema_overview.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.705079 incawrapper-1.1.1/incawrapper/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/visualization/diagnositics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-13 12:40:40.000000 incawrapper-1.1.1/incawrapper/visualization/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.709079 incawrapper-1.1.1/incawrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-13 12:40:45.000000 incawrapper-1.1.1/incawrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-13 12:40:45.000000 incawrapper-1.1.1/incawrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:40:45.000000 incawrapper-1.1.1/incawrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 12:40:45.000000 incawrapper-1.1.1/incawrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:40:45.000000 incawrapper-1.1.1/incawrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 12:40:40.000000 incawrapper-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-13 12:40:45.713079 incawrapper-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:40:40.000000 incawrapper-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:40:45.709079 incawrapper-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAFitData.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAMonteCarloResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAScript.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_INCAScript_writing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_dataschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_linting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_utils_chemical_formula.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-13 12:40:40.000000 incawrapper-1.1.1/tests/test_utils_merge_reversible_reactions.py
```

### Comparing `incawrapper-1.1.0/LICENSE` & `incawrapper-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/PKG-INFO` & `incawrapper-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incawrapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: General Repository for Omics Data Handling tools
 Home-page: 
 Author: AutoFlow, Matthias Mattonovich and Viktor Hesselberg-Thomsen
 Author-email: vikhes@dtu.dk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `incawrapper-1.1.0/README.md` & `incawrapper-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAFitData.py` & `incawrapper-1.1.1/incawrapper/core/INCAFitData.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import numpy as np
 from incawrapper.core import load_matlab_file
 from dataclasses import dataclass
 import pathlib
 from typing import Dict, Iterable, Callable
 import scipy.stats
 
+
 @dataclass
 class INCAFitData:
     """
     This class parses the output from INCA and stores the data in a dataclass. On init the class
     loads the matlab file and parses the data into several pandas dataframe, which can be accessed
     via the class attributes. This class is not intended to be used directly, but rather through
     the INCAResults class.
@@ -44,50 +45,50 @@
     def raw(self) -> Dict:
         """Gets the raw parsed matlab structure that contains the fitting results.
 
         Returns
         -------
         Dict
             This attribute contains the raw fitdata from the INCA output."""
-        return load_matlab_file.load_matlab_file(self.inca_matlab_file)['f']
+        return load_matlab_file.load_matlab_file(self.inca_matlab_file)["f"]
 
     @property
     def alpha(self) -> float:
         """Gets the alpha value used for to obtain the confidence intervals.
 
         Returns
         -------
         float
             This attribute contains the alpha value used for to obtain the confidence intervals.
         """
         return self.raw["alf"]
-    
+
     @property
     def chi2(self) -> float:
         """Gets the chi2 value of the fit.
 
         Returns
         -------
         float
             This attribute contains the chi2 value of the fit.
         """
         return self.raw["chi2"]
-    
+
     @property
     def degrees_of_freedom(self) -> int:
         """Gets the degrees of freedom of the fit.
 
         Returns
         -------
         int
             This attribute contains the degrees of freedom of the fit.
         """
 
         return self.raw["dof"]
-    
+
     @property
     def expected_chi2(self) -> Iterable[float]:
         """Gets the expected chi2 interval of the fit. The first value is the lower bound and the second
         value is the upper bound.
 
         Returns
         -------
@@ -96,17 +97,17 @@
         """
         return self.raw["Echi2"]
 
     @property
     def fitted_parameters(self) -> pd.DataFrame:
         """
         Gets the fitted parameters and their associated standard error, lower bound, upper bound and other
-        information. This information is equivalent to the table shown in the main window of the Flux 
+        information. This information is equivalent to the table shown in the main window of the Flux
         Estimation tab in the INCA GUI.
-        
+
         Returns
         -------
         pd.DataFrame
             This attribute contains the fitted parameters from the INCA output.
             The columns of the dataframe are:
             * type: type of the parameter (Flux, Pool, or MS)
             * id: id of the parameter (flux, pool, or MS)
@@ -114,41 +115,46 @@
             * val: fitted value of the parameter
             * std: estimated standard deviation of the fitted value
             * lb: lower bound of the fitted value (Obtained from continuation or monte carlo simulation)
             * ub: upper bound of the fitted value (Obtained from continuation or monte carlo simulation)
             * unit: unit of the parameter
             * free: boolean indicating if the parameter was fitted or not
             * cor: correlation vector for this parameter to the other fitted parameters. The order matches
-            the order of the other parameters in the dataframe 
+            the order of the other parameters in the dataframe
             * cov: covariance vector similar to the cor column
-            * vals: value of the parameter of each restart of the estimation algorithm (length of vals is 
+            * vals: value of the parameter of each restart of the estimation algorithm (length of vals is
             equal to the number of fit_starts option)
             * base: don't know what this is
         """
-        df = pd.DataFrame.from_records(self.raw["par"]).reindex(
-            columns=[
-                "type",
-                "id",
-                "eqn",
-                "val",
-                "std",
-                "lb",
-                "ub",
-                "unit",
-                "free",
-                "alf",
-                "chi2s",
-                "cont",
-                "cor",
-                "cov",
-                "vals",
-                "base",
-            ]
+        df = (
+            pd.DataFrame.from_records(self.raw["par"])
+            .reindex(
+                columns=[
+                    "type",
+                    "id",
+                    "eqn",
+                    "val",
+                    "std",
+                    "lb",
+                    "ub",
+                    "unit",
+                    "free",
+                    "alf",
+                    "chi2s",
+                    "cont",
+                    "cor",
+                    "cov",
+                    "vals",
+                    "base",
+                ]
+            )
+            .apply(lambda x: pd.to_numeric(x, errors="ignore"))
         )
         return df
+
     @property
     def measurements_and_fit_overview(self):
         """
         Gets an overview of the measurements and their overall fit,
         i.e. the conbined values accross all data points in the measurement. For
         example if the same flux or fragment is measured multiple times in the same
         experiment. Further for fragements this combines all the all mass isopote
@@ -163,15 +169,15 @@
     def measurements_and_fit_detailed(self) -> pd.DataFrame:
         """
         Gets a dataframe all measuremets, their associatted fitted value and weighted residuals.
 
         Returns
         -------
         pd.DataFame
-            This attribute contains an overview of the measurements and their overall fit. The columns 
+            This attribute contains an overview of the measurements and their overall fit. The columns
             of the dataframe are:
             * expt: experiment id
             * id: measurement id
             * type: measurement type (Flux, Fragment, or pool size)
             * time: time of measurement
             * data: measured data
             * std: standard deviation of the measurement
@@ -183,19 +189,17 @@
         detailed_info = np.array([])
         for measurement in self.raw["mnt"]:
             detailed_info = np.append(detailed_info, measurement["res"])
         df = (
             pd.DataFrame.from_records(detailed_info)
             # drop the columns which are not needed
             # esens and msens are the sensitivity diagnostics, which are handled seperatly
-            .drop(
-                columns=["esens", "msens", 'cont']
-            ).rename(
-                columns={"val": "weighted residual"}
-            ).reindex(
+            .drop(columns=["esens", "msens", "cont"])
+            .rename(columns={"val": "weighted residual"})
+            .reindex(
                 columns=[
                     "type",
                     "expt",
                     "id",
                     "peak",
                     "time",
                     "data",
@@ -205,38 +209,41 @@
                     "cont",
                     "base",
                 ]
             )
         )
         return df
 
-
-    def get_goodness_of_fit(self)->None:
+    def get_goodness_of_fit(self) -> None:
         """
         Return the goodness of fit for the model. This is the chi2 value divided by the degrees of freedom
         """
         fit_accepted = self.expected_chi2[0] <= self.chi2 <= self.expected_chi2[1]
 
         print(
-        f'''Fit accepted: {fit_accepted}
+            f"""Fit accepted: {fit_accepted}
 Confidence level: {self.alpha}
 Chi-square value (SSR): {self.chi2}
-Expected chi-square range: {self.expected_chi2}'''
+Expected chi-square range: {self.expected_chi2}"""
         )
-    
-    def test_normality_of_residuals(self, test_function: Callable = scipy.stats.shapiro, alpha: float = None)->None:
+
+    def test_normality_of_residuals(
+        self, test_function: Callable = scipy.stats.shapiro, alpha: float = None
+    ) -> None:
         """
         Test the normality of the residuals of the model. This is done by default using the Shapiro-Wilk test.
         The user can specify a different test using the test_function argument. The test function should take
         an array of residuals as input and return a test statistic and a p-value. The p-value is compared to the
         alpha value to determine if the residuals are normally distributed. The default alpha is the overall alpha
         value for the model. This can be changed using the alpha argument.
         """
         if alpha is None:
             alpha = self.alpha
-        
-        residuals = self.measurements_and_fit_detailed['weighted residual']
+
+        residuals = self.measurements_and_fit_detailed["weighted residual"]
         test_statistic, p_value = test_function(residuals)
         # The shapiro test test the null hypothsis that the data is drawn from a normal distribution
-        # Therefore if the p-value is greater than the alpha value the null hypothesis is accepted, i.e. 
+        # Therefore if the p-value is greater than the alpha value the null hypothesis is accepted, i.e.
         # residuals are normally distributed
-        print(f'Residuals are normally distributed: {p_value > alpha} on a {alpha} significance level')
+        print(
+            f"Residuals are normally distributed: {p_value > alpha} on a {alpha} significance level"
+        )
```

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAModel.py` & `incawrapper-1.1.1/incawrapper/core/INCAModel.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAMonteCarloResults.py` & `incawrapper-1.1.1/incawrapper/core/INCAMonteCarloResults.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAResults.py` & `incawrapper-1.1.1/incawrapper/core/INCAResults.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAScript.py` & `incawrapper-1.1.1/incawrapper/core/INCAScript.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCAScript_writing.py` & `incawrapper-1.1.1/incawrapper/core/INCAScript_writing.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/INCASimulation.py` & `incawrapper-1.1.1/incawrapper/core/INCASimulation.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/dataschemas.py` & `incawrapper-1.1.1/incawrapper/core/dataschemas.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/load_matlab_file.py` & `incawrapper-1.1.1/incawrapper/core/load_matlab_file.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/core/run_inca.py` & `incawrapper-1.1.1/incawrapper/core/run_inca.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/utils/__init__.py` & `incawrapper-1.1.1/incawrapper/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/utils/chemical_formula.py` & `incawrapper-1.1.1/incawrapper/utils/chemical_formula.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/utils/merge_reversible_reactions.py` & `incawrapper-1.1.1/incawrapper/utils/merge_reversible_reactions.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/utils/schema_overview.py` & `incawrapper-1.1.1/incawrapper/utils/schema_overview.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/visualization/diagnositics.py` & `incawrapper-1.1.1/incawrapper/visualization/diagnositics.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper/visualization/visualization.py` & `incawrapper-1.1.1/incawrapper/visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/incawrapper.egg-info/PKG-INFO` & `incawrapper-1.1.1/incawrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incawrapper
-Version: 1.1.0
+Version: 1.1.1
 Summary: General Repository for Omics Data Handling tools
 Home-page: 
 Author: AutoFlow, Matthias Mattonovich and Viktor Hesselberg-Thomsen
 Author-email: vikhes@dtu.dk
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `incawrapper-1.1.0/incawrapper.egg-info/SOURCES.txt` & `incawrapper-1.1.1/incawrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/setup.cfg` & `incawrapper-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAFitData.py` & `incawrapper-1.1.1/tests/test_INCAFitData.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAModel.py` & `incawrapper-1.1.1/tests/test_INCAModel.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAMonteCarloResults.py` & `incawrapper-1.1.1/tests/test_INCAMonteCarloResults.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAResults.py` & `incawrapper-1.1.1/tests/test_INCAResults.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAScript.py` & `incawrapper-1.1.1/tests/test_INCAScript.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_INCAScript_writing.py` & `incawrapper-1.1.1/tests/test_INCAScript_writing.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_dataschemas.py` & `incawrapper-1.1.1/tests/test_dataschemas.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_diagnostics.py` & `incawrapper-1.1.1/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_utils_chemical_formula.py` & `incawrapper-1.1.1/tests/test_utils_chemical_formula.py`

 * *Files identical despite different names*

### Comparing `incawrapper-1.1.0/tests/test_utils_merge_reversible_reactions.py` & `incawrapper-1.1.1/tests/test_utils_merge_reversible_reactions.py`

 * *Files identical despite different names*

