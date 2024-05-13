# Comparing `tmp/pz_rail_flexzboost-0.2.0.tar.gz` & `tmp/pz_rail_flexzboost-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_flexzboost-0.2.0.tar", last modified: Wed May  8 20:29:45 2024, max compression
+gzip compressed data, was "pz_rail_flexzboost-1.0.0.tar", last modified: Mon May 13 20:23:40 2024, max compression
```

## Comparing `pz_rail_flexzboost-0.2.0.tar` & `pz_rail_flexzboost-1.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/archive/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/x_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/archive/x_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.648092 pz_rail_flexzboost-0.2.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/flexzboost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:29:45.000000 pz_rail_flexzboost-0.2.0/src/rail/flexzboost/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:29:45.652093 pz_rail_flexzboost-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-08 20:29:36.000000 pz_rail_flexzboost-0.2.0/tests/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.431437 pz_rail_flexzboost-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.431437 pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.431437 pz_rail_flexzboost-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.431437 pz_rail_flexzboost-1.0.0/archive/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/archive/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/archive/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/archive/x_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/archive/x_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.427437 pz_rail_flexzboost-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.427437 pz_rail_flexzboost-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.427437 pz_rail_flexzboost-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.431437 pz_rail_flexzboost-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    14067 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/src/rail/estimation/algos/flexzboost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/src/rail/flexzboost/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/src/rail/flexzboost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:23:40.000000 pz_rail_flexzboost-1.0.0/src/rail/flexzboost/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:40.435437 pz_rail_flexzboost-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-13 20:23:34.000000 pz_rail_flexzboost-1.0.0/tests/test_algos.py
```

### Comparing `pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_flexzboost-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/pull_request_template.md` & `pz_rail_flexzboost-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/workflows/linting.yml` & `pz_rail_flexzboost-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/workflows/publish-to-pypi.yml` & `pz_rail_flexzboost-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/workflows/smoke-test.yml` & `pz_rail_flexzboost-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.github/workflows/testing-and-coverage.yml` & `pz_rail_flexzboost-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.gitignore` & `pz_rail_flexzboost-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.pre-commit-config.yaml` & `pz_rail_flexzboost-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/.prepare_project.sh` & `pz_rail_flexzboost-1.0.0/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/LICENSE` & `pz_rail_flexzboost-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/PKG-INFO` & `pz_rail_flexzboost-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.2.0
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_flexzboost-0.2.0/README.md` & `pz_rail_flexzboost-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/archive/README.md` & `pz_rail_flexzboost-1.0.0/archive/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/archive/pypi.yaml` & `pz_rail_flexzboost-1.0.0/archive/pypi.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/pyproject.toml` & `pz_rail_flexzboost-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/PKG-INFO` & `pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-flexzboost
-Version: 0.2.0
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_flexzboost-0.2.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt` & `pz_rail_flexzboost-1.0.0/src/pz_rail_flexzboost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/src/rail/estimation/algos/flexzboost.py` & `pz_rail_flexzboost-1.0.0/src/rail/estimation/algos/flexzboost.py`

 * *Files identical despite different names*

### Comparing `pz_rail_flexzboost-0.2.0/tests/test_algos.py` & `pz_rail_flexzboost-1.0.0/tests/test_algos.py`

 * *Files identical despite different names*

