# Comparing `tmp/csle_cluster-0.5.2.tar.gz` & `tmp/csle_cluster-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_cluster-0.5.2.tar", last modified: Tue Apr 30 10:50:37 2024, max compression
+gzip compressed data, was "csle_cluster-0.5.3.tar", last modified: Mon May 13 17:20:39 2024, max compression
```

## Comparing `csle_cluster-0.5.2.tar` & `csle_cluster-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     4307 2024-01-29 12:14:49.000000 csle_cluster-0.5.2/README.md
--rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-08-08 14:54:06.000000 csle_cluster-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     2067 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.302945 csle_cluster-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.302945 csle_cluster-0.5.2/src/csle_cluster/
--rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.5.2/src/csle_cluster/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_cluster-0.5.2/src/csle_cluster/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   240982 2024-04-30 09:37:30.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_controller.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   270830 2024-04-30 09:37:30.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    94763 2024-01-29 11:24:00.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   349493 2024-01-29 11:24:00.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   207915 2024-01-29 11:24:00.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   204861 2024-01-29 11:24:00.000000 csle_cluster-0.5.2/src/csle_cluster/cluster_manager/query_cluster_manager.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/src/csle_cluster/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.2/src/csle_cluster/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      459 2023-08-08 14:54:06.000000 csle_cluster-0.5.2/src/csle_cluster/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.306945 csle_cluster-0.5.2/src/csle_cluster.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-04-30 10:50:37.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      835 2024-04-30 10:50:37.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:37.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      689 2024-04-30 10:50:37.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       13 2024-04-30 10:50:37.000000 csle_cluster-0.5.2/src/csle_cluster.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:37.310945 csle_cluster-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)   355781 2024-01-29 11:24:00.000000 csle_cluster-0.5.2/tests/test_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4307 2024-01-29 12:14:49.000000 csle_cluster-0.5.3/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      672 2023-08-08 14:54:06.000000 csle_cluster-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2067 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/csle_cluster/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_cluster-0.5.3/src/csle_cluster/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.974861 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   240982 2024-04-30 09:37:30.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_controller.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   270830 2024-05-13 17:10:17.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    94763 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   349493 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   207915 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   204861 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/src/csle_cluster/cluster_manager/query_cluster_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/src/csle_cluster/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 csle_cluster-0.5.3/src/csle_cluster/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      459 2023-08-08 14:54:06.000000 csle_cluster-0.5.3/src/csle_cluster/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.970861 csle_cluster-0.5.3/src/csle_cluster.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      794 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      835 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-04 13:33:55.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      689 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       13 2024-05-13 17:20:39.000000 csle_cluster-0.5.3/src/csle_cluster.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:39.978861 csle_cluster-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)   355781 2024-01-29 11:24:00.000000 csle_cluster-0.5.3/tests/test_cluster_manager.py
```

### Comparing `csle_cluster-0.5.2/PKG-INFO` & `csle_cluster-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_cluster
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.5.2/README.md` & `csle_cluster-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/pyproject.toml` & `csle_cluster-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/setup.cfg` & `csle_cluster-0.5.3/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	grpcio>=1.57.0
 	grpcio-tools>=1.57.0
-	csle-base>=0.5.2
-	csle-collector>=0.5.2
-	csle-common>=0.5.2
-	csle-ryu>=0.5.2
-	gym-csle-stopping-game>=0.5.2
-	gym-csle-intrusion-response-game>=0.5.2
-	gym-csle-apt-game>=0.5.2
-	gym-csle-cyborg>=0.5.2
-	csle-tolerance>=0.5.2
+	csle-base>=0.5.3
+	csle-collector>=0.5.3
+	csle-common>=0.5.3
+	csle-ryu>=0.5.3
+	gym-csle-stopping-game>=0.5.3
+	gym-csle-intrusion-response-game>=0.5.3
+	gym-csle-apt-game>=0.5.3
+	gym-csle-cyborg>=0.5.3
+	csle-tolerance>=0.5.3
 python_requires = >=3.5
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_controller.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_controller.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_pb2.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/cluster_manager_util.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/cluster_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster/cluster_manager/query_cluster_manager.py` & `csle_cluster-0.5.3/src/csle_cluster/cluster_manager/query_cluster_manager.py`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster.egg-info/PKG-INFO` & `csle_cluster-0.5.3/src/csle_cluster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-cluster
-Version: 0.5.2
+Version: 0.5.3
 Summary: Scripts for cluster management in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_cluster-0.5.2/src/csle_cluster.egg-info/SOURCES.txt` & `csle_cluster-0.5.3/src/csle_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_cluster-0.5.2/src/csle_cluster.egg-info/requires.txt` & `csle_cluster-0.5.3/src/csle_cluster.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
-csle-base>=0.5.2
-csle-collector>=0.5.2
-csle-common>=0.5.2
-csle-ryu>=0.5.2
-gym-csle-stopping-game>=0.5.2
-gym-csle-intrusion-response-game>=0.5.2
-gym-csle-apt-game>=0.5.2
-gym-csle-cyborg>=0.5.2
-csle-tolerance>=0.5.2
+csle-base>=0.5.3
+csle-collector>=0.5.3
+csle-common>=0.5.3
+csle-ryu>=0.5.3
+gym-csle-stopping-game>=0.5.3
+gym-csle-intrusion-response-game>=0.5.3
+gym-csle-apt-game>=0.5.3
+gym-csle-cyborg>=0.5.3
+csle-tolerance>=0.5.3
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

### Comparing `csle_cluster-0.5.2/tests/test_cluster_manager.py` & `csle_cluster-0.5.3/tests/test_cluster_manager.py`

 * *Files identical despite different names*

