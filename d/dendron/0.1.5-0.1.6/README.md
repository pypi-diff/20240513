# Comparing `tmp/dendron-0.1.5.tar.gz` & `tmp/dendron-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dendron-0.1.5.tar", last modified: Fri Apr  5 03:32:01 2024, max compression
+gzip compressed data, was "dendron-0.1.6.tar", last modified: Sun May 12 23:16:52 2024, max compression
```

## Comparing `dendron-0.1.5.tar` & `dendron-0.1.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/
--rw-r--r--   0 richard   (1000) richard   (1000)     1504 2024-02-06 04:46:44.000000 dendron-0.1.5/LICENSE
--rw-r--r--   0 richard   (1000) richard   (1000)     2704 2024-04-05 03:32:01.682918 dendron-0.1.5/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)     1957 2024-03-15 03:58:37.000000 dendron-0.1.5/README.md
--rw-r--r--   0 richard   (1000) richard   (1000)      888 2024-04-05 03:31:45.000000 dendron-0.1.5/pyproject.toml
--rw-r--r--   0 richard   (1000) richard   (1000)       65 2024-04-05 03:32:01.682918 dendron-0.1.5/setup.cfg
--rw-r--r--   0 richard   (1000) richard   (1000)      316 2024-04-05 03:31:36.000000 dendron-0.1.5/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.678918 dendron-0.1.5/src/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.678918 dendron-0.1.5/src/dendron/
--rw-r--r--   0 richard   (1000) richard   (1000)      565 2024-04-05 03:31:50.000000 dendron-0.1.5/src/dendron/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1929 2024-01-30 20:13:57.000000 dendron-0.1.5/src/dendron/action_node.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/src/dendron/actions/
--rw-r--r--   0 richard   (1000) richard   (1000)      359 2024-02-20 05:31:46.000000 dendron-0.1.5/src/dendron/actions/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)      446 2024-02-11 21:58:50.000000 dendron-0.1.5/src/dendron/actions/always_failure.py
--rw-r--r--   0 richard   (1000) richard   (1000)      485 2024-02-11 21:58:56.000000 dendron-0.1.5/src/dendron/actions/always_success.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1805 2024-02-11 22:46:52.000000 dendron-0.1.5/src/dendron/actions/async_action.py
--rw-r--r--   0 richard   (1000) richard   (1000)    10231 2024-03-15 02:40:04.000000 dendron-0.1.5/src/dendron/actions/causal_lm_action.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    11138 2024-04-05 02:40:01.000000 dendron-0.1.5/src/dendron/actions/image_lm_action.py
--rw-r--r--   0 richard   (1000) richard   (1000)     3856 2024-02-11 22:50:10.000000 dendron-0.1.5/src/dendron/actions/pipeline_action.py
--rw-r--r--   0 richard   (1000) richard   (1000)      803 2024-02-11 22:51:35.000000 dendron-0.1.5/src/dendron/actions/simple_action.py
--rw-r--r--   0 richard   (1000) richard   (1000)      768 2024-02-20 06:18:52.000000 dendron-0.1.5/src/dendron/basic_types.py
--rw-r--r--   0 richard   (1000) richard   (1000)     7803 2024-01-30 21:21:57.000000 dendron-0.1.5/src/dendron/behavior_tree.py
--rw-r--r--   0 richard   (1000) richard   (1000)    13978 2024-02-21 15:39:55.000000 dendron-0.1.5/src/dendron/behavior_tree_factory.py
--rw-r--r--   0 richard   (1000) richard   (1000)     6551 2024-01-29 23:24:00.000000 dendron-0.1.5/src/dendron/blackboard.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1978 2024-01-30 20:07:23.000000 dendron-0.1.5/src/dendron/condition_node.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/src/dendron/conditions/
--rw-r--r--   0 richard   (1000) richard   (1000)      251 2024-02-20 05:46:13.000000 dendron-0.1.5/src/dendron/conditions/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     9653 2024-04-05 03:15:34.000000 dendron-0.1.5/src/dendron/conditions/completion_condition.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1604 2024-01-31 17:14:20.000000 dendron-0.1.5/src/dendron/conditions/conjunction_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1607 2024-01-31 17:13:25.000000 dendron-0.1.5/src/dendron/conditions/disjunction_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)      519 2024-01-31 17:14:46.000000 dendron-0.1.5/src/dendron/conditions/goal_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)      978 2024-02-20 06:18:57.000000 dendron-0.1.5/src/dendron/conditions/simple_condition.py
--rw-r--r--   0 richard   (1000) richard   (1000)     4720 2024-01-30 19:50:57.000000 dendron-0.1.5/src/dendron/control_node.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/src/dendron/controls/
--rw-r--r--   0 richard   (1000) richard   (1000)       61 2024-02-20 19:41:41.000000 dendron-0.1.5/src/dendron/controls/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     3303 2024-02-20 05:23:43.000000 dendron-0.1.5/src/dendron/controls/fallback.py
--rw-r--r--   0 richard   (1000) richard   (1000)     3186 2024-02-20 05:47:14.000000 dendron-0.1.5/src/dendron/controls/sequence.py
--rw-r--r--   0 richard   (1000) richard   (1000)     3536 2024-01-30 19:24:27.000000 dendron-0.1.5/src/dendron/decorator_node.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/src/dendron/decorators/
--rw-r--r--   0 richard   (1000) richard   (1000)      271 2024-02-20 06:24:51.000000 dendron-0.1.5/src/dendron/decorators/__init__.py
--rw-r--r--   0 richard   (1000) richard   (1000)     2130 2024-02-20 06:24:11.000000 dendron-0.1.5/src/dendron/decorators/blackboard_history.py
--rw-r--r--   0 richard   (1000) richard   (1000)      982 2024-02-20 06:24:17.000000 dendron-0.1.5/src/dendron/decorators/force_failure.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1009 2024-02-20 06:24:22.000000 dendron-0.1.5/src/dendron/decorators/force_success.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1539 2024-02-20 06:24:27.000000 dendron-0.1.5/src/dendron/decorators/inverter.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1877 2024-02-20 06:24:33.000000 dendron-0.1.5/src/dendron/decorators/repeat.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1850 2024-02-20 06:24:38.000000 dendron-0.1.5/src/dendron/decorators/retry.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1471 2024-02-20 06:24:43.000000 dendron-0.1.5/src/dendron/decorators/run_once.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1780 2024-02-20 06:24:47.000000 dendron-0.1.5/src/dendron/decorators/timeout.py
--rw-r--r--   0 richard   (1000) richard   (1000)     6557 2024-02-21 00:52:52.000000 dendron-0.1.5/src/dendron/tree_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)     4148 2024-01-24 22:59:31.000000 dendron-0.1.5/src/dendron/xml_utilities.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/src/dendron.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     2704 2024-04-05 03:32:01.000000 dendron-0.1.5/src/dendron.egg-info/PKG-INFO
--rw-r--r--   0 richard   (1000) richard   (1000)     1773 2024-04-05 03:32:01.000000 dendron-0.1.5/src/dendron.egg-info/SOURCES.txt
--rw-r--r--   0 richard   (1000) richard   (1000)        1 2024-04-05 03:32:01.000000 dendron-0.1.5/src/dendron.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      134 2024-04-05 03:32:01.000000 dendron-0.1.5/src/dendron.egg-info/requires.txt
--rw-r--r--   0 richard   (1000) richard   (1000)        8 2024-04-05 03:32:01.000000 dendron-0.1.5/src/dendron.egg-info/top_level.txt
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-04-05 03:32:01.682918 dendron-0.1.5/tests/
--rw-r--r--   0 richard   (1000) richard   (1000)      645 2023-12-08 23:55:17.000000 dendron-0.1.5/tests/test_behavior_tree_factory.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1022 2023-12-01 00:21:57.000000 dendron-0.1.5/tests/test_blackboard.py
--rw-r--r--   0 richard   (1000) richard   (1000)      533 2023-12-04 19:47:31.000000 dendron-0.1.5/tests/test_derived_action_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)      375 2024-02-11 22:04:25.000000 dendron-0.1.5/tests/test_fallback_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)      530 2024-02-11 22:05:06.000000 dendron-0.1.5/tests/test_inverter_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)      758 2023-12-30 03:05:43.000000 dendron-0.1.5/tests/test_logging.py
--rw-r--r--   0 richard   (1000) richard   (1000)      384 2024-02-11 22:05:25.000000 dendron-0.1.5/tests/test_sequence_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)     1475 2024-02-11 22:55:52.000000 dendron-0.1.5/tests/test_simple_action_node.py
--rw-r--r--   0 richard   (1000) richard   (1000)     2141 2023-12-07 23:43:34.000000 dendron-0.1.5/tests/test_xml_utilities.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.066385 dendron-0.1.6/
+-rw-r--r--   0 richard   (1000) richard   (1000)     1504 2024-02-06 04:46:44.000000 dendron-0.1.6/LICENSE
+-rw-r--r--   0 richard   (1000) richard   (1000)     3954 2024-05-12 23:16:52.066385 dendron-0.1.6/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)     3207 2024-04-16 16:50:56.000000 dendron-0.1.6/README.md
+-rw-r--r--   0 richard   (1000) richard   (1000)      888 2024-05-12 23:16:47.000000 dendron-0.1.6/pyproject.toml
+-rw-r--r--   0 richard   (1000) richard   (1000)       65 2024-05-12 23:16:52.066385 dendron-0.1.6/setup.cfg
+-rw-r--r--   0 richard   (1000) richard   (1000)      316 2024-05-12 23:16:49.000000 dendron-0.1.6/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.062385 dendron-0.1.6/src/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.062385 dendron-0.1.6/src/dendron/
+-rw-r--r--   0 richard   (1000) richard   (1000)      565 2024-05-12 23:16:45.000000 dendron-0.1.6/src/dendron/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1929 2024-01-30 20:13:57.000000 dendron-0.1.6/src/dendron/action_node.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.062385 dendron-0.1.6/src/dendron/actions/
+-rw-r--r--   0 richard   (1000) richard   (1000)      359 2024-02-20 05:31:46.000000 dendron-0.1.6/src/dendron/actions/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      446 2024-02-11 21:58:50.000000 dendron-0.1.6/src/dendron/actions/always_failure.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      485 2024-02-11 21:58:56.000000 dendron-0.1.6/src/dendron/actions/always_success.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1805 2024-02-11 22:46:52.000000 dendron-0.1.6/src/dendron/actions/async_action.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    10246 2024-05-12 22:46:19.000000 dendron-0.1.6/src/dendron/actions/causal_lm_action.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11153 2024-05-12 22:46:40.000000 dendron-0.1.6/src/dendron/actions/image_lm_action.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     3856 2024-02-11 22:50:10.000000 dendron-0.1.6/src/dendron/actions/pipeline_action.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      803 2024-02-11 22:51:35.000000 dendron-0.1.6/src/dendron/actions/simple_action.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      768 2024-02-20 06:18:52.000000 dendron-0.1.6/src/dendron/basic_types.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     7803 2024-01-30 21:21:57.000000 dendron-0.1.6/src/dendron/behavior_tree.py
+-rw-r--r--   0 richard   (1000) richard   (1000)    13978 2024-02-21 15:39:55.000000 dendron-0.1.6/src/dendron/behavior_tree_factory.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     6551 2024-01-29 23:24:00.000000 dendron-0.1.6/src/dendron/blackboard.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1978 2024-01-30 20:07:23.000000 dendron-0.1.6/src/dendron/condition_node.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.062385 dendron-0.1.6/src/dendron/conditions/
+-rw-r--r--   0 richard   (1000) richard   (1000)      251 2024-02-20 05:46:13.000000 dendron-0.1.6/src/dendron/conditions/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     9668 2024-05-12 22:46:55.000000 dendron-0.1.6/src/dendron/conditions/completion_condition.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1604 2024-01-31 17:14:20.000000 dendron-0.1.6/src/dendron/conditions/conjunction_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1607 2024-01-31 17:13:25.000000 dendron-0.1.6/src/dendron/conditions/disjunction_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      519 2024-01-31 17:14:46.000000 dendron-0.1.6/src/dendron/conditions/goal_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      978 2024-02-20 06:18:57.000000 dendron-0.1.6/src/dendron/conditions/simple_condition.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     4720 2024-01-30 19:50:57.000000 dendron-0.1.6/src/dendron/control_node.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.062385 dendron-0.1.6/src/dendron/controls/
+-rw-r--r--   0 richard   (1000) richard   (1000)       61 2024-02-20 19:41:41.000000 dendron-0.1.6/src/dendron/controls/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     3303 2024-02-20 05:23:43.000000 dendron-0.1.6/src/dendron/controls/fallback.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     3186 2024-02-20 05:47:14.000000 dendron-0.1.6/src/dendron/controls/sequence.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     3536 2024-01-30 19:24:27.000000 dendron-0.1.6/src/dendron/decorator_node.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.066385 dendron-0.1.6/src/dendron/decorators/
+-rw-r--r--   0 richard   (1000) richard   (1000)      271 2024-02-20 06:24:51.000000 dendron-0.1.6/src/dendron/decorators/__init__.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     2130 2024-02-20 06:24:11.000000 dendron-0.1.6/src/dendron/decorators/blackboard_history.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      982 2024-02-20 06:24:17.000000 dendron-0.1.6/src/dendron/decorators/force_failure.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1009 2024-02-20 06:24:22.000000 dendron-0.1.6/src/dendron/decorators/force_success.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1539 2024-02-20 06:24:27.000000 dendron-0.1.6/src/dendron/decorators/inverter.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1877 2024-02-20 06:24:33.000000 dendron-0.1.6/src/dendron/decorators/repeat.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1850 2024-02-20 06:24:38.000000 dendron-0.1.6/src/dendron/decorators/retry.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1471 2024-02-20 06:24:43.000000 dendron-0.1.6/src/dendron/decorators/run_once.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1780 2024-02-20 06:24:47.000000 dendron-0.1.6/src/dendron/decorators/timeout.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     6557 2024-02-21 00:52:52.000000 dendron-0.1.6/src/dendron/tree_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     4148 2024-01-24 22:59:31.000000 dendron-0.1.6/src/dendron/xml_utilities.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.066385 dendron-0.1.6/src/dendron.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     3954 2024-05-12 23:16:52.000000 dendron-0.1.6/src/dendron.egg-info/PKG-INFO
+-rw-r--r--   0 richard   (1000) richard   (1000)     1773 2024-05-12 23:16:52.000000 dendron-0.1.6/src/dendron.egg-info/SOURCES.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)        1 2024-05-12 23:16:52.000000 dendron-0.1.6/src/dendron.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      134 2024-05-12 23:16:52.000000 dendron-0.1.6/src/dendron.egg-info/requires.txt
+-rw-r--r--   0 richard   (1000) richard   (1000)        8 2024-05-12 23:16:52.000000 dendron-0.1.6/src/dendron.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-12 23:16:52.066385 dendron-0.1.6/tests/
+-rw-r--r--   0 richard   (1000) richard   (1000)      645 2023-12-08 23:55:17.000000 dendron-0.1.6/tests/test_behavior_tree_factory.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1022 2023-12-01 00:21:57.000000 dendron-0.1.6/tests/test_blackboard.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      533 2023-12-04 19:47:31.000000 dendron-0.1.6/tests/test_derived_action_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      375 2024-02-11 22:04:25.000000 dendron-0.1.6/tests/test_fallback_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      530 2024-02-11 22:05:06.000000 dendron-0.1.6/tests/test_inverter_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      758 2023-12-30 03:05:43.000000 dendron-0.1.6/tests/test_logging.py
+-rw-r--r--   0 richard   (1000) richard   (1000)      384 2024-02-11 22:05:25.000000 dendron-0.1.6/tests/test_sequence_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     1475 2024-02-11 22:55:52.000000 dendron-0.1.6/tests/test_simple_action_node.py
+-rw-r--r--   0 richard   (1000) richard   (1000)     2141 2023-12-07 23:43:34.000000 dendron-0.1.6/tests/test_xml_utilities.py
```

### Comparing `dendron-0.1.5/LICENSE` & `dendron-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/pyproject.toml` & `dendron-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dendron"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name = "Richard Kelley" },
 ]
 license = {text = "BSD License"}
 description = "A library for working with LLMs and behavior trees."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `dendron-0.1.5/src/dendron/__init__.py` & `dendron-0.1.6/src/dendron/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Dendron is a library for building behavior trees that use
 large language models and vision language models.
 """
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 __author__ = "Richard Kelley"
 
 from .action_node import ActionNode
 from .basic_types import NodeType, NodeStatus
 from .behavior_tree import BehaviorTree 
 from .behavior_tree_factory import BehaviorTreeFactory
 from .blackboard import Blackboard, BlackboardEntryMetadata
```

