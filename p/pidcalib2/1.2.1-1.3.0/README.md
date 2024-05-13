# Comparing `tmp/pidcalib2-1.2.1.tar.gz` & `tmp/pidcalib2-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-3s3n37xq/pidcalib2-1.2.1.tar", last modified: Sun Mar 17 20:20:39 2024, max compression
+gzip compressed data, was "/builds/lhcb-rta/pidcalib2/dist/.tmp-6zdby1x9/pidcalib2-1.3.0.tar", last modified: Mon May 13 09:49:26 2024, max compression
```

## Comparing `pidcalib2-1.2.1.tar` & `pidcalib2-1.3.0.tar`

### file list

```diff
@@ -1,75 +1,89 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)       69 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.coveragerc
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     2267 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2266 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      691 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)    18151 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.pylintrc
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/.sourcery.yaml
--rw-rw-rw-   0 root         (0) root         (0)    35065 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15428 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    14817 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)    15142 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/notebooks/plots.ipynb
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/requirements-ci.txt
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1173 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     5737 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/aliases.py
--rw-rw-rw-   0 root         (0) root         (0)     3339 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/argparse_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     9884 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/data/
--rw-rw-rw-   0 root         (0) root         (0)   822144 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/data/samples.json
--rw-rw-rw-   0 root         (0) root         (0)     9362 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/make_eff_hists.py
--rw-rw-rw-   0 root         (0) root         (0)     3996 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/markdown_table.py
--rw-rw-rw-   0 root         (0) root         (0)     3496 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/merge_trees.py
--rw-rw-rw-   0 root         (0) root         (0)    17721 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/pid_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6754 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/pklhisto2root.py
--rw-rw-rw-   0 root         (0) root         (0)    15528 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/plot_calib_distributions.py
--rw-rw-rw-   0 root         (0) root         (0)     9937 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/ref_calib.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/samples.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/tests/
--rw-rw-rw-   0 root         (0) root         (0)       57 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_binning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/
--rw-rw-rw-   0 root         (0) root         (0)     9898 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/cal_test_data.csv
--rw-rw-rw-   0 root         (0) root         (0)     5653 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/cal_test_data.pkl
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/custom_binning.json
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
--rw-rw-rw-   0 root         (0) root         (0)    36807 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
--rw-rw-rw-   0 root         (0) root         (0)     2556 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
--rw-rw-rw-   0 root         (0) root         (0)      865 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
--rw-rw-rw-   0 root         (0) root         (0)     2507 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-test-down-Pi-DLLK>4-P.pkl
--rw-rw-rw-   0 root         (0) root         (0)    20907 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_PID_eff.root
--rw-rw-rw-   0 root         (0) root         (0)     8045 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data.csv
--rw-rw-rw-   0 root         (0) root         (0)     9244 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data.root
--rw-rw-rw-   0 root         (0) root         (0)     9817 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/sweights_2023/
--rw-rw-rw-   0 root         (0) root         (0)  2143759 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/sweights_2023/00199935_00000001_1.pid_tuple_sweights.root
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/test_file_list
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_data/test_samples.json
--rw-rw-rw-   0 root         (0) root         (0)    10655 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_make_eff_hist.py
--rw-rw-rw-   0 root         (0) root         (0)     4109 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_merge_trees.py
--rw-rw-rw-   0 root         (0) root         (0)     8095 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_pid_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2549 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_pklhisto2root.py
--rw-rw-rw-   0 root         (0) root         (0)     5475 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_plot_calib_distributions.py
--rw-rw-rw-   0 root         (0) root         (0)     4097 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_ref_calib.py
--rw-rw-rw-   0 root         (0) root         (0)     4597 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    27903 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/src/pidcalib2/utils.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15428 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2212 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      305 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      103 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/src/pidcalib2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-17 20:20:39.000000 pidcalib2-1.2.1/typings/
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-03-17 20:19:57.000000 pidcalib2-1.2.1/typings/ROOT.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.coveragerc
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2267 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      691 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    18151 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/.sourcery.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    35065 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15428 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    14817 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)   202824 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/2023_Examples.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/notebooks/example_hists/
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-K-(DLLp-DLLK)>15-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-K-(DLLp-DLLK)>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-K-DLLK>0-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-K-DLLK>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2523 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-P-(DLLp-DLLK)>15-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2521 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-P-(DLLp-DLLK)>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-P-DLLp>15-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-P-DLLp>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-Pi-DLLK>0-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-Pi-DLLK>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2509 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-Pi-DLLp>15-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/example_hists/effhists-2023-down-Pi-DLLp>5-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)    15142 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/notebooks/plots.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/requirements-ci.txt
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2/
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5953 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/aliases.py
+-rw-rw-rw-   0 root         (0) root         (0)     3339 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/argparse_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9884 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2/data/
+-rw-rw-rw-   0 root         (0) root         (0)   823183 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/data/samples.json
+-rw-rw-rw-   0 root         (0) root         (0)     9362 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/make_eff_hists.py
+-rw-rw-rw-   0 root         (0) root         (0)     3996 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/markdown_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     3496 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/merge_trees.py
+-rw-rw-rw-   0 root         (0) root         (0)    17721 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/pid_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6754 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/pklhisto2root.py
+-rw-rw-rw-   0 root         (0) root         (0)    15664 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/plot_calib_distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9937 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/ref_calib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/samples.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_binning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/
+-rw-rw-rw-   0 root         (0) root         (0)     9898 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/cal_test_data.csv
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/cal_test_data.pkl
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/custom_binning.json
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)    36807 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2556 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)      865 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)     2507 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-test-down-Pi-DLLK>4-P.pkl
+-rw-rw-rw-   0 root         (0) root         (0)    20907 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_PID_eff.root
+-rw-rw-rw-   0 root         (0) root         (0)     8045 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data.csv
+-rw-rw-rw-   0 root         (0) root         (0)     9244 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data.root
+-rw-rw-rw-   0 root         (0) root         (0)     9817 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data_subdir.root
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/sweights_2023/
+-rw-rw-rw-   0 root         (0) root         (0)  2143759 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/sweights_2023/00199935_00000001_1.pid_tuple_sweights.root
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/test_file_list
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_data/test_samples.json
+-rw-rw-rw-   0 root         (0) root         (0)    10655 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_make_eff_hist.py
+-rw-rw-rw-   0 root         (0) root         (0)     4109 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_merge_trees.py
+-rw-rw-rw-   0 root         (0) root         (0)     8095 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_pid_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2549 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_pklhisto2root.py
+-rw-rw-rw-   0 root         (0) root         (0)     5475 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_plot_calib_distributions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_ref_calib.py
+-rw-rw-rw-   0 root         (0) root         (0)     4597 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/tests/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    28539 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/src/pidcalib2/utils.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-13 09:49:25.000000 pidcalib2-1.3.0/src/pidcalib2/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15428 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      305 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/src/pidcalib2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:49:26.000000 pidcalib2-1.3.0/typings/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-13 09:48:09.000000 pidcalib2-1.3.0/typings/ROOT.pyi
```

### Comparing `pidcalib2-1.2.1/.gitignore` & `pidcalib2-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/.gitlab-ci.yml` & `pidcalib2-1.3.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/.pre-commit-config.yaml` & `pidcalib2-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/.pylintrc` & `pidcalib2-1.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/LICENSE` & `pidcalib2-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/PKG-INFO` & `pidcalib2-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.2.1
+Version: 1.3.0
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pidcalib2-1.2.1/README.md` & `pidcalib2-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/notebooks/plots.ipynb` & `pidcalib2-1.3.0/notebooks/plots.ipynb`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/pyproject.toml` & `pidcalib2-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/requirements-dev.txt` & `pidcalib2-1.3.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/setup.cfg` & `pidcalib2-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/setup.py` & `pidcalib2-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/__init__.py` & `pidcalib2-1.3.0/src/pidcalib2/__init__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/__main__.py` & `pidcalib2-1.3.0/src/pidcalib2/__main__.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/aliases.py` & `pidcalib2-1.3.0/src/pidcalib2/aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,8 +113,15 @@
     "TRACK_GHOSTPROB": "{}_GHOSTPROB",
     "PROBNN_D": "{}_PROBNN_D",
     "PROBNN_E": "{}_PROBNN_E",
     "PROBNN_K": "{}_PROBNN_K",
     "PROBNN_MU": "{}_PROBNN_MU",
     "PROBNN_P": "{}_PROBNN_P",
     "PROBNN_PI": "{}_PROBNN_PI",
+    "IPCHI2": "{}_MINIPCHI2",
+    "TRCHI2NDOF": "{}_TCHI2DOF",
+    "nTracks": "nTracks",
+    "nMuonTracks": "nMuonTracks",
+    "RUNNUMBER": "RUNNUMBER",
+    "nRich1Hits": "nRich1Hits",
+    "nRich2Hits": "nRich2Hits"
 }
```

