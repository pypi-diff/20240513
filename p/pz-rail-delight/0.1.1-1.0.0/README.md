# Comparing `tmp/pz_rail_delight-0.1.1.tar.gz` & `tmp/pz_rail_delight-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_delight-0.1.1.tar", last modified: Wed May  8 15:54:43 2024, max compression
+gzip compressed data, was "pz_rail_delight-1.0.0.tar", last modified: Mon May 13 20:03:09 2024, max compression
```

## Comparing `pz_rail_delight-0.1.1.tar` & `pz_rail_delight-1.0.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.433392 pz_rail_delight-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.421392 pz_rail_delight-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.421392 pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.421392 pz_rail_delight-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-08 15:54:43.433392 pz_rail_delight-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:54:43.433392 pz_rail_delight-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.433392 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.421392 pz_rail_delight-0.1.1/src/rail/delight/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/delight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 15:54:43.000000 pz_rail_delight-0.1.1/src/rail/delight/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.421392 pz_rail_delight-0.1.1/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/estimation/algos/delight_hybrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.425392 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g_gaussian_coefficients.txt
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i_gaussian_coefficients.txt
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r_gaussian_coefficients.txt
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u_gaussian_coefficients.txt
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y_gaussian_coefficients.txt
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z_gaussian_coefficients.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.429392 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008_fluxredshiftmod.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
--rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008_fluxredshiftmod.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.417392 pz_rail_delight-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:54:43.429392 pz_rail_delight-0.1.1/tests/delight/
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/tests/delight/delightPZ.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-08 15:54:36.000000 pz_rail_delight-0.1.1/tests/delight/test_algos.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.115077 pz_rail_delight-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.115077 pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.115077 pz_rail_delight-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-13 20:03:09.000000 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-05-13 20:03:09.000000 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:03:09.000000 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-13 20:03:09.000000 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 20:03:09.000000 pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.119077 pz_rail_delight-1.0.0/src/rail/delight/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/delight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 20:03:08.000000 pz_rail_delight-1.0.0/src/rail/delight/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.119077 pz_rail_delight-1.0.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/estimation/algos/delight_hybrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.119077 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g_gaussian_coefficients.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i_gaussian_coefficients.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r_gaussian_coefficients.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u_gaussian_coefficients.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y_gaussian_coefficients.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z_gaussian_coefficients.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008_fluxredshiftmod.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+-rw-r--r--   0 runner    (1001) docker     (127)    45000 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008_fluxredshiftmod.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.111077 pz_rail_delight-1.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:03:09.127077 pz_rail_delight-1.0.0/tests/delight/
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/tests/delight/delightPZ.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 20:03:02.000000 pz_rail_delight-1.0.0/tests/delight/test_algos.py
```

### Comparing `pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz_rail_delight-1.0.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/pull_request_template.md` & `pz_rail_delight-1.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/workflows/linting.yml` & `pz_rail_delight-1.0.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_delight-1.0.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/workflows/smoke-test.yml` & `pz_rail_delight-1.0.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_delight-1.0.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.gitignore` & `pz_rail_delight-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/.pre-commit-config.yaml` & `pz_rail_delight-1.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/LICENSE` & `pz_rail_delight-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/PKG-INFO` & `pz_rail_delight-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-delight
-Version: 0.1.1
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_delight-0.1.1/README.md` & `pz_rail_delight-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/pyproject.toml` & `pz_rail_delight-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/PKG-INFO` & `pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-delight
-Version: 0.1.1
+Version: 1.0.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_delight-0.1.1/src/pz_rail_delight.egg-info/SOURCES.txt` & `pz_rail_delight-1.0.0/src/pz_rail_delight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/estimation/algos/delight_hybrid.py` & `pz_rail_delight-1.0.0/src/rail/estimation/algos/delight_hybrid.py`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z_gaussian_coefficients.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z_gaussian_coefficients.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008_fluxredshiftmod.txt` & `pz_rail_delight-1.0.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008_fluxredshiftmod.txt`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/tests/delight/delightPZ.yaml` & `pz_rail_delight-1.0.0/tests/delight/delightPZ.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_delight-0.1.1/tests/delight/test_algos.py` & `pz_rail_delight-1.0.0/tests/delight/test_algos.py`

 * *Files identical despite different names*

