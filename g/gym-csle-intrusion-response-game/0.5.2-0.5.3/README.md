# Comparing `tmp/gym_csle_intrusion_response_game-0.5.2.tar.gz` & `tmp/gym_csle_intrusion_response_game-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_intrusion_response_game-0.5.2.tar", last modified: Tue Apr 30 10:50:07 2024, max compression
+gzip compressed data, was "gym_csle_intrusion_response_game-0.5.3.tar", last modified: Mon May 13 17:20:10 2024, max compression
```

## Comparing `gym_csle_intrusion_response_game-0.5.2.tar` & `gym_csle_intrusion_response_game-0.5.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:07.022793 gym_csle_intrusion_response_game-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-04-30 10:50:07.022793 gym_csle_intrusion_response_game-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-08-08 14:54:06.000000 gym_csle_intrusion_response_game-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1918 2024-04-30 10:50:07.026793 gym_csle_intrusion_response_game-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:06.982793 gym_csle_intrusion_response_game-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:06.982793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1479 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:06.986793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1841 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:06.998793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4661 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4392 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     4160 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6988 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5336 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:07.022793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)      749 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    15417 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    18684 2024-04-30 09:37:30.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    14261 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13470 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    17124 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:07.022793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    55338 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:06.986793 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-04-30 10:50:06.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1979 2024-04-30 10:50:06.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:06.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 11:24:24.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-04-30 10:50:06.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       33 2024-04-30 10:50:06.000000 gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:07.022793 gym_csle_intrusion_response_game-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      732 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.2/tests/test_intrusion_response_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      713 2023-08-08 14:54:06.000000 gym_csle_intrusion_response_game-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1918 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1479 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1841 2023-04-30 06:59:23.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4661 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4392 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4160 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6988 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5336 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3445 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      749 2023-04-23 07:07:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15417 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    18684 2024-04-30 09:37:30.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14261 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13470 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    17124 2024-01-29 12:14:49.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    55338 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.982685 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      709 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1979 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 11:24:24.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       33 2024-05-13 17:20:10.000000 gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:10.986685 gym_csle_intrusion_response_game-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      732 2024-01-29 11:24:00.000000 gym_csle_intrusion_response_game-0.5.3/tests/test_intrusion_response_game_util.py
```

### Comparing `gym_csle_intrusion_response_game-0.5.2/PKG-INFO` & `gym_csle_intrusion_response_game-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_intrusion_response_game
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.5.2/pyproject.toml` & `gym_csle_intrusion_response_game-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/setup.cfg` & `gym_csle_intrusion_response_game-0.5.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
-	csle-base>=0.5.2
-	csle-common>=0.5.2
-	csle-attacker>=0.5.2
-	csle-defender>=0.5.2
-	csle-collector>=0.5.2
+	csle-base>=0.5.3
+	csle-common>=0.5.3
+	csle-attacker>=0.5.3
+	csle-defender>=0.5.3
+	csle-collector>=0.5.3
 python_requires = >=3.8
 package_dir = 
 	=src
 packages = find:
 zip_safe = no
 
 [options.packages.find]
```

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/__init__.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/constants/constants.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_local_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/intrusion_response_game_state_local.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/local_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_attacker_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/dao/workflow_intrusion_response_pomdp_defender_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/__init__.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_local_stopping_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_attacker.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/envs/intrusion_response_game_workflow_pomdp_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game/util/intrusion_response_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-intrusion-response-game
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment of an intrusion response game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_intrusion_response_game-0.5.2/src/gym_csle_intrusion_response_game.egg-info/requires.txt` & `gym_csle_intrusion_response_game-0.5.3/src/gym_csle_intrusion_response_game.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 gymnasium>=0.27.1
-csle-base>=0.5.2
-csle-common>=0.5.2
-csle-attacker>=0.5.2
-csle-defender>=0.5.2
-csle-collector>=0.5.2
+csle-base>=0.5.3
+csle-common>=0.5.3
+csle-attacker>=0.5.3
+csle-defender>=0.5.3
+csle-collector>=0.5.3
 
 [testing]
 pytest>=6.0
 pytest-cov>=2.0
 pytest-mock>=3.6.0
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
```

### Comparing `gym_csle_intrusion_response_game-0.5.2/tests/test_intrusion_response_game_util.py` & `gym_csle_intrusion_response_game-0.5.3/tests/test_intrusion_response_game_util.py`

 * *Files identical despite different names*