### Comparing `pidcalib2-1.2.1/src/pidcalib2/argparse_tools.py` & `pidcalib2-1.3.0/src/pidcalib2/argparse_tools.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/binning.py` & `pidcalib2-1.3.0/src/pidcalib2/binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/data/samples.json` & `pidcalib2-1.3.0/src/pidcalib2/data/samples.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953609986504725%*

 * *Differences: {"'2023-MagDown-K'": "{'files': {insert: [(5, "*

 * *                     "'root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000006_1.pid_tuple.root')]}, "*

 * *                     "'sweight_dir': "*

 * *                     "'root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/DstToD0Pi_D0ToKPi/2023_full/K/'}",*

 * * "'2023-MagDown-P'": "OrderedDict([('files', "*

 * *                     "['root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/anaprod/lhcb/LHCb/Collisio […]*

```diff
@@ -749,37 +749,55 @@
     },
     "2023-MagDown-K": {
         "files": [
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000001_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000002_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000003_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000004_1.pid_tuple.root",
-            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000005_1.pid_tuple.root"
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000005_1.pid_tuple.root",
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000006_1.pid_tuple.root"
         ],
         "probe_prefix": "K",
-        "sweight_dir": "root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/DstToD0Pi_D0ToKPi/K/",
+        "sweight_dir": "root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/DstToD0Pi_D0ToKPi/2023_full/K/",
         "tuple_names": {
             "K": [
                 "DstToD0Pi_D0ToKPi"
             ],
             "Pi": [
                 "DstToD0Pi_D0ToKPi"
             ]
         }
     },
+    "2023-MagDown-P": {
+        "files": [
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/anaprod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00220504/0000/00220504_00000001_1.pid_tuple.root",
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/anaprod/lhcb/LHCb/Collision23/PID_TUPLE.ROOT/00220504/0000/00220504_00000002_1.pid_tuple.root"
+        ],
+        "probe_prefix": "p",
+        "sweight_dir": "root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/Collision23/L0ToPPi/",
+        "tuple_names": {
+            "P": [
+                "L0ToPPi_LL_LowPT",
+                "L0ToPPi_LL_MidPT",
+                "L0ToPPi_LL_HighPT",
+                "L0ToPPi_LL_VeryHighPT"
+            ]
+        }
+    },
     "2023-MagDown-Pi": {
         "files": [
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000001_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000002_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000003_1.pid_tuple.root",
             "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000004_1.pid_tuple.root",
-            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000005_1.pid_tuple.root"
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000005_1.pid_tuple.root",
+            "root://eoslhcb.cern.ch//eos/lhcb/grid/prod/lhcb/LHCb//Collision23/PID_TUPLE.ROOT/00199935/0000/00199935_00000006_1.pid_tuple.root"
         ],
         "probe_prefix": "pi",
-        "sweight_dir": "root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/DstToD0Pi_D0ToKPi/Pi/",
+        "sweight_dir": "root://eoslhcb.cern.ch//eos/lhcb/wg/rta/WP4/PIDCalib2_sWeights/DstToD0Pi_D0ToKPi/2023_full/Pi/",
         "tuple_names": {
             "K": [
                 "DstToD0Pi_D0ToKPi"
             ],
             "Pi": [
                 "DstToD0Pi_D0ToKPi"
             ]
```

### Comparing `pidcalib2-1.2.1/src/pidcalib2/make_eff_hists.py` & `pidcalib2-1.3.0/src/pidcalib2/make_eff_hists.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/markdown_table.py` & `pidcalib2-1.3.0/src/pidcalib2/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/merge_trees.py` & `pidcalib2-1.3.0/src/pidcalib2/merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/pid_data.py` & `pidcalib2-1.3.0/src/pidcalib2/pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/pklhisto2root.py` & `pidcalib2-1.3.0/src/pidcalib2/pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/plot_calib_distributions.py` & `pidcalib2-1.3.0/src/pidcalib2/plot_calib_distributions.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,21 +376,23 @@
                 cut_stats,
                 binning_range_cuts,
                 calib_sample["cuts"] if "cuts" in calib_sample else [],
                 config["cuts"] if "cuts" in config else [],
             )
 
             # If no binning
