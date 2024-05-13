# Comparing `tmp/csle_attack_profiler-0.5.2.tar.gz` & `tmp/csle_attack_profiler-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attack_profiler-0.5.2.tar", last modified: Tue Apr 30 10:51:12 2024, max compression
+gzip compressed data, was "csle_attack_profiler-0.5.3.tar", last modified: Mon May 13 17:21:15 2024, max compression
```

## Comparing `csle_attack_profiler-0.5.2.tar` & `csle_attack_profiler-0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:12.399118 csle_attack_profiler-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      652 2024-04-30 10:51:12.399118 csle_attack_profiler-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3911 2024-04-30 10:35:50.000000 csle_attack_profiler-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      681 2024-04-30 09:37:32.000000 csle_attack_profiler-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1779 2024-04-30 10:51:12.399118 csle_attack_profiler-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-04-30 09:37:32.000000 csle_attack_profiler-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:12.395118 csle_attack_profiler-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:12.395118 csle_attack_profiler-0.5.2/src/csle_attack_profiler/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2024-04-30 09:37:32.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10535 2024-04-30 10:08:07.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler/attack_profiler.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    24128 2024-04-30 09:44:49.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler/hmm_profiling.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:12.399118 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      652 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      572 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      502 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       21 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:12.399118 csle_attack_profiler-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)    44600 2024-04-30 10:47:04.000000 csle_attack_profiler-0.5.2/tests/test_attack_profiler.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2780 2024-04-30 10:47:26.000000 csle_attack_profiler-0.5.2/tests/test_hmm_profiler.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1286 2024-04-30 10:44:25.000000 csle_attack_profiler-0.5.2/tests/test_kullback.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      652 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3933 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      681 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1779 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:15.967079 csle_attack_profiler-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/src/csle_attack_profiler/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10535 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler/attack_profiler.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    24128 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler/hmm_profiling.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      652 2024-05-13 17:21:15.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      572 2024-05-13 17:21:15.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:21:15.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:51:12.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      502 2024-05-13 17:21:15.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       21 2024-05-13 17:21:15.000000 csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:15.971079 csle_attack_profiler-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)    44600 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/tests/test_attack_profiler.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2780 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/tests/test_hmm_profiler.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1286 2024-05-13 17:10:17.000000 csle_attack_profiler-0.5.3/tests/test_kullback.py
```

### Comparing `csle_attack_profiler-0.5.2/PKG-INFO` & `csle_attack_profiler-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attack_profiler
-Version: 0.5.2
+Version: 0.5.3
 Summary: Library with MITRE attack profiler for CSLE
 Author: Bength Pappila
 Author-email: brpa@kth.se
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attack_profiler-0.5.2/README.md` & `csle_attack_profiler-0.5.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ```
 ## API documentation
 
 This section contains instructions for generating API documentation using `sphinx`.
 
 ### Latest Documentation
 
-The latest documentation is available at [https://limmen.dev/csle/docs/csle-base](https://limmen.dev/csle/docs/csle-base)
+The latest documentation is available at [https://limmen.dev/csle/docs/csle-attack-profiler](https://limmen.dev/csle/docs/csle-attack-profiler)
 
 ### Generate API Documentation
 
 First make sure that the `CSLE_HOME` environment variable is set:
 ```bash
 echo $CSLE_HOME
 ```
```

### Comparing `csle_attack_profiler-0.5.2/pyproject.toml` & `csle_attack_profiler-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/setup.cfg` & `csle_attack_profiler-0.5.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 install_requires = 
 	mitreattack-python==2.0.14
-	csle-base==0.5.2
-	csle-common==0.5.2
+	csle-base==0.5.3
+	csle-common==0.5.3
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
 testing = 
 	pytest>=6.0
```

### Comparing `csle_attack_profiler-0.5.2/src/csle_attack_profiler/attack_profiler.py` & `csle_attack_profiler-0.5.3/src/csle_attack_profiler/attack_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/src/csle_attack_profiler/hmm_profiling.py` & `csle_attack_profiler-0.5.3/src/csle_attack_profiler/hmm_profiling.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/PKG-INFO` & `csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attack-profiler
-Version: 0.5.2
+Version: 0.5.3
 Summary: Library with MITRE attack profiler for CSLE
 Author: Bength Pappila
 Author-email: brpa@kth.se
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attack_profiler-0.5.2/src/csle_attack_profiler.egg-info/SOURCES.txt` & `csle_attack_profiler-0.5.3/src/csle_attack_profiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/tests/test_attack_profiler.py` & `csle_attack_profiler-0.5.3/tests/test_attack_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/tests/test_hmm_profiler.py` & `csle_attack_profiler-0.5.3/tests/test_hmm_profiler.py`

 * *Files identical despite different names*

### Comparing `csle_attack_profiler-0.5.2/tests/test_kullback.py` & `csle_attack_profiler-0.5.3/tests/test_kullback.py`

 * *Files identical despite different names*

