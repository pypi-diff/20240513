# Comparing `tmp/adafruit-circuitpython-is31fl3731-3.3.9.tar.gz` & `tmp/adafruit_circuitpython_is31fl3731-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-is31fl3731-3.3.9.tar", last modified: Fri May 26 16:17:09 2023, max compression
+gzip compressed data, was "adafruit_circuitpython_is31fl3731-3.4.0.tar", last modified: Mon May 13 17:00:18 2024, max compression
```

## Comparing `adafruit-circuitpython-is31fl3731-3.3.9.tar` & `adafruit_circuitpython_is31fl3731-3.4.0.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.997976 adafruit-circuitpython-is31fl3731-3.3.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.989976 adafruit-circuitpython-is31fl3731-3.3.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.989976 adafruit-circuitpython-is31fl3731-3.3.9/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-26 16:17:08.997976 adafruit-circuitpython-is31fl3731-3.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-26 16:17:08.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-26 16:17:08.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:17:08.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:17:08.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:17:08.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/
--rw-r--r--   0 runner    (1001) docker     (123)    12667 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/charlie_bonnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/charlie_wing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/keybow2040.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/led_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/matrix_11x7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/rgbmatrix5x5.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/scroll_phat_hd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.993976 adafruit-circuitpython-is31fl3731-3.3.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:08.997976 adafruit-circuitpython-is31fl3731-3.3.9/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_blink_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_frame_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_keybow_2040_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_ledshim_fade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_ledshim_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_animated_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_marquee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_numbers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_rgbmatrix5x5_rainbow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_text_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_wave_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 16:17:01.000000 adafruit-circuitpython-is31fl3731-3.3.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:16:53.000000 adafruit-circuitpython-is31fl3731-3.3.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:17:08.997976 adafruit-circuitpython-is31fl3731-3.3.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.150207 adafruit_circuitpython_is31fl3731-3.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.138207 adafruit_circuitpython_is31fl3731-3.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.138207 adafruit_circuitpython_is31fl3731-3.4.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.138207 adafruit_circuitpython_is31fl3731-3.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.142207 adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-13 17:00:18.146207 adafruit_circuitpython_is31fl3731-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.146207 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4870 2024-05-13 17:00:18.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-13 17:00:18.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:00:18.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 17:00:18.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 17:00:18.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.142207 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/
+-rw-r--r--   0 runner    (1001) docker     (127)    15602 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/charlie_bonnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/charlie_wing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/keybow2040.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/led_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/matrix_11x7.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/rgbmatrix5x5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/scroll_phat_hd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.146207 adafruit_circuitpython_is31fl3731-3.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.146207 adafruit_circuitpython_is31fl3731-3.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:00:18.146207 adafruit_circuitpython_is31fl3731-3.4.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_16x9_charlieplexed_pwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_blink_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_frame_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_keybow_2040_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_ledshim_fade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_ledshim_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_animated_gif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_marquee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_rgbmatrix5x5_rainbow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_text_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_wave_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-13 17:00:15.000000 adafruit_circuitpython_is31fl3731-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-13 17:00:06.000000 adafruit_circuitpython_is31fl3731-3.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:00:18.150207 adafruit_circuitpython_is31fl3731-3.4.0/setup.cfg
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_is31fl3731-3.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/.gitignore` & `adafruit_circuitpython_is31fl3731-3.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/.pre-commit-config.yaml` & `adafruit_circuitpython_is31fl3731-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/.pylintrc` & `adafruit_circuitpython_is31fl3731-3.4.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_is31fl3731-3.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/LICENSE` & `adafruit_circuitpython_is31fl3731-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/MIT.txt` & `adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/LICENSES/Unlicense.txt` & `adafruit_circuitpython_is31fl3731-3.4.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/PKG-INFO` & `adafruit_circuitpython_is31fl3731-3.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3731
-Version: 3.3.9
+Version: 3.4.0
 Summary: CircuitPython library for IS31FL3731 charlieplex LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731
 Keywords: adafruit,is31fl3731,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
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
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
+Requires-Dist: adafruit-circuitpython-framebuf; extra == "optional"
+Requires-Dist: pillow; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-is31fl3731/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/is31fl3731/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/README.rst` & `adafruit_circuitpython_is31fl3731-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-is31fl3731
-Version: 3.3.9
+Version: 3.4.0
 Summary: CircuitPython library for IS31FL3731 charlieplex LED matrices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731
 Keywords: adafruit,is31fl3731,led,matrix,charlieplex,featherwingbreakout,hardware,micropython,circuitpython
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
+Requires-Dist: adafruit-circuitpython-busdevice
+Provides-Extra: optional
+Requires-Dist: adafruit-circuitpython-framebuf; extra == "optional"
+Requires-Dist: pillow; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-is31fl3731/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/is31fl3731/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_circuitpython_is31fl3731.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/is31fl3731_16x9_charlieplexed_pwm.py
 examples/is31fl3731_blink_example.py
 examples/is31fl3731_frame_example.py
 examples/is31fl3731_keybow_2040_rainbow.py
 examples/is31fl3731_ledshim_fade.py
 examples/is31fl3731_ledshim_rainbow.py
 examples/is31fl3731_pillow_animated_gif.py
 examples/is31fl3731_pillow_marquee.py
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/__init__.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -43,23 +43,45 @@
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
-
 # imports
 import math
 import time
 from micropython import const
 
 from adafruit_bus_device.i2c_device import I2CDevice
 
