# Comparing `tmp/csle_tolerance-0.5.2.tar.gz` & `tmp/csle_tolerance-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_tolerance-0.5.2.tar", last modified: Tue Apr 30 10:50:43 2024, max compression
+gzip compressed data, was "csle_tolerance-0.5.3.tar", last modified: Mon May 13 17:20:45 2024, max compression
```

## Comparing `csle_tolerance-0.5.2.tar` & `csle_tolerance-0.5.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/
--rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)      674 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/pyproject.toml
--rw-rw-r--   0 kim       (1000) kim       (1000)     1929 2024-04-30 10:50:43.162974 csle_tolerance-0.5.2/setup.cfg
--rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/setup.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.154974 csle_tolerance-0.5.2/src/
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.154974 csle_tolerance-0.5.2/src/csle_tolerance/
--rw-rw-r--   0 kim       (1000) kim       (1000)       39 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-04-30 10:49:10.000000 csle_tolerance-0.5.2/src/csle_tolerance/__version__.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/constants/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/constants/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)      315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/constants/constants.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/dao/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5699 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5231 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/envs/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    11235 2024-01-29 12:14:49.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     8025 2024-01-29 12:14:49.000000 csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance/util/
--rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/__init__.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2587 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/general_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)    13315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     5895 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py
--rw-rw-r--   0 kim       (1000) kim       (1000)     2058 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/src/csle_tolerance/util/pomdp_solve_parser.py
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/
--rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/PKG-INFO
--rw-rw-r--   0 kim       (1000) kim       (1000)     1007 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/SOURCES.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/dependency_links.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-09-16 07:31:36.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/not-zip-safe
--rw-rw-r--   0 kim       (1000) kim       (1000)      571 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/requires.txt
--rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-04-30 10:50:43.000000 csle_tolerance-0.5.2/src/csle_tolerance.egg-info/top_level.txt
-drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-04-30 10:50:43.158974 csle_tolerance-0.5.2/tests/
--rw-rw-r--   0 kim       (1000) kim       (1000)      405 2024-01-29 11:24:00.000000 csle_tolerance-0.5.2/tests/test_intrusion_recovery_pomdp_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1929 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       39 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2024-05-13 17:19:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      315 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance/dao/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5370 2024-05-13 17:10:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_game_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5699 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5231 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_response_cmdp_config.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/src/csle_tolerance/envs/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11235 2024-01-29 12:14:49.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8025 2024-01-29 12:14:49.000000 csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_response_cmdp_env.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/src/csle_tolerance/util/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2587 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/general_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    20399 2024-05-13 17:10:17.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5895 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_response_cmdp_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2058 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/src/csle_tolerance/util/pomdp_solve_parser.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.174893 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      741 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1064 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-09-16 07:31:36.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      571 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2024-05-13 17:20:45.000000 csle_tolerance-0.5.3/src/csle_tolerance.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2024-05-13 17:20:45.178893 csle_tolerance-0.5.3/tests/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      405 2024-01-29 11:24:00.000000 csle_tolerance-0.5.3/tests/test_intrusion_recovery_pomdp_util.py
```

### Comparing `csle_tolerance-0.5.2/PKG-INFO` & `csle_tolerance-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_tolerance
-Version: 0.5.2
+Version: 0.5.3
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.2/pyproject.toml` & `csle_tolerance-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/setup.cfg` & `csle_tolerance-0.5.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
 	gymnasium>=0.27.1
 	numpy>=1.23.5
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

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py` & `csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/dao/intrusion_response_cmdp_config.py` & `csle_tolerance-0.5.3/src/csle_tolerance/dao/intrusion_response_cmdp_config.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py` & `csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/envs/intrusion_response_cmdp_env.py` & `csle_tolerance-0.5.3/src/csle_tolerance/envs/intrusion_response_cmdp_env.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/util/general_util.py` & `csle_tolerance-0.5.3/src/csle_tolerance/util/general_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py` & `csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_recovery_pomdp_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import List
 from scipy.stats import betabinom
 import numpy as np
 from csle_tolerance.dao.intrusion_recovery_pomdp_config import IntrusionRecoveryPomdpConfig
