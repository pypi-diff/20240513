# Comparing `tmp/cads_api_client-1.0.1.tar.gz` & `tmp/cads_api_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cads_api_client-1.0.1.tar", last modified: Fri May 10 12:58:06 2024, max compression
+gzip compressed data, was "cads_api_client-1.0.2.tar", last modified: Mon May 13 12:26:19 2024, max compression
```

## Comparing `cads_api_client-1.0.1.tar` & `cads_api_client-1.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.506692 cads_api_client-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.506692 cads_api_client-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.github/workflows/on-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.pre-commit-config-cruft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/cads_api_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/cads_api_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/cads_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-10 12:58:06.000000 cads_api_client-1.0.1/cads_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/ci/environment-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/ci/environment-integration.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.510692 cads_api_client-1.0.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_client_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_constraints_test.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_filters_and_pagination_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/notebooks/cads_api_licences_tests.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:58:06.514692 cads_api_client-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_10_catalogue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_20_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_30_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_40_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/integration_test_50_legacy_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_00_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_10_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-10 12:57:57.000000 cads_api_client-1.0.1/tests/test_10_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.743149 cads_api_client-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.github/workflows/on-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8827 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.pre-commit-config-cruft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/cads_api_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/cads_api_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/cads_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16585 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 12:26:19.000000 cads_api_client-1.0.2/cads_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.747149 cads_api_client-1.0.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/ci/environment-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/ci/environment-integration.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    15779 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_client_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_constraints_test.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12254 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_filters_and_pagination_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/notebooks/cads_api_licences_tests.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:19.751149 cads_api_client-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_10_catalogue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_20_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_30_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_40_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/integration_test_50_legacy_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_00_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_10_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14768 2024-05-13 12:26:11.000000 cads_api_client-1.0.2/tests/test_10_processing.py
```

### Comparing `cads_api_client-1.0.1/.cruft.json` & `cads_api_client-1.0.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/.github/workflows/on-push.yml` & `cads_api_client-1.0.2/.github/workflows/on-push.yml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/.gitignore` & `cads_api_client-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/.pre-commit-config.yaml` & `cads_api_client-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/LICENSE` & `cads_api_client-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/Makefile` & `cads_api_client-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/PKG-INFO` & `cads_api_client-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.1/README.md` & `cads_api_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client/__init__.py` & `cads_api_client-1.0.2/cads_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client/api_client.py` & `cads_api_client-1.0.2/cads_api_client/api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client/catalogue.py` & `cads_api_client-1.0.2/cads_api_client/catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client/config.py` & `cads_api_client-1.0.2/cads_api_client/config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client/legacy_api_client.py` & `cads_api_client-1.0.2/cads_api_client/legacy_api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 
 import cdsapi.api
 import requests
 
 from . import api_client, processing
 
 LEGACY_KWARGS = [
-    "quiet",
-    "debug",
     "verify",
     "timeout",
     "progress",
     "full_stack",
     "delete",
     "retry_max",
     "sleep_max",
@@ -68,14 +66,16 @@
 
 
 class LegacyApiClient(cdsapi.api.Client):  # type: ignore[misc]
     def __init__(
         self,
         url: str | None = None,
         key: str | None = None,
+        quiet: bool = False,
+        debug: bool = False,
         *args: Any,
         **kwargs: Any,
     ) -> None:
         kwargs.update(zip(LEGACY_KWARGS, args))
 
         self.url, self.key, _ = cdsapi.api.get_url_key_verify(url, key, None)
         self.session = kwargs.pop("session", requests.Session())
@@ -90,16 +90,16 @@
         self.timeout = kwargs.pop("timeout", 60)
         self.retry_max = kwargs.pop("retry_max", 500)
         self.retry_options = {
             "maximum_tries": self.retry_max,
             "retry_after": self.sleep_max,
         }
 
-        self.quiet = kwargs.pop("quiet", False)
-        self._debug = kwargs.pop("debug", False)
+        self.quiet = quiet
+        self._debug = debug
 
         if kwargs:
             warnings.warn(
                 "This is a beta version."
                 f" The following parameters have not been implemented yet: {kwargs}.",
                 UserWarning,
             )
```

### Comparing `cads_api_client-1.0.1/cads_api_client/processing.py` & `cads_api_client-1.0.2/cads_api_client/processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,20 +232,16 @@
     def wait_on_result(self, retry_options: Dict[str, Any] = {}) -> None:
         sleep = 1.0
         status = None
         while True:
             if status != (status := self._robust_status(retry_options=retry_options)):
                 logger.info(f"status has been updated to {status}")
             if status == "successful":
-                # workaround for the server-side 404 due to database replicas out od sync
-                time.sleep(1)
                 break
             elif status == "failed":
-                # workaround for the server-side 404 due to database replicas out od sync
-                time.sleep(1)
                 results = multiurl.robust(self.make_results, **retry_options)(self.url)
                 raise ProcessingFailedError(error_json_to_message(results.json))
             elif status in ("accepted", "running"):
                 sleep *= 1.5
                 if sleep > self.sleep_max:
                     sleep = self.sleep_max
             else:
```

### Comparing `cads_api_client-1.0.1/cads_api_client/profile.py` & `cads_api_client-1.0.2/cads_api_client/profile.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/cads_api_client.egg-info/PKG-INFO` & `cads_api_client-1.0.2/cads_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cads-api-client
-Version: 1.0.1
+Version: 1.0.2
 Summary: CADS API Python client
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `cads_api_client-1.0.1/cads_api_client.egg-info/SOURCES.txt` & `cads_api_client-1.0.2/cads_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/docs/Makefile` & `cads_api_client-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/docs/conf.py` & `cads_api_client-1.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/docs/make.bat` & `cads_api_client-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/notebooks/cads_api_client_test.ipynb` & `cads_api_client-1.0.2/notebooks/cads_api_client_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/notebooks/cads_api_constraints_test.ipynb` & `cads_api_client-1.0.2/notebooks/cads_api_constraints_test.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/notebooks/cads_api_filters_and_pagination_tests.ipynb` & `cads_api_client-1.0.2/notebooks/cads_api_filters_and_pagination_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/notebooks/cads_api_licences_tests.ipynb` & `cads_api_client-1.0.2/notebooks/cads_api_licences_tests.ipynb`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/pyproject.toml` & `cads_api_client-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/conftest.py` & `cads_api_client-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/integration_test_10_catalogue.py` & `cads_api_client-1.0.2/tests/integration_test_10_catalogue.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/integration_test_20_processing.py` & `cads_api_client-1.0.2/tests/integration_test_20_processing.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/integration_test_30_remote.py` & `cads_api_client-1.0.2/tests/integration_test_30_remote.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/integration_test_40_api_client.py` & `cads_api_client-1.0.2/tests/integration_test_40_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/integration_test_50_legacy_api_client.py` & `cads_api_client-1.0.2/tests/integration_test_50_legacy_api_client.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/test_10_config.py` & `cads_api_client-1.0.2/tests/test_10_config.py`

 * *Files identical despite different names*

### Comparing `cads_api_client-1.0.1/tests/test_10_processing.py` & `cads_api_client-1.0.2/tests/test_10_processing.py`

 * *Files identical despite different names*

