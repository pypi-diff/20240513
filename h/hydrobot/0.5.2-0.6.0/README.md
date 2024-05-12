# Comparing `tmp/hydrobot-0.5.2.tar.gz` & `tmp/hydrobot-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydrobot-0.5.2.tar", last modified: Wed Apr 10 21:28:36 2024, max compression
+gzip compressed data, was "hydrobot-0.6.0.tar", last modified: Sun May 12 23:08:50 2024, max compression
```

## Comparing `hydrobot-0.5.2.tar` & `hydrobot-0.6.0.tar`

### file list

```diff
@@ -1,98 +1,105 @@
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/
--rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.5.2/.editorconfig
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/.github/
--rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.5.2/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.5.2/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-04-03 19:58:45.000000 hydrobot-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.5.2/.readthedocs.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.5.2/AUTHORS.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     7309 2024-04-10 20:37:44.000000 hydrobot-0.5.2/CONTRIBUTING.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1699 2024-04-10 20:44:58.000000 hydrobot-0.5.2/HISTORY.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.5.2/LICENSE
--rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.5.2/MANIFEST.in
--rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.5.2/Makefile
--rw-r--r--   0 nic       (1000) nic       (1000)     7028 2024-04-10 21:28:36.461589 hydrobot-0.5.2/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     5295 2024-04-10 21:26:54.000000 hydrobot-0.5.2/README.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/docs/
--rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.5.2/docs/Makefile
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.441589 hydrobot-0.5.2/docs/_build/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.441589 hydrobot-0.5.2/docs/_build/html/
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/docs/_build/html/_static/
--rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.5.2/docs/_build/html/_static/file.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.2/docs/_build/html/_static/minus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.5.2/docs/_build/html/_static/plus.png
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.2/docs/authors.rst
--rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-04-10 20:44:58.000000 hydrobot-0.5.2/docs/conf.py
--rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.5.2/docs/contributing.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.5.2/docs/history.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.5.2/docs/hydrobot.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.5.2/docs/index.rst
--rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.5.2/docs/installation.rst
--rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.5.2/docs/make.bat
--rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.5.2/docs/modules.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.5.2/docs/readme.rst
--rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.5.2/docs/usage.rst
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/hydrobot/
--rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-04-10 21:26:54.000000 hydrobot-0.5.2/hydrobot/__init__.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/hydrobot/config/
--rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.5.2/hydrobot/config/QualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.5.2/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
--rw-r--r--   0 nic       (1000) nic       (1000)     6472 2024-04-10 20:44:58.000000 hydrobot-0.5.2/hydrobot/data_acquisition.py
--rw-r--r--   0 nic       (1000) nic       (1000)     8005 2024-04-03 19:54:56.000000 hydrobot-0.5.2/hydrobot/data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)    32675 2024-04-03 02:25:29.000000 hydrobot-0.5.2/hydrobot/data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    15368 2024-04-10 20:48:54.000000 hydrobot-0.5.2/hydrobot/evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     7516 2024-03-11 01:19:58.000000 hydrobot-0.5.2/hydrobot/filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    20256 2024-04-10 20:44:58.000000 hydrobot-0.5.2/hydrobot/plotter.py
--rw-r--r--   0 nic       (1000) nic       (1000)    52155 2024-04-10 20:37:44.000000 hydrobot-0.5.2/hydrobot/processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     7778 2024-04-03 02:25:29.000000 hydrobot-0.5.2/hydrobot/utils.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/hydrobot.egg-info/
--rw-r--r--   0 nic       (1000) nic       (1000)     7028 2024-04-10 21:28:36.000000 hydrobot-0.5.2/hydrobot.egg-info/PKG-INFO
--rw-r--r--   0 nic       (1000) nic       (1000)     2123 2024-04-10 21:28:36.000000 hydrobot-0.5.2/hydrobot.egg-info/SOURCES.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-04-10 21:28:36.000000 hydrobot-0.5.2/hydrobot.egg-info/dependency_links.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      311 2024-04-10 21:28:36.000000 hydrobot-0.5.2/hydrobot.egg-info/requires.txt
--rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-04-10 21:28:36.000000 hydrobot-0.5.2/hydrobot.egg-info/top_level.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.5.2/old_setup.cfg
--rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.5.2/old_setup.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.451589 hydrobot-0.5.2/prototypes/
--rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-08 04:10:48.000000 hydrobot-0.5.2/prototypes/Class_script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/prototypes/example_script/
--rw-r--r--   0 nic       (1000) nic       (1000)     9920 2024-04-10 20:37:44.000000 hydrobot-0.5.2/prototypes/example_script/WaterTemp_CheckData.R
--rw-r--r--   0 nic       (1000) nic       (1000)     1099 2024-04-10 20:50:08.000000 hydrobot-0.5.2/prototypes/example_script/config.yaml
--rw-r--r--   0 nic       (1000) nic       (1000)     5680 2024-04-10 21:15:13.000000 hydrobot-0.5.2/prototypes/example_script/script.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/prototypes/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.2/prototypes/output_dump/.gitignore
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/prototypes/py_scripts/
--rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/atmospheric_spike_removal.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/example_plot_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-03 02:25:29.000000 hydrobot-0.5.2/prototypes/py_scripts/gap_finder.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/new_ws_plot_with_check_data.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/prototypes/py_scripts/output_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.5.2/prototypes/py_scripts/output_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/plot_with_check_data.py
--rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/process_script.py
--rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.5.2/prototypes/py_scripts/spike_removal_util.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/stage_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/py_scripts/water_temp_full_process.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.5.2/prototypes/py_scripts/water_temp_spike_removal.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/prototypes/script_dump/
--rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/script_dump/.gitignore
--rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/site_list_reader.py
--rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.5.2/prototypes/site_parameters.json
--rw-r--r--   0 nic       (1000) nic       (1000)     3195 2024-04-10 21:26:54.000000 hydrobot-0.5.2/pyproject.toml
--rw-r--r--   0 nic       (1000) nic       (1000)     2419 2024-04-03 02:25:29.000000 hydrobot-0.5.2/requirements_dev.txt
--rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.5.2/requirements_test.txt
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-04-10 21:28:36.461589 hydrobot-0.5.2/setup.cfg
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/tests/
--rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.5.2/tests/.coverage
--rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.5.2/tests/__init__.py
--rw-r--r--   0 nic       (1000) nic       (1000)     1017 2024-04-10 21:24:02.000000 hydrobot-0.5.2/tests/conftest.py
-drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-04-10 21:28:36.461589 hydrobot-0.5.2/tests/test_data/
--rw-r--r--   0 nic       (1000) nic       (1000)      245 2024-04-10 20:44:58.000000 hydrobot-0.5.2/tests/test_data/site_list_response.xml
--rw-r--r--   0 nic       (1000) nic       (1000)    13995 2024-04-10 20:44:58.000000 hydrobot-0.5.2/tests/test_data/xml_test_data_file.xml
--rw-r--r--   0 nic       (1000) nic       (1000)     2929 2024-03-11 01:19:58.000000 hydrobot-0.5.2/tests/test_data_sources.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9730 2024-04-07 23:09:32.000000 hydrobot-0.5.2/tests/test_data_structure.py
--rw-r--r--   0 nic       (1000) nic       (1000)    13746 2024-04-10 20:48:54.000000 hydrobot-0.5.2/tests/test_evaluator.py
--rw-r--r--   0 nic       (1000) nic       (1000)     9481 2024-03-11 01:19:58.000000 hydrobot-0.5.2/tests/test_filters.py
--rw-r--r--   0 nic       (1000) nic       (1000)    25001 2024-04-10 20:44:58.000000 hydrobot-0.5.2/tests/test_processor.py
--rw-r--r--   0 nic       (1000) nic       (1000)     2557 2024-04-07 23:15:31.000000 hydrobot-0.5.2/tests/test_utils.py
--rw-r--r--   0 nic       (1000) nic       (1000)    24135 2024-04-07 23:21:22.000000 hydrobot-0.5.2/tests/test_web_integration.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.092015 hydrobot-0.6.0/
+-rw-r--r--   0 nic       (1000) nic       (1000)      292 2023-09-27 02:03:08.000000 hydrobot-0.6.0/.editorconfig
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:49.972016 hydrobot-0.6.0/.github/
+-rw-r--r--   0 nic       (1000) nic       (1000)      333 2023-09-27 02:03:08.000000 hydrobot-0.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 nic       (1000) nic       (1000)     1207 2023-10-16 02:52:42.000000 hydrobot-0.6.0/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)      514 2024-04-03 19:58:45.000000 hydrobot-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     1068 2024-03-11 01:19:58.000000 hydrobot-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)      212 2023-10-16 02:52:42.000000 hydrobot-0.6.0/AUTHORS.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     7309 2024-04-10 20:37:44.000000 hydrobot-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     2257 2024-05-12 22:58:08.000000 hydrobot-0.6.0/HISTORY.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1610 2023-10-16 02:47:23.000000 hydrobot-0.6.0/LICENSE
+-rw-r--r--   0 nic       (1000) nic       (1000)      298 2024-03-11 01:19:58.000000 hydrobot-0.6.0/MANIFEST.in
+-rw-r--r--   0 nic       (1000) nic       (1000)     2336 2024-03-11 01:19:58.000000 hydrobot-0.6.0/Makefile
+-rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-12 23:08:50.092015 hydrobot-0.6.0/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     5295 2024-05-12 23:02:36.000000 hydrobot-0.6.0/README.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:49.972016 hydrobot-0.6.0/docs/
+-rw-r--r--   0 nic       (1000) nic       (1000)      609 2023-11-02 03:51:37.000000 hydrobot-0.6.0/docs/Makefile
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:49.962016 hydrobot-0.6.0/docs/_build/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:49.962016 hydrobot-0.6.0/docs/_build/html/
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.002015 hydrobot-0.6.0/docs/_build/html/_static/
+-rw-r--r--   0 nic       (1000) nic       (1000)      286 2023-12-12 21:10:33.000000 hydrobot-0.6.0/docs/_build/html/_static/file.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.0/docs/_build/html/_static/minus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       90 2023-12-12 21:10:33.000000 hydrobot-0.6.0/docs/_build/html/_static/plus.png
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.0/docs/authors.rst
+-rwxr-xr-x   0 nic       (1000) nic       (1000)     5087 2024-04-10 21:52:59.000000 hydrobot-0.6.0/docs/conf.py
+-rw-r--r--   0 nic       (1000) nic       (1000)       33 2023-09-27 02:03:08.000000 hydrobot-0.6.0/docs/contributing.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       28 2023-09-27 02:03:08.000000 hydrobot-0.6.0/docs/history.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1190 2024-03-11 01:19:58.000000 hydrobot-0.6.0/docs/hydrobot.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      305 2023-11-02 03:51:37.000000 hydrobot-0.6.0/docs/index.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)     1555 2024-03-11 01:19:58.000000 hydrobot-0.6.0/docs/installation.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)      806 2023-11-02 03:51:37.000000 hydrobot-0.6.0/docs/make.bat
+-rw-r--r--   0 nic       (1000) nic       (1000)       61 2023-12-12 21:10:41.000000 hydrobot-0.6.0/docs/modules.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       27 2023-09-27 02:03:08.000000 hydrobot-0.6.0/docs/readme.rst
+-rw-r--r--   0 nic       (1000) nic       (1000)       71 2023-11-02 03:51:37.000000 hydrobot-0.6.0/docs/usage.rst
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.002015 hydrobot-0.6.0/hydrobot/
+-rw-r--r--   0 nic       (1000) nic       (1000)      153 2024-05-12 23:02:36.000000 hydrobot-0.6.0/hydrobot/__init__.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.012015 hydrobot-0.6.0/hydrobot/config/
+-rw-r--r--   0 nic       (1000) nic       (1000)      105 2024-03-11 01:19:58.000000 hydrobot-0.6.0/hydrobot/config/QualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)       55 2024-03-11 01:19:58.000000 hydrobot-0.6.0/hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
+-rw-r--r--   0 nic       (1000) nic       (1000)     7562 2024-05-09 04:26:05.000000 hydrobot-0.6.0/hydrobot/data_acquisition.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     8472 2024-05-10 02:48:43.000000 hydrobot-0.6.0/hydrobot/data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    31704 2024-05-10 02:39:03.000000 hydrobot-0.6.0/hydrobot/data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    19638 2024-05-09 04:54:35.000000 hydrobot-0.6.0/hydrobot/evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     8425 2024-05-09 22:46:55.000000 hydrobot-0.6.0/hydrobot/filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    19993 2024-05-10 02:48:43.000000 hydrobot-0.6.0/hydrobot/plotter.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    62690 2024-05-10 02:48:43.000000 hydrobot-0.6.0/hydrobot/processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     7778 2024-04-03 02:25:29.000000 hydrobot-0.6.0/hydrobot/utils.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.082015 hydrobot-0.6.0/hydrobot.egg-info/
+-rw-r--r--   0 nic       (1000) nic       (1000)     7090 2024-05-12 23:08:49.000000 hydrobot-0.6.0/hydrobot.egg-info/PKG-INFO
+-rw-r--r--   0 nic       (1000) nic       (1000)     2439 2024-05-12 23:08:49.000000 hydrobot-0.6.0/hydrobot.egg-info/SOURCES.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        1 2024-05-12 23:08:49.000000 hydrobot-0.6.0/hydrobot.egg-info/dependency_links.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      343 2024-05-12 23:08:49.000000 hydrobot-0.6.0/hydrobot.egg-info/requires.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)        9 2024-05-12 23:08:49.000000 hydrobot-0.6.0/hydrobot.egg-info/top_level.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      422 2024-03-11 01:19:58.000000 hydrobot-0.6.0/old_setup.cfg
+-rw-r--r--   0 nic       (1000) nic       (1000)     1571 2024-03-11 01:19:58.000000 hydrobot-0.6.0/old_setup.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.012015 hydrobot-0.6.0/prototypes/
+-rw-r--r--   0 nic       (1000) nic       (1000)     4257 2024-04-08 04:10:48.000000 hydrobot-0.6.0/prototypes/Class_script.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.062015 hydrobot-0.6.0/prototypes/example_script/
+-rw-r--r--   0 nic       (1000) nic       (1000)       22 2024-05-06 01:52:39.000000 hydrobot-0.6.0/prototypes/example_script/.gitignore
+-rwxr-xr-x   0 nic       (1000) nic       (1000)   450560 2024-05-03 01:38:55.000000 hydrobot-0.6.0/prototypes/example_script/40X_XXX_WaterTemperature.accdb
+-rwxr-xr-x   0 nic       (1000) nic       (1000)   214752 2024-05-03 01:38:55.000000 hydrobot-0.6.0/prototypes/example_script/40X_XXX_WaterTemperature.hts
+-rw-r--r--   0 nic       (1000) nic       (1000)     9598 2024-05-09 22:47:37.000000 hydrobot-0.6.0/prototypes/example_script/AP_CheckData.R
+-rw-r--r--   0 nic       (1000) nic       (1000)      832 2024-05-08 23:03:49.000000 hydrobot-0.6.0/prototypes/example_script/AP_config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)    10505 2024-05-09 04:54:35.000000 hydrobot-0.6.0/prototypes/example_script/WaterTemp_CheckData.R
+-rw-r--r--   0 nic       (1000) nic       (1000)     1392 2024-05-12 23:02:36.000000 hydrobot-0.6.0/prototypes/example_script/config.yaml
+-rw-r--r--   0 nic       (1000) nic       (1000)     4796 2024-05-12 23:02:36.000000 hydrobot-0.6.0/prototypes/example_script/script.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.062015 hydrobot-0.6.0/prototypes/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.0/prototypes/output_dump/.gitignore
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.062015 hydrobot-0.6.0/prototypes/py_scripts/
+-rw-r--r--   0 nic       (1000) nic       (1000)     1515 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/atmospheric_spike_removal.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1051 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/example_plot_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1581 2024-04-03 02:25:29.000000 hydrobot-0.6.0/prototypes/py_scripts/gap_finder.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1319 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/new_ws_plot_with_check_data.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.062015 hydrobot-0.6.0/prototypes/py_scripts/output_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2023-11-02 01:24:43.000000 hydrobot-0.6.0/prototypes/py_scripts/output_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1001 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/plot_with_check_data.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     4222 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/process_script.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      933 2023-12-03 22:14:39.000000 hydrobot-0.6.0/prototypes/py_scripts/spike_removal_util.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3509 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/stage_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     3627 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/py_scripts/water_temp_full_process.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1927 2023-11-02 02:57:00.000000 hydrobot-0.6.0/prototypes/py_scripts/water_temp_spike_removal.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.062015 hydrobot-0.6.0/prototypes/script_dump/
+-rw-r--r--   0 nic       (1000) nic       (1000)      144 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/script_dump/.gitignore
+-rw-r--r--   0 nic       (1000) nic       (1000)     1419 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/site_list_reader.py
+-rw-r--r--   0 nic       (1000) nic       (1000)      443 2024-03-11 01:19:58.000000 hydrobot-0.6.0/prototypes/site_parameters.json
+-rw-r--r--   0 nic       (1000) nic       (1000)     3507 2024-05-12 23:07:12.000000 hydrobot-0.6.0/pyproject.toml
+-rw-r--r--   0 nic       (1000) nic       (1000)     3430 2024-05-03 01:38:55.000000 hydrobot-0.6.0/requirements_dev.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)      506 2024-03-11 01:19:58.000000 hydrobot-0.6.0/requirements_test.txt
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2024-05-12 23:08:50.092015 hydrobot-0.6.0/setup.cfg
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.082015 hydrobot-0.6.0/tests/
+-rw-r--r--   0 nic       (1000) nic       (1000)    53248 2024-02-26 00:40:14.000000 hydrobot-0.6.0/tests/.coverage
+-rw-r--r--   0 nic       (1000) nic       (1000)       38 2023-11-02 02:57:00.000000 hydrobot-0.6.0/tests/__init__.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     1017 2024-04-10 21:52:59.000000 hydrobot-0.6.0/tests/conftest.py
+drwxr-xr-x   0 nic       (1000) nic       (1000)        0 2024-05-12 23:08:50.082015 hydrobot-0.6.0/tests/test_data/
+-rw-r--r--   0 nic       (1000) nic       (1000)      245 2024-04-10 21:52:59.000000 hydrobot-0.6.0/tests/test_data/site_list_response.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)    74114 2024-05-03 01:38:55.000000 hydrobot-0.6.0/tests/test_data/xml_test_data_file.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)     6584 2024-05-03 01:38:55.000000 hydrobot-0.6.0/tests/test_data/xml_test_data_no_check.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)    12469 2024-05-03 01:38:55.000000 hydrobot-0.6.0/tests/test_data/xml_test_data_no_qual.xml
+-rw-r--r--   0 nic       (1000) nic       (1000)     2929 2024-03-11 01:19:58.000000 hydrobot-0.6.0/tests/test_data_sources.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     9736 2024-05-03 01:38:55.000000 hydrobot-0.6.0/tests/test_data_structure.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    17323 2024-05-09 02:28:04.000000 hydrobot-0.6.0/tests/test_evaluator.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    11873 2024-05-09 22:46:55.000000 hydrobot-0.6.0/tests/test_filters.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    45119 2024-05-10 02:44:18.000000 hydrobot-0.6.0/tests/test_processor.py
+-rw-r--r--   0 nic       (1000) nic       (1000)     2557 2024-04-07 23:15:31.000000 hydrobot-0.6.0/tests/test_utils.py
+-rw-r--r--   0 nic       (1000) nic       (1000)    27001 2024-05-09 22:50:28.000000 hydrobot-0.6.0/tests/test_web_integration.py
```

### Comparing `hydrobot-0.5.2/.gitignore` & `hydrobot-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/.pre-commit-config.yaml` & `hydrobot-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/.readthedocs.yaml` & `hydrobot-0.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/CONTRIBUTING.rst` & `hydrobot-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/HISTORY.rst` & `hydrobot-0.6.0/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -72,7 +72,19 @@
 * Added a supplementary R script to repo
 
 0.5.2 (2024-04-10)
 ----------------------------------
 
 * Updated from standard plotly to streamlit dash
 * Added to QC encoder: Water Temp downgraded to 200 if last check longer than 2 months ago.
+
+0.6.0 (2024-05-13)
+----------------------------------
+
+* Processor objest now works with pd.Dataframes rather than pd.Series
+* Out of validation range now has adjustable ranges, can support multiple maximum QCs with different time period lengths
+* Changes to data and quality codes now have reason codes associated with any changes
+* Check data can be read from xml directly
+* Any missing xml data is no longer read in as zeroes
+* config.yaml supports 'today' input for to_date
+* Added in a constant shift value in config.yaml
+* Various DevOps improvements
```

### Comparing `hydrobot-0.5.2/LICENSE` & `hydrobot-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/Makefile` & `hydrobot-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/PKG-INFO` & `hydrobot-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobot
-Version: 0.5.2
+Version: 0.6.0
 Summary: A suite of processing tools for Hilltop hydrological data.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
 Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
 Project-URL: Documentation, https://hydrobot.readthedocs.io
 Project-URL: Package, https://pypi.org/project/hydrobot
@@ -19,14 +19,16 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: hilltop-py>=2.3.1
 Requires-Dist: data-annalist>=0.4.1
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: defusedxml>=0.7.1
 Requires-Dist: plotly>=5.20.0
+Requires-Dist: streamlit>=1.33.0
+Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.2; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Requires-Dist: pytest-dependency>=0.5.2; extra == "test"
 Requires-Dist: pytest-mock>=3.12.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
@@ -80,27 +82,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.5.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.5.2/
+    python -m venv path/to/venv/hydrobot0.6.0/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.5.2/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.0/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -115,17 +117,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.2_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.0_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.2_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.0_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.5.2/README.rst` & `hydrobot-0.6.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -39,27 +39,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.5.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.5.2/
+    python -m venv path/to/venv/hydrobot0.6.0/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.5.2/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.0/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -74,17 +74,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.2_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.0_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.2_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.0_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.5.2/docs/Makefile` & `hydrobot-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/docs/conf.py` & `hydrobot-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/docs/hydrobot.rst` & `hydrobot-0.6.0/docs/hydrobot.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/docs/installation.rst` & `hydrobot-0.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/docs/make.bat` & `hydrobot-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/hydrobot/data_acquisition.py` & `hydrobot-0.6.0/hydrobot/data_acquisition.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Main module."""
 
 from xml.etree import ElementTree
 
 import pandas as pd
+import yaml
 from annalist.annalist import Annalist
 from hilltoppy.utils import build_url, get_hilltop_xml
 
 from hydrobot.data_structure import parse_xml
 
 annalizer = Annalist()
 
@@ -105,30 +106,29 @@
         "TimeRange",
         site=site,
         measurement=measurement,
         tstype=tstype,
     )
 
     hilltop_xml = get_hilltop_xml(url)
-    print(url)
 
     data_object = parse_xml(hilltop_xml)
 
     return hilltop_xml, data_object
 
 
 def get_series(
     base_url,
     hts,
     site,
     measurement,
     from_date,
     to_date,
     tstype="Standard",
-) -> tuple[ElementTree.Element, pd.Series | pd.DataFrame]:
+) -> tuple[ElementTree.Element, pd.DataFrame]:
     """Pack data from get_data as a pd.Series.
 
     Parameters
     ----------
     base_url : str
         The base URL of the web service.
     hts : str
@@ -169,51 +169,59 @@
                 timestamps = data.index.map(
                     lambda x: pd.Timestamp(int(x) - mowsecs_offset, unit="s")
                 )
                 data.index = pd.to_datetime(timestamps)
             else:
                 data.index = pd.to_datetime(data.index)
     else:
-        data = pd.Series({})
+        data = pd.DataFrame({})
     return xml, data
 
 
