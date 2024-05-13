# Comparing `tmp/resample-1.8.2.tar.gz` & `tmp/resample-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resample-1.8.2.tar", last modified: Fri Apr 19 10:08:53 2024, max compression
+gzip compressed data, was "resample-1.9.0.tar", last modified: Mon May 13 13:17:52 2024, max compression
```

## Comparing `resample-1.8.2.tar` & `resample-1.9.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.812294 resample-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-19 10:08:50.000000 resample-1.8.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.800294 resample-1.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.804293 resample-1.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-19 10:08:50.000000 resample-1.8.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-19 10:08:50.000000 resample-1.8.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-19 10:08:50.000000 resample-1.8.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-19 10:08:50.000000 resample-1.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-19 10:08:50.000000 resample-1.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 10:08:50.000000 resample-1.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-19 10:08:50.000000 resample-1.8.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-19 10:08:50.000000 resample-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 10:08:50.000000 resample-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-19 10:08:53.812294 resample-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-19 10:08:50.000000 resample-1.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.804293 resample-1.8.2/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-19 10:08:50.000000 resample-1.8.2/benchmarks/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-19 10:08:50.000000 resample-1.8.2/benchmarks/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-19 10:08:50.000000 resample-1.8.2/benchmarks/test_rcont.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-19 10:08:50.000000 resample-1.8.2/benchmarks/test_usp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.808294 resample-1.8.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-19 10:08:50.000000 resample-1.8.2/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.808294 resample-1.8.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    46843 2024-04-19 10:08:50.000000 resample-1.8.2/doc/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    86616 2024-04-19 10:08:50.000000 resample-1.8.2/doc/bench_rcont.json
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-19 10:08:50.000000 resample-1.8.2/doc/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-19 10:08:50.000000 resample-1.8.2/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.808294 resample-1.8.2/doc/example/
--rw-r--r--   0 runner    (1001) docker     (127)   179554 2024-04-19 10:08:50.000000 resample-1.8.2/doc/example/tag_and_probe.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-19 10:08:50.000000 resample-1.8.2/doc/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-19 10:08:50.000000 resample-1.8.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-19 10:08:50.000000 resample-1.8.2/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 10:08:50.000000 resample-1.8.2/doc/make_raw_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-19 10:08:50.000000 resample-1.8.2/doc/plot_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-19 10:08:50.000000 resample-1.8.2/doc/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.808294 resample-1.8.2/doc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/confidence_intervals.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/jackknife_vs_bootstrap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    73522 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/permutation_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   141793 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/sklearn.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42094 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/usp_continuous_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorial/variance_fit_parameters.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-19 10:08:50.000000 resample-1.8.2/doc/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-19 10:08:50.000000 resample-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:08:53.812294 resample-1.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.804293 resample-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.812294 resample-1.8.2/src/resample/
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-04-19 10:08:50.000000 resample-1.8.2/src/resample/permutation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.812294 resample-1.8.2/src/resample.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-19 10:08:53.000000 resample-1.8.2/src/resample.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-19 10:08:53.000000 resample-1.8.2/src/resample.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:08:53.000000 resample-1.8.2/src/resample.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-19 10:08:53.000000 resample-1.8.2/src/resample.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-19 10:08:53.000000 resample-1.8.2/src/resample.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:08:53.812294 resample-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-19 10:08:50.000000 resample-1.8.2/tests/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-19 10:08:50.000000 resample-1.8.2/tests/test_empirical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2024-04-19 10:08:50.000000 resample-1.8.2/tests/test_jackknife.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-04-19 10:08:50.000000 resample-1.8.2/tests/test_permutation.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-19 10:08:50.000000 resample-1.8.2/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.359008 resample-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 13:17:44.000000 resample-1.9.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.351008 resample-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.351008 resample-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-13 13:17:44.000000 resample-1.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-13 13:17:44.000000 resample-1.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-13 13:17:44.000000 resample-1.9.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 13:17:44.000000 resample-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-13 13:17:44.000000 resample-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 13:17:44.000000 resample-1.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-13 13:17:44.000000 resample-1.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-13 13:17:44.000000 resample-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 13:17:44.000000 resample-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-13 13:17:52.359008 resample-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-13 13:17:44.000000 resample-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.351008 resample-1.9.0/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 13:17:44.000000 resample-1.9.0/benchmarks/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 13:17:44.000000 resample-1.9.0/benchmarks/test_jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 13:17:44.000000 resample-1.9.0/benchmarks/test_rcont.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 13:17:44.000000 resample-1.9.0/benchmarks/test_usp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.355008 resample-1.9.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-13 13:17:44.000000 resample-1.9.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.355008 resample-1.9.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    46843 2024-05-13 13:17:44.000000 resample-1.9.0/doc/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86616 2024-05-13 13:17:44.000000 resample-1.9.0/doc/bench_rcont.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-13 13:17:44.000000 resample-1.9.0/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-13 13:17:44.000000 resample-1.9.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.355008 resample-1.9.0/doc/example/
+-rw-r--r--   0 runner    (1001) docker     (127)   179554 2024-05-13 13:17:44.000000 resample-1.9.0/doc/example/tag_and_probe.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-13 13:17:44.000000 resample-1.9.0/doc/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 13:17:44.000000 resample-1.9.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-13 13:17:44.000000 resample-1.9.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-13 13:17:44.000000 resample-1.9.0/doc/make_raw_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-13 13:17:44.000000 resample-1.9.0/doc/plot_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-13 13:17:44.000000 resample-1.9.0/doc/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.355008 resample-1.9.0/doc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/confidence_intervals.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/jackknife_vs_bootstrap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   136674 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/leave-one-out-cross-validation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    73522 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/permutation_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   141793 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/sklearn.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42094 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/usp_continuous_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19860 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorial/variance_fit_parameters.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-13 13:17:44.000000 resample-1.9.0/doc/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 13:17:44.000000 resample-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:17:52.359008 resample-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.351008 resample-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.359008 resample-1.9.0/src/resample/
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20775 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11232 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15914 2024-05-13 13:17:44.000000 resample-1.9.0/src/resample/permutation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.359008 resample-1.9.0/src/resample.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-13 13:17:52.000000 resample-1.9.0/src/resample.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 13:17:52.000000 resample-1.9.0/src/resample.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:17:52.000000 resample-1.9.0/src/resample.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-13 13:17:52.000000 resample-1.9.0/src/resample.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 13:17:52.000000 resample-1.9.0/src/resample.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:17:52.359008 resample-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-13 13:17:44.000000 resample-1.9.0/tests/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-13 13:17:44.000000 resample-1.9.0/tests/test_empirical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-05-13 13:17:44.000000 resample-1.9.0/tests/test_jackknife.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-13 13:17:44.000000 resample-1.9.0/tests/test_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-13 13:17:44.000000 resample-1.9.0/tests/test_util.py
```

### Comparing `resample-1.8.2/.github/workflows/docs.yml` & `resample-1.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/.github/workflows/release.yml` & `resample-1.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/.github/workflows/test.yml` & `resample-1.9.0/.github/workflows/test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -8,27 +8,27 @@
   cancel-in-progress: true
 
 env:
   PIP_ONLY_BINARY: ":all:"
 
 jobs:
   test:
