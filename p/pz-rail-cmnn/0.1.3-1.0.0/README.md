# Comparing `tmp/pz-rail-cmnn-0.1.3.tar.gz` & `tmp/pz_rail_cmnn-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-cmnn-0.1.3.tar", last modified: Tue Oct 31 21:08:25 2023, max compression
+gzip compressed data, was "pz_rail_cmnn-1.0.0.tar", last modified: Mon May 13 20:01:30 2024, max compression
```

## Comparing `pz-rail-cmnn-0.1.3.tar` & `pz_rail_cmnn-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.691927 pz-rail-cmnn-0.1.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.691927 pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.695927 pz-rail-cmnn-0.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.695927 pz-rail-cmnn-0.1.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    16913 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/examples/CMNN_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.687927 pz-rail-cmnn-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.695927 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.687927 pz-rail-cmnn-0.1.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/src/rail/cmnn/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/src/rail/cmnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-31 21:08:25.000000 pz-rail-cmnn-0.1.3/src/rail/cmnn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.687927 pz-rail-cmnn-0.1.3/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/src/rail/estimation/algos/cmnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.687927 pz-rail-cmnn-0.1.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 21:08:25.699928 pz-rail-cmnn-0.1.3/tests/cmnn/
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2023-10-31 21:08:11.000000 pz-rail-cmnn-0.1.3/tests/cmnn/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/src/rail/cmnn/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/src/rail/cmnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:01:30.000000 pz_rail_cmnn-1.0.0/src/rail/cmnn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/src/rail/estimation/algos/cmnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.170703 pz_rail_cmnn-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:01:30.174703 pz_rail_cmnn-1.0.0/tests/cmnn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 20:01:24.000000 pz_rail_cmnn-1.0.0/tests/cmnn/test_algos.py
```

### Comparing `pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_cmnn-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/pull_request_template.md` & `pz_rail_cmnn-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/workflows/linting.yml` & `pz_rail_cmnn-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/workflows/publish-to-pypi.yml` & `pz_rail_cmnn-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/workflows/smoke-test.yml` & `pz_rail_cmnn-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.github/workflows/testing-and-coverage.yml` & `pz_rail_cmnn-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.gitignore` & `pz_rail_cmnn-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/.pre-commit-config.yaml` & `pz_rail_cmnn-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/LICENSE` & `pz_rail_cmnn-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/PKG-INFO` & `pz_rail_cmnn-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.1.3
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-cmnn-0.1.3/README.md` & `pz_rail_cmnn-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/pyproject.toml` & `pz_rail_cmnn-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/PKG-INFO` & `pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-cmnn
-Version: 0.1.3
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-cmnn-0.1.3/src/pz_rail_cmnn.egg-info/SOURCES.txt` & `pz_rail_cmnn-1.0.0/src/pz_rail_cmnn.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 .github/ISSUE_TEMPLATE/1-bug_report.md
 .github/ISSUE_TEMPLATE/2-feature_request.md
 .github/workflows/add-issue-to-project-tracker.yml
 .github/workflows/linting.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/smoke-test.yml
 .github/workflows/testing-and-coverage.yml
-examples/CMNN_demo.ipynb
 src/pz_rail_cmnn.egg-info/PKG-INFO
 src/pz_rail_cmnn.egg-info/SOURCES.txt
 src/pz_rail_cmnn.egg-info/dependency_links.txt
 src/pz_rail_cmnn.egg-info/requires.txt
 src/pz_rail_cmnn.egg-info/top_level.txt
 src/rail/cmnn/__init__.py
 src/rail/cmnn/_version.py
```

### Comparing `pz-rail-cmnn-0.1.3/src/rail/estimation/algos/cmnn.py` & `pz_rail_cmnn-1.0.0/src/rail/estimation/algos/cmnn.py`

 * *Files identical despite different names*

### Comparing `pz-rail-cmnn-0.1.3/tests/cmnn/test_algos.py` & `pz_rail_cmnn-1.0.0/tests/cmnn/test_algos.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 import pytest
 from rail.core.stage import RailStage
 
 # from rail.core.data import DataStore, TableHandle
-from rail.core.algo_utils import one_algo
+from rail.utils.testing_utils import one_algo
 
-# from rail.core.utils import RAILDIR
 from rail.estimation.algos import cmnn
 
 default_dict = {"zmin": 0.0, "zmax": 3.0, "nzbins": 301, "min_n": 4}
 
 
 @pytest.mark.parametrize(
     "out_method,zb_expected",
```

