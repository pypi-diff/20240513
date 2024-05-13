# Comparing `tmp/pz_rail_pipelines-0.1.4.tar.gz` & `tmp/pz_rail_pipelines-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_pipelines-0.1.4.tar", last modified: Thu Apr 25 01:55:57 2024, max compression
+gzip compressed data, was "pz_rail_pipelines-1.0.0.tar", last modified: Mon May 13 20:37:33 2024, max compression
```

## Comparing `pz_rail_pipelines-0.1.4.tar` & `pz_rail_pipelines-1.0.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/.prepare_project.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/nb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/estimate_all.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/estimate_all_hsc.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/inform_all.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/estimation/inform_all_hsc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/nb/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/examples/goldenspike/goldenspike.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/nb/examples/survey_nonuniformity/
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/nb/examples/survey_nonuniformity/survey_nonuniform.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 01:55:57.225616 pz_rail_pipelines-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 01:55:57.000000 pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.213616 pz_rail_pipelines-0.1.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 01:55:56.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/estimate_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/inform_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.217615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/goldenspike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/survey_nonuniformity/
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/name_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 01:55:57.221615 pz_rail_pipelines-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-25 01:55:48.000000 pz_rail_pipelines-0.1.4/tests/test_pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.409572 pz_rail_pipelines-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.401572 pz_rail_pipelines-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.401572 pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.401572 pz_rail_pipelines-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/.prepare_project.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-13 20:37:33.409572 pz_rail_pipelines-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.397572 pz_rail_pipelines-1.0.0/nb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/nb/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)    14280 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/estimation/estimate_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12122 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/estimation/estimate_all_hsc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8196 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/estimation/inform_all.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/estimation/inform_all_hsc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.397572 pz_rail_pipelines-1.0.0/nb/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/nb/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/examples/goldenspike/goldenspike.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/nb/examples/survey_nonuniformity/
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/nb/examples/survey_nonuniformity/survey_nonuniform.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:37:33.409572 pz_rail_pipelines-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.397572 pz_rail_pipelines-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.397572 pz_rail_pipelines-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/rail/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:37:33.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/rail/pipelines/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/estimation/estimate_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/estimation/inform_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.397572 pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/goldenspike/
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/goldenspike/goldenspike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/survey_nonuniformity/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/src/rail/pipelines/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/src/rail/pipelines/utils/name_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:37:33.405572 pz_rail_pipelines-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-13 20:37:26.000000 pz_rail_pipelines-1.0.0/tests/test_pipelines.py
```

### Comparing `pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_pipelines-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/pull_request_template.md` & `pz_rail_pipelines-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/workflows/linting.yml` & `pz_rail_pipelines-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/workflows/publish-to-pypi.yml` & `pz_rail_pipelines-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/workflows/smoke-test.yml` & `pz_rail_pipelines-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.github/workflows/testing-and-coverage.yml` & `pz_rail_pipelines-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.gitignore` & `pz_rail_pipelines-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.pre-commit-config.yaml` & `pz_rail_pipelines-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/.prepare_project.sh` & `pz_rail_pipelines-1.0.0/.prepare_project.sh`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/LICENSE` & `pz_rail_pipelines-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/PKG-INFO` & `pz_rail_pipelines-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.1.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_pipelines-0.1.4/README.md` & `pz_rail_pipelines-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/nb/estimation/estimate_all.ipynb` & `pz_rail_pipelines-1.0.0/nb/estimation/estimate_all.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999565972222222%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [4]}}}'}*

```diff
@@ -9,15 +9,15 @@
             },
             "outputs": [],
             "source": [
                 "# usual imports\n",
                 "import os\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "from rail.bpz.utils import RAIL_BPZ_DIR\n",
                 "from rail.pipelines.estimation.estimate_all import EstimatePipeline\n",
                 "from rail.core import common_params\n",
                 "from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType\n",
                 "import qp\n",
                 "import ceci"
             ]
```

### Comparing `pz_rail_pipelines-0.1.4/nb/estimation/estimate_all_hsc.ipynb` & `pz_rail_pipelines-1.0.0/nb/estimation/estimate_all_hsc.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999543128654971%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [4]}}}'}*

```diff
@@ -9,15 +9,15 @@
             },
             "outputs": [],
             "source": [
                 "# usual imports\n",
                 "import os\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "#from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR\n",
                 "from rail.pipelines.estimation.estimate_all import EstimatePipeline\n",
                 "from rail.core import common_params\n",
                 "from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType\n",
                 "import qp\n",
                 "import ceci\n"
             ]
```

### Comparing `pz_rail_pipelines-0.1.4/nb/estimation/inform_all.ipynb` & `pz_rail_pipelines-1.0.0/nb/estimation/inform_all.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998914930555556%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [3]}}}'}*

```diff
@@ -8,15 +8,15 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# usual imports\n",
                 "import os\n",
                 "import numpy as np\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "from rail.bpz.utils import RAIL_BPZ_DIR\n",
                 "from rail.pipelines.estimation.inform_all import InformPipeline\n",
                 "from rail.core import common_params"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `pz_rail_pipelines-0.1.4/nb/estimation/inform_all_hsc.ipynb` & `pz_rail_pipelines-1.0.0/nb/estimation/inform_all_hsc.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833333%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(3, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [3]}}}'}*