-    runs-on: ubuntu-latest
+    runs-on: ${{ matrix.os }}
 
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         include:
           # version number must be string, otherwise 3.10 becomes 3.1
           - os: windows-latest
             python-version: "3.12"
           - os: ubuntu-latest
             python-version: "3.10"
           - os: macos-latest
-            python-version: "3.8"
+            python-version: "3.9"
       fail-fast: false
     steps:
     - uses: actions/checkout@v4
     - uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - run: python -m pip install --upgrade pip
@@ -39,8 +39,8 @@
 
     # toml is needed only by coveralls
     - if: ${{ matrix.os == 'ubuntu-latest' }}
       run: |
         python -m pip install toml
         JUPYTER_PLATFORM_DIRS=1 coverage run -m pytest
     - if: ${{ matrix.os == 'ubuntu-latest' }}
-      uses: AndreMiras/coveralls-python-action@develop
+      uses: coverallsapp/github-action@v2
```

### Comparing `resample-1.8.2/.pre-commit-config.yaml` & `resample-1.9.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,24 +14,24 @@
   - id: mixed-line-ending
   - id: sort-simple-yaml
   - id: file-contents-sorter
   - id: trailing-whitespace
 
 # Ruff linter, replacement for flake8, isort, pydocstyle
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: 'v0.3.7'
+  rev: 'v0.4.3'
   hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
 # Python formatting
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 24.4.0
+  rev: 24.4.2
   hooks:
   - id: black
 
 # Python type checking
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: 'v1.9.0'
+  rev: 'v1.10.0'
   hooks:
   - id: mypy
     args: [--allow-redefinition, --ignore-missing-imports]