### Comparing `dendron-0.1.5/src/dendron/action_node.py` & `dendron-0.1.6/src/dendron/action_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/actions/async_action.py` & `dendron-0.1.6/src/dendron/actions/async_action.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/actions/causal_lm_action.py` & `dendron-0.1.6/src/dendron/actions/causal_lm_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,15 +145,15 @@
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case True, False:
                 self.bnb_cfg.load_in_4bit = True
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case False, True:
                 self.bnb_cfg.load_in_8bit = True
             case False, False:
-                pass
+                self.bnb_cfg = None
 
         if cfg.use_flash_attn_2:
             self.attn_implementation = "flash_attention_2"
         else:
             self.attn_implementation = "sdpa"
 
         if cfg.auto_load:
```

### Comparing `dendron-0.1.5/src/dendron/actions/image_lm_action.py` & `dendron-0.1.6/src/dendron/actions/image_lm_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case True, False:
                 self.bnb_cfg.load_in_4bit = True
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case False, True:
                 self.bnb_cfg.load_in_8bit = True
             case False, False:
-                pass
+                self.bnb_cfg = None
                 
         if cfg.use_flash_attn_2:
             self.attn_implementation = "flash_attention_2"
         else:
             self.attn_implementation = "sdpa"
 
         if cfg.auto_load:
```

### Comparing `dendron-0.1.5/src/dendron/actions/pipeline_action.py` & `dendron-0.1.6/src/dendron/actions/pipeline_action.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/actions/simple_action.py` & `dendron-0.1.6/src/dendron/actions/simple_action.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/basic_types.py` & `dendron-0.1.6/src/dendron/basic_types.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/behavior_tree.py` & `dendron-0.1.6/src/dendron/behavior_tree.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/behavior_tree_factory.py` & `dendron-0.1.6/src/dendron/behavior_tree_factory.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/blackboard.py` & `dendron-0.1.6/src/dendron/blackboard.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/condition_node.py` & `dendron-0.1.6/src/dendron/condition_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/conditions/completion_condition.py` & `dendron-0.1.6/src/dendron/conditions/completion_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case True, False:
                 self.bnb_cfg.load_in_4bit = True
                 self.bnb_cfg.bnb_4bit_compute_dtype = cfg.torch_dtype
             case False, True:
                 self.bnb_cfg.load_in_8bit = True
             case False, False:
-                pass
+                self.bnb_cfg = None
                 
         if cfg.use_flash_attn_2:
             self.attn_implementation = "flash_attention_2"
         else:
             self.attn_implementation = "sdpa"
 
         if cfg.auto_load:
```

### Comparing `dendron-0.1.5/src/dendron/conditions/conjunction_node.py` & `dendron-0.1.6/src/dendron/conditions/conjunction_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/conditions/disjunction_node.py` & `dendron-0.1.6/src/dendron/conditions/disjunction_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/conditions/goal_node.py` & `dendron-0.1.6/src/dendron/conditions/goal_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/conditions/simple_condition.py` & `dendron-0.1.6/src/dendron/conditions/simple_condition.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/control_node.py` & `dendron-0.1.6/src/dendron/control_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/controls/fallback.py` & `dendron-0.1.6/src/dendron/controls/fallback.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/controls/sequence.py` & `dendron-0.1.6/src/dendron/controls/sequence.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorator_node.py` & `dendron-0.1.6/src/dendron/decorator_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/blackboard_history.py` & `dendron-0.1.6/src/dendron/decorators/blackboard_history.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/force_failure.py` & `dendron-0.1.6/src/dendron/decorators/force_failure.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/force_success.py` & `dendron-0.1.6/src/dendron/decorators/force_success.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/inverter.py` & `dendron-0.1.6/src/dendron/decorators/inverter.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/repeat.py` & `dendron-0.1.6/src/dendron/decorators/repeat.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/retry.py` & `dendron-0.1.6/src/dendron/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/run_once.py` & `dendron-0.1.6/src/dendron/decorators/run_once.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/decorators/timeout.py` & `dendron-0.1.6/src/dendron/decorators/timeout.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/tree_node.py` & `dendron-0.1.6/src/dendron/tree_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron/xml_utilities.py` & `dendron-0.1.6/src/dendron/xml_utilities.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/src/dendron.egg-info/SOURCES.txt` & `dendron-0.1.6/src/dendron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_behavior_tree_factory.py` & `dendron-0.1.6/tests/test_behavior_tree_factory.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_blackboard.py` & `dendron-0.1.6/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_derived_action_node.py` & `dendron-0.1.6/tests/test_derived_action_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_inverter_node.py` & `dendron-0.1.6/tests/test_inverter_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_logging.py` & `dendron-0.1.6/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_simple_action_node.py` & `dendron-0.1.6/tests/test_simple_action_node.py`

 * *Files identical despite different names*

### Comparing `dendron-0.1.5/tests/test_xml_utilities.py` & `dendron-0.1.6/tests/test_xml_utilities.py`

 * *Files identical despite different names*