-            for var in bin_vars_without_binnings:
-                var_range = df[var].max() - df[var].min()
-                var_min = df[var].min() - 0.1 * var_range
-                var_max = df[var].max() + 0.1 * var_range
+            for v in bin_vars_without_binnings:
+                vmin = int(df[v].min()) if df[v].min().dtype == "bool" else df[v].min()
+                vmax = int(df[v].max()) if df[v].max().dtype == "bool" else df[v].max()
+                var_range = vmax - vmin
+                var_min = vmin - 0.1 * var_range
+                var_max = vmax + 0.1 * var_range
                 binning.set_binning(
                     config["particle"],
-                    var,
+                    v,
                     list(np.linspace(var_min, var_max, config["bins"] + 1)),
                 )
             # Empty the list to avoid redefining the binning in each step
             bin_vars_without_binnings = []
 
             hists = {
                 var: utils.make_hist(df, config["particle"], [var])
```

### Comparing `pidcalib2-1.2.1/src/pidcalib2/ref_calib.py` & `pidcalib2-1.3.0/src/pidcalib2/ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/samples.py` & `pidcalib2-1.3.0/src/pidcalib2/samples.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_binning.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/cal_test_data.csv` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/cal_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/cal_test_data.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/cal_test_data.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P-pre1.1.0.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-K-DLLK>4-P.ETA.nTracks.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-Pi-DLLK<0-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-Turbo18-up-pi-DLLK<4-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/effhists-test-down-Pi-DLLK>4-P.pkl` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/effhists-test-down-Pi-DLLK>4-P.pkl`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_PID_eff.root` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_PID_eff.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data.csv` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data.csv`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data.root` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/ref_test_data_subdir.root` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/ref_test_data_subdir.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/sweights_2023/00199935_00000001_1.pid_tuple_sweights.root` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/sweights_2023/00199935_00000001_1.pid_tuple_sweights.root`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_data/test_samples.json` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_data/test_samples.json`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_make_eff_hist.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_make_eff_hist.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_merge_trees.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_merge_trees.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_pid_data.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_pid_data.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_pklhisto2root.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_pklhisto2root.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_plot_calib_distributions.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_plot_calib_distributions.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_ref_calib.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_ref_calib.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/tests/test_utils.py` & `pidcalib2-1.3.0/src/pidcalib2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pidcalib2-1.2.1/src/pidcalib2/utils.py` & `pidcalib2-1.3.0/src/pidcalib2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         eff_histo = eff_hists[prefix]["eff"]
         axes = [
             pid_data.get_reference_branch_name(
                 prefix, axis.metadata["name"], bin_vars[axis.metadata["name"]]
             )
             for axis in eff_histo.axes
         ]
+        reference_branch_names = []
         for bin_var, branch_name in bin_vars.items():
             ref_branch_name = pid_data.get_reference_branch_name(
                 prefix, bin_var, branch_name
             )
             bins = []
             for axis in eff_histo.axes:
                 if axis.metadata["name"] == bin_var:
@@ -197,17 +198,20 @@
                 df_new[ref_branch_name],
                 bins,
                 labels=False,
                 include_lowest=True,
                 right=False,
                 precision=0,
             )
