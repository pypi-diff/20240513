# Comparing `tmp/csle_attacker-0.5.2.tar.gz` & `tmp/csle_attacker-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_attacker-0.5.2.tar", last modified: Tue Apr 30 10:49:36 2024, max compression
+gzip compressed data, was "csle_attacker-0.5.3.tar", last modified: Mon May 13 17:19:42 2024, max compression
```

## Comparing `csle_attacker-0.5.2.tar` & `csle_attacker-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     3866 2024-01-29 11:24:00.000000 csle_attacker-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-08-08 14:54:06.000000 csle_attacker-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1734 2024-04-30 10:49:36.290637 csle_attacker-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.282637 csle_attacker-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.282637 csle_attacker-0.5.2/src/csle_attacker/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_attacker-0.5.2/src/csle_attacker/__version__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      941 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/attacker.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/src/csle_attacker/emulation/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      994 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/attacker_stopping_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/emulated_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11564 2023-07-28 08:44:18.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4678 2023-07-28 08:44:18.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/post_exploit_middleware.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/recon_middleware.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/src/csle_attacker/emulation/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    45676 2024-01-29 11:24:00.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/util/exploit_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     7720 2023-07-28 08:44:18.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/util/nikto_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    34952 2024-01-29 11:24:00.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/util/nmap_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    30139 2023-07-28 08:44:18.000000 csle_attacker-0.5.2/src/csle_attacker/emulation/util/shell_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/src/csle_attacker.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-04-30 10:49:36.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      941 2024-04-30 10:49:36.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:49:36.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      475 2024-04-30 10:49:36.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       14 2024-04-30 10:49:36.000000 csle_attacker-0.5.2/src/csle_attacker.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:36.286637 csle_attacker-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1790 2024-01-29 11:24:00.000000 csle_attacker-0.5.2/tests/test_shell_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3866 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2023-08-08 14:54:06.000000 csle_attacker-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1734 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/csle_attacker/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_attacker-0.5.3/src/csle_attacker/__version__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      941 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/attacker.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/src/csle_attacker/emulation/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      994 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/attacker_stopping_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11411 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/emulated_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11564 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4678 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/post_exploit_middleware.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5951 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/recon_middleware.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/src/csle_attacker/emulation/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    45676 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/exploit_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7720 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/nikto_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    34952 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/nmap_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    30139 2023-07-28 08:44:18.000000 csle_attacker-0.5.3/src/csle_attacker/emulation/util/shell_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.158508 csle_attacker-0.5.3/src/csle_attacker.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      649 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      941 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:55.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      475 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       14 2024-05-13 17:19:42.000000 csle_attacker-0.5.3/src/csle_attacker.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:19:42.162508 csle_attacker-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1790 2024-01-29 11:24:00.000000 csle_attacker-0.5.3/tests/test_shell_util.py
```

### Comparing `csle_attacker-0.5.2/PKG-INFO` & `csle_attacker-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_attacker
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.5.2/README.md` & `csle_attacker-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/pyproject.toml` & `csle_attacker-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/setup.cfg` & `csle_attacker-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

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

### Comparing `csle_attacker-0.5.2/src/csle_attacker/attacker.py` & `csle_attacker-0.5.3/src/csle_attacker/attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/attacker_stopping_middleware.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/attacker_stopping_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/emulated_attacker.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/emulated_attacker.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/exploit_middleware.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/post_exploit_middleware.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/post_exploit_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/recon_middleware.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/recon_middleware.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/util/exploit_util.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/util/exploit_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/util/nikto_util.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/util/nikto_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/util/nmap_util.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/util/nmap_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker/emulation/util/shell_util.py` & `csle_attacker-0.5.3/src/csle_attacker/emulation/util/shell_util.py`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/src/csle_attacker.egg-info/PKG-INFO` & `csle_attacker-0.5.3/src/csle_attacker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-attacker
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for emulated cyber attacks in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_attacker-0.5.2/src/csle_attacker.egg-info/SOURCES.txt` & `csle_attacker-0.5.3/src/csle_attacker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_attacker-0.5.2/tests/test_shell_util.py` & `csle_attacker-0.5.3/tests/test_shell_util.py`

 * *Files identical despite different names*

