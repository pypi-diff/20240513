# Comparing `tmp/pz_rail_pzflow-0.0.4.tar.gz` & `tmp/pz_rail_pzflow-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_pzflow-0.0.4.tar", last modified: Wed May  8 20:28:56 2024, max compression
+gzip compressed data, was "pz_rail_pzflow-1.0.0.tar", last modified: Mon May 13 20:38:33 2024, max compression
```

## Comparing `pz_rail_pzflow-0.0.4.tar` & `pz_rail_pzflow-1.0.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:28:56.283645 pz_rail_pzflow-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:28:56.000000 pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/creation/engines/flowEngine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/estimation/algos/pzflow_nf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/pzflow/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/pzflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:28:55.000000 pz_rail_pzflow-0.0.4/src/rail/pzflow/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/src/rail/tools/flow_handle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.275645 pz_rail_pzflow-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:56.279645 pz_rail_pzflow-0.0.4/tests/pzflow/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/tests/pzflow/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-08 20:28:49.000000 pz_rail_pzflow-0.0.4/tests/pzflow/test_flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.012484 pz_rail_pzflow-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-13 20:38:33.012484 pz_rail_pzflow-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:38:33.012484 pz_rail_pzflow-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.004484 pz_rail_pzflow-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.012484 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-13 20:38:32.000000 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-13 20:38:33.000000 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:38:32.000000 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-13 20:38:32.000000 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:38:32.000000 pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.004484 pz_rail_pzflow-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.004484 pz_rail_pzflow-1.0.0/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/src/rail/creation/engines/flowEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.004484 pz_rail_pzflow-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    10837 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/src/rail/estimation/algos/pzflow_nf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/src/rail/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/src/rail/pzflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:38:32.000000 pz_rail_pzflow-1.0.0/src/rail/pzflow/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.008484 pz_rail_pzflow-1.0.0/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/src/rail/tools/flow_handle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.004484 pz_rail_pzflow-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:33.012484 pz_rail_pzflow-1.0.0/tests/pzflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/tests/pzflow/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-05-13 20:38:25.000000 pz_rail_pzflow-1.0.0/tests/pzflow/test_flowEngine.py
```

### Comparing `pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_pzflow-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/pull_request_template.md` & `pz_rail_pzflow-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/workflows/linting.yml` & `pz_rail_pzflow-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/workflows/publish-to-pypi.yml` & `pz_rail_pzflow-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/workflows/smoke-test.yml` & `pz_rail_pzflow-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.github/workflows/testing-and-coverage.yml` & `pz_rail_pzflow-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.gitignore` & `pz_rail_pzflow-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/.pre-commit-config.yaml` & `pz_rail_pzflow-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/LICENSE` & `pz_rail_pzflow-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/PKG-INFO` & `pz_rail_pzflow-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pzflow
-Version: 0.0.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_pzflow-0.0.4/README.md` & `pz_rail_pzflow-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/pyproject.toml` & `pz_rail_pzflow-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/PKG-INFO` & `pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pzflow
-Version: 0.0.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_pzflow-0.0.4/src/pz_rail_pzflow.egg-info/SOURCES.txt` & `pz_rail_pzflow-1.0.0/src/pz_rail_pzflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/src/rail/creation/engines/flowEngine.py` & `pz_rail_pzflow-1.0.0/src/rail/creation/engines/flowEngine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/src/rail/estimation/algos/pzflow_nf.py` & `pz_rail_pzflow-1.0.0/src/rail/estimation/algos/pzflow_nf.py`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/src/rail/tools/flow_handle.py` & `pz_rail_pzflow-1.0.0/src/rail/tools/flow_handle.py`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/tests/pzflow/test_algos.py` & `pz_rail_pzflow-1.0.0/tests/pzflow/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz_rail_pzflow-0.0.4/tests/pzflow/test_flowEngine.py` & `pz_rail_pzflow-1.0.0/tests/pzflow/test_flowEngine.py`

 * *Files identical despite different names*

