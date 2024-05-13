# Comparing `tmp/gym_csle_cyborg-0.5.2.tar.gz` & `tmp/gym_csle_cyborg-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_csle_cyborg-0.5.2.tar", last modified: Tue Apr 30 10:51:03 2024, max compression
+gzip compressed data, was "gym_csle_cyborg-0.5.3.tar", last modified: Mon May 13 17:21:07 2024, max compression
```

## Comparing `gym_csle_cyborg-0.5.2.tar` & `gym_csle_cyborg-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      696 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1868 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.107072 gym_csle_cyborg-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.107072 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/
--rw-rw-r--   0 kim       (1000) kim       (1000)      469 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.107072 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2774 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      788 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/activity_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1926 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/blue_agent_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      939 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/compromised_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6822 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/csle_cyborg_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     3966 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/csle_cyborg_wrapper_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     6284 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/cyborg_wrapper_state.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      260 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/decoy_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      302 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/exploit_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     1154 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/red_agent_action_type.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      197 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/red_agent_type.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)      174 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    49858 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/cyborg_scenario_two_defender.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    88819 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/cyborg_scenario_two_wrapper.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    33843 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/util/cyborg_env_util.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.107072 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      673 2024-04-30 10:51:03.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1239 2024-04-30 10:51:03.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:51:03.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-01-26 10:26:28.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      576 2024-04-30 10:51:03.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       16 2024-04-30 10:51:03.000000 gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:51:03.111073 gym_csle_cyborg-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)     1140 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/tests/test_csle_cyborg_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)   167720 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.2/tests/test_csle_cyborg_version_two_wrapper.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      696 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1868 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.723030 gym_csle_cyborg-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.727030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      469 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.727030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2774 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.727030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      788 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/activity_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1926 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/blue_agent_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      939 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/compromised_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6822 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/csle_cyborg_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3966 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/csle_cyborg_wrapper_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6284 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/cyborg_wrapper_state.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      260 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/decoy_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      302 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/exploit_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1154 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/red_agent_action_type.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      197 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/red_agent_type.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      174 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    49858 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/cyborg_scenario_two_defender.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    88819 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/cyborg_scenario_two_wrapper.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 12:14:49.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33843 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/util/cyborg_env_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.727030 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      673 2024-05-13 17:21:07.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1239 2024-05-13 17:21:07.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:21:07.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-01-26 10:26:28.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      576 2024-05-13 17:21:07.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       16 2024-05-13 17:21:07.000000 gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:21:07.731030 gym_csle_cyborg-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1140 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/tests/test_csle_cyborg_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)   167720 2024-04-30 09:37:30.000000 gym_csle_cyborg-0.5.3/tests/test_csle_cyborg_version_two_wrapper.py
```

### Comparing `gym_csle_cyborg-0.5.2/PKG-INFO` & `gym_csle_cyborg-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym_csle_cyborg
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment wrapper for CybORG
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_cyborg-0.5.2/pyproject.toml` & `gym_csle_cyborg-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/setup.cfg` & `gym_csle_cyborg-0.5.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
 	csle-cyborg>=0.0.2
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

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/constants/constants.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/constants/constants.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/activity_type.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/activity_type.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/blue_agent_action_type.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/blue_agent_action_type.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/compromised_type.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/compromised_type.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/csle_cyborg_config.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/csle_cyborg_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/csle_cyborg_wrapper_config.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/csle_cyborg_wrapper_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/cyborg_wrapper_state.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/cyborg_wrapper_state.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/dao/red_agent_action_type.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/dao/red_agent_action_type.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/cyborg_scenario_two_defender.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/cyborg_scenario_two_defender.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/envs/cyborg_scenario_two_wrapper.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/envs/cyborg_scenario_two_wrapper.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg/util/cyborg_env_util.py` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg/util/cyborg_env_util.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/PKG-INFO` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gym-csle-cyborg
-Version: 0.5.2
+Version: 0.5.3
 Summary: OpenAI gym reinforcement learning environment wrapper for CybORG
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/SOURCES.txt` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/src/gym_csle_cyborg.egg-info/requires.txt` & `gym_csle_cyborg-0.5.3/src/gym_csle_cyborg.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 gymnasium>=0.27.1
 csle-cyborg>=0.0.2
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

### Comparing `gym_csle_cyborg-0.5.2/tests/test_csle_cyborg_config.py` & `gym_csle_cyborg-0.5.3/tests/test_csle_cyborg_config.py`

 * *Files identical despite different names*

### Comparing `gym_csle_cyborg-0.5.2/tests/test_csle_cyborg_version_two_wrapper.py` & `gym_csle_cyborg-0.5.3/tests/test_csle_cyborg_version_two_wrapper.py`

 * *Files identical despite different names*

