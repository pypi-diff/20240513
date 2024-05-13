# Comparing `tmp/pz_rail-0.99.3.tar.gz` & `tmp/pz_rail-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail-0.99.3.tar", last modified: Wed Apr 24 01:18:43 2024, max compression
+gzip compressed data, was "pz_rail-1.0.0.tar", last modified: Mon May 13 16:17:54 2024, max compression
```

## Comparing `pz_rail-0.99.3.tar` & `pz_rail-1.0.0.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.493364 pz_rail-0.99.3/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/build_documentation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/smoke-test-head.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 01:18:33.000000 pz_rail-0.99.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 01:18:33.000000 pz_rail-0.99.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-24 01:18:43.493364 pz_rail-0.99.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-24 01:18:33.000000 pz_rail-0.99.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 01:18:33.000000 pz_rail-0.99.3/conda-reqs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.477364 pz_rail-0.99.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/_static/css/notebooks.css
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/demos.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/nbconvert-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/citing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/demonstrations.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/fix_an_issue.rst
--rw-r--r--   0 runner    (1001) docker     (127)    17570 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/new_algorithm.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/new_rail_stage.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13974 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-24 01:18:33.000000 pz_rail-0.99.3/docs/source/sharing_pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 01:18:33.000000 pz_rail-0.99.3/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.481364 pz_rail-0.99.3/examples/core_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11369 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/FileIO_DataStore.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Iterate_Tabular_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Run_Saved_Pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    13855 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/Useful_Utilities.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8447 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/hyperbolic_magnitude_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/pipe_example.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/core_examples/pipe_example_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.485364 pz_rail-0.99.3/examples/creation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18074 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/degradation-demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    17118 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/dsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_GridSelection_for_HSC.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    14843 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_ObsConditions.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9426 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/fsps_sed_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/photometric_realization_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    66554 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19565 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/creation_examples/posterior-demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.485364 pz_rail-0.99.3/examples/estimation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)    34096 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16877 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/CMNN_Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     8664 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/GPz_estimation_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/NZDir.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    25938 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/RAIL_estimation_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    28442 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/nzdir_as_pipeline.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    30501 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/somocluSOM_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36871 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/somocluSOMcluster_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    20794 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/estimation_examples/test_sampled_summarizers.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/examples/evaluation_examples/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    18248 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/Evaluation_Demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    29795 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/Evaluation_by_type.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/evaluation_examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/examples/goldenspike_examples/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/cleanup_pipeline.sh
--rw-r--r--   0 runner    (1001) docker     (127)    25361 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-04-24 01:18:33.000000 pz_rail-0.99.3/examples/goldenspike_examples/goldenspike_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-24 01:18:33.000000 pz_rail-0.99.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 01:18:33.000000 pz_rail-0.99.3/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 01:18:33.000000 pz_rail-0.99.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 01:18:43.493364 pz_rail-0.99.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 01:18:33.000000 pz_rail-0.99.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/src/pz_rail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/pz_rail.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/src/rail/hub/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-24 01:18:33.000000 pz_rail-0.99.3/src/rail/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 01:18:43.000000 pz_rail-0.99.3/src/rail/hub/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.473364 pz_rail-0.99.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 01:18:43.489364 pz_rail-0.99.3/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 01:18:33.000000 pz_rail-0.99.3/tests/hub/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.481211 pz_rail-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.461211 pz_rail-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.461211 pz_rail-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.465211 pz_rail-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/build_documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/smoke-test-head.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 16:17:48.000000 pz_rail-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 16:17:48.000000 pz_rail-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-13 16:17:54.481211 pz_rail-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-05-13 16:17:48.000000 pz_rail-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-13 16:17:48.000000 pz_rail-1.0.0/conda-reqs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.465211 pz_rail-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.457211 pz_rail-1.0.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.465211 pz_rail-1.0.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/_static/css/notebooks.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/demos.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/nbconvert-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.465211 pz_rail-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/demonstrations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/fix_an_issue.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17570 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/new_algorithm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/new_rail_stage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13974 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-05-13 16:17:48.000000 pz_rail-1.0.0/docs/source/sharing_pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 16:17:48.000000 pz_rail-1.0.0/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.465211 pz_rail-1.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.469211 pz_rail-1.0.0/examples/core_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    11370 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14992 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/FileIO_DataStore.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6366 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/Iterate_Tabular_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/Run_Saved_Pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13868 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/Useful_Utilities.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/hyperbolic_magnitude_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/pipe_example.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/core_examples/pipe_example_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.469211 pz_rail-1.0.0/examples/creation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18068 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/degradation-demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/dsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/example_ObsConditions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21721 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/fsps_sed_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/photerr_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11831 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/photometric_realization_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    65163 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19560 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/creation_examples/posterior-demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.473211 pz_rail-1.0.0/examples/estimation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    34102 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/BPZ_lite_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    22711 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/CMNN_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    11974 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/GPz_estimation_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19361 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/NZDir.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    25944 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/RAIL_estimation_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    28448 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/nzdir_as_pipeline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/somocluSOM_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36877 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    20800 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/estimation_examples/test_sampled_summarizers.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.473211 pz_rail-1.0.0/examples/evaluation_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    18254 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/Evaluation_Demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29801 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/Evaluation_by_type.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/evaluation_examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.477211 pz_rail-1.0.0/examples/goldenspike_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/cleanup_pipeline.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    26923 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/goldenspike.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/goldenspike.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-13 16:17:48.000000 pz_rail-1.0.0/examples/goldenspike_examples/goldenspike_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-13 16:17:48.000000 pz_rail-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-13 16:17:48.000000 pz_rail-1.0.0/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 16:17:48.000000 pz_rail-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:17:54.481211 pz_rail-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 16:17:48.000000 pz_rail-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.461211 pz_rail-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.477211 pz_rail-1.0.0/src/pz_rail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/pz_rail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/pz_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/pz_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/pz_rail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/pz_rail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.461211 pz_rail-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.477211 pz_rail-1.0.0/src/rail/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 16:17:48.000000 pz_rail-1.0.0/src/rail/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 16:17:54.000000 pz_rail-1.0.0/src/rail/hub/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.461211 pz_rail-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:17:54.477211 pz_rail-1.0.0/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 16:17:48.000000 pz_rail-1.0.0/tests/hub/test_import.py
```

### Comparing `pz_rail-0.99.3/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/pull_request_template.md` & `pz_rail-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/workflows/build_documentation.yml` & `pz_rail-1.0.0/.github/workflows/build_documentation.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/workflows/linting.yml` & `pz_rail-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/workflows/publish-to-pypi.yml` & `pz_rail-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/workflows/smoke-test-head.yml` & `pz_rail-1.0.0/.github/workflows/smoke-test-head.yml`

 * *Files 14% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         rail install --from-source --package-file rail_packages.yml
     - name: Set up fsps
       run: |
         git clone "https://github.com/cconroy20/fsps.git" "/opt/hostedtoolcache/Python/fsps"
         echo "SPS_HOME=/opt/hostedtoolcache/Python/fsps" >> $GITHUB_ENV
     - name: Run notebooks
       run: |
-        rail render-nb --skip examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb examples/${{ matrix.notebook-dir }}_examples/*.ipynb
+        rail render-nb --skip examples/creation_examples/dsps_sed_demo.ipynb  --skip examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb examples/${{ matrix.notebook-dir }}_examples/*.ipynb
     - name: Send status to Slack app (RAIL CI Reporter)
       if: ${{ failure() && github.event_name != 'workflow_dispatch' }}
       id: slack
       uses: slackapi/slack-github-action@v1.24.0
       with:
         # For posting a rich message using Block Kit
         payload: |
```

### Comparing `pz_rail-0.99.3/.github/workflows/smoke-test.yml` & `pz_rail-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.github/workflows/testing-and-coverage.yml` & `pz_rail-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.gitignore` & `pz_rail-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.pre-commit-config.yaml` & `pz_rail-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/.readthedocs.yaml` & `pz_rail-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/LICENSE` & `pz_rail-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/PKG-INFO` & `pz_rail-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.3
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail-0.99.3/README.md` & `pz_rail-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/Makefile` & `pz_rail-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/_static/css/notebooks.css` & `pz_rail-1.0.0/docs/_static/css/notebooks.css`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/conf.py` & `pz_rail-1.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/demos.rst` & `pz_rail-1.0.0/docs/demos.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/index.rst` & `pz_rail-1.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/citing.rst` & `pz_rail-1.0.0/docs/source/citing.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/contributing.rst` & `pz_rail-1.0.0/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/demonstrations.rst` & `pz_rail-1.0.0/docs/source/demonstrations.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/fix_an_issue.rst` & `pz_rail-1.0.0/docs/source/fix_an_issue.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/installation.rst` & `pz_rail-1.0.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/new_algorithm.rst` & `pz_rail-1.0.0/docs/source/new_algorithm.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/new_rail_stage.rst` & `pz_rail-1.0.0/docs/source/new_rail_stage.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/overview.rst` & `pz_rail-1.0.0/docs/source/overview.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/docs/source/sharing_pipeline.rst` & `pz_rail-1.0.0/docs/source/sharing_pipeline.rst`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb` & `pz_rail-1.0.0/examples/core_examples/Build_Save_Load_Run_Pipeline.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981886288998358%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'from rail.creation.degraders.spectroscopic_degraders "*

 * *            "import LineConfusion\\n'), (6, 'from rail.creation.degraders.quantityCut import "*

 * *            "QuantityCut\\n'), (7, 'from rail.creation.degraders.lsst_error_model import "*

 * *            "LSSTErrorModel\\n'), (11, 'from rail.tools.table_tools import ColumnMapper, "*

 * *            "TableConverter')], delete: [11, 7, 6, 5]}}, 6: {'source': {insert: [(0, 'from "*

 * *            "rail.utils.path_utils import fi […]*

