# Comparing `tmp/csle_defender-0.5.2.tar.gz` & `tmp/csle_defender-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_defender-0.5.2.tar", last modified: Tue Apr 30 10:49:41 2024, max compression
+gzip compressed data, was "csle_defender-0.5.3.tar", last modified: Mon May 13 17:19:47 2024, max compression
```

## Comparing `csle_defender-0.5.2.tar` & `csle_defender-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.774665 csle_defender-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      644 2024-04-30 10:49:41.774665 csle_defender-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3801 2024-01-29 11:24:00.000000 csle_defender-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-08-08 14:54:06.000000 csle_defender-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1729 2024-04-30 10:49:41.774665 csle_defender-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_defender-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.770665 csle_defender-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.774665 csle_defender-0.5.2/src/csle_defender/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_defender-0.5.2/src/csle_defender/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_defender-0.5.2/src/csle_defender/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1197 2023-03-28 14:03:22.000000 csle_defender-0.5.2/src/csle_defender/defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.774665 csle_defender-0.5.2/src/csle_defender/emulation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_defender-0.5.2/src/csle_defender/emulation/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1291 2024-01-29 11:24:00.000000 csle_defender-0.5.2/src/csle_defender/emulation/defender_stopping_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2568 2024-01-29 11:24:00.000000 csle_defender-0.5.2/src/csle_defender/emulation/emulated_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.774665 csle_defender-0.5.2/src/csle_defender.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      644 2024-04-30 10:49:41.000000 csle_defender-0.5.2/src/csle_defender.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      572 2024-04-30 10:49:41.000000 csle_defender-0.5.2/src/csle_defender.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:49:41.000000 csle_defender-0.5.2/src/csle_defender.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:05.000000 csle_defender-0.5.2/src/csle_defender.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      475 2024-04-30 10:49:41.000000 csle_defender-0.5.2/src/csle_defender.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       14 2024-04-30 10:49:41.000000 csle_defender-0.5.2/src/csle_defender.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:41.774665 csle_defender-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      774 2024-01-29 11:24:00.000000 csle_defender-0.5.2/tests/test_defender_stopping_middleware.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.262540 csle_defender-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      644 2024-05-13 17:19:47.262540 csle_defender-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3801 2024-01-29 11:24:00.000000 csle_defender-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-08-08 14:54:06.000000 csle_defender-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1729 2024-05-13 17:19:47.262540 csle_defender-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_defender-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.258540 csle_defender-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.258540 csle_defender-0.5.3/src/csle_defender/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_defender-0.5.3/src/csle_defender/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_defender-0.5.3/src/csle_defender/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1197 2023-03-28 14:03:22.000000 csle_defender-0.5.3/src/csle_defender/defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.262540 csle_defender-0.5.3/src/csle_defender/emulation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_defender-0.5.3/src/csle_defender/emulation/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1291 2024-01-29 11:24:00.000000 csle_defender-0.5.3/src/csle_defender/emulation/defender_stopping_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2568 2024-01-29 11:24:00.000000 csle_defender-0.5.3/src/csle_defender/emulation/emulated_defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.262540 csle_defender-0.5.3/src/csle_defender.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      644 2024-05-13 17:19:47.000000 csle_defender-0.5.3/src/csle_defender.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      572 2024-05-13 17:19:47.000000 csle_defender-0.5.3/src/csle_defender.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:47.000000 csle_defender-0.5.3/src/csle_defender.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:36:05.000000 csle_defender-0.5.3/src/csle_defender.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      475 2024-05-13 17:19:47.000000 csle_defender-0.5.3/src/csle_defender.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       14 2024-05-13 17:19:47.000000 csle_defender-0.5.3/src/csle_defender.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:47.262540 csle_defender-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      774 2024-01-29 11:24:00.000000 csle_defender-0.5.3/tests/test_defender_stopping_middleware.py
```

### Comparing `csle_defender-0.5.2/PKG-INFO` & `csle_defender-0.5.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_defender
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.5.2/README.md` & `csle_defender-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/pyproject.toml` & `csle_defender-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/setup.cfg` & `csle_defender-0.5.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.5.2
-	csle-common>=0.5.2
+	csle-base>=0.5.3
+	csle-common>=0.5.3
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_defender-0.5.2/src/csle_defender/defender.py` & `csle_defender-0.5.3/src/csle_defender/defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/src/csle_defender/emulation/defender_stopping_middleware.py` & `csle_defender-0.5.3/src/csle_defender/emulation/defender_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/src/csle_defender/emulation/emulated_defender.py` & `csle_defender-0.5.3/src/csle_defender/emulation/emulated_defender.py`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/src/csle_defender.egg-info/PKG-INFO` & `csle_defender-0.5.3/src/csle_defender.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-defender
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for emulated defenses in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_defender-0.5.2/src/csle_defender.egg-info/SOURCES.txt` & `csle_defender-0.5.3/src/csle_defender.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_defender-0.5.2/tests/test_defender_stopping_middleware.py` & `csle_defender-0.5.3/tests/test_defender_stopping_middleware.py`

 * *Files identical despite different names*

