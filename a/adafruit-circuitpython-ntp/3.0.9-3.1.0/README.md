# Comparing `tmp/adafruit-circuitpython-ntp-3.0.9.tar.gz` & `tmp/adafruit_circuitpython_ntp-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ntp-3.0.9.tar", last modified: Fri May 26 15:54:49 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_ntp-3.1.0.tar", last modified: Mon May 13 13:20:07 2024, max compression
```

## Comparing `adafruit-circuitpython-ntp-3.0.9.tar` & `adafruit_circuitpython_ntp-3.1.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.856985 adafruit-circuitpython-ntp-3.0.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.856985 adafruit-circuitpython-ntp-3.0.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.856985 adafruit-circuitpython-ntp-3.0.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.856985 adafruit-circuitpython-ntp-3.0.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-05-26 15:54:49.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 15:54:49.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:54:49.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 15:54:49.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:54:49.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-26 15:54:42.000000 adafruit-circuitpython-ntp-3.0.9/adafruit_ntp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-26 15:54:42.000000 adafruit-circuitpython-ntp-3.0.9/examples/ntp_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-26 15:54:42.000000 adafruit-circuitpython-ntp-3.0.9/examples/ntp_set_rtc.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-26 15:54:42.000000 adafruit-circuitpython-ntp-3.0.9/examples/ntp_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-26 15:54:42.000000 adafruit-circuitpython-ntp-3.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 15:54:32.000000 adafruit-circuitpython-ntp-3.0.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:54:49.860985 adafruit-circuitpython-ntp-3.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.436174 adafruit_circuitpython_ntp-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 13:20:07.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/adafruit_ntp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.440174 adafruit_circuitpython_ntp-3.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_set_rtc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/examples/ntp_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-13 13:20:05.000000 adafruit_circuitpython_ntp-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-13 13:19:58.000000 adafruit_circuitpython_ntp-3.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:20:07.444174 adafruit_circuitpython_ntp-3.1.0/setup.cfg
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_ntp-3.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/.gitignore` & `adafruit_circuitpython_ntp-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/.pre-commit-config.yaml` & `adafruit_circuitpython_ntp-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/.pylintrc` & `adafruit_circuitpython_ntp-3.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_ntp-3.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/LICENSE` & `adafruit_circuitpython_ntp-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_ntp-3.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/LICENSES/MIT.txt` & `adafruit_circuitpython_ntp-3.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_ntp-3.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/PKG-INFO` & `adafruit_circuitpython_ntp-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ntp
-Version: 3.0.9
+Version: 3.1.0
 Summary: Network Time Protocol (NTP) helper for Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NTP
 Keywords: adafruit,blinka,circuitpython,micropython,ntp,ntp,,network,,time
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Provides-Extra: optional
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ntp/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ntp/en/latest/
     :alt: Documentation Status
@@ -73,29 +74,25 @@
     pip3 install adafruit-circuitpython-ntp
 
 Usage Example
 =============
 
 .. code-block:: python
 
+    import adafruit_connection_manager
     import adafruit_ntp
-    import socketpool
+    import os
     import time
     import wifi
 
-    # Get wifi details and more from a secrets.py file
-    try:
-        from secrets import secrets
-    except ImportError:
-        print("WiFi secrets are kept in secrets.py, please add them there!")
-        raise
-
-    wifi.radio.connect(secrets["ssid"], secrets["password"])
+    wifi_ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+    wifi_password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+    wifi.radio.connect(wifi_ssid, wifi_password)
 
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     while True:
         print(ntp.datetime)
         time.sleep(1)
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/README.rst` & `adafruit_circuitpython_ntp-3.1.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -55,29 +55,25 @@
     pip3 install adafruit-circuitpython-ntp
 
 Usage Example
 =============
 
 .. code-block:: python
 
+    import adafruit_connection_manager
     import adafruit_ntp
-    import socketpool
+    import os
     import time
     import wifi
 
