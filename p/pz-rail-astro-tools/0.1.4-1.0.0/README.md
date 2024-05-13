# Comparing `tmp/pz_rail_astro_tools-0.1.4.tar.gz` & `tmp/pz_rail_astro_tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_astro_tools-0.1.4.tar", last modified: Wed May  8 15:27:25 2024, max compression
+gzip compressed data, was "pz_rail_astro_tools-1.0.0.tar", last modified: Mon May 13 19:53:42 2024, max compression
```

## Comparing `pz_rail_astro_tools-0.1.4.tar` & `pz_rail_astro_tools-1.0.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.355141 pz_rail_astro_tools-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:27:25.000000 pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:27:24.000000 pz_rail_astro_tools-0.1.4/src/rail/astro_tools/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.355141 pz_rail_astro_tools-0.1.4/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/grid_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/lsst_error_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/observing_condition_degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/photometric_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_selections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/creation/engines/gcr_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.363141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.387141 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
--rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/src/rail/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/src/rail/tools/photometry_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.359141 pz_rail_astro_tools-0.1.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/tests/astro_tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:27:25.391141 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/
--rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-08 15:27:18.000000 pz_rail_astro_tools-0.1.4/tests/astro_tools/test_gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 19:53:42.000000 pz_rail_astro_tools-1.0.0/src/rail/astro_tools/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/grid_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/lsst_error_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19987 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/observing_condition_degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/photometric_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22182 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_selections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/creation/engines/gcr_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.802474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.810474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-13 19:53:35.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127) 13823712 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.834474 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits
+-rw-r--r--   0 runner    (1001) docker     (127)  1581120 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/src/rail/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    18419 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/src/rail/tools/photometry_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.806474 pz_rail_astro_tools-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/tests/astro_tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:53:42.838474 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)   179385 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24490 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_degraders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-13 19:53:36.000000 pz_rail_astro_tools-1.0.0/tests/astro_tools/test_gcr_engine.py
```

### Comparing `pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_astro_tools-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/pull_request_template.md` & `pz_rail_astro_tools-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/workflows/linting.yml` & `pz_rail_astro_tools-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/workflows/publish-to-pypi.yml` & `pz_rail_astro_tools-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/workflows/smoke-test.yml` & `pz_rail_astro_tools-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.github/workflows/testing-and-coverage.yml` & `pz_rail_astro_tools-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.gitignore` & `pz_rail_astro_tools-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/.pre-commit-config.yaml` & `pz_rail_astro_tools-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/LICENSE` & `pz_rail_astro_tools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/PKG-INFO` & `pz_rail_astro_tools-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-0.1.4/README.md` & `pz_rail_astro_tools-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/pyproject.toml` & `pz_rail_astro_tools-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/PKG-INFO` & `pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-astro-tools
-Version: 0.1.4
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <lsst-desc-rail-admin@slac.stanford.edu>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_astro_tools-0.1.4/src/pz_rail_astro_tools.egg-info/SOURCES.txt` & `pz_rail_astro_tools-1.0.0/src/pz_rail_astro_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/grid_selection.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/grid_selection.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/lsst_error_model.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/lsst_error_model.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/observing_condition_degrader.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/observing_condition_degrader.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/photometric_errors.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/photometric_errors.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_degraders.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/degraders/spectroscopic_selections.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/degraders/spectroscopic_selections.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/creation/engines/gcr_engine.py` & `pz_rail_astro_tools-1.0.0/src/rail/creation/engines/gcr_engine.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5` & `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/hsc_ratios_and_specz.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits` & `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-dr6-galcounts-i20-i25.3-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits` & `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/DC2-mask-neg-nside-128.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_airmass_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits` & `pz_rail_astro_tools-1.0.0/src/rail/examples_data/creation_data/data/survey_conditions/minion_1016_dc2_Median_fiveSigmaDepth_i_and_nightlt1825_HEAL.fits`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/src/rail/tools/photometry_tools.py` & `pz_rail_astro_tools-1.0.0/src/rail/tools/photometry_tools.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/schema.yaml` & `pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/schema.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5` & `pz_rail_astro_tools-1.0.0/tests/astro_tools/gcr_test_data/test_object_tract_4850.hdf5`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_core.py` & `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_core.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_degraders.py` & `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz_rail_astro_tools-0.1.4/tests/astro_tools/test_gcr_engine.py` & `pz_rail_astro_tools-1.0.0/tests/astro_tools/test_gcr_engine.py`

 * *Files identical despite different names*

