# Comparing `tmp/adafruit-circuitpython-bme680-3.7.4.tar.gz` & `tmp/adafruit_circuitpython_bme680-3.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bme680-3.7.4.tar", last modified: Sat Dec 23 16:47:23 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_bme680-3.7.5.tar", last modified: Mon May 13 13:19:18 2024, max compression
```

## Comparing `adafruit-circuitpython-bme680-3.7.4.tar` & `adafruit_circuitpython_bme680-3.7.5.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.486342 adafruit-circuitpython-bme680-3.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.490342 adafruit-circuitpython-bme680-3.7.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.490342 adafruit-circuitpython-bme680-3.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.490342 adafruit-circuitpython-bme680-3.7.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)    28054 2023-12-23 16:47:16.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_bme680.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2023-12-23 16:47:23.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2023-12-23 16:47:23.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-23 16:47:23.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-23 16:47:23.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-23 16:47:23.000000 adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.490342 adafruit-circuitpython-bme680-3.7.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-23 16:47:16.000000 adafruit-circuitpython-bme680-3.7.4/examples/bme680_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-23 16:47:16.000000 adafruit-circuitpython-bme680-3.7.4/examples/bme680_spi.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-12-23 16:47:16.000000 adafruit-circuitpython-bme680-3.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-23 16:47:08.000000 adafruit-circuitpython-bme680-3.7.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-23 16:47:23.494342 adafruit-circuitpython-bme680-3.7.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.492548 adafruit_circuitpython_bme680-3.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.480548 adafruit_circuitpython_bme680-3.7.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.484548 adafruit_circuitpython_bme680-3.7.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.484548 adafruit_circuitpython_bme680-3.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)    28054 2024-05-13 13:19:15.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_bme680.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-13 13:19:18.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 13:19:18.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:19:18.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:19:18.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 13:19:18.000000 adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:19:18.488548 adafruit_circuitpython_bme680-3.7.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-13 13:19:15.000000 adafruit_circuitpython_bme680-3.7.5/examples/bme680_displayio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 13:19:15.000000 adafruit_circuitpython_bme680-3.7.5/examples/bme680_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 13:19:15.000000 adafruit_circuitpython_bme680-3.7.5/examples/bme680_spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 13:19:15.000000 adafruit_circuitpython_bme680-3.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 13:19:07.000000 adafruit_circuitpython_bme680-3.7.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:19:18.492548 adafruit_circuitpython_bme680-3.7.5/setup.cfg
```

### Comparing `adafruit-circuitpython-bme680-3.7.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_bme680-3.7.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/.gitignore` & `adafruit_circuitpython_bme680-3.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/.pre-commit-config.yaml` & `adafruit_circuitpython_bme680-3.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/.pylintrc` & `adafruit_circuitpython_bme680-3.7.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_bme680-3.7.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/LICENSE` & `adafruit_circuitpython_bme680-3.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/LICENSES/BSD-3-Clause.txt` & `adafruit_circuitpython_bme680-3.7.5/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_bme680-3.7.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/LICENSES/MIT.txt` & `adafruit_circuitpython_bme680-3.7.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/LICENSES/Unlicense.txt` & `adafruit_circuitpython_bme680-3.7.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/PKG-INFO` & `adafruit_circuitpython_bme680-3.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.7.4
+Version: 3.7.5
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.7.4/README.rst` & `adafruit_circuitpython_bme680-3.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/adafruit_bme680.py` & `adafruit_circuitpython_bme680-3.7.5/adafruit_bme680.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     from circuitpython_typing import ReadableBuffer
     from busio import I2C, SPI
     from digitalio import DigitalInOut
 
 except ImportError:
     pass
 
-__version__ = "3.7.4"
+__version__ = "3.7.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BME680.git"
 
 
 #    I2C ADDRESS/BITS/SETTINGS NEW
 #    -----------------------------------------------------------------------
 _BME68X_ENABLE_HEATER = const(0x00)
 _BME68X_DISABLE_HEATER = const(0x01)
```

### Comparing `adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/PKG-INFO` & `adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bme680
-Version: 3.7.4
+Version: 3.7.5
 Summary: CircuitPython driver for BME680 sensor over I2C
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BME680
 Keywords: adafruit,blinka,circuitpython,micropython,bme680,hardware,temperature,pressure,humidity,gas
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bme680-3.7.4/adafruit_circuitpython_bme680.egg-info/SOURCES.txt` & `adafruit_circuitpython_bme680-3.7.5/adafruit_circuitpython_bme680.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -30,9 +30,10 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/bme680_displayio_simpletest.py
 examples/bme680_simpletest.py
 examples/bme680_spi.py
```

### Comparing `adafruit-circuitpython-bme680-3.7.4/docs/_static/favicon.ico` & `adafruit_circuitpython_bme680-3.7.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/docs/conf.py` & `adafruit_circuitpython_bme680-3.7.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/docs/index.rst` & `adafruit_circuitpython_bme680-3.7.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/examples/bme680_simpletest.py` & `adafruit_circuitpython_bme680-3.7.5/examples/bme680_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/examples/bme680_spi.py` & `adafruit_circuitpython_bme680-3.7.5/examples/bme680_spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bme680-3.7.4/pyproject.toml` & `adafruit_circuitpython_bme680-3.7.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bme680"
 description = "CircuitPython driver for BME680 sensor over I2C"
-version = "3.7.4"
+version = "3.7.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BME680"}
 keywords = [
     "adafruit",
```