+from csle_tolerance.dao.intrusion_recovery_game_config import IntrusionRecoveryGameConfig
 
 
 class IntrusionRecoveryPomdpUtil:
     """
     Class with utility functions for the intrusion-recovery POMDP
     """
 
@@ -22,15 +23,15 @@
     def initial_belief(p_a: float) -> List[float]:
         """
         Gets the initial belief state of the POMDP
 
         :param p_a: the attack probability
         :return: the initial belief state
         """
-        return [1 - p_a, p_a, 0]
+        return [1, 0, 0]
 
     @staticmethod
     def action_space() -> List[int]:
         """
         Gets the action space of the POMDP
 
         :return: a list with the actions
@@ -162,14 +163,41 @@
             return (1.0 - p_c_1) * p_a
         elif s_prime == 1 and s == 1 and a == 0:
             return (1 - p_c_2) * (1 - p_u)
         else:
             return 0
 
     @staticmethod
+    def transition_function_game(s: int, s_prime: int, a1: int, a2: int, p_a: float, p_c_1: float) -> float:
+        """
+        The transition function of the POSG
+
+        :param s: the state
+        :param s_prime: the next state
+        :param a1: the defender action
+        :param a2: the attacker action
+        :param p_a: the intrusion probability
+        :param p_c_1: the crash probability
+        :return: P(s_prime | s, a1, a2)
+        """
+        if s == 2 and s_prime == 2:
+            return 1.0
+        elif s_prime == 2 and s in [0, 1]:
+            return p_c_1
+        elif s_prime == 0 and a1 == 0 and a2 == 1 and s == 0:
+            return (1 - p_a) * (1 - p_c_1)
+        elif (s_prime == 0 and a2 == 0 and s == 0) or (s_prime == 0 and s == 1 and a1 == 1) \
+                or (s_prime == 1 and s == 1 and a1 == 0):
+            return (1 - p_c_1)
+        elif (s_prime == 1 and s == 0 and a2 == 1):
+            return (1 - p_c_1) * p_a
+        else:
+            return 0
+
+    @staticmethod
     def transition_tensor(states: List[int], actions: List[int], p_a: float, p_c_1: float, p_c_2: float, p_u: float) \
             -> List[List[List[float]]]:
         """
         Creates a |A|x|S|x|S| tensor with the transition probabilities of the POMDP
 
         :param states: the list of states
         :param actions: the list of actions
@@ -183,19 +211,48 @@
         for a in actions:
             a_transitions = []
             for s in states:
                 s_a_transitions = []
                 for s_prime in states:
                     s_a_transitions.append(IntrusionRecoveryPomdpUtil.transition_function(
                         s=s, s_prime=s_prime, a=a, p_a=p_a, p_c_1=p_c_1, p_c_2=p_c_2, p_u=p_u))
+                assert round(sum(s_a_transitions), 2) == 1.0
                 a_transitions.append(s_a_transitions)
             transition_tensor.append(a_transitions)
         return transition_tensor
 
     @staticmethod
+    def transition_tensor_game(states: List[int], defender_actions: List[int], attacker_actions: List[int],
+                               p_a: float, p_c_1: float) -> List[List[List[List[float]]]]:
+        """
+        Creates a |A|x|A|x|S|x|S| tensor with the transition probabilities of the POSG
+
+        :param states: the list of states
+        :param defender_actions: the list of defender actions
+        :param attacker_actions: the list of attacker actions
+        :param p_a: the intrusion probability
+        :param p_c_1: the crash probability
+        :return: the transition tensor
+        """
+        transition_tensor = []
+        for a1 in defender_actions:
+            a1_transitions = []
+            for a2 in attacker_actions:
+                a2_transitions = []
+                for s in states:
+                    s_a1_a2_transitions = []
+                    for s_prime in states:
+                        s_a1_a2_transitions.append(IntrusionRecoveryPomdpUtil.transition_function_game(
+                            s=s, s_prime=s_prime, a1=a1, a2=a2, p_a=p_a, p_c_1=p_c_1))
+                    a2_transitions.append(s_a1_a2_transitions)
+                a1_transitions.append(a2_transitions)
+            transition_tensor.append(a1_transitions)
+        return transition_tensor
+
+    @staticmethod
     def sample_initial_state(b1: List[float]) -> int:
         """
         Samples the initial state
 
         :param b1: the initial belief
         :return: the initial state
         """
