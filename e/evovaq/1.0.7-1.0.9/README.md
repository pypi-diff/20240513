# Comparing `tmp/evovaq-1.0.7.tar.gz` & `tmp/evovaq-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evovaq-1.0.7.tar", last modified: Tue Nov 21 16:34:51 2023, max compression
+gzip compressed data, was "evovaq-1.0.9.tar", last modified: Tue Nov 21 16:57:35 2023, max compression
```

## Comparing `evovaq-1.0.7.tar` & `evovaq-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:34:51.053215 evovaq-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-21 16:34:38.000000 evovaq-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-21 16:34:51.053215 evovaq-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-21 16:34:38.000000 evovaq-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:34:51.049215 evovaq-1.0.7/evovaq/
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/BigBangBigCrunch.py
--rw-r--r--   0 runner    (1001) docker     (127)    12174 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/CHCAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11458 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/DifferentialEvolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    11165 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/GeneticAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5821 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/HillClimbing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/MemeticAlgorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/ParticleSwarmOptimization.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-11-21 16:34:38.000000 evovaq-1.0.7/evovaq/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:34:51.049215 evovaq-1.0.7/evovaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-11-21 16:34:51.000000 evovaq-1.0.7/evovaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-21 16:34:51.000000 evovaq-1.0.7/evovaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 16:34:51.000000 evovaq-1.0.7/evovaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-11-21 16:34:51.000000 evovaq-1.0.7/evovaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-21 16:34:51.000000 evovaq-1.0.7/evovaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-21 16:34:38.000000 evovaq-1.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-21 16:34:51.053215 evovaq-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-11-21 16:34:38.000000 evovaq-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:57:35.216295 evovaq-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-21 16:57:22.000000 evovaq-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-21 16:57:35.216295 evovaq-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-21 16:57:22.000000 evovaq-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:57:35.216295 evovaq-1.0.9/evovaq/
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/BigBangBigCrunch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12174 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/CHCAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/DifferentialEvolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11165 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/GeneticAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/HillClimbing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/MemeticAlgorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/ParticleSwarmOptimization.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4310 2023-11-21 16:57:22.000000 evovaq-1.0.9/evovaq/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 16:57:35.216295 evovaq-1.0.9/evovaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-21 16:57:35.000000 evovaq-1.0.9/evovaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2023-11-21 16:57:35.000000 evovaq-1.0.9/evovaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 16:57:35.000000 evovaq-1.0.9/evovaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-11-21 16:57:35.000000 evovaq-1.0.9/evovaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-21 16:57:35.000000 evovaq-1.0.9/evovaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-21 16:57:22.000000 evovaq-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-21 16:57:35.216295 evovaq-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-11-21 16:57:22.000000 evovaq-1.0.9/setup.py
```

### Comparing `evovaq-1.0.7/LICENSE` & `evovaq-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/PKG-INFO` & `evovaq-1.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: evovaq
-Version: 1.0.7
+Version: 1.0.9
 Summary: EVOlutionary algorithms toolbox for VAriational Quantum circuits
 Home-page: https://github.com/Quasar-UniNA/EVOVAQ
 Author: Angela Chiatto
 Author-email: angela.chiatto@unina.it
 License: MIT
 Keywords: Quantum Computing,Evolutionary Algorithms,Variational Quantum Circuits
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
-Requires-Dist: setuptools==65.5.1
 Requires-Dist: tabulate==0.8.10
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: matplotlib==3.5.1
 Requires-Dist: pandas==1.4.2
 Requires-Dist: openpyxl==3.0.9
 Requires-Dist: scikit-learn==1.1.3
 Requires-Dist: qiskit==0.36.2
```

### Comparing `evovaq-1.0.7/evovaq/BigBangBigCrunch.py` & `evovaq-1.0.9/evovaq/BigBangBigCrunch.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/CHCAlgorithm.py` & `evovaq-1.0.9/evovaq/CHCAlgorithm.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/DifferentialEvolution.py` & `evovaq-1.0.9/evovaq/DifferentialEvolution.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/GeneticAlgorithm.py` & `evovaq-1.0.9/evovaq/GeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/HillClimbing.py` & `evovaq-1.0.9/evovaq/HillClimbing.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/MemeticAlgorithm.py` & `evovaq-1.0.9/evovaq/MemeticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/ParticleSwarmOptimization.py` & `evovaq-1.0.9/evovaq/ParticleSwarmOptimization.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq/problem.py` & `evovaq-1.0.9/evovaq/problem.py`

 * *Files identical despite different names*

### Comparing `evovaq-1.0.7/evovaq.egg-info/PKG-INFO` & `evovaq-1.0.9/evovaq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: evovaq
-Version: 1.0.7
+Version: 1.0.9
 Summary: EVOlutionary algorithms toolbox for VAriational Quantum circuits
 Home-page: https://github.com/Quasar-UniNA/EVOVAQ
 Author: Angela Chiatto
 Author-email: angela.chiatto@unina.it
 License: MIT
 Keywords: Quantum Computing,Evolutionary Algorithms,Variational Quantum Circuits
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy==1.23.5
-Requires-Dist: setuptools==65.5.1
 Requires-Dist: tabulate==0.8.10
 Requires-Dist: tqdm==4.64.1
 Requires-Dist: matplotlib==3.5.1
 Requires-Dist: pandas==1.4.2
 Requires-Dist: openpyxl==3.0.9
 Requires-Dist: scikit-learn==1.1.3
 Requires-Dist: qiskit==0.36.2
```

### Comparing `evovaq-1.0.7/evovaq.egg-info/requires.txt` & `evovaq-1.0.9/evovaq.egg-info/requires.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 numpy==1.23.5
-setuptools==65.5.1
 tabulate==0.8.10
 tqdm==4.64.1
 matplotlib==3.5.1
 pandas==1.4.2
 openpyxl==3.0.9
 scikit-learn==1.1.3
 qiskit==0.36.2
```

### Comparing `evovaq-1.0.7/setup.py` & `evovaq-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,26 +2,25 @@
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='evovaq',
     packages=['evovaq'],
-    version='1.0.7',
+    version='1.0.9',
     description='EVOlutionary algorithms toolbox for VAriational Quantum circuits',
     author='Angela Chiatto',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='angela.chiatto@unina.it',
     license='MIT',
     url='https://github.com/Quasar-UniNA/EVOVAQ',
     keywords=['Quantum Computing', 'Evolutionary Algorithms', 'Variational Quantum Circuits'],
     install_requires=[
         'numpy==1.23.5',
-        'setuptools==65.5.1',
         'tabulate==0.8.10',
         'tqdm==4.64.1',
         'matplotlib==3.5.1',
         'pandas==1.4.2',
         'openpyxl==3.0.9',
         'scikit-learn==1.1.3',
         'qiskit==0.36.2',
```

