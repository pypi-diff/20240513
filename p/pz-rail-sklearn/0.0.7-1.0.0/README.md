# Comparing `tmp/pz_rail_sklearn-0.0.7.tar.gz` & `tmp/pz_rail_sklearn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_sklearn-0.0.7.tar", last modified: Wed May  8 15:55:31 2024, max compression
+gzip compressed data, was "pz_rail_sklearn-1.0.0.tar", last modified: Mon May 13 20:38:54 2024, max compression
```

## Comparing `pz_rail_sklearn-0.0.7.tar` & `pz_rail_sklearn-1.0.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:55:31.866723 pz_rail_sklearn-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/k_nearneigh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12447 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/nz_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/estimation/algos/sklearn_neurnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/src/rail/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/src/rail/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:55:31.000000 pz_rail_sklearn-0.0.7/src/rail/sklearn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.858723 pz_rail_sklearn-0.0.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:55:31.862723 pz_rail_sklearn-0.0.7/tests/sklearn/
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-08 15:55:25.000000 pz_rail_sklearn-0.0.7/tests/sklearn/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.926383 pz_rail_sklearn-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.926383 pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.926383 pz_rail_sklearn-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.922383 pz_rail_sklearn-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.922383 pz_rail_sklearn-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.922383 pz_rail_sklearn-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/src/rail/estimation/algos/k_nearneigh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12447 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/src/rail/estimation/algos/nz_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/src/rail/estimation/algos/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/src/rail/estimation/algos/sklearn_neurnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/src/rail/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/src/rail/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:38:54.000000 pz_rail_sklearn-1.0.0/src/rail/sklearn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.922383 pz_rail_sklearn-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:38:54.930383 pz_rail_sklearn-1.0.0/tests/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-13 20:38:48.000000 pz_rail_sklearn-1.0.0/tests/sklearn/test_algos.py
```

### Comparing `pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_sklearn-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/pull_request_template.md` & `pz_rail_sklearn-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/workflows/linting.yml` & `pz_rail_sklearn-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/workflows/publish-to-pypi.yml` & `pz_rail_sklearn-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/workflows/smoke-test.yml` & `pz_rail_sklearn-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.github/workflows/testing-and-coverage.yml` & `pz_rail_sklearn-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.gitignore` & `pz_rail_sklearn-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/.pre-commit-config.yaml` & `pz_rail_sklearn-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/LICENSE` & `pz_rail_sklearn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/PKG-INFO` & `pz_rail_sklearn-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.7
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_sklearn-0.0.7/README.md` & `pz_rail_sklearn-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/pyproject.toml` & `pz_rail_sklearn-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/PKG-INFO` & `pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-sklearn
-Version: 0.0.7
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_sklearn-0.0.7/src/pz_rail_sklearn.egg-info/SOURCES.txt` & `pz_rail_sklearn-1.0.0/src/pz_rail_sklearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/k_nearneigh.py` & `pz_rail_sklearn-1.0.0/src/rail/estimation/algos/k_nearneigh.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/nz_dir.py` & `pz_rail_sklearn-1.0.0/src/rail/estimation/algos/nz_dir.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/random_forest.py` & `pz_rail_sklearn-1.0.0/src/rail/estimation/algos/random_forest.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/src/rail/estimation/algos/sklearn_neurnet.py` & `pz_rail_sklearn-1.0.0/src/rail/estimation/algos/sklearn_neurnet.py`

 * *Files identical despite different names*

### Comparing `pz_rail_sklearn-0.0.7/tests/sklearn/test_algos.py` & `pz_rail_sklearn-1.0.0/tests/sklearn/test_algos.py`

 * *Files identical despite different names*