```diff
@@ -33,21 +33,21 @@
             "outputs": [],
             "source": [
                 "import os\n",
                 "import numpy as np\n",
                 "import ceci\n",
                 "import rail\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.creation.degradation.spectroscopic_degraders import LineConfusion\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.spectroscopic_degraders import LineConfusion\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
                 "from rail.creation.engines.flowEngine import FlowCreator, FlowPosterior\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.util_stages import ColumnMapper, TableConverter"
+                "from rail.tools.table_tools import ColumnMapper, TableConverter"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We'll start by setting up the RAIL data store. RAIL uses [ceci](https://github.com/LSSTDESC/ceci), which is designed for pipelines rather than interactive notebooks; the data store will work around that and enable us to use data interactively.\n",
@@ -90,15 +90,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "\n",
                 "flow_file = find_rail_file(\"examples_data/goldenspike_data/data/pretrained_flow.pkl\")\n",
                 "bands = [\"u\", \"g\", \"r\", \"i\", \"z\", \"y\"]\n",
                 "band_dict = {band: f\"mag_{band}_lsst\" for band in bands}\n",
                 "rename_dict = {f\"mag_{band}_lsst_err\": f\"mag_err_{band}_lsst\" for band in bands}\n",
                 "post_grid = [float(x) for x in np.linspace(0.0, 5, 21)]"
             ]
@@ -367,15 +367,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "1cc5b75da6b94fd59f6c7b0992047078a9372d2242c3f23a554e39af5a039534"
             }
         }
     },
```