-__version__ = "3.3.9"
+try:
+    import typing
+    import busio
+    from circuitpython_typing import TypeAlias, Union
+    from circuitpython_typing import (
+        WriteableBuffer,
+        ReadableBuffer,
+    )  # Import ReadableBuffer here
+
+    from typing import (
+        TYPE_CHECKING,
+        List,
+        Tuple,
+        Optional,
+        Iterable,
+    )
+
+    from PIL import Image
+
+except ImportError as e:
+    pass
+
+
+__version__ = "3.4.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731.git"
 
 _MODE_REGISTER = const(0x00)
 _FRAME_REGISTER = const(0x01)
 _AUTOPLAY1_REGISTER = const(0x02)
 _AUTOPLAY2_REGISTER = const(0x03)
 _BLINK_REGISTER = const(0x05)
@@ -85,63 +107,79 @@
 class IS31FL3731:
     """
     The IS31FL3731 is an abstract class contain the main function related to this chip.
     Each board needs to define width, height and pixel_addr.
 
     :param ~busio.I2C i2c: the connected i2c bus i2c_device
     :param int address: the device address; defaults to 0x74
+    :param Iterable frames: list of frame indexes to use. int's 0-7.
     """
 
-    width = 16
-    height = 9
+    width: int = 16
+    height: int = 9
 
-    def __init__(self, i2c, address=0x74, frames=None):
+    def __init__(
+        self,
+        i2c: busio.I2C,
+        frames: Optional[Iterable] = None,
+        address: int = 0x74,
+    ):
         self.i2c_device = I2CDevice(i2c, address)
         self._frame = None
         self._init(frames=frames)
 
-    def _i2c_read_reg(self, reg, result):
+    def _i2c_read_reg(
+        self, reg: Optional[int] = None, result: Optional[WriteableBuffer] = None
+    ) -> Optional[WriteableBuffer]:
         # Read a buffer of data from the specified 8-bit I2C register address.
         # The provided result parameter will be filled to capacity with bytes
         # of data read from the register.
         with self.i2c_device as i2c:
             i2c.write_then_readinto(bytes([reg]), result)
             return result
         return None
 
-    def _i2c_write_reg(self, reg, data):
+    def _i2c_write_reg(
+        self, reg: Optional[int] = None, data: Optional[ReadableBuffer] = None
+    ) -> None:
         # Write a contiguous block of data (bytearray) starting at the
         # specified I2C register address (register passed as argument).
         self._i2c_write_block(bytes([reg]) + data)
 
