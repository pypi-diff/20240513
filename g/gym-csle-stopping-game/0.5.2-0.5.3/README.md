# Comparing `tmp/gym_csle_stopping_game-0.5.2.tar.gz` & `tmp/gym_csle_stopping_game-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_stopping_game-0.5.2.tar", last modified: Tue Apr 30 10:49:55 2024, max compression
+gzip compressed data, was "gym_csle_stopping_game-0.5.3.tar", last modified: Mon May 13 17:20:00 2024, max compression
```

## Comparing `gym_csle_stopping_game-0.5.2.tar` & `gym_csle_stopping_game-0.5.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-08-08 14:54:06.000000 gym_csle_stopping_game-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1894 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.654736 gym_csle_stopping_game-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.654736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/
--rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.654736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3494 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6640 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3753 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2828 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_state.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    22753 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10877 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    10580 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11363 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/util/stopping_game_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.654736 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-04-30 10:49:55.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1195 2024-04-30 10:49:55.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:49:55.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-04-30 10:49:55.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       23 2024-04-30 10:49:55.000000 gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:49:55.658736 gym_csle_stopping_game-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     4825 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.2/tests/test_stopping_game_dao.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8353 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.2/tests/test_stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      703 2023-08-08 14:54:06.000000 gym_csle_stopping_game-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1894 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      657 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1030 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3494 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6640 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3753 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2828 2024-04-30 03:46:58.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_state.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       74 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    22753 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10877 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10580 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2023-03-28 14:03:22.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11363 2024-04-30 09:37:30.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/stopping_game_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.382620 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      705 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1195 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:50:52.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      557 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       23 2024-05-13 17:20:00.000000 gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:00.386620 gym_csle_stopping_game-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4825 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.3/tests/test_stopping_game_dao.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8353 2024-01-29 12:14:49.000000 gym_csle_stopping_game-0.5.3/tests/test_stopping_game_util.py
```

### Comparing `gym_csle_stopping_game-0.5.2/PKG-INFO` & `gym_csle_stopping_game-0.5.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_stopping_game
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.5.2/pyproject.toml` & `gym_csle_stopping_game-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/setup.cfg` & `gym_csle_stopping_game-0.5.3/setup.cfg`

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

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/__init__.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/__init__.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/constants/constants.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_attacker_mdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_config.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_defender_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/dao/stopping_game_state.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/dao/stopping_game_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_env.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_mdp_attacker_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/envs/stopping_game_pomdp_defender_env.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game/util/stopping_game_util.py` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game/util/stopping_game_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/PKG-INFO` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-stopping-game
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment of a Dynkin (Optimal stopping) game in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/SOURCES.txt` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/src/gym_csle_stopping_game.egg-info/requires.txt` & `gym_csle_stopping_game-0.5.3/src/gym_csle_stopping_game.egg-info/requires.txt`

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

### Comparing `gym_csle_stopping_game-0.5.2/tests/test_stopping_game_dao.py` & `gym_csle_stopping_game-0.5.3/tests/test_stopping_game_dao.py`

 * *Files identical despite different names*

### Comparing `gym_csle_stopping_game-0.5.2/tests/test_stopping_game_util.py` & `gym_csle_stopping_game-0.5.3/tests/test_stopping_game_util.py`

 * *Files identical despite different names*