```

### Comparing `resample-1.8.2/CITATION.cff` & `resample-1.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/LICENSE` & `resample-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/PKG-INFO` & `resample-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.8.2
+Version: 1.9.0
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy>=1.21
 Requires-Dist: scipy>=1.10
```

### Comparing `resample-1.8.2/README.rst` & `resample-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/benchmarks/test_bootstrap.py` & `resample-1.9.0/benchmarks/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/benchmarks/test_jackknife.py` & `resample-1.9.0/benchmarks/test_jackknife.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/benchmarks/test_rcont.py` & `resample-1.9.0/benchmarks/test_rcont.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/benchmarks/test_usp.py` & `resample-1.9.0/benchmarks/test_usp.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/Makefile` & `resample-1.9.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/_static/logo.svg` & `resample-1.9.0/doc/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/bench_rcont.json` & `resample-1.9.0/doc/bench_rcont.json`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/changelog.rst` & `resample-1.9.0/doc/changelog.rst`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/conf.py` & `resample-1.9.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/example/tag_and_probe.ipynb` & `resample-1.9.0/doc/example/tag_and_probe.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/make.bat` & `resample-1.9.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/make_raw_logo.py` & `resample-1.9.0/doc/make_raw_logo.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/plot_bench.py` & `resample-1.9.0/doc/plot_bench.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/confidence_intervals.ipynb` & `resample-1.9.0/doc/tutorial/confidence_intervals.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/jackknife_vs_bootstrap.ipynb` & `resample-1.9.0/doc/tutorial/jackknife_vs_bootstrap.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/permutation_tests.ipynb` & `resample-1.9.0/doc/tutorial/permutation_tests.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/sklearn.ipynb` & `resample-1.9.0/doc/tutorial/sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/usp_continuous_data.ipynb` & `resample-1.9.0/doc/tutorial/usp_continuous_data.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/doc/tutorial/variance_fit_parameters.ipynb` & `resample-1.9.0/doc/tutorial/variance_fit_parameters.ipynb`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/pyproject.toml` & `resample-1.9.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     "Programming Language :: Python :: 3",
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3.12',
     'Programming Language :: Python :: Implementation :: CPython',
     'Programming Language :: Python :: Implementation :: PyPy',
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "http://github.com/resample-project/resample"
@@ -45,18 +46,21 @@
 [tool.setuptools_scm]
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.ruff]
-select = ["E", "F", "W", "D"]
+extend-select = ["E", "F", "W", "D"]
 ignore = ["D212", "D203"]
 unfixable = ["ERA"]
 
+[tool.ruff.per-file-ignores]
+"test_*.py" = ["D"]
+
 [tool.mypy]
 strict = true
 no_implicit_optional = false
 allow_redefinition = true
 ignore_missing_imports = true
 show_error_codes = true
 files = "src/resample/*.py"
```

### Comparing `resample-1.8.2/src/resample/__init__.py` & `resample-1.9.0/src/resample/__init__.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/src/resample/_util.py` & `resample-1.9.0/src/resample/_util.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/src/resample/bootstrap.py` & `resample-1.9.0/src/resample/bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/src/resample/empirical.py` & `resample-1.9.0/src/resample/empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/src/resample/jackknife.py` & `resample-1.9.0/src/resample/jackknife.py`

 * *Files 10% similar despite different names*

