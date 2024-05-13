# Comparing `tmp/pyBlindOpt-0.1.3.1.tar.gz` & `tmp/pyblindopt-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyBlindOpt-0.1.3.1.tar", last modified: Thu Mar 21 21:48:05 2024, max compression
+gzip compressed data, was "pyblindopt-0.1.3.2.tar", last modified: Mon May 13 17:32:35 2024, max compression
```

## Comparing `pyBlindOpt-0.1.3.1.tar` & `pyblindopt-0.1.3.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:48:05.619006 pyBlindOpt-0.1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-21 21:48:05.619006 pyBlindOpt-0.1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-21 21:48:05.619006 pyBlindOpt-0.1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:48:05.615006 pyBlindOpt-0.1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:48:05.615006 pyBlindOpt-0.1.3.1/src/pyBlindOpt/
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/de.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/gwo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/hc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/pso.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/sa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:48:05.619006 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-21 21:48:05.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-21 21:48:05.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 21:48:05.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-21 21:48:05.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 21:48:05.000000 pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:48:05.619006 pyBlindOpt-0.1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_de.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_ga.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_gwo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_hc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_pso.py
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_sa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-21 21:47:57.000000 pyBlindOpt-0.1.3.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:32:35.120492 pyblindopt-0.1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/src/pyBlindOpt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10222 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/egwo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/gwo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/hc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/pso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/sa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/src/pyBlindOpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-05-13 17:32:35.000000 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-13 17:32:35.000000 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:32:35.000000 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 17:32:35.000000 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 17:32:35.000000 pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:32:35.124492 pyblindopt-0.1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_de.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_egwo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_gwo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_hc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_pso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_sa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 17:32:28.000000 pyblindopt-0.1.3.2/test/test_utils.py
```

### Comparing `pyBlindOpt-0.1.3.1/LICENSE` & `pyblindopt-0.1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/PKG-INFO` & `pyblindopt-0.1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyBlindOpt
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: A library that implements several derivation-free optimization algorithms (such as genetic optimization).
 Home-page: https://github.com/mariolpantunes/pyBlindOpt
 Author: Mário Antunes
 Author-email: mario.antunes@ua.pt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
-Requires-Dist: joblib>=1.3.2
-Requires-Dist: tqdm>=4.66.1
+Requires-Dist: numpy>=1.26
+Requires-Dist: joblib>=1.4.2
+Requires-Dist: tqdm>=4.66.4
 
 # pyBlindOpt
 
 A library that implements several derivation-free optimization algorithms (such as genetic optimization).
 Currently, it implements six different algorithms:
 1. Hill climbing is a mathematical optimization technique that belongs to the family of local search. It is an iterative algorithm that starts with an arbitrary solution to a problem and then attempts to find a better solution by making an incremental change to the solution.
 2. Simulated annealing is a probabilistic technique for approximating the global optimum of a given function. Specifically, it is a metaheuristic to approximate global optimization in a large search space for an optimization problem.
```

### Comparing `pyBlindOpt-0.1.3.1/README.md` & `pyblindopt-0.1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/setup.cfg` & `pyblindopt-0.1.3.2/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyBlindOpt
-version = 0.1.3.1
+version = 0.1.3.2
 author = Mário Antunes
 author_email = mario.antunes@ua.pt
 description = A library that implements several derivation-free optimization algorithms (such as genetic optimization).
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/mariolpantunes/pyBlindOpt
 classifiers = 
@@ -14,17 +14,17 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	numpy >= 1.23
-	joblib>=1.3.2
-	tqdm>=4.66.1
+	numpy >= 1.26
+	joblib>=1.4.2
+	tqdm>=4.66.4
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/__init__.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/de.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/de.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/ga.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/ga.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/gwo.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/gwo.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/hc.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/hc.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/init.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/init.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/pso.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/pso.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/sa.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/sa.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt/utils.py` & `pyblindopt-0.1.3.2/src/pyBlindOpt/utils.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/PKG-INFO` & `pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyBlindOpt
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: A library that implements several derivation-free optimization algorithms (such as genetic optimization).
 Home-page: https://github.com/mariolpantunes/pyBlindOpt
 Author: Mário Antunes
 Author-email: mario.antunes@ua.pt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.23
-Requires-Dist: joblib>=1.3.2
-Requires-Dist: tqdm>=4.66.1
+Requires-Dist: numpy>=1.26
+Requires-Dist: joblib>=1.4.2
+Requires-Dist: tqdm>=4.66.4
 
 # pyBlindOpt
 
 A library that implements several derivation-free optimization algorithms (such as genetic optimization).
 Currently, it implements six different algorithms:
 1. Hill climbing is a mathematical optimization technique that belongs to the family of local search. It is an iterative algorithm that starts with an arbitrary solution to a problem and then attempts to find a better solution by making an incremental change to the solution.
 2. Simulated annealing is a probabilistic technique for approximating the global optimum of a given function. Specifically, it is a metaheuristic to approximate global optimization in a large search space for an optimization problem.
```

### Comparing `pyBlindOpt-0.1.3.1/src/pyBlindOpt.egg-info/SOURCES.txt` & `pyblindopt-0.1.3.2/src/pyBlindOpt.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pyBlindOpt/__init__.py
 src/pyBlindOpt/de.py
+src/pyBlindOpt/egwo.py
 src/pyBlindOpt/ga.py
 src/pyBlindOpt/gwo.py
 src/pyBlindOpt/hc.py
 src/pyBlindOpt/init.py
 src/pyBlindOpt/pso.py
 src/pyBlindOpt/sa.py
 src/pyBlindOpt/utils.py
 src/pyBlindOpt.egg-info/PKG-INFO
 src/pyBlindOpt.egg-info/SOURCES.txt
 src/pyBlindOpt.egg-info/dependency_links.txt
 src/pyBlindOpt.egg-info/requires.txt
 src/pyBlindOpt.egg-info/top_level.txt
 test/test_de.py
+test/test_egwo.py
 test/test_ga.py
 test/test_gwo.py
 test/test_hc.py
 test/test_init.py
 test/test_pso.py
 test/test_sa.py
 test/test_utils.py
```

### Comparing `pyBlindOpt-0.1.3.1/test/test_de.py` & `pyblindopt-0.1.3.2/test/test_de.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_ga.py` & `pyblindopt-0.1.3.2/test/test_ga.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_gwo.py` & `pyblindopt-0.1.3.2/test/test_gwo.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # define global variable and callback
 total = 0
 def callback(epoch, obj, pop):
     global total
     total += 1
 
 
-class TestPSO(unittest.TestCase):
+class TestGWO(unittest.TestCase):
     def test_gwo_00(self):
         bounds = np.asarray([(-5.0, 5.0)])
         result, _ = gwo.grey_wolf_optimization(f1, bounds, n_iter=100, verbose=False)
         desired = np.array([0])
         np.testing.assert_allclose(result, desired, atol=1)
     
     def test_gwo_01(self):
```

### Comparing `pyBlindOpt-0.1.3.1/test/test_hc.py` & `pyblindopt-0.1.3.2/test/test_hc.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_init.py` & `pyblindopt-0.1.3.2/test/test_init.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_pso.py` & `pyblindopt-0.1.3.2/test/test_pso.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_sa.py` & `pyblindopt-0.1.3.2/test/test_sa.py`

 * *Files identical despite different names*

### Comparing `pyBlindOpt-0.1.3.1/test/test_utils.py` & `pyblindopt-0.1.3.2/test/test_utils.py`

 * *Files identical despite different names*

