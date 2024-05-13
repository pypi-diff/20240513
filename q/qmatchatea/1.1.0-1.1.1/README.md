# Comparing `tmp/qmatchatea-1.1.0.tar.gz` & `tmp/qmatchatea-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qmatchatea-1.1.0.tar", last modified: Thu May  9 14:54:47 2024, max compression
+gzip compressed data, was "qmatchatea-1.1.1.tar", last modified: Mon May 13 08:37:31 2024, max compression
```

## Comparing `qmatchatea-1.1.0.tar` & `qmatchatea-1.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.718386 qmatchatea-1.1.0/
--rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/LICENSE
--rw-r--r--   0 quantum    (128) quantum    (128)      891 2024-01-16 18:26:28.000000 qmatchatea-1.1.0/NOTICE
--rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)     2549 2024-01-16 18:26:28.000000 qmatchatea-1.1.0/README.md
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/
--rw-r--r--   0 quantum    (128) quantum    (128)     1084 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/__init__.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/circuit/
--rw-r--r--   0 quantum    (128) quantum    (128)      640 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/qmatchatea/circuit/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)    47446 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/circuit.py
--rw-r--r--   0 quantum    (128) quantum    (128)    13179 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/observables.py
--rw-r--r--   0 quantum    (128) quantum    (128)    19048 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/circuit/operations.py
--rw-r--r--   0 quantum    (128) quantum    (128)    16545 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/interface.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7469 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/par_simulations.py
--rw-r--r--   0 quantum    (128) quantum    (128)    20020 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/preprocessing.py
--rw-r--r--   0 quantum    (128) quantum    (128)    33472 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/py_emulator.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7951 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/tensor_compiler.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea/utils/
--rw-r--r--   0 quantum    (128) quantum    (128)      645 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/__init__.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8166 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/mpi_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)     7085 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/qk_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)     6496 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/sf_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)    15538 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/simulation_results.py
--rw-r--r--   0 quantum    (128) quantum    (128)     8653 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/tn_utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)    30231 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/utils/utils.py
--rw-r--r--   0 quantum    (128) quantum    (128)      500 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/qmatchatea/version.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/qmatchatea.egg-info/
--rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/PKG-INFO
--rw-r--r--   0 quantum    (128) quantum    (128)      930 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/SOURCES.txt
--rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/dependency_links.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       92 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/requires.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-09 14:54:47.000000 qmatchatea-1.1.0/qmatchatea.egg-info/top_level.txt
--rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-09 14:54:47.718386 qmatchatea-1.1.0/setup.cfg
--rw-r--r--   0 quantum    (128) quantum    (128)     2485 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/setup.py
-drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-09 14:54:47.714386 qmatchatea-1.1.0/tests/
--rw-r--r--   0 quantum    (128) quantum    (128)     7191 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_basic_circuits.py
--rw-r--r--   0 quantum    (128) quantum    (128)    11887 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_examples.py
--rw-r--r--   0 quantum    (128) quantum    (128)     1379 2022-12-06 17:46:42.000000 qmatchatea-1.1.0/tests/tests_formatting.py
--rw-r--r--   0 quantum    (128) quantum    (128)     9540 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_linter.py
--rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_mpi4py.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10753 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_observables.py
--rw-r--r--   0 quantum    (128) quantum    (128)    10441 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_qcircuit.py
--rw-r--r--   0 quantum    (128) quantum    (128)     2978 2024-05-09 14:52:16.000000 qmatchatea-1.1.0/tests/tests_tensor_compiler.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/
+-rw-r--r--   0 quantum    (128) quantum    (128)    10764 2022-12-06 17:46:42.000000 qmatchatea-1.1.1/LICENSE
+-rw-r--r--   0 quantum    (128) quantum    (128)      891 2024-01-16 18:26:28.000000 qmatchatea-1.1.1/NOTICE
+-rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)     2549 2024-01-16 18:26:28.000000 qmatchatea-1.1.1/README.md
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/qmatchatea/
+-rw-r--r--   0 quantum    (128) quantum    (128)     1084 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/__init__.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/qmatchatea/circuit/
+-rw-r--r--   0 quantum    (128) quantum    (128)      640 2022-12-06 17:46:42.000000 qmatchatea-1.1.1/qmatchatea/circuit/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    47446 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/circuit/circuit.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    13179 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/circuit/observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    19048 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/circuit/operations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    16545 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/interface.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7469 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/par_simulations.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    20020 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/preprocessing.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    33472 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/py_emulator.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7951 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/tensor_compiler.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/qmatchatea/utils/
+-rw-r--r--   0 quantum    (128) quantum    (128)      645 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/__init__.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8166 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/mpi_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     7085 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/qk_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     6496 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/sf_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    15538 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/simulation_results.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     8653 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/tn_utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    30231 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/qmatchatea/utils/utils.py
+-rw-r--r--   0 quantum    (128) quantum    (128)      500 2024-05-13 08:34:47.000000 qmatchatea-1.1.1/qmatchatea/version.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/qmatchatea.egg-info/
+-rw-r--r--   0 quantum    (128) quantum    (128)     3238 2024-05-13 08:37:31.000000 qmatchatea-1.1.1/qmatchatea.egg-info/PKG-INFO
+-rw-r--r--   0 quantum    (128) quantum    (128)      930 2024-05-13 08:37:31.000000 qmatchatea-1.1.1/qmatchatea.egg-info/SOURCES.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)        1 2024-05-13 08:37:31.000000 qmatchatea-1.1.1/qmatchatea.egg-info/dependency_links.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       92 2024-05-13 08:37:31.000000 qmatchatea-1.1.1/qmatchatea.egg-info/requires.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       11 2024-05-13 08:37:31.000000 qmatchatea-1.1.1/qmatchatea.egg-info/top_level.txt
+-rw-r--r--   0 quantum    (128) quantum    (128)       38 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/setup.cfg
+-rw-r--r--   0 quantum    (128) quantum    (128)     2485 2024-05-13 08:34:47.000000 qmatchatea-1.1.1/setup.py
+drwxr-xr-x   0 quantum    (128) quantum    (128)        0 2024-05-13 08:37:31.419597 qmatchatea-1.1.1/tests/
+-rw-r--r--   0 quantum    (128) quantum    (128)     7191 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_basic_circuits.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    11887 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_examples.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     1379 2022-12-06 17:46:42.000000 qmatchatea-1.1.1/tests/tests_formatting.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     9540 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_linter.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     3297 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_mpi4py.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10753 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_observables.py
+-rw-r--r--   0 quantum    (128) quantum    (128)    10441 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_qcircuit.py
+-rw-r--r--   0 quantum    (128) quantum    (128)     2978 2024-05-09 14:55:01.000000 qmatchatea-1.1.1/tests/tests_tensor_compiler.py
```

### Comparing `qmatchatea-1.1.0/LICENSE` & `qmatchatea-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/NOTICE` & `qmatchatea-1.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/PKG-INFO` & `qmatchatea-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qmatchatea
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quantum matcha TEA python library for tensor network emulation of quantum circuits.
 Home-page: https://baltig.infn.it/quantum_matcha_tea/py_api_quantum_matcha_tea
 Author: Marco Ballarin
 Author-email: marco97.ballarin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: matplotlib>=3.1.3
