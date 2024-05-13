# Comparing `tmp/agent_evaluation-0.1.0.tar.gz` & `tmp/agent_evaluation-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_evaluation-0.1.0.tar", last modified: Fri May  3 22:25:06 2024, max compression
+gzip compressed data, was "agent_evaluation-0.2.0.tar", last modified: Mon May 13 21:14:24 2024, max compression
```

## Comparing `agent_evaluation-0.1.0.tar` & `agent_evaluation-0.2.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.504644 agent_evaluation-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-03 22:25:06.504644 agent_evaluation-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-03 22:25:06.504644 agent_evaluation-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.496644 agent_evaluation-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.504644 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 22:25:06.000000 agent_evaluation-0.1.0/src/agent_evaluation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/base_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/model_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/evaluators/evaluator_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/runner/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/target_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/targets/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/base_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_agent/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_agent/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_knowledge_base/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_knowledge_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/bedrock_knowledge_base/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/boto3_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/targets/q_business/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/q_business/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/q_business/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/targets/sagemaker_endpoint/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/sagemaker_endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/sagemaker_endpoint/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/targets/target_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.496644 agent_evaluation-0.1.0/src/agenteval/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.496644 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/generate_evaluation.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/generate_initial_prompt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/generate_test_status.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/generate_user_response.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_evaluation.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_initial_prompt.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_test_status.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_user_response.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.500644 agent_evaluation-0.1.0/src/agenteval/templates/summary/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/templates/summary/agenteval_summary.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 22:25:06.504644 agent_evaluation-0.1.0/src/agenteval/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/utils/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-03 22:24:58.000000 agent_evaluation-0.1.0/src/agenteval/utils/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.059161 agent_evaluation-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3740 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 21:14:24.000000 agent_evaluation-0.2.0/src/agent_evaluation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/model_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/evaluators/evaluator_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/runner/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/target_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/targets/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/base_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_agent/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_knowledge_base/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_knowledge_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/bedrock_knowledge_base/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/boto3_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.063161 agent_evaluation-0.2.0/src/agenteval/targets/q_business/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/q_business/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/q_business/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agenteval/targets/sagemaker_endpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/sagemaker_endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/sagemaker_endpoint/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/targets/target_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.059161 agent_evaluation-0.2.0/src/agenteval/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.059161 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/generate_evaluation.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/generate_initial_prompt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/generate_test_status.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/generate_user_response.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_evaluation.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_initial_prompt.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_test_status.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_user_response.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agenteval/templates/summary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/templates/summary/agenteval_summary.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:14:24.067161 agent_evaluation-0.2.0/src/agenteval/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/utils/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 21:14:15.000000 agent_evaluation-0.2.0/src/agenteval/utils/imports.py
```

### Comparing `agent_evaluation-0.1.0/LICENSE` & `agent_evaluation-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/PKG-INFO` & `agent_evaluation-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agent-evaluation
-Version: 0.1.0
+Version: 0.2.0
 Summary: A generative AI-powered framework for testing virtual agents.
-Home-page: https://github.com/awslabs/agent-evaluation
+Home-page: https://awslabs.github.io/agent-evaluation/
 Author: Amazon Web Services
 Author-email: agent-evaluation-oss-core-team@amazon.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Testing
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: agent-evaluation Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: agent-evaluation Version: 0.2.0 Summary: A
 generative AI-powered framework for testing virtual agents. Home-page: https://
-github.com/awslabs/agent-evaluation Author: Amazon Web Services Author-email:
+awslabs.github.io/agent-evaluation/ Author: Amazon Web Services Author-email:
 agent-evaluation-oss-core-team@amazon.com License: Apache 2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities Classifier: Topic :: Software Development ::
 Testing Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `agent_evaluation-0.1.0/README.md` & `agent_evaluation-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/setup.py` & `agent_evaluation-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from distutils.core import setup
 
 from setuptools import find_packages
 
 DIST_NAME = "agent-evaluation"
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 DESCRIPTION = "A generative AI-powered framework for testing virtual agents."
 AUTHOR = "Amazon Web Services"
 EMAIL = "agent-evaluation-oss-core-team@amazon.com"
-URL = "https://github.com/awslabs/agent-evaluation"
+URL = "https://awslabs.github.io/agent-evaluation/"
 PACKAGE_DIR = "src"
 REQUIRES_PYTHON = ">=3.9"
 PACKAGE_DATA = {
     "": [
         "templates/**/*",
     ],
 }
```

### Comparing `agent_evaluation-0.1.0/src/agent_evaluation.egg-info/PKG-INFO` & `agent_evaluation-0.2.0/src/agent_evaluation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: agent-evaluation
-Version: 0.1.0
+Version: 0.2.0
 Summary: A generative AI-powered framework for testing virtual agents.
-Home-page: https://github.com/awslabs/agent-evaluation
+Home-page: https://awslabs.github.io/agent-evaluation/
 Author: Amazon Web Services
 Author-email: agent-evaluation-oss-core-team@amazon.com
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Testing
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: agent-evaluation Version: 0.1.0 Summary: A
+Metadata-Version: 2.1 Name: agent-evaluation Version: 0.2.0 Summary: A
 generative AI-powered framework for testing virtual agents. Home-page: https://