-def import_inspections(filename):
+def import_inspections(filename, check_col, logger_col, source="INS", use_for_qc=True):
     """Import inspections as generated by R script."""
     try:
         insp_df = pd.read_csv(filename)
         if not insp_df.empty:
             insp_df["Time"] = pd.to_datetime(insp_df["Date"] + " " + insp_df["Time"])
             insp_df = insp_df.set_index("Time")
             insp_df = insp_df.drop(columns=["Date"])
             insp_df["Comment"] = insp_df.apply(
                 lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
             )
         else:
-            insp_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
+            insp_df = pd.DataFrame({"Time": [], "Value": [], "Comment": []})
     except FileNotFoundError:
-        insp_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
+        insp_df = pd.DataFrame({"Time": [], "Value": [], "Comment": []})
+    insp_df = insp_df.rename(columns={check_col: "Value", logger_col: "Logger"})
+    insp_df = insp_df[~insp_df["Value"].isna()]
+    insp_df["Source"] = source
+    insp_df["QC"] = use_for_qc
     return insp_df
 
 
-def import_prov_wq(filename):
+def import_prov_wq(filename, check_col, logger_col, source="SOE", use_for_qc=False):
     """Import prov_wq checks as obtained by R script."""
     try:
         prov_df = pd.read_csv(filename)
         if not prov_df.empty:
             prov_df["Time"] = pd.to_datetime(prov_df["Date"] + " " + prov_df["Time"])
             prov_df = prov_df.set_index("Time")
             prov_df = prov_df.drop(columns=["Date"])
             prov_df["Comment"] = prov_df.apply(
                 lambda x: f"{x['InspectionStaff']}: {x['Notes']}", axis=1
             )
         else:
-            prov_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
+            prov_df = pd.DataFrame({"Time": [], "Value": [], "Comment": []})
     except FileNotFoundError:
-        prov_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
+        prov_df = pd.DataFrame({"Time": [], "Value": [], "Comment": []})
+    prov_df = prov_df.rename(columns={check_col: "Value", logger_col: "Logger"})
+    prov_df = prov_df[~prov_df["Value"].isna()]
+    prov_df["Source"] = source
+    prov_df["QC"] = use_for_qc
     return prov_df
 
 
 def import_ncr(filename):
     """Import non conformance data as obtained by R script."""
     try:
         ncr_df = pd.read_csv(filename)
@@ -225,7 +233,34 @@
                 axis=1,
             )
         else:
             ncr_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
     except FileNotFoundError:
         ncr_df = pd.DataFrame({"Time": [], "Temp Check": [], "Comment": []})
     return ncr_df
+
+
+def config_yaml_import(file_name: str):
+    """
+    Import config.yaml.
+
+    Parameters
+    ----------
+    file_name : str
+        Path to config.yaml
+
+    Returns
+    -------
+    dict
+        For inputting into processor processing_parameters
+    """
+    with open(file_name) as yaml_file:
+        processing_parameters = yaml.safe_load(yaml_file)
+
+    if "inspection_expiry" in processing_parameters:
+        a = processing_parameters["inspection_expiry"]
+        d = {}
+        for key in a:
+            d[pd.DateOffset(**a[key])] = key
+        processing_parameters["inspection_expiry"] = d
+
+    return processing_parameters
```

### Comparing `hydrobot-0.5.2/hydrobot/data_sources.py` & `hydrobot-0.6.0/hydrobot/data_sources.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,57 +5,63 @@
 import numpy as np
 import pandas as pd
 
 
 class QualityCodeEvaluator:
     """Basic QualityCodeEvaluator only compares magnitude of differences."""
 
-    def __init__(self, qc_500_limit, qc_600_limit, name=""):
+    def __init__(self, qc_500_limit, qc_600_limit, name="", constant_check_shift=0):
         """Initialize QualityCodeEvaluator.
 
         Parameters
         ----------
         qc_500_limit : numerical
             Threshold between QC 400 and QC 500
         qc_600_limit : numerical
             Threshold between QC 500 and QC 600
         name : str
             Name of the data source
+        constant_check_shift : numerical
+            Shifts the check data by a fixed amount
         """
         self.qc_500_limit = qc_500_limit
         self.qc_600_limit = qc_600_limit
         self.name = name
+        self.constant_check_shift = constant_check_shift
 
     def __repr__(self):
         """QualityCodeEvaluator representation."""
         return repr(f"QualityCodeEvaluator '{self.name}'")
 
     def find_qc(self, base_datum, check_datum):
-        """Find the base quality codes.
+        """
+        Find the base quality codes.
 
         Parameters
         ----------
         base_datum : numerical
             Closest continuum datum point to the check
         check_datum : numerical
-            The check data to verify the continuous data
+            The check data to verify the continuous data, shifted by any constant_check_shift
 
         Returns
         -------
         int
             The Quality code
 
         """
+        check_datum = check_datum + self.constant_check_shift
         diff = np.abs(base_datum - check_datum)
         if diff < self.qc_600_limit:
             qc = 600
         elif diff < self.qc_500_limit:
             qc = 500
         else:
             qc = 400
+
         return qc
 
 
 class TwoLevelQualityCodeEvaluator(QualityCodeEvaluator):
     """QualityCodeEvaluator for standards such as water level.
 
     Fixed error up to given threshold, percentage error after that.
@@ -65,16 +71,18 @@
         self,
         qc_500_limit,
         qc_600_limit,
         qc_500_percent,
         qc_600_percent,
         limit_percent_threshold,
         name="",
+        constant_check_shift=0,
     ):
-        """Initialize TwoLevelQualityCodeEvaluator.
+        """
+        Initialize TwoLevelQualityCodeEvaluator.
 
         Parameters
         ----------
         qc_500_limit : numerical
             Threshold between QC 400 and QC 500 for linear portion
         qc_600_limit : numerical
             Threshold between QC 500 and QC 600 for linear portion
@@ -84,37 +92,40 @@
             Threshold between QC 500 and QC 600 for percentage portion
         limit_percent_threshold
             Value at which the evaluator transitions between linear and percentage
             QC comparison
         name : str
             Name of the data source
         """
-        QualityCodeEvaluator.__init__(self, qc_500_limit, qc_600_limit, name)
+        QualityCodeEvaluator.__init__(
+            self, qc_500_limit, qc_600_limit, name, constant_check_shift
+        )
         self.qc_500_percent = qc_500_percent
         self.qc_600_percent = qc_600_percent
         self.limit_percent_threshold = limit_percent_threshold
 
     def find_qc(self, base_datum, check_datum):
         """Find the base quality codes with two stages.
 
         The two stages are: a flat and percentage QC threshold.
 
         Parameters
         ----------
         base_datum : numerical
             Closest continuum datum point to the check
         check_datum : numerical
-            The check data to verify the continuous data
+            The check data to verify the continuous data, shifted by any constant_check_shift
 
         Returns
         -------
         int
             The Quality code
 
         """
+        check_datum = check_datum + self.constant_check_shift
         if base_datum < self.limit_percent_threshold:
             # flat qc check
             diff = np.abs(base_datum - check_datum)
             if diff < self.qc_600_limit:
                 qc = 600
             elif diff < self.qc_500_limit:
                 qc = 500
```

### Comparing `hydrobot-0.5.2/hydrobot/data_structure.py` & `hydrobot-0.6.0/hydrobot/data_structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,27 +134,27 @@
         True
         """
         item_info_root = ElementTree.Element(
             "ItemInfo", attrib={"ItemNumber": str(self.item_number)}
         )
 
         item_name_element = ElementTree.SubElement(item_info_root, "ItemName")
-        item_name_element.text = self.item_name
+        item_name_element.text = str(self.item_name)
 
         item_format_element = ElementTree.SubElement(item_info_root, "ItemFormat")
-        item_format_element.text = self.item_format
+        item_format_element.text = str(self.item_format)
 
         divisor_element = ElementTree.SubElement(item_info_root, "Divisor")
-        divisor_element.text = self.divisor
+        divisor_element.text = str(self.divisor)
 
         units_element = ElementTree.SubElement(item_info_root, "Units")
-        units_element.text = self.units
+        units_element.text = str(self.units)
 
         format_element = ElementTree.SubElement(item_info_root, "Format")
-        format_element.text = self.format
+        format_element.text = str(self.format)
 
         return item_info_root
 
     def __repr__(self):
         """Overwriting the __repr__ to mimic xml tree structure."""
         repr = f"""
         <ItemInfo ItemNumber="{self.item_number}">
@@ -347,26 +347,26 @@
         """
         data_source_root = ElementTree.Element(
             "DataSource",
             attrib={"Name": self.name, "NumItems": str(self.num_items)},
         )
 
         ts_type_element = ElementTree.SubElement(data_source_root, "TSType")
-        ts_type_element.text = self.ts_type
+        ts_type_element.text = str(self.ts_type)
 
         data_type_element = ElementTree.SubElement(data_source_root, "DataType")
-        data_type_element.text = self.data_type
+        data_type_element.text = str(self.data_type)
 
         interpolation_element = ElementTree.SubElement(
             data_source_root, "Interpolation"
         )
-        interpolation_element.text = self.interpolation
+        interpolation_element.text = str(self.interpolation)
 
         item_format_element = ElementTree.SubElement(data_source_root, "ItemFormat")
-        item_format_element.text = self.item_format
+        item_format_element.text = str(self.item_format)
 
         if self.item_info is not None:
             data_source_root.extend(
                 [element.to_xml_tree() for element in self.item_info]
             )
         return data_source_root
 
@@ -392,15 +392,15 @@
 class Data:
     """Data Class."""
 
     def __init__(
         self,
         date_format: str,
         num_items: int,
-        timeseries: pd.Series | pd.DataFrame,
+        timeseries: pd.DataFrame,
     ):
         """
         Initialize a Data instance.
 
         Parameters
         ----------
         date_format : str
@@ -495,22 +495,15 @@
             elif child.tag == "Gap":
                 pass
             else:
                 raise ValueError(
                     "Possibly Malformed XML: Data items not tagged with 'E' or 'V'."
                 )
 
-        if num_items > 1:
-            timeseries = pd.DataFrame(data_list).set_index("T")
-        else:
-            data_key = list(data_list[0].keys())[1]
-            timeseries = pd.Series(
-                [dat[data_key] for dat in data_list],
-                index=[dat["T"] for dat in data_list],
-            )
+        timeseries = pd.DataFrame(data_list).set_index("T")
         return cls(date_format, num_items, timeseries)
 
     def to_xml_tree(self):
         """
         Convert the Data instance to an XML ElementTree.
 
         Returns
@@ -537,38 +530,27 @@
             "Data",
             attrib={
                 "DateFormat": self.date_format,
                 "NumItems": str(self.num_items),
             },
         )
 
-        if isinstance(self.timeseries, pd.Series):
-            for date, val in self.timeseries.items():
-                if pd.isna(val):
-                    element = ElementTree.SubElement(data_root, "Gap")
-                else:
-                    element = ElementTree.SubElement(data_root, "E")
-                    timestamp = ElementTree.SubElement(element, "T")
-                    timestamp.text = str(date)
-                    val_item = ElementTree.SubElement(element, "I1")
-                    val_item.text = str(val)
-        elif isinstance(self.timeseries, pd.DataFrame):
-            for date, row in self.timeseries.iterrows():
-                if pd.isna(row).all():
-                    # If all values in a row are NaNs, insert a Gap.
-                    element = ElementTree.SubElement(data_root, "Gap")
-                else:
-                    element = ElementTree.SubElement(data_root, "E")
-                    timestamp = ElementTree.SubElement(element, "T")
-                    timestamp.text = str(date)
-                    for i, val in enumerate(row):
-                        # If only one field in the element is a NaN, leave it blank?
-                        val_item = ElementTree.SubElement(element, f"I{i+1}")
-                        if not pd.isna(val):
-                            val_item.text = str(val)
+        for date, row in self.timeseries.iterrows():
+            if (pd.isna(row).sum() > 0) or (sum(row.to_numpy() == "nan") > 0):
+                # If all values in a row are NaNs, insert a Gap.
+                element = ElementTree.SubElement(data_root, "Gap")
+            else:
+                element = ElementTree.SubElement(data_root, "E")
+                timestamp = ElementTree.SubElement(element, "T")
+                timestamp.text = str(date)
+                for i, val in enumerate(row):
+                    # If only one field in the element is a NaN, leave it blank?
+                    val_item = ElementTree.SubElement(element, f"I{i+1}")
+                    if not pd.isna(val):
+                        val_item.text = str(val)
 
         # Collapse all duplicate Gap tags into a single Gap marker:
         current_gap_count = 0
         gaps_to_remove = []
         for elem in data_root:
             if elem.tag == "Gap":
                 current_gap_count += 1
@@ -780,15 +762,15 @@
 {self.data_source}
 {self.data}
 </DataSourceBlob[Measurement]">
         """
         return re.sub(r"^\s*\n", "", repr, flags=re.MULTILINE)
 
 
-def parse_xml(source) -> list[DataSourceBlob] | None:
+def parse_xml(source) -> list[DataSourceBlob]:
     """
     Parse Hilltop XML to get a list of DataSourceBlob objects.
 
     Parameters
     ----------
     source : str or ElementTree.Element or bytes or bytearray or file-like object
         The source XML to parse. It can be a raw XML string, an ElementTree object,
@@ -836,22 +818,20 @@
         # file-like object.
         root = DefusedElementTree.parse(source).getroot()
     else:
         raise ValueError("Unsupported XML source type.")
 
     if root.tag == "HilltopServer":
         ElementTree.indent(root, space="\t")
-        print("Hilltop xml possibly returned no data. Check for yourself:")
-        ElementTree.dump(root)
         err_text = root.findtext("Error")
-        if "No data from " in str(err_text):
-            warnings.warn(str(err_text), stacklevel=1)
-            return None
+        if "No data" in str(err_text):
+            warnings.warn(f"Empty hilltop response: {err_text}", stacklevel=1)
         else:
             raise ValueError(err_text)
+
     elif root.tag != "Hilltop":
         raise ValueError(
             f"Possibly malformed Hilltop xml. Root tag is '{root.tag}',"
             " should be 'Hilltop'."
         )
     data_source_blob_list = []
     for child in root.iter():
@@ -885,33 +865,33 @@
                 _, sorted_item_list = zip(*sorted_items, strict=True)
 
                 sorted_item_names = list(sorted_item_names)
                 data_source_blob.data_source.item_info = list(sorted_item_list)
 
             else:
                 sorted_item_names = []
