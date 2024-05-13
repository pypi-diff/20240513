# Comparing `tmp/nz_seqtech-0.2.7.tar.gz` & `tmp/nz_seqtech-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nz_seqtech-0.2.7.tar", last modified: Fri Apr 19 09:02:14 2024, max compression
+gzip compressed data, was "nz_seqtech-0.2.8.tar", last modified: Mon May 13 16:00:40 2024, max compression
```

## Comparing `nz_seqtech-0.2.7.tar` & `nz_seqtech-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.374693 nz_seqtech-0.2.7/nz_seqtech/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/classical_ml_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/classical_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    15119 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/quantum_dna_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/nz_seqtech/quantum_ml_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/nz_seqtech.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 09:02:14.000000 nz_seqtech-0.2.7/nz_seqtech.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 09:02:14.378693 nz_seqtech-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 09:02:07.000000 nz_seqtech-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:00:40.387358 nz_seqtech-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-13 16:00:40.387358 nz_seqtech-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:00:40.387358 nz_seqtech-0.2.8/nz_seqtech/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/nz_seqtech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20097 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/nz_seqtech/classical_ml_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/nz_seqtech/classical_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15119 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/nz_seqtech/quantum_dna_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/nz_seqtech/quantum_ml_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:00:40.387358 nz_seqtech-0.2.8/nz_seqtech.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-13 16:00:40.000000 nz_seqtech-0.2.8/nz_seqtech.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-13 16:00:40.000000 nz_seqtech-0.2.8/nz_seqtech.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:00:40.000000 nz_seqtech-0.2.8/nz_seqtech.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-13 16:00:40.000000 nz_seqtech-0.2.8/nz_seqtech.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 16:00:40.000000 nz_seqtech-0.2.8/nz_seqtech.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:00:40.387358 nz_seqtech-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-13 16:00:35.000000 nz_seqtech-0.2.8/setup.py
```

### Comparing `nz_seqtech-0.2.7/LICENSE` & `nz_seqtech-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/PKG-INFO` & `nz_seqtech-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nz_seqtech
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for DNA sequence encoding in quantum machine learning
 Home-page: https://nz-seqtech.com/
 Author: Nouhaila Innan and Muhammad Al-Zafar Khan
 Author-email: nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com
 License: Apache
 Project-URL: Documentation, https://nz-seqtech.readthedocs.io/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: qiskit
+Requires-Dist: qiskit==0.24.1
 Requires-Dist: matplotlib
 Requires-Dist: qiskit-algorithms
 Requires-Dist: qiskit-machine-learning==0.6.1
 Requires-Dist: qiskit-aer
 
 
 <img align="right" src="https://github.com/Innanov/logos/blob/main/logo.png?raw=true" width="25%">
```

### Comparing `nz_seqtech-0.2.7/README.md` & `nz_seqtech-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech/__init__.py` & `nz_seqtech-0.2.8/nz_seqtech/__init__.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech/classical_ml_models.py` & `nz_seqtech-0.2.8/nz_seqtech/classical_ml_models.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech/classical_operations.py` & `nz_seqtech-0.2.8/nz_seqtech/classical_operations.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech/quantum_dna_encoding.py` & `nz_seqtech-0.2.8/nz_seqtech/quantum_dna_encoding.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech/quantum_ml_models.py` & `nz_seqtech-0.2.8/nz_seqtech/quantum_ml_models.py`

 * *Files identical despite different names*

### Comparing `nz_seqtech-0.2.7/nz_seqtech.egg-info/PKG-INFO` & `nz_seqtech-0.2.8/nz_seqtech.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nz_seqtech
-Version: 0.2.7
+Version: 0.2.8
 Summary: A library for DNA sequence encoding in quantum machine learning
 Home-page: https://nz-seqtech.com/
 Author: Nouhaila Innan and Muhammad Al-Zafar Khan
 Author-email: nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com
 License: Apache
 Project-URL: Documentation, https://nz-seqtech.readthedocs.io/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: wheel
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
-Requires-Dist: qiskit
+Requires-Dist: qiskit==0.24.1
 Requires-Dist: matplotlib
 Requires-Dist: qiskit-algorithms
 Requires-Dist: qiskit-machine-learning==0.6.1
 Requires-Dist: qiskit-aer
 
 
 <img align="right" src="https://github.com/Innanov/logos/blob/main/logo.png?raw=true" width="25%">
```

### Comparing `nz_seqtech-0.2.7/setup.py` & `nz_seqtech-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 #with open("README.md", 'r', encoding='utf-8') as f:
     #long_description = f.read()
 with open("README.md") as readme:
     long_description = readme.read()    
     
 setup(
     name='nz_seqtech',
-    version='0.2.7',
+    version='0.2.8',
     license='Apache',
     description='A library for DNA sequence encoding in quantum machine learning',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url ='https://nz-seqtech.com/',
     author='Nouhaila Innan and Muhammad Al-Zafar Khan',
     author_email='nouhaila.innan@zaiku.com, muhammad.khan@zaikugroup.com',
     packages=find_packages(),
     install_requires=[
     'wheel',    
     'numpy',
     'pandas',
     'scikit-learn',
-    'qiskit',
+    'qiskit==0.24.1',
     'matplotlib',
     'qiskit-algorithms',
     'qiskit-machine-learning==0.6.1',
     'qiskit-aer' 
     ],
     project_urls={
         'Documentation': 'https://nz-seqtech.readthedocs.io/',
```

