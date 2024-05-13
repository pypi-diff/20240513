# Comparing `tmp/pz_rail_bpz-0.1.3.tar.gz` & `tmp/pz_rail_bpz-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_bpz-0.1.3.tar", last modified: Wed May  8 20:28:07 2024, max compression
+gzip compressed data, was "pz_rail_bpz-1.0.0.tar", last modified: Mon May 13 19:54:11 2024, max compression
```

## Comparing `pz_rail_bpz-0.1.3.tar` & `pz_rail_bpz-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.777781 pz_rail_bpz-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    33376 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/BPZ_lite_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22592 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/BPZ_lite_with_custom_SEDs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   460800 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/nonphysical_dc2_templates.tar
--rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/test_dc2_train_customtemp_broadttypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/examples/test_dc2_training_9816_broadtypes.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/bpz/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/bpz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 20:28:07.000000 pz_rail_bpz-0.1.3/src/rail/bpz/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/bpz/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    26660 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/estimation/algos/bpz_lite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.773781 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/test_bpz.columns
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 20:28:07.781782 pz_rail_bpz-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/tests/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-08 20:28:00.000000 pz_rail_bpz-0.1.3/tests/validation_10gal.pq
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.862935 pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.862935 pz_rail_bpz-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.862935 pz_rail_bpz-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    33376 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22592 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   460800 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/examples/nonphysical_dc2_templates.tar
+-rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/examples/test_dc2_train_customtemp_broadttypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    83848 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/examples/test_dc2_training_9816_broadtypes.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/src/rail/bpz/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/src/rail/bpz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:54:11.000000 pz_rail_bpz-1.0.0/src/rail/bpz/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/src/rail/bpz/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    26660 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/src/rail/estimation/algos/bpz_lite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.858935 pz_rail_bpz-1.0.0/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/src/rail/examples_data/estimation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:54:11.866935 pz_rail_bpz-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/tests/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-13 19:54:05.000000 pz_rail_bpz-1.0.0/tests/validation_10gal.pq
```

### Comparing `pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_bpz-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/pull_request_template.md` & `pz_rail_bpz-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/workflows/linting.yml` & `pz_rail_bpz-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_bpz-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/workflows/smoke-test.yml` & `pz_rail_bpz-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_bpz-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.gitignore` & `pz_rail_bpz-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.pre-commit-config.yaml` & `pz_rail_bpz-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/.prepare_project.sh` & `pz_rail_bpz-1.0.0/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/LICENSE` & `pz_rail_bpz-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/PKG-INFO` & `pz_rail_bpz-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.1.3
+Version: 1.0.0
 Author-email: LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_bpz-0.1.3/README.md` & `pz_rail_bpz-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/examples/BPZ_lite_demo.ipynb` & `pz_rail_bpz-1.0.0/examples/BPZ_lite_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/examples/BPZ_lite_with_custom_SEDs.ipynb` & `pz_rail_bpz-1.0.0/examples/BPZ_lite_with_custom_SEDs.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/examples/nonphysical_dc2_templates.tar` & `pz_rail_bpz-1.0.0/examples/nonphysical_dc2_templates.tar`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/examples/test_dc2_train_customtemp_broadttypes.hdf5` & `pz_rail_bpz-1.0.0/examples/test_dc2_train_customtemp_broadttypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/examples/test_dc2_training_9816_broadtypes.hdf5` & `pz_rail_bpz-1.0.0/examples/test_dc2_training_9816_broadtypes.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/pyproject.toml` & `pz_rail_bpz-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/PKG-INFO` & `pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-bpz
-Version: 0.1.3
+Version: 1.0.0
 Author-email: LSST DESC PZ WG <samuel.j.schmidt@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_bpz-0.1.3/src/pz_rail_bpz.egg-info/SOURCES.txt` & `pz_rail_bpz-1.0.0/src/pz_rail_bpz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/src/rail/estimation/algos/bpz_lite.py` & `pz_rail_bpz-1.0.0/src/rail/estimation/algos/bpz_lite.py`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/src/rail/examples_data/estimation_data/configs/test_bpz.columns` & `pz_rail_bpz-1.0.0/src/rail/examples_data/estimation_data/configs/test_bpz.columns`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/tests/test_algos.py` & `pz_rail_bpz-1.0.0/tests/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz_rail_bpz-0.1.3/tests/validation_10gal.pq` & `pz_rail_bpz-1.0.0/tests/validation_10gal.pq`

 * *Files identical despite different names*

