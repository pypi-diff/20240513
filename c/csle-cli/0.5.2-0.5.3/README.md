# Comparing `tmp/csle_cli-0.5.2.tar.gz` & `tmp/csle_cli-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cli-0.5.2.tar", last modified: Tue Apr 30 10:50:31 2024, max compression
+gzip compressed data, was "csle_cli-0.5.3.tar", last modified: Mon May 13 17:20:34 2024, max compression
```

## Comparing `csle_cli-0.5.2.tar` & `csle_cli-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-04-30 10:50:31.894918 csle_cli-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)    23697 2024-01-29 12:14:49.000000 csle_cli-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-08-08 14:54:06.000000 csle_cli-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1998 2024-04-30 10:50:31.894918 csle_cli-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.890918 csle_cli-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/src/csle_cli/
--rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.5.2/src/csle_cli/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_cli-0.5.2/src/csle_cli/__version__.py
--rwxrwxr-x   0 kim       (1000) kim       (1000)   118330 2024-04-30 09:37:30.000000 csle_cli-0.5.2/src/csle_cli/cli.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/src/csle_cli.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      387 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       47 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/entry_points.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.5.2/src/csle_cli.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      699 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        9 2024-04-30 10:50:31.000000 csle_cli-0.5.2/src/csle_cli.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:31.894918 csle_cli-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      352 2023-08-08 14:54:06.000000 csle_cli-0.5.2/tests/test_cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:34.322827 csle_cli-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-05-13 17:20:34.322827 csle_cli-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)    23697 2024-01-29 12:14:49.000000 csle_cli-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      668 2023-08-08 14:54:06.000000 csle_cli-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1998 2024-05-13 17:20:34.322827 csle_cli-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cli-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:34.318827 csle_cli-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:34.322827 csle_cli-0.5.3/src/csle_cli/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       38 2023-03-28 14:03:22.000000 csle_cli-0.5.3/src/csle_cli/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_cli-0.5.3/src/csle_cli/__version__.py
+-rwxrwxr-x   0 kim       (1000) kim       (1000)   118330 2024-05-13 17:10:17.000000 csle_cli-0.5.3/src/csle_cli/cli.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:34.322827 csle_cli-0.5.3/src/csle_cli.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      619 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      387 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       47 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:51:27.000000 csle_cli-0.5.3/src/csle_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      699 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        9 2024-05-13 17:20:34.000000 csle_cli-0.5.3/src/csle_cli.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:34.322827 csle_cli-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      352 2023-08-08 14:54:06.000000 csle_cli-0.5.3/tests/test_cli.py
```

### Comparing `csle_cli-0.5.2/PKG-INFO` & `csle_cli-0.5.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.5.2/README.md` & `csle_cli-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_cli-0.5.2/pyproject.toml` & `csle_cli-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cli-0.5.2/setup.cfg` & `csle_cli-0.5.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	click>=8.1.3
-	csle-base>=0.5.2
-	csle-common>=0.5.2
-	csle-cluster>=0.5.2
-	csle-collector>=0.5.2
-	csle-attacker>=0.5.2
-	csle-defender>=0.5.2
-	csle-system-identification>=0.5.2
-	gym-csle-stopping-game>=0.5.2
-	gym-csle-apt-game>=0.5.2
-	gym-csle-cyborg>=0.5.2
-	gym-csle-intrusion-response-game>=0.5.2
-	csle-agents>=0.5.2
-	csle-tolerance>=0.5.2
+	csle-base>=0.5.3
+	csle-common>=0.5.3
+	csle-cluster>=0.5.3
+	csle-collector>=0.5.3
+	csle-attacker>=0.5.3
+	csle-defender>=0.5.3
+	csle-system-identification>=0.5.3
+	gym-csle-stopping-game>=0.5.3
+	gym-csle-apt-game>=0.5.3
+	gym-csle-cyborg>=0.5.3
+	gym-csle-intrusion-response-game>=0.5.3
+	csle-agents>=0.5.3
+	csle-tolerance>=0.5.3
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cli-0.5.2/src/csle_cli/cli.py` & `csle_cli-0.5.3/src/csle_cli/cli.py`

 * *Files identical despite different names*

### Comparing `csle_cli-0.5.2/src/csle_cli.egg-info/PKG-INFO` & `csle_cli-0.5.3/src/csle_cli.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cli
-Version: 0.5.2
+Version: 0.5.3
 Summary: CLI tool for CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cli-0.5.2/src/csle_cli.egg-info/requires.txt` & `csle_cli-0.5.3/src/csle_cli.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 click>=8.1.3
-csle-base>=0.5.2
-csle-common>=0.5.2
-csle-cluster>=0.5.2
-csle-collector>=0.5.2
-csle-attacker>=0.5.2
-csle-defender>=0.5.2
-csle-system-identification>=0.5.2
-gym-csle-stopping-game>=0.5.2
-gym-csle-apt-game>=0.5.2
-gym-csle-cyborg>=0.5.2
-gym-csle-intrusion-response-game>=0.5.2
-csle-agents>=0.5.2
-csle-tolerance>=0.5.2
+csle-base>=0.5.3
+csle-common>=0.5.3
+csle-cluster>=0.5.3
+csle-collector>=0.5.3
+csle-attacker>=0.5.3
+csle-defender>=0.5.3
+csle-system-identification>=0.5.3
+gym-csle-stopping-game>=0.5.3
+gym-csle-apt-game>=0.5.3
+gym-csle-cyborg>=0.5.3
+gym-csle-intrusion-response-game>=0.5.3
+csle-agents>=0.5.3
+csle-tolerance>=0.5.3
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