-    # Get wifi details and more from a secrets.py file
-    try:
-        from secrets import secrets
-    except ImportError:
-        print("WiFi secrets are kept in secrets.py, please add them there!")
-        raise
+    wifi_ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+    wifi_password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+    wifi.radio.connect(wifi_ssid, wifi_password)
 
-    wifi.radio.connect(secrets["ssid"], secrets["password"])
-
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     while True:
         print(ntp.datetime)
         time.sleep(1)
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/PKG-INFO` & `adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ntp
-Version: 3.0.9
+Version: 3.1.0
 Summary: Network Time Protocol (NTP) helper for Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NTP
 Keywords: adafruit,blinka,circuitpython,micropython,ntp,ntp,,network,,time
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
+Requires-Dist: Adafruit-Blinka
+Provides-Extra: optional
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ntp/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ntp/en/latest/
     :alt: Documentation Status
@@ -73,29 +74,25 @@
     pip3 install adafruit-circuitpython-ntp
 
 Usage Example
 =============
 
 .. code-block:: python
 
+    import adafruit_connection_manager
     import adafruit_ntp
-    import socketpool
+    import os
     import time
     import wifi
 
-    # Get wifi details and more from a secrets.py file
-    try:
-        from secrets import secrets
-    except ImportError:
-        print("WiFi secrets are kept in secrets.py, please add them there!")
-        raise
-
-    wifi.radio.connect(secrets["ssid"], secrets["password"])
+    wifi_ssid = os.getenv("CIRCUITPY_WIFI_SSID")
+    wifi_password = os.getenv("CIRCUITPY_WIFI_PASSWORD")
+    wifi.radio.connect(wifi_ssid, wifi_password)
 
