# Comparing `tmp/pynajax-0.1.1.tar.gz` & `tmp/pynajax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynajax-0.1.1.tar", last modified: Wed May  8 14:52:59 2024, max compression
+gzip compressed data, was "pynajax-0.1.2.tar", last modified: Mon May 13 16:58:31 2024, max compression
```

## Comparing `pynajax-0.1.1.tar` & `pynajax-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.850229 pynajax-0.1.1/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.587388 pynajax-0.1.1/.github/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.637243 pynajax-0.1.1/.github/workflows/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1423 2024-05-08 14:38:55.000000 pynajax-0.1.1/.github/workflows/ci.yml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3077 2024-04-03 20:32:36.000000 pynajax-0.1.1/.gitignore
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1069 2024-04-03 20:32:36.000000 pynajax-0.1.1/LICENSE
--rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4504 2024-05-08 14:52:59.845062 pynajax-0.1.1/PKG-INFO
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1955 2024-05-08 14:38:55.000000 pynajax-0.1.1/README.md
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.654775 pynajax-0.1.1/docs/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.683219 pynajax-0.1.1/docs/examples/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      710 2024-05-08 02:28:34.000000 pynajax-0.1.1/docs/examples/README.md
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1707 2024-05-08 02:28:34.000000 pynajax-0.1.1/docs/examples/plot_benchmark_bin_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1524 2024-05-08 02:28:34.000000 pynajax-0.1.1/docs/examples/plot_benchmark_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1940 2024-05-08 14:38:55.000000 pynajax-0.1.1/docs/examples/plot_benchmark_event_trigger_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1610 2024-05-08 02:28:34.000000 pynajax-0.1.1/docs/examples/plot_benchmark_threshold.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      821 2024-05-08 02:28:34.000000 pynajax-0.1.1/docs/gallery_conf.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1762 2024-04-03 20:32:36.000000 pynajax-0.1.1/docs/gen_ref_pages.py
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.688953 pynajax-0.1.1/docs/images/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    38967 2024-05-08 14:38:55.000000 pynajax-0.1.1/docs/images/convolve_benchmark.png
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1943 2024-05-08 14:38:55.000000 pynajax-0.1.1/docs/index.md
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.694920 pynajax-0.1.1/docs/javascripts/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      384 2024-04-03 20:32:36.000000 pynajax-0.1.1/docs/javascripts/katex.js
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     2012 2024-05-08 02:28:34.000000 pynajax-0.1.1/mkdocs.yml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1407 2024-05-08 02:28:34.000000 pynajax-0.1.1/noxfile.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3020 2024-05-08 02:28:34.000000 pynajax-0.1.1/pyproject.toml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       38 2024-05-08 14:52:59.851205 pynajax-0.1.1/setup.cfg
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.597929 pynajax-0.1.1/src/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.757401 pynajax-0.1.1/src/pynajax/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      112 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/__init__.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5592 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/jax_core_bin_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6148 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/jax_core_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1437 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/jax_core_threshold.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6927 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/jax_process_perievent.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     8469 2024-05-08 02:28:34.000000 pynajax-0.1.1/src/pynajax/utils.py
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.832437 pynajax-0.1.1/src/pynajax.egg-info/
--rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4504 2024-05-08 14:52:59.764191 pynajax-0.1.1/src/pynajax.egg-info/PKG-INFO
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      948 2024-05-08 14:52:59.000000 pynajax-0.1.1/src/pynajax.egg-info/SOURCES.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        1 2024-05-08 14:52:59.000000 pynajax-0.1.1/src/pynajax.egg-info/dependency_links.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      282 2024-05-08 14:52:59.000000 pynajax-0.1.1/src/pynajax.egg-info/requires.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        8 2024-05-08 14:52:59.000000 pynajax-0.1.1/src/pynajax.egg-info/top_level.txt
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-08 14:52:59.826226 pynajax-0.1.1/tests/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       18 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/__init__.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      546 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/conftest.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1438 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/mock.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5237 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/test_jax_core_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     4373 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/test_jax_core_perievent.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    16141 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/test_jax_numpy_compatibility.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      111 2024-05-08 02:28:34.000000 pynajax-0.1.1/tests/test_pynapple.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.385098 pynajax-0.1.2/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.157584 pynajax-0.1.2/.github/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.204484 pynajax-0.1.2/.github/workflows/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1416 2024-05-13 16:44:00.000000 pynajax-0.1.2/.github/workflows/ci.yml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3077 2024-04-03 20:32:36.000000 pynajax-0.1.2/.gitignore
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1069 2024-04-03 20:32:36.000000 pynajax-0.1.2/LICENSE
+-rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-13 16:58:31.380343 pynajax-0.1.2/PKG-INFO
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1988 2024-05-13 16:44:08.000000 pynajax-0.1.2/README.md
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.222247 pynajax-0.1.2/docs/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.250811 pynajax-0.1.2/docs/examples/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      710 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/README.md
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1707 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_bin_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1524 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1940 2024-05-08 14:38:55.000000 pynajax-0.1.2/docs/examples/plot_benchmark_event_trigger_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1610 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_threshold.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      821 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/gallery_conf.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1762 2024-04-03 20:32:36.000000 pynajax-0.1.2/docs/gen_ref_pages.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.256562 pynajax-0.1.2/docs/images/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    38967 2024-05-08 14:38:55.000000 pynajax-0.1.2/docs/images/convolve_benchmark.png
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1977 2024-05-13 16:44:08.000000 pynajax-0.1.2/docs/index.md
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.262682 pynajax-0.1.2/docs/javascripts/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      384 2024-04-03 20:32:36.000000 pynajax-0.1.2/docs/javascripts/katex.js
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     2012 2024-05-08 02:28:34.000000 pynajax-0.1.2/mkdocs.yml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1407 2024-05-08 02:28:34.000000 pynajax-0.1.2/noxfile.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3194 2024-05-13 16:58:08.000000 pynajax-0.1.2/pyproject.toml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       38 2024-05-13 16:58:31.386071 pynajax-0.1.2/setup.cfg
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.168317 pynajax-0.1.2/src/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.295817 pynajax-0.1.2/src/pynajax/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      112 2024-05-13 16:58:08.000000 pynajax-0.1.2/src/pynajax/__init__.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5592 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_bin_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6148 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1437 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_threshold.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6928 2024-05-13 16:44:00.000000 pynajax-0.1.2/src/pynajax/jax_process_perievent.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     8469 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/utils.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.368364 pynajax-0.1.2/src/pynajax.egg-info/
+-rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-13 16:58:31.302780 pynajax-0.1.2/src/pynajax.egg-info/PKG-INFO
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      948 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/SOURCES.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        1 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/dependency_links.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      282 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/requires.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        8 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/top_level.txt
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.362108 pynajax-0.1.2/tests/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       18 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/__init__.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      546 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/conftest.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1438 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/mock.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5237 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_jax_core_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5256 2024-05-13 16:44:00.000000 pynajax-0.1.2/tests/test_jax_core_perievent.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    16141 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_jax_numpy_compatibility.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      111 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_pynapple.py
```

### Comparing `pynajax-0.1.1/.github/workflows/ci.yml` & `pynajax-0.1.2/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install .[dev]
 
       - name: Clone and install pynapple
         run: |