### Comparing `pz_rail-0.99.3/examples/core_examples/FileIO_DataStore.ipynb` & `pz_rail-1.0.0/examples/core_examples/FileIO_DataStore.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976636904761905%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(0, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -56,15 +56,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "\n",
                 "traindata_io = tables_io.read(trainFile)[\"photometry\"]"
             ]
         },
         {
@@ -389,13 +389,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb` & `pz_rail-1.0.0/examples/core_examples/FluxtoMag_and_Deredden_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975227591036415%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(6, 'from rail.utils.path_utils import find_rail_file\\n'), "*

 * *            "(7, 'from rail.tools.photometry_tools import LSSTFluxToMagConverter, Dereddener')], "*

 * *            'delete: [7, 6]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -23,16 +23,16 @@
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "import os\n",
                 "import tables_io\n",
                 "import tempfile\n",
                 "from rail.core.stage import RailStage\n",
                 "from rail.core.data import TableHandle\n",
-                "from rail.core.utils import find_rail_file\n",
-                "from rail.tools.util_photometry import LSSTFluxToMagConverter, Dereddener"
+                "from rail.utils.path_utils import find_rail_file\n",
+                "from rail.tools.photometry_tools import LSSTFluxToMagConverter, Dereddener"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "0ce08f0d-15f2-418b-8b3d-94937918b865",
             "metadata": {
@@ -228,13 +228,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/Iterate_Tabular_Data.ipynb` & `pz_rail-1.0.0/examples/core_examples/Iterate_Tabular_Data.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9968033509700176%*

 * *Differences: {"'cells'": "{6: {'source': {insert: [(0, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [0]}}, 15: {'source': ['from rail.tools.table_tools import ColumnMapper']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -74,15 +74,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "8ec1cb98",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "pdfs_file = find_rail_file(\"examples_data/testdata/test_dc2_training_9816.hdf5\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f60cfe60",
             "metadata": {},
@@ -174,15 +174,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "2f0543b0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.util_stages import ColumnMapper"
+                "from rail.tools.table_tools import ColumnMapper"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7a9451bb",
             "metadata": {},
@@ -215,13 +215,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/README.md` & `pz_rail-1.0.0/examples/core_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/core_examples/Run_Saved_Pipeline.ipynb` & `pz_rail-1.0.0/examples/core_examples/Run_Saved_Pipeline.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974371693121693%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(2, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [2]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -30,15 +30,15 @@
             "execution_count": null,
             "id": "a29a1b21",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "import ceci\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "\n",
                 "# To create a catalog, you need a model of what the distrubutions of the colors \n",
                 "# are--that's what this flow file is:\n",
                 "flow_file = find_rail_file('examples_data/goldenspike_data/data/pretrained_flow.pkl')\n",
                 "os.environ['FLOWDIR'] = os.path.dirname(flow_file)"
             ]
         },
@@ -94,13 +94,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/Useful_Utilities.ipynb` & `pz_rail-1.0.0/examples/core_examples/Useful_Utilities.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997490763546798%*

 * *Differences: {"'cells'": "{9: {'source': {insert: [(2, 'print(rail.tools.table_tools.ColumnMapper)')], delete: "*

 * *            "[2]}}, 22: {'source': {insert: [(1, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            "delete: [1]}}, 24: {'source': {insert: [(0, 'from rail.utils.path_utils import "*

 * *            "find_rail_file\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -91,15 +91,15 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# with prefix\n",
                 "\n",
-                "print(rail.core.util_stages.ColumnMapper)"
+                "print(rail.tools.table_tools.ColumnMapper)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -224,15 +224,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "\n",
                 "flow_file = os.path.join(\n",
                 "    RAILDIR, \"rail/examples_data/goldenspike_data/data/pretrained_flow.pkl\"\n",
                 ")"
             ]
         },
         {
@@ -246,15 +246,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "\n",
                 "flow_file = find_rail_file('examples_data/goldenspike_data/data/pretrained_flow.pkl')"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -581,13 +581,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/hyperbolic_magnitude_test.ipynb` & `pz_rail-1.0.0/examples/core_examples/hyperbolic_magnitude_test.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981068121693122%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(8, 'from rail.tools.photometry_tools import "*

 * *            "HyperbolicSmoothing, HyperbolicMagnitudes')], delete: [8]}}, 6: {'source': {insert: "*

 * *            "[(0, 'from rail.utils.path_utils import find_rail_file\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -34,15 +34,15 @@
                 "\n",
                 "import numpy as np\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "import rail\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.tools.util_photometry import HyperbolicSmoothing, HyperbolicMagnitudes"
+                "from rail.tools.photometry_tools import HyperbolicSmoothing, HyperbolicMagnitudes"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "26ff5986-1a7f-4de4-99f9-31f2c3361c7d",
             "metadata": {},
             "source": [
@@ -71,15 +71,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "e15ae47d-5e50-410a-890c-caf30763d1ed",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.pq')\n",
                 "test_mags = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "fc93c6ca-9c8f-4b1f-9d25-362606756a71",
@@ -233,13 +233,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/core_examples/pipe_example.yml` & `pz_rail-1.0.0/examples/core_examples/pipe_example.yml`

 * *Files 10% similar despite different names*

```diff
@@ -9,18 +9,18 @@
   max_threads: 2
 stages:
 - classname: FlowCreator
   module_name: rail.creation.engines.flowEngine
   name: flow_engine_test
   nprocess: 1
 - classname: LSSTErrorModel
-  module_name: rail.creation.degradation.lsst_error_model
+  module_name: rail.creation.degraders.lsst_error_model
   name: lsst_error_model_test
   nprocess: 1
 - classname: ColumnMapper
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: col_remapper_test
   nprocess: 1
 - classname: TableConverter
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: table_conv_test
   nprocess: 1
```

### Comparing `pz_rail-0.99.3/examples/core_examples/pipe_example_config.yml` & `pz_rail-1.0.0/examples/core_examples/pipe_example_config.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/creation_examples/README.md` & `pz_rail-1.0.0/examples/creation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/creation_examples/degradation-demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/degradation-demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998626373626374%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(3, 'from rail.creation.degraders.spectroscopic_degraders "*

 * *            "import (\\n'), (7, 'from rail.creation.degraders.lsst_error_model import "*

 * *            "LSSTErrorModel\\n'), (8, 'from rail.creation.degraders.quantityCut import "*

 * *            "QuantityCut\\n')], delete: [8, 7, 3]}}}"}*

```diff
@@ -36,20 +36,20 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "from pzflow.examples import get_example_flow\n",
                 "from rail.creation.engines.flowEngine import FlowCreator\n",
-                "from rail.creation.degradation.spectroscopic_degraders import (\n",
+                "from rail.creation.degraders.spectroscopic_degraders import (\n",
                 "    InvRedshiftIncompleteness,\n",
                 "    LineConfusion,\n",
                 ")\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
                 "from rail.core.stage import RailStage\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/dsps_sed_demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/dsps_sed_demo.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950942968242076%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(2, 'author: Luca Tortorelli\\n'), (4, 'last run "*

 * *            'successfully: May 10, 2024\\n\'), (6, "This notebook demonstrates some basic usage of '*

 * *            'the rail_dsps library. In particular, for a galaxy with some arbitrary star formation '*

 * *            "history, we'll see how to calculate its restframe SED, and its absolute and apparent "*

 * *            'magnitude in some band.\\n"), (8, \'SPS calculations are based on a set of template '*

 * *            'SEDs of s […]*

```diff
@@ -7,21 +7,23 @@
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "source": [
                 "# Demo of SED and photometry calculations with DSPS\n",
                 "\n",
-                "author: Luca Tortorelli, Andrew Hearin\n",
+                "author: Luca Tortorelli\n",
                 "\n",
-                "last run successfully: Aug 1, 2023\n",
+                "last run successfully: May 10, 2024\n",
                 "\n",
-                "This notebook demonstrates some basic usage of the DSPS library. In particular, for a galaxy with some arbitrary star formation history, we'll see how to calculate its restframe SED, and its absolute and apparent magnitude in some band.\n",
+                "This notebook demonstrates some basic usage of the rail_dsps library. In particular, for a galaxy with some arbitrary star formation history, we'll see how to calculate its restframe SED, and its absolute and apparent magnitude in some band.\n",
                 "\n",
-                "SPS calculations are based on a set of template SEDs of simple stellar populations (SSPs). Supplying such templates is outside the planned scope of the DSPS package, and so they will need to be retrieved from some other library. For example, the FSPS library supplies such templates in a convenient form."
+                "SPS calculations are based on a set of template SEDs of simple stellar populations (SSPs). Supplying such templates is outside the planned scope of the DSPS package, and so they will need to be retrieved from some other library. For example, the FSPS library supplies such templates in a convenient form.\n",
+                "\n",
+                "In case the user is not aware of how to generate these templates, the code automatically downloads a pre-defined library from NERSC."
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
@@ -37,40 +39,44 @@
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "source": [
-                "The SingleSedModeler class allows the user to generate a single rest-frame SED at the time with DSPS.\n",
+                "The SingleSedModeler class allows the user to generate a single rest-frame SED at the time with rail_dsps.\n",
                 "\n",
                 "Some example galaxy properties that are required to create a single SED model are generated via this notebook and stored into an hdf5 table. The required galaxy properties are:\n",
                 "\n",
                 "- galaxy redshifts\n",
                 "- the grid of cosmic time over which the star-formation history of galaxies is evaluated in units of Gyr\n",
                 "- the star-formation history of galaxies in units of Msun/yr\n",
                 "- galaxy metallicity at the time of observation in units of log10(Z)\n",
                 "- log normal scatter of the galaxy metallicity at the time of observation\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 1,
             "metadata": {
+                "ExecuteTime": {
+                    "end_time": "2024-05-10T15:41:08.510620Z",
+                    "start_time": "2024-05-10T15:41:05.620759Z"
+                },
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rail.dsps\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.data import TableHandle\n",
+                "from rail.core.data import Hdf5Handle\n",
                 "import numpy as np\n",
                 "import h5py"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -81,18 +87,17 @@
                 }
             },
             "outputs": [],
             "source": [
                 "DS = RailStage.data_store\n",
                 "DS.__class__.allow_overwrite = True\n",
                 "\n",
-                "RAIL_DSPS_DIR = os.path.abspath(os.path.join(os.path.dirname(rail.dsps.__file__), '..', '..'))\n",
-                "default_rail_fsps_files_folder = os.path.join(RAIL_DSPS_DIR, 'rail', 'examples_data', 'creation_data',\n",
-                "                                              'data', 'dsps_default_data')\n",
-                "input_file = os.path.join(default_rail_fsps_files_folder, 'input_galaxy_properties_dsps.hdf5')"
+                "RAIL_DSPS_DIR = os.path.abspath(os.path.join(os.path.dirname(rail.dsps.__file__), '..'))\n",
+                "default_rail_fsps_files_folder = os.path.join(RAIL_DSPS_DIR, 'examples_data/creation_data/data/dsps_default_data')\n",
+                "trainFile = os.path.join(default_rail_fsps_files_folder, 'input_galaxy_properties_dsps.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
@@ -113,15 +118,15 @@
                 "gal_lgmet_scatter = 0.2 # lognormal scatter in the metallicity distribution function\n",
                 "\n",
                 "cosmic_time_grid = np.full((n_galaxies, len(gal_t_table)), gal_t_table)\n",
                 "star_formation_history = np.full((n_galaxies, len(gal_sfr_table)), gal_sfr_table)\n",
                 "stellar_metallicity = np.full(n_galaxies, gal_lgmet)\n",
                 "stellar_metallicity_scatter = np.full(n_galaxies, gal_lgmet_scatter)\n",
                 "\n",
-                "with h5py.File(input_file, 'w') as h5table:\n",
+                "with h5py.File(trainFile, 'w') as h5table:\n",
                 "    h5table.create_dataset(name='redshifts', data=redshift)\n",
                 "    h5table.create_dataset(name='cosmic_time_grid', data=cosmic_time_grid)\n",
                 "    h5table.create_dataset(name='star_formation_history', data=star_formation_history)\n",
                 "    h5table.create_dataset(name='stellar_metallicity', data=stellar_metallicity)\n",
                 "    h5table.create_dataset(name='stellar_metallicity_scatter', data=stellar_metallicity_scatter)"
             ]
         },
@@ -131,18 +136,15 @@
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
-            "source": [
-                "trainFile = os.path.join(input_file)\n",
-                "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)"
-            ]
+            "source": "training_data = DS.read_file(\"training_data\", Hdf5Handle, trainFile)"
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
@@ -160,36 +162,35 @@
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
                 "dspssinglesedmodeler = rail.dsps.DSPSSingleSedModeler.make_stage(name='DSPSSingleSedModeler',\n",
-                "                                                                 ssp_templates_file=os.path.join(RAIL_DSPS_DIR,'rail/examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
+                "                                                                 ssp_templates_file=os.path.join(RAIL_DSPS_DIR,'examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
                 "                                                                 redshift_key='redshifts',\n",
                 "                                                                 cosmic_time_grid_key='cosmic_time_grid',\n",
                 "                                                                 star_formation_history_key='star_formation_history',\n",
                 "                                                                 stellar_metallicity_key='stellar_metallicity',\n",
                 "                                                                 stellar_metallicity_scatter_key='stellar_metallicity_scatter',\n",
-                "                                                                 restframe_sed_key='restframe_seds', default_cosmology=True)"
+                "                                                                 restframe_sed_key='restframe_seds', default_cosmology=True,\n",
+                "                                                                 min_wavelength=250, max_wavelength=12000)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
-            "source": [
-                "dspssinglesedmodel = dspssinglesedmodeler.fit_model(input_data=training_data)"
-            ]
+            "source": "dspssinglesedmodel = dspssinglesedmodeler.fit_model(input_data=training_data)"
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
@@ -235,15 +236,15 @@
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rail.dsps\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.data import TableHandle\n",
+                "from rail.core.data import Hdf5Handle\n",
                 "import numpy as np\n",
                 "import h5py"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -254,17 +255,16 @@
                 }
             },
             "outputs": [],
             "source": [
                 "DS = RailStage.data_store\n",
                 "DS.__class__.allow_overwrite = True\n",
                 "\n",
-                "default_rail_fsps_files_folder = os.path.join(RAIL_DSPS_DIR, 'rail', 'examples_data', 'creation_data',\n",
-                "                                              'data', 'dsps_default_data')\n",
-                "input_file = os.path.join(default_rail_fsps_files_folder, 'input_galaxy_properties_dsps.hdf5')"
+                "default_rail_fsps_files_folder = os.path.join(RAIL_DSPS_DIR, 'examples_data/creation_data/data/dsps_default_data')\n",
+                "trainFile = os.path.join(default_rail_fsps_files_folder, 'input_galaxy_properties_dsps.hdf5')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
@@ -285,15 +285,15 @@
                 "gal_lgmet_scatter = 0.2 # lognormal scatter in the metallicity distribution function\n",
                 "\n",
                 "cosmic_time_grid = np.full((n_galaxies, len(gal_t_table)), gal_t_table)\n",
                 "star_formation_history = np.full((n_galaxies, len(gal_sfr_table)), gal_sfr_table)\n",
                 "stellar_metallicity = np.full(n_galaxies, gal_lgmet)\n",
                 "stellar_metallicity_scatter = np.full(n_galaxies, gal_lgmet_scatter)\n",
                 "\n",
-                "with h5py.File(input_file, 'w') as h5table:\n",
+                "with h5py.File(trainFile, 'w') as h5table:\n",
                 "    h5table.create_dataset(name='redshifts', data=redshift)\n",
                 "    h5table.create_dataset(name='cosmic_time_grid', data=cosmic_time_grid)\n",
                 "    h5table.create_dataset(name='star_formation_history', data=star_formation_history)\n",
                 "    h5table.create_dataset(name='stellar_metallicity', data=stellar_metallicity)\n",
                 "    h5table.create_dataset(name='stellar_metallicity_scatter', data=stellar_metallicity_scatter)"
             ]
         },
@@ -303,39 +303,37 @@
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
-            "source": [
-                "trainFile = os.path.join(input_file)\n",
-                "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)"
-            ]
+            "source": "training_data = DS.read_file(\"training_data\", Hdf5Handle, trainFile)"
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
             "source": [
                 "dspspopulationsedmodeler = rail.dsps.DSPSPopulationSedModeler.make_stage(name='DSPSPopulationSedModeler',\n",
                 "                                                                         ssp_templates_file=os.path.join(RAIL_DSPS_DIR,\n",
-                "                                                                         'rail/examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
+                "                                                                         'examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
                 "                                                                         redshift_key='redshifts',\n",
                 "                                                                         cosmic_time_grid_key='cosmic_time_grid',\n",
                 "                                                                         star_formation_history_key='star_formation_history',\n",
                 "                                                                         stellar_metallicity_key='stellar_metallicity',\n",
                 "                                                                         stellar_metallicity_scatter_key='stellar_metallicity_scatter',\n",
-                "                                                                         restframe_sed_key='restframe_seds', default_cosmology=True)"
+                "                                                                         restframe_sed_key='restframe_seds', default_cosmology=True,\n",
+                "                                                                         min_wavelength=250, max_wavelength=12000)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
@@ -387,14 +385,15 @@
                 "\n",
                 "Generating the observed photometry with DSPS is simple and requires only few input from the user. The required input are:\n",
                 "- the redshift dataset keyword of the hdf5 table containing the rest-frame SEDs output from the DSPSPopulationSedModeler\n",
                 "- the rest-frame SEDs dataset keyword of the hdf5 table containing the rest-frame SEDs output from the DSPSPopulationSedModeler\n",
                 "- the absolute and apparent magnitudes dataset keyword of the output hdf5 table\n",
                 "- the folder path containing the filter bands\n",
                 "- the name of the filter bands in order of increasing wavelength\n",
+                "- the minimum and maximum wavelength used in the DSPSPopulationSedModeler class to generate the rest-frame SEDs\n",
                 "- the path to the SSP template files\n",
                 "- a boolean keyword to use (True) the default cosmology in DSPS.\n",
                 "\n",
                 "If the latter keyword is set to False, then the user has to manually provide the values of Om0, w0, wa and h in the .sample function."
             ]
         },
         {
@@ -407,15 +406,15 @@
                 }
             },
             "outputs": [],
             "source": [
                 "import os\n",
                 "import rail.dsps\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.data import TableHandle"
+                "from rail.core.data import Hdf5Handle"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
@@ -424,31 +423,28 @@
                 }
             },
             "outputs": [],
             "source": [
                 "DS = RailStage.data_store\n",
                 "DS.__class__.allow_overwrite = True\n",
                 "\n",
-                "input_file = 'model_DSPSPopulationSedModeler.hdf5'"
+                "trainFile = 'model_DSPSPopulationSedModeler.hdf5'"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
                     "outputs_hidden": false
                 }
             },
             "outputs": [],