-            if len(sorted_item_names) > 1 and isinstance(
+            if len(sorted_item_names) > 0 and isinstance(
                 data_source_blob.data.timeseries, pd.DataFrame
             ):
                 cols = {
                     col: name
                     for col, name in zip(
                         data_source_blob.data.timeseries.columns,
                         sorted_item_names,
                         strict=True,
                     )
                 }
                 data_source_blob.data.timeseries = (
                     data_source_blob.data.timeseries.rename(columns=cols)
                 )
-            elif len(sorted_item_names) > 0:
-                data_source_blob.data.timeseries.name = sorted_item_names[0]
             else:
                 # It seems that if iteminfo is missing it's always a QC
-                data_source_blob.data.timeseries.name = "QualityCode"
+                data_source_blob.data.timeseries = (
+                    data_source_blob.data.timeseries.rename(columns={"I1": "Value"})
+                )
             data_source_blob.data.timeseries.index.name = "Time"
             data_source_blob_list += [data_source_blob]
 
     return data_source_blob_list
 
 
 def write_hilltop_xml(data_source_blob_list, output_path):
```

### Comparing `hydrobot-0.5.2/hydrobot/evaluator.py` & `hydrobot-0.6.0/hydrobot/evaluator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 """Tools for checking quality and finding problems in the data."""
+
 import warnings
 
 import numpy as np
 import pandas as pd
 from annalist.annalist import Annalist
 
 from hydrobot.data_sources import QualityCodeEvaluator
 
 annalizer = Annalist()
 
 
-def gap_finder(data: pd.Series):
+def gap_finder(data: pd.Series) -> list:
     """
-    Find gaps in a series of data (indicated by np.isnan()).
-
-    Returns a list of tuples indicating the start of the gap, and the number
-    of entries that are NaN
+    Find the indices and lengths of gaps (sequences of NaN values) in a pandas Series.
 
     Parameters
     ----------
-    data : pandas.Series
-        Input data to be clipped.
+    data : pd.Series
+        Input Series containing NaN values.
 
     Returns
     -------
-    List of Tuples
-        Each element in the list gives the index value for the start of the gap
-        and the length of the gap
+    list :
+        List of tuples, each containing the index of a NaN value, the length of the gap
+        containing it, and True for strictness.
     """
-    idx0 = np.flatnonzero(np.r_[True, np.diff(np.isnan(data)) != 0, True])
+    # Find the indices where NaN values start and end
+    idx0 = np.flatnonzero(np.r_[True, np.diff(pd.isna(data)) != 0, True])
+
+    # Calculate the length of each gap
     count = np.diff(idx0)
-    idx = idx0[:-1]
-    valid_mask = pd.isna(data.iloc[idx])
-    out_idx = idx[valid_mask]
+
+    # Mask for the gaps that contain NaN values
+    valid_mask = pd.isna(data.iloc[idx0[:-1]])
+
+    # Select indices of gaps that contain NaN values
+    out_idx = idx0[:-1][valid_mask]
+
+    # Select lengths of gaps that contain NaN values
     out_count = count[valid_mask]
+
+    # Select indices of NaN values in the original Series
     indices = data.iloc[out_idx].index
-    out = zip(indices, out_count, strict=True)
 
-    return list(out)
+    # Create a list of tuples containing index, gap length, and strictness
+    out = list(zip(indices, out_count, [True] * len(indices), strict=True))
+
+    return out
 
 
 def small_gap_closer(series: pd.Series, gap_limit: int) -> pd.Series:
     """
     Remove small gaps from a series.
 
     Gaps are defined by a sequential number of np.NaN values
@@ -78,15 +88,15 @@
 
 
 def check_data_quality_code(
     series: pd.Series,
     check_series: pd.Series,
     qc_evaluator: QualityCodeEvaluator,
     gap_limit=10800,
-) -> pd.Series:
+) -> pd.DataFrame:
     """
     Quality Code Check Data.
 
     Quality codes data based on the difference between the standard series and
     the check data
 
     Parameters
@@ -106,24 +116,31 @@
         The QC values of the series, indexed by the END time of the QC period
     """
     first_data_date = series.index[0]
     last_data_date = series.index[-1]
     if check_series.empty and isinstance(first_data_date, pd.Timestamp):
         # Maybe you should go find that check data
         warnings.warn("Warning: No check data", stacklevel=2)
-        return pd.Series({first_data_date: np.NaN})
+        return pd.DataFrame(
+            columns=["Value", "Code", "Details"],
+            index=[first_data_date],
+        )
     first_check_date = check_series.index[0]
     last_check_date = check_series.index[-1]
     if (
         isinstance(first_data_date, pd.Timestamp)
         and isinstance(last_data_date, pd.Timestamp)
         and isinstance(first_check_date, pd.Timestamp)
         and isinstance(last_check_date, pd.Timestamp)
     ):
-        qc_series = pd.Series({first_data_date: np.NaN})
+        # qc_series = pd.Series({first_data_date: np.NaN})
+        qc_frame = pd.DataFrame(
+            columns=["Value", "Code", "Details"],
+            index=[first_data_date],
+        )
         if first_check_date < first_data_date or last_check_date > last_data_date:
             # Can't check something that's not there
             raise KeyError(
                 "Error: check data out of range. "
                 f"First check date: {first_check_date}. "
                 f"First data date: {first_data_date}. "
                 f"Last check date: {last_check_date}. "
@@ -136,65 +153,91 @@
                     adjusted_time = find_nearest_valid_time(series, check_time)
                     if abs((adjusted_time - check_time).total_seconds()) < gap_limit:
                         qc_value = qc_evaluator.find_qc(
                             series[adjusted_time], check_value
                         )
                     else:
                         qc_value = 200
-                    qc_series[check_time] = qc_value
+                    qc_frame.loc[check_time, "Value"] = qc_value
+                    qc_frame.loc[check_time, "Code"] = "CHK"
+                    qc_frame.loc[check_time, "Details"] = (
+                        f"Check value at {check_time} used to validate "
+                        f"data value at {adjusted_time}."
+                    )
                 else:
                     raise KeyError("Series indices should be pandas.Timestamp.")
-            qc_series = qc_series.shift(-1, fill_value=0)
-        return pd.Series(qc_series)
+            qc_frame = qc_frame.shift(periods=-1)
+            qc_frame.loc[qc_frame.index[-1], "Value"] = 0
+        return qc_frame
     else:
         raise KeyError("Series indices should be pandas.Timestamp.")
 
 
-def missing_data_quality_code(series, qc_series, gap_limit):
+def missing_data_quality_code(std_series, qc_data, gap_limit):
     """
     Make sure that missing data is QC100.
 
-    Returns qc_series with QC100 values added where series is NaN
+    Returns qc_data with QC100 values added where std_series is NaN
 
     Parameters
     ----------
-    series : pd.Series
+    std_series : pd.Series
         Base series which may contain NaNs
-    qc_series
-        QC series for base series without QC100 values
+    qc_data
+        QC series for base std_series without QC100 values
     gap_limit
         Maximum size of gaps which will be ignored
 
     Returns
     -------
     pd.Series
         The modified QC series, indexed by the start time of the QC period
     """
-    for gap in gap_finder(series):
+    for gap in gap_finder(std_series):
         if gap[1] > gap_limit:
-            end_idx = series.index.get_loc(gap[0]) + gap[1]
+            end_idx = std_series.index.get_loc(gap[0]) + gap[1]
             # end of gap should recover the value from previous
-            if end_idx < len(series):
-                prev_values = qc_series[qc_series.index <= series.index[end_idx]]
-                prev_values = prev_values[prev_values > 100]
-                prev_values = prev_values.sort_index()
-                qc_series[series.index[end_idx]] = prev_values.iloc[-1]
-                qc_series = qc_series.sort_index()
+            if end_idx < len(std_series):
+                prev_qc_data = qc_data[qc_data.index <= std_series.index[end_idx]]
+                prev_qc_data = prev_qc_data[prev_qc_data["Value"] > 100]
+                prev_qc_data = prev_qc_data.sort_index()
+                qc_data.loc[std_series.index[end_idx]] = prev_qc_data.iloc[-1]
+                if std_series.index[end_idx] in prev_qc_data.index:
+                    qc_data.loc[std_series.index[end_idx], "Details"] = (
+                        qc_data.loc[std_series.index[end_idx], "Details"]
+                        + f" [End of gap which started at {gap[0]}]"
+                    )
+                else:
+                    qc_data.loc[std_series.index[end_idx], "Details"] = (
+                        f"End of gap which started at {gap[0]}. "
+                        f"Returning to QC code first assigned at {prev_qc_data.index[-1]}"
+                    )
+                qc_data = qc_data.sort_index()
 
             # getting rid of any stray QC codes in the middle
-
-            drop_series = qc_series
+            drop_series = qc_data["Value"]
             drop_series = drop_series[drop_series.index > gap[0]]
-            drop_series = drop_series[drop_series.index <= series.index[end_idx - 1]]
-            qc_series = qc_series.drop(drop_series.index)
+            drop_series = drop_series[
+                drop_series.index <= std_series.index[end_idx - 1]
+            ]
+            qc_data = qc_data.drop(drop_series.index)
 
             # start of gap
-            qc_series[gap[0]] = 100
+            qc_data.loc[gap[0], "Value"] = 100
+            qc_data.loc[gap[0], "Code"] = "GAP"
+            if end_idx >= len(std_series):
+                gap_end = std_series.index[-1]
+            else:
+                gap_end = std_series.index[end_idx]
+            qc_data.loc[
+                gap[0], "Details"
+            ] = f"Missing data amounting to {(gap_end - gap[0])}"
+            qc_data = qc_data.sort_index()
 
-    return qc_series.sort_index()
+    return qc_data.sort_index()
 
 
 def find_nearest_time(series, dt):
     """
     Find the time in the series that is closest to dt.
 
     For example for the series::
@@ -350,17 +393,19 @@
     gap_time = ave_period * (len(base_series) - len(base_series.dropna()) + 1)
     print(f"Missing {gap_time} of data, that's {gap_time/total_time*100}%")
 
     # QCs
     split_data = splitter(base_series, qc_series, frequency)
     for qc in split_data:
         print(
-            f"Data that is QC{qc} makes up {len(split_data[qc].dropna()) / len(base_series.dropna()) * 100:.2f}% of "
-            f"the "
-            f"workable data and {len(split_data[qc].dropna()) / len(base_series) * 100:.2f}% of the time period"
+            f"Data that is QC{qc} makes up "
+            f"{len(split_data[qc].dropna()) / len(base_series.dropna()) * 100:.2f}% "
+            "of the workable data and "
+            f"{len(split_data[qc].dropna()) / len(base_series) * 100:.2f}% "
+            "of the time period"
         )
 
 
 def splitter(base_series, qc_series, frequency):
     """
     Split the data up by QC code.
 
@@ -379,14 +424,15 @@
     Returns
     -------
     dict of int:pd.Series pairs
         Keys are the QC values as ints, values are series of data that fits
     """
     qc_list = [0, 100, 200, 300, 400, 500, 600]
     return_dict = {}
+
     for qc in qc_list:
         if qc == 100:
             return_dict[qc] = (
                 base_data_meets_qc(base_series, qc_series, qc)
                 .fillna(base_series.median())
                 .asfreq(frequency)
             )
@@ -394,15 +440,15 @@
             return_dict[qc] = base_data_meets_qc(base_series, qc_series, qc).asfreq(
                 frequency
             )
 
     return return_dict
 
 
-def max_qc_limiter(qc_series: pd.Series, max_qc) -> pd.Series:
+def max_qc_limiter(qc_data: pd.DataFrame, max_qc) -> pd.DataFrame:
     """
     Enforce max_qc on a QC series.
 
     Replaces all values with QCs above max_qc with max_qc
 
     Parameters
     ----------
@@ -412,92 +458,162 @@
         maximum allowed value. None imposes no limit.
 
     Returns
     -------
     pd.Series
         qc_series with too high QCs limited to max_qc
     """
-    return pd.Series(qc_series.clip(np.NaN, max_qc))
+    clipped_data = qc_data["Value"].clip(np.NaN, max_qc)
+
+    diff_idxs = qc_data[qc_data["Value"] != clipped_data].index
+
+    qc_data.loc[diff_idxs, "Code"] = qc_data.loc[diff_idxs, "Code"] + ", LIM"
+    qc_data.loc[diff_idxs, "Details"] = (
+        qc_data.loc[diff_idxs, "Details"]
+        + f" [Site QC limit applies to a maximum of {max_qc}.]"
+    )
+    qc_data["Value"] = clipped_data
+
+    return qc_data
 
 
 def quality_encoder(
     base_series: pd.Series,
     check_series: pd.Series,
     qc_evaluator: QualityCodeEvaluator,
     gap_limit: int,
     max_qc=np.NaN,
+    interval_dict: dict = None,
 ) -> pd.Series:
     """
     Return complete QC series.
 
     Parameters
     ----------
     base_series : pd.Series
         Base time series data
     check_series : pd.Series
         Check data time series
     qc_evaluator : data_sources.QualityCodeEvaluator
         Handler for QC comparisons
-    gap_limit
+    gap_limit : int
         Maximum size of gaps which will be ignored
-    max_qc
+    max_qc : numeric
         Maximum allowed QC value
+    interval_dict : dict
+        Key:Value pairs of max_interval:downgraded_qc for single_downgrade_out_of_validation
 
     Returns
     -------
     pd.Series
         The modified QC series, indexed by the start time of the QC period
     """
     qc_series = check_data_quality_code(base_series, check_series, qc_evaluator)
-    qc_series = downgrade_out_of_validation(qc_series, check_series)
+    if interval_dict is None:
+        interval_dict = {}
+    qc_series = bulk_downgrade_out_of_validation(
+        qc_series, check_series, interval_dict=interval_dict
+    )
     qc_series = missing_data_quality_code(base_series, qc_series, gap_limit=gap_limit)
+
     qc_series = max_qc_limiter(qc_series, max_qc)
     # qc_series.index.name = "Time"
     # qc_series.name = "Value"
     return qc_series
 
 
-_default_date_offset = pd.DateOffset(months=2)
+def bulk_downgrade_out_of_validation(
+    qc_frame: pd.DataFrame,
+    check_series: pd.Series,
+    interval_dict: dict,
+    day_end_rounding: bool = True,
+):
+    """
+    Applies caps on quality codes for any data that has gaps between check data that is too large.
 
+    Utilises single_downgrade_out_of_validation multiple times for different time periods.
 
-def downgrade_out_of_validation(
-    qc_series: pd.Series,
+    Parameters
+    ----------
+    qc_series : pd.Series
+        Quality series that potentially needs downgrading
+    check_series : pd.Series
+        Check series to check for frequency of checks
+    interval_dict : dict
+        Key:Value pairs of max_interval:downgraded_qc for single_downgrade_out_of_validation
+    day_end_rounding : bool
+        Whether to round to the day end. If true, downgraded data starts at midnight
+
+    Returns
+    -------
+    pd.Series
+        The qc_series with any downgraded QCs added in
+
+    """
+    for key in interval_dict:
+        qc_frame = single_downgrade_out_of_validation(
+            qc_frame, check_series, key, interval_dict[key], day_end_rounding
+        )
+    return qc_frame
+
+
+def single_downgrade_out_of_validation(
+    qc_frame: pd.DataFrame,
     check_series: pd.Series,
-    max_interval: pd.DateOffset = _default_date_offset,
+    max_interval: pd.DateOffset,
     downgraded_qc: int = 200,
     day_end_rounding: bool = True,
 ):
     """
-    Downgrades any data that has gaps between check data that is too large.
+    Applies a cap on quality codes for any data that has gaps between check data that is too large.
+
+    Only applies a single cap quality code, see bulk_downgrade_out_of_validation for multiple steps.
 
     Parameters
     ----------
-    qc_series : pd.Series
+    qc_frame : pd.DataFrame
         Quality series that potentially needs downgrading
     check_series : pd.Series
         Check series to check for frequency of checks
     max_interval : pd.DateOffset
         How long of a gap between checks before the data gets downgraded
     downgraded_qc : int
         Which code the quality data gets downgraded to
     day_end_rounding : bool
         Whether to round to the day end. If true, downgraded data starts at midnight
 
     Returns
     -------
-    pd.Series
-        The qc_series with any downgraded data added in
+    pd.DataFrame
+        The qc_series with any downgraded QCs added in
     """
     # When they should have their next check by
     due_date = check_series.index + max_interval
     due_date = due_date[:-1]
     if day_end_rounding:
         due_date = due_date.ceil("D")
     # Whether there has been a check since then
-    overdue = due_date < check_series.index[1:]
+    overdue = (due_date < check_series.index[1:]) & (
+        qc_frame.loc[check_series.index[:-1], "Value"] > downgraded_qc
+    )
     # Select overdue times
     unvalidated = due_date[overdue]
-    downgraded_times = pd.Series([downgraded_qc for i in unvalidated], unvalidated)
+    downgraded_times = pd.DataFrame(
+        {
+            "Value": [downgraded_qc for _ in unvalidated],
+            "Code": ["OOV" for _ in unvalidated],
+            "Details": [
+                "Site inspection overdue. Last inspection at "
+                f"{check_series.index[idx]}. Data downgraded to QC{downgraded_qc} "
+                "until next inspection."
+                for idx in range(len(unvalidated))
+            ],
+        },
+        index=unvalidated,
+    )
+
     # combine and sort
     if not downgraded_times.empty:
-        qc_series = pd.concat([qc_series, downgraded_times]).sort_index()
-    return qc_series
+        qc_frame = pd.concat([qc_frame, downgraded_times]).sort_index()
+    # qc_frame.loc[qc_frame.index[-1], "Value"] = 0
+
+    return qc_frame
```

### Comparing `hydrobot-0.5.2/hydrobot/filters.py` & `hydrobot-0.6.0/hydrobot/filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -141,15 +141,16 @@
     return gaps_series
 
 
 def remove_range(
     input_series: pd.Series,
     from_date: str | None,
     to_date: str | None,
-    insert_gaps: bool | int = False,
+    min_gap_length: int = 1,
+    insert_gaps: str = "none",
 ):
     """
     Remove data from series in given range.
 
     Returns the input series without data between from_date and to_date
     inclusive.
 
@@ -162,32 +163,51 @@
     ----------
     input_series : pd.Series
         The series to have a section removed
     from_date : str | None
         Start of removed section
     to_date : str | None
         End of removed section
-    insert_gaps : bool or int
-        If True, inserts a gap.
-        If False, does not insert a gap.
-        If int, will insert gaps if missing more data points than insert_gaps
+    min_gap_length : int
+        Will insert gaps based on insert_gaps strategy if missing more data points than
+        min_gap_length in a row.
+    insert_gaps : str
+        If "all" will insert np.NaN at every missing point.
+        If "start" will insert np.NaN only at from_date.
+        If "end" will insert np.NaN only at to_date.
+        If "none" will insert no np.NaN values, and remove all timestamps completely.
 
     Returns
     -------
     pd.Series
         The series with relevant slice removed
     """
+    input_series = input_series.copy()
     slice_to_remove = input_series.loc[from_date:to_date]
-    series_to_return = input_series.drop(slice_to_remove.index)
-    if isinstance(insert_gaps, bool):
-        if insert_gaps:
-            series_to_return[from_date] = np.NaN
+
+    if len(slice_to_remove) >= min_gap_length:
+        if insert_gaps == "all":
+            series_to_return = input_series.copy()
+            series_to_return.loc[from_date:to_date] = np.NaN
+        else:
+            series_to_return = input_series.drop(slice_to_remove.index)
+            if insert_gaps == "start":
+                start_idx = slice_to_remove.index[0]
+                series_to_return[start_idx] = np.NaN
+            elif insert_gaps == "end":
+                end_idx = slice_to_remove.index[-1]
+                series_to_return[end_idx] = np.NaN
+            elif insert_gaps == "none":
+                pass
+            else:
+                raise ValueError(
+                    f"Unknown value for argument {insert_gaps}. Choose one of 'all', 'start', 'end', 'none'."
+                )
     else:
-        if len(slice_to_remove) > insert_gaps:
-            series_to_return[from_date] = np.NaN
+        series_to_return = input_series.drop(slice_to_remove.index)
     return series_to_return.sort_index()
 
 
 def trim_series(std_series: pd.Series, check_series: pd.Series) -> pd.Series:
     """
     Remove end of std series to match check series.
```

### Comparing `hydrobot-0.5.2/hydrobot/plotter.py` & `hydrobot-0.6.0/hydrobot/plotter.py`

 * *Files 21% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         gap_range = base_series.iloc[lower_idx:upper_idx]
         plt.plot(gap_range.index, gap_range)
         plt.plot(
             check,
             check_series[check],
             label="Check data",
             marker="o",
-            color="darkturquoise",
+            color="darkcyan",
         )
         plt.title(f"Check at {check}")
     if show:
         plt.show()
 
 
 def qc_colour(qc):
@@ -113,16 +113,16 @@
 
     Returns
     -------
     String
         Hex code for the colour of the QC
     """
     qc_dict = {
-        None: "darkslategrey",
-        "nan": "darkslategrey",
+        None: "darkgray",
+        "nan": "darkgray",
         0: "#9900ff",
         100: "#ff0000",
         200: "#8B5A00",
         300: "#d3d3d3",
         400: "#ffa500",
         500: "#00bfff",
         600: "#006400",
@@ -162,15 +162,15 @@
             marker=f"{'x' if qc==100 else '.'}",
         )
     plt.plot(
         check_series.index,
         check_series,
         label="Check data",
         marker="o",
-        color="gray",
+        color="darkgray",
         linestyle="None",
     )
     plt.xticks(rotation=45, ha="right")
 
     plt.legend()
     if show:
         plt.show()
@@ -192,16 +192,16 @@
     frequency : DateOffset or str
         Frequency to which the data gets set to
     show : bool
         Whether to show the plot directly when called
 
     Returns
     -------
-    None
-        Displays a plot
+    go.Figure
+
     """
     split_data = splitter(base_series, qc_series, frequency)
     fig = go.Figure()
     for qc in split_data:
         fig.add_trace(
             go.Scatter(
                 x=split_data[qc].index,
@@ -214,15 +214,15 @@
     if check_series is not None:
         fig.add_trace(
             go.Scatter(
                 x=check_series.index,
                 y=check_series,
                 mode="markers",
                 name="Check data",
-                marker=dict(color="darkturquoise", size=10),
+                marker=dict(color="darkcyan", size=10),
             )
         )
     fig.update_layout(
         title="Quality Control Plot",
         xaxis=dict(title="Date"),
         yaxis=dict(title="Value"),
         legend=dict(yanchor="top", y=0.99, xanchor="left", x=0.01),
@@ -260,15 +260,15 @@
         Displays a plot
     """
     qc_plotter(base_series, check_series, qc_series, frequency, show=False)
     plt.plot(
         raw_series.index,
         raw_series,
         label="Raw data",
-        color="black",
+        color="darkgray",
         marker="",
         linestyle="dashed",
     )
     plt.legend()
     if show:
         plt.show()
 
@@ -297,93 +297,89 @@
     frequency : DateOffset or str
         Frequency to which the data gets set to
     show : bool
         Whether to show the plot directly when called
 
     Returns
     -------
-    None
-        Displays a plot
+    comparison_qc_plotter_plotly
     """
     fig = qc_plotter_plotly(
         base_series, check_series, qc_series, frequency, show=False, **kwargs
     )
 
     fig.add_trace(
         go.Scatter(
             x=raw_series.index,
             y=raw_series,
             mode="lines",
             name="Raw data",
-            line=dict(color="black", dash="dash"),
+            line=dict(color="darkgray", dash="dash"),
         )
     )
     if show:
         fig.show()
     return fig
 
 
-def make_processing_dash(
-    fig,
-    title,
-    raw_standard_series,
-    hilltop_standard_series,
-    raw_check_series,
-    prov_wq,
-    inspections,
-    ncrs,
-):
+def make_processing_dash(fig, processor, check_data):
     """Make the processing dash.
 
     Sorry about these docs I'm in a rush.
     """
+    standard_data = processor.standard_data
+    check_data["Value"] += processor.quality_code_evaluator.constant_check_shift
+
+    htp_check = check_data[check_data["Source"] == "HTP"]
+    srv_check = check_data[check_data["Source"] == "INS"]
+    pwq_check = check_data[check_data["Source"] == "SOE"]
     fig.add_trace(
         go.Scatter(
-            x=raw_standard_series.index,
-            y=raw_standard_series.to_numpy(),
+            x=standard_data["Raw"].index,
+            y=standard_data["Raw"].to_numpy(),
             mode="lines",
             name="Raw data",
-            line=dict(color="darkslategray", width=0.5),
+            line=dict(color="darkgray", width=0.5),
             opacity=0.5,
         )
     )
     fig.add_trace(
         go.Scatter(
-            x=raw_check_series.index,
-            y=raw_check_series["Water Temperature Check"],
+            x=htp_check.index,
+            y=htp_check["Value"],
             mode="markers",
             name="Check data",
-            marker=dict(color="darkturquoise", size=10),
+            marker=dict(color="darkcyan", size=10),
         )
     )
     fig.add_trace(
         go.Scatter(
-            x=prov_wq.index,
-            y=prov_wq["Temp Check"],
+            x=pwq_check.index,
+            y=pwq_check["Value"],
             mode="markers",
             name="ProvWQ Check",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+            marker=dict(color="darkgray", size=10, symbol="square-open"),
         )
     )
     fig.add_trace(
         go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Check"],
+            x=srv_check.index,
+            y=srv_check["Value"],
             mode="markers",
             name="S123 Check",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+            marker=dict(color="darkgray", size=10, symbol="circle-open-dot"),
         )
     )
     fig.add_trace(
         go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Logger"],
+            x=srv_check.index,
+            y=srv_check["Logger"],
             mode="markers",
             name="S123 Logger",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+            marker=dict(color="darkgray", size=10, symbol="x-thin-open"),
         )
     )
     fig_subplots = make_subplots(
         rows=2,
         cols=1,
         shared_xaxes=True,
         vertical_spacing=0.02,
@@ -393,91 +389,85 @@
         ],
         row_heights=[0.7, 0.3],
     )
 
     for trace in fig.data:
         fig_subplots.add_trace(trace, row=1, col=1)
 
-    fig_subplots.update_layout(title=title)
+    fig_subplots.update_layout(title=processor.site)
 
     def find_nearest_periodic_indices(periodic_series, check_series):
         nearest_periodic_indices = []
         for check_index in check_series.index:
             # Calculate the difference between the check_index and every periodic index
             time_diff = np.abs(periodic_series.index - check_index)
 
             # Find the index in standard_series with the minimum time difference
             nearest_index = np.argmin(time_diff)
 
             nearest_periodic_indices.append(nearest_index)
 
         return nearest_periodic_indices
 
-    nearest_check_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, raw_check_series["Water Temperature Check"]
-    )
+    nearest_htp_indices = find_nearest_periodic_indices(standard_data, htp_check)
 
-    nearest_prov_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, prov_wq
-    )
+    nearest_pwq_indices = find_nearest_periodic_indices(standard_data, pwq_check)
 
-    nearest_inspection_indices = find_nearest_periodic_indices(
-        hilltop_standard_series, inspections
-    )
+    nearest_srv_indices = find_nearest_periodic_indices(standard_data, srv_check)
 
-    edited_blocks = change_blocks(raw_standard_series, hilltop_standard_series)
+    edited_blocks = change_blocks(standard_data["Raw"], standard_data["Value"])
 
     first_change = True
     for change_start, change_end in edited_blocks:
         fig_subplots.add_vrect(
             x0=change_start,
             x1=change_end,
             showlegend=first_change,
-            fillcolor="blue",
+            fillcolor="teal",
             opacity=0.25,
             line_width=0,
             name="Changes",
             row=1,
             col=1,
         )
         first_change = False
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=raw_check_series["Water Temperature Check"].index,
-            y=raw_check_series["Water Temperature Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_check_indices].to_numpy(),
+            x=htp_check["Value"].index,
+            y=htp_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_htp_indices].to_numpy(),
             mode="markers",
             name="Check data",
-            marker=dict(color="darkturquoise", size=10, symbol="circle"),
+            marker=dict(color="darkcyan", size=10, symbol="circle"),
             showlegend=False,
         ),
         row=2,
         col=1,
     )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_check_indices].index,
-            y=raw_check_series["Water Temperature Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_check_indices].to_numpy(),
+            x=standard_data["Value"].iloc[nearest_htp_indices].index,
+            y=htp_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_htp_indices].to_numpy(),
             mode="markers",
             name="Check Align",
-            marker=dict(color="darkturquoise", size=10, symbol="circle"),
+            marker=dict(color="darkcyan", size=10, symbol="circle"),
             showlegend=False,
             opacity=0.5,
             hoverinfo="skip",
         ),
         row=2,
         col=1,
     )
     arrow_annotations = []
     for stand, check in zip(
-        hilltop_standard_series.iloc[nearest_check_indices].items(),
-        raw_check_series["Water Temperature Check"].items(),
+        standard_data["Value"].iloc[nearest_htp_indices].items(),
+        htp_check["Value"].items(),
         strict=True,
     ):
         # If the timestamps are not the same
         if stand[0] != check[0] and not pd.isna(check[1]):
             arrow_annotations.append(
                 dict(
                     ax=check[0],
@@ -485,188 +475,188 @@
                     x=stand[0],
                     y=check[1] - stand[1],
                     axref="x2",
                     ayref="y2",
                     xref="x2",
                     yref="y2",
                     arrowhead=2,
-                    arrowcolor="darkturquoise",
+                    arrowcolor="darkcyan",
                     showarrow=True,
                     opacity=0.5,
                     standoff=6,
                 )
             )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=prov_wq.index,
-            y=prov_wq["Temp Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_prov_indices].to_numpy(),
+            x=pwq_check.index,
+            y=pwq_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_pwq_indices].to_numpy(),
             mode="markers",
             name="ProvWQ Check",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+            marker=dict(color="darkgray", size=10, symbol="square-open"),
             showlegend=False,
         ),
         row=2,
         col=1,
     )
     fig_subplots.add_trace(
         go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_prov_indices].index,
-            y=prov_wq["Temp Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_prov_indices].to_numpy(),
+            x=standard_data["Value"].iloc[nearest_pwq_indices].index,
+            y=pwq_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_pwq_indices].to_numpy(),
             mode="markers",
             name="ProvWQ Align",
-            marker=dict(color="darkslategray", size=10, symbol="square-open"),
+            marker=dict(color="darkgray", size=10, symbol="square-open"),
             showlegend=False,
             opacity=0.5,
             hoverinfo="skip",
         ),
         row=2,
         col=1,
     )
     for stand, prov in zip(
-        hilltop_standard_series.iloc[nearest_prov_indices].items(),
-        prov_wq.iterrows(),
+        standard_data["Value"].iloc[nearest_pwq_indices].items(),
+        pwq_check.iterrows(),
         strict=True,
     ):
         # If the timestamps are not the same
-        if stand[0] != prov[0] and not pd.isna(prov[1]["Temp Check"]):
+        if stand[0] != prov[0] and not pd.isna(prov[1]["Value"]):
             arrow_annotations.append(
                 dict(
                     ax=prov[0],
-                    ay=prov[1]["Temp Check"] - stand[1],
+                    ay=prov[1]["Value"] - stand[1],
                     x=stand[0],
-                    y=prov[1]["Temp Check"] - stand[1],
+                    y=prov[1]["Value"] - stand[1],
                     axref="x2",
                     ayref="y2",
                     xref="x2",
                     yref="y2",
                     arrowhead=2,
-                    arrowcolor="darkslategray",
+                    arrowcolor="darkgray",
                     showarrow=True,
                     opacity=0.5,
                     standoff=6,
                 )
             )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy(),
+            x=srv_check.index,
+            y=srv_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_srv_indices].to_numpy(),
             mode="markers",
             name="S123 Check",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+            marker=dict(color="darkgray", size=10, symbol="circle-open-dot"),
             showlegend=False,
         ),
         row=2,
         col=1,
     )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
-            y=inspections["Temp Check"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy(),
+            x=standard_data["Value"].iloc[nearest_srv_indices].index,
+            y=srv_check["Value"].to_numpy()
+            - standard_data["Value"].iloc[nearest_srv_indices].to_numpy(),
             mode="markers",
             name="S123 Check Aligned",
-            marker=dict(color="darkslategray", size=10, symbol="circle-open-dot"),
+            marker=dict(color="darkgray", size=10, symbol="circle-open-dot"),
             showlegend=False,
             opacity=0.5,
             hoverinfo="skip",
         ),
         row=2,
         col=1,
     )
 
     for stand, insp in zip(
-        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
-        inspections.iterrows(),
+        standard_data["Value"].iloc[nearest_srv_indices].items(),
+        srv_check.iterrows(),
         strict=True,
     ):
         # If the timestamps are not the same
-        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
+        if stand[0] != insp[0] and not pd.isna(insp[1]["Logger"]):
             arrow_annotations.append(
                 dict(
                     ax=insp[0],
-                    ay=insp[1]["Temp Check"] - stand[1],
+                    ay=insp[1]["Value"] - stand[1],
                     x=stand[0],
-                    y=insp[1]["Temp Check"] - stand[1],
+                    y=insp[1]["Value"] - stand[1],
                     axref="x2",
                     ayref="y2",
                     xref="x2",
                     yref="y2",
                     arrowhead=2,
-                    arrowcolor="darkslategray",
+                    arrowcolor="darkgray",
                     showarrow=True,
                     opacity=0.5,
                     standoff=6,
                 )
             )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=inspections.index,
-            y=inspections["Temp Logger"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy(),
+            x=srv_check.index,
+            y=srv_check["Logger"].to_numpy()
+            - standard_data["Value"].iloc[nearest_srv_indices].to_numpy(),
             mode="markers",
             name="S123 Logger",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+            marker=dict(color="darkgray", size=10, symbol="x-thin-open"),
             showlegend=False,
         ),
         row=2,
         col=1,
     )
 
     fig_subplots.add_trace(
         go.Scatter(
-            x=hilltop_standard_series.iloc[nearest_inspection_indices].index,
-            y=inspections["Temp Logger"].to_numpy()
-            - hilltop_standard_series.iloc[nearest_inspection_indices].to_numpy(),
+            x=standard_data["Value"].iloc[nearest_srv_indices].index,
+            y=srv_check["Logger"].to_numpy()
+            - standard_data["Value"].iloc[nearest_srv_indices].to_numpy(),
             mode="markers",
             name="S123 Logger Aligned",
-            marker=dict(color="darkslategray", size=10, symbol="x-thin-open"),
+            marker=dict(color="darkgray", size=10, symbol="x-thin-open"),
             showlegend=False,
             opacity=0.5,
             hoverinfo="skip",
         ),
         row=2,
         col=1,
     )
 
     for stand, insp in zip(
-        hilltop_standard_series.iloc[nearest_inspection_indices].items(),
-        inspections.iterrows(),
+        standard_data["Value"].iloc[nearest_srv_indices].items(),
+        srv_check.iterrows(),
         strict=True,
     ):
         # If the timestamps are not the same
-        if stand[0] != insp[0] and not pd.isna(insp[1]["Temp Logger"]):
+        if stand[0] != insp[0] and not pd.isna(insp[1]["Logger"]):
             arrow_annotations.append(
                 dict(
                     ax=insp[0],
-                    ay=insp[1]["Temp Logger"] - stand[1],
+                    ay=insp[1]["Logger"] - stand[1],
                     x=stand[0],
-                    y=insp[1]["Temp Logger"] - stand[1],
+                    y=insp[1]["Logger"] - stand[1],
                     axref="x2",
                     ayref="y2",
                     xref="x2",
                     yref="y2",
                     arrowhead=2,
-                    arrowcolor="darkslategray",
+                    arrowcolor="darkgray",
                     showarrow=True,
                     opacity=0.5,
                     standoff=6,
                 )
             )
 
     fig_subplots.update_layout(annotations=arrow_annotations)
 
-    qc400 = 1.2
-    qc500 = 0.8
+    qc400 = processor.quality_code_evaluator.qc_500_limit
+    qc500 = processor.quality_code_evaluator.qc_600_limit
 
     fig_subplots.add_hline(
         y=qc400,
         line=dict(color="#ffa500", width=1, dash="dash"),
         name="QC400",
         row=2,
         col=1,
```

### Comparing `hydrobot-0.5.2/hydrobot/processor.py` & `hydrobot-0.6.0/hydrobot/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Processor class."""
 
 import re
 import warnings
-from functools import wraps
+from datetime import datetime
 
 import numpy as np
 import pandas as pd
 from annalist.annalist import Annalist
 from annalist.decorators import ClassLogger
 from hilltoppy import Hilltop
 
@@ -18,69 +18,14 @@
     filters,
     plotter,
     utils,
 )
 
 annalizer = Annalist()
 