+            reference_branch_names.append(f"{ref_branch_name}_PIDCalibBin")
 
-        df_nan = df_new[df_new.isna().any(axis=1)]
-        df_new.dropna(inplace=True)
+        # Assign indices to events that have lie within the binning range for
+        # this particle/prefix's branches/variables
+        df_nan = df_new[df_new[reference_branch_names].isna().any(axis=1)]
+        df_new.dropna(inplace=True, subset=reference_branch_names)
         index_names = [f"{axis}_PIDCalibBin" for axis in axes]
         indices = np.ravel_multi_index(
             df_new[index_names].transpose().to_numpy().astype(int),
             eff_histo.axes.size,
         )
         df_new[f"{prefix}_PIDCalibBin"] = indices
         df_new = pd.concat([df_new, df_nan]).sort_index()
@@ -230,24 +234,25 @@
         df: Input dataframe.
         prefixes: Branch prefixes of the particles in the reference sample.
         eff_hists: Efficiency histograms for each prefix/particle.
         compatibility: Treat empty efficiency histogram bins as PIDCalib1 did
     """
     df_new = df.copy()
 
-    # We separate the dataframe into two parts: one where all the events have
-    # PID indices (events inside the PID binning) and those that don't.
-    # Efficiency is added only for events inside the PID binning.
-    df_nan = df_new[df_new.isna().any(axis=1)]
-    df_new.dropna(inplace=True)
-
     df_new["PIDCalibEff"] = 1
     df_new["PIDCalibRelErr2"] = 0
 
     for prefix in prefixes:
+        # We separate the dataframe into two parts: one where all the events have
+        # PID indices for the prefix/particle in question (events inside the PID
+        # binning) and those that don't. Efficiencies are added only for events
+        # inside the PID binning.
+        df_nan = df_new[df_new[[f"{prefix}_PIDCalibBin"]].isna().any(axis=1)]
+        df_new.dropna(inplace=True, subset=[f"{prefix}_PIDCalibBin"])
+
         efficiency_table = eff_hists[prefix]["eff"].values().flatten()
         error_table = np.sqrt(eff_hists[prefix]["eff"].variances().flatten())  # type: ignore # noqa
 
         # The original PIDCalib assigned bins with no events in the total
         # histogram an efficiency of zero. This should not come up often and the
         # user should be warned about it. In any case it does not seem right -
         # we assign the bin a NaN. This might cause slightly different results
@@ -259,18 +264,24 @@
         df_new[f"{prefix}_PIDCalibEff"] = np.take(
             efficiency_table, df_new[f"{prefix}_PIDCalibBin"]
         )
         # Assign errors by taking the error value from the relevant bin
         df_new[f"{prefix}_PIDCalibErr"] = np.take(
             error_table, df_new[f"{prefix}_PIDCalibBin"]
         )
+
+        df_new = pd.concat([df_new, df_nan]).sort_index()
+
+    # Assign the overall efficiencies and corresponding errors.
+    # -999 is assigned if any of the individual particles' efficiencies are
+    # undefined/-999
+    for prefix in prefixes:
         df_new["PIDCalibEff"] *= df_new[f"{prefix}_PIDCalibEff"]
-        df_new["PIDCalibRelErr2"] += (
-            df_new[f"{prefix}_PIDCalibErr"] / df_new[f"{prefix}_PIDCalibEff"]
-        ) ** 2
+        df_new["PIDCalibRelErr2"] += (df_new[f"{prefix}_PIDCalibErr"] / df_new[
+                                      f"{prefix}_PIDCalibEff"])**2
 
     df_new["PIDCalibErr"] = np.sqrt(df_new["PIDCalibRelErr2"])
     for prefix in prefixes:
         # The absolute value is so that we match PIDCalib1. However if any of
         # the efficiencies are negative the overall efficiency and error are
         # meaningless.
         df_new["PIDCalibErr"] *= df_new[f"{prefix}_PIDCalibEff"]
@@ -287,16 +298,14 @@
         df_new.loc[negative_mask, ["PIDCalibErr"]] = -999
         log.warning(
             (
                 f"{np.count_nonzero(negative_mask)} events include tracks with "
                 "negative efficiencies; assigning -999"
             )
         )
-
-    df_new = pd.concat([df_new, df_nan]).sort_index()
     log.debug("Particle efficiencies assigned")
 
     num_outside_range = len(df_nan.index)
     num_outside_range_frac = len(df_nan.index) / len(df_new.index)
     log.warning(
         (
             "Events out of binning range: "
```

### Comparing `pidcalib2-1.2.1/src/pidcalib2.egg-info/PKG-INFO` & `pidcalib2-1.3.0/src/pidcalib2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pidcalib2
-Version: 1.2.1
+Version: 1.3.0
 Summary: A set of tools for estimating LHCb PID efficiencies
 Home-page: https://gitlab.cern.ch/lhcb-rta/pidcalib2
 Author: Daniel Cervenkov
 Author-email: daniel.cervenkov@cern.ch
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Tracker, https://gitlab.cern.ch/lhcb-rta/pidcalib2/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