-    def _i2c_write_block(self, data):
+    def _i2c_write_block(self, data: Optional[ReadableBuffer]) -> None:
         # Write a buffer of data (byte array) to the specified I2C register
         # address.
         with self.i2c_device as i2c:
             i2c.write(data)
 
-    def _bank(self, bank=None):
+    def _bank(self, bank: Optional[int] = None) -> Optional[int]:
         if bank is None:
             result = bytearray(1)
             return self._i2c_read_reg(_BANK_ADDRESS, result)[0]
         self._i2c_write_reg(_BANK_ADDRESS, bytearray([bank]))
         return None
 
-    def _register(self, bank, register, value=None):
+    def _register(
+        self,
+        bank: Optional[int] = None,
+        register: Optional[int] = None,
+        value: Optional[int] = None,
+    ) -> Optional[int]:
         self._bank(bank)
         if value is None:
             result = bytearray(1)
             return self._i2c_read_reg(register, result)[0]
         self._i2c_write_reg(register, bytearray([value]))
         return None
 
-    def _mode(self, mode=None):
+    def _mode(self, mode: Optional[int] = None) -> int:
+        """Function for setting _register mode"""
         return self._register(_CONFIG_BANK, _MODE_REGISTER, mode)
 
-    def _init(self, frames=None):
+    def _init(self, frames: Iterable) -> None:
         self.sleep(True)
         # Clear config; sets to Picture Mode, no audio sync, maintains sleep
         self._bank(_CONFIG_BANK)
         self._i2c_write_block(bytes([0] * 14))
         enable_data = bytes([_ENABLE_OFFSET] + [255] * 18)
         fill_data = bytearray([0] * 25)
         # Initialize requested frames, or all 8 if unspecified
@@ -150,29 +188,34 @@
             self._i2c_write_block(enable_data)  # Set all enable bits
             for row in range(6):  # Barebones quick fill() w/0
                 fill_data[0] = _COLOR_OFFSET + row * 24
                 self._i2c_write_block(fill_data)
         self._frame = 0  # To match config bytes above
         self.sleep(False)
 
-    def reset(self):
+    def reset(self) -> None:
         """Kill the display for 10MS"""
         self.sleep(True)
         time.sleep(0.01)  # 10 MS pause to reset.
         self.sleep(False)
 
-    def sleep(self, value):
+    def sleep(self, value: bool) -> Optional[int]:
         """
         Set the Software Shutdown Register bit
 
         :param value: True to set software shutdown bit; False unset
         """
         return self._register(_CONFIG_BANK, _SHUTDOWN_REGISTER, not value)
 
-    def autoplay(self, delay=0, loops=0, frames=0):
+    def autoplay(
+        self,
+        delay: int = 0,
+        loops: int = 0,
+        frames: int = 0,
+    ) -> None:
         """
         Start autoplay
 
         :param delay: in ms
         :param loops: number of loops - 0->7
         :param frames: number of frames: 0->7
         """
@@ -186,23 +229,28 @@
             raise ValueError("Frames out of range")
         if not 1 <= delay <= 64:
             raise ValueError("Delay out of range")
         self._register(_CONFIG_BANK, _AUTOPLAY1_REGISTER, loops << 4 | frames)
         self._register(_CONFIG_BANK, _AUTOPLAY2_REGISTER, delay % 64)
         self._mode(_AUTOPLAY_MODE | self._frame)
 
-    def fade(self, fade_in=None, fade_out=None, pause=0):
+    def fade(
+        self,
+        fade_in: Optional[int] = None,
+        fade_out: Optional[int] = None,
+        pause: int = 0,
+    ) -> int:
         """
         Start and stop the fade feature.  If both fade_in and fade_out are None (the
         default), the breath feature is used for fading.  if fade_in is None, then
         fade_in = fade_out.  If fade_out is None, then fade_out = fade_in
 
-        :param fade_in: positive number; 0->100
-        :param fade-out: positive number; 0->100
-        :param pause: breath register 2 pause value
+        :param fade_in: int positive number; 0->100
+        :param fade-out: int positive number; 0->100
+        :param pause: int breath register 2 pause value
         """
         if fade_in is None and fade_out is None:
             self._register(_CONFIG_BANK, _BREATH2_REGISTER, 0)
             return
         if fade_in is None:
             fade_in = fade_out
         elif fade_out is None:
@@ -219,35 +267,41 @@
         if not 0 <= fade_out <= 7:
             raise ValueError("Fade out out of range")
         if not 0 <= pause <= 7:
             raise ValueError("Pause out of range")
         self._register(_CONFIG_BANK, _BREATH1_REGISTER, fade_out << 4 | fade_in)
         self._register(_CONFIG_BANK, _BREATH2_REGISTER, 1 << 4 | pause)
 
-    def frame(self, frame=None, show=True):
+    def frame(self, frame: Optional[int] = None, show: bool = True) -> Optional[int]:
         """
         Set the current frame
 
-        :param frame: frame number; 0-7 or None. If None function returns current frame
-        :param show: True to show the frame; False to not show.
+        :param frame: int frame number; 0-7 or None. If None function returns current frame
+        :param show: bool True to show the frame; False to not show.
         """
         if frame is None:
             return self._frame
         if not 0 <= frame <= 8:
             raise ValueError("Frame out of range")
         self._frame = frame
         if show:
             self._register(_CONFIG_BANK, _FRAME_REGISTER, frame)
         return None
 
-    def audio_sync(self, value=None):
+    def audio_sync(self, value: Optional[int]) -> Optional[int]:
         """Set the audio sync feature register"""
         return self._register(_CONFIG_BANK, _AUDIOSYNC_REGISTER, value)
 
-    def audio_play(self, sample_rate, audio_gain=0, agc_enable=False, agc_fast=False):
+    def audio_play(
+        self,
+        sample_rate: int,
+        audio_gain: int = 0,
+        agc_enable: bool = False,
+        agc_fast: bool = False,
+    ) -> None:
         """Controls the audio play feature"""
         if sample_rate == 0:
             self._mode(_PICTURE_MODE)
             return
         sample_rate //= 46
         if not 1 <= sample_rate <= 256:
             raise ValueError("Sample rate out of range")
@@ -258,34 +312,39 @@
         self._register(
             _CONFIG_BANK,
             _GAIN_REGISTER,
             bool(agc_enable) << 3 | bool(agc_fast) << 4 | audio_gain,
         )
         self._mode(_AUDIOPLAY_MODE)
 
-    def blink(self, rate=None):
+    def blink(self, rate: Optional[int] = None) -> Optional[int]:
         """Updates the blink register"""
         # pylint: disable=no-else-return
         # This needs to be refactored when it can be tested
         if rate is None:
             return (self._register(_CONFIG_BANK, _BLINK_REGISTER) & 0x07) * 270
         elif rate == 0:
             self._register(_CONFIG_BANK, _BLINK_REGISTER, 0x00)
             return None
         rate //= 270
         self._register(_CONFIG_BANK, _BLINK_REGISTER, rate & 0x07 | 0x08)
         return None
 
-    def fill(self, color=None, blink=None, frame=None):
+    def fill(
+        self,
+        color: Optional[int] = None,
+        frame: Optional[int] = None,
+        blink: bool = False,
+    ):
         """
         Fill the display with a brightness level
 
         :param color: brightness 0->255
-        :param blink: True if blinking is required
-        :param frame: which frame to fill 0->7
+        :param blink: bool True to blink
+        :param frame: int the frame to set the pixel, default 0
         """
         if frame is None:
             frame = self._frame
         self._bank(frame)
         if color is not None:
             if not 0 <= color <= 255:
                 raise ValueError("Color out of range")
@@ -297,61 +356,100 @@
         if blink is not None:
             data = bool(blink) * 0xFF
             for col in range(18):
                 self._register(frame, _BLINK_OFFSET + col, data)
 
     # This function must be replaced for each board
     @staticmethod
-    def pixel_addr(x, y):
+    def pixel_addr(x: int, y: int) -> int:
         """Calulate the offset into the device array for x,y pixel"""
         return x + y * 16
 
     # pylint: disable-msg=too-many-arguments