-github.com/awslabs/agent-evaluation Author: Amazon Web Services Author-email:
+awslabs.github.io/agent-evaluation/ Author: Amazon Web Services Author-email:
 agent-evaluation-oss-core-team@amazon.com License: Apache 2.0 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities Classifier: Topic :: Software Development ::
 Testing Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

### Comparing `agent_evaluation-0.1.0/src/agent_evaluation.egg-info/SOURCES.txt` & `agent_evaluation-0.2.0/src/agent_evaluation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/__init__.py` & `agent_evaluation-0.2.0/src/agenteval/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
-__version__ = "0.1.0"
+from importlib.metadata import version
 
 import logging
 import os
 
 from jinja2 import Environment, PackageLoader, select_autoescape
 from rich.logging import RichHandler
 
 from .hook import Hook
+from .target_response import TargetResponse
+
+__all__ = ["Hook", "TargetResponse"]
+__version__ = version("agent-evaluation")
 
-__all__ = ["Hook"]
 
 _LOG_LEVEL_ENV = "LOG_LEVEL"
 
 
 def configure_logger():
     # supress logs from botocore
     logging.getLogger("botocore").setLevel(logging.CRITICAL)
```

### Comparing `agent_evaluation-0.1.0/src/agenteval/cli.py` & `agent_evaluation-0.2.0/src/agenteval/cli.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/conversation.py` & `agent_evaluation-0.2.0/src/agenteval/conversation.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/evaluators/base_evaluator.py` & `agent_evaluation-0.2.0/src/agenteval/evaluators/base_evaluator.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/evaluator.py` & `agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/evaluator.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/evaluators/claude_3/model_configs.py` & `agent_evaluation-0.2.0/src/agenteval/evaluators/claude_3/model_configs.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/evaluators/evaluator_factory.py` & `agent_evaluation-0.2.0/src/agenteval/evaluators/evaluator_factory.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/hook.py` & `agent_evaluation-0.2.0/src/agenteval/hook.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/plan.py` & `agent_evaluation-0.2.0/src/agenteval/plan.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/runner/runner.py` & `agent_evaluation-0.2.0/src/agenteval/runner/runner.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/runner/summary.py` & `agent_evaluation-0.2.0/src/agenteval/runner/summary.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/base_target.py` & `agent_evaluation-0.2.0/src/agenteval/targets/base_target.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 
-from agenteval.target_response import TargetResponse
+from agenteval import TargetResponse
 
 
 class BaseTarget(ABC):
     """The `BaseTarget` abstract base class defines the common interface for target
     classes.
     """
```

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/bedrock_agent/target.py` & `agent_evaluation-0.2.0/src/agenteval/targets/bedrock_agent/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 
-from agenteval.target_response import TargetResponse
+from agenteval import TargetResponse
 from agenteval.targets import Boto3Target
 
 _SERVICE_NAME = "bedrock-agent-runtime"
 
 
 class BedrockAgentTarget(Boto3Target):
     def __init__(self, bedrock_agent_id: str, bedrock_agent_alias_id: str, **kwargs):
```

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/bedrock_knowledge_base/target.py` & `agent_evaluation-0.2.0/src/agenteval/targets/bedrock_knowledge_base/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agenteval.target_response import TargetResponse
+from agenteval import TargetResponse
 from agenteval.targets import Boto3Target
 
 _SERVICE_NAME = "bedrock-agent-runtime"
 
 
 class BedrockKnowledgeBaseTarget(Boto3Target):
     def __init__(self, knowledge_base_id: str, model_id: str, **kwargs):
```

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/boto3_target.py` & `agent_evaluation-0.2.0/src/agenteval/targets/boto3_target.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/sagemaker_endpoint/target.py` & `agent_evaluation-0.2.0/src/agenteval/targets/sagemaker_endpoint/target.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from typing import Optional
 
 from jsonpath_ng import parse
 
-from agenteval.target_response import TargetResponse
+from agenteval import TargetResponse
 from agenteval.targets import Boto3Target
 
 _SERVICE_NAME = "sagemaker-runtime"
 _CONTENT_TYPE = "application/json"
 _ACCEPT = "application/json"
```

### Comparing `agent_evaluation-0.1.0/src/agenteval/targets/target_factory.py` & `agent_evaluation-0.2.0/src/agenteval/targets/target_factory.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_evaluation.jinja` & `agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_evaluation.jinja`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_initial_prompt.jinja` & `agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_initial_prompt.jinja`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_test_status.jinja` & `agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_test_status.jinja`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/templates/evaluators/claude_3/system/generate_user_response.jinja` & `agent_evaluation-0.2.0/src/agenteval/templates/evaluators/claude_3/system/generate_user_response.jinja`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/templates/summary/agenteval_summary.md.jinja` & `agent_evaluation-0.2.0/src/agenteval/templates/summary/agenteval_summary.md.jinja`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/test.py` & `agent_evaluation-0.2.0/src/agenteval/test.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/test_result.py` & `agent_evaluation-0.2.0/src/agenteval/test_result.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/trace.py` & `agent_evaluation-0.2.0/src/agenteval/trace.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/utils/aws.py` & `agent_evaluation-0.2.0/src/agenteval/utils/aws.py`

 * *Files identical despite different names*

### Comparing `agent_evaluation-0.1.0/src/agenteval/utils/imports.py` & `agent_evaluation-0.2.0/src/agenteval/utils/imports.py`

 * *Files identical despite different names*