```diff
@@ -8,15 +8,15 @@
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "# usual imports\n",
                 "import os\n",
                 "import numpy as np\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "#from rail.estimation.algos.bpz_version.utils import RAIL_BPZ_DIR\n",
                 "from rail.pipelines.estimation.inform_all import InformPipeline\n",
                 "from rail.core import common_params"
             ]
         },
         {
             "cell_type": "code",
```

### Comparing `pz_rail_pipelines-0.1.4/nb/examples/goldenspike/goldenspike.ipynb` & `pz_rail_pipelines-1.0.0/nb/examples/goldenspike/goldenspike.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968303571428572%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(2, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            "delete: [2]}}, 3: {'source': {insert: [(0, 'from rail.utils.path_utils import "*

 * *            "RAILDIR\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -13,15 +13,15 @@
             "execution_count": null,
             "id": "227aa23e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "import ceci\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "from rail.pipelines.examples.goldenspike.goldenspike import GoldenspikePipeline"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "b972d07a",
@@ -34,15 +34,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "23efbbb5",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')\n",
                 "pipe.initialize(dict(model=flow_file), dict(output_dir='.', log_dir='.', resume=False), None)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -115,13 +115,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail_pipelines-0.1.4/nb/examples/survey_nonuniformity/survey_nonuniform.ipynb` & `pz_rail_pipelines-1.0.0/nb/examples/survey_nonuniformity/survey_nonuniform.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997780539772727%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(4, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [4]}}, 16: {'source': {insert: [(0, 'from rail.utils.path_utils import "*

 * *            "RAILDIR\\n')], delete: [0]}}}"}*

```diff
@@ -7,15 +7,15 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# usual imports\n",
                 "import os\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "from rail.pipelines.examples.survey_nonuniformity.survey_nonuniformity import SurveyNonuniformDegraderPipeline\n",
                 "from rail.core import common_params\n",
                 "from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType\n",
                 "import qp\n",
                 "import ceci"
             ]
         },
@@ -271,15 +271,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ff0d1439-169b-45dc-b224-27cc3189aab9",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')\n",
                 "pipe_info = pipe.initialize(dict(model=flow_file), dict(output_dir='.', log_dir='.', resume=True), None)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `pz_rail_pipelines-0.1.4/pyproject.toml` & `pz_rail_pipelines-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/PKG-INFO` & `pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-pipelines
-Version: 0.1.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_pipelines-0.1.4/src/pz_rail_pipelines.egg-info/SOURCES.txt` & `pz_rail_pipelines-1.0.0/src/pz_rail_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/estimate_all.py` & `pz_rail_pipelines-1.0.0/src/rail/pipelines/estimation/estimate_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
 
 import ceci
 
 
 namer = NameFactory()
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 
 input_file = 'rubin_dm_dc2_example.pq'
 
 
 class EstimatePipeline(RailPipeline):
 
     def __init__(self):
```

### Comparing `pz_rail_pipelines-0.1.4/src/rail/pipelines/estimation/inform_all.py` & `pz_rail_pipelines-1.0.0/src/rail/pipelines/estimation/inform_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
 
 import ceci
 
 
 namer = NameFactory()
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 
 input_file = 'rubin_dm_dc2_example.pq'
 
 
 class InformPipeline(RailPipeline):
 
     def __init__(self):
```

### Comparing `pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/goldenspike/goldenspike.py` & `pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/goldenspike/goldenspike.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
 
 import ceci
 
 
 namer = NameFactory()
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')
 
 
 class GoldenspikePipeline(RailPipeline):
 
     def __init__(self):
         RailPipeline.__init__(self)
```

### Comparing `pz_rail_pipelines-0.1.4/src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py` & `pz_rail_pipelines-1.0.0/src/rail/pipelines/examples/survey_nonuniformity/survey_nonuniformity.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
 
 import ceci
 
 namer = NameFactory()
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')
 
 
 class SurveyNonuniformDegraderPipeline(RailPipeline):
     
     def __init__(self):
         RailPipeline.__init__(self)
```

### Comparing `pz_rail_pipelines-0.1.4/src/rail/pipelines/utils/name_factory.py` & `pz_rail_pipelines-1.0.0/src/rail/pipelines/utils/name_factory.py`

 * *Files identical despite different names*

### Comparing `pz_rail_pipelines-0.1.4/tests/test_pipelines.py` & `pz_rail_pipelines-1.0.0/tests/test_pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from rail.pipelines.examples.goldenspike.goldenspike import GoldenspikePipeline
 from rail.pipelines.utils.name_factory import NameFactory, DataType, CatalogType, ModelType, PdfType
 from rail.core.stage import RailStage, RailPipeline
-from rail.core.utils import RAILDIR
+from rail.utils.path_utils import RAILDIR
 
 
 def test_golden():
     namer = NameFactory()
     flow_file = os.path.join(RAILDIR, 'rail/examples_data/goldenspike_data/data/pretrained_flow.pkl')
     output_dir = namer.get_project_dir('.', 'tmp_test', 'tmp_test')
     try:
```