-    def pixel(self, x, y, color=None, blink=None, frame=None):
-        """
-        Blink or brightness for x-, y-pixel
+    def pixel(
+        self,
+        x: int,
+        y: int,
+        color: Optional[int] = None,
+        frame: Optional[int] = None,
+        blink: bool = False,
+        rotate: int = 0,
+    ) -> Optional[int]:
+        """
+        Matrix display configuration
+
+        :param x: int horizontal pixel position
+        :param y: int vertical pixel position
+        :param color: int brightness value 0->255
+        :param blink: bool True to blink
+        :param frame: int the frame to set the pixel, default 0
+        :param rotate: int display rotation (0, 90, 180, 270)
+        """
+        # pylint: disable=too-many-branches
+
+        if rotate not in (0, 90, 180, 270):
+            raise ValueError("Rotation must be 0, 90, 180, or 270 degrees")
+
+        if rotate == 0:
+            check_x = 0 <= x <= self.width
+            check_y = 0 <= y <= self.height
+            if not (check_x and check_y):
+                return None
+            pixel = self.pixel_addr(x, y)
+        elif rotate == 90:
+            check_x = 0 <= y <= self.width
+            check_y = 0 <= x <= self.height
+            if not (check_x and check_y):
+                return None
+            pixel = self.pixel_addr(y, self.height - x - 1)
+        elif rotate == 180:
+            check_x = 0 <= x <= self.width
+            check_y = 0 <= y <= self.height
+            if not (check_x and check_y):
+                return None
+            pixel = self.pixel_addr(self.width - x - 1, self.height - y - 1)
+        elif rotate == 270:
+            check_x = 0 <= y <= self.width
+            check_y = 0 <= x <= self.height
+            if not (check_x and check_y):
+                return None
+            pixel = self.pixel_addr(self.width - y - 1, x)
 
-        :param x: horizontal pixel position
-        :param y: vertical pixel position
-        :param color: brightness value 0->255
-        :param blink: True to blink
-        :param frame: the frame to set the pixel
-        """
-        if not 0 <= x <= self.width:
-            return None
-        if not 0 <= y <= self.height:
-            return None
-        pixel = self.pixel_addr(x, y)
         if color is None and blink is None:
             return self._register(self._frame, pixel)
+        # frames other than 0 only used in animation. allow None.
         if frame is None:
             frame = self._frame
+        # Brightness
         if color is not None:
             if not 0 <= color <= 255:
-                raise ValueError("Color out of range")
+                raise ValueError("Brightness or Color out of range (0-255)")
             self._register(frame, _COLOR_OFFSET + pixel, color)
-        if blink is not None:
+        # Blink works but not well while animated
+        if blink:
             addr, bit = divmod(pixel, 8)
             bits = self._register(frame, _BLINK_OFFSET + addr)
             if blink:
                 bits |= 1 << bit
             else:
                 bits &= ~(1 << bit)
             self._register(frame, _BLINK_OFFSET + addr, bits)
         return None
 
     # pylint: enable-msg=too-many-arguments
 