-            "source": [
-                "trainFile = os.path.join(input_file)\n",
-                "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)"
-            ]
+            "source": "training_data = DS.read_file(\"training_data\", Hdf5Handle, trainFile)"
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "collapsed": false,
                 "jupyter": {
@@ -459,19 +455,20 @@
             "source": [
                 "dspsphotometrycreator = rail.dsps.DSPSPhotometryCreator.make_stage(name='DSPSPhotometryCreator',\n",
                 "                                                         redshift_key='redshifts',\n",
                 "                                                         restframe_sed_key='restframe_seds',\n",
                 "                                                         absolute_mags_key='rest_frame_absolute_mags',\n",
                 "                                                         apparent_mags_key='apparent_mags',\n",
                 "                                                         filter_folder=os.path.join(RAIL_DSPS_DIR,\n",
-                "                                                         'rail/examples_data/creation_data/data/dsps_default_data/filters'),\n",
+                "                                                         'examples_data/creation_data/data/dsps_default_data/filters'),\n",
                 "                                                         instrument_name='lsst',\n",
                 "                                                         wavebands='u,g,r,i,z,y',\n",
+                "                                                         min_wavelength=250, max_wavelength=12000,\n",
                 "                                                         ssp_templates_file=os.path.join(RAIL_DSPS_DIR,\n",
-                "                                                         'rail/examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
+                "                                                         'examples_data/creation_data/data/dsps_default_data/ssp_data_fsps_v3.2_lgmet_age.h5'),\n",
                 "                                                         default_cosmology=True)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/example_GridSelection_for_HSC.ipynb` & `pz_rail-1.0.0/examples/creation_examples/example_GridSelection_for_HSC.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973119087702421%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(8, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [8]}}, 10: {'source': ['from rail.creation.degraders.grid_selection import "*

 * *            "GridSelection']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -34,15 +34,15 @@
                 "import os\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import tables_io\n",
                 "import pandas as pd\n",
                 "#from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "%matplotlib inline "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "4e1841bd-ec07-4929-9a07-88f962080677",
@@ -132,15 +132,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "9a57be3c-8d1e-4da2-82bf-0ed7912d918b",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.creation.degradation.grid_selection import GridSelection"
+                "from rail.creation.degraders.grid_selection import GridSelection"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "cb7b98d1-c497-49fc-9af8-0a5522575e9f",
             "metadata": {},
@@ -313,13 +313,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/example_ObsConditions.ipynb` & `pz_rail-1.0.0/examples/creation_examples/example_ObsConditions.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973820546737213%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(2, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [2]}}, 10: {'source': ['from rail.creation.degraders import "*

 * *            "observing_condition_degrader\\n', 'from "*

 * *            "rail.creation.degraders.observing_condition_degrader import ObsCondition']}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -72,15 +72,15 @@
             "execution_count": null,
             "id": "ad5b5402-33ba-410a-94e3-692baf88795c",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import rail\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "DS = RailStage.data_store\n",
                 "DS.__class__.allow_overwrite = True"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aa290f92-3f7c-4736-8b19-92018efee2d9",
@@ -140,16 +140,16 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ae04bfec-aed2-45cc-8df1-93d5fa3d28e7",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.creation.degradation import observing_condition_degrader\n",
-                "from rail.creation.degradation.observing_condition_degrader import ObsCondition"
+                "from rail.creation.degraders import observing_condition_degrader\n",
+                "from rail.creation.degraders.observing_condition_degrader import ObsCondition"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "dd785f06-891b-4f5f-800f-b30929c8d07f",
             "metadata": {},
@@ -435,13 +435,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb` & `pz_rail-1.0.0/examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981436387686388%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(7, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [7]}}, 12: {'source': {insert: [(1, 'from rail.creation.degraders import "*

 * *            "spectroscopic_selections\\n'), (3, 'from "*

 * *            "rail.creation.degraders.spectroscopic_selections import SpecSelection_zCOSMOS')], "*

 * *            'delete: [3, 1]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -38,15 +38,15 @@
                 "import rail\n",
                 "import os\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import tables_io\n",
                 "import pandas as pd\n",
                 "#from rail.core.data import TableHandle\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "from rail.core.stage import RailStage\n",
                 "%matplotlib inline "
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -147,17 +147,17 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "24c937c7-34e0-4b79-ad6c-1461f4ddc793",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import sys\n",
-                "from rail.creation.degradation import spectroscopic_selections\n",
+                "from rail.creation.degraders import spectroscopic_selections\n",
                 "from importlib import reload\n",
-                "from rail.creation.degradation.spectroscopic_selections import SpecSelection_zCOSMOS"
+                "from rail.creation.degraders.spectroscopic_selections import SpecSelection_zCOSMOS"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "144af9b4-436b-4eda-9047-433940141f45",
             "metadata": {},
@@ -287,15 +287,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/fsps_sed_demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/fsps_sed_demo.ipynb`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/creation_examples/photometric_realization_demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/photometric_realization_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998456790123457%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(3, 'from rail.creation.degraders.lsst_error_model import "*

 * *            "LSSTErrorModel\\n')], delete: [3]}}}"}*

```diff
@@ -23,15 +23,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "from pzflow.examples import get_example_flow\n",
                 "from rail.creation.engines.flowEngine import FlowCreator\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
                 "from rail.core.stage import RailStage\n"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756596436651583%*

 * *Differences: {"'cells'": "{0: {'source': {delete: [0]}}, 1: {'source': '## Read skysim v3.1.0 and cosmoDC2 "*

 * *            "v1.1.4 catalogs with the GCRCatalogs class, alternatively curl from web repository'}, "*

 * *            '2: {\'source\': [\'try:\\n\', \'    import GCRCatalogs\\n\', "    skysim3 = '*

 * *            'GCRCatalogs.load_catalog(\'skysim_v3.1.0\')\\n", "    cosmodc2 = '*

 * *            'GCRCatalogs.load_catalog(\'cosmoDC2_v1.1.4_small\')\\n", \'    skysim3_allcols = '*

 * *            "skysim3.list_all_native_quantities( […]*

```diff
@@ -5,138 +5,73 @@
             "execution_count": null,
             "id": "c087f952-7aad-4b5e-96f2-8fe4bb72243b",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "import GCRCatalogs\n",
                 "import matplotlib.pyplot as plt\n",
                 "import pandas as pd\n",
                 "import corner\n",
                 "import numpy as np\n",
                 "import h5py\n",
                 "from astropy.table import Table\n",
                 "import os"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6b84d8ef-ea56-4bb8-b15f-5a5b10691d66",
             "metadata": {},
-            "source": [
-                "## Read skysim v3.1.0 and cosmoDC2 v1.1.4 catalogs with the GCRCatalogs class"
-            ]
+            "source": "## Read skysim v3.1.0 and cosmoDC2 v1.1.4 catalogs with the GCRCatalogs class, alternatively curl from web repository"
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "3f367960-308e-49a9-8ba1-095c409b7915",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "skysim3 = GCRCatalogs.load_catalog('skysim_v3.1.0')\n",
-                "cosmodc2 = GCRCatalogs.load_catalog('cosmoDC2_v1.1.4_small')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "a0675c78-2fff-4692-bfbb-de25a5a60e62",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "skysim3_allcols = skysim3.list_all_native_quantities()\n",
-                "cosmodc2_allcols = cosmodc2.list_all_native_quantities()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "c12c1711-b8a7-4d60-9d94-4455b37a2490",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "skysim3_relevantcols = ['LSST_obs_g','LSST_obs_i','LSST_obs_r','LSST_obs_u','LSST_obs_y','LSST_obs_z','LSST_rest_G','LSST_rest_I','LSST_rest_R',\n",
+                "try:\n",
+                "    import GCRCatalogs\n",
+                "    skysim3 = GCRCatalogs.load_catalog('skysim_v3.1.0')\n",
+                "    cosmodc2 = GCRCatalogs.load_catalog('cosmoDC2_v1.1.4_small')\n",
+                "    skysim3_allcols = skysim3.list_all_native_quantities()\n",
+                "    cosmodc2_allcols = cosmodc2.list_all_native_quantities()\n",
+                "    skysim3_relevantcols = ['LSST_obs_g','LSST_obs_i','LSST_obs_r','LSST_obs_u','LSST_obs_y','LSST_obs_z','LSST_rest_G','LSST_rest_I','LSST_rest_R',\n",
                 "                        'LSST_rest_U' ,'LSST_rest_Y','LSST_rest_Z','lg_met_mean','lg_met_scatter','log_sm','log_ssfr','obs_sfr','obs_sm',\n",
                 "                        'redshift','sfr','HSC_obs_g','HSC_obs_i','HSC_obs_r','HSC_obs_y','HSC_obs_z','HSC_rest_G','HSC_rest_I','HSC_rest_R',\n",
                 "                        'HSC_rest_Y','HSC_rest_Z', 'diffmah_early_index', 'lg_met_scatter', \n",
                 "                        'diffstar_u_indx_lo', 'diffstar_u_tau_dep', 'diffmah_mah_logtc', 'diffmah_logmp_fit',\n",
                 "                        'lg_met_mean', 'diffstar_u_qs', 'diffstar_u_q_rejuv', 'diffstar_u_lgmcrit',\n",
                 "                        'diffstar_u_qt', 'diffmah_late_index', 'diffstar_u_q_drop', 'diffstar_u_lgy_at_mcrit',\n",
-                "                        'diffstar_u_indx_hi']"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f7f7ed74-1146-4094-b95a-3524e208bb49",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "cosmodc2_relevantcols = ['LSST_filters/magnitude:LSST_u:rest','LSST_filters/magnitude:LSST_g:rest','LSST_filters/magnitude:LSST_r:rest',\n",
+                "                        'diffstar_u_indx_hi']\n",
+                "    cosmodc2_relevantcols = ['LSST_filters/magnitude:LSST_u:rest','LSST_filters/magnitude:LSST_g:rest','LSST_filters/magnitude:LSST_r:rest',\n",
                 "                         'LSST_filters/magnitude:LSST_i:rest','LSST_filters/magnitude:LSST_z:rest','LSST_filters/magnitude:LSST_y:rest',\n",
                 "                         'LSST_filters/magnitude:LSST_u:observed','LSST_filters/magnitude:LSST_g:observed','LSST_filters/magnitude:LSST_r:observed',\n",
                 "                         'LSST_filters/magnitude:LSST_i:observed','LSST_filters/magnitude:LSST_z:observed','LSST_filters/magnitude:LSST_y:observed',\n",
-                "                         'baseDC2/sfr','baseDC2/redshift','baseDC2/obs_sfr','baseDC2/obs_sm','baseDC2/sm']"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "f8769596-f16f-46f5-84ed-e88aa56f0ef0",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "skysim3_quantities = skysim3.get_quantities(skysim3_relevantcols, native_filters=['healpix_pixel == 9816'])\n",
-                "cosmodc2_quantities = cosmodc2.get_quantities(cosmodc2_relevantcols, native_filters=['healpix_pixel == 9816'])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "20db1f1b-d877-4134-9991-7b448d09a584",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "skysim3_df = pd.DataFrame(skysim3_quantities)\n",
-                "cosmodc2_df = pd.DataFrame(cosmodc2_quantities)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "cfdc79d5-b9d7-4b3e-9ae0-b7ebcac8838f",
-            "metadata": {},
-            "source": [
-                "## Select a random subset of 100k objects per catalog to facilitate plotting"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "934e777e-232e-4bc8-a59e-0331541aa074",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "skysim3_df_100k = skysim3_df.sample(n=100000)\n",
-                "cosmodc2_df_100k = cosmodc2_df.sample(n=100000)"
+                "                         'baseDC2/sfr','baseDC2/redshift','baseDC2/obs_sfr','baseDC2/obs_sm','baseDC2/sm']\n",
+                "    skysim3_quantities = skysim3.get_quantities(skysim3_relevantcols, native_filters=['healpix_pixel == 9816'])\n",
+                "    cosmodc2_quantities = cosmodc2.get_quantities(cosmodc2_relevantcols, native_filters=['healpix_pixel == 9816'])\n",
+                "    skysim3_df = pd.DataFrame(skysim3_quantities)\n",
+                "    cosmodc2_df = pd.DataFrame(cosmodc2_quantities)\n",
+                "    # Select a random subset of 100k objects per catalog to facilitate plotting\n",
+                "    skysim3_df_100k = skysim3_df.sample(n=100000)\n",
+                "    cosmodc2_df_100k = cosmodc2_df.sample(n=100000)\n",
+                "    \n",
+                "except ModuleNotFoundError:\n",
+                "    output_directory = os.getcwd()\n",
+                "    os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/skysim_v3.1.0_100kpublic.csv '\n",
+                "              '--output-dir {}'.format(output_directory))\n",
+                "    os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/cosmodc2_100kpublic.csv '\n",
+                "              '--output-dir {}'.format(output_directory))\n",
+                "    skysim3_df_100k = pd.read_csv(os.path.join(output_directory, 'skysim_v3.1.0_100kpublic.csv'))\n",
+                "    cosmodc2_df_100k = pd.read_csv(os.path.join(output_directory, 'cosmodc2_100kpublic.csv'))"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b7090af7-a65b-4bbe-ab17-37ea5219c112",
             "metadata": {
                 "tags": []
@@ -753,51 +688,19 @@
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "output_directory = os.getcwd()\n",
                 "\n",
-                "if not os.path.isfile(os.path.join(output_directory,'COSMOS2020_CLASSIC_R1_v2.0.fits')):\n",
-                "    os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/COSMOS2020_CLASSIC_R1_v2.0.fits '\n",
+                "if not os.path.isfile(os.path.join(output_directory,'COSMOS2020_CLASSIC_R1_v2.0_100k.fits')):\n",
+                "    os.system('curl -O https://portal.nersc.gov/cfs/lsst/PZ/COSMOS2020_CLASSIC_R1_v2.0_100k.fits '\n",
                 "              '--output-dir {}'.format(output_directory))\n",
                 "\n",
-                "cosmos2020 = Table.read(os.path.join(output_directory,'COSMOS2020_CLASSIC_R1_v2.0.fits'), format='fits')"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "30624b69-b012-4f3c-994e-03f2fb0e1352",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "mask_bad_values = np.where((cosmos2020['CFHT_u_MAG_AUTO'] > 0) & \n",
-                "                             (cosmos2020['HSC_i_MAG_AUTO'] > 0)&\n",
-                "                             (cosmos2020['HSC_g_MAG_AUTO'] > 0)&\n",
-                "                             (cosmos2020['HSC_r_MAG_AUTO'] > 0) & \n",
-                "                             (cosmos2020['HSC_z_MAG_AUTO'] > 0)&\n",
-                "                             (cosmos2020['HSC_y_MAG_AUTO'] > 0)&\n",
-                "                             (cosmos2020['UVISTA_J_MAG_AUTO'] > 0) &\n",
-                "                             (cosmos2020['UVISTA_H_MAG_AUTO'] > 0) & \n",
-                "                             (cosmos2020['UVISTA_Ks_MAG_AUTO'] > 0))"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "e4dd14a6-585c-45bf-9522-6454ef335f6b",
-            "metadata": {
-                "tags": []
-            },
-            "outputs": [],
-            "source": [
-                "cosmos2020 = cosmos2020[mask_bad_values]"
+                "cosmos2020 = Table.read(os.path.join(output_directory,'COSMOS2020_CLASSIC_R1_v2.0_100k.fits'), format='fits')"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "aea7d6bc-40b0-40c8-b604-0e81e2155a0b",
             "metadata": {},
             "source": [
@@ -809,16 +712,16 @@
             "execution_count": null,
             "id": "a34df6e0-3ecc-413b-a53f-1a8496b038fc",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "skysim3_df_lsst_y1_all = skysim3_df.loc[skysim3_df['LSST_obs_i']<=24.1]\n",
-                "cosmodc2_df_lsst_y1_all = cosmodc2_df.loc[cosmodc2_df['LSST_filters/magnitude:LSST_i:observed']<=24.1]"
+                "skysim3_df_lsst_y1 = skysim3_df_100k.loc[skysim3_df_100k['LSST_obs_i']<=24.1]\n",
+                "cosmodc2_df_lsst_y1 = cosmodc2_df_100k.loc[cosmodc2_df_100k['LSST_filters/magnitude:LSST_i:observed']<=24.1]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "42cc8668-d57d-48cb-9e65-eef4a663c744",
             "metadata": {
@@ -837,16 +740,16 @@
             "execution_count": null,
             "id": "200713a3-f6fd-4c5f-a46a-6f1d3ed92bc6",
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
-                "skysim3_df_lsst_y1 = skysim3_df_lsst_y1_all.sample(n=100000)\n",
-                "cosmodc2_df_lsst_y1 = cosmodc2_df_lsst_y1_all.sample(n=100000)"
+                "#skysim3_df_lsst_y1 = skysim3_df_lsst_y1_all.sample(n=100000)\n",
+                "#cosmodc2_df_lsst_y1 = cosmodc2_df_lsst_y1_all.sample(n=100000)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "a2e2d8bf-cd2c-45b2-97f0-80cde932eb91",
             "metadata": {},
             "source": [
@@ -1492,21 +1395,22 @@
             "source": [
                 "plt.clf()\n",
                 "\n",
                 "plt.rcParams['xtick.labelsize']=15\n",
                 "plt.rcParams['ytick.labelsize']=15\n",
                 "\n",
                 "extents = [(-1.5,4.), (-1.5,4.), (-1.5,4.), (-1.5,4.),(-1.5,4.)]\n",
+                "colours = [r'$(u-g)_{obs}$',r'$(g-r)_{obs}$',r'$(r-i)_{obs}$',r'$(i-z)_{obs}$',r'$(z-y)_{obs}$']\n",
                 "\n",
                 "fig = corner.corner(cosmos2020_colors[:,:5], hist_kwargs=dict(density=True, linewidth=1.5), range=extents,\n",
-                "                    color='blue', labels=colours[:5], label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
+                "                    color='blue', labels=colours, label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
                 "                    plot_datapoints=False, levels=(1-np.exp(-0.5),1-np.exp(-2),1-np.exp(-4.5)), show_titles=False,\n",
                 "                    title_fmt='.4f')\n",
                 "fig = corner.corner(dsps_colors[:,:5], fig=fig, hist_kwargs=dict(density=True, linewidth=1.5), range=extents,\n",
-                "                    color='red', labels=colours[:5], label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
+                "                    color='red', labels=colours, label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
                 "                    plot_datapoints=False, levels=(1-np.exp(-0.5),1-np.exp(-2),1-np.exp(-4.5)), show_titles=False,\n",
                 "                    title_fmt='.4f')\n",
                 "                    \n",
                 "axes = np.array(fig.axes)\n",
                 "proxy = [plt.Rectangle((0,0),1,1,fc = 'blue'), \n",
                 "         plt.Rectangle((0,0),1,1,fc = 'red')]\n",
                 "\n",
@@ -1526,38 +1430,39 @@
             "source": [
                 "plt.clf()\n",
                 "\n",
                 "plt.rcParams['xtick.labelsize']=15\n",
                 "plt.rcParams['ytick.labelsize']=15\n",
                 "\n",
                 "extents = [(-1.5,4.), (-1.5,4.), (-1.5,4.)]\n",
+                "colours = [r'$(y-J)_{obs}$',r'$(J-H)_{obs}$',r'$(H-Ks)_{obs}$']\n",
                 "\n",
                 "fig = corner.corner(cosmos2020_colors[:,5:], hist_kwargs=dict(density=True, linewidth=1.5), range=extents,\n",
-                "                    color='blue', labels=colours[5:], label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
+                "                    color='blue', labels=colours, label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
                 "                    plot_datapoints=False, levels=(1-np.exp(-0.5),1-np.exp(-2),1-np.exp(-4.5)), show_titles=False,\n",
                 "                    title_fmt='.4f')\n",
                 "fig = corner.corner(dsps_colors[:,5:], fig=fig, hist_kwargs=dict(density=True, linewidth=1.5), range=extents,\n",
-                "                    color='red', labels=colours[5:], label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
+                "                    color='red', labels=colours, label_kwargs={\"fontsize\":30}, use_math_text=True,\n",
                 "                    plot_datapoints=False, levels=(1-np.exp(-0.5),1-np.exp(-2),1-np.exp(-4.5)), show_titles=False,\n",
                 "                    title_fmt='.4f')\n",
                 "                    \n",
                 "axes = np.array(fig.axes)\n",
                 "proxy = [plt.Rectangle((0,0),1,1,fc = 'blue'), \n",
                 "         plt.Rectangle((0,0),1,1,fc = 'red')]\n",
                 "\n",
                 "axes[2].legend(proxy, ['COSMOS2020','DSPS from skysim v3.1.0'],loc='upper right',fontsize=20)\n",
                 "plt.show()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "new_rail_env",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
-            "name": "new_rail_env"
+            "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
```

### Comparing `pz_rail-0.99.3/examples/creation_examples/posterior-demo.ipynb` & `pz_rail-1.0.0/examples/creation_examples/posterior-demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9983174312915692%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(5, 'from rail.creation.degraders.lsst_error_model import "*

 * *            "LSSTErrorModel\\n'), (6, 'from rail.creation.degraders.quantityCut import "*

 * *            "QuantityCut\\n'), (7, 'from rail.creation.degraders.spectroscopic_degraders import "*

 * *            "(\\n'), (13, 'from rail.tools.table_tools import ColumnMapper\\n')], delete: [13, 7, "*

 * *            "6, 5]}}, 30: {'source': {insert: [(0, 'from rail.tools.table_tools import "*

 * *            "RowSelector\\n')], delete […]*

```diff
@@ -35,23 +35,23 @@
             "outputs": [],
             "source": [
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "from pzflow.examples import get_example_flow\n",
                 "from rail.creation.engines.flowEngine import FlowCreator, FlowPosterior\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
-                "from rail.creation.degradation.spectroscopic_degraders import (\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.spectroscopic_degraders import (\n",
                 "    InvRedshiftIncompleteness,\n",
                 "    LineConfusion,\n",
                 ")\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.util_stages import ColumnMapper\n"
+                "from rail.tools.table_tools import ColumnMapper\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
@@ -455,15 +455,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.util_stages import RowSelector\n",
+                "from rail.tools.table_tools import RowSelector\n",
                 "\n",
                 "# dict to save the marginalized posteriors\n",
                 "pdfs_u_marginalized = {}\n",
                 "\n",
                 "row3_selector = RowSelector.make_stage(name=\"select_row3\", start=3, stop=4)\n",
                 "row3_degraded = row3_selector(samples_degraded)\n",
                 "\n",
@@ -526,15 +526,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.13"
+            "version": "3.10.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "1cc5b75da6b94fd59f6c7b0992047078a9372d2242c3f23a554e39af5a039534"
             }
         }
     },
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_demo.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/BPZ_lite_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997738921957672%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(9, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -32,15 +32,15 @@
                 "import pickle\n",
                 "import matplotlib.pyplot as plt\n",
                 "import numpy as np\n",
                 "import pandas as pd\n",
                 "import desc_bpz\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "b04c8503-74ee-4de7-b0f7-a2d8d1398db7",
             "metadata": {},
@@ -711,13 +711,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9971210706504825%*

 * *Differences: {"'cells'": "{0: {'id': '404017cc'}, 6: {'source': {insert: [(0, 'from rail.utils.path_utils "*

 * *            "import RAILDIR\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -1,11 +1,12 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
+            "id": "404017cc",
             "metadata": {},
             "source": [
                 "# Running BPZliteEstimator with a custom set of SEDs\n",
                 "\n",
                 "**Authors:** Sam Schmidt\n",
                 "\n",
                 "**Last Successfully Run:** Nov 14, 2023"
@@ -60,15 +61,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "064164cf-c923-4f34-96ba-5549f6b6df10",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "import os\n",
                 "custom_data_path = RAILDIR + '/rail/examples_data/estimation_data/data'\n",
                 "sedpath = RAILDIR + '/rail/examples_data/estimation_data/data/SED'\n",
                 "tarpath = RAILDIR + '/rail/examples_data/estimation_data/data/nonphysical_dc2_templates.tar'\n",
                 "\n",
                 "os.environ['tempbpzsedpath'] = sedpath\n",
                 "os.environ['tempbpztarpath'] = tarpath\n",
@@ -573,13 +574,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/CMNN_Demo.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/CMNN_Demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976453081232493%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(0, 'from rail.utils.path_utils import RAILDIR\\n')], "*

 * *            'delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -136,15 +136,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import RAILDIR\n",
+                "from rail.utils.path_utils import RAILDIR\n",
                 "trainFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = os.path.join(RAILDIR, 'rail/examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
@@ -380,13 +380,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9848857786357786%*

 * *Differences: {"'cells'": "{0: {delete: ['attachments']}, 3: {delete: ['attachments']}, 4: {'source': {insert: "*

 * *            "[(0, 'from rail.utils.path_utils import find_rail_file\\n')], delete: [0]}}, 5: "*

 * *            "{delete: ['attachments']}, 7: {delete: ['attachments']}, 9: {delete: "*

 * *            "['attachments']}, 11: {delete: ['attachments']}, 13: {delete: ['attachments']}, 15: "*

 * *            "{delete: ['attachments']}, 19: {delete: ['attachments']}, 21: {delete: "*

 * *            "['attachments']}, 23: {delete: ['att […]*

```diff
@@ -1,11 +1,10 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "# FlexZBoost PDF Representation Comparison\n",
                 "\n",
                 "**Author:** Drew Oldag\n",
                 "\n",
@@ -39,36 +38,34 @@
             "outputs": [],
             "source": [
                 "DS = RailStage.data_store\n",
                 "DS.__class__.allow_overwrite = True"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Create references to the training and test data."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Define the configurations for the ML model to be trained by Flexcode. Specifically we'll use Xgboost with a set of 35 cosine basis functions."
             ]
         },
         {
@@ -84,15 +81,14 @@
                 "               hdf5_groupname='photometry',\n",
                 "               regression_params={'max_depth': 8,'objective':'reg:squarederror'})\n",
                 "\n",
                 "fz_modelfile = 'demo_FZB_model.pkl'"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Define the RAIL stage to train the model"
             ]
         },
         {
@@ -102,15 +98,14 @@
             "outputs": [],
             "source": [
                 "from rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\n",
                 "inform_pzflex = FlexZBoostInformer.make_stage(name='inform_fzboost', model=fz_modelfile, **fz_dict)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Then we'll run that stage to train the model and store the result in a file name `demo_FZB_model.pkl`."
             ]
         },
         {
@@ -120,15 +115,14 @@
             "outputs": [],
             "source": [
                 "%%time\n",
                 "inform_pzflex.inform(training_data)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we configure the RAIL stage that will evaluate test data using the saved model.\n",
                 "Note that we specify `qp_representation='flexzboost'` here to instruct `rail_flexzboost` to store the model weights using `qp_flexzboost`."
             ]
         },
@@ -141,15 +135,14 @@
                 "pzflex_qp_flexzboost = FlexZBoostEstimator.make_stage(name='fzboost_flexzboost', hdf5_groupname='photometry',\n",
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            output='flexzboost.hdf5',\n",
                 "                            qp_representation='flexzboost')"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we actually evaluate the test data, 20,449 example galaxies, using the trained model, and then print out the size of the file that was saved. \n",
                 "\n",
                 "Note that the final output size will depend on the number of basis functions used by the model. Again, for this experiment, we used 35 basis functions."
             ]
@@ -169,15 +162,14 @@
                 "\n",
                 "fzresults_qp_flexzboost = pzflex_qp_flexzboost.estimate(test_data)\n",
                 "file_size = os.path.getsize(output_file_name)\n",
                 "print(\"File Size is :\", file_size, \"bytes\")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Example calculating median and mode. Note that we're using the `%%timeit` magic command to get an estimate of the time required for calculating `median`, but we're using `%%time` to estimate the `mode`. This is because `qp` will cache the output of the `pdf` function for a given grid. If we used `%%timeit`, then the resulting estimate would average the run time of one non-cached calculation and N-1 cached calculations. "
             ]
         },
         {
@@ -206,15 +198,14 @@
             "outputs": [],
             "source": [
                 "%%time\n",
                 "fz_modes_qp_flexzboost = fzresults_qp_flexzboost().mode(grid=zgrid)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Plotting median values."
             ]
         },
         {
@@ -228,15 +219,14 @@
                 "plt.hist(fz_medians_qp_flexzboost, bins=np.linspace(-.005,3.005,101));\n",
                 "plt.xlabel(\"redshift\")\n",
                 "plt.ylabel(\"Number\")\n",
                 "bins = np.linspace(-5, 5, 11)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Example convertion to a `qp.hist` histogram representation."
             ]
         },
         {
@@ -247,15 +237,14 @@
             "source": [
                 "%%timeit\n",
                 "bins = np.linspace(-5, 5, 11)\n",
                 "fzresults_qp_flexzboost().convert_to(qp.hist_gen, bins=bins)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Now we'll repeat the experiment using `qp.interp` storage. Again, we'll define the RAIL stage to evaluate the test data using the saved model, but instruct `rail_flexzboost` to store the output as x,y interpolated values using `qp.interp`."
             ]
         },
         {
@@ -268,15 +257,14 @@
                 "                            model=inform_pzflex.get_handle('model'),\n",
                 "                            output='interp.hdf5',\n",
                 "                            qp_representation='interp',\n",
                 "                            calculated_point_estimates=[])"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Finally we evaluate the test data again using the trained model, and then print out the size of the file that was saved using the x,y interpolated technique.\n",
                 "\n",
                 "The final file size will depend on the size of the x grid that defines the interpolation. However, we can see that in order to match the storage requirements of `qp_flexzboost`, the x grid would need to be smaller than the number of basis functions used by the model. For this experiment, we used 35 basis functions."
             ]
@@ -296,15 +284,14 @@
                 "\n",
                 "fzresults_qp_interp = pzflex_qp_interp.estimate(test_data)\n",
                 "file_size = os.path.getsize(output_file_name)\n",
                 "print(\"File Size is :\", file_size, \"bytes\")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Example calculating median and mode. Note that we're using the `%%timeit` magic command to get an estimate of the time required for calculating `median`, but we're using `%%time` to estimate the `mode`. This is because `qp` will cache the output of the `pdf` function for a given grid. If we used `%%timeit`, then the resulting estimate would average the run time of one non-cached calculation and N-1 cached calculations."
             ]
         },
         {
@@ -333,15 +320,14 @@
             "outputs": [],
             "source": [
                 "%%time\n",
                 "fz_modes_qp_interp = fzresults_qp_interp().mode(grid=zgrid)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Plotting median values."
             ]
         },
         {
@@ -353,15 +339,14 @@
                 "fz_medians_qp_interp = fzresults_qp_interp().median()\n",
                 "plt.hist(fz_medians_qp_interp, bins=np.linspace(-.005,3.005,101));\n",
                 "plt.xlabel(\"redshift\")\n",
                 "plt.ylabel(\"Number\")"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Example convertion to a `qp.hist` histogram representation."
             ]
         },
         {
@@ -372,15 +357,14 @@
             "source": [
                 "%%timeit\n",
                 "bins = np.linspace(-5, 5, 11)\n",
                 "fzresults_qp_interp().convert_to(qp.hist_gen, bins=bins)"
             ]
         },
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "We'll clean up the files that were produced: the model pickle file, and the output data file. "
             ]
         },
         {
@@ -422,15 +406,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         },
         "vscode": {
             "interpreter": {
                 "hash": "47c0d775efeae3192041035019ca2d946443ef986557562adbc143cc5fa38455"
             }
         }
     },
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/GPz_estimation_example.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/GPz_estimation_example.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976190476190476%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [1]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -57,15 +57,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "631b2b33-c93b-41b8-b3be-a526418f0f57",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# find_rail_file is a convenience function that finds a file in the RAIL ecosystem   We have several example data files that are copied with RAIL that we can use for our example run, let's grab those files, one for training/validation, and the other for testing:\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
@@ -242,13 +242,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/NZDir.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/NZDir.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973137973137973%*

 * *Differences: {"'cells'": "{7: {'source': {insert: [(0, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            "delete: [0]}}, 23: {'source': {insert: [(4, 'Let\\'s import the necessary modules "*

 * *            'from rail.creation.degraders, we will put in "line confusion" for 5% of our sample, '*

 * *            "and then cut the sample at magnitude 23.5:')], delete: [4]}}, 24: {'source': {insert: "*

 * *            "[(0, 'from rail.creation.degraders.spectroscopic_degraders import LineConfusion\\n'), "*

 * *            " […]*

```diff
@@ -82,15 +82,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "f4d40906-f918-4a97-bf33-c6cb4c5e1614",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -281,26 +281,26 @@
             "id": "0e803663-7e59-4ee0-9afc-2c50be21dee3",
             "metadata": {},
             "source": [
                 "## Non-representative data\n",
                 "\n",
                 "That looks very nice, while there is a little bit of \"slosh\" outside of each bin, we have a relatively compact and accurate representation from the DIR method!  This makes sense, as our training and test data are drawn from the same underlying distribution (in this case cosmoDC2_v1.1.4).  However, how will things look if we are missing chunks of data, or have incorrect redshifts in our spec-z sample?  We can use RAIL's degradation modules to do just that: place incorrect redshifts for percentage of the training data, and we can make a magnitude cut that will limite the redshift and color range of our training data: <br>\n",
                 "\n",
-                "Let's import the necessary modules from rail.creation.degradation, we will put in \"line confusion\" for 5% of our sample, and then cut the sample at magnitude 23.5:"
+                "Let's import the necessary modules from rail.creation.degraders, we will put in \"line confusion\" for 5% of our sample, and then cut the sample at magnitude 23.5:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "ca0e32a2-622f-4d2a-b73e-480117c2cf17",
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.creation.degradation.spectroscopic_degraders import LineConfusion\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.spectroscopic_degraders import LineConfusion\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
                 "from rail.core.data import PqHandle"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "7f7ca3e9-75e6-48bd-843f-8ad415a7188a",
@@ -480,13 +480,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/RAIL_estimation_demo.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/RAIL_estimation_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9976810515873016%*

 * *Differences: {"'cells'": "{15: {'source': {insert: [(0, 'from rail.utils.path_utils import "*

 * *            "find_rail_file\\n')], delete: [0]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -167,15 +167,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
@@ -532,13 +532,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.6"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/README.md` & `pz_rail-1.0.0/examples/estimation_examples/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme` & `pz_rail-1.0.0/examples/estimation_examples/SimpleSOM_demo.ipynb.fixme`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999968998015873%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(10, 'from rail.utils.path_utils import RAILDIR')], delete: "*

 * *            '[10]}}}'}*

```diff
@@ -42,15 +42,15 @@
                 "import rail\n",
                 "import qp\n",
                 "import os\n",
                 "import tables_io\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
                 "from minisom import MiniSom\n",
-                "from rail.core.utils import RAILDIR"
+                "from rail.utils.path_utils import RAILDIR"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "7ab63889",
             "metadata": {},
             "source": [
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/nzdir_as_pipeline.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/nzdir_as_pipeline.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975818452380952%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(1, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [1]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -46,15 +46,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "8a682c95",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load up the example healpix 9816 data and stick in the DataStore\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
@@ -199,13 +199,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/somocluSOM_demo.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/somocluSOM_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984803391053392%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(9, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [9]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -43,15 +43,15 @@
                 "import pickle\n",
                 "import rail\n",
                 "import os\n",
                 "import qp\n",
                 "import tables_io\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import find_rail_file\n"
+                "from rail.utils.path_utils import find_rail_file\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "6c3e1005",
             "metadata": {},
             "source": [
@@ -763,15 +763,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/somocluSOMcluster_demo.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/somocluSOMcluster_demo.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984886532738095%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(10, 'from rail.utils.path_utils import "*

 * *            "find_rail_file\\n')], delete: [10]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -45,15 +45,15 @@
                 "import pickle\n",
                 "import rail\n",
                 "import os\n",
                 "import qp\n",
                 "import tables_io\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "from rail.estimation.algos.somoclu_som import SOMocluInformer, SOMocluSummarizer\n",
                 "from rail.estimation.algos.somoclu_som import get_bmus, plot_som"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "31350a6b",
@@ -883,15 +883,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `pz_rail-0.99.3/examples/estimation_examples/test_sampled_summarizers.ipynb` & `pz_rail-1.0.0/examples/estimation_examples/test_sampled_summarizers.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977190671350508%*

 * *Differences: {"'cells'": "{10: {'source': {insert: [(1, 'from rail.utils.path_utils import "*

 * *            "find_rail_file\\n')], delete: [1]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -117,15 +117,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "0ecdeb24-b5d9-4985-8968-a87158a53757",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Load up the example healpix 9816 data and stick in the DataStore\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "trainFile = find_rail_file('examples_data/testdata/test_dc2_training_9816.hdf5')\n",
                 "testFile = find_rail_file('examples_data/testdata/test_dc2_validation_9816.hdf5')\n",
                 "training_data = DS.read_file(\"training_data\", TableHandle, trainFile)\n",
                 "test_data = DS.read_file(\"test_data\", TableHandle, testFile)"
             ]
         },
         {
@@ -669,13 +669,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/evaluation_examples/Evaluation_Demo.ipynb` & `pz_rail-1.0.0/examples/evaluation_examples/Evaluation_Demo.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977322446072446%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(0, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -89,15 +89,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "try:\n",
                 "    pdfs_file = find_rail_file('examples_data/evaluation_data/data/output_fzboost.hdf5')\n",
                 "except ValueError:\n",
                 "    pdfs_file = 'examples_data/evaluation_data/data/output_fzboost.hdf5'\n",
                 "    try:\n",
                 "        os.makedirs(os.path.dirname(pdfs_file))\n",
                 "    except FileExistsError:\n",
@@ -560,13 +560,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/evaluation_examples/Evaluation_by_type.ipynb` & `pz_rail-1.0.0/examples/evaluation_examples/Evaluation_by_type.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9977480786618445%*

 * *Differences: {"'cells'": "{4: {'source': {insert: [(1, 'from rail.utils.path_utils import find_rail_file\\n')], "*

 * *            'delete: [1]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.10.0'}}"}*

```diff
@@ -57,15 +57,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "from rail.core.utils import find_rail_file\n",
+                "from rail.utils.path_utils import find_rail_file\n",
                 "possible_local_file = './examples_data/evaluation_data/data/output_fzboost.hdf5'\n",
                 "if os.path.exists(possible_local_file):\n",
                 "    pdfs_file = os.path.abspath(possible_local_file)\n",
                 "else:\n",
                 "    pdfs_file = 'examples_data/evaluation_data/data/output_fzboost.hdf5'\n",
                 "    try:\n",
                 "        os.makedirs(os.path.dirname(pdfs_file))\n",
@@ -906,13 +906,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pz_rail-0.99.3/examples/evaluation_examples/utils.py` & `pz_rail-1.0.0/examples/evaluation_examples/utils.py`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/goldenspike_examples/README.md` & `pz_rail-1.0.0/examples/goldenspike_examples/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 This directory contains an example notebook showing a simplified version of the end-to-end functionality of RAIL.
 
-- [goldenspike.ipynb](https://lsstdescrail.readthedocs.io/en/latest/source/other-notebooks.html#goldenspike-an-example-of-an-end-to-end-analysis-using-rail) is a notebook that chains together the functionality of the creation, estimation, and evaluation modules.
+- [goldenspike.ipynb](https://rail-hub.readthedocs.io/projects/rail-notebooks/en/latest/rendered/goldenspike_examples/goldenspike.html) is a notebook that chains together the functionality of the creation, estimation, and evaluation modules.
 
 - `goldenspike.yml`, a pipeline file (plus `goldenspike_config.yml`, its associated config file).
 
 ---
  
   To run the pipeline file from the command line, you must:
  - `cd` to your `rail/` directory
```

### Comparing `pz_rail-0.99.3/examples/goldenspike_examples/cleanup.sh` & `pz_rail-1.0.0/examples/goldenspike_examples/cleanup.sh`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.ipynb` & `pz_rail-1.0.0/examples/goldenspike_examples/goldenspike.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9886556876823558%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(4, 'from collections import OrderedDict\\n')]}}, 4: "*

 * *            "{'source': {insert: [(2, 'from rail.creation.degraders.lsst_error_model import "*

 * *            "LSSTErrorModel\\n'), (3, 'from rail.creation.degraders.spectroscopic_degraders import "*

 * *            "(\\n'), (7, 'from rail.creation.degraders.quantityCut import QuantityCut\\n'), (11, "*

 * *            "'from rail.tools.table_tools import ColumnMapper, TableConverter\\n'), (20, 'from "*

 * *            "rail.evaluation […]*

```diff
@@ -56,46 +56,48 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Prerquisites: os, numpy, pathlib, pzflow, tables_io\n",
                 "import os\n",
                 "import numpy as np\n",
                 "from pathlib import Path\n",
+                "from collections import OrderedDict\n",
                 "from pzflow.examples import get_galaxy_data\n",
                 "import tables_io\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "material-funeral",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Various rail modules\n",
                 "import rail\n",
-                "from rail.creation.degradation.lsst_error_model import LSSTErrorModel\n",
-                "from rail.creation.degradation.spectroscopic_degraders import (\n",
+                "from rail.creation.degraders.lsst_error_model import LSSTErrorModel\n",
+                "from rail.creation.degraders.spectroscopic_degraders import (\n",
                 "    InvRedshiftIncompleteness,\n",
                 "    LineConfusion,\n",
                 ")\n",
-                "from rail.creation.degradation.quantityCut import QuantityCut\n",
+                "from rail.creation.degraders.quantityCut import QuantityCut\n",
                 "from rail.creation.engines.flowEngine import FlowModeler, FlowCreator, FlowPosterior\n",
                 "from rail.core.data import TableHandle\n",
                 "from rail.core.stage import RailStage\n",
-                "from rail.core.util_stages import ColumnMapper, TableConverter\n",
+                "from rail.tools.table_tools import ColumnMapper, TableConverter\n",
                 "\n",
                 "from rail.estimation.algos.bpz_lite import BPZliteInformer, BPZliteEstimator\n",
                 "from rail.estimation.algos.k_nearneigh import KNearNeighInformer, KNearNeighEstimator\n",
                 "from rail.estimation.algos.flexzboost import FlexZBoostInformer, FlexZBoostEstimator\n",
                 "\n",
                 "from rail.estimation.algos.naive_stack import NaiveStackSummarizer\n",
                 "from rail.estimation.algos.point_est_hist import PointEstHistSummarizer\n",
                 "\n",
-                "from rail.evaluation.evaluator import OldEvaluator\n"
+                "from rail.evaluation.dist_to_point_evaluator import DistToPointEvaluator\n",
+                "\n"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "scheduled-chamber",
             "metadata": {},
             "source": [
@@ -279,14 +281,15 @@
                 ")\n",
                 "\n",
                 "line_confusion = LineConfusion.make_stage(\n",
                 "    name=\"line_confusion\",\n",
                 "    true_wavelen=5007.0,\n",
                 "    wrong_wavelen=3727.0,\n",
                 "    frac_wrong=0.05,\n",
+                "    seed = 1337\n",
                 ")\n",
                 "\n",
                 "quantity_cut = QuantityCut.make_stage(\n",
                 "    name=\"quantity_cut\",\n",
                 "    cuts={\"mag_i_lsst\": 25.0},\n",
                 ")\n",
                 "\n",
@@ -411,14 +414,37 @@
                 "test_data_pq = col_remapper_test(test_data_errs)\n",
                 "test_data = table_conv_test(test_data_pq)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "eb3b5698-6f44-4f93-a2a4-f817a68026b2",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "test_data_handle = TableHandle('input')\n",
+                "od = OrderedDict()\n",
+                "od['photometry'] = test_data_orig.data.to_records()\n",
+                "test_data_handle.set_data(od)\n",
+                "test_data_handle.path  = './test_data_orig.hdf5'\n",
+                "test_data_handle.write()"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "58e17656-a898-42b9-a809-7a6f32638990",
+            "metadata": {},
+            "outputs": [],
+            "source": []
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "inclusive-effect",
             "metadata": {},
             "outputs": [],
             "source": [
                 "test_table = tables_io.convertObj(test_data.data, tables_io.types.PD_DATAFRAME)\n",
                 "test_table.head()\n"
             ]
@@ -555,25 +581,58 @@
                 "Each call to the `Evaluator.evaluate` will create a table with the various performance metrics. \n",
                 "We will store all of these tables in a dictionary, keyed by the name of the estimator."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "id": "4f4b8b5a-3f5d-4192-b258-e35a2f0e5d4a",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ztrue_file = './test_data_orig.hdf5'\n",
+                "ztrue_data = DS.read_file('ztrue_data', TableHandle, ztrue_file)\n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "id": "portuguese-graduate",
             "metadata": {},
             "outputs": [],
             "source": [
                 "eval_dict = dict(bpz=bpz_estimated, fzboost=fzboost_estimated, knn=knn_estimated)\n",
-                "truth = test_data_orig\n",
+                "\n",
+                "evaluator_stage_dict = dict(\n",
+                "    metrics=['cdeloss', 'pit', 'brier'],\n",
+                "    _random_state=None,\n",
+                "    metric_config={\n",
+                "        'brier': {'limits':(0,3.1)},\n",
+                "        'pit':{'tdigest_compression': 1000},\n",
+                "    }\n",
+                ")\n",
+                "truth = ztrue_data\n",
                 "\n",
                 "result_dict = {}\n",
                 "for key, val in eval_dict.items():\n",
-                "    the_eval = OldEvaluator.make_stage(name=f\"{key}_eval\", truth=truth)\n",
-                "    result_dict[key] = the_eval.evaluate(val, truth)\n"
+                "    the_eval = DistToPointEvaluator.make_stage(name=f'{key}_dist_to_point', force_exact=True, **evaluator_stage_dict)\n",
+                "    result_dict[key] = the_eval.evaluate(val, truth)\n",
+                "    \n",
+                "    \n",
+                "    \n"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "093c617a-b862-47c3-ad38-20de5d44cfb4",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "result_dict"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "danish-miller",
             "metadata": {},
             "source": [
@@ -585,15 +644,15 @@
             "cell_type": "code",
             "execution_count": null,
             "id": "constant-peripheral",
             "metadata": {},
             "outputs": [],
             "source": [
                 "results_tables = {\n",
-                "    key: tables_io.convertObj(val.data, tables_io.types.PD_DATAFRAME)\n",
+                "    key: tables_io.convertObj(val['summary'].data, tables_io.types.PD_DATAFRAME)\n",
                 "    for key, val in result_dict.items()\n",
                 "}\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -790,15 +849,17 @@
                 "Finally, you'll notice that we've written a large number of temporary files in the course of running this demo, to delete these and clean up the directory just run the `cleanup.sh` script in this directory to delete the data files."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "racial-stocks",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "# TODO fix and add clean up scripts\n"
             ]
         }
     ],
     "metadata": {
@@ -813,13 +874,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.10.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike.yml` & `pz_rail-1.0.0/examples/goldenspike_examples/goldenspike.yml`

 * *Files 11% similar despite different names*

```diff
@@ -14,51 +14,51 @@
   name: flow_modeler
   nprocess: 1
 - classname: FlowCreator
   module_name: rail.creation.engines.flowEngine
   name: flow_creator_train
   nprocess: 1
 - classname: LSSTErrorModel
-  module_name: rail.creation.degradation.lsst_error_model
+  module_name: rail.creation.degraders.lsst_error_model
   name: lsst_error_model_train
   nprocess: 1
 - classname: InvRedshiftIncompleteness
-  module_name: rail.creation.degradation.spectroscopic_degraders
+  module_name: rail.creation.degraders.spectroscopic_degraders
   name: inv_redshift
   nprocess: 1
 - classname: LineConfusion
-  module_name: rail.creation.degradation.spectroscopic_degraders
+  module_name: rail.creation.degraders.spectroscopic_degraders
   name: line_confusion
   nprocess: 1
 - classname: QuantityCut
-  module_name: rail.creation.degradation.quantityCut
+  module_name: rail.creation.degraders.quantityCut
   name: quantity_cut
   nprocess: 1
 - classname: ColumnMapper
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: col_remapper_train
   nprocess: 1
 - classname: TableConverter
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: table_conv_train
   nprocess: 1
 - classname: FlowCreator
   module_name: rail.creation.engines.flowEngine
   name: flow_creator_test
   nprocess: 1
 - classname: LSSTErrorModel
-  module_name: rail.creation.degradation.lsst_error_model
+  module_name: rail.creation.degraders.lsst_error_model
   name: lsst_error_model_test
   nprocess: 1
 - classname: ColumnMapper
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: col_remapper_test
   nprocess: 1
 - classname: TableConverter
-  module_name: rail.core.utilStages
+  module_name: rail.tools.table_tools
   name: table_conv_test
   nprocess: 1
 - classname: BPZliteInformer
   module_name: rail.estimation.algos.bpz_lite
   name: inform_bpz
   nprocess: 1
 - classname: KNearNeighInformer
```

### Comparing `pz_rail-0.99.3/examples/goldenspike_examples/goldenspike_config.yml` & `pz_rail-1.0.0/examples/goldenspike_examples/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/pyproject.toml` & `pz_rail-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail-0.99.3/src/pz_rail.egg-info/PKG-INFO` & `pz_rail-1.0.0/src/pz_rail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail
-Version: 0.99.3
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail-0.99.3/src/pz_rail.egg-info/SOURCES.txt` & `pz_rail-1.0.0/src/pz_rail.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 examples/creation_examples/cleanup.sh
 examples/creation_examples/degradation-demo.ipynb
 examples/creation_examples/dsps_sed_demo.ipynb
 examples/creation_examples/example_GridSelection_for_HSC.ipynb
 examples/creation_examples/example_ObsConditions.ipynb
 examples/creation_examples/example_SpecSelection_for_zCOSMOS.ipynb
 examples/creation_examples/fsps_sed_demo.ipynb
+examples/creation_examples/photerr_demo.ipynb
 examples/creation_examples/photometric_realization_demo.ipynb
 examples/creation_examples/plotting_interface_skysim_cosmoDC2_COSMOS2020_demo.ipynb
 examples/creation_examples/posterior-demo.ipynb
 examples/estimation_examples/BPZ_lite_demo.ipynb
 examples/estimation_examples/BPZ_lite_with_custom_SEDs.ipynb
 examples/estimation_examples/CMNN_Demo.ipynb
 examples/estimation_examples/Fzboost_PDF_Representation_Comparison.ipynb
```