-    pool = socketpool.SocketPool(wifi.radio)
+    pool = adafruit_connection_manager.get_radio_socketpool(wifi.radio)
     ntp = adafruit_ntp.NTP(pool, tz_offset=0)
 
     while True:
         print(ntp.datetime)
         time.sleep(1)
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/adafruit_circuitpython_ntp.egg-info/SOURCES.txt` & `adafruit_circuitpython_ntp-3.1.0/adafruit_circuitpython_ntp.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -29,10 +29,11 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/ntp_connection_manager.py
 examples/ntp_cpython.py
 examples/ntp_set_rtc.py
 examples/ntp_simpletest.py
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/adafruit_ntp.py` & `adafruit_circuitpython_ntp-3.1.0/adafruit_ntp.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,78 +18,89 @@
  * Adafruit CircuitPython firmware for the supported boards:
    https://github.com/adafruit/circuitpython/releases
 
 """
 import struct
 import time
 
-__version__ = "3.0.9"
+from micropython import const
+
+
+__version__ = "3.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NTP.git"
 
 NTP_TO_UNIX_EPOCH = 2208988800  # 1970-01-01 00:00:00
+PACKET_SIZE = const(48)
 
 
 class NTP:
     """Network Time Protocol (NTP) helper module for CircuitPython.
     This module does not handle daylight savings or local time. It simply requests
     UTC from a NTP server.
     """
 
     def __init__(
         self,
         socketpool,
         *,
         server: str = "0.adafruit.pool.ntp.org",
         port: int = 123,
-        tz_offset: int = 0,
+        tz_offset: float = 0,
         socket_timeout: int = 10,
     ) -> None:
         """
         :param object socketpool: A socket provider such as CPython's `socket` module.
         :param str server: The domain of the ntp server to query.
         :param int port: The port of the ntp server to query.
         :param float tz_offset: Timezone offset in hours from UTC. Only useful for timezone ignorant
             CircuitPython. CPython will determine timezone automatically and adjust (so don't use
             this.) For example, Pacific daylight savings time is -7.
         :param int socket_timeout: UDP socket timeout, in seconds.
         """
         self._pool = socketpool
         self._server = server
         self._port = port
-        self._packet = bytearray(48)
-        self._tz_offset = tz_offset * 60 * 60
+        self._socket_address = None
+        self._packet = bytearray(PACKET_SIZE)
+        self._tz_offset = int(tz_offset * 60 * 60)
         self._socket_timeout = socket_timeout
 
         # This is our estimated start time for the monotonic clock. We adjust it based on the ntp
         # responses.
         self._monotonic_start = 0
 
         self.next_sync = 0
 
     @property
     def datetime(self) -> time.struct_time:
         """Current time from NTP server. Accessing this property causes the NTP time request,
         unless there has already been a recent request. Raises OSError exception if no response
         is received within socket_timeout seconds"""
         if time.monotonic_ns() > self.next_sync:
+            if self._socket_address is None:
+                self._socket_address = self._pool.getaddrinfo(self._server, self._port)[
+                    0
+                ][4]
+
             self._packet[0] = 0b00100011  # Not leap second, NTP version 4, Client mode
-            for i in range(1, len(self._packet)):
+            for i in range(1, PACKET_SIZE):
                 self._packet[i] = 0
             with self._pool.socket(self._pool.AF_INET, self._pool.SOCK_DGRAM) as sock:
+                # Since the ESP32SPI doesn't support sendto, we are using
+                # connect + send to standardize code
                 sock.settimeout(self._socket_timeout)
-                sock.sendto(self._packet, (self._server, self._port))
-                sock.recvfrom_into(self._packet)
+                sock.connect(self._socket_address)
+                sock.send(self._packet)
+                sock.recv_into(self._packet)
                 # Get the time in the context to minimize the difference between it and receiving
                 # the packet.
                 destination = time.monotonic_ns()
             poll = struct.unpack_from("!B", self._packet, offset=2)[0]
             self.next_sync = destination + (2**poll) * 1_000_000_000
-            seconds = struct.unpack_from(
-                "!I", self._packet, offset=len(self._packet) - 8
-            )[0]
+            seconds = struct.unpack_from("!I", self._packet, offset=PACKET_SIZE - 8)[0]
             self._monotonic_start = (
                 seconds
                 + self._tz_offset
                 - NTP_TO_UNIX_EPOCH
                 - (destination // 1_000_000_000)
             )
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/docs/_static/favicon.ico` & `adafruit_circuitpython_ntp-3.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/docs/conf.py` & `adafruit_circuitpython_ntp-3.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -96,27 +96,18 @@
 napoleon_numpy_docstring = False
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-on_rtd = os.environ.get("READTHEDOCS", None) == "True"
+import sphinx_rtd_theme
 
-if not on_rtd:  # only import and set the theme if we're building docs locally
-    try:
-        import sphinx_rtd_theme
-
-        html_theme = "sphinx_rtd_theme"
-        html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
-    except:
-        html_theme = "default"
-        html_theme_path = ["."]
-else:
-    html_theme_path = ["."]
+html_theme = "sphinx_rtd_theme"
+html_theme_path = [sphinx_rtd_theme.get_html_theme_path(), "."]
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 # The name of an image file (relative to this directory) to use as a favicon of
```

### Comparing `adafruit-circuitpython-ntp-3.0.9/docs/examples.rst` & `adafruit_circuitpython_ntp-3.1.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/docs/index.rst` & `adafruit_circuitpython_ntp-3.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/examples/ntp_set_rtc.py` & `adafruit_circuitpython_ntp-3.1.0/examples/ntp_set_rtc.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/examples/ntp_simpletest.py` & `adafruit_circuitpython_ntp-3.1.0/examples/ntp_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ntp-3.0.9/pyproject.toml` & `adafruit_circuitpython_ntp-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ntp"
 description = "Network Time Protocol (NTP) helper for Python"
-version = "3.0.9"
+version = "3.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NTP"}
 keywords = [
     "adafruit",
```