-    def image(self, img, blink=None, frame=None):
+    def image(
+        self, img: Image, frame: Optional[int] = None, blink: bool = False
+    ) -> None:
         """Set buffer to value of Python Imaging Library image.  The image should
         be in 8-bit mode (L) and a size equal to the display size.
 
         :param img: Python Imaging Library image
         :param blink: True to blink
-        :param frame: the frame to set the image
+        :param frame: the frame to set the image, default 0
         """
         if img.mode != "L":
             raise ValueError("Image must be in mode L.")
         imwidth, imheight = img.size
         if imwidth != self.width or imheight != self.height:
             raise ValueError(
                 "Image must be same dimensions as display ({0}x{1}).".format(
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/charlie_bonnet.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/charlie_bonnet.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/charlie_wing.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/charlie_wing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/keybow2040.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/keybow2040.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/led_shim.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/led_shim.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/matrix.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/matrix.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,55 +25,64 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 from . import IS31FL3731
 
+try:
+    from typing import Optional
+
+    try:
+        from PIL import Image
+    except ImportError:
+        # placeholder if PIL unavailable
+        Image = None
+except ImportError as e:
+    pass
+
 
 class Matrix(IS31FL3731):
-    """Supports the Charlieplexed feather wing"""
+    """Charlieplexed Featherwing & IS31FL3731 I2C Modules"""
 
-    width = 16
-    height = 9
+    width: int = 16
+    height: int = 9
 
     @staticmethod
-    def pixel_addr(x, y):
+    def pixel_addr(x: int, y: int) -> int:
         """Calulate the offset into the device array for x,y pixel"""
         return x + y * 16
 
     # This takes precedence over image() in __init__ and is tuned for the
     # Matrix class. Some shortcuts can be taken because matrix layout is
     # very straightforward, and a few large write operations are used
     # rather than pixel-by-pixel writes, yielding significant speed gains
     # for animation. Buffering the full matrix for a quick write is not a
     # memory concern here, as by definition this method is used with PIL
     # images; we're not running on a RAM-constrained microcontroller.
-    def image(self, img, blink=None, frame=None):
+    def image(self, img: Image, frame: Optional[int] = None, blink: bool = False):
         """Set buffer to value of Python Imaging Library image.
         The image should be in 8-bit mode (L) and a size equal to the
         display size.
 
         :param img: Python Imaging Library image
         :param blink: True to blink
         :param frame: the frame to set the image
         """
         if img.mode != "L":
             raise ValueError("Image must be in mode L.")
         if img.size[0] != self.width or img.size[1] != self.height:
             raise ValueError(
-                "Image must be same dimensions as display ({0}x{1}).".format(
-                    self.width, self.height
-                )
+                f"Image must be same dimensions as display {self.width}x{self.height}"
             )
 
         # Frame-select and then write pixel data in one big operation
         if frame is not None:
             self._bank(frame)
         # We can safely reduce the image to a "flat" byte sequence because
         # the matrix layout is known linear; no need to go through a 2D
         # pixel array or invoke pixel_addr().
         self._i2c_write_block(bytes([0x24]) + img.tobytes())
         # Set or clear blink state if requested, for all pixels at once
-        if blink is not None:
+        if blink:
             # 0x12 is _BLINK_OFFSET in __init__.py
             self._i2c_write_block(bytes([0x12] + [1 if blink else 0] * 18))
```

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/matrix_11x7.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/matrix_11x7.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/rgbmatrix5x5.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/rgbmatrix5x5.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/adafruit_is31fl3731/scroll_phat_hd.py` & `adafruit_circuitpython_is31fl3731-3.4.0/adafruit_is31fl3731/scroll_phat_hd.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/docs/_static/favicon.ico` & `adafruit_circuitpython_is31fl3731-3.4.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/docs/api.rst` & `adafruit_circuitpython_is31fl3731-3.4.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/docs/conf.py` & `adafruit_circuitpython_is31fl3731-3.4.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,27 +97,18 @@
 
 
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

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/docs/examples.rst` & `adafruit_circuitpython_is31fl3731-3.4.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/docs/index.rst` & `adafruit_circuitpython_is31fl3731-3.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_blink_example.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_blink_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_frame_example.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_frame_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_keybow_2040_rainbow.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_keybow_2040_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_ledshim_rainbow.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_ledshim_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_animated_gif.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_animated_gif.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_marquee.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_marquee.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_pillow_numbers.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_pillow_numbers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_rgbmatrix5x5_rainbow.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_rgbmatrix5x5_rainbow.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_simpletest.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_text_example.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_text_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/examples/is31fl3731_wave_example.py` & `adafruit_circuitpython_is31fl3731-3.4.0/examples/is31fl3731_wave_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-is31fl3731-3.3.9/pyproject.toml` & `adafruit_circuitpython_is31fl3731-3.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-is31fl3731"
 description = "CircuitPython library for IS31FL3731 charlieplex LED matrices."
-version = "3.3.9"
+version = "3.4.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IS31FL3731"}
 keywords = [
     "adafruit",
```