@@ -214,14 +271,28 @@
         observation_probs = []
         for o in observations:
             observation_probs.append(observation_tensor[s_prime][o])
         o = np.random.choice(np.arange(0, len(observations)), p=observation_probs)
         return int(o)
 
     @staticmethod
+    def sample_next_state_game(transition_tensor: List[List[List[List[float]]]], s: int, a1: int, a2: int) -> int:
+        """
+        Samples the next observation
+
+        :param s: the current state
+        :param a1: the defender action
+        :param a2: the attacker action
+        :param transition_tensor: the transition tensor
+        :return: the next state a
+        """
+        s_prime = np.random.choice(np.arange(0, len(transition_tensor[a1][a2][s])), p=transition_tensor[a1][a2][s])
+        return int(s_prime)
+
+    @staticmethod
     def bayes_filter(s_prime: int, o: int, a: int, b: List[float], states: List[int], observations: List[int],
                      observation_tensor: List[List[float]], transition_tensor: List[List[List[float]]]) -> float:
         """
         A Bayesian filter to compute b[s_prime] of the POMDP
 
         :param s_prime: the state to compute the belief for
         :param o: the latest observation
@@ -338,7 +409,96 @@
         for s in config.states:
             for a in config.actions:
                 for s_prime in config.states:
                     for o in config.observations:
                         c = config.cost_tensor[a][s]
                         file_str = file_str + f"R: {a} : {s} : {s_prime} : {o} {c:.80f}\n"
         return file_str
+
+    @staticmethod
+    def generate_transitions(game_config: IntrusionRecoveryGameConfig) -> List[str]:
+        """
+        Generates the transition rows of the POSG config file of HSVI
+
+        :param game_config: the game configuration
+        :return: list of transition rows
+        """
+        transitions = []
+        for s in game_config.states:
+            for a1 in game_config.actions:
+                for a2 in game_config.actions:
+                    for s_prime in game_config.states:
+                        for i, _ in enumerate(game_config.observations):
+                            tr_prob = game_config.transition_tensor[a1][a2][s][s_prime]
+                            obs_prob = game_config.observation_tensor[a2][i]
+                            prob = tr_prob * obs_prob
+                            if prob > 0:
+                                transition = f"{s} {a1} {a2} {i} {s_prime} {prob}"
+                                transitions.append(transition)
+
+        return transitions
+
+    @staticmethod
+    def generate_rewards(game_config: IntrusionRecoveryGameConfig) -> List[str]:
+        """
+        Generates the reward rows of the POSG config file of HSVI
+
+        :param game_config: the game configuration
+        :return: list of reward rows
+        """
+        rewards = []
+        for s in game_config.states:
+            for a1 in game_config.actions:
+                for a2 in game_config.actions:
+                    r = -game_config.cost_tensor[a1][s]
+                    if r != 0:
+                        rew = f"{s} {a1} {a2} {r}"
+                        rewards.append(rew)
+        return rewards
+
+    @staticmethod
+    def generate_os_posg_game_file(game_config: IntrusionRecoveryGameConfig) -> str:
+        """
+        Generates the POSG game file for HSVI
+
+        :param game_config: the game configuration
+        :return: a string with the contents of the config file
+        """
+        num_partitions = 1
+        transitions = IntrusionRecoveryPomdpUtil.generate_transitions(game_config=game_config)
+        rewards = IntrusionRecoveryPomdpUtil.generate_rewards(game_config=game_config)
+        game_description = f"{len(game_config.states)} {num_partitions} {len(game_config.actions)} " \
+                           f"{len(game_config.actions)} " \
+                           f"{len(game_config.observations)} {len(transitions)} " \
+                           f"{len(rewards)} {game_config.discount_factor}"
+        state_desriptions = []
+        for s in game_config.states:
+            state_desriptions.append(f"{s} {0}")
+        player_1_actions = ["WAIT", "RECOVER"]
+        player_2_actions = ["FALSEALARM", "ATTACK"]
+
+        player_2_legal_actions = []
+        for _ in game_config.states:
+            player_2_legal_actions.append(" ".join(list(map(lambda x: str(x), game_config.actions))))
+
+        player_1_legal_actions = []
+        player_1_legal_actions.append(" ".join(list(map(lambda x: str(x), game_config.actions))))
+
+        obs_desriptions = []
+        for i, o in enumerate(game_config.observations):
+            obs_desriptions.append(f"o_{o}")
+
+        initial_belief_str = f"{0} {' '.join(list(map(lambda x: str(x), game_config.b1)))}"
+        game_file_str = ""
+        game_file_str = game_file_str + game_description + "\n"
+        game_file_str = game_file_str + "\n".join(state_desriptions) + "\n"
+        game_file_str = game_file_str + "\n".join(player_1_actions) + "\n"
+        game_file_str = game_file_str + "\n".join(player_2_actions) + "\n"
+        game_file_str = game_file_str + "\n".join(obs_desriptions) + "\n"
+        game_file_str = game_file_str + "\n".join(player_2_legal_actions) + "\n"
+        game_file_str = game_file_str + "\n".join(player_1_legal_actions) + "\n"
+        game_file_str = game_file_str + "\n".join(transitions) + "\n"
+        game_file_str = game_file_str + "\n".join(rewards) + "\n"
+        game_file_str = game_file_str + initial_belief_str
+        with open('recovery_game.txt', 'w') as f:
+            f.write(game_file_str)
+        return game_file_str
```

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/util/intrusion_response_cmdp_util.py` & `csle_tolerance-0.5.3/src/csle_tolerance/util/intrusion_response_cmdp_util.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance/util/pomdp_solve_parser.py` & `csle_tolerance-0.5.3/src/csle_tolerance/util/pomdp_solve_parser.py`

 * *Files identical despite different names*

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/PKG-INFO` & `csle_tolerance-0.5.3/src/csle_tolerance.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-tolerance
-Version: 0.5.2
+Version: 0.5.3
 Summary: An intrusion-tolerant system: Tolerance: (T)w(o)-(l)ev(e)l (r)ecovery (a)nd respo(n)se (c)ontrol with f(e)edback.
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes Intrusion-tolerance
 Platform: unix
 Platform: linux
```

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/SOURCES.txt` & `csle_tolerance-0.5.3/src/csle_tolerance.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/csle_tolerance.egg-info/dependency_links.txt
 src/csle_tolerance.egg-info/not-zip-safe
 src/csle_tolerance.egg-info/requires.txt
 src/csle_tolerance.egg-info/top_level.txt
 src/csle_tolerance/constants/__init__.py
 src/csle_tolerance/constants/constants.py
 src/csle_tolerance/dao/__init__.py
+src/csle_tolerance/dao/intrusion_recovery_game_config.py
 src/csle_tolerance/dao/intrusion_recovery_pomdp_config.py
 src/csle_tolerance/dao/intrusion_response_cmdp_config.py
 src/csle_tolerance/envs/__init__.py
 src/csle_tolerance/envs/intrusion_recovery_pomdp_env.py
 src/csle_tolerance/envs/intrusion_response_cmdp_env.py
 src/csle_tolerance/util/__init__.py
 src/csle_tolerance/util/general_util.py
```

### Comparing `csle_tolerance-0.5.2/src/csle_tolerance.egg-info/requires.txt` & `csle_tolerance-0.5.3/src/csle_tolerance.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 gymnasium>=0.27.1
 numpy>=1.23.5
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