```diff
@@ -315,7 +315,44 @@
     """
     # formula is (n - 1) / n * sum((fj - mean(fj)) ** 2)
     #   = np.var(fj, ddof=0) * (n - 1)
     sample = np.atleast_1d(sample)
     thetas = jackknife(fn, sample, *args)
     n = len(sample)
     return (n - 1) * np.var(thetas, ddof=0, axis=0)
+
+
+def cross_validation(
+    predict: Callable[..., float], x: "ArrayLike", y: "ArrayLike", *args: "ArrayLike"
+) -> float:
+    """
+    Calculate mean-squared error of model with leave-one-out-cross-validation.
+
+    Wikipedia:
+    https://en.wikipedia.org/wiki/Cross-validation_(statistics)
+
+    Parameters
+    ----------
+    predict : callable
+        Function with the signature (x_in, y_in, x_out, *args). It takes x_in, y_in,
+        which are arrays with the same length. x_out should be one element of the x
+        array. *args are further optional arguments for the function. The function
+        should return the prediction y(x_out).
+    x : array-like
+        Explanatory variable. Must be an array of shape (N, ...), where N is the number
+        of samples.
+    y : array-like
+        Observations. Must be an array of shape (N, ...).
+    *args:
+        Optional arguments which are passed unmodified to predict.
+
+    Returns
+    -------
+    float
+        Variance of the difference (y[i] - predict(..., x[i], *args)).
+
+    """
+    deltas = []
+    for i, (x_in, y_in) in enumerate(resample(x, y, copy=False)):
+        yip = predict(x_in, y_in, x[i], *args)
+        deltas.append((y[i] - yip))
+    return np.var(deltas)  # type:ignore
```

### Comparing `resample-1.8.2/src/resample/permutation.py` & `resample-1.9.0/src/resample/permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/src/resample.egg-info/PKG-INFO` & `resample-1.9.0/src/resample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resample
-Version: 1.8.2
+Version: 1.9.0
 Summary: Resampling-based inference in Python
 Author-email: Daniel Saxton <dsaxton@pm.me>, Hans Dembinski <hans.dembinski@gmail.com>
 License: BSD-3-Clause
 Project-URL: repository, http://github.com/resample-project/resample
 Project-URL: documentation, https://resample.readthedocs.io/en/stable/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy>=1.21
 Requires-Dist: scipy>=1.10
```

### Comparing `resample-1.8.2/src/resample.egg-info/SOURCES.txt` & `resample-1.9.0/src/resample.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 doc/plot_bench.py
 doc/reference.rst
 doc/tutorials.rst
 doc/_static/logo.svg
 doc/example/tag_and_probe.ipynb
 doc/tutorial/confidence_intervals.ipynb
 doc/tutorial/jackknife_vs_bootstrap.ipynb
+doc/tutorial/leave-one-out-cross-validation.ipynb
 doc/tutorial/permutation_tests.ipynb
 doc/tutorial/sklearn.ipynb
 doc/tutorial/usp_continuous_data.ipynb
 doc/tutorial/variance_fit_parameters.ipynb
 src/resample/__init__.py
 src/resample/_util.py
 src/resample/bootstrap.py
```

### Comparing `resample-1.8.2/tests/test_bootstrap.py` & `resample-1.9.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/tests/test_empirical.py` & `resample-1.9.0/tests/test_empirical.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/tests/test_jackknife.py` & `resample-1.9.0/tests/test_jackknife.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import numpy as np
 import pytest
 from numpy.testing import assert_almost_equal, assert_equal
-
-from resample.jackknife import bias, bias_corrected, jackknife, resample, variance
+from scipy.optimize import curve_fit
+from resample.jackknife import (
+    bias,
+    bias_corrected,
+    jackknife,
+    resample,
+    variance,
+    cross_validation,
+)
 
 
 def test_resample_1d():
     data = (1, 2, 3)
 
     r = []
     for x in resample(data):
@@ -116,7 +123,26 @@
         r = list(resample(data, False))
 
     assert_equal(r, list(resample(data, copy=False)))
 
     with pytest.warns(VisibleDeprecationWarning):
         with pytest.raises(ValueError):  # too many arguments
             resample(data, True, 1)
+
+
+@pytest.mark.filterwarnings("ignore:Covariance")
+def test_cross_validation():
+    x = [1, 2, 3]
+    y = [3, 4, 5]
+
+    def predict(xi, yi, xo, npar):
+        def model(x, *par):
+            return np.polyval(par, x)
+
+        popt = curve_fit(model, xi, yi, p0=np.zeros(npar))[0]
+        return model(xo, *popt)
+
+    v = cross_validation(predict, x, y, 2)
+    assert v == pytest.approx(0)
+
+    v2 = cross_validation(predict, x, y, 1)
+    assert v2 == pytest.approx(1.5)
```

### Comparing `resample-1.8.2/tests/test_permutation.py` & `resample-1.9.0/tests/test_permutation.py`

 * *Files identical despite different names*

### Comparing `resample-1.8.2/tests/test_util.py` & `resample-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

