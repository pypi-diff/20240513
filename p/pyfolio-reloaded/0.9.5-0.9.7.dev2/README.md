# Comparing `tmp/pyfolio-reloaded-0.9.5.tar.gz` & `tmp/pyfolio_reloaded-0.9.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfolio-reloaded-0.9.5.tar", last modified: Fri Jan 13 00:14:42 2023, max compression
+gzip compressed data, was "pyfolio_reloaded-0.9.7.dev2.tar", last modified: Mon May 13 15:45:20 2024, max compression
```

## Comparing `pyfolio-reloaded-0.9.5.tar` & `pyfolio_reloaded-0.9.7.dev2.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.880304 pyfolio-reloaded-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/workflows/build_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/workflows/conda_package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/workflows/test_wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.github/workflows/unit_tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17980 2023-01-13 00:14:42.876304 pyfolio-reloaded-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13951 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/WHATSNEW.md
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/build_and_deploy_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.856303 pyfolio-reloaded-0.9.5/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/conda/recipe/
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/conda/recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/source/api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 00:14:42.880304 pyfolio-reloaded-0.9.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.860303 pyfolio-reloaded-0.9.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.864303 pyfolio-reloaded-0.9.5/src/pyfolio/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9284 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/deprecate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.868304 pyfolio-reloaded-0.9.5/src/pyfolio/examples/
--rw-r--r--   0 runner    (1001) docker     (123)  2409115 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/results.pickle
--rw-r--r--   0 runner    (1001) docker     (123)   141738 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1053570 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/sector_mappings_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   603437 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/single_stock_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  2066435 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/slippage_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  3787905 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/examples/zipline_algo_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/interesting_periods.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/ipycompat.py
--rw-r--r--   0 runner    (1001) docker     (123)    21753 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/perf_attrib.py
--rw-r--r--   0 runner    (1001) docker     (123)    62180 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)    14510 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/round_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)    44740 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/tears.py
--rw-r--r--   0 runner    (1001) docker     (123)    36354 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/txn.py
--rw-r--r--   0 runner    (1001) docker     (123)    16067 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/src/pyfolio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.872304 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17980 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-13 00:14:42.000000 pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.876304 pyfolio-reloaded-0.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/matplotlibrc
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_capacity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 00:14:42.876304 pyfolio-reloaded-0.9.5/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    25231 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/factor_loadings.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20879 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/factor_returns.csv
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/intercepts.csv
--rw-r--r--   0 runner    (1001) docker     (123)    11610 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/positions.csv
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/residuals.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/returns.csv
--rw-r--r--   0 runner    (1001) docker     (123)   171201 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_LMCAP.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176341 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_LT_MOMENTUM.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176325 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_MACDSignal.csv
--rw-r--r--   0 runner    (1001) docker     (123)   176472 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_VLTY.csv
--rw-r--r--   0 runner    (1001) docker     (123)   163470 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_caps.csv
--rw-r--r--   0 runner    (1001) docker     (123)    14737 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_gross_lev.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)    72979 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_pos.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_returns.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)    79854 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_sectors.csv
--rw-r--r--   0 runner    (1001) docker     (123)   168354 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_shares_held.csv
--rw-r--r--   0 runner    (1001) docker     (123)   139637 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_txn.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)   162991 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_data/test_volumes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_perf_attrib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_pos.py
--rw-r--r--   0 runner    (1001) docker     (123)    10205 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_round_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_tears.py
--rw-r--r--   0 runner    (1001) docker     (123)    12772 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-01-13 00:14:31.000000 pyfolio-reloaded-0.9.5/tests/test_txn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/build_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/conda_package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/test_wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.github/workflows/unit_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13951 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/WHATSNEW.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       93 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/build_and_deploy_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/conda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/conda/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/conda/recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7669 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:45:20.563405 pyfolio_reloaded-0.9.7.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.535405 pyfolio_reloaded-0.9.7.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.539404 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/deprecate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.547405 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)  2409115 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/results.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/round_trip_tear_sheet_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  1053570 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/sector_mappings_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   603437 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/single_stock_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2066435 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/slippage_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  3787905 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/zipline_algo_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/interesting_periods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/ipycompat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21754 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62305 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44741 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/tears.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36354 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/txn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.559404 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 15:45:20.000000 pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.555405 pyfolio_reloaded-0.9.7.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/matplotlibrc
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_capacity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:45:20.559404 pyfolio_reloaded-0.9.7.dev2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    25231 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_loadings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20879 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_returns.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/intercepts.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    11610 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/positions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9589 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/residuals.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/returns.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   171201 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LMCAP.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176341 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LT_MOMENTUM.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176325 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_MACDSignal.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   176472 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_VLTY.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   163470 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_caps.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14737 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_gross_lev.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    72979 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_pos.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    16393 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_returns.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)    79854 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_sectors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   168354 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_shares_held.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   139637 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_txn.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   162991 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_volumes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18856 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_perf_attrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_pos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10205 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_tears.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12845 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-13 15:45:13.000000 pyfolio_reloaded-0.9.7.dev2/tests/test_txn.py
```

### Comparing `pyfolio-reloaded-0.9.5/.github/workflows/build_wheels.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/build_wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -2,64 +2,64 @@
 
 on:
   workflow_dispatch:
     inputs:
       publish_to_pypi:
         description: 'Publish to PyPI?'
         required: true