-DEFAULTS = {
-    "high_clip": 20000,
-    "low_clip": 0,
-    "delta": 1000,
-    "span": 10,
-    "gap_limit": 12,
-    "max_qc": np.NaN,
-}
-
-
-def stale_warning(method):
-    """Decorate dangerous functions.
-
-    Check whether the data is stale, and warn user if so.
-    Warning will then take input form user to determine whether to proceed or cancel.
-    Cancelling will return a null function, which returns None with no side effects no
-    matter what the input
-
-    Currently broken
-
-    Parameters
-    ----------
-    method : function
-        A function that might have some problems if the parameters have been changed
-        but the data hasn't been updated
-
-    Returns
-    -------
-    function
-        null function if warning is heeded, otherwise
-    """
-
-    @wraps(method)
-    def _impl(self, *method_args, **method_kwargs):
-        if self._stale:
-            warnings.warn(
-                "Warning: a key parameter of the data has changed but the data itself "
-                "has not been reloaded.",
-                stacklevel=2,
-            )
-            while True:
-                user_input = input("Do you want to continue? y/n: ")
-
-                if user_input.lower() in ["y", "ye", "yes"]:
-                    print("Continuing")
-                    return method(self, *method_args, **method_kwargs)
-                if user_input.lower() in ["n", "no"]:
-                    print("Function cancelled")
-                    return lambda *x: None
-                print("Type y or n (or yes or no, or even ye, all ye who enter here)")
-        else:
-            return method(self, *method_args, **method_kwargs)
-
-    return _impl
-
 
 class Processor:
     """A class used to process data from a Hilltop server."""
 
     @ClassLogger  # type: ignore
     def __init__(
         self,
@@ -90,14 +35,16 @@
         standard_measurement_name: str,
         frequency: str,
         from_date: str | None = None,
         to_date: str | None = None,
         check_hts: str | None = None,
         check_measurement_name: str | None = None,
         defaults: dict | None = None,
+        interval_dict: dict | None = None,
+        constant_check_shift: float = 0,
         **kwargs,
     ):
         """
         Constructs all the necessary attributes for the Processor object.
 
         Parameters
         ----------
@@ -117,40 +64,43 @@
             The end date of the data (default is None).
         check_hts : str, optional
             The Hilltop service to be checked (default is None).
         check_measurement : str, optional
             The measurement to be checked (default is None).
         defaults : dict, optional
             The default settings (default is None).
+        interval_dict : dict, optional
+            Determines how data with old checks is downgraded
         kwargs : dict
             Additional keyword arguments.
         """
-        if defaults is None:
-            self._defaults = DEFAULTS
-        else:
-            self._defaults = defaults
-        if check_hts is None:
-            check_hts = standard_hts
+        self._defaults = defaults
         if check_measurement_name is None:
             check_measurement_name = standard_measurement_name
 
         standard_hilltop = Hilltop(base_url, standard_hts, **kwargs)
-        check_hilltop = Hilltop(base_url, check_hts, **kwargs)
-        if (
-            site in standard_hilltop.available_sites
-            and site in check_hilltop.available_sites
-        ):
+        if check_hts is not None:
+            check_hilltop = Hilltop(base_url, check_hts, **kwargs)
+            if site in check_hilltop.available_sites:
+                self._site = site
+            else:
+                raise ValueError(
+                    f"Site '{site}' not found for both base_url and hts combos."
+                    f"Available sites in check_hts are: "
+                    f"{[s for s in check_hilltop.available_sites]}"
+                )
+        else:
+            check_hilltop = None
+        if site in standard_hilltop.available_sites:
             self._site = site
         else:
             raise ValueError(
                 f"Site '{site}' not found for both base_url and hts combos."
                 f"Available sites in standard_hts are: "
                 f"{[s for s in standard_hilltop.available_sites]}"
-                f"Available sites in check_hts are: "
-                f"{[s for s in check_hilltop.available_sites]}"
             )
 
         # standard
         available_standard_measurements = standard_hilltop.get_measurement_list(site)
         self._standard_measurement_name = standard_measurement_name
         matches = re.search(r"([^\[\n]+)(\[(.+)\])?", standard_measurement_name)
 
@@ -166,197 +116,210 @@
                 f"Standard measurement name '{standard_measurement_name}' not found at"
                 f" site '{site}'. "
                 "Available measurements are "
                 f"{list(available_standard_measurements.MeasurementName)}"
             )
 
         # check
-        available_check_measurements = check_hilltop.get_measurement_list(site)
         self._check_measurement_name = check_measurement_name
         matches = re.search(r"([^\[\n]+)(\[(.+)\])?", check_measurement_name)
+        if check_hilltop is not None:
+            available_check_measurements = check_hilltop.get_measurement_list(site)
+            if self._check_measurement_name not in list(
+                available_check_measurements.MeasurementName
+            ):
+                raise ValueError(
+                    f"Check measurement name '{self._check_measurement_name}' "
+                    f"not found at site '{site}'. "
+                    "Available measurements are "
+                    f"{list(available_check_measurements.MeasurementName)}"
+                )
 
         if matches is not None:
             self.check_item_name = matches.groups()[0].strip(" ")
             self.check_data_source_name = matches.groups()[2]
             if self.check_data_source_name is None:
                 self.check_data_source_name = self.check_item_name
-        if self._check_measurement_name not in list(
-            available_check_measurements.MeasurementName
-        ):
-            raise ValueError(
-                f"Check measurement name '{self._check_measurement_name}' "
-                f"not found at site '{site}'. "
-                "Available measurements are "
-                f"{list(available_check_measurements.MeasurementName)}"
-            )
 
+        self.standard_item_info = {
+            "ItemName": self.standard_item_name,
+            "ItemFormat": "F",
+            "Divisor": 1,
+            "Units": "",
+            "Format": "###.##",
+        }
+
+        self.check_item_info = {
+            "ItemName": self.check_item_name,
+            "ItemFormat": "F",
+            "Divisor": 1,
+            "Units": "",
+            "Format": "$$$",
+        }
         self._base_url = base_url
         self._standard_hts = standard_hts
         self._check_hts = check_hts
         self._frequency = frequency
         self._from_date = from_date
         self._to_date = to_date
         self._quality_code_evaluator = data_sources.get_qc_evaluator(
             standard_measurement_name
         )
-        self._stale = True
-        self._no_data = True
-        self._standard_series = pd.Series({})
-        self._check_series = pd.Series({})
-        self._quality_series = pd.Series({})
+        self._quality_code_evaluator.constant_check_shift = constant_check_shift
+
+        if interval_dict is None:
+            self._interval_dict = {}
+        else:
+            self._interval_dict = interval_dict
+
+        self._standard_data = pd.DataFrame(
+            columns=[
+                "Time",
+                "Raw",
+                "Value",
+                "Changes",
+                "Remove",
+            ]
+        ).set_index("Time")
+        self._check_data = pd.DataFrame(
+            columns=[
+                "Time",
+                "Raw",
+                "Value",
+                "Changes",
+                "Recorder Time",
+                "Comment",
+                "Source",
+                "QC",
+            ]
+        ).set_index("Time")
+        self._quality_data = pd.DataFrame(
+            columns=[
+                "Time",
+                "Raw",
+                "Value",
+                "Code",
+                "Details",
+            ]
+        ).set_index("Time")
 
-        self.raw_standard_series = pd.Series({})
         self.raw_standard_blob = None
         self.raw_standard_xml = None
-        self.raw_quality_series = pd.Series({})
+
         self.raw_quality_blob = None
         self.raw_quality_xml = None
-        self.raw_check_data = pd.DataFrame({})
+
         self.raw_check_blob = None
         self.raw_check_xml = None
 
+        get_check = self._check_hts is not None
+
         # Load data for the first time
-        self.import_data(from_date=self.from_date, to_date=self.to_date)
+        self.import_data(
+            from_date=self.from_date, to_date=self.to_date, check=get_check
+        )
 
     @property
     def standard_measurement_name(self):  # type: ignore
         """str: The site to be processed."""
         return self._standard_measurement_name
 
     @property
     def site(self):  # type: ignore
-        """
-        str: The site to be processed.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The site to be processed."""
         return self._site
 
     @property
     def from_date(self):  # type: ignore
-        """
-        str: The start date of the data.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The start date of the data."""
         return self._from_date
 
     @property
     def to_date(self):  # type: ignore
-        """
-        str: The end date of the data.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The end date of the data."""
         return self._to_date
 
     @property
     def frequency(self):  # type: ignore
-        """
-        str: The frequency of the data.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The frequency of the data."""
         return self._frequency
 
     @property
     def base_url(self):  # type: ignore
-        """
-        str: The base URL of the Hilltop server.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The base URL of the Hilltop server."""
         return self._base_url
 
     @property
     def standard_hts(self):  # type: ignore
-        """
-        str: The standard Hilltop service.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The standard Hilltop service."""
         return self._standard_hts
 
     @property
     def check_hts(self):  # type: ignore
-        """
-        str: The Hilltop service to be checked.
-
-        Setting this property will mark the data as stale.
-        """
+        """str: The Hilltop service to be checked."""
         return self._check_hts
 
     @property
     def quality_code_evaluator(self):  # type: ignore
         """Measurement property."""
         return self._quality_code_evaluator
 
     @ClassLogger
     @quality_code_evaluator.setter
     def quality_code_evaluator(self, value):
         self._quality_code_evaluator = value
-        self._stale = True
 
     @property
     def defaults(self):  # type: ignore
-        """
-        dict: The default settings.
-
-        Setting this property will mark the data as stale.
-        """
+        """dict: The default settings."""
         return self._defaults
 
     @property  # type: ignore
-    def standard_series(self) -> pd.Series:  # type: ignore
+    def standard_data(self) -> pd.DataFrame:  # type: ignore
         """pd.Series: The standard series data."""
-        return self._standard_series
+        return self._standard_data
 
     @ClassLogger  # type: ignore
-    @standard_series.setter
-    def standard_series(self, value):
-        self._standard_series = value
+    @standard_data.setter
+    def standard_data(self, value):
+        self._standard_data = value
 
-    @property
-    def check_series(self):  # type: ignore
+    @property  # type: ignore
+    def check_data(self) -> pd.DataFrame:  # type: ignore
         """pd.Series: The series containing check data."""
-        return self._check_series
+        return self._check_data
 
     @ClassLogger  # type: ignore
-    @check_series.setter
-    def check_series(self, value):
-        self._check_series = value
+    @check_data.setter
+    def check_data(self, value):
+        self._check_data = value
 
-    @property
-    def quality_series(self):  # type: ignore
-        """
-        pd.Series: The quality series data.
-
-        Setting this property will mark the data as stale.
-        """
-        return self._quality_series
+    @property  # type: ignore
+    def quality_data(self) -> pd.DataFrame:  # type: ignore
+        """pd.Series: The quality series data."""
+        return self._quality_data
 
     @ClassLogger  # type: ignore
-    @quality_series.setter
-    def quality_series(self, value):
-        self._quality_series = value
-        self._stale = True
+    @quality_data.setter
+    def quality_data(self, value):
+        self._quality_data = value
 
     @ClassLogger
     def import_standard(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
     ):
         """
         Import standard data.
 
         Parameters
         ----------
         from_date : str or None, optional
-            The start date for data retrieval. If None, defaults to earliest available
+            The start date for data retrieval. If None, defaults to the earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
 
         Returns
         -------
@@ -402,98 +365,114 @@
             tstype="Standard",
         )
 
         blob_found = False
 
         date_format = "Calendar"
         data_source_list = []
+        raw_standard_data = pd.DataFrame({})
         if blob_list is None or len(blob_list) == 0:
             warnings.warn(
                 "No standard data found within specified date range.",
                 stacklevel=1,
             )
         else:
             for blob in blob_list:
                 data_source_list += [blob.data_source.name]
                 if (blob.data_source.name == self.standard_data_source_name) and (
                     blob.data_source.ts_type == "StdSeries"
                 ):
-                    self.raw_standard_series = blob.data.timeseries
+                    raw_standard_data = blob.data.timeseries
                     date_format = blob.data.date_format
-                    if self.raw_standard_series is not None:
+                    if raw_standard_data is not None:
                         # Found it. Now we extract it.
                         blob_found = True
                         self.raw_standard_blob = blob
                         self.raw_standard_xml = xml_tree
+                        self.standard_item_info[
+                            "ItemName"
+                        ] = blob.data_source.item_info[0].item_name
+                        self.standard_item_info[
+                            "ItemFormat"
+                        ] = blob.data_source.item_info[0].item_format
+                        self.standard_item_info["Divisor"] = blob.data_source.item_info[
+                            0
+                        ].divisor
+                        self.standard_item_info["Units"] = blob.data_source.item_info[
+                            0
+                        ].units
+                        self.standard_item_info["Format"] = blob.data_source.item_info[
+                            0
+                        ].format
             if not blob_found:
                 raise ValueError(
                     f"Standard Data Not Found under name "
                     f"{self._standard_measurement_name}. "
                     f"Available data sources are: {data_source_list}"
                 )
 
-            if not isinstance(self.raw_standard_series, pd.Series):
+            if not isinstance(raw_standard_data, pd.DataFrame):
                 raise TypeError(
-                    f"Expecting pd.Series for Standard data, but got {type(self.raw_standard_series)}"
-                    "from parser."
+                    "Expecting pd.DataFrame for Standard data, "
+                    f"but got {type(raw_standard_data)} from parser."
                 )
-            if not self.raw_standard_series.empty:
+            if not raw_standard_data.empty:
                 if date_format == "mowsecs":
-                    self.raw_standard_series.index = utils.mowsecs_to_datetime_index(
-                        self.raw_standard_series.index
+                    raw_standard_data.index = utils.mowsecs_to_datetime_index(
+                        raw_standard_data.index
                     )
                 else:
-                    self.raw_standard_series.index = pd.to_datetime(
-                        self.raw_standard_series.index
-                    )
-                self.raw_standard_series = self.raw_standard_series.asfreq(
+                    raw_standard_data.index = pd.to_datetime(raw_standard_data.index)
+                raw_standard_data = raw_standard_data.asfreq(
                     self._frequency, fill_value=np.NaN
                 )
             if self.raw_standard_blob is not None:
-                fmt = self.raw_standard_blob.data_source.item_info[0].item_format
-                div = self.raw_standard_blob.data_source.item_info[0].divisor
+                fmt = self.standard_item_info["ItemFormat"]
+                div = self.standard_item_info["Divisor"]
             else:
                 warnings.warn(
                     "Could not extract standard data format from data source. "
                     "Defaulting to float format.",
                     stacklevel=1,
                 )
                 fmt = "F"
                 div = 1
             if div is None or div == "None":
                 div = 1
             if fmt == "I":
-                self.raw_standard_series = self.raw_standard_series.astype(int) / int(
-                    div
-                )
+                raw_standard_data.iloc[:, 0] = raw_standard_data.iloc[:, 0].astype(
+                    int
+                ) / int(div)
             elif fmt == "F":
-                self.raw_standard_series = self.raw_standard_series.astype(
+                raw_standard_data.iloc[:, 0] = raw_standard_data.iloc[:, 0].astype(
                     np.float32
                 ) / float(div)
             elif fmt == "D":  # Not sure if this would ever really happen, but...
-                self.raw_standard_series = utils.mowsecs_to_datetime_index(
-                    self.raw_standard_series
+                raw_standard_data.iloc[:, 0] = utils.mowsecs_to_datetime_index(
+                    raw_standard_data.iloc[:, 0]
                 )
             else:
                 raise ValueError(f"Unknown Format Spec: {fmt}")
-            self.standard_series = self.raw_standard_series
+
+            self.standard_data["Raw"] = raw_standard_data.iloc[:, 0]
+            self.standard_data["Value"] = self.standard_data["Raw"]
 
     @ClassLogger
     def import_quality(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
     ):
         """
         Import quality data.
 
         Parameters
         ----------
         from_date : str or None, optional
-            The start date for data retrieval. If None, defaults to earliest available
+            The start date for data retrieval. If None, defaults to the earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
 
         Returns
         -------
@@ -533,14 +512,15 @@
             self._standard_measurement_name,
             from_date,
             to_date,
             tstype="Quality",
         )
 
         blob_found = False
+        raw_quality_data = pd.DataFrame({})
 
         if blob_list is None or len(blob_list) == 0:
             warnings.warn(
                 "No Quality data available for the range specified.",
                 stacklevel=1,
             )
         else:
@@ -548,58 +528,59 @@
             for blob in blob_list:
                 if (blob.data_source.name == self.standard_data_source_name) and (
                     blob.data_source.ts_type == "StdQualSeries"
                 ):
                     # Found it. Now we extract it.
                     blob_found = True
 
-                    self.raw_quality_series = blob.data.timeseries
+                    raw_quality_data = blob.data.timeseries
                     date_format = blob.data.date_format
-                    if self.raw_quality_series is not None:
+                    if raw_quality_data is not None:
                         # Found it. Now we extract it.
                         blob_found = True
                         self.raw_quality_blob = blob
                         self.raw_quality_xml = xml_tree
             if not blob_found:
                 warnings.warn(
                     "No Quality data found in the server response.",
                     stacklevel=2,
                 )
 
-            if not isinstance(self.raw_quality_series, pd.Series):
+            if not isinstance(raw_quality_data, pd.DataFrame):
                 raise TypeError(
-                    f"Expecting pd.Series for Quality data, but got "
-                    f"{type(self.raw_quality_series)} from parser."
+                    f"Expecting pd.DataFrame for Quality data, but got "
+                    f"{type(raw_quality_data)} from parser."
                 )
-            if not self.raw_quality_series.empty:
+            if not raw_quality_data.empty:
                 if date_format == "mowsecs":