-Requires-Dist: qtealeaves>=1.1.4
+Requires-Dist: qtealeaves>=1.1.6
 Requires-Dist: qiskit==0.38.0
 Requires-Dist: mpi4py
 Requires-Dist: joblib
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
```

### Comparing `qmatchatea-1.1.0/README.md` & `qmatchatea-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/__init__.py` & `qmatchatea-1.1.1/qmatchatea/__init__.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/circuit/__init__.py` & `qmatchatea-1.1.1/qmatchatea/circuit/__init__.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/circuit/circuit.py` & `qmatchatea-1.1.1/qmatchatea/circuit/circuit.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/circuit/observables.py` & `qmatchatea-1.1.1/qmatchatea/circuit/observables.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/circuit/operations.py` & `qmatchatea-1.1.1/qmatchatea/circuit/operations.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/interface.py` & `qmatchatea-1.1.1/qmatchatea/interface.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/par_simulations.py` & `qmatchatea-1.1.1/qmatchatea/par_simulations.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/preprocessing.py` & `qmatchatea-1.1.1/qmatchatea/preprocessing.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/py_emulator.py` & `qmatchatea-1.1.1/qmatchatea/py_emulator.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/tensor_compiler.py` & `qmatchatea-1.1.1/qmatchatea/tensor_compiler.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/__init__.py` & `qmatchatea-1.1.1/qmatchatea/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/mpi_utils.py` & `qmatchatea-1.1.1/qmatchatea/utils/mpi_utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/qk_utils.py` & `qmatchatea-1.1.1/qmatchatea/utils/qk_utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/sf_utils.py` & `qmatchatea-1.1.1/qmatchatea/utils/sf_utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/simulation_results.py` & `qmatchatea-1.1.1/qmatchatea/utils/simulation_results.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/tn_utils.py` & `qmatchatea-1.1.1/qmatchatea/utils/tn_utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea/utils/utils.py` & `qmatchatea-1.1.1/qmatchatea/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/qmatchatea.egg-info/PKG-INFO` & `qmatchatea-1.1.1/qmatchatea.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qmatchatea
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quantum matcha TEA python library for tensor network emulation of quantum circuits.
 Home-page: https://baltig.infn.it/quantum_matcha_tea/py_api_quantum_matcha_tea
 Author: Marco Ballarin
 Author-email: marco97.ballarin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: numpy>=1.18.1
 Requires-Dist: scipy>=1.4.1
 Requires-Dist: matplotlib>=3.1.3
-Requires-Dist: qtealeaves>=1.1.4
+Requires-Dist: qtealeaves>=1.1.6
 Requires-Dist: qiskit==0.38.0
 Requires-Dist: mpi4py
 Requires-Dist: joblib
 
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 ![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)
```

### Comparing `qmatchatea-1.1.0/qmatchatea.egg-info/SOURCES.txt` & `qmatchatea-1.1.1/qmatchatea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/setup.py` & `qmatchatea-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 else:
     install_requires = []
 
 install_requires = [
     "numpy>=1.18.1",
     "scipy>=1.4.1",
     "matplotlib>=3.1.3",
-    "qtealeaves>=1.1.4",
+    "qtealeaves>=1.1.6",
     "qiskit==0.38.0",
     "mpi4py",
     "joblib",
 ]
 
 # Get the readme file
 if os.path.isfile("README.md"):
```

### Comparing `qmatchatea-1.1.0/tests/tests_basic_circuits.py` & `qmatchatea-1.1.1/tests/tests_basic_circuits.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_examples.py` & `qmatchatea-1.1.1/tests/tests_examples.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_formatting.py` & `qmatchatea-1.1.1/tests/tests_formatting.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_linter.py` & `qmatchatea-1.1.1/tests/tests_linter.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_mpi4py.py` & `qmatchatea-1.1.1/tests/tests_mpi4py.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_observables.py` & `qmatchatea-1.1.1/tests/tests_observables.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_qcircuit.py` & `qmatchatea-1.1.1/tests/tests_qcircuit.py`

 * *Files identical despite different names*

### Comparing `qmatchatea-1.1.0/tests/tests_tensor_compiler.py` & `qmatchatea-1.1.1/tests/tests_tensor_compiler.py`

 * *Files identical despite different names*

