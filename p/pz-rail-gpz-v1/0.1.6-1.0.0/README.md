# Comparing `tmp/pz_rail_gpz_v1-0.1.6.tar.gz` & `tmp/pz_rail_gpz_v1-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_gpz_v1-0.1.6.tar", last modified: Wed May  8 15:50:45 2024, max compression
+gzip compressed data, was "pz_rail_gpz_v1-1.0.0.tar", last modified: Mon May 13 20:37:04 2024, max compression
```

## Comparing `pz_rail_gpz_v1-0.1.6.tar` & `pz_rail_gpz_v1-1.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.341369 pz_rail_gpz_v1-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-08 15:50:45.341369 pz_rail_gpz_v1-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:50:45.341369 pz_rail_gpz_v1-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.333369 pz_rail_gpz_v1-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.341369 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.333369 pz_rail_gpz_v1-0.1.6/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.333369 pz_rail_gpz_v1-0.1.6/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/src/rail/estimation/algos/_gpz_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/src/rail/estimation/algos/gpz.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/src/rail/gpz/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/src/rail/gpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:50:45.000000 pz_rail_gpz_v1-0.1.6/src/rail/gpz/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:50:45.337369 pz_rail_gpz_v1-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-08 15:50:39.000000 pz_rail_gpz_v1-0.1.6/tests/test_gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.036927 pz_rail_gpz_v1-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-13 20:37:04.036927 pz_rail_gpz_v1-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:37:04.036927 pz_rail_gpz_v1-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.028927 pz_rail_gpz_v1-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-13 20:37:04.000000 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 20:37:04.000000 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:37:04.000000 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 20:37:04.000000 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:37:04.000000 pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.028927 pz_rail_gpz_v1-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.028927 pz_rail_gpz_v1-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/src/rail/estimation/algos/_gpz_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/src/rail/estimation/algos/gpz.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/src/rail/gpz/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/src/rail/gpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:37:03.000000 pz_rail_gpz_v1-1.0.0/src/rail/gpz/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:04.032927 pz_rail_gpz_v1-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-13 20:36:58.000000 pz_rail_gpz_v1-1.0.0/tests/test_gpz.py
```

### Comparing `pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_gpz_v1-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/pull_request_template.md` & `pz_rail_gpz_v1-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/workflows/linting.yml` & `pz_rail_gpz_v1-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/workflows/publish-to-pypi.yml` & `pz_rail_gpz_v1-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/workflows/smoke-test.yml` & `pz_rail_gpz_v1-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.github/workflows/testing-and-coverage.yml` & `pz_rail_gpz_v1-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.gitignore` & `pz_rail_gpz_v1-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.pre-commit-config.yaml` & `pz_rail_gpz_v1-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/.prepare_project.sh` & `pz_rail_gpz_v1-1.0.0/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/LICENSE` & `pz_rail_gpz_v1-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/PKG-INFO` & `pz_rail_gpz_v1-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.6
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_gpz_v1-0.1.6/README.md` & `pz_rail_gpz_v1-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/pyproject.toml` & `pz_rail_gpz_v1-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/PKG-INFO` & `pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-gpz-v1
-Version: 0.1.6
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_gpz_v1-0.1.6/src/pz_rail_gpz_v1.egg-info/SOURCES.txt` & `pz_rail_gpz_v1-1.0.0/src/pz_rail_gpz_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/src/rail/estimation/algos/_gpz_util.py` & `pz_rail_gpz_v1-1.0.0/src/rail/estimation/algos/_gpz_util.py`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/src/rail/estimation/algos/gpz.py` & `pz_rail_gpz_v1-1.0.0/src/rail/estimation/algos/gpz.py`

 * *Files identical despite different names*

### Comparing `pz_rail_gpz_v1-0.1.6/tests/test_gpz.py` & `pz_rail_gpz_v1-1.0.0/tests/test_gpz.py`

 * *Files identical despite different names*