-                    self.raw_quality_series.index = utils.mowsecs_to_datetime_index(
-                        self.raw_quality_series.index
+                    raw_quality_data.index = utils.mowsecs_to_datetime_index(
+                        raw_quality_data.index
                     )
                 else:
-                    self.raw_quality_series.index = pd.to_datetime(
-                        self.raw_quality_series.index
-                    )
+                    raw_quality_data.index = pd.to_datetime(raw_quality_data.index)
+            raw_quality_data.iloc[:, 0] = raw_quality_data.iloc[:, 0].astype(
+                int, errors="ignore"
+            )
 
-            self.quality_series = self.raw_quality_series.astype(int)
-            self._quality_series.name = self._standard_measurement_name + " [Quality]"
+            self.quality_data["Raw"] = raw_quality_data.iloc[:, 0]
+            self.quality_data["Value"] = self.quality_data["Raw"]
 
     @ClassLogger
     def import_check(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
     ):
         """
         Import Check data.
 
         Parameters
         ----------
         from_date : str or None, optional
-            The start date for data retrieval. If None, defaults to earliest available
+            The start date for data retrieval. If None, defaults to the earliest available
             data.
         to_date : str or None, optional
             The end date for data retrieval. If None, defaults to latest available
             data.
 
         Returns
         -------
@@ -646,14 +627,15 @@
         date_format = "Calendar"
         if blob_list is None or len(blob_list) == 0:
             warnings.warn(
                 "No Check data available for the range specified.",
                 stacklevel=2,
             )
         else:
+            raw_check_data = pd.DataFrame({})
             data_source_options = []
             for blob in blob_list:
                 data_source_options += [blob.data_source.name]
                 if (blob.data_source.name == self.check_data_source_name) and (
                     blob.data_source.ts_type == "CheckSeries"
                 ):
                     # Found it. Now we extract it.
@@ -662,67 +644,78 @@
                     date_format = blob.data.date_format
 
                     # This could be a pd.Series
                     import_data = blob.data.timeseries
                     if import_data is not None:
                         self.raw_check_blob = blob
                         self.raw_check_xml = xml_tree
-                        self.raw_check_data = import_data
+                        raw_check_data = import_data
+                        self.check_item_info["ItemName"] = blob.data_source.item_info[
+                            0
+                        ].item_name
+                        self.check_item_info["ItemFormat"] = blob.data_source.item_info[
+                            0
+                        ].item_format
+                        self.check_item_info["Divisor"] = blob.data_source.item_info[
+                            0
+                        ].divisor
+                        self.check_item_info["Units"] = blob.data_source.item_info[
+                            0
+                        ].units
+                        self.check_item_info["Format"] = blob.data_source.item_info[
+                            0
+                        ].format
             if not blob_found:
                 warnings.warn(
                     f"Check data {self.check_data_source_name} not found in server "
                     f"response. Available options are {data_source_options}",
                     stacklevel=2,
                 )
 
-            if not isinstance(self.raw_check_data, pd.DataFrame):
+            if not isinstance(raw_check_data, pd.DataFrame):
                 raise TypeError(
-                    f"Expecting pd.DataFrame for Check data, but got {type(self.raw_check_data)}"
+                    f"Expecting pd.DataFrame for Check data, but got {type(raw_check_data)}"
                     "from parser."
                 )
-            if not self.raw_check_data.empty:
+            if not raw_check_data.empty:
                 if date_format == "mowsecs":
-                    self.raw_check_data.index = utils.mowsecs_to_datetime_index(
-                        self.raw_check_data.index
+                    raw_check_data.index = utils.mowsecs_to_datetime_index(
+                        raw_check_data.index
                     )
                 else:
-                    self.raw_check_data.index = pd.to_datetime(
-                        self.raw_check_data.index
-                    )
+                    raw_check_data.index = pd.to_datetime(raw_check_data.index)
 
-            if not self.raw_check_data.empty and self.raw_check_blob is not None:
+            if not raw_check_data.empty and self.raw_check_blob is not None:
                 # TODO: Maybe this should happen in the parser?
                 for i, item in enumerate(self.raw_check_blob.data_source.item_info):
                     fmt = item.item_format
                     div = item.divisor
-                    col = self.raw_check_data.iloc[:, i]
+                    col = raw_check_data.iloc[:, i]
                     if fmt == "I":
-                        self.raw_check_data.iloc[:, i] = col.astype(int) / int(div)
+                        raw_check_data.iloc[:, i] = col.astype(int) / int(div)
                     elif fmt == "F":
-                        self.raw_check_data.iloc[:, i] = col.astype(np.float32) / float(
-                            div
-                        )
+                        raw_check_data.iloc[:, i] = col.astype(np.float32) / float(div)
                     elif fmt == "D":
-                        if self.raw_check_data.iloc[:, i].dtype != pd.Timestamp:
+                        if raw_check_data.iloc[:, i].dtype != pd.Timestamp:
                             if date_format == "mowsecs":
-                                self.raw_check_data.iloc[
+                                raw_check_data.iloc[
                                     :, i
                                 ] = utils.mowsecs_to_datetime_index(col)
                             else:
-                                self.raw_check_data.iloc[:, i] = col.astype(
-                                    pd.Timestamp
-                                )
+                                raw_check_data.iloc[:, i] = col.astype(pd.Timestamp)
                     elif fmt == "S":
-                        self.raw_check_data.iloc[:, i] = col.astype(str)
+                        raw_check_data.iloc[:, i] = col.astype(str)
 
-            if not self.raw_check_data.empty:
-                self.check_series = self.raw_check_data[self.check_item_name]
-            else:
-                self.check_series = pd.Series({})
-            self._check_series.name = self._standard_measurement_name + " [Check]"
+            if not raw_check_data.empty:
+                self.check_data["Raw"] = raw_check_data[self.check_item_name]
+                self.check_data["Value"] = self.check_data["Raw"]
+                self.check_data["Recorder Time"] = raw_check_data["Recorder Time"]
+                self.check_data["Comment"] = raw_check_data["Comment"]
+                self.check_data["Source"] = "HTP"
+                self.check_data["QC"] = True
 
     def import_data(
         self,
         from_date: str | None = None,
         to_date: str | None = None,
         standard: bool = True,
         check: bool = True,
@@ -750,56 +743,40 @@
         parameters `_from_date` and `_to_date`. It updates the internal series data in
         the Processor instance for standard, check, and quality measurements
         separately.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
-        >>> processor.set_date_range("2022-01-01", "2022-12-31")
-        >>> processor.import_data(standard=True, check=True)
-        >>> processor.stale
+        >>> processor.import_data("2022-01-01", "2022-12-31",standard=True, check=True)
         False
         """
-        if (
-            self._standard_series is not None
-            and not self._standard_series.empty
-            and self._quality_series is not None
-            and not self._quality_series.empty
-            and self._check_series is not None
-            and not self._check_series.empty
-        ):
-            warnings.warn(
-                "When you reimport, you are overwriting your data. You will lose all"
-                "progess up to this point.",
-                stacklevel=1,
-            )
         if standard:
             self.import_standard(from_date, to_date)
         if quality:
             self.import_quality(from_date, to_date)
         if check:
             self.import_check(from_date, to_date)
-        self._stale = False
 
     @ClassLogger
     def add_standard(self, extra_standard):
         """
         Incorporate extra standard data into the standard series using utils.merge_series.
 
         Parameters
         ----------
         extra_standard
             extra standard data
 
         Returns
         -------
-        None, but adds data to self.standard_series
+        None, but adds data to self.standard_data
         """
-        combined = utils.merge_series(self.standard_series, extra_standard)
-        self.standard_series = combined
+        combined = utils.merge_series(self.standard_data["Value"], extra_standard)
+        self.standard_data["Value"] = combined
 
     @ClassLogger
     def add_check(self, extra_check):
         """
         Incorporate extra check data into the check series using utils.merge_series.
 
         Parameters
@@ -807,16 +784,16 @@
         extra_check
             extra check data
 
         Returns
         -------
         None, but adds data to self.check_series
         """
-        combined = utils.merge_series(self.check_series, extra_check)
-        self.check_series = combined
+        combined = utils.merge_series(self.check_data["Value"], extra_check)
+        self.check_data["Value"] = combined
 
     @ClassLogger
     def add_quality(self, extra_quality):
         """
         Incorporate extra quality data into the quality series using utils.merge_series.
 
         Parameters
@@ -824,23 +801,26 @@
         extra_quality
             extra quality data
 
         Returns
         -------
         None, but adds data to self.quality_series
         """
-        combined = utils.merge_series(self.quality_series, extra_quality)
-        self.quality_series = combined
+        combined = utils.merge_series(self.quality_data["Value"], extra_quality)
+        self.quality_data["Value"] = combined
 
-    # @stale_warning  # type: ignore
     @ClassLogger
     def gap_closer(self, gap_limit: int | None = None):
         """
         Close small gaps in the standard series.
 
+        DEPRECATED: The use of this method is discouraged as it completely removes rows
+        from the dataframes. The gap closing functionality has been moved to
+        data_exporter, where gaps are handled automatically before data export.
+
         Parameters
         ----------
         gap_limit : int or None, optional
             The maximum number of consecutive missing values to close, by default None.
             If None, the gap limit from the class defaults is used.
 
         Returns
@@ -853,37 +833,56 @@
         missing values with interpolated or backfilled values. The gap closure is
         performed using the evaluator.small_gap_closer function.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.gap_closer(gap_limit=5)
-        >>> processor.standard_series
+        >>> processor.standard_data["Value"]
         <updated standard series with closed gaps>
         """
+        warnings.warn(
+            "DEPRECATED: The use of gap_closer is discouraged as it completely "
+            "removes rows from the dataframes.",
+            stacklevel=1,
+        )
         if gap_limit is None:
-            gap_limit = int(self._defaults["gap_limit"])
-        self.standard_series = evaluator.small_gap_closer(
-            self._standard_series, gap_limit=gap_limit
+            if "gap_limit" not in self._defaults:
+                raise ValueError("gap_limit value required, no value found in defaults")
+            else:
+                gap_limit = int(self._defaults["gap_limit"])
+
+        gapless = evaluator.small_gap_closer(
+            self._standard_data["Value"].squeeze(), gap_limit=gap_limit
         )
+        self._standard_data = self._standard_data.loc[gapless.index]
 
-    # @stale_warning  # type: ignore
     @ClassLogger
     def quality_encoder(
-        self, gap_limit: int | None = None, max_qc: int | float | None = None
+        self,
+        gap_limit: int | None = None,
+        max_qc: int | float | None = None,
+        interval_dict: dict | None = None,
     ):
         """
         Encode quality information in the quality series.
 
         Parameters
         ----------
         gap_limit : int or None, optional
             The maximum number of consecutive missing values to consider as gaps, by
             default None.
             If None, the gap limit from the class defaults is used.
+        max_qc : numeric or None, optional
+            Maximum quality code possible at site
+            If None, the max qc from the class defaults is used.
+        interval_dict : dict or None, optional
+            Dictionary that dictates when to downgrade data with old checks
+            Takes pd.DateOffset:quality_code pairs
+            If None, the interval_dict from the class defaults is used.
 
         Returns
         -------
         None
 
         Notes
         -----
@@ -892,31 +891,81 @@
         the evaluator.quality_encoder function to determine the quality flags for the
         data.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.quality_encoder(gap_limit=5)
-        >>> processor.quality_series
+        >>> processor.quality_data["Value"]
         <updated quality series with encoded quality flags>
         """
         if gap_limit is None:
-            gap_limit = int(self._defaults["gap_limit"])
+            if "gap_limit" not in self._defaults:
+                raise ValueError("gap_limit value required, no value found in defaults")
+            else:
+                gap_limit = int(self._defaults["gap_limit"])
         if max_qc is None:
             max_qc = self._defaults["max_qc"] if "max_qc" in self._defaults else np.NaN
-        self.quality_series = evaluator.quality_encoder(
-            self._standard_series,
-            self._check_series,
+
+        if interval_dict is None:
+            interval_dict = self._interval_dict
+
+        qc_checks = self.check_data[self.check_data["QC"]]
+
+        chk_frame = evaluator.check_data_quality_code(
+            self.standard_data["Value"],
+            qc_checks["Value"],
             self._quality_code_evaluator,
+        )
+        self._apply_quality(chk_frame, replace=True)
+
+        oov_frame = evaluator.bulk_downgrade_out_of_validation(
+            self.quality_data, qc_checks["Value"], self._interval_dict
+        )
+        self._apply_quality(oov_frame)
+
+        msg_frame = evaluator.missing_data_quality_code(
+            self.standard_data["Value"],
+            self.quality_data,
             gap_limit=gap_limit,
-            max_qc=max_qc,
         )
+        self._apply_quality(msg_frame)
+
+        lim_frame = evaluator.max_qc_limiter(self.quality_data, max_qc)
+        self._apply_quality(lim_frame)
+
+    def _apply_quality(
+        self,
+        changed_data,
+        replace=False,
+    ):
+        if replace:
+            self.quality_data = changed_data
+        else:
+            # Step 1: Merge the dataframes using an outer join
+            merged_df = self.quality_data.merge(
+                changed_data,
+                how="outer",
+                left_index=True,
+                right_index=True,
+                suffixes=("_old", "_new"),
+            )
+
+            # Step 2: Replace NaN values in df1 with corresponding values from df2
+            merged_df["Value"] = merged_df["Value_old"].fillna(merged_df["Value_new"])
+            merged_df["Code"] = merged_df["Code_old"].fillna(merged_df["Code_new"])
+            merged_df["Details"] = merged_df["Details_old"].fillna(
+                merged_df["Details_new"]
+            )
+
+            # Step 3: Combine the two dataframes, prioritizing non-null values from df2
+            self.quality_data = merged_df[["Value", "Code", "Details"]].combine_first(
+                self.quality_data
+            )
 
-    # @stale_warning  # type: ignore
-    @ClassLogger
     def clip(self, low_clip: float | None = None, high_clip: float | None = None):
         """
         Clip data within specified low and high values.
 
         Parameters
         ----------
         low_clip : float or None, optional
@@ -936,27 +985,58 @@
         specified low and high values. It uses the filters.clip function for the actual
         clipping process.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.clip(low_clip=0, high_clip=100)
-        >>> processor.standard_series
+        >>> processor.standard_data["Value"]
         <clipped standard series within the specified range>
-        >>> processor.check_series
+        >>> processor.check_data["Value"]
         <clipped check series within the specified range>
         """
         if low_clip is None:
-            low_clip = float(self._defaults["low_clip"])
+            low_clip = (
+                float(self._defaults["low_clip"])
+                if "low_clip" in self._defaults
+                else np.NaN
+            )
         if high_clip is None:
-            high_clip = float(self._defaults["high_clip"])
+            high_clip = (
+                float(self._defaults["high_clip"])
+                if "high_clip" in self._defaults
+                else np.NaN
+            )
 
-        self.standard_series = filters.clip(self._standard_series, low_clip, high_clip)
+        clipped = filters.clip(
+            self._standard_data["Value"].squeeze(), low_clip, high_clip
+        )
+
+        self._standard_data = self._apply_changes(
+            self._standard_data, clipped, "CLP", mark_remove=True
+        )
+
+    @staticmethod
+    def _apply_changes(
+        dataframe,
+        changed_values,
+        change_code,
+        mark_remove=False,
+    ):
+        both_none_mask = pd.isna(dataframe["Value"]) & pd.isna(changed_values)
+
+        # Create a mask for cases where values are different excluding both being None-like
+        diffs_mask = (dataframe["Value"] != changed_values) & ~(both_none_mask)
+
+        if mark_remove:
+            dataframe.loc[diffs_mask, "Remove"] = mark_remove
+        dataframe.loc[diffs_mask, "Changes"] = change_code
+        dataframe["Value"] = changed_values
+        return dataframe
 
-    # @stale_warning  # type: ignore
     @ClassLogger
     def remove_outliers(self, span: int | None = None, delta: float | None = None):
         """
         Remove outliers from the data.
 
         Parameters
         ----------
@@ -977,33 +1057,36 @@
         span and delta values. It utilizes the filters.remove_outliers function for
         the actual outlier removal process.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.remove_outliers(span=10, delta=2.0)
-        >>> processor.standard_series
+        >>> processor.standard_data["Value"]
         <standard series with outliers removed>
         """
         if span is None:
-            span = int(self._defaults["span"])
+            if "span" not in self._defaults:
+                raise ValueError("span value required, no value found in defaults")
+            else:
+                span = int(self._defaults["span"])
         if delta is None:
-            delta = float(self._defaults["delta"])
+            if "delta" not in self._defaults:
+                raise ValueError("delta value required, no value found in defaults")
+            else:
+                delta = float(self._defaults["delta"])
 
-        if isinstance(self._standard_series, pd.Series):
-            self.standard_series = filters.remove_outliers(
-                self._standard_series, span, delta
-            )
-        else:
-            raise TypeError(
-                "Standard Series should be pd.Series, "
-                f"found {type(self._standard_series)}."
-            )
+        rm_outliers = filters.remove_outliers(
+            self._standard_data["Value"].squeeze(), span, delta
+        )
+
+        self._standard_data = self._apply_changes(
+            self._standard_data, rm_outliers, "OUT", mark_remove=True
+        )
 
-    # @stale_warning  # type: ignore
     @ClassLogger
     def remove_spikes(
         self,
         low_clip: float | None = None,
         high_clip: float | None = None,
         span: int | None = None,
         delta: float | None = None,
@@ -1036,55 +1119,127 @@
         parameters. It utilizes the filters.remove_spikes function for the actual
         spike removal process.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.remove_spikes(low_clip=10, high_clip=20, span=5, delta=2.0)
-        >>> processor.standard_series
+        >>> processor.standard_data["Value"]
         <standard series with spikes removed>
         """
         if low_clip is None:
-            low_clip = float(self._defaults["low_clip"])
+            low_clip = (
+                float(self._defaults["low_clip"])
+                if "low_clip" in self._defaults
+                else np.NaN
+            )
         if high_clip is None:
-            high_clip = float(self._defaults["high_clip"])
+            high_clip = (
+                float(self._defaults["high_clip"])
+                if "low_clip" in self._defaults
+                else np.NaN
+            )
         if span is None:
-            span = int(self._defaults["span"])
+            if "span" not in self._defaults:
+                raise ValueError("span value required, no value found in defaults")
+            else:
+                span = int(self._defaults["span"])
         if delta is None:
-            delta = float(self._defaults["delta"])
+            if "delta" not in self._defaults:
+                raise ValueError("delta value required, no value found in defaults")
+            else:
+                delta = float(self._defaults["delta"])
 
-        if isinstance(self._standard_series, pd.Series):
-            self.standard_series = filters.remove_spikes(
-                self._standard_series, span, low_clip, high_clip, delta
-            )
-        else:
-            raise TypeError(
-                "Standard Series should be pd.Series,"
-                f"found {type(self._standard_series)}"
-            )
+        rm_spikes = filters.remove_spikes(
+            self._standard_data["Value"].squeeze(),
+            span,
+            low_clip,
+            high_clip,
+            delta,
+        )
+
+        self._standard_data = self._apply_changes(
+            self._standard_data, rm_spikes, "SPK", mark_remove=True
+        )
 
     @ClassLogger
     def remove_flatlined_values(self, span: int = 3):
         """Remove repeated values in std series a la flatline_value_remover()."""
-        self.standard_series = filters.flatline_value_remover(
-            self._standard_series, span=span
+        rm_fln = filters.flatline_value_remover(self._standard_data["Value"], span=span)
+
+        self._standard_data = self._apply_changes(
+            self._standard_data, rm_fln, "FLN", mark_remove=True
+        )
+
+    @ClassLogger
+    def remove_range(
+        self,
+        from_date,
+        to_date,
+    ):
+        """
+        Mark a range in standard_data for removal.
+
+        Parameters
+        ----------
+        from_date : str
+            The start date of the range to delete.
+        to_date : str
+            The end date of the range to delete.
+
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        This method deletes a specified range of data from the selected time series
+        types. The range is defined by the `from_date` and `to_date` parameters.
+
+        Examples
+        --------
+        >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
+        >>> processor.remove_range(from_date="2022-01-01", to_date="2022-12-31", \
+                tstype_standard=True)
+        >>> processor.standard_data
+        <standard series with specified range deleted>
+        >>> processor.remove_range(from_date="2022-01-01", to_date="2022-12-31", \
+                tstype_check=True)
+        >>> processor.check_data
+        <check series with specified range deleted>
+        """
+        rm_range = filters.remove_range(
+            self._standard_data["Value"],
+            from_date,
+            to_date,
+            insert_gaps="all",
+        )
+        self.standard_data = self._apply_changes(
+            self._standard_data, rm_range, "MAN", mark_remove=True
         )
 
     @ClassLogger
     def delete_range(
         self,
         from_date,
         to_date,
         tstype_standard=True,
         tstype_check=False,
         tstype_quality=False,
+        gap_limit=None,
     ):
         """
         Delete a range of data from specified time series types.
 
+        DEPRECATED: The use of this method is discouraged as it completely removes rows
+        from the dataframes. User is encouraged to use 'remove_range' which marks rows
+        for removal, but retains the timestamp to be associated with the other values
+        in the row such as the raw value, reason for removal, etc.
+
         Parameters
         ----------
         from_date : str
             The start date of the range to delete.
         to_date : str
             The end date of the range to delete.
         tstype_standard : bool, optional
@@ -1104,32 +1259,58 @@
         types. The range is defined by the `from_date` and `to_date` parameters.
 
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.delete_range(from_date="2022-01-01", to_date="2022-12-31", \
                 tstype_standard=True)
-        >>> processor.standard_series
+        >>> processor.standard_data
         <standard series with specified range deleted>
         >>> processor.delete_range(from_date="2022-01-01", to_date="2022-12-31", \
                 tstype_check=True)
-        >>> processor.check_series
+        >>> processor.check_data
         <check series with specified range deleted>
         """
+        warnings.warn(
+            "DEPRECATED: The use of delete_range is discouraged as it completely "
+            "removes rows from the dataframes. User is encouraged to use "
+            "'remove_range' which marks rows for removal, but retains the timestamp "
+            "to be associated with the other values "
+            "in the row such as the raw value, reason for removal, etc.",
+            stacklevel=1,
+        )
+        if gap_limit is None:
+            if "gap_limit" not in self._defaults:
+                raise ValueError("gap_limit value required, no value found in defaults")
+            else:
+                gap_limit = self._defaults["gap_limit"]
+
         if tstype_standard:
-            self.standard_series = filters.remove_range(
-                self._standard_series, from_date, to_date
+            self.standard_data = filters.remove_range(
+                self._standard_data,
+                from_date,
+                to_date,
+                min_gap_length=gap_limit,
+                insert_gaps="start",
             )
         if tstype_check:
-            self.check_series = filters.remove_range(
-                self._check_series, from_date, to_date
+            self.check_data = filters.remove_range(
+                self._check_data,
+                from_date,
+                to_date,
+                min_gap_length=gap_limit,
+                insert_gaps="start",
             )
         if tstype_quality:
-            self.quality_series = filters.remove_range(
-                self._quality_series, from_date, to_date
+            self.quality_data = filters.remove_range(
+                self._quality_data,
+                from_date,
+                to_date,
+                min_gap_length=gap_limit,
+                insert_gaps="start",
             )
 
     @ClassLogger
     def insert_missing_nans(self):
         """
         Set the data to the correct frequency, filled with NaNs as appropriate.
 
@@ -1150,24 +1331,24 @@
         Examples
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.insert_missing_nans()
         >>> processor.standard_series
         <standard series with missing values filled with NaNs>
         """
-        self.standard_series = self._standard_series.asfreq(self._frequency)
+        self.standard_data = self._standard_data.asfreq(self._frequency)
 
     @ClassLogger
     def data_exporter(
         self,
         file_location,
         ftype="xml",
         standard: bool = True,
         quality: bool = True,
-        check: bool = False,
+        check: bool = True,
         trimmed=True,
     ):
         """
         Export data to CSV file.
 
         Parameters
         ----------
@@ -1200,41 +1381,48 @@
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.data_exporter("output.xml", trimmed=True)
         >>> # Check the generated XML file at 'output.xml'
         """
         export_selections = [standard, quality, check]
         if trimmed:
-            std_series = filters.trim_series(
-                self._standard_series,
-                self._check_series,
+            std_data = filters.trim_series(
+                self._standard_data["Value"],
+                self._check_data["Value"],
             )
         else:
-            std_series = self._standard_series
+            std_data = self._standard_data
 
         if ftype == "csv":
-            all_series = [
-                self._standard_series,
-                self._quality_series,
-                self._check_series,
+            all_data = [
+                self._standard_data["Value"],
+                self._quality_data["Value"],
+                self._check_data["Value"],
             ]
+            columns = ["Standard", "Quality", "Check"]
+
+            for data, col in zip(all_data, columns, strict=True):
+                data.name = col
+
             export_list = [
-                i for (i, v) in zip(all_series, export_selections, strict=True) if v
+                i for (i, v) in zip(all_data, export_selections, strict=True) if v
             ]
             data_sources.series_export_to_csv(file_location, series=export_list)
         elif ftype == "hilltop_csv":
             data_sources.hilltop_export(
                 file_location,
                 self._site,
                 self._quality_code_evaluator.name,
-                std_series,
-                self._check_series,
-                self._quality_series,
+                std_data,
+                self._check_data["Value"],
+                self._quality_data["Value"],
             )
         elif ftype == "xml":
+            if self.check_data.empty:
+                check = False
             blob_list = self.to_xml_data_structure(
                 standard=standard, quality=quality, check=check
             )
             data_structure.write_hilltop_xml(blob_list, file_location)
         else:
             raise ValueError("Invalid ftype (filetype)")
 
@@ -1256,38 +1444,38 @@
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.import_data()
         >>> processor.diagnosis()
         >>> # View diagnostic information about the data.
         """
         evaluator.diagnose_data(
-            self._standard_series,
-            self._check_series,
-            self._quality_series,
+            self._standard_data["Value"],
+            self._check_data["Value"],
+            self._quality_data["Value"],
             self._frequency,
         )
 
     def plot_qc_series(self, check=False, show=True):
         """Implement qc_plotter()."""
         fig = plotter.qc_plotter_plotly(
-            self._standard_series,
-            (self._check_series if check else None),
-            self._quality_series,
+            self._standard_data["Value"],
+            (self._check_data["Value"] if check else None),
+            self._quality_data["Value"],
             self._frequency,
             show=show,
         )
         return fig
 
     def plot_comparison_qc_series(self, show=True):
         """Implement comparison_qc_plotter()."""
         fig = plotter.comparison_qc_plotter_plotly(
-            self._standard_series,
-            self.raw_standard_series,
-            self._check_series,
-            self._quality_series,
+            self._standard_data["Value"],
+            self._standard_data["Raw"],
+            self._check_data["Value"],
+            self._quality_data["Value"],
             self._frequency,
             show=show,
         )
         return fig
 
     def plot_gaps(self, span=None, show=True):
         """
@@ -1315,17 +1503,17 @@
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.import_data()
         >>> processor.plot_gaps(span=10, show=True)
         >>> # Display a plot showing gaps in the standard series.
         """
         if span is None:
-            plotter.gap_plotter(self._standard_series, show=show)
+            plotter.gap_plotter(self._standard_data["Value"], show=show)
         else:
-            plotter.gap_plotter(self._standard_series, span, show=show)
+            plotter.gap_plotter(self._standard_data["Value"], span, show=show)
 
     def plot_checks(self, span=None, show=True):
         """
         Plot checks against the standard series data.
 
         Parameters
         ----------
@@ -1349,18 +1537,25 @@
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.import_data()
         >>> processor.plot_checks(span=10, show=True)
         >>> # Display a plot comparing checks to the standard series.
         """
         if span is None:
-            plotter.check_plotter(self._standard_series, self._check_series, show=show)
+            plotter.check_plotter(
+                self._standard_data["Value"],
+                self._check_data["Value"],
+                show=show,
+            )
         else:
             plotter.check_plotter(
-                self._standard_series, self._check_series, span, show=show
+                self._standard_data["Value"],
+                self._check_data["Value"],
+                span,
+                show=show,
             )
 
     def to_xml_data_structure(self, standard=True, quality=True, check=True):
         """
         Convert Processor object data to a list of XML data structures.
 
         Returns
@@ -1380,118 +1575,201 @@
         --------
         >>> processor = Processor(base_url="https://hilltop-server.com", site="Site1")
         >>> processor.import_data()
         >>> xml_data_list = processor.to_xml_data_structure()
         >>> # Convert Processor data to a list of XML data structures.
         """
         data_blob_list = []
-        selections = [standard, quality, check]
-        dtypes = ["standard", "quality", "check"]
-        blobs = [
-            self.raw_standard_blob,
-            self.raw_quality_blob,
-            self.raw_check_blob,
-        ]
-        selected_types = [dt for sel, dt in zip(selections, dtypes, strict=True) if sel]
-        selected_blobs = [
-            blob for sel, blob in zip(selections, blobs, strict=True) if sel
-        ]
 
-        for dtype, raw_blob in zip(selected_types, selected_blobs, strict=True):
-            if raw_blob is None:
-                raise ValueError(
-                    f"Can't reconstruct the {dtype} data structure without having an xml import"
-                    " to mimic."
-                )
-            if (
-                hasattr(raw_blob, "data_source")
-                and raw_blob.data_source is not None
-                and hasattr(raw_blob.data_source, "item_info")
-                and (raw_blob.data_source.item_info) is not None
-            ):
-                item_info_list = []
-                for i, info in enumerate(raw_blob.data_source.item_info):
-                    item_info = data_structure.ItemInfo(
-                        item_number=i,
-                        item_name=info.item_name,
-                        item_format=info.item_format,
-                        divisor=info.divisor,
-                        units=info.units,
-                        format=info.format,
+        if standard:
+            standard_item_info = data_structure.ItemInfo(
+                item_number=1,
+                item_name=self.standard_item_info["ItemName"],
+                item_format=self.standard_item_info["ItemFormat"],
+                divisor=self.standard_item_info["Divisor"],
+                units=self.standard_item_info["Units"],
+                format=self.standard_item_info["Format"],
+            )
+            standard_data_source = data_structure.DataSource(
+                name=self.standard_data_source_name,
+                num_items=1,
+                ts_type="StdSeries",
+                data_type="SimpleTimeSeries",
+                interpolation="Instant",
+                item_format="1",
+                item_info=[standard_item_info],
+            )
+            formatted_std_timeseries = self.standard_data["Value"].astype(str)
+            if standard_item_info.item_format == "F":
+                pattern = re.compile(r"#+\.?(#*)")
+                match = pattern.match(standard_item_info.format)
+                float_format = "{:.1f}"
+                if match:
+                    group = match.group(1)
+                    dp = len(group)
+                    float_format = "{:." + str(dp) + "f}"
+                    formatted_std_timeseries = (
+                        self.standard_data["Value"]
+                        .astype(np.float64)
+                        .map(lambda x, f=float_format: f.format(x))
                     )
-                    item_info_list += [item_info]
+
+            actual_nan_timeseries = formatted_std_timeseries.replace("nan", np.nan)
+
+            # TODO: Handle gaps
+            if "gap_limit" not in self._defaults:
+                pass
             else:
-                item_info_list = []
+                standard_timeseries = evaluator.small_gap_closer(
+                    actual_nan_timeseries,
+                    gap_limit=self._defaults["gap_limit"],
+                )
 
-            data_source = data_structure.DataSource(
-                name=self._standard_measurement_name,
-                num_items=raw_blob.data_source.num_items,
-                ts_type=raw_blob.data_source.ts_type,
-                data_type=raw_blob.data_source.data_type,
-                interpolation=raw_blob.data_source.interpolation,
-                item_format=raw_blob.data_source.item_format,
-                item_info=raw_blob.data_source.item_info,
+            standard_data = data_structure.Data(
+                date_format="Calendar",
+                num_items=3,
+                timeseries=standard_timeseries.to_frame(),
             )
 
-            if dtype == "standard":
-                if isinstance(self._standard_series, pd.Series):
-                    timeseries = self._standard_series
-                else:
-                    raise TypeError(
-                        "Standard Series should be pd.Series, "
-                        f"found {type(self._standard_series)}"
-                    )
+            standard_data_blob = data_structure.DataSourceBlob(
+                site_name=self.site,
+                data_source=standard_data_source,
+                data=standard_data,
+            )
+            data_blob_list += [standard_data_blob]
 
-            elif dtype == "quality":
-                if isinstance(self._quality_series, pd.Series):
-                    timeseries = self._quality_series
-                else:
-                    raise TypeError(
-                        "Quality Series should be pd.Series, "
-                        f"found {type(self._quality_series)}"
-                    )
-            elif dtype == "check":
-                if isinstance(self._check_series, pd.Series):
-                    timeseries = self.raw_check_data
-                    timeseries[self.check_item_name] = self._check_series
-                else:
-                    raise TypeError(
-                        "Check Data should be pd.Series, "
-                        f"found {type(self._check_series)}"
-                    )
-            else:
-                raise ValueError("No data found for export.")
-            if (
-                hasattr(raw_blob.data_source, "item_info")
-                and raw_blob.data_source.item_info is not None
-            ):
-                for i, info in enumerate(raw_blob.data_source.item_info):
-                    if info.item_format == "F":
-                        pattern = re.compile(r"#+\.?(#*)")
-                        match = pattern.match(info.format)
-                        float_format = "{:.1f}"
-                        if match:
-                            group = match.group(1)
-                            dp = len(group)
-                            float_format = "{:." + str(dp) + "f}"
-                        if isinstance(timeseries, pd.DataFrame):
-                            timeseries.iloc[:, i] = timeseries.iloc[:, i].map(
-                                lambda x, f=float_format: f.format(x)
-                            )
-                        elif isinstance(timeseries, pd.Series):
-                            timeseries = timeseries.map(
-                                lambda x, f=float_format: f.format(x)
-                            )
-            data = data_structure.Data(
-                date_format=raw_blob.data.date_format,
-                num_items=raw_blob.data.num_items,
-                timeseries=timeseries,
-            )
-
-            data_blob = data_structure.DataSourceBlob(
-                site_name=raw_blob.site_name,
-                data_source=data_source,
-                data=data,
+        if check:
+            check_item_info = data_structure.ItemInfo(
+                item_number=1,
+                item_name=self.check_item_info["ItemName"],
+                item_format=self.check_item_info["ItemFormat"],
+                divisor=self.check_item_info["Divisor"],
+                units=self.check_item_info["Units"],
+                format=self.check_item_info["Format"],
+            )
+            recorder_time_item_info = data_structure.ItemInfo(
+                item_number=2,
+                item_name="Recorder Time",
+                item_format="D",
+                divisor="1",
+                units="",
+                format="###",
+            )
+            comment_item_info = data_structure.ItemInfo(
+                item_number=3,
+                item_name="Comment",
+                item_format="F",
+                divisor="1",
+                units="",
+                format="###",
+            )
+
+            check_data_source = data_structure.DataSource(
+                name=self.check_data_source_name,
+                num_items=3,
+                ts_type="CheckSeries",
+                data_type="SimpleTimeSeries",
+                interpolation="Discrete",
+                item_format="45",
+                item_info=[
+                    check_item_info,
+                    recorder_time_item_info,
+                    comment_item_info,
+                ],
+            )
+
+            if check_item_info.item_format == "F":
+                pattern = re.compile(r"#+\.?(#*)")
+                match = pattern.match(check_item_info.format)
+                float_format = "{:.1f}"
+                if match:
+                    group = match.group(1)
+                    dp = len(group)
+                    float_format = "{:." + str(dp) + "f}"
+                    self.check_data.loc[:, "Value"] = self.check_data.loc[
+                        :, "Value"
+                    ].map(lambda x, f=float_format: f.format(x))
+
+            check_data = data_structure.Data(
+                date_format="Calendar",
+                num_items=3,
+                timeseries=self.check_data[["Value", "Recorder Time", "Comment"]],
+            )
+
+            check_data_blob = data_structure.DataSourceBlob(
+                site_name=self.site,
+                data_source=check_data_source,
+                data=check_data,
             )
+            data_blob_list += [check_data_blob]
 
-            data_blob_list += [data_blob]
+        if quality:
+            quality_data_source = data_structure.DataSource(
+                name=self.standard_data_source_name,
+                num_items=1,
+                ts_type="StdQualSeries",
+                data_type="SimpleTimeSeries",
+                interpolation="Event",
+                item_format="0",
+            )
+
+            quality_data = data_structure.Data(
+                date_format="Calendar",
+                num_items=3,
+                timeseries=self.quality_data["Value"].to_frame(),
+            )
+
+            quality_data_blob = data_structure.DataSourceBlob(
+                site_name=self.site,
+                data_source=quality_data_source,
+                data=quality_data,
+            )
+            data_blob_list += [quality_data_blob]
         return data_blob_list
+
+
+def hydrobot_config_yaml_init(config_path):
+    """
+    Initialises a Processor class given a config file.
+
+    Parameters
+    ----------
+    config_path : string
+        Path to config.yaml.
+
+    Returns
+    -------
+    Processor, Annalist
+    """
+    processing_parameters = data_acquisition.config_yaml_import(config_path)
+
+    ###################################################################################
+    # Setting up logging with Annalist
+    ###################################################################################
+
+    ann = Annalist()
+    ann.configure(
+        logfile=processing_parameters["logfile"],
+        analyst_name=processing_parameters["analyst_name"],
+        stream_format_str=processing_parameters["format"]["stream"],
+        file_format_str=processing_parameters["format"]["file"],
+    )
+
+    ###################################################################################
+    # Creating a Hydrobot Processor object which contains the data to be processed
+    ###################################################################################
+    now = datetime.now()
+    data = Processor(
+        processing_parameters["base_url"],
+        processing_parameters["site"],
+        processing_parameters["standard_hts_filename"],
+        processing_parameters["standard_measurement_name"],
+        processing_parameters.get("frequency", None),
+        processing_parameters["from_date"],
+        processing_parameters.get("to_date", now.strftime("%d-%m-%Y %H:%M:%S")),
+        processing_parameters.get("check_hts_filename", None),
+        processing_parameters.get("check_measurement_name", None),
+        processing_parameters["defaults"],
+        processing_parameters["inspection_expiry"],
+        constant_check_shift=processing_parameters["constant_check_shift"],
+    )
+    return data, ann
```

### Comparing `hydrobot-0.5.2/hydrobot/utils.py` & `hydrobot-0.6.0/hydrobot/utils.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/hydrobot.egg-info/PKG-INFO` & `hydrobot-0.6.0/hydrobot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydrobot
-Version: 0.5.2
+Version: 0.6.0
 Summary: A suite of processing tools for Hilltop hydrological data.
 Author-email: Nic Mostert <nicolas.mostert@horizons.govt.nz>, Sam Irvine <sam.irvine@horizons.govt.nz>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/HorizonsRC/hydrobot
 Project-URL: Issues, https://github.com/HorizonsRC/hydrobot/issues
 Project-URL: Documentation, https://hydrobot.readthedocs.io
 Project-URL: Package, https://pypi.org/project/hydrobot
@@ -19,14 +19,16 @@
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: hilltop-py>=2.3.1
 Requires-Dist: data-annalist>=0.4.1
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: defusedxml>=0.7.1
 Requires-Dist: plotly>=5.20.0
+Requires-Dist: streamlit>=1.33.0
+Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: test
 Requires-Dist: pytest>=7.4.2; extra == "test"
 Requires-Dist: pytest-cov>=4.1.0; extra == "test"
 Requires-Dist: pytest-dependency>=0.5.2; extra == "test"
 Requires-Dist: pytest-mock>=3.12.0; extra == "test"
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
@@ -80,27 +82,27 @@
   * Visualizing check points from various sources.
 
 Usage (Alpha)
 -------------
 
 The Alpha release of Hydrobot supports a "hybrid" workflow. This means that some external tools are still required to do a full processing. Importantly, the hybrid workflow relies on some R scripts to obtain check data from sources other than Hilltop. Further processing using Hilltop manager is also supported.
 
-NOTE: Hydrobot 0.5.2 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
+NOTE: Hydrobot 0.6.0 supports only Water Temperature processing at the moment, but more measurements will be supported in patches as the processing progresses.
 
 Initial Setup (Repeat for each release)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 #. Install a Python 3.11 interpreter. Note that 3.12 is not supported just yet.
-#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.5.2". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
+#. In your favourite shell, create a new virtual environment using this python interpreter and name it "hydrobot0.6.0". It's important that this is stored somewhere locally. I suggest creating a folder for virtual environments in your home folder::
 
-    python -m venv path/to/venv/hydrobot0.5.2/
+    python -m venv path/to/venv/hydrobot0.6.0/
 
 #. Activate this virtual environment. In powershell this should be something like::
 
-    ./path/to/venv/hydrobot0.5.2/Scripts/Activate.ps1
+    ./path/to/venv/hydrobot0.6.0/Scripts/Activate.ps1
 
 #. If you're sure your venv is active (ensure with `which python` and confirm that you're using the interpreter in your venv folder), install the latest version of Hydrobot using pip::
 
     pip install hydrobot
 
 #. Record which version of dependencies you have installed. The following pip freeze records which dependencies are
 installed by the hydrobot install process for if auditing/reprocessing is required later::
@@ -115,17 +117,17 @@
 Processing Steps
 ^^^^^^^^^^^^^^^^
 
 #. Open Logsheet Loader. Fill it as normal, and note the start date of your processing period (i.e. end date of the previous period).
 #. Navigate to the data source and site folder, and create your processing folder.
 #. Copy all the processing files in this folder into your processing folder::
 
-    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.5.2_Files\
+    \\ares\Environmental Data Validation\Water Temperature\Documents\Hydrobot_0.6.0_Files\
 
-    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.5.2_Files/
+    //ares/Environmental\ Data\ Validation/Water\ Temperature/Documents/Hydrobot_0.6.0_Files/
 
 #. In your processing folder, open the `config.yaml` file and change the fields `site`, `from_date`, `to_date`, `analyst_name`. Feel free to mess with the other values once you get the hang of it. No one will die.
 
 #. Run the R script. I'm not an R guy so I'm not sure how to do this other than to open it in R studio, highlighting all the code, and hitting `Ctrl+Enter`. This should create a bunch of `.csv` files containing the check data from various sources. This is a good reasource for perusal during processing, but will be imbibed by hydrobot to for QC encoding.
 
 #. Make sure your virtual environment is set up and active. Ensure with `which python` and confirm that your python interpreter is running from your venv folder.
```

### Comparing `hydrobot-0.5.2/hydrobot.egg-info/SOURCES.txt` & `hydrobot-0.6.0/hydrobot.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,19 @@
 hydrobot.egg-info/requires.txt
 hydrobot.egg-info/top_level.txt
 hydrobot/config/QualityCodeEvaluator_QC_config.csv
 hydrobot/config/TwoLevelQualityCodeEvaluator_QC_config.csv
 prototypes/Class_script.py
 prototypes/site_list_reader.py
 prototypes/site_parameters.json
+prototypes/example_script/.gitignore
+prototypes/example_script/40X_XXX_WaterTemperature.accdb
+prototypes/example_script/40X_XXX_WaterTemperature.hts
+prototypes/example_script/AP_CheckData.R
+prototypes/example_script/AP_config.yaml
 prototypes/example_script/WaterTemp_CheckData.R
 prototypes/example_script/config.yaml
 prototypes/example_script/script.py
 prototypes/output_dump/.gitignore
 prototypes/py_scripts/atmospheric_spike_removal.py
 prototypes/py_scripts/example_plot_script.py
 prototypes/py_scripts/gap_finder.py
@@ -72,8 +77,10 @@
 tests/test_data_structure.py
 tests/test_evaluator.py
 tests/test_filters.py
 tests/test_processor.py
 tests/test_utils.py
 tests/test_web_integration.py
 tests/test_data/site_list_response.xml
-tests/test_data/xml_test_data_file.xml
+tests/test_data/xml_test_data_file.xml
+tests/test_data/xml_test_data_no_check.xml
+tests/test_data/xml_test_data_no_qual.xml
```

### Comparing `hydrobot-0.5.2/old_setup.py` & `hydrobot-0.6.0/old_setup.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/Class_script.py` & `hydrobot-0.6.0/prototypes/Class_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/example_script/WaterTemp_CheckData.R` & `hydrobot-0.6.0/prototypes/example_script/AP_CheckData.R`

 * *Files 15% similar despite different names*

```diff
@@ -1,236 +1,240 @@
-#########################################################################################
-#
-#  Task Name:       <- Pull Water Temp check data
-#
-#  Task Purpose:    <- This code pulls the Water Temp check and inspection data from both Survey123
-#                       and 'Provisional WaterQuality.hts' for a given site and start date
-#
-#  Task Outputs:    <- A csv of all Water Temp combined check and inspection data that is saved in
-#                       the current folder [was specified folder]
-#
-#  Notes:           <- Now reads site and dates from config.yaml in the same folder as this script,
-#                       and outputs to current folder
-#
-#  Created by:      <- Hannah Marley
-#  Created on:      <- 19/01/2022
-#
-#  Last updated:    <- Sam Irvine
-#  Last updated by: <- 02/04/2024
-#
-#
-#  Written in R version 4.1.1
-#
-########################################################################################
-
-
-
-# load required libraries
-library(RODBC); library(dplyr); library(DT);
-library(tidyverse); library(Hilltop); library(lubridate)
-library(yaml)
-
-rm(list = ls())
-# --------------------------------------------------------------------------------
-# --- Define site, start date, and folder file path to save inspection data to ---
-# --------------------------------------------------------------------------------
-config_yaml = yaml.load_file("./config.yaml")
-site = config_yaml$site
-startDate = as.Date(config_yaml$from_date)-1  # choose one day before your batch start date
-endDate = as.Date(config_yaml$to_date)+1  # choose one day after your batch end date
-folder_filepath = "./" # here
-
-# -----------------------------------------------------
-
-
-
-# --- Retrieve check & inspection data from Survey123 ---
-
-# Connect to Survey123
-ch <- odbcDriverConnect('driver={SQL Server};server=DBSurvey123Live.horizons.govt.nz;database=survey123;trusted_connection=true')
-
-
-# Get inspection info
-inspections_Survey123 <- sqlQuery(ch, paste0("SELECT Hydro_Inspection.id, Hydro_Inspection.arrival_time, Hydro_Inspection.sitename,
-                                             Hydro_Inspection.weather, Hydro_Inspection.notes,
-                                             Hydro_Inspection.departure_time, Hydro_Inspection.creator,
-                                             DO_Inspection.inspection_id, DO_Inspection.do_notes,
-                                             WaterLevel_Inspection.inspection_id, WaterLevel_Inspection.wl_notes,
-                                             WaterTemp_Inspection.inspection_id, WaterTemp_Inspection.inspection_time, WaterTemp_Inspection.wt_device,
-                                             WaterTemp_Inspection.handheld_temp, WaterTemp_Inspection.logger_temp
-                                             FROM [dbo].Hydro_Inspection
-                                             FULL JOIN [dbo].DO_Inspection ON DO_Inspection.inspection_id = Hydro_Inspection.id
-                                             FULL JOIN [dbo].WaterLevel_Inspection ON WaterLevel_Inspection.inspection_id = Hydro_Inspection.id
-                                             FULL JOIN [dbo].WaterTemp_Inspection ON WaterTemp_Inspection.inspection_id = Hydro_Inspection.id
-                                             WHERE Hydro_Inspection.sitename = '", site, "'
-                                             AND Hydro_Inspection.arrival_time >= '", startDate, "'
-                                             AND Hydro_Inspection.arrival_time <= '", endDate, "'"),
-                                  stringsAsFactors = F)
-
-
-close(ch)
-
-
-
-# Format data
-Inspections = inspections_Survey123 %>%
-  select(id, sitename, arrival_time, inspection_time, departure_time, creator, weather,
-         notes, wl_notes, wt_device, do_notes,
-         handheld_temp, logger_temp
-  ) %>%
-  # mutate(inspection_time = round_date(inspection_time, "15 minutes"),
-  mutate(Date = ifelse(!is.na(inspection_time),
-                       as.Date(as.character(inspection_time)),
-                               as.Date(as.character(arrival_time))),
-         # for some reason above line is displaying as numeric format, so need this next line to force to Date
-         Date = as.Date(Date),
-         Time = ifelse(!is.na(inspection_time), format(inspection_time, "%H:%M:%S"), format(arrival_time, "%H:%M:%S")))
-
-colnames(Inspections) = c("ID", "Site Name",
-                          "Arrival Time", "Inspection Time", "Departure Time",
-                          "InspectionStaff",
-                          "Weather", "Notes", "Water level notes", "MeterID", "DO Notes",
-                          "Temp Check", "Temp Logger",
-                          "Date", "Time")
-
-Inspections = Inspections %>%
-  select("ID", "Site Name", "Date", "Time", "Weather",
-         "Arrival Time", "Inspection Time", "Departure Time", "InspectionStaff",
-         "Notes", "Water level notes", "MeterID", "DO Notes",
-         "Temp Check", "Temp Logger") %>%
-  mutate(`Arrival Time` = as.character(`Arrival Time`),
-         `Inspection Time` = as.character(`Inspection Time`),
-         `Departure Time` = as.character(`Departure Time`)) %>%
-  unique(.)
-
-
-write.csv(Inspections, paste0(folder_filepath, "WaterTemp_Inspections.csv"), row.names = FALSE)
-
-
-
-# --- Retrieve check & inspection data from Provisional WQ ---
-
-# data source
-dat = HilltopData("//ares/Environmental Archive/Provisional WaterQuality.hts")
-meas = "Field Temperature (HRC) [Field Temperature (HRC)]"
-#(measurements = MeasurementList(dat, site))
-
-# Get the data from Hilltop
-sites = SiteList(dat)
-
-if (site %in% sites){
-  provisWQ_dat = GetData(dat, site, meas, startDate, "", WQParams = TRUE)
-  provisWQ_dat = fortify.zoo(provisWQ_dat, melt = FALSE)
-
-  # --- Join all data together and format ---
-
-  provisWQ_dat = provisWQ_dat %>%
-    # mutate(Index = round_date(Index, "15 minutes"),
-    mutate("Arrival Time" = as.character(Index),
-           Date = as.Date(Index),
-           Time = format(Index, "%H:%M:%S"),
-           ID = NA,
-           `Site Name` = site,
-           `Inspection Time` = NA,
-           `Departure Time` = NA,
-           `Water level notes` = NA,
-           `DO Notes` = NA,
-           `Temp Logger` = NA) %>%
-    rename("Temp Check" = "Field Temperature (HRC)",
-           "InspectionStaff" = "SampledBy",
-           "Notes" = "Comments") %>%
-    select("ID", "Site Name", "Date", "Time", "Weather",
-           "Arrival Time", "Inspection Time", "Departure Time", "InspectionStaff",
-           "Notes", "Water level notes", "MeterID", "DO Notes",
-           "Temp Check", "Temp Logger") %>%
-    #rbind(., Inspections) %>%
-    #select(-ID) %>%
-    arrange(desc(`Arrival Time`))
-  # --- save to csv ---
-  write.csv(provisWQ_dat, paste0(folder_filepath, "WaterTemp_ProvWQ.csv"), row.names = FALSE)
-  full_dat = provisWQ_dat %>%
-    rbind(., Inspections) %>%
-    select(-ID) %>%
-    arrange(desc(`Arrival Time`))
-} else {
-  full_dat = Inspections
-}
-
-# ------ Pull non-conformances for sites ------
-# Connect to survey123 sql table
-ch = odbcDriverConnect('driver={SQL Server};server=DBSurvey123Live.horizons.govt.nz;database=survey123;trusted_connection=true')
-
-NCR = sqlQuery(ch, paste0("SELECT Hydro_Inspection.id, Hydro_Inspection.sitename,
-                                             Non_Conformances.*
-                                             FROM [dbo].Non_Conformances
-                                             INNER JOIN Hydro_Inspection ON Non_Conformances.inspection_id = Hydro_Inspection.id
-                                             WHERE Hydro_Inspection.sitename = '", site, "'"),
-               stringsAsFactors = F)
-
-close(ch)
-
-
-# Connect to logsheets
-ch1 = odbcConnectAccess2007("//ares/HydrologySoftware/Catchment Data Tools/CDT4.accdb")
-
-NCRs = sqlQuery(ch1, paste0("SELECT NonConformance.*
-                                            FROM NonConformance
-                                            WHERE NonConformance.Sitename= '", site, "'"), stringsAsFactors = F)
-NCRs
-
-close(ch1)
-
-
-NCR_survey123 = NCR %>%
-  mutate(created_date = as.character(created_date),
-         edit_date = as.character(edit_date)) %>%
-  select(sitename, created_date, creator, edit_date, summary, missing_record, days_missing_record, corrective_action) %>%
-  rename("Sitename" = "sitename",
-         "Entrydate" = "created_date",
-         "Reportby" = "creator",
-         "ReportDate" = "edit_date",
-         "NC_Summary" = "summary",
-         "MissingRecord" = "missing_record",
-         "MissingRecord_Days" = "days_missing_record",
-         "CorrectiveAction" = "corrective_action")
-
-
-NCRs = NCRs %>%
-  mutate(Entrydate = as.character(Entrydate),
-         ReportDate = as.character(ReportDate)) %>%
-  select(Sitename, Entrydate, Reportby, ReportDate, NC_Summary, MissingRecord, MissingRecord_Days, CorrectiveAction)
-
-NCRs = NCRs %>%
-  rbind(., NCR_survey123) %>%
-  mutate(Date = as.Date(ReportDate)) %>%
-  arrange(Date) %>%
-  select(-Date) %>%
-  filter(as.Date(ReportDate) >= startDate,
-         as.Date(ReportDate) <= endDate) %>%
-  unique(.)
-
-write.csv(NCRs, paste0(folder_filepath, "WaterTemp_non-conformance_reports.csv"), row.names = FALSE)
-
-
-
-
-
-# ------ Keep just check data, format to fit Hilltop and save as csv ------
-
-check_data = full_dat %>%
-  select(Date, Time, `Temp Check`, `Arrival Time`, `Inspection Time`, Notes) %>%
-  filter(!is.na(`Temp Check`),
-         Date <= endDate) %>%
-  mutate(`Recorder Time` = ifelse(!is.na(`Inspection Time`), `Inspection Time`, `Arrival Time`)) %>%
-  distinct(Date, `Temp Check`, .keep_all = TRUE) %>%
-  rename("Water Temperature check" = "Temp Check",
-         "Comment" = "Notes") %>%
-  mutate(`Water Temperature check` = as.numeric(`Water Temperature check`)) %>%
-  select(Date, Time, `Water Temperature check`, `Recorder Time`, Comment) %>%
-  arrange(`Recorder Time`)
-
-
-write.csv(check_data, paste0(folder_filepath, "WaterTemp_check_data.csv"), row.names = FALSE)
-
-
-
-rm(list = ls())
+#########################################################################################
+#
+#  Task Name:       <- Pull Atmospheric Pressure check data
+#
+#  Task Purpose:    <- This code pulls the DO check and inspection data from both Survey123
+#                       and 'Provisional WaterQuality.hts' for a given site and start date
+#
+#  Task Outputs:    <- A csv of all DO combined check and inspection data that is saved in
+#                       the specified folder
+#
+#  Notes:           <-
+#
+#  Created by:      <- Hannah Marley
+#  Created on:      <- 02/12/2022
+#
+#  Last updated:    <- 05/03/2024
+#  Last updated by: <- Nic
+#
+#
+#  Written in R version 4.1.1
+#
+########################################################################################
+
+# Make sure the script is working in the right place
+setwd(dirname(rstudioapi::getActiveDocumentContext()$path))
+# setwd(getSrcDirectory(function(){})[1]) # might need to use this if it's run as a script
+
+# load required libraries
+library(RODBC); library(dplyr); library(DT)
+library(tidyverse); library(Hilltop); library(lubridate)
+library(yaml)
+
+# --------------------------------------------------------------------------------
+# --- Define site, start date, and folder file path to save inspection data to ---
+# --------------------------------------------------------------------------------
+config_yaml = yaml.load_file("./config.yaml")
+site = config_yaml$site
+
+startDate = as.Date(config_yaml$from_date)-1  # choose one day before your batch start date
+if (is.null(config_yaml$to_date)) {
+  config_yaml$to_date = format(Sys.time(), "%Y-%m-%d %H:%M:%S")
+}
+endDate = as.Date(config_yaml$to_date)+1  # choose one day after your batch end date
+folder_filepath = "./" # here
+
+# -----------------------------------------------------
+
+
+
+# --- Retrieve check & inspection data from Survey123 ---
+
+# Connect to Survey123
+ch <- odbcDriverConnect('driver={SQL Server};server=DBSurvey123Live.horizons.govt.nz;database=survey123;trusted_connection=true')
+
+
+# Get inspection info
+inspections_Survey123 <- sqlQuery(ch, paste0("SELECT Hydro_Inspection.id, Hydro_Inspection.arrival_time, Hydro_Inspection.sitename,
+                                             Hydro_Inspection.weather, Hydro_Inspection.notes,
+                                             Hydro_Inspection.departure_time, Hydro_Inspection.creator,
+                                             DO_Inspection.inspection_id, DO_Inspection.handheld_baro, DO_Inspection.logger_baro,
+                                             DO_Inspection.do_notes, DO_Inspection.inspection_id,
+                                             WaterLevel_Inspection.inspection_id,
+                                             WaterLevel_Inspection.wl_notes,
+                                             WaterTemp_Inspection.inspection_id, WaterTemp_Inspection.wt_device,
+                                             WaterTemp_Inspection.handheld_temp, WaterTemp_Inspection.logger_temp
+                                             FROM [dbo].Hydro_Inspection
+                                             FULL JOIN [dbo].DO_Inspection ON DO_Inspection.inspection_id = Hydro_Inspection.id
+                                             FULL JOIN [dbo].WaterLevel_Inspection ON WaterLevel_Inspection.inspection_id = Hydro_Inspection.id
+                                             FULL JOIN [dbo].WaterTemp_Inspection ON WaterTemp_Inspection.inspection_id = Hydro_Inspection.id
+                                             WHERE Hydro_Inspection.sitename = '", site, "'
+                                             AND Hydro_Inspection.arrival_time >= '", startDate, "'"),
+                                  stringsAsFactors = F)
+
+
+close(ch)
+
+
+
+# Format data
+Inspections = inspections_Survey123 %>%
+  select(id, sitename, arrival_time, departure_time, creator, weather,
+         notes, wl_notes, wt_device, do_notes,
+         handheld_baro, logger_baro
+  ) %>%
+  mutate(arrival_time = round_date(arrival_time, "15 minutes"),
+         Date = as.Date(as.character(arrival_time)),
+         Time = format(arrival_time, "%H:%M:%S"))
+
+colnames(Inspections) = c("ID", "Site Name", "Arrival Time", "Departure Time", "InspectionStaff",
+                          "Weather", "Notes", "Water level notes", "MeterID", "DO Notes",
+                          "Value", "Logger",
+                          "Date", "Time")
+
+Inspections = Inspections %>%
+  select("ID", "Site Name", "Date", "Time", "Weather",
+         "Arrival Time", "Departure Time", "InspectionStaff",
+         "Notes", "Water level notes", "MeterID", "DO Notes",
+         "Value", "Logger") %>%
+  mutate(`Arrival Time` = as.character(`Arrival Time`),
+         `Departure Time` = as.character(`Departure Time`)) %>%
+  unique(.)
+
+write.csv(Inspections, paste0(folder_filepath, "AP_Inspections.csv"), row.names = FALSE)
+
+
+
+# --- Retrieve check & inspection data from Provisional WQ ---
+
+# data source
+dat = HilltopData("//ares/Environmental Archive/Provisional WaterQuality.hts")
+meas = "Field Baro Pressure (HRC) [Field Baro Pressure (HRC)]"
+#(measurements = MeasurementList(dat, site))
+sites = SiteList(dat)
+
+if (site %in% sites){
+
+  # Get the data from Hilltop
+  provisWQ_dat = GetData(dat, site, meas, startDate, "", WQParams = TRUE)
+  provisWQ_dat = fortify.zoo(provisWQ_dat, melt = FALSE)
+
+  provisWQ_dat = provisWQ_dat %>%
+     mutate(Index = round_date(Index, "15 minutes"),
+            "Arrival Time" = as.character(Index),
+            Date = as.Date(Index),
+            Time = format(Index, "%H:%M:%S"),
+            ID = NA,
+            `Site Name` = site,
+            `Departure Time` = NA,
+            `Water level notes` = NA,
+            `DO Notes` = NA,
+            `Logger` = NA) %>%
+     rename("Value" = "Field Baro Pressure (HRC)",
+            "InspectionStaff" = "SampledBy",
+            "Notes" = "Comments") %>%
+     select(ID, `Site Name`, Date, Time, Weather, `Arrival Time`, `Departure Time`,
+            InspectionStaff, Notes, `Water level notes`, MeterID,
+            `DO Notes`, `Value`,
+            `Logger`) %>%
+  #   rbind(., Inspections) %>%
+  #   select(-ID) %>%
+     arrange(desc(`Arrival Time`))
+  # --- save to csv ---
+  write.csv(provisWQ_dat, paste0(folder_filepath, "AP_ProvWQ.csv"), row.names = FALSE)
+  full_dat = provisWQ_dat %>%
+    rbind(., Inspections) %>%
+    select(-ID) %>%
+    arrange(desc(`Arrival Time`))
+} else {
+ full_dat = Inspections
+}
+
+
+
+
+
+
+
+# ------ Pull non-conformances for sites ------
+
+# Connect to survey123 sql table
+ch = odbcDriverConnect('driver={SQL Server};server=sql3dev.horizons.govt.nz;database=survey123;trusted_connection=true')
+
+NCR = sqlQuery(ch, paste0("SELECT Hydro_Inspection.id, Hydro_Inspection.sitename,
+                                             Non_Conformances.*
+                                             FROM [dbo].Non_Conformances
+                                             INNER JOIN Hydro_Inspection ON Non_Conformances.inspection_id = Hydro_Inspection.id
+                                             WHERE Hydro_Inspection.sitename = '", site, "'"),
+               stringsAsFactors = F)
+
+close(ch)
+
+
+# Connect to logsheets
+ch1 = odbcConnectAccess2007("//ares/HydrologySoftware/Catchment Data Tools/CDT4.accdb")
+
+NCRs = sqlQuery(ch1, paste0("SELECT NonConformance.* FROM NonConformance WHERE NonConformance.Sitename= '", site, "'"),
+                stringsAsFactors = F)
+
+close(ch1)
+
+
+
+NCR_survey123 = NCR %>%
+  mutate(created_date = as.character(created_date),
+         edit_date = as.character(edit_date)) %>%
+  select(sitename, created_date, creator, edit_date, summary, missing_record, days_missing_record, corrective_action) %>%
+  rename("Sitename" = "sitename",
+         "Entrydate" = "created_date",
+         "Reportby" = "creator",
+         "ReportDate" = "edit_date",
+         "NC_Summary" = "summary",
+         "MissingRecord" = "missing_record",
+         "MissingRecord_Days" = "days_missing_record",
+         "CorrectiveAction" = "corrective_action")
+
+
+NCRs = NCRs %>%
+  mutate(Entrydate = as.character(Entrydate),
+         ReportDate = as.character(ReportDate)) %>%
+  select(Sitename, Entrydate, Reportby, ReportDate, NC_Summary, MissingRecord, MissingRecord_Days, CorrectiveAction)
+
+NCRs = NCRs %>%
+  rbind(., NCR_survey123) %>%
+  mutate(Date = as.Date(ReportDate)) %>%
+  arrange(Date) %>%
+  select(-Date) %>%
+  filter(as.Date(ReportDate) >= startDate,
+         as.Date(ReportDate) <= endDate)
+
+write.csv(NCRs, paste0(folder_filepath, "AP_non-conformance_reports.csv"), row.names = FALSE)
+
+
+
+
+
+# ------ Keep just check data, format to fit Hilltop and save as csv ------
+
+check_data = full_dat %>%
+  select(Date, Time, `Value`, `Arrival Time`, Notes) %>%
+  filter(!is.na(`Value`),
+         Date <= endDate) %>%
+  distinct(Date, `Value`, .keep_all = TRUE) %>%
+  dplyr::rename("Check Pressure" = "Value",
+         "Recorder Time" = "Arrival Time",
+        "Comment" = "Notes") %>%
+  mutate(`Check Pressure` = as.numeric(`Check Pressure`)) %>%
+  #select(Date, Time, `Check Pressure`, `Recorder Time`, Comment) %>%
+  arrange(`Recorder Time`)
+
+# Escape newlines
+check_data$Comment = gsub("\r?\n|\r", "---NEWLINE---",check_data$Comment)
+
+write.csv(check_data,
+          paste0(folder_filepath,
+                 paste0("AP_check_data_", gsub("-", "", Sys.Date()), ".csv")),
+          row.names = FALSE)
+
+
+
+rm(list = ls())
```

### Comparing `hydrobot-0.5.2/prototypes/example_script/config.yaml` & `hydrobot-0.6.0/prototypes/example_script/config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+#################################################################################
+# Hydrobot 0.6.0 Configuration File
+#################################################################################
+
 # Hilltop Server Configuration
 base_url: "http://hilltopdev.horizons.govt.nz/"
 standard_hts_filename: "RawLoggerNet.hts"
-check_hts_filename: "boo.hts"
+# check_hts_filename: "boo.hts"
 
 # Data Source Configuration
-site: "Manawatu at Foxton"
-standard_measurement_name: "Water Temperature"
-check_measurement_name: "Water Temperature Check [Water Temperature]"
+site: "Rangitikei at McKelvies"
+standard_measurement_name: "Atmospheric Pressure"
+check_measurement_name: "Check Pressure [Atmospheric Pressure Inspections]"
 frequency: "15min"
 
 # Processing Configuration
-from_date: "2021-12-21 11:15"
-to_date: "2024-04-02 10:00"
+from_date: "2023-04-13 11:30:00"
 defaults:
   delta: 5
   gap_limit: 12
-  high_clip: 35
-  low_clip: 0
+  high_clip: 1200
+  low_clip: 800
   max_qc: 600
   span: 10
 
 # Annalist Configuration
 analyst_name: Nic
 logfile: "hydrobot_logs.csv"
 format:
@@ -29,7 +32,15 @@
 
 # Survey123 SQL Configuration
 s123_sql_server: "DBSurvey123Live.horizons.govt.nz"
 s123_database: "survey123"
 s123_query_type: "WaterTemp"
 # s123_sql_driver: "SQL Server" # If on Windows
 s123_sql_driver: "/opt/microsoft/msodbcsql17/lib64/libmsodbcsql-17.10.so.5.1" # If on WSL
+
+inspection_expiry:
+    500:
+        months: 2
+    0:
+        months: 4
+
+constant_check_shift: 0
```

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/atmospheric_spike_removal.py` & `hydrobot-0.6.0/prototypes/py_scripts/atmospheric_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/example_plot_script.py` & `hydrobot-0.6.0/prototypes/py_scripts/example_plot_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/gap_finder.py` & `hydrobot-0.6.0/prototypes/py_scripts/gap_finder.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/new_ws_plot_with_check_data.py` & `hydrobot-0.6.0/prototypes/py_scripts/new_ws_plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/plot_with_check_data.py` & `hydrobot-0.6.0/prototypes/py_scripts/plot_with_check_data.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/process_script.py` & `hydrobot-0.6.0/prototypes/py_scripts/process_script.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/spike_removal_util.py` & `hydrobot-0.6.0/prototypes/py_scripts/spike_removal_util.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/stage_full_process.py` & `hydrobot-0.6.0/prototypes/py_scripts/stage_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/water_temp_full_process.py` & `hydrobot-0.6.0/prototypes/py_scripts/water_temp_full_process.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/py_scripts/water_temp_spike_removal.py` & `hydrobot-0.6.0/prototypes/py_scripts/water_temp_spike_removal.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/prototypes/site_list_reader.py` & `hydrobot-0.6.0/prototypes/site_list_reader.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/pyproject.toml` & `hydrobot-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hydrobot"
 description = "A suite of processing tools for Hilltop hydrological data."
-version = "0.5.2"
+version = "0.6.0"
 authors = [
     { name = "Nic Mostert", email = "nicolas.mostert@horizons.govt.nz" },
     { name = "Sam Irvine", email = "sam.irvine@horizons.govt.nz" }
 ]
 requires-python = "==3.11.*"
 dependencies = [
     "hilltop-py>=2.3.1",
     "data-annalist>=0.4.1",
     "matplotlib>=3.8.0",
     "defusedxml>=0.7.1",
-    "plotly>=5.20.0"
+    "plotly>=5.20.0",
+    "streamlit>=1.33.0",
+    "pyyaml>=6.0.1"
 ]
 classifiers=[
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.11",
@@ -96,15 +98,15 @@
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["S311", "S101", "F841"]
 "docs/*" = ["I001"]
 "prototypes" = ["D"]
 
 [tool.bumpversion]
-current_version = "0.5.2"
+current_version = "0.6.0"
 commit = true
 tag = true
 tag_name = "{new_version}"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "{current_version}"
@@ -115,7 +117,17 @@
 search = "__version__ = \"{current_version}\""
 replace = "__version__ = \"{new_version}\""
 
 [[tool.bumpversion.files]]
 filename = "README.rst"
 search = "{current_version}"
 replace = "{new_version}"
+
+[[tool.bumpversion.files]]
+filename = "prototypes/example_script/config.yaml"
+search = "{current_version}"
+replace = "{new_version}"
+
+[[tool.bumpversion.files]]
+filename = "prototypes/example_script/script.py"
+search = "{current_version}"
+replace = "{new_version}"
```

### Comparing `hydrobot-0.5.2/requirements_dev.txt` & `hydrobot-0.6.0/requirements_dev.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,136 +1,186 @@
 alabaster==0.7.13
+altair==5.3.0
+annotated-types==0.6.0
 appdirs==1.4.4
 argh==0.29.4
 asttokens==2.4.0
 attrs==23.1.0
 Babel==2.12.1
 backcall==0.2.0
+beautifulsoup4==4.12.3
 black==23.9.1
+blinker==1.7.0
+build==1.0.3
+bump-my-version==0.17.3
 bump2version==1.0.1
 cachetools==5.3.1
+cattrs==23.2.3
 certifi==2023.7.22
 cffi==1.15.1
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.2.0
 click==8.1.7
 colorama==0.4.6
 comm==0.1.4
 contourpy==1.1.1
 coverage==7.3.1
 cryptography==41.0.4
 cycler==0.12.1
-data-annalist==0.3.6
+dash==2.16.1
+dash-core-components==2.0.0
+dash-html-components==2.0.0
+dash-table==5.0.0
+data-annalist==0.4.3
 debugpy==1.8.0
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.7
+docformatter==1.7.5
 docutils==0.20.1
 entrypoints==0.3
 exceptiongroup==1.1.3
 executing==2.0.0
 filelock==3.12.4
 flake8==6.1.0
+Flask==3.0.2
 fonttools==4.43.1
+furo==2024.1.29
+gitdb==4.0.11
+GitPython==3.1.43
 hilltop-py==2.3.1
+-e git+https://github.com/HorizonsRC/hydrobot.git@7386b3048b162bfc5d6e4be5a0870ab992e04c3f#egg=hydrobot
 identify==2.5.30
 idna==3.4
 imagesize==1.4.1
 importlib-metadata==6.8.0
 iniconfig==2.0.0
 ipykernel==6.25.2
 ipympl==0.9.3
 ipython==8.16.1
 ipython-genutils==0.2.0
 ipywidgets==8.1.1
+itsdangerous==2.1.2
 jaraco.classes==3.3.0
 jedi==0.19.1
 jeepney==0.8.0
 Jinja2==3.1.2
+jsonschema==4.21.1
+jsonschema-specifications==2023.12.1
 jupyter_client==8.4.0
 jupyter_core==5.4.0
 jupyterlab-widgets==3.0.9
 keyring==24.2.0
 kiwisolver==1.4.5
+lsprotocol==2023.0.0
 markdown-it-py==3.0.0
 MarkupSafe==2.1.3
 matplotlib==3.8.0
 matplotlib-inline==0.1.6
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.1.0
 mypy-extensions==1.0.0
 nest-asyncio==1.5.8
 nh3==0.2.14
 nodeenv==1.8.0
 numpy==1.26.0
 orjson==3.9.7
 packaging==23.1
-pandas==2.1.1
+pandas==2.2.1
 parso==0.8.3
 pathspec==0.11.2
 pathtools==0.1.2
 patsy==0.5.3
 pexpect==4.8.0
 pickleshare==0.7.5
 Pillow==10.0.1
 pkginfo==1.9.6
 platformdirs==3.10.0
 plotly==5.20.0
+plotly-resampler==0.9.2
 pluggy==1.3.0
 pre-commit==3.5.0
-prompt-toolkit==3.0.39
+prompt-toolkit==3.0.36
+protobuf==4.25.3
 psutil==5.9.5
 ptyprocess==0.7.0
 pure-eval==0.2.2
 py==1.11.0
+pyarrow==15.0.2
 pycodestyle==2.11.0
 pycparser==2.21
-pydantic==1.10.13
+pydantic==1.10.15
+pydantic-settings==2.1.0
+pydantic_core==2.16.3
+pydeck==0.8.1b0
 pyflakes==3.1.0
+pygls==1.2.1
 Pygments==2.16.1
+pyodbc==5.1.0
 pyparsing==3.1.1
 pyproject-api==1.6.1
+pyproject_hooks==1.0.0
+pyright==1.1.338
 pytest==7.4.2
-pytest-dependency==0.5.1
+pytest-cov==4.1.0
+pytest-dependency==0.6.0
 pytest-mock==3.12.0
 python-dateutil==2.8.2
+python-dotenv==1.0.1
 pytz==2023.3.post1
 PyYAML==6.0.1
 pyzmq==25.1.1
+questionary==2.0.1
 readme-renderer==42.0
+referencing==0.34.0
 regex==2023.8.8
 requests==2.31.0
 requests-toolbelt==1.0.0
+retrying==1.3.4
 rfc3986==2.0.0
 rich==13.5.3
+rich-click==1.7.3
+rpds-py==0.18.0
+ruff==0.1.6
+ruff-lsp==0.0.45
 scipy==1.11.3
 SecretStorage==3.3.3
 six==1.16.0
+smmap==5.0.1
 snowballstemmer==2.2.0
+soupsieve==2.5
 Sphinx==7.2.6
+sphinx-basic-ng==1.0.0b2
 sphinxcontrib-applehelp==1.0.7
 sphinxcontrib-devhelp==1.0.5
 sphinxcontrib-htmlhelp==2.0.4
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.6
 sphinxcontrib-serializinghtml==1.1.9
 sphinxcontrib-websupport==1.2.4
 stack-data==0.6.3
 statsmodels==0.14.0
+streamlit==1.34.0
+tenacity==8.2.3
 tokenize-rt==5.2.0
 toml==0.10.2
 tomli==2.0.1
+tomlkit==0.12.3
+toolz==0.12.1
 tornado==6.3.3
 tox==4.11.3
 tqdm==4.66.1
 traitlets==5.11.2
+tsdownsample==0.1.2
 twine==4.0.2
 typing_extensions==4.8.0
 tzdata==2023.3
+untokenize==0.1.1
 urllib3==2.0.5
 virtualenv==20.24.5
 watchdog==3.0.0
 wcwidth==0.2.8
+Werkzeug==3.0.1
 widgetsnbextension==4.0.9
 zipp==3.17.0
```

### Comparing `hydrobot-0.5.2/tests/.coverage` & `hydrobot-0.6.0/tests/.coverage`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/tests/conftest.py` & `hydrobot-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/tests/test_data/xml_test_data_file.xml` & `hydrobot-0.6.0/tests/test_data/xml_test_data_no_qual.xml`

 * *Files 4% similar despite different names*

#### Comparing `hydrobot-0.5.2/tests/test_data/xml_test_data_file.xml` & `hydrobot-0.6.0/tests/test_data/xml_test_data_no_qual.xml`

```diff
@@ -8,15 +8,15 @@
       <Interpolation>Incremental</Interpolation>
       <ItemFormat>0</ItemFormat>
       <ItemInfo ItemNumber="1">
         <ItemName>General Nastiness</ItemName>
         <ItemFormat>I</ItemFormat>
         <Divisor>1</Divisor>
         <Units>out of 10</Units>
-        <Format>#.###</Format>
+        <Format>###.##</Format>
       </ItemInfo>
     </DataSource>
     <Data DateFormat="mowsecs" NumItems="1">
       <E>
         <T>2619302400</T>
         <I1>10</I1>
       </E>
@@ -55,28 +55,14 @@
       <E>
         <T>2619305100</T>
         <I1>10</I1>
       </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
-    <DataSource Name="General Nastiness" NumItems="1">
-      <TSType>StdQualSeries</TSType>
-      <DataType>SimpleTimeSeries</DataType>
-      <Interpolation>Event</Interpolation>
-      <ItemFormat>0</ItemFormat>
-    </DataSource>
-    <Data DateFormat="mowsecs" NumItems="1">
-      <E>
-        <T>2619302400</T>
-        <I1>500</I1>
-      </E>
-    </Data>
-  </Measurement>
-  <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="General Nastiness" NumItems="3">
       <TSType>CheckSeries</TSType>
       <DataType>SimpleTimeSeries</DataType>
       <Interpolation>Discrete</Interpolation>
       <ItemFormat>140</ItemFormat>
       <ItemInfo ItemNumber="1">
         <ItemName>General Nastiness</ItemName>
@@ -181,28 +167,14 @@
       <E>
         <T>2619305100</T>
         <I1>4.0</I1>
       </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
-    <DataSource Name="Number of Actual Whole Human Turds Floating By" NumItems="1">
-      <TSType>StdQualSeries</TSType>
-      <DataType>Turds per Second</DataType>
-      <Interpolation>Event</Interpolation>
-      <ItemFormat>0</ItemFormat>
-    </DataSource>
-    <Data DateFormat="mowsecs" NumItems="1">
-      <E>
-        <T>2619302400</T>
-        <I1>200</I1>
-      </E>
-    </Data>
-  </Measurement>
-  <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Number of Actual Whole Human Turds Floating By" NumItems="4">
       <TSType>CheckSeries</TSType>
       <DataType>Turds per Second</DataType>
       <Interpolation>Discrete</Interpolation>
       <ItemFormat>140</ItemFormat>
       <ItemInfo ItemNumber="1">
         <ItemName>Turdidity Sensor Reading</ItemName>
@@ -318,28 +290,14 @@
       <E>
         <T>2619305100</T>
         <I1>4</I1>
       </E>
     </Data>
   </Measurement>
   <Measurement SiteName="Mid Stream at Cowtoilet Farm">
-    <DataSource Name="Dead Cow Concentration" NumItems="1">
-      <TSType>StdQualSeries</TSType>
-      <DataType>Dead Cows</DataType>
-      <Interpolation>Event</Interpolation>
-      <ItemFormat>0</ItemFormat>
-    </DataSource>
-    <Data DateFormat="mowsecs" NumItems="1">
-      <E>
-        <T>2619302399</T>
-        <I1>600</I1>
-      </E>
-    </Data>
-  </Measurement>
-  <Measurement SiteName="Mid Stream at Cowtoilet Farm">
     <DataSource Name="Dead Cow Concentration" NumItems="3">
       <TSType>CheckSeries</TSType>
       <DataType>Dead Cows</DataType>
       <Interpolation>Discrete</Interpolation>
       <ItemFormat>140</ItemFormat>
       <ItemInfo ItemNumber="1">
         <ItemName>Dead Cow Concentration</ItemName>
```

### Comparing `hydrobot-0.5.2/tests/test_data_sources.py` & `hydrobot-0.6.0/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/tests/test_data_structure.py` & `hydrobot-0.6.0/tests/test_data_structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     tstypes = [
         "StdSeries",
         "StdQualSeries",
         "CheckSeries",
     ]
 
     data_types = [
-        pd.Series,
-        pd.Series,
+        pd.DataFrame,
+        pd.DataFrame,
         pd.DataFrame,
     ]
 
     blob_list = []
     for ds in datasources:
         for ts, dt in zip(tstypes, data_types, strict=True):
             blob = {
```

### Comparing `hydrobot-0.5.2/tests/test_utils.py` & `hydrobot-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hydrobot-0.5.2/tests/test_web_integration.py` & `hydrobot-0.6.0/tests/test_web_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test actual integration tests."""
+
 from xml.etree import ElementTree
 
 import pandas as pd
 import pytest
 from annalist.annalist import Annalist
 from defusedxml import ElementTree as DefusedElementTree
 from hilltoppy.utils import build_url, get_hilltop_xml
@@ -26,37 +27,37 @@
     -----
     This test checks the connection to the specified server and various functionalities
     of the Processor class.
     The test configuration includes parameters such as base_url, file names,
     site information, date range, and default settings.
     Annalist is configured to log information during the test.
     Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (`standard_series`, `check_data`
-    , `check_series`, `quality_series`) are not empty.
+    Assertions are made to ensure that essential series (`standard_data`, `check_data`
+    , `check_data`, `quality_data`) are not empty.
     Data clipping, removal of flatlined values and spikes, range deletion, insertion of
     missing NaNs, gap closure, quality encoding, XML data structure creation,
     data export, and diagnosis are tested.
 
     Assertions
     ----------
     Various assertions are included throughout the test to verify the expected behavior
     of Processor methods and properties.
     These assertions cover the state of data series before and after certain operations,
     ensuring data integrity and functionality.
     """
     processing_parameters = {
         "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
+        "standard_hts_filename": "RawLoggerNet.hts",
+        "check_hts_filename": "Archive.hts",
         "site": "Whanganui at Te Rewa",
         "from_date": "2021-06-28 00:00",
         "to_date": "2021-07-01 23:00",
         "frequency": "5min",
         "standard_measurement_name": "Stage",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "check_measurement_name": "Water Temperature Check [Water Temperature]",
         "defaults": {
             "high_clip": 20000,
             "low_clip": 0,
             "delta": 1000,
             "span": 10,
             "gap_limit": 12,
             "max_qc": 600,
@@ -169,18 +170,18 @@
 
     check_blobs = parse_xml(check_root)
 
     check_output_path = tmp_path / "check_output.xml"
 
     write_hilltop_xml(check_blobs, check_output_path)
 
-    with open(check_input_path) as f:
+    with open(check_input_path, encoding="utf8") as f:
         check_input_xml = f.read()
 
-    with open(check_output_path) as f:
+    with open(check_output_path, encoding="utf8") as f:
         check_output_xml = f.read()
 
     check_input_tree = DefusedElementTree.fromstring(check_input_xml)
     check_output_tree = DefusedElementTree.fromstring(check_output_xml)
 
     assert ElementTree.indent(check_input_tree) == ElementTree.indent(check_output_tree)
 
@@ -200,16 +201,16 @@
     -----
     This test checks the connection to the specified server and various functionalities
     of the Processor class. The test configuration includes parameters such as
     base_url, file names, site information, date range, and default settings.
 
     Annalist is configured to log information during the test.
     Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
+    Assertions are made to ensure that essential series (standard_data, check_data,
+    check_data, quality_data) are not empty.
 
     Data clipping, removal of flatlined values and spikes, range deletion, insertion of
     missing NaNs, gap closure, quality encoding, XML data structure creation, data
     export, and diagnosis are tested.
 
     Assertions
     ----------
@@ -217,24 +218,24 @@
     of Processor methods and properties.
 
     These assertions cover the state of data series before and after certain
     operations, ensuring data integrity and functionality.
     """
     processing_parameters = {
         "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
+        "standard_hts_filename": "RawLoggerNet.hts",
+        "check_hts_filename": "Archive.hts",
         "site": "Whanganui at Te Rewa",
         "from_date": "2021-01-01 00:00",
         "to_date": "2021-02-02 23:00",
         "frequency": "5min",
         "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "check_measurement_name": "Water Temperature Check [Water Temperature]",
         "defaults": {
-            "high_clip": 5000,
+            "high_clip": 100000,
             "low_clip": 0,
             "delta": 1000,
             "span": 10,
             "gap_limit": 12,
             "max_qc": 600,
         },
     }
@@ -259,97 +260,167 @@
         processing_parameters["from_date"],
         processing_parameters["to_date"],
         processing_parameters["check_hts_filename"],
         processing_parameters["check_measurement_name"],
         processing_parameters["defaults"],
     )
 
-    assert not data.standard_series.empty
-    assert not data.check_series.empty
-    assert not data.quality_series.empty
+    assert isinstance(data.standard_data, pd.DataFrame)
+    assert isinstance(data.quality_data, pd.DataFrame)
+    assert isinstance(data.check_data, pd.DataFrame)
+
+    assert not data.standard_data.empty
+    assert not data.check_data.empty
+    assert not data.quality_data.empty
 
-    standard_before_clip = data.standard_series
-    check_before_clip = data.check_series
+    clip_one = "2021-01-15 12:00"
+    clip_two = "2021-02-01 00:00"
 
+    data.standard_data.loc[clip_one, "Value"] = 100001
+    data.standard_data.loc[clip_two, "Value"] = -5
     data.clip()
 
-    standard_after_clip = data.standard_series
-    check_after_clip = data.check_series
+    assert pd.isna(data.standard_data.loc[clip_one, "Value"])
+    assert pd.isna(data.standard_data.loc[clip_two, "Value"])
 
-    assert not standard_before_clip.equals(standard_after_clip)
-    assert check_before_clip.equals(check_after_clip)
+    assert data.standard_data.loc[clip_one, "Changes"] == "CLP"
+    assert data.standard_data.loc[clip_two, "Changes"] == "CLP"
 
-    assert (
-        data.standard_series[
-            standard_before_clip > processing_parameters["defaults"]["high_clip"]
-        ]
-        .isna()
-        .all()
-    )
-    assert (
-        data.check_series[
-            check_before_clip > processing_parameters["defaults"]["high_clip"]
-        ]
-        .isna()
-        .all()
-    )
+    assert data.standard_data.loc[clip_one, "Remove"]
+    assert data.standard_data.loc[clip_two, "Remove"]
+
+    flat_one = "2021-01-20 12:05"
+    flat_two = "2021-01-20 12:10"
+    flat_three = "2021-01-20 12:15"
+
+    flat_val = data.standard_data.loc["2021-01-20 12:00", "Value"]
 
+    data.standard_data.loc[flat_one, "Value"] = flat_val
+    data.standard_data.loc[flat_two, "Value"] = flat_val
+    data.standard_data.loc[flat_three, "Value"] = flat_val
     data.remove_flatlined_values()
-    # TODO: Write test for remove_flatlined_values
+
+    assert pd.isna(data.standard_data.loc[flat_one, "Value"])
+    assert pd.isna(data.standard_data.loc[flat_two, "Value"])
+    assert pd.isna(data.standard_data.loc[flat_three, "Value"])
+
+    assert data.standard_data.loc[flat_one, "Changes"] == "FLN"
+    assert data.standard_data.loc[flat_two, "Changes"] == "FLN"
+    assert data.standard_data.loc[flat_three, "Changes"] == "FLN"
+
+    assert data.standard_data.loc[flat_one, "Remove"]
+    assert data.standard_data.loc[flat_two, "Remove"]
+    assert data.standard_data.loc[flat_three, "Remove"]
+
+    spike = "2021-01-10 08:00"
+
+    data.standard_data.loc[spike, "Value"] = 100
 
     data.remove_spikes()
-    # TODO: Write test for remove_spikes
 
-    # Checking that the data points I want to delete actually exist:
-    start_idx = "2021-01-01 11:00"
-    end_idx = "2021-01-01 11:30"
-    assert pd.to_datetime(start_idx) in data.standard_series
-    assert pd.to_datetime(end_idx) in data.standard_series
+    assert pd.isna(data.standard_data.loc[spike, "Value"])
 
-    # Make a small gap
-    data.delete_range(start_idx, end_idx)
+    assert data.standard_data.loc[spike, "Changes"] == "SPK"
+
+    assert data.standard_data.loc[spike, "Remove"]
 
-    # Check that gap was made
+    start_idx = "2021-01-05 12:00"
+    end_idx = "2021-01-05 12:30"
+
+    print(data.standard_data.loc[start_idx:end_idx])
+    data.remove_range(start_idx, end_idx)
+    print(data.standard_data.loc[start_idx:end_idx])
+
+    assert pd.isna(
+        data.standard_data.loc[start_idx:end_idx, "Value"]
+    ).all(), "processor.remove_range appears to be broken."
     assert (
-        pd.to_datetime(start_idx) not in data.standard_series
+        data.standard_data.loc[start_idx:end_idx, "Changes"]
+        .apply(lambda x: x == "MAN")
+        .all()
+    ), "processor.remove_range appears to be broken."
+
+    # Small Gap
+    start_idx = "2021-02-02 11:00"
+    end_idx = "2021-02-02 11:30"
+
+    data.delete_range(start_idx, end_idx)
+    # Check that row was completely deleted
+    assert (
+        pd.to_datetime(start_idx) not in data.standard_data.index
     ), "processor.delete_range appears to be broken."
     assert (
-        pd.to_datetime(end_idx) not in data.standard_series
+        pd.to_datetime(end_idx) not in data.standard_data.index
     ), "processor.delete_range appears to be broken."
 
     # Insert nans where values are missing
     data.insert_missing_nans()
 
     # Check that NaNs are inserted
     assert pd.isna(
-        data.standard_series[start_idx]
+        data.standard_data.loc[start_idx, "Value"]
     ), "processor.insert_missing_nans appears to be broken."
     assert pd.isna(
-        data.standard_series[end_idx]
+        data.standard_data.loc[end_idx, "Value"]
     ), "processor.insert_missing_nans appears to be broken."
 
     # "Close" gaps (i.e. remove nan rows)
+    print(data.standard_data.loc[start_idx])
     data.gap_closer()
 
     # Check that gap was closed
     assert (
-        pd.to_datetime(start_idx) not in data.standard_series
+        pd.to_datetime(start_idx) not in data.standard_data.index
     ), "processor.gap_closer appears to be broken."
     assert (
-        pd.to_datetime(end_idx) not in data.standard_series
+        pd.to_datetime(end_idx) not in data.standard_data.index
     ), "processor.gap_closer appears to be broken."
 
+    # BigGap
+    start_idx = "2021-01-30 00:00"
+    end_idx = "2021-02-01 00:00"
+
+    data.delete_range(start_idx, end_idx)
+    # Check that row was completely deleted
+    assert (
+        pd.to_datetime(start_idx) not in data.standard_data.index
+    ), "processor.delete_range appears to be broken."
+    assert (
+        pd.to_datetime(end_idx) not in data.standard_data.index
+    ), "processor.delete_range appears to be broken."
+
+    # Insert nans where values are missing
+    data.insert_missing_nans()
+
+    # Check that NaNs are inserted
+    assert pd.isna(
+        data.standard_data.loc[start_idx, "Value"]
+    ), "processor.insert_missing_nans appears to be broken."
+    assert pd.isna(
+        data.standard_data.loc[end_idx, "Value"]
+    ), "processor.insert_missing_nans appears to be broken."
+
+    # "Close" gaps (i.e. remove nan rows)
+    print(data.standard_data.loc[start_idx])
+    data.gap_closer()
+
+    # Check that gap was closed
+    # assert (
+    #     pd.to_datetime(start_idx) not in data.standard_data.index
+    # ), "processor.gap_closer appears to be broken."
+    # assert (
+    #     pd.to_datetime(end_idx) not in data.standard_data.index
+    # ), "processor.gap_closer appears to be broken."
+
     data.quality_encoder()
 
     # TODO: Write test for quality_encoder
 
     data.to_xml_data_structure()
 
-    # TODO: Write test for to_xml_data_structure
-
     data.data_exporter(tmp_path / "xml_data.xml")
     data.data_exporter(tmp_path / "csv_data.csv", ftype="csv")
     data.data_exporter(tmp_path / "hilltop_csv_data.csv", ftype="hilltop_csv")
 
     # TODO: Write tests for data_exporter
 
     data.diagnosis()
@@ -372,38 +443,38 @@
     of the Processor class.
 
     The test configuration includes parameters such as base_url, file names, site
     information, date range, and default settings.
 
     Annalist is configured to log information during the test.
     Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
+    Assertions are made to ensure that essential series (standard_data, check_data,
+    check_data, quality_data) are not empty.
 
     Data clipping, removal of flatlined values and spikes, range deletion, insertion of
     missing NaNs, gap closure, quality encoding, XML data structure creation, data
     export, and diagnosis are tested.
 
     Assertions
     ----------
     Various assertions are included throughout the test to verify the expected behavior
     of Processor methods and properties.
     These assertions cover the state of data series before and after certain
     operations, ensuring data integrity and functionality.
     """
     processing_parameters = {
         "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
+        "standard_hts_filename": "RawLoggerNet.hts",
+        "check_hts_filename": "Archive.hts",
         "site": "Whanganui at Te Rewa",
-        "from_date": "2003-01-01 00:00",
-        "to_date": "2003-02-02 23:00",
+        "from_date": "1903-01-01 00:00",
+        "to_date": "1903-02-02 23:00",
         "frequency": "5min",
         "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "check_measurement_name": "Water Temperature Check [Water Temperature]",
         "defaults": {
             "high_clip": 5000,
             "low_clip": 0,
             "delta": 1000,
             "span": 10,
             "gap_limit": 12,
             "max_qc": 600,
@@ -430,25 +501,25 @@
             processing_parameters["frequency"],
             processing_parameters["from_date"],
             processing_parameters["to_date"],
             processing_parameters["check_hts_filename"],
             processing_parameters["check_measurement_name"],
             processing_parameters["defaults"],
         )
-
-        assert data.standard_series.empty
-        assert data.check_series.empty
-        assert data.quality_series.empty
-        assert data.raw_standard_series.empty
+        assert isinstance(data.standard_data, pd.DataFrame)
+        assert isinstance(data.quality_data, pd.DataFrame)
+        assert isinstance(data.check_data, pd.DataFrame)
+
+        assert data.standard_data.empty
+        assert data.check_data.empty
+        assert data.quality_data.empty
         assert data.raw_standard_blob is None
         assert data.raw_standard_xml is None
-        assert data.raw_quality_series.empty
         assert data.raw_quality_blob is None
         assert data.raw_quality_xml is None
-        assert data.raw_check_data.empty
         assert data.raw_check_blob is None
         assert data.raw_check_xml is None
 
 
 @pytest.mark.slow()
 @pytest.mark.remote()
 def test_failed_requests(tmp_path):
@@ -466,38 +537,38 @@
     of the Processor class.
 
     The test configuration includes parameters such as base_url, file names, site
     information, date range, and default settings.
 
     Annalist is configured to log information during the test.
     Processor is instantiated with the provided processing parameters.
-    Assertions are made to ensure that essential series (standard_series, check_data,
-    check_series, quality_series) are not empty.
+    Assertions are made to ensure that essential series (standard_data, check_data,
+    check_data, quality_data) are not empty.
 
     Data clipping, removal of flatlined values and spikes, range deletion, insertion of
     missing NaNs, gap closure, quality encoding, XML data structure creation, data
     export, and diagnosis are tested.
 
     Assertions
     ----------
     Various assertions are included throughout the test to verify the expected behavior
     of Processor methods and properties.
     These assertions cover the state of data series before and after certain
     operations, ensuring data integrity and functionality.
     """
     processing_parameters = {
         "base_url": "http://hilltopdev.horizons.govt.nz/",
-        "standard_hts_filename": "RawLogger.hts",
-        "check_hts_filename": "boo.hts",
+        "standard_hts_filename": "RawLoggerNet.hts",
+        "check_hts_filename": "Archive.hts",
         "site": "Whanganui at Te Rewa",
         "from_date": "2003-01-01 00:00",
         "to_date": "2003-02-02 23:00",
         "frequency": "4min",
         "standard_measurement_name": "Water level statistics: Point Sample",
-        "check_measurement_name": "External S.G. [Water Level NRT]",
+        "check_measurement_name": "Water Temperature Check [Water Temperature]",
         "defaults": {
             "high_clip": 5000,
             "low_clip": 0,
             "delta": 1000,
             "span": 10,
             "gap_limit": 12,
             "max_qc": 600,
@@ -584,15 +655,14 @@
                 processing_parameters["check_measurement_name"],
                 processing_parameters["defaults"],
             )
         assert (
             "Standard measurement name 'Notarealmeasurement' not found at site"
             in str(excinfo.value)
         )
-
         with pytest.raises(
             ValueError,
             match=r"Unrecognised start time",
         ) as excinfo:
             _ = Processor(
                 processing_parameters["base_url"],
                 processing_parameters["site"],
@@ -645,15 +715,16 @@
                 "Notarealhtsfilename",
                 processing_parameters["check_measurement_name"],
                 processing_parameters["defaults"],
             )
         assert "No sites found for the base_url and hts combo." in str(excinfo.value)
 
         with pytest.raises(
-            ValueError, match=r"Check measurement name 'Notarealmeasurement' not found "
+            ValueError,
+            match=r"Check measurement name 'Notarealmeasurement' not found ",
         ) as excinfo:
             _ = Processor(
                 processing_parameters["base_url"],
                 processing_parameters["site"],
                 processing_parameters["standard_hts_filename"],
                 processing_parameters["standard_measurement_name"],
                 processing_parameters["frequency"],
```