-        type: boolean
-        default: false
+        type: string
+        default: 'false'
 
 jobs:
   dist:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
         python-version: [ "3.10" ]
 
     steps:
       - name: Checkout pyfolio
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Build wheels
         run: pipx run build
 
       - name: Store artifacts
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           path: dist/*
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
   upload_pypi:
     needs: [ dist ]
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v3
+      - uses: actions/download-artifact@v4
         with:
           name: artifact
           path: dist
 
       - name: publish to testpypi
         uses: pypa/gh-action-pypi-publish@release/v1
-        if: ${{ inputs.publish_to_pypi == false }}
+        if: ${{ inputs.publish_to_pypi == 'false' }}
         with:
           user: __token__
           password: ${{ secrets.TESTPYPI_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
 
       - name: publish to pypi
         uses: pypa/gh-action-pypi-publish@release/v1
-        if: ${{ inputs.publish_to_pypi == true }}
+        if: ${{ inputs.publish_to_pypi == 'true' }}
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
```

### Comparing `pyfolio-reloaded-0.9.5/.github/workflows/conda_package.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/conda_package.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
       fail-fast: false
       matrix:
         os: [ macos-latest, windows-latest, ubuntu-latest ]
         python: [ '3.7', '3.8', '3.9']
 
     steps:
       - name: Checkout pyfolio-reloaded
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
       - name: Setup miniconda3
-        uses: conda-incubator/setup-miniconda@v2
+        uses: conda-incubator/setup-miniconda@v3
         with:
           miniconda-version: latest
           auto-update-conda: true
           channel-priority: true
           mamba-version: "*"
           python-version: ${{ matrix.python }}
           activate-environment: recipe
@@ -46,35 +46,35 @@
 
       - name: activate uploader
         # address broken client under py3.9
         if: ${{ matrix.python == '3.9' }}
         run: conda activate up
 
       - name: store windows result
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'windows-latest' }}
         with:
           path: win-64/*.tar.bz2
 
       - name: upload windows
         if: ${{ matrix.os == 'windows-latest' }}
         run: anaconda upload -l main -u ml4t win-64/*.tar.bz2
 
       - name: store linux result
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'ubuntu-latest' }}
         with:
           path: linux-64/*.tar.bz2
 
       - name: upload linux
         if: ${{ matrix.os  == 'ubuntu-latest' }}
         run: anaconda upload -l main -u ml4t linux-64/*.tar.bz2
 
       - name: store macos result
-        uses: actions/upload-artifact@v2
+        uses: actions/upload-artifact@v4
         if: ${{ matrix.os == 'macos-latest' }}
         with:
           path: osx-64/*.tar.bz2
 
       - name: upload macos
         if: ${{ matrix.os == 'macos-latest' }}
         run: anaconda upload -l main -u ml4t osx-64/*.tar.bz2
```

### Comparing `pyfolio-reloaded-0.9.5/.github/workflows/unit_tests.yml` & `pyfolio_reloaded-0.9.7.dev2/.github/workflows/unit_tests.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest , windows-latest, macos-latest ]
-        python-version: [ 3.8, 3.9, '3.10', '3.11']
+        python-version: [ '3.9', '3.10', '3.11', '3.12']
     steps:
       - name: Checkout pyfolio
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install pyfolio
         run: |
           python -m pip install --upgrade pip
           pip install tox tox-gh-actions
```

### Comparing `pyfolio-reloaded-0.9.5/.gitignore` & `pyfolio_reloaded-0.9.7.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/LICENSE` & `pyfolio_reloaded-0.9.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/PKG-INFO` & `pyfolio_reloaded-0.9.7.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfolio-reloaded
-Version: 0.9.5
+Version: 0.9.7.dev2
 Summary: Performance and risk analysis of financial portfolios with Python
 Author: Quantopian Inc
 Author-email: pm@ml4trading.io
 Maintainer: Stefan Jansen
 Maintainer-email: pm@ml4trading.io
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -211,28 +211,58 @@
 Project-URL: homepage, https://ml4trading.io
 Project-URL: repository, https://github.com/stefan-jansen/pyfolio-reloaded
 Project-URL: documentation, https://pyfolio.ml4trading.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=3.2.3
+Requires-Dist: matplotlib>=1.4.0
+Requires-Dist: numpy>=1.11.1
+Requires-Dist: pandas>=1.3
+Requires-Dist: pytz>=2014.10
+Requires-Dist: scipy>=0.14.0
+Requires-Dist: scikit-learn>=0.16.1
+Requires-Dist: seaborn>=0.7.1
+Requires-Dist: empyrical-reloaded>=0.5.9
 Provides-Extra: test
+Requires-Dist: tox>=2.3.1; extra == "test"
+Requires-Dist: coverage>=4.0.3; extra == "test"
+Requires-Dist: coveralls==3.0.1; extra == "test"
+Requires-Dist: pytest>=6.2; extra == "test"
+Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
+Requires-Dist: pytest-cov>=2.12; extra == "test"
+Requires-Dist: parameterized>=0.6.1; extra == "test"
+Requires-Dist: pytest-rerunfailures; extra == "test"
+Requires-Dist: flake8>=3.9.1; extra == "test"
+Requires-Dist: black; extra == "test"
 Provides-Extra: dev
+Requires-Dist: flake8>=3.9.1; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: Cython; extra == "docs"
+Requires-Dist: Sphinx>=1.3.2; extra == "docs"
+Requires-Dist: numpydoc>=0.5.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=0.6.0; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: sphinx-markdown-tables; extra == "docs"
+Requires-Dist: sphinx_copybutton; extra == "docs"
+Requires-Dist: m2r2; extra == "docs"
 
 <p align="center">
 <a href="https://pyfolio.ml4trading.io">
 <img src="https://i.imgur.com/GD6TZ0D.png" width="35%">
 </a>
 </p>
```

### Comparing `pyfolio-reloaded-0.9.5/README.md` & `pyfolio_reloaded-0.9.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/WHATSNEW.md` & `pyfolio_reloaded-0.9.7.dev2/WHATSNEW.md`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/conda/recipe/meta.yaml` & `pyfolio_reloaded-0.9.7.dev2/conda/recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/docs/Makefile` & `pyfolio_reloaded-0.9.7.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/docs/deploy.py` & `pyfolio_reloaded-0.9.7.dev2/docs/deploy.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/docs/make.bat` & `pyfolio_reloaded-0.9.7.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/docs/source/api-reference.rst` & `pyfolio_reloaded-0.9.7.dev2/docs/source/api-reference.rst`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/docs/source/conf.py` & `pyfolio_reloaded-0.9.7.dev2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/pyproject.toml` & `pyfolio_reloaded-0.9.7.dev2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pyfolio-reloaded"
 description = "Performance and risk analysis of financial portfolios with Python"
 
-requires-python = '>=3.8'
+requires-python = '>=3.9'
 dynamic = ["version"]
 readme = "README.md"
 authors = [
     { name = 'Quantopian Inc' },
     { email = 'pm@ml4trading.io' }
 ]
 maintainers = [
@@ -16,34 +16,34 @@
 license = { file = "LICENSE" }
 
 classifiers = [
     'Development Status :: 4 - Beta',
     'License :: OSI Approved :: Apache Software License',
     'Natural Language :: English',
     'Programming Language :: Python',
-    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Operating System :: OS Independent',
     'Intended Audience :: Science/Research',
     'Topic :: Office/Business :: Financial :: Investment',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
 
 dependencies = [
     "ipython >=3.2.3",
     "matplotlib >=1.4.0",
     "numpy >=1.11.1",
-    "pandas >=0.18.1",
+    "pandas >=1.3",
     "pytz >=2014.10",
     "scipy >=0.14.0",
     "scikit-learn >=0.16.1",
     "seaborn >=0.7.1",
-    "empyrical-reloaded >=0.5.8",
+    "empyrical-reloaded >=0.5.9",
 ]
 
 [project.urls]
 homepage = 'https://ml4trading.io'
 repository = 'https://github.com/stefan-jansen/pyfolio-reloaded'
 documentation = 'https://pyfolio.ml4trading.io'
 
@@ -61,14 +61,15 @@
     "tox >=2.3.1",
     "coverage >=4.0.3",
     "coveralls ==3.0.1",
     "pytest >=6.2",
     'pytest-xdist >=2.5.0',
     "pytest-cov >=2.12",
     "parameterized >=0.6.1",
+    "pytest-rerunfailures",
     "flake8 >=3.9.1",
     "black",
 ]
 dev = [
     "flake8 >=3.9.1",
     "black",
     "pre-commit >=2.12.1",
@@ -129,35 +130,39 @@
   docs/source/conf.py
 \)
 '''
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,39}-pandas12, py{38,39,310}-pandas{13,14,15}, py311-pandas15
+envlist = py39-pandas{11,12},py{39,310}-pandas{13,14,15}, py{39,310, 311,312}-pandas{20,21,22}
 isolated_build = True
 skip_missing_interpreters = True
 minversion = 3.23.0
 
 [gh-actions]
 python =
-    3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
+    3.12: py312
 
 [testenv]
 usedevelop = True
 setenv =
     MPLBACKEND = Agg
 
 changedir = tmp
 extras = test
 deps =
+    pandas11: pandas>=1.1.0,<1.2
     pandas12: pandas>=1.2.0,<1.3
     pandas13: pandas>=1.3.0,<1.4
     pandas14: pandas>=1.4.0,<1.5
     pandas15: pandas>=1.5.0,<1.6
+    pandas20: pandas>=2.0,<2.1
+    pandas21: pandas>=2.1,<2.2
+    pandas22: pandas>=2.2,<2.3
 
 commands =
     pytest -n 2 --cov={toxinidir}/src --cov-report term  --cov-report=xml --cov-report=html:htmlcov {toxinidir}/tests
 """
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/__init__.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/capacity.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/capacity.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/deprecate.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/deprecate.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/examples/results.pickle` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/results.pickle`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/examples/sector_mappings_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/sector_mappings_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/examples/single_stock_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/single_stock_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/examples/slippage_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/slippage_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/examples/zipline_algo_example.ipynb` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/examples/zipline_algo_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/interesting_periods.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/interesting_periods.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/ipycompat.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/ipycompat.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/perf_attrib.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/perf_attrib.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     factor_loadings,
     transactions=None,
     pos_in_dollars=True,
 ):
     """
     Attributes the performance of a returns stream to a set of risk factors.
 
-    Preprocesses inputs, and then calls empyrical.perf_attrib. See
+    Pre-processes inputs, and then calls empyrical.perf_attrib. See
     empyrical.perf_attrib for more info.
 
     Performance attribution determines how much each risk factor, e.g.,
     momentum, the technology sector, etc., contributed to total returns, as
     well as the daily exposure to each of the risk factors. The returns that
     can be attributed to one of the given risk factors are the
     `common_returns`, and the returns that _cannot_ be attributed to a risk
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/plotting.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import datetime
 import calendar
+import datetime
 from collections import OrderedDict
 from functools import wraps
 
 import empyrical as ep
 import matplotlib
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import pytz
 import scipy as sp
+import seaborn as sns
 from matplotlib import figure
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 from matplotlib.ticker import FuncFormatter
 
-import seaborn as sns
 from . import capacity
 from . import pos
 from . import timeseries
 from . import txn
 from . import utils
 from .utils import APPROX_BDAYS_PER_MONTH, MM_DISPLAY_UNIT
 
@@ -440,15 +440,18 @@
     df_cum_rets = ep.cum_returns(returns, starting_value=1.0)
     df_drawdowns = timeseries.gen_drawdown_table(returns, top=top)
 
     df_cum_rets.plot(ax=ax, **kwargs)
 
     lim = ax.get_ylim()
     colors = sns.cubehelix_palette(len(df_drawdowns))[::-1]
-    for i, (peak, recovery) in df_drawdowns[["Peak date", "Recovery date"]].iterrows():
+    # print(df_drawdowns)
+    for i, (peak, recovery) in (
+        df_drawdowns[["Peak date", "Recovery date"]].dropna(how="all").iterrows()
+    ):
         if pd.isnull(recovery):
             recovery = returns.index[-1]
         ax.fill_between((peak, recovery), lim[0], lim[1], alpha=0.4, color=colors[i])
     ax.set_ylim(lim)
     ax.set_title("Top %i drawdown periods" % top)
     ax.set_ylabel("Cumulative returns")
     ax.legend(["Portfolio"], loc="upper left", frameon=True, framealpha=0.5)
@@ -544,14 +547,15 @@
     factor_returns=None,
     positions=None,
     transactions=None,
     turnover_denom="AGB",
     live_start_date=None,
     bootstrap=False,
     header_rows=None,
+    return_df=False,
 ):
     """
     Prints some performance metrics of the strategy.
 
     - Shows amount of time the strategy has been run in backtest and
       out-of-sample (in live trading).
 
@@ -666,14 +670,16 @@
                 perf_stats.loc[stat, column] = str(np.round(value * 100, 3)) + "%"
     if header_rows is None:
         header_rows = date_rows
     else:
         header_rows = OrderedDict(header_rows)
         header_rows.update(date_rows)
 
+    if return_df:
+        return perf_stats
     utils.print_table(
         perf_stats,
         float_format="{0:.2f}".format,
         header_rows=header_rows,
     )
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/pos.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/pos.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/round_trips.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/round_trips.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,30 @@
 
 PNL_STATS = [
     ("Total profit", lambda x: x.sum()),
     ("Gross profit", lambda x: x[x > 0].sum()),
     ("Gross loss", lambda x: x[x < 0].sum()),
     (
         "Profit factor",
-        lambda x: x[x > 0].sum() / x[x < 0].abs().sum()
-        if x[x < 0].abs().sum() != 0
-        else np.nan,
+        lambda x: (
+            x[x > 0].sum() / x[x < 0].abs().sum()
+            if x[x < 0].abs().sum() != 0
+            else np.nan
+        ),
     ),
     ("Avg. trade net profit", "mean"),
     ("Avg. winning trade", lambda x: x[x > 0].mean()),
     ("Avg. losing trade", lambda x: x[x < 0].mean()),
     (
         "Ratio Avg. Win:Avg. Loss",
-        lambda x: x[x > 0].mean() / x[x < 0].abs().mean()
-        if x[x < 0].abs().mean() != 0
-        else np.nan,
+        lambda x: (
+            x[x > 0].mean() / x[x < 0].abs().mean()
+            if x[x < 0].abs().mean() != 0
+            else np.nan
+        ),
     ),
     ("Largest winning trade", "max"),
     ("Largest losing trade", "min"),
 ]
 
 SUMMARY_STATS = [
     ("Total number of round_trips", "count"),
@@ -63,15 +67,15 @@
     ("Largest losing trade", "min"),
 ]
 
 DURATION_STATS = [
     ("Avg duration", lambda x: x.mean()),
     ("Median duration", lambda x: x.median()),
     ("Longest duration", lambda x: x.max()),
-    ("Shortest duration", lambda x: x.min())
+    ("Shortest duration", lambda x: x.min()),
     #  FIXME: Instead of x.max() - x.min() this should be
     #  rts.close_dt.max() - rts.open_dt.min() which is not
     #  available here. As it would require a new approach here
     #  that passes in multiple fields we disable these measures
     #  for now.
     #  ('Avg # round_trips per day', lambda x: float(len(x)) /
     #   (x.max() - x.min()).days),
@@ -160,15 +164,15 @@
     For example, the following transactions would constitute one round trip:
     index                  amount   price    symbol
     2004-01-09 12:18:01    10       50      'AAPL'
     2004-01-09 15:12:53    10       100      'AAPL'
     2004-01-13 14:41:23    -10      100      'AAPL'
     2004-01-13 15:23:34    -10      200       'AAPL'
 
-    First, the first two and last two round_trips will be merged into a two
+    First, the first two and last two round_trips will be merged into two
     single transactions (computing the price via vwap). Then, during
     the portfolio reconstruction, the two resulting transactions will
     be merged and result in 1 round-trip trade with a PnL of
     (150 * 20) - (75 * 20) = 1500.
 
     Note, that round trips do not have to close out positions
     completely. For example, we could have removed the last
@@ -188,16 +192,16 @@
         use .shift() or positions.sum(axis='columns') / (1+returns).
 
     Returns
     -------
     round_trips : pd.DataFrame
         DataFrame with one row per round trip.  The returns column
         contains returns in respect to the portfolio value while
-        rt_returns are the returns in regards to the invested capital
-        into that partiulcar round-trip.
+        rt_returns are the returns regarding the invested capital
+        into that particular round-trip.
     """
 
     transactions = _groupby_consecutive(transactions)
     roundtrips = []
 
     for sym, trans_sym in transactions.groupby("symbol"):
         trans_sym = trans_sym.sort_index()
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/tears.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/tears.py`

 * *Files 0% similar despite different names*

```diff
@@ -903,14 +903,15 @@
     """
 
     positions = utils.check_intraday(
         estimate_intraday, returns, positions, transactions
     )
 
     transactions_closed = round_trips.add_closing_transactions(positions, transactions)
+
     # extract_round_trips requires BoD portfolio_value
     trades = round_trips.extract_round_trips(
         transactions_closed,
         portfolio_value=positions.sum(axis="columns") / (1 + returns),
     )
 
     if len(trades) < 5:
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/timeseries.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/txn.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/txn.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio/utils.py` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     "#ffd8b1",
     "#000080",
     "#808080",
 ]
 
 pandas_version = Version(pd.__version__)
 
-pandas_one_point_one_or_less = pandas_version < Version("1.2")
+pandas_one_point_three_or_less = pandas_version < Version("1.4")
 
 
 def one_dec_places(x, pos):
     """
     Adds 1/10th decimal to plot ticks.
     """
 
@@ -308,16 +308,16 @@
         Daily net position values, adjusted for intraday movement.
     """
 
     if estimate == "infer":
         if positions is not None and transactions is not None:
             if detect_intraday(positions, transactions):
                 warnings.warn(
-                    "Detected intraday strategy; inferring positi"
-                    + "ons from transactions. Set estimate_intraday"
+                    "Detected intraday strategy; inferring positions"
+                    + "from transactions. Set estimate_intraday"
                     + "=False to disable."
                 )
                 return estimate_intraday(returns, positions, transactions)
             else:
                 return positions
         else:
             return positions
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/PKG-INFO` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfolio-reloaded
-Version: 0.9.5
+Version: 0.9.7.dev2
 Summary: Performance and risk analysis of financial portfolios with Python
 Author: Quantopian Inc
 Author-email: pm@ml4trading.io
 Maintainer: Stefan Jansen
 Maintainer-email: pm@ml4trading.io
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -211,28 +211,58 @@
 Project-URL: homepage, https://ml4trading.io
 Project-URL: repository, https://github.com/stefan-jansen/pyfolio-reloaded
 Project-URL: documentation, https://pyfolio.ml4trading.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ipython>=3.2.3
+Requires-Dist: matplotlib>=1.4.0
+Requires-Dist: numpy>=1.11.1
+Requires-Dist: pandas>=1.3
+Requires-Dist: pytz>=2014.10
+Requires-Dist: scipy>=0.14.0
+Requires-Dist: scikit-learn>=0.16.1
+Requires-Dist: seaborn>=0.7.1
+Requires-Dist: empyrical-reloaded>=0.5.9
 Provides-Extra: test
+Requires-Dist: tox>=2.3.1; extra == "test"
+Requires-Dist: coverage>=4.0.3; extra == "test"
+Requires-Dist: coveralls==3.0.1; extra == "test"
+Requires-Dist: pytest>=6.2; extra == "test"
+Requires-Dist: pytest-xdist>=2.5.0; extra == "test"
+Requires-Dist: pytest-cov>=2.12; extra == "test"
+Requires-Dist: parameterized>=0.6.1; extra == "test"
+Requires-Dist: pytest-rerunfailures; extra == "test"
+Requires-Dist: flake8>=3.9.1; extra == "test"
+Requires-Dist: black; extra == "test"
 Provides-Extra: dev
+Requires-Dist: flake8>=3.9.1; extra == "dev"
+Requires-Dist: black; extra == "dev"
+Requires-Dist: pre-commit>=2.12.1; extra == "dev"
 Provides-Extra: docs
-License-File: LICENSE
+Requires-Dist: Cython; extra == "docs"
+Requires-Dist: Sphinx>=1.3.2; extra == "docs"
+Requires-Dist: numpydoc>=0.5.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=0.6.0; extra == "docs"
+Requires-Dist: pydata-sphinx-theme; extra == "docs"
+Requires-Dist: sphinx-markdown-tables; extra == "docs"
+Requires-Dist: sphinx_copybutton; extra == "docs"
+Requires-Dist: m2r2; extra == "docs"
 
 <p align="center">
 <a href="https://pyfolio.ml4trading.io">
 <img src="https://i.imgur.com/GD6TZ0D.png" width="35%">
 </a>
 </p>
```

### Comparing `pyfolio-reloaded-0.9.5/src/pyfolio_reloaded.egg-info/SOURCES.txt` & `pyfolio_reloaded-0.9.7.dev2/src/pyfolio_reloaded.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_capacity.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_capacity.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/factor_loadings.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_loadings.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/factor_returns.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/factor_returns.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/positions.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/positions.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/residuals.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/residuals.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/returns.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/returns.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_LMCAP.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LMCAP.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_LT_MOMENTUM.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_LT_MOMENTUM.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_MACDSignal.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_MACDSignal.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_VLTY.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_VLTY.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_caps.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_caps.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_gross_lev.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_gross_lev.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_pos.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_pos.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_returns.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_returns.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_sectors.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_sectors.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_shares_held.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_shares_held.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_txn.csv.gz` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_txn.csv.gz`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_data/test_volumes.csv` & `pyfolio_reloaded-0.9.7.dev2/tests/test_data/test_volumes.csv`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_perf_attrib.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_perf_attrib.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,17 @@
     _cumulative_returns_less_costs,
 )
 
 TEST_DATA = Path(__file__).parent / "test_data"
 
 
 def _empyrical_compat_perf_attrib_result(index, columns, data):
-    if ep.__version__ < "0.5.2":
+    major, minor, micro = ep.__version__.split(".")
+    major, minor, micro = int(major), int(minor), int(micro)
+    if major == 0 and (minor < 5 or (minor == 5 and micro < 2)):
         # Newer columns were added in empyrical v0.5.2. These exist in older
         # and newer empyrical:
         columns = [
             "risk_factor1",
             "risk_factor2",
             "common_returns",
             "specific_returns",
@@ -507,15 +509,15 @@
                 self.assertNotIn(date, perf_attrib_data.index)
 
             # raise exception if all stocks are filtered out
             empty_factor_loadings = factor_loadings.drop(
                 ["AAPL", "TLT", "XOM"], level="ticker"
             )
 
-            with self.assertRaisesRegexp(
+            with self.assertRaisesRegex(
                 ValueError, "No factor loadings were available"
             ):
 
                 exposures, perf_attrib_data = perf_attrib(
                     returns, positions, factor_returns, empty_factor_loadings
                 )
```

### Comparing `pyfolio-reloaded-0.9.5/tests/test_pos.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_pos.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_round_trips.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_round_trips.py`

 * *Files identical despite different names*

### Comparing `pyfolio-reloaded-0.9.5/tests/test_tears.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_tears.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
             parse_dates=True,
         )
     )
 
     @parameterized.expand(
         [
             ({},),
-            ({"slippage": 1},),
+            # ({"slippage": 1},),
             ({"live_start_date": test_returns.index[-20]},),
             ({"round_trips": True},),
             ({"hide_positions": True},),
             ({"cone_std": 1},),
             ({"bootstrap": True},),
         ]
     )
```

### Comparing `pyfolio-reloaded-0.9.5/tests/test_timeseries.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_timeseries.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from unittest import TestCase, skipIf
 from parameterized import parameterized
 from numpy.testing import assert_allclose, assert_almost_equal
 from pandas.testing import assert_series_equal
 import numpy as np
 import pandas as pd
 
-from src.pyfolio import timeseries
-from pyfolio.utils import to_utc, to_series, pandas_one_point_one_or_less
+from pyfolio import timeseries
+from pyfolio.utils import to_utc, to_series, pandas_one_point_three_or_less
 
 import gzip
 
 DECIMAL_PLACES = 8
 
 
 class TestDrawdown(TestCase):
@@ -129,24 +129,28 @@
     def test_get_max_drawdown(
         self, px, expected_peak, expected_valley, expected_recovery
     ):
         rets = px.pct_change().iloc[1:]
 
         peak, valley, recovery = timeseries.get_max_drawdown(rets)
         # Need to use isnull because the result can be NaN, NaT, etc.
-        self.assertTrue(pd.isnull(peak)) if expected_peak is None else self.assertEqual(
-            peak, expected_peak
-        )
-        self.assertTrue(
-            pd.isnull(valley)
-        ) if expected_valley is None else self.assertEqual(valley, expected_valley)
-        self.assertTrue(
-            pd.isnull(recovery)
-        ) if expected_recovery is None else self.assertEqual(
-            recovery, expected_recovery
+        (
+            self.assertTrue(pd.isnull(peak))
+            if expected_peak is None
+            else self.assertEqual(peak, expected_peak)
+        )
+        (
+            self.assertTrue(pd.isnull(valley))
+            if expected_valley is None
+            else self.assertEqual(valley, expected_valley)
+        )
+        (
+            self.assertTrue(pd.isnull(recovery))
+            if expected_recovery is None
+            else self.assertEqual(recovery, expected_recovery)
         )
 
     @parameterized.expand(
         [
             (
                 pd.Series(px_list_2, index=dt),
                 pd.Timestamp("2000-1-4"),
@@ -170,33 +174,33 @@
         expected_valley,
         expected_recovery,
         expected_duration,
     ):
         rets = px.pct_change().iloc[1:]
 
         drawdowns = timeseries.gen_drawdown_table(rets, top=1)
-        self.assertTrue(
-            pd.isnull(drawdowns.loc[0, "Peak date"])
-        ) if expected_peak is None else self.assertEqual(
-            drawdowns.loc[0, "Peak date"], expected_peak
-        )
-        self.assertTrue(
-            pd.isnull(drawdowns.loc[0, "Valley date"])
-        ) if expected_valley is None else self.assertEqual(
-            drawdowns.loc[0, "Valley date"], expected_valley
-        )
-        self.assertTrue(
-            pd.isnull(drawdowns.loc[0, "Recovery date"])
-        ) if expected_recovery is None else self.assertEqual(
-            drawdowns.loc[0, "Recovery date"], expected_recovery
-        )
-        self.assertTrue(
-            pd.isnull(drawdowns.loc[0, "Duration"])
-        ) if expected_duration is None else self.assertEqual(
-            drawdowns.loc[0, "Duration"], expected_duration
+        (
+            self.assertTrue(pd.isnull(drawdowns.loc[0, "Peak date"]))
+            if expected_peak is None
+            else self.assertEqual(drawdowns.loc[0, "Peak date"], expected_peak)
+        )
+        (
+            self.assertTrue(pd.isnull(drawdowns.loc[0, "Valley date"]))
+            if expected_valley is None
+            else self.assertEqual(drawdowns.loc[0, "Valley date"], expected_valley)
+        )
+        (
+            self.assertTrue(pd.isnull(drawdowns.loc[0, "Recovery date"]))
+            if expected_recovery is None
+            else self.assertEqual(drawdowns.loc[0, "Recovery date"], expected_recovery)
+        )
+        (
+            self.assertTrue(pd.isnull(drawdowns.loc[0, "Duration"]))
+            if expected_duration is None
+            else self.assertEqual(drawdowns.loc[0, "Duration"], expected_duration)
         )
 
     def test_drawdown_overlaps(self):
         rand = np.random.RandomState(1337)
         n_samples = 252 * 5
         spy_returns = pd.Series(
             rand.standard_t(3.1, n_samples),
@@ -289,15 +293,15 @@
             (
                 simple_rets[:5],
                 2,
                 [np.nan, np.inf, np.inf, 11.224972160321, np.nan],
             )
         ]
     )
-    @skipIf(pandas_one_point_one_or_less, "pandas<1.2 returns np.inf not np.nan")
+    @skipIf(pandas_one_point_three_or_less, "pandas<=1.3 returns np.inf not np.nan")
     def test_sharpe_2(self, returns, rolling_sharpe_window, expected):
         np.testing.assert_array_almost_equal(
             timeseries.rolling_sharpe(returns, rolling_sharpe_window).to_numpy(),
             np.asarray(expected),
         )
 
     @parameterized.expand([(simple_rets[:5], simple_benchmark, 2, 0)])
```

### Comparing `pyfolio-reloaded-0.9.5/tests/test_txn.py` & `pyfolio_reloaded-0.9.7.dev2/tests/test_txn.py`

 * *Files identical despite different names*