-          git clone -b dev https://github.com/pynapple-org/pynapple.git ../pynapple
+          git clone https://github.com/pynapple-org/pynapple.git ../pynapple
           pip install -e ../pynapple
 
       - name: Run nox
         run: |
           nox
 
       - name: Coveralls
```

### Comparing `pynajax-0.1.1/.gitignore` & `pynajax-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/LICENSE` & `pynajax-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/PKG-INFO` & `pynajax-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynajax
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JAX backend for pynapple.
 Author: pynajax authors
 License: MIT License
         
         Copyright (c) 2024 pynapple-org
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,15 +59,16 @@
 
 # pynajax
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/pynapple-org/pynajax/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![pynajax CI](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml/badge.svg)](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg?branch=main)](https://coveralls.io/github/pynapple-org/pynajax?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg)](https://coveralls.io/github/pynapple-org/pynajax)
+![PyPI - Version](https://img.shields.io/pypi/v/pynajax)
 
 Welcome to `pynajax`, a GPU accelerated backend for [pynapple](https://github.com/pynapple-org/pynapple) built on top on [jax](https://github.com/google/jax). It offers a fast acceleration for the core pynapple functions using GPU. 
 
 > **Warning**
 > ⚠️ This package is not meant to be used on its own. It should only be used through the pynapple API.
 
 ## Installation
```

### Comparing `pynajax-0.1.1/README.md` & `pynajax-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pynajax
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/pynapple-org/pynajax/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![pynajax CI](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml/badge.svg)](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg?branch=main)](https://coveralls.io/github/pynapple-org/pynajax?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg)](https://coveralls.io/github/pynapple-org/pynajax)
+![PyPI - Version](https://img.shields.io/pypi/v/pynajax)
 
 Welcome to `pynajax`, a GPU accelerated backend for [pynapple](https://github.com/pynapple-org/pynapple) built on top on [jax](https://github.com/google/jax). It offers a fast acceleration for the core pynapple functions using GPU. 
 
 > **Warning**
 > ⚠️ This package is not meant to be used on its own. It should only be used through the pynapple API.
 
 ## Installation
```

### Comparing `pynajax-0.1.1/docs/examples/README.md` & `pynajax-0.1.2/docs/examples/README.md`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/examples/plot_benchmark_bin_average.py` & `pynajax-0.1.2/docs/examples/plot_benchmark_bin_average.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/examples/plot_benchmark_convolve.py` & `pynajax-0.1.2/docs/examples/plot_benchmark_convolve.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/examples/plot_benchmark_event_trigger_average.py` & `pynajax-0.1.2/docs/examples/plot_benchmark_event_trigger_average.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/examples/plot_benchmark_threshold.py` & `pynajax-0.1.2/docs/examples/plot_benchmark_threshold.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/gallery_conf.py` & `pynajax-0.1.2/docs/gallery_conf.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/gen_ref_pages.py` & `pynajax-0.1.2/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/images/convolve_benchmark.png` & `pynajax-0.1.2/docs/images/convolve_benchmark.png`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/docs/index.md` & `pynajax-0.1.2/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pynajax 
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/pynapple-org/pynajax/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![pynajax CI](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml/badge.svg)](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg?branch=main)](https://coveralls.io/github/pynapple-org/pynajax?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg)](https://coveralls.io/github/pynapple-org/pynajax)
+![PyPI - Version](https://img.shields.io/pypi/v/pynajax)
 
 Welcome to `pynajax`, a GPU accelerated backend for [pynapple](https://github.com/pynapple-org/pynapple) built on top on [jax](https://github.com/google/jax). It offers a fast acceleration for the core pynapple functions using GPU. 
 
 
 !!! warning
 
     This package is not meant to be used on its own. It should only be used through the pynapple API.
@@ -50,8 +51,8 @@
 
 ## Benchmark
 
 This benchmark for the `convolve` function was run on a GPU.
 
 ![benchmark_convolve](./images/convolve_benchmark.png)
 
-See the documentation for others benchmarks.
+See the documentation for others benchmarks.
```

### Comparing `pynajax-0.1.1/mkdocs.yml` & `pynajax-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/noxfile.py` & `pynajax-0.1.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/pyproject.toml` & `pynajax-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pynajax"
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name = "pynajax authors"}]
 description = "A JAX backend for pynapple."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["neuroscience", "jax-backend", "pynapple"]
 license = { file = "LICENSE" }
 classifiers = [
@@ -106,7 +106,15 @@
 # overlap with the use of a formatter, like Black, but we can override this behavior by
 # explicitly adding the rule.
 extend-select = ["F", "W", "B", "I"]
 ignore = ["E731"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
+
+[tool.coverage.report] # Numba compiled functions
+exclude_also = [
+    "def _get_bin_edges",
+    "def _get_mask_and_count",
+    "def _get_idxs",
+    "def _get_slicing"    
+]
```

### Comparing `pynajax-0.1.1/src/pynajax/jax_core_bin_average.py` & `pynajax-0.1.2/src/pynajax/jax_core_bin_average.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/src/pynajax/jax_core_convolve.py` & `pynajax-0.1.2/src/pynajax/jax_core_convolve.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/src/pynajax/jax_core_threshold.py` & `pynajax-0.1.2/src/pynajax/jax_core_threshold.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/src/pynajax/jax_process_perievent.py` & `pynajax-0.1.2/src/pynajax/jax_process_perievent.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,17 +141,16 @@
     res = res.reshape(*res.shape[:-2], -1)  # flatten features
 
     extra_elements = data_array.shape[1] % batch_size
     if extra_elements:
         # compute residual slice
         slc = data_array[:, -extra_elements:]
         slc = jnp.full((tot_size, *slc.shape[1:]), np.nan).at[ix_shift].set(slc[ix_orig])
-
         resid = _dot_prod_feature(count_array, slc)
-        resid = resid.transpose(1, 2, 0).reshape(*res.shape[:-1], -1)
+        # resid = resid.transpose(1, 2, 0).reshape(*res.shape[:-1], -1)
         res = np.concatenate([res, resid], axis=2)
 
     # reshape back to original
     res = res.reshape((np.sum(windows) + 1, count_array.shape[-1], *shape[1:]))
 
     res = jnp.apply_along_axis(jnp.divide, 1, res, tot_count)
```

### Comparing `pynajax-0.1.1/src/pynajax/utils.py` & `pynajax-0.1.2/src/pynajax/utils.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/src/pynajax.egg-info/PKG-INFO` & `pynajax-0.1.2/src/pynajax.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynajax
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JAX backend for pynapple.
 Author: pynajax authors
 License: MIT License
         
         Copyright (c) 2024 pynapple-org
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -59,15 +59,16 @@
 
 # pynajax
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/pynapple-org/pynajax/blob/main/LICENSE)
 ![Python version](https://img.shields.io/badge/python-3.10-blue.svg)
 [![Project Status: Active – The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![pynajax CI](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml/badge.svg)](https://github.com/pynapple-org/pynajax/actions/workflows/ci.yml)
-[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg?branch=main)](https://coveralls.io/github/pynapple-org/pynajax?branch=main)
+[![Coverage Status](https://coveralls.io/repos/github/pynapple-org/pynajax/badge.svg)](https://coveralls.io/github/pynapple-org/pynajax)
+![PyPI - Version](https://img.shields.io/pypi/v/pynajax)
 
 Welcome to `pynajax`, a GPU accelerated backend for [pynapple](https://github.com/pynapple-org/pynapple) built on top on [jax](https://github.com/google/jax). It offers a fast acceleration for the core pynapple functions using GPU. 
 
 > **Warning**
 > ⚠️ This package is not meant to be used on its own. It should only be used through the pynapple API.
 
 ## Installation
```

### Comparing `pynajax-0.1.1/src/pynajax.egg-info/SOURCES.txt` & `pynajax-0.1.2/src/pynajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/tests/conftest.py` & `pynajax-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/tests/mock.py` & `pynajax-0.1.2/tests/mock.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/tests/test_jax_core_convolve.py` & `pynajax-0.1.2/tests/test_jax_core_convolve.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.1/tests/test_jax_numpy_compatibility.py` & `pynajax-0.1.2/tests/test_jax_numpy_compatibility.py`

 * *Files identical despite different names*

