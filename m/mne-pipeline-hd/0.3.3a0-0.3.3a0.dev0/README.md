# Comparing `tmp/mne-pipeline-hd-0.3.3a0.tar.gz` & `tmp/mne_pipeline_hd-0.3.3a0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-pipeline-hd-0.3.3a0.tar", last modified: Thu Jul 27 11:12:00 2023, max compression
+gzip compressed data, was "mne_pipeline_hd-0.3.3a0.dev0.tar", last modified: Mon May 13 19:56:59 2024, max compression
```

## Comparing `mne-pipeline-hd-0.3.3a0.tar` & `mne_pipeline_hd-0.3.3a0.dev0.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.759886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/check_ressources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/dev_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    57606 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    28799 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.767886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49094 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/base_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/education_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    65760 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/function_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/gui_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    84283 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/loading_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    27186 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    30254 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    70457 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/parameter_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    22826 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/plot_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/welcome_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.771885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/function_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    59334 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.771885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/default_settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/functions.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_license.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21717 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    24707 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png
--rw-r--r--   0 runner    (1001) docker     (123)    16878 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/parameters.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_param_guis.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_qsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_welcome_window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:12:00.763886 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:12:00.000000 mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-27 11:11:38.000000 mne-pipeline-hd-0.3.3a0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:12:00.775885 mne-pipeline-hd-0.3.3a0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.008757 mne_pipeline_hd-0.3.3a0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-13 19:56:59.008757 mne_pipeline_hd-0.3.3a0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4300 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:58.996757 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:58.996757 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/check_ressources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/console_widget_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/dev_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.000758 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/default_settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/functions.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_license.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21717 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24707 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_icon_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_logo_evee_smaller.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/parameters.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.000758 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54470 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33021 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.004758 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50673 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/base_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12749 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9136 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/education_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66010 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/function_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21928 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/gui_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83169 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/loading_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27472 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76176 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/parameter_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22877 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/plot_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6764 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/welcome_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.004758 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17490 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/function_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68143 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11272 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27469 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.008757 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_base_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_parameter_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_qsettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_welcome_window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:56:59.008757 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 19:56:58.000000 mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-13 19:56:50.000000 mne_pipeline_hd-0.3.3a0.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:56:59.008757 mne_pipeline_hd-0.3.3a0.dev0/setup.cfg
```

### Comparing `mne-pipeline-hd-0.3.3a0/LICENSE.txt` & `mne_pipeline_hd-0.3.3a0.dev0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mne-pipeline-hd-0.3.3a0/PKG-INFO` & `mne_pipeline_hd-0.3.3a0.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,28 @@
-Metadata-Version: 2.1
-Name: mne-pipeline-hd
-Version: 0.3.3a0
-Summary: A Pipeline-GUI for MNE-Python from MEG-Lab Heidelberg
-Author-email: Martin Schulz <dev@mgschulz.de>
-License: BSD-3-Clause
-Project-URL: Homepage, https://github.com/marsipu/mne-pipeline-hd
-Project-URL: Repository, https://github.com/marsipu/mne-pipeline-hd.git
-Keywords: mne-python,meg,eeg,pipeline,gui,heidelberg
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # mne-pipeline-hd
 
 ### A Pipeline-GUI for [MNE-Python](https://mne.tools/stable/index.html)  from MEG-Lab Heidelberg
 
-![mne-pipeline-hd Logo](mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg)
+![mne-pipeline-hd Logo](mne_pipeline_hd/extra/mne_pipeline_logo_evee_smaller.jpg)
 
 ## Installation
 
 1. Install MNE-python as instructed on
-   the [website](https://www.martinos.org/mne/stable/install_mne_python.html),
-   I would recommend to install in a separate conda environment with:
-   `conda env create -n mne_p -f environment.yml`
-2. `conda activate mne_p`
-3. `pip install https://github.com/marsipu/mne-pipeline-hd/zipball/main`
+   the [website](https://www.martinos.org/mne/stable/install_mne_python.html)
+2. Then run `pip install https://github.com/marsipu/mne-pipeline-hd/zipball/main` in the conda-enviroment you created in step 1 for MNE-Python.
 
 ## Update
 
 Run `pip install --upgrade --no-deps --force-reinstall https://github.com/marsipu/mne-pipeline-hd/zipball/main`
 for an update to the development version
 or `pip install --upgrade mne-pipeline-hd` for the latest release.
 
 ## Start
 
-Run `mne_pipeline_hd` in your mne_pipeline-environment (`conda activate mne_p`)
+Run `mne_pipeline_hd` in your conda-environment where you installed mne-python and mne-pipeline-hd.
 
 **or**
 
 run \_\_main\_\_.py from the terminal or an IDE like PyCharm, VSCode, Atom,
 etc.
 
 ***When using the pipeline and its functions bear in mind that the pipeline is
@@ -51,18 +30,18 @@
 The basic functions supplied are just a suggestion and you should verify before
 usage if they do what you need.
 They are also partly still adjusted to specific requirements which may not
 apply to all data.***
 
 ## Bug-Report/Feature-Request
 
-Please report bugs on GitHub as an issue or to me (dev@earthman-music.de)
+Please report bugs on GitHub as an issue or to me (dev@mgschulz.de)
 directly.
 And if you got ideas on how to improve the pipeline or some feature-requests,
-you are welcome to open an issue too or send an e-mail (dev@earthman-music.de)
+you are welcome to open an issue too or send an e-mail (dev@mgschulz.de)
 
 ## Contribute and build your own functions/fix bugs
 
 I you want to help by contributing, I would be very happy:
 
 You need a [GitHub-Account](https://github.com/)
 and should
@@ -71,21 +50,22 @@
 
 1. Fork this repository on GitHub
 2. Move to the folder where you want to clone to
 3. Clone **your forked repository** with git from a
    terminal: `git clone <url you get from the green clone-button from your forked repository on GitHub>`
 4. Add upstream to git for
    updates: `git remote add upstream git://github.com/marsipu/mne-pipeline-hd.git`
-5. Install development version with pip: `pip install -e ./`
-6. Create a branch for changes: `git checkout -b <branch-name>`
-7. Commit changes: `git commit -am "<your commit message>"`
-8. Push changes to your forked repository on GitHub: `git push`
-9. Make "New pull request" from your new feature branch
+5. Install development version with pip: `pip install -e .[tests]`
+6. Install the pre-commit hooks with: `pre-commit install`
+7. Create a branch for changes: `git checkout -b <branch-name>`
+8. Commit changes: `git commit -am "<your commit message>"`
+9. Push changes to your forked repository on GitHub: `git push`
+10. Make "New pull request" from your new feature branch
 
-You can always [write me](mailto:dev@earthman-music.de), if you have questions
+You can always [write me an e-mail](mailto:dev@mgschulz.de), if you have questions
 about the contribution-process
 or about the program-structure.
 
 ## Acknowledgments
 
 This Pipeline is build on top
 of [MNE-Python](https://mne.tools/stable/index.html)
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/__main__.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,139 +1,141 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
-# flake: noqa E402
 
-import logging
 import os
+import re
 import sys
 from importlib import resources
+from os.path import join
 
-from PyQt5.QtCore import QTimer, Qt
-from PyQt5.QtGui import QIcon, QFont
-from PyQt5.QtWidgets import QApplication
+import qtpy
+from qtpy.QtCore import QTimer, Qt
+from qtpy.QtGui import QIcon, QFont
+from qtpy.QtWidgets import QApplication
 
+import mne_pipeline_hd
 from mne_pipeline_hd.gui.gui_utils import StdoutStderrStream, UncaughtHook
 from mne_pipeline_hd.gui.welcome_window import WelcomeWindow
 from mne_pipeline_hd.pipeline.legacy import legacy_import_check
-from mne_pipeline_hd.pipeline.pipeline_utils import ismac, islin, QS
+from mne_pipeline_hd.pipeline.pipeline_utils import (
+    ismac,
+    islin,
+    QS,
+    iswin,
+    init_logging,
+    logger,
+)
 
 # Check for changes in required packages
 legacy_import_check()
 
 import qdarktheme  # noqa: E402
 
 
+def init_streams():
+    # Redirect stdout and stderr to capture it later in GUI
+    sys.stdout = StdoutStderrStream("stdout")
+    sys.stderr = StdoutStderrStream("stderr")
+
+
 def main():
     app_name = "mne-pipeline-hd"
     organization_name = "marsipu"
     domain_name = "https://github.com/marsipu/mne-pipeline-hd"
 
     qdarktheme.enable_hi_dpi()
 
     app = QApplication.instance()
     if not app:
         app = QApplication(sys.argv)
     app.setApplicationName(app_name)
     app.setOrganizationName(organization_name)
     app.setOrganizationDomain(domain_name)
-
-    # Disable Help-Button
-    try:
-        app.setAttribute(Qt.AA_DisableWindowContextHelpButton, True)
-    except AttributeError:
-        print("pyqt-Version is < 5.12")
+    # For Spyder to make console accessible again
+    app.lastWindowClosed.connect(app.quit)
 
     # Avoid file-dialog-problems with custom file-managers in linux
     if islin:
         app.setAttribute(Qt.AA_DontUseNativeDialogs, True)
 
     # Mac-Workarounds
     if ismac:
         # Workaround for not showing with PyQt < 5.15.2
         os.environ["QT_MAC_WANTS_LAYER"] = "1"
 
-    # Avoid Mayavi-Issues
-    os.environ["ETS_TOOLKIT"] = "qt4"
-    os.environ["QT_API"] = "pyqt5"
-
     # ToDo: MP
     # # Set multiprocessing method to spawn
     # multiprocessing.set_start_method('spawn')
 
-    # Redirect stdout to capture it later in GUI
-    sys.stdout = StdoutStderrStream("stdout")
-    # Redirect stderr to capture it later in GUI
-    sys.stderr = StdoutStderrStream("stderr")
+    init_streams()
+
+    debug_mode = os.environ.get("MNEPHD_DEBUG", False) == "true"
+    init_logging(debug_mode)
 
-    # Initialize Logger (root)
-    logger = logging.getLogger()
-    logger.setLevel(QS().value("log_level", defaultValue=logging.INFO))
-    formatter = logging.Formatter(
-        "%(asctime)s: %(message)s", datefmt="%Y/%m/%d %H:%M:%S"
-    )
-    console_handler = logging.StreamHandler()
-    console_handler.setFormatter(formatter)
-    logger.addHandler(console_handler)
-    logger.info("Starting MNE-Pipeline HD")
+    logger().info("Starting MNE-Pipeline HD")
+
+    # Show Qt-binding
+    if any([qtpy.PYQT5, qtpy.PYQT6]):
+        qt_version = qtpy.PYQT_VERSION
+    else:
+        qt_version = qtpy.PYSIDE_VERSION
+    logger().info(f"Using {qtpy.API_NAME} {qt_version}")
 
     # Initialize Exception-Hook
-    qt_exception_hook = UncaughtHook()
-    # this registers the exception_hook() function
-    # as hook with the Python interpreter
-    sys.excepthook = qt_exception_hook.exception_hook
+    if debug_mode:
+        logger().info("Debug-Mode is activated")
+    else:
+        qt_exception_hook = UncaughtHook()
+        # this registers the exception_hook() function
+        # as hook with the Python interpreter
+        sys.excepthook = qt_exception_hook.exception_hook
 
     # Initialize Layout
     font_family = QS().value("app_font")
     font_size = QS().value("app_font_size")
     app.setFont(QFont(font_family, font_size))
 
     # Set Style and Window-Icon
     app_style = QS().value("app_style")
 
     # Legacy 20230717
     if app_style not in ["dark", "light", "auto"]:
         app_style = "auto"
 
-    if app_style == "dark":
-        qdarktheme.setup_theme("dark")
+    qdarktheme.setup_theme(app_style)
+    st = qdarktheme.load_stylesheet(app_style)
+    is_dark = "background:rgba(32, 33, 36, 1.000)" in st
+    if is_dark:
         icon_name = "mne_pipeline_icon_dark.png"
-    elif app_style == "light":
-        qdarktheme.setup_theme("light")
-        icon_name = "mne_pipeline_icon_light.png"
+        # Fix ToolTip-Problem on Windows
+        # https://github.com/5yutan5/PyQtDarkTheme/issues/239
+        if iswin:
+            match = re.search(r"QToolTip \{([^\{\}]+)\}", st)
+            if match is not None:
+                replace_str = "QToolTip {" + match.group(1) + ";border: 0px}"
+                st = st.replace(match.group(0), replace_str)
+                QApplication.instance().setStyleSheet(st)
     else:
-        qdarktheme.setup_theme("auto")
-        st = qdarktheme.load_stylesheet("auto")
-        if "background:rgba(32, 33, 36, 1.000)" in st:
-            icon_name = "mne_pipeline_icon_dark.png"
-        else:
-            icon_name = "mne_pipeline_icon_light.png"
+        icon_name = "mne_pipeline_icon_light.png"
 
-    with resources.path("mne_pipeline_hd.resource", icon_name) as icon_path:
-        app_icon = QIcon(str(icon_path))
+    icon_path = join(resources.files(mne_pipeline_hd.extra), icon_name)
+    app_icon = QIcon(str(icon_path))
     app.setWindowIcon(app_icon)
 
     # Initiate WelcomeWindow
     WelcomeWindow()
 
-    # Redirect stdout to capture it later in GUI
-    sys.stdout = StdoutStderrStream("stdout")
-    # Redirect stderr to capture it later in GUI
-    sys.stderr = StdoutStderrStream("stderr")
-
     # Command-Line interrupt with Ctrl+C possible
     timer = QTimer()
     timer.timeout.connect(lambda: None)
     timer.start(500)
 
-    # For Spyder to make console accessible again
-    app.lastWindowClosed.connect(app.quit)
-
     sys.exit(app.exec())
 
 
 if __name__ == "__main__":
     # Todo: Make Exception-Handling for PyQt-Start working (from event-loop?)
     main()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/conftest.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/conftest.py`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/development/dev_utils.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/development/dev_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+# -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 import sys
 import traceback
 from ast import literal_eval
 
-from PyQt5.QtWidgets import (
+from qtpy.QtWidgets import (
     QWidget,
     QVBoxLayout,
     QGridLayout,
     QComboBox,
     QHBoxLayout,
     QLineEdit,
     QPushButton,
     QDialog,
     QApplication,
 )
 
 from mne_pipeline_hd.gui import parameter_widgets
 from mne_pipeline_hd.gui.base_widgets import SimpleDict
 from mne_pipeline_hd.gui.parameter_widgets import Param
-from mne_pipeline_hd.tests.test_param_guis import gui_kwargs, parameters
+from mne_pipeline_hd.tests.test_parameter_widgets import gui_kwargs, parameters
 
 
 class ParamGuis(QWidget):
     def __init__(self):
         super().__init__()
 
         self.gui_dict = dict()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/operations.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,45 +4,66 @@
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from __future__ import print_function
 
 import gc
-import logging
 import os
 import shutil
 import subprocess
 import sys
 import time
 from functools import reduce
 from itertools import combinations
 from os import environ
 from os.path import isdir, isfile, join
-from pathlib import Path
 
 import autoreject as ar
 import mne
 import mne_connectivity
 import numpy as np
-from mne.preprocessing import ICA
+from mne.preprocessing import ICA, find_bad_channels_maxwell
+from mne_connectivity import SpectralConnectivity
 
-from mne_pipeline_hd.pipeline.loading import MEEG
+from mne_pipeline_hd.pipeline.loading import MEEG, FSMRI
 from mne_pipeline_hd.pipeline.pipeline_utils import (
     check_kwargs,
     compare_filep,
     ismac,
     iswin,
+    get_n_jobs,
+    logger,
 )
 
 
 # Todo: Create docstrings for each function
 # =============================================================================
 # PREPROCESSING AND GETTING TO EVOKED AND TFR
 # =============================================================================
+def find_bads(meeg, n_jobs, **kwargs):
+    raw = meeg.load_raw()
+
+    if raw.info["dev_head_t"] is None:
+        coord_frame = "meg"
+    else:
+        coord_frame = "head"
+
+    # Set number of CPU-cores to use
+    os.environ["OMP_NUM_THREADS"] = str(get_n_jobs(n_jobs))
+
+    noisy_chs, flat_chs = find_bad_channels_maxwell(
+        raw, coord_frame=coord_frame, **kwargs
+    )
+    logger().info(f"Noisy channels: {noisy_chs}\n" f"Flat channels: {flat_chs}")
+    raw.info["bads"] = noisy_chs + flat_chs + raw.info["bads"]
+    meeg.set_bad_channels(raw.info["bads"])
+    meeg.save_raw(raw)
+
+
 def filter_data(
     meeg,
     filter_target,
     highpass,
     lowpass,
     filter_length,
     l_trans_bandwidth,
@@ -63,15 +84,15 @@
     filtered_path = meeg.io_dict[filter_target]["path"]
     results = compare_filep(
         meeg, filtered_path, ["highpass", "lowpass", "bad_interpolation"]
     )
 
     if any([results[key] != "equal" for key in results]):
         # Load Data
-        data = meeg.io_dict[filter_target]["load"]()
+        data = meeg.load(filter_target)
 
         # use cuda for filtering if enabled
         if enable_cuda:
             mne.cuda.init_cuda(ignore_config=True)
             n_jobs = "cuda"
 
         # Filter Data
@@ -107,17 +128,17 @@
                 fir_design=fir_design,
                 skip_by_annotation=skip_by_annotation,
                 pad=fir_pad,
             )
 
         # Save Data
         if filter_target == "raw":
-            meeg.io_dict["raw_filtered"]["save"](data)
+            meeg.save("raw_filtered", data)
         else:
-            meeg.io_dict[filter_target]["save"](data)
+            meeg.save(filter_target, data)
 
         # Remove raw to avoid memory overload
         del data
         gc.collect()
 
     else:
         print(
@@ -171,35 +192,46 @@
                 f"and lowpass={lowpass}"
             )
 
     else:
         print("no erm_file assigned")
 
 
+def notch_filter(meeg, notch_frequencies, n_jobs):
+    raw_filtered = meeg.load_filtered()
+
+    raw_filtered = raw_filtered.notch_filter(notch_frequencies, n_jobs=1)
+    meeg.save_filtered(raw_filtered)
+
+
 def interpolate_bads(meeg, bad_interpolation):
-    data = meeg.io_dict[bad_interpolation]["load"]()
+    data = meeg.load(bad_interpolation)
 
     if bad_interpolation == "evoked":
         for evoked in data:
-            evoked.interpolate_bads()
-    else:
-        data.interpolate_bads()
+            # Add bads for channels present
+            evoked.info["bads"] = [b for b in meeg.bad_channels if b in data.ch_names]
+            evoked.interpolate_bads(reset_bads=True)
+    else:
+        # Add bads for channels present
+        data.info["bads"] = [b for b in meeg.bad_channels if b in data.ch_names]
+        data.interpolate_bads(reset_bads=True)
 
-    meeg.io_dict[bad_interpolation]["save"](data)
+    meeg.save(bad_interpolation, data)
 
 
 def add_erm_ssp(
     meeg, erm_ssp_duration, erm_n_grad, erm_n_mag, erm_n_eeg, n_jobs, show_plots
 ):
     raw_filtered = meeg.load_filtered()
     erm_filtered = meeg.load_erm_processed()
 
     # Only include channels from Empty-Room-Data,
     # which are present in filtered-data
-    erm_filtered = erm_filtered.copy().pick_channels(
+    erm_filtered = erm_filtered.copy().pick(
         [ch for ch in erm_filtered.ch_names if ch in raw_filtered.ch_names]
     )
 
     erm_projs = mne.compute_proj_raw(
         erm_filtered,
         duration=erm_ssp_duration,
         n_grad=erm_n_grad,
@@ -411,17 +443,15 @@
 
         for q in equals:
             if (
                 q not in events[:, 0]
                 and q not in events[:, 0] + 1
                 and q not in events[:, 0] - 1
             ):
-                events = np.append(
-                    events, [[q, 0, int(2**a + 2**b + 2**c)]], axis=0
-                )
+                events = np.append(events, [[q, 0, int(2**a + 2**b + 2**c)]], axis=0)
 
     for a, b in combinations(range(6), 2):
         equals = np.intersect1d(evs_tol[a], evs_tol[b])
         too_close = np.where(np.diff(equals) <= 1)
         if np.size(too_close) >= 1:
             equals = np.delete(equals, too_close, 0)
             equals -= 1
@@ -483,15 +513,15 @@
     raw_filtered = meeg.load_filtered()
     events = meeg.load_events()
 
     # Pick selected channel_types if not done before
     raw_filtered.pick(ch_types)
 
     if len(ch_names) > 0 and ch_names != "all":
-        raw_filtered.pick_channels(ch_names)
+        raw_filtered.pick(ch_names)
 
     if bad_interpolation is None:
         # Exclude bad-channels if no Bad-Channel-Interpolation is intended
         # after making the epochs or the Evokeds
         raw_filtered.pick("all", exclude="bads")
 
     epochs = mne.Epochs(
@@ -508,15 +538,15 @@
         decim=decim,
         on_missing="ignore",
         reject_by_annotation=reject_by_annotation,
     )
 
     if (
         any([i is not None for i in [use_autoreject, reject, flat]])
-        and bad_interpolation == "Evokeds"
+        and bad_interpolation == "evokeds"
     ):
         raise RuntimeWarning(
             'With bad_interpolation="Evokeds", '
             "the bad channels are still included and "
             "may heavily influence the outcome of dropping epochs with reject,"
             " flat or autoreject!"
             "\n(to solve this you could uncheck autoreject, "
@@ -532,15 +562,15 @@
         epochs, reject_log = ar_object.fit_transform(epochs, return_log=True)
         meeg.save_reject_log(reject_log)
 
     else:
         if use_autoreject == "Threshold":
             reject = meeg.load_json("autoreject_threshold")
             if reject is None or overwrite_ar:
-                reject = ar.get_rejection_threshold(epochs)
+                reject = ar.get_rejection_threshold(epochs, random_state=8)
                 meeg.save_json("autoreject_threshold", reject)
             print(
                 f"Dropping bad epochs with autoreject"
                 f" rejection-thresholds: {reject}"
             )
 
         else:
@@ -570,36 +600,30 @@
     ica_method,
     ica_fitto,
     n_components,
     ica_noise_cov,
     ica_remove_proj,
     ica_reject,
     ica_autoreject,
+    overwrite_ar,
     ch_types,
     ch_names,
     reject_by_annotation,
     ica_eog,
     eog_channel,
     ica_ecg,
     ecg_channel,
     **kwargs,
 ):
-    if ica_fitto == "epochs":
-        data = meeg.load_epochs()
-        # Bad-Channels and Channel-Types are already picked in epoch_raw
-    else:
-        if ica_fitto == "raw":
-            data = meeg.load_raw()
-
-        else:
-            data = meeg.load_filtered()
-
+    data = meeg.load(ica_fitto)
+    # Bad-Channels and Channel-Types are already picked in epochs
+    if ica_fitto != "epochs":
         data.pick(ch_types, exclude="bads")
         if len(ch_names) > 0 and ch_names != "all":
-            data.pick_channels(ch_names)
+            data.pick(ch_names)
 
     # Filter if data is not highpass-filtered >= 1
     if data.info["highpass"] < 1:
         filt_data = data.filter(1, None)
     else:
         filt_data = data
 
@@ -620,20 +644,20 @@
     if ica_autoreject and ica_fitto != "epochs":
         # Estimate Reject-Thresholds on simulated epochs
         # Creating simulated epochs with len 1s
         simulated_events = mne.make_fixed_length_events(data, duration=1)
         simulated_epochs = mne.Epochs(
             data, simulated_events, baseline=None, tmin=0, tmax=1, proj=False
         )
-        reject = ar.get_rejection_threshold(simulated_epochs)
+        reject = ar.get_rejection_threshold(simulated_epochs, random_state=8)
         print(f"Autoreject Rejection-Threshold: {reject}")
     elif ica_autoreject and ica_fitto == "epochs":
         reject = meeg.load_json("autoreject_threshold")
-        if not reject:
-            reject = ar.get_rejection_threshold(data)
+        if reject is None or overwrite_ar:
+            reject = ar.get_rejection_threshold(data, random_state=8)
             meeg.save_json("autoreject_threshold", reject)
     else:
         reject = ica_reject
 
     # Remove projections
     if ica_remove_proj:
         filt_data.del_proj()
@@ -686,14 +710,19 @@
             )
 
         if eog_epochs:
             ica.exclude += eog_indices
             meeg.save_eog_epochs(eog_epochs)
             meeg.save_json("eog_indices", eog_indices)
             meeg.save_json("eog_scores", eog_scores)
+    else:
+        # Remove old eog_epochs, eog_indices and eog_scores if new ICA is calculated
+        meeg.remove_path("epochs_eog")
+        meeg.remove_json("eog_indices")
+        meeg.remove_json("eog_scores")
 
     if ica_ecg:
         create_ecg_kwargs = check_kwargs(kwargs, mne.preprocessing.create_ecg_epochs)
         find_ecg_kwargs = check_kwargs(kwargs, ica.find_bads_ecg)
 
         # Using an ECG channel to select components
         if ecg_channel and ecg_channel in eog_ecg_raw.ch_names:
@@ -723,203 +752,61 @@
             )
 
         if ecg_epochs:
             ica.exclude += ecg_indices
             meeg.save_ecg_epochs(ecg_epochs)
             meeg.save_json("ecg_indices", ecg_indices)
             meeg.save_json("ecg_scores", ecg_scores)
+    else:
+        # Remove old ecg_epochs, ecg_indices and ecg_scores if new ICA is calculated
+        meeg.remove_path("epochs_ecg")
+        meeg.remove_json("ecg_indices")
+        meeg.remove_json("ecg_scores")
 
     meeg.save_ica(ica)
     # Add components to ica_exclude-dictionary
-    meeg.pr.ica_exclude[meeg.name] = ica.exclude
-
-
-def _ica_plotto_helper(meeg, ica_plotto):
-    ica = meeg.load_ica()
-
-    if ica_plotto == "raw":
-        data = meeg.load_raw()
-
-    elif ica_plotto == "raw_filtered":
-        data = meeg.load_filtered()
-
-    elif ica_plotto == "epochs":
-        data = meeg.load_epochs()
-
-    elif ica_plotto == "epochs_eog":
-        data = meeg.load_eog_epochs()
-
-    elif ica_plotto == "epochs_ecg":
-        data = meeg.load_ecg_epochs()
-
-    elif ica_plotto == "evoked":
-        data = meeg.load_evokeds()
-
-    elif ica_plotto == "evoked (EOG)":
-        data = meeg.load_eog_epochs().average()
-
-    elif ica_plotto == "evoked (ECG)":
-        data = meeg.load_ecg_epochs().average()
-
-    else:
-        data = None
+    meeg.pr.meeg_ica_exclude[meeg.name] = ica.exclude
 
-    return ica, data
 
+def apply_ica(meeg, ica_apply_target, n_pca_components):
+    # Check file-parameters to make sure,
+    # that ica is not applied twice in a row
 
-def plot_ica_components(meeg, show_plots):
+    data = meeg.load(ica_apply_target)
     ica = meeg.load_ica()
-    components_fig = ica.plot_components(title=meeg.name, show=show_plots)
-    meeg.plot_save("ica", subfolder="components", matplotlib_figure=components_fig)
-
-    return components_fig, ica
-
-
-def plot_ica_sources(meeg, ica_source_data, show_plots):
-    ica, data = _ica_plotto_helper(meeg, ica_source_data)
-    sources_fig = ica.plot_sources(
-        data, stop=ica.n_components, title=meeg.name, show=show_plots
-    )
-    meeg.plot_save("ica", subfolder="sources", matplotlib_figure=sources_fig)
-
-    return sources_fig, ica
-
-
-def plot_ica_overlay(meeg, ica_overlay_data, show_plots):
-    ica, data = _ica_plotto_helper(meeg, ica_overlay_data)
-    overlay_figs = list()
 
-    if ica_overlay_data == "Evokeds":
-        for evoked in [e for e in data if e.comment in meeg.sel_trials]:
-            ovl_fig = ica.plot_overlay(
-                evoked, title=f"{meeg.name}-{evoked.comment}", show=show_plots
-            )
-            overlay_figs.append(ovl_fig)
+    if len(ica.exclude) == 0:
+        print(f"No components excluded for {meeg.name}")
     else:
-        ovl_fig = ica.plot_overlay(data, title=meeg.name, show=show_plots)
-        overlay_figs.append(ovl_fig)
-
-    meeg.plot_save("ica", subfolder="overlay", matplotlib_figure=overlay_figs)
-
-    return overlay_figs
-
-
-def plot_ica_properties(meeg, show_plots):
-    ica = meeg.load_ica()
-    epochs = meeg.load_epochs()
-
-    eog_indices = meeg.load_json("eog_indices", default=list())
-    ecg_indices = meeg.load_json("ecg_indices", default=list())
-    psd_args = {"fmax": meeg.pa["lowpass"]}
-
-    if len(eog_indices) > 0:
-        eog_epochs = meeg.load_eog_epochs()
-        eog_prop_figs = ica.plot_properties(
-            eog_epochs, eog_indices, psd_args=psd_args, show=show_plots
-        )
-        meeg.plot_save(
-            "ica", subfolder="properties", trial="eog", matplotlib_figure=eog_prop_figs
-        )
-
-    if len(ecg_indices) > 0:
-        ecg_epochs = meeg.load_ecg_epochs()
-        ecg_prop_figs = ica.plot_properties(
-            ecg_epochs, ecg_indices, psd_args=psd_args, show=show_plots
-        )
-        meeg.plot_save(
-            "ica", subfolder="properties", trial="ecg", matplotlib_figure=ecg_prop_figs
-        )
-
-    remaining_indices = [
-        ix for ix in ica.exclude if ix not in eog_indices + ecg_indices
-    ]
-    if len(remaining_indices) > 0:
-        prop_figs = ica.plot_properties(
-            epochs, remaining_indices, psd_args=psd_args, show=show_plots
-        )
-        meeg.plot_save(
-            "ica", subfolder="properties", trial="manually", matplotlib_figure=prop_figs
-        )
-
-
-def plot_ica_scores(meeg, show_plots):
-    eog_scores = meeg.load_json("eog_scores", default=list())
-    if len(eog_scores) > 1:
-        ica = meeg.load_ica()
-        eog_score_fig = ica.plot_scores(
-            eog_scores, title=f"{meeg.name}: EOG", show=show_plots
-        )
-        meeg.plot_save(
-            "ica", subfolder="scores", trial="eog", matplotlib_figure=eog_score_fig
-        )
-    else:
-        eog_score_fig = None
-
-    ecg_scores = meeg.load_json("ecg_scores", default=list())
-    if len(ecg_scores) > 1:
-        ica = meeg.load_ica()
-        ecg_score_fig = ica.plot_scores(
-            ecg_scores, title=f"{meeg.name}: ECG", show=show_plots
-        )
-        meeg.plot_save(
-            "ica", subfolder="scores", trial="ecg", matplotlib_figure=ecg_score_fig
-        )
-    else:
-        ecg_score_fig = None
-
-    return eog_score_fig, ecg_score_fig
-
-
-def apply_ica(meeg, n_pca_components):
-    # Check file-parameters to make sure,
-    # that ica is not applied twice in a row
-    epochs_file = Path(meeg.epochs_path).name
-    if (
-        epochs_file in meeg.file_parameters
-        and meeg.file_parameters[epochs_file]["FUNCTION"] == "apply_ica"
-    ):
-        print(
-            f"Not applying ICA because it was already applied to this file "
-            f'on {meeg.file_parameters[epochs_file]["TIME"]}. '
-            f"If you want to apply ICA again, delete the epochs-File in "
-            "FileManagement and redo the epochs."
-        )
-    else:
-        epochs = meeg.load_epochs()
-        ica = meeg.load_ica()
-
-        if len(ica.exclude) == 0:
-            print(f"No components excluded for {meeg.name}")
-        else:
-            ica_epochs = ica.apply(epochs, n_pca_components=n_pca_components)
-            meeg.save_epochs(ica_epochs)
+        applied_data = ica.apply(data, n_pca_components=n_pca_components)
+        meeg.save(ica_apply_target, applied_data)
 
         # Apply to Empty-Room-Data as well if present
         if meeg.erm:
             try:
                 erm_data = meeg.load_erm_processed()
             except FileNotFoundError:
                 erm_data = meeg.load_erm()
             try:
-                ica.apply(erm_data, n_pca_components)
+                ica.apply(erm_data, n_pca_components=n_pca_components)
             # Todo: Unmeddling ERM-SSP and ICA stuff
             except ValueError:
                 print(
                     "There is an unresolved issue with combining SSP "
                     "from ERM and applying ICA on this ERM"
                 )
             else:
                 meeg.save_erm_processed(erm_data)
 
 
 def get_evokeds(meeg):
-    epochs = meeg.load_epochs()
-    evokeds = []
-    for trial in meeg.sel_trials:
-        evoked = epochs[trial].average()
+    meeg.load_epochs()
+    evokeds = list()
+    for trial, epoch in meeg.get_trial_epochs():
+        evoked = epoch.average()
         # Todo: optional if you want weights in your evoked.comment?!
         evoked.comment = trial
         evokeds.append(evoked)
 
     meeg.save_evokeds(evokeds)
 
 
@@ -931,20 +818,30 @@
         gfp = np.sqrt((d * d).mean(axis=0))
         gfp_dict[ch_type] = gfp
 
     return gfp_dict
 
 
 def grand_avg_evokeds(group, ga_interpolate_bads, ga_drop_bads):
-    trial_dict = {}
+    trial_dict = dict()
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
         print(f"Add {name} to grand_average")
         evokeds = meeg.load_evokeds()
         for evoked in evokeds:
+            if ga_interpolate_bads:
+                bad_evoked = evoked.copy().pick(np.arange(len(meeg.bad_channels)))
+                bad_evoked = bad_evoked.rename_channels(
+                    {
+                        old: new
+                        for old, new in zip(bad_evoked.ch_names, meeg.bad_channels)
+                    }
+                )
+                bad_evoked.info["bads"] = meeg.bad_channels
+                evoked.add_channels([bad_evoked])
             if evoked.nave != 0:
                 if evoked.comment in trial_dict:
                     trial_dict[evoked.comment].append(evoked)
                 else:
                     trial_dict.update({evoked.comment: [evoked]})
             else:
                 print(f"{evoked.comment} for {name} got nave=0")
@@ -959,14 +856,30 @@
             )
             ga.comment = trial
             ga_evokeds[trial] = ga
 
     group.save_ga_evokeds(ga_evokeds)
 
 
+def compute_psd_raw(meeg, psd_method, n_jobs, **kwargs):
+    raw = meeg.load_filtered()
+    psd_raw = raw.compute_psd(
+        method=psd_method, fmax=raw.info["lowpass"], n_jobs=n_jobs, **kwargs
+    )
+    meeg.save_psd_raw(psd_raw)
+
+
+def compute_psd_epochs(meeg, psd_method, n_jobs, **kwargs):
+    epochs = meeg.load_epochs()
+    psd_epochs = epochs.compute_psd(
+        method=psd_method, fmax=epochs.info["lowpass"], n_jobs=n_jobs, **kwargs
+    )
+    meeg.save_psd_epochs(psd_epochs)
+
+
 def tfr(
     meeg,
     tfr_freqs,
     tfr_n_cycles,
     tfr_average,
     tfr_use_fft,
     tfr_baseline,
@@ -976,48 +889,48 @@
     stockwell_width,
     n_jobs,
     **kwargs,
 ):
     powers = list()
     itcs = list()
 
-    epochs = meeg.load_epochs()
+    meeg.load_epochs()
 
     # Calculate Time-Frequency for each trial from epochs
     # using the selected method
-    for trial in meeg.sel_trials:
+    for trial, epoch in meeg.get_trial_epochs():
         if tfr_method == "multitaper":
             multitaper_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_multitaper)
             tfr_result = mne.time_frequency.tfr_multitaper(
-                epochs[trial],
+                epoch,
                 freqs=tfr_freqs,
                 n_cycles=tfr_n_cycles,
                 time_bandwidth=multitaper_bandwidth,
                 n_jobs=n_jobs,
                 use_fft=tfr_use_fft,
                 return_itc=tfr_average,
                 average=tfr_average,
                 **multitaper_kwargs,
             )
         elif tfr_method == "stockwell":
             fmin, fmax = tfr_freqs[[0, -1]]
             stockwell_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_stockwell)
             tfr_result = mne.time_frequency.tfr_stockwell(
-                epochs[trial],
+                epoch,
                 fmin=fmin,
                 fmax=fmax,
                 width=stockwell_width,
                 n_jobs=n_jobs,
                 return_itc=True,
                 **stockwell_kwargs,
             )
         else:
             morlet_kwargs = check_kwargs(kwargs, mne.time_frequency.tfr_morlet)
             tfr_result = mne.time_frequency.tfr_morlet(
-                epochs[trial],
+                epoch,
                 freqs=tfr_freqs,
                 n_cycles=tfr_n_cycles,
                 n_jobs=n_jobs,
                 use_fft=tfr_use_fft,
                 return_itc=tfr_average,
                 average=tfr_average,
                 **morlet_kwargs,
@@ -1082,15 +995,15 @@
             for pw in trial_dict[trial]:
                 if len(commons) == 0:
                     for c in pw.ch_names:
                         commons.add(c)
                 commons = commons & set(pw.ch_names)
             print(f"{trial}:Reducing all n_channels to {len(commons)}")
             for idx, pw in enumerate(trial_dict[trial]):
-                trial_dict[trial][idx] = pw.pick_channels(list(commons))
+                trial_dict[trial][idx] = pw.pick(list(commons))
 
             ga = mne.grand_average(
                 trial_dict[trial], interpolate_bads=True, drop_bads=True
             )
             ga.comment = trial
             ga_dict[trial] = ga
 
@@ -1216,16 +1129,15 @@
         + "Bash output follows below.\n\n"
     )
 
     command = [
         "mne",
         "make_scalp_surfaces",
         "--overwrite",
-        "--subject",
-        fsmri.name,
+        f"--subject={fsmri.name}",
         "--force",
     ]
 
     run_freesurfer_subprocess(
         command, fsmri.subjects_dir, fsmri.fs_path, fsmri.mne_path
     )
 
@@ -1273,23 +1185,25 @@
     bem_solution = mne.make_bem_solution(bem_model)
     fsmri.save_bem_solution(bem_solution)
 
 
 def morph_fsmri(meeg, morph_to):
     if meeg.fsmri.name != morph_to:
         forward = meeg.load_forward()
+        fsmri_to = FSMRI(morph_to, meeg.ct)
         morph = mne.compute_source_morph(
             forward["src"],
             subject_from=meeg.fsmri.name,
             subject_to=morph_to,
             subjects_dir=meeg.subjects_dir,
+            src_to=fsmri_to.load_source_space(),
         )
         meeg.save_source_morph(morph)
     else:
-        logging.info(
+        logger().info(
             f"There is no need to morph the source-space for {meeg.name}, "
             f'because the morph-destination "{morph_to}" '
             f"is the same as the associated FSMRI."
         )
 
 
 def morph_labels_from_fsaverage(fsmri):
@@ -1391,33 +1305,38 @@
     meeg.save_inverse_operator(inverse_operator)
 
 
 def source_estimate(meeg, inverse_method, pick_ori, lambda2):
     inverse_operator = meeg.load_inverse_operator()
     evokeds = meeg.load_evokeds()
 
-    stcs = {}
+    stcs = dict()
     for evoked in [ev for ev in evokeds if ev.comment in meeg.sel_trials]:
         stc = mne.minimum_norm.apply_inverse(
             evoked, inverse_operator, lambda2, method=inverse_method, pick_ori=pick_ori
         )
         stcs.update({evoked.comment: stc})
 
     meeg.save_source_estimates(stcs)
 
 
 def label_time_course(meeg, target_labels, extract_mode):
+    if len(target_labels) == 0:
+        raise RuntimeError(
+            "No labels selected for label time course extraction. "
+            "Please select at least one label."
+        )
     stcs = meeg.load_source_estimates()
     src = meeg.fsmri.load_source_space()
     labels = meeg.fsmri.get_labels(target_labels)
 
-    ltc_dict = {}
+    ltc_dict = dict()
 
     for trial in stcs:
-        ltc_dict[trial] = {}
+        ltc_dict[trial] = dict()
         times = stcs[trial].times
         for label in labels:
             ltc = stcs[trial].extract_label_time_course(label, src, mode=extract_mode)[
                 0
             ]
             ltc_dict[trial][label.name] = np.vstack((ltc, times))
 
@@ -1442,16 +1361,16 @@
         lambda2 = 1.0 / snr**2
         for evoked in evokeds:
             trial = evoked.comment
             stcs[trial] = mne.minimum_norm.apply_inverse(
                 evoked, inv_op, lambda2, method="dSPM"
             )
 
-    mixn_dips = {}
-    mixn_stcs = {}
+    mixn_dips = dict()
+    mixn_stcs = dict()
 
     for evoked in [ev for ev in evokeds if ev.comment in meeg.sel_trials]:
         alpha = 30  # regularization parameter between 0 and 100 (100 is high)
         n_mxne_iter = 10  # if > 1 use L0.5/L2 reweighted mixed norm solver
         # if n_mxne_iter > 1 dSPM weighting can be avoided.
         trial = evoked.comment
         mixn_dipoles, dip_residual = mne.inverse_sparse.mixed_norm(
@@ -1506,19 +1425,19 @@
         )
 
     evokeds = meeg.load_evokeds()
     noise_covariance = meeg.load_noise_covariance()
     bem = meeg.fsmri.load_bem_solution()
     trans = meeg.load_transformation()
 
-    ecd_dips = {}
+    ecd_dips = dict()
 
     for evoked in evokeds:
         trial = evoked.comment
-        ecd_dips[trial] = {}
+        ecd_dips[trial] = dict()
         for dip in ecd_time:
             tmin, tmax = ecd_time[dip]
             copy_evoked = evoked.copy().crop(tmin, tmax)
 
             try:
                 ecd_position = ecd_positions[meeg.name][dip]
                 ecd_orientation = ecd_orientations[meeg.name][dip]
@@ -1558,46 +1477,65 @@
 
 
 def apply_morph(meeg, morph_to):
     if meeg.fsmri.name != morph_to:
         stcs = meeg.load_source_estimates()
         morph = meeg.load_source_morph()
 
-        morphed_stcs = {}
+        morphed_stcs = dict()
         for trial in stcs:
             morphed_stcs[trial] = morph.apply(stcs[trial])
         meeg.save_morphed_source_estimates(morphed_stcs)
     else:
-        logging.info(
+        logger().info(
             f"{meeg.name} is already in source-space of {morph_to} "
             f"and won't be morphed"
         )
 
 
 def src_connectivity(
     meeg,
     target_labels,
     inverse_method,
     lambda2,
     con_methods,
     con_fmin,
     con_fmax,
+    con_time_window,
     n_jobs,
 ):
+    if len(target_labels) == 0:
+        raise RuntimeError(
+            "No labels selected for connectivity estimation. "
+            "Please select at least one label."
+        )
     info = meeg.load_info()
-    all_epochs = meeg.load_epochs()
     inverse_operator = meeg.load_inverse_operator()
     src = inverse_operator["src"]
     labels = meeg.fsmri.get_labels(target_labels)
 
-    con_dict = {}
+    if len(labels) == 0:
+        raise RuntimeError("No labels found, check your target_labels")
+    if len(meeg.sel_trials) == 0:
+        raise RuntimeError(
+            "No trials selected, check your Selected IDs in Preparation/"
+        )
+
+    con_dict = dict()
+
+    for trial, epoch in meeg.get_trial_epochs():
+        con_dict[trial] = dict()
+        epochs = epoch
+
+        # Crop if necessary
+        if con_time_window is not None:
+            epochs = epochs.copy().crop(
+                tmin=con_time_window[0], tmax=con_time_window[1]
+            )
 
-    for trial in [t for t in all_epochs.event_id if t]:
-        con_dict[trial.split("/")[0]] = {}
-        epochs = all_epochs[trial.split("/")[0]]
         # Compute inverse solution and for each epoch.
         # By using "return_generator=True" stcs will be a generator object
         # instead of a list.
         stcs = mne.minimum_norm.apply_inverse_epochs(
             epochs,
             inverse_operator,
             lambda2,
@@ -1609,14 +1547,15 @@
         label_ts = mne.extract_label_time_course(
             stcs, labels, src, mode="mean_flip", return_generator=True
         )
 
         sfreq = info["sfreq"]  # the sampling frequency
         con = mne_connectivity.spectral_connectivity_epochs(
             label_ts,
+            names=target_labels,
             method=con_methods,
             mode="multitaper",
             sfreq=sfreq,
             fmin=con_fmin,
             fmax=con_fmax,
             faverage=True,
             mt_adaptive=True,
@@ -1625,74 +1564,27 @@
 
         if not isinstance(con, list):
             con = [con]
 
         # con is a 3D array, get the connectivity for the first (and only)
         # freq. band for each con_method
         for method, c in zip(con_methods, con):
-            con_dict[trial.split("/")[0]][method] = c.get_data(output="dense")[:, :, 0]
-
-    meeg.save_connectivity(con_dict)
-
-    for trial in all_epochs.event_id:
-        con_dict[trial.split("/")[1]] = {}
-        # epochs = all_epochs[trial.split('/')[1]][:2]
-        epochs = all_epochs[trial.split("/")[1]]
-        # Compute inverse solution and for each epoch.
-        # By using "return_generator=True" stcs will be a generator object
-        # instead of a list.
-        stcs = mne.minimum_norm.apply_inverse_epochs(
-            epochs,
-            inverse_operator,
-            lambda2,
-            inverse_method,
-            pick_ori="normal",
-            return_generator=True,
-        )
-
-        # Average the source estimates within each label using
-        # sign-flips to reduce signal cancellations, also here we return a
-        # generator
-
-        label_ts = mne.extract_label_time_course(
-            stcs, labels, src, mode="mean_flip", return_generator=True
-        )
-
-        sfreq = info["sfreq"]  # the sampling frequency
-        con = mne_connectivity.spectral_connectivity(
-            label_ts,
-            method=con_methods,
-            mode="multitaper",
-            sfreq=sfreq,
-            fmin=con_fmin,
-            fmax=con_fmax,
-            faverage=True,
-            mt_adaptive=True,
-            n_jobs=n_jobs,
-        )
-
-        if not isinstance(con, list):
-            con = [con]
-
-        # con is a 3D array, get the connectivity for the first
-        # (and only) freq. band for each con_method
-        for method, c in zip(con_methods, con):
-            con_dict[trial.split("/")[1]][method] = c.get_data(output="dense")[:, :, 0]
+            con_dict[trial][method] = c
 
     meeg.save_connectivity(con_dict)
 
 
 def grand_avg_morphed(group, morph_to):
     # for less memory only import data from stcs and add it to one
     # stc in the end!!!
     n_chunks = 8
     # divide in chunks to save memory
-    fusion_dict = {}
+    fusion_dict = dict()
     for i in range(0, len(group.group_list), n_chunks):
-        sub_trial_dict = {}
+        sub_trial_dict = dict()
         ga_chunk = group.group_list[i : i + n_chunks]
         print(ga_chunk)
         for name in ga_chunk:
             meeg = MEEG(name, group.ct)
             print(f"Add {name} to grand_average")
             if morph_to == meeg.fsmri.name:
                 stcs = meeg.load_source_estimates()
@@ -1718,15 +1610,15 @@
                 sub_trial_average.data /= n_subjects
                 sub_trial_average.comment = trial
                 if trial in fusion_dict:
                     fusion_dict[trial].append(sub_trial_average)
                 else:
                     fusion_dict.update({trial: [sub_trial_average]})
 
-    ga_stcs = {}
+    ga_stcs = dict()
     for trial in fusion_dict:
         if len(fusion_dict[trial]) != 0:
             print(f"grand_average for {group.name}-{trial}")
             trial_average = fusion_dict[trial][0].copy()
             n_subjects = len(fusion_dict[trial])
 
             for trial_index in range(1, n_subjects):
@@ -1737,89 +1629,82 @@
 
             ga_stcs[trial] = trial_average
 
     group.save_ga_stc(ga_stcs)
 
 
 def grand_avg_ltc(group):
-    ltc_average_dict = {}
+    ltc_average_dict = dict()
     times = None
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
         print(f"Add {name} to grand_average")
         ltc_dict = meeg.load_ltc()
         for trial in ltc_dict:
             if trial not in ltc_average_dict:
-                ltc_average_dict[trial] = {}
+                ltc_average_dict[trial] = dict()
             for label in ltc_dict[trial]:
                 # First row of array is label-time-course-data,
                 # second row is time-array
                 if label in ltc_average_dict[trial]:
                     ltc_average_dict[trial][label].append(ltc_dict[trial][label][0])
                 else:
                     ltc_average_dict[trial][label] = [ltc_dict[trial][label][0]]
                 # Should be the same for each trial and label
                 times = ltc_dict[trial][label][1]
 
-    ga_ltc = {}
+    ga_ltc = dict()
     for trial in ltc_average_dict:
-        ga_ltc[trial] = {}
+        ga_ltc[trial] = dict()
         for label in ltc_average_dict[trial]:
             if len(ltc_average_dict[trial][label]) != 0:
                 print(f"grand_average for {trial}-{label}")
                 ltc_list = ltc_average_dict[trial][label]
-                # Take the absolute values
-                ltc_list = [abs(it) for it in ltc_list]
-                n_subjects = len(ltc_list)
-                average = ltc_list[0]
-                for idx in range(1, n_subjects):
-                    average += ltc_list[idx]
-
-                average /= n_subjects
+                average = np.mean(ltc_list, axis=0)
 
                 ga_ltc[trial][label] = np.vstack((average, times))
 
     group.save_ga_ltc(ga_ltc)
 
 
 def grand_avg_connect(group):
     # Prepare the Average-Dict
-    con_average_dict = {}
+    con_average_dict = dict()
     for name in group.group_list:
         meeg = MEEG(name, group.ct)
         print(f"Add {name} to grand_average")
         con_dict = meeg.load_connectivity()
         for trial in con_dict:
             if trial not in con_average_dict:
-                con_average_dict[trial] = {}
-            for con_method in con_dict[trial]:
-                if con_method in con_average_dict[trial]:
-                    con_average_dict[trial][con_method].append(
-                        con_dict[trial][con_method]
-                    )
-                else:
-                    con_average_dict[trial][con_method] = [con_dict[trial][con_method]]
+                con_average_dict[trial] = dict()
+            for con_method, con in con_dict[trial].items():
+                if con_method not in con_average_dict[trial]:
+                    con_average_dict[trial][con_method] = list()
+                con_average_dict[trial][con_method].append(con)
 
-    ga_con = {}
+    ga_con_dict = dict()
     for trial in con_average_dict:
-        ga_con[trial] = {}
-        for con_method in con_average_dict[trial]:
-            if len(con_average_dict[trial][con_method]) != 0:
+        ga_con_dict[trial] = dict()
+        for con_method, con_list in con_average_dict[trial].items():
+            if len(con_list) != 0:
                 print(f"grand_average for {trial}-{con_method}")
-                con_list = con_average_dict[trial][con_method]
-                n_subjects = len(con_list)
-                average = con_list[0]
-                for idx in range(1, n_subjects):
-                    average += con_list[idx]
+                avg_data = np.mean([con.get_data() for con in con_list], axis=0)
 
-                average /= n_subjects
-
-                ga_con[trial][con_method] = average
+                ga_con = SpectralConnectivity(
+                    data=avg_data,
+                    freqs=con_list[0].freqs,
+                    n_nodes=con_list[0].n_nodes,
+                    names=con_list[0].names,
+                    indices=con_list[0].indices,
+                    method=con_list[0].method,
+                    n_epochs_used=len(con_list),
+                )
+                ga_con_dict[trial][con_method] = ga_con
 
-    group.save_ga_con(ga_con)
+    group.save_ga_con(ga_con_dict)
 
 
 def print_info(meeg):
     print(meeg.load_info())
     for n in range(20):
         print(f"\r{n}", end="")
         time.sleep(0.1)
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/functions/plot.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/functions/plot.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,281 +3,338 @@
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from __future__ import print_function
 
-import gc
-import multiprocessing
+import itertools
+from functools import partial
 from os.path import join
 
 import matplotlib.pyplot as plt
 import mne
 import mne_connectivity
 import numpy as np
 
 # Make use of program also possible with sensor-space installation of mne
-from mne_pipeline_hd.pipeline.loading import FSMRI
+from mne_pipeline_hd.pipeline.loading import MEEG
 from mne_pipeline_hd.pipeline.plot_utils import pipeline_plot
 
 try:
     from nilearn.plotting import plot_anat
 except (ModuleNotFoundError, ValueError):
     pass
 
 from mne_pipeline_hd.functions import operations as op
 
 
 # ==============================================================================
 # PLOTTING FUNCTIONS
 # ==============================================================================
+def _save_raw_on_close(_, meeg, raw, raw_type):
+    # Save bad-channels
+    meeg.set_bad_channels(raw.info["bads"])
+    # Save raw for annotations
+    meeg.save(raw_type, raw)
 
-def plot_raw(meeg, show_plots):
+
+def plot_raw(meeg, show_plots, close_func=_save_raw_on_close, **kwargs):
     raw = meeg.load_raw()
 
     try:
         events = meeg.load_events()
     except FileNotFoundError:
         events = None
-        print('No events found')
+        print("No events found")
 
-    raw.plot(events=events, n_channels=30, bad_color='red', scalings='auto',
-             title=f'{meeg.name}', show=show_plots)
+    fig = raw.plot(
+        events=events,
+        bad_color="red",
+        scalings="auto",
+        title=f"{meeg.name}",
+        show=show_plots,
+        **kwargs,
+    )
+
+    if hasattr(fig, "canvas"):
+        # Connect to closing of Matplotlib-Figure
+        fig.canvas.mpl_connect(
+            "close_event",
+            partial(close_func, meeg=meeg, raw=raw, raw_type="raw"),
+        )
+    else:
+        # Connect to closing of PyQt-Figure
+        fig.gotClosed.connect(
+            partial(close_func, None, meeg=meeg, raw=raw, raw_type="raw")
+        )
 
 
-def plot_filtered(meeg, show_plots):
+def plot_filtered(meeg, show_plots, close_func=_save_raw_on_close, **kwargs):
     raw = meeg.load_filtered()
 
     try:
         events = meeg.load_events()
     except FileNotFoundError:
         events = None
-        print('No events found')
+        print("No events found")
 
-    raw.plot(events=events, n_channels=30, bad_color='red',
-             scalings=dict(mag=1e-12, grad=4e-11, eeg=20e-5, stim=1),
-             title=f'{meeg.name} highpass={meeg.pa["highpass"]} '
-                   f'lowpass={meeg.pa["lowpass"]}',
-             show=show_plots)
+    raw.plot(
+        events=events,
+        bad_color="red",
+        scalings="auto",
+        title=f'{meeg.name} highpass={meeg.pa["highpass"]} '
+        f'lowpass={meeg.pa["lowpass"]}',
+        show=show_plots,
+        **kwargs,
+    )
 
 
 def plot_sensors(meeg, plot_sensors_kind, ch_types, show_plots):
     loaded_info = meeg.load_info()
     if len(ch_types) > 1:
-        ch_types = 'all'
+        ch_types = "all"
     elif len(ch_types) == 1:
         ch_types = ch_types[0]
     else:
         ch_types = None
-    mne.viz.plot_sensors(loaded_info, kind=plot_sensors_kind, ch_type=ch_types,
-                         title=meeg.name, show_names=True,
-                         show=show_plots)
+    mne.viz.plot_sensors(
+        loaded_info,
+        kind=plot_sensors_kind,
+        ch_type=ch_types,
+        title=meeg.name,
+        show_names=True,
+        show=show_plots,
+    )
 
 
 @pipeline_plot
 def plot_events(meeg, show_plots):
     events = meeg.load_events()
 
     fig = mne.viz.plot_events(events, event_id=meeg.event_id, show=show_plots)
     fig.suptitle(meeg.name)
 
-    meeg.plot_save('events', matplotlib_figure=fig)
+    meeg.plot_save("events", matplotlib_figure=fig)
 
     return fig
 
 
-def plot_power_spectra(meeg, show_plots, n_jobs):
-    raw = meeg.load_filtered()
-
-    # Does not accept -1 for n_jobs
-    if n_jobs == -1:
-        n_jobs = multiprocessing.cpu_count()
-
-    fig = raw.plot_psd(fmax=raw.info['lowpass'], show=show_plots,
-                       n_jobs=n_jobs)
-    fig.suptitle(meeg.name)
-
-    meeg.plot_save('power_spectra', subfolder='raw', matplotlib_figure=fig)
+def plot_power_spectra(meeg, show_plots):
+    psd = meeg.load_psd_raw()
+    fig = psd.plot(show=show_plots)
+    fig.suptitle(f"Raw: {meeg.name}", x=0.3)
 
+    meeg.plot_save("power_spectra", subfolder="raw", matplotlib_figure=fig)
 
-def plot_power_spectra_topo(meeg, show_plots, n_jobs):
-    raw = meeg.load_filtered()
 
-    # Does not accept -1 for n_jobs
-    if n_jobs == -1:
-        n_jobs = multiprocessing.cpu_count()
+def plot_power_spectra_topomap(meeg, psd_topomap_bands, show_plots):
+    psd = meeg.load_psd_raw()
+    fig = psd.plot_topomap(badns=psd_topomap_bands, show=show_plots)
+    fig.suptitle(f"Raw: {meeg.name}", x=0.3)
 
-    fig = raw.plot_psd_topo(show=show_plots, n_jobs=n_jobs)
+    meeg.plot_save("power_spectra", subfolder="raw_topo", matplotlib_figure=fig)
 
-    meeg.plot_save('power_spectra', subfolder='raw_topo',
-                   matplotlib_figure=fig)
-
-
-def plot_power_spectra_epochs(meeg, show_plots, n_jobs):
-    epochs = meeg.load_epochs()
-
-    # Does not accept -1 for n_jobs
-    if n_jobs == -1:
-        n_jobs = multiprocessing.cpu_count()
 
+def plot_power_spectra_epochs(meeg, show_plots):
+    psd = meeg.load_psd_epochs()
     for trial in meeg.sel_trials:
-        fig = epochs[trial].plot_psd(show=show_plots, n_jobs=n_jobs)
-        fig.suptitle(meeg.name + '-' + trial)
-        meeg.plot_save('power_spectra', subfolder='epochs', trial=trial,
-                       matplotlib_figure=fig)
+        fig = psd[trial].plot(show=show_plots)
+        fig.suptitle(f"Epochs: {meeg.name}-{trial}", x=0.3)
+        meeg.plot_save(
+            "power_spectra", subfolder="epochs", trial=trial, matplotlib_figure=fig
+        )
 
 
-def plot_power_spectra_epochs_topo(meeg, show_plots, n_jobs):
-    epochs = meeg.load_epochs()
+def plot_power_spectra_epochs_topomap(meeg, psd_topomap_bands, show_plots):
+    psd = meeg.load_psd_epochs()
     for trial in meeg.sel_trials:
-        fig = epochs[trial].plot_psd_topomap(show=show_plots, n_jobs=n_jobs)
-        fig.suptitle(meeg.name + '-' + trial)
-        meeg.plot_save('power_spectra', subfolder='epochs_topo', trial=trial,
-                       matplotlib_figure=fig)
+        fig = psd[trial].plot_topomap(bands=psd_topomap_bands, show=show_plots)
+        fig.suptitle(f"Epochs: {meeg.name}-{trial}")
+        meeg.plot_save(
+            "power_spectra", subfolder="epochs_topo", trial=trial, matplotlib_figure=fig
+        )
 
 
 def plot_tfr(meeg, show_plots):
     powers = meeg.load_power_tfr_average()
 
     for power in powers:
-        print('Plotting TFR')
-        fig1 = power.plot(title=f'{meeg.name}-{power.comment}', combine='mean',
-                          show=show_plots)
-        print('Plotting TFR-Topo')
-        fig2 = power.plot_topo(title=f'{meeg.name}-{power.comment}',
-                               show=show_plots)
-        print('Plotting TFR-Joint')
-        fig3 = power.plot_joint(title=f'{meeg.name}-{power.comment}',
-                                show=show_plots)
-        print('Plotting TFR-Topomap')
-        fig4 = power.plot_topomap(title=f'{meeg.name}-{power.comment}',
-                                  show=show_plots)
-
-        meeg.plot_save('time_frequency', subfolder='plot', trial=power.comment,
-                       matplotlib_figure=fig1)
-        meeg.plot_save('time_frequency', subfolder='topo', trial=power.comment,
-                       matplotlib_figure=fig2)
-        meeg.plot_save('time_frequency', subfolder='joint',
-                       trial=power.comment, matplotlib_figure=fig3)
-        meeg.plot_save('time_frequency', subfolder='topomap',
-                       trial=power.comment, matplotlib_figure=fig4)
+        print("Plotting TFR")
+        fig1 = power.plot(
+            title=f"{meeg.name}-{power.comment}", combine="mean", show=show_plots
+        )
+        print("Plotting TFR-Topo")
+        fig2 = power.plot_topo(title=f"{meeg.name}-{power.comment}", show=show_plots)
+        print("Plotting TFR-Joint")
+        fig3 = power.plot_joint(title=f"{meeg.name}-{power.comment}", show=show_plots)
+        print("Plotting TFR-Topomap")
+        fig4 = power.plot_topomap(show=show_plots)
+
+        meeg.plot_save(
+            "time_frequency",
+            subfolder="plot",
+            trial=power.comment,
+            matplotlib_figure=fig1,
+        )
+        meeg.plot_save(
+            "time_frequency",
+            subfolder="topo",
+            trial=power.comment,
+            matplotlib_figure=fig2,
+        )
+        meeg.plot_save(
+            "time_frequency",
+            subfolder="joint",
+            trial=power.comment,
+            matplotlib_figure=fig3,
+        )
+        meeg.plot_save(
+            "time_frequency",
+            subfolder="topomap",
+            trial=power.comment,
+            matplotlib_figure=fig4,
+        )
 
     try:
         itcs = meeg.load_itc_tfr_average()
     except (FileNotFoundError, UnboundLocalError):
-        print(f'{meeg.itc_tfr_average_path} not found!')
+        print(f"{meeg.itc_tfr_average_path} not found!")
     else:
         for itc in itcs:
-            fig5 = itc.plot_topo(title=f'{meeg.name}-{itc.comment}-itc',
-                                 vmin=0., vmax=1., cmap='Reds',
-                                 show=show_plots)
-            meeg.plot_save('time_frequency', subfolder='itc',
-                           trial=itc.comment, matplotlib_figure=fig5)
+            fig5 = itc.plot(
+                title=f"{meeg.name}-{itc.comment}-itc",
+                combine="mean",
+                show=show_plots,
+            )
+            meeg.plot_save(
+                "time_frequency",
+                subfolder="itc",
+                trial=itc.comment,
+                matplotlib_figure=fig5,
+            )
 
 
 def plot_epochs(meeg, show_plots):
     epochs = meeg.load_epochs()
 
     for trial in meeg.sel_trials:
-        fig = mne.viz.plot_epochs(epochs[trial], title=meeg.name,
-                                  show=show_plots)
+        fig = mne.viz.plot_epochs(epochs[trial], title=meeg.name, show=show_plots)
         fig.suptitle(trial)
 
 
 def plot_epochs_image(meeg, show_plots):
     epochs = meeg.load_epochs()
     for trial in meeg.sel_trials:
-        figures = mne.viz.plot_epochs_image(epochs[trial],
-                                            title=meeg.name + '_' + trial,
-                                            show=show_plots)
+        figures = mne.viz.plot_epochs_image(
+            epochs[trial], title=meeg.name + "_" + trial, show=show_plots
+        )
 
         for idx, fig in enumerate(figures):
-            meeg.plot_save('epochs', subfolder='image', trial=trial, idx=idx,
-                           matplotlib_figure=fig)
+            meeg.plot_save(
+                "epochs", subfolder="image", trial=trial, idx=idx, matplotlib_figure=fig
+            )
 
 
 def plot_epochs_topo(meeg, show_plots):
     epochs = meeg.load_epochs()
     for trial in meeg.sel_trials:
-        fig = mne.viz.plot_topo_image_epochs(epochs, title=meeg.name,
-                                             show=show_plots)
+        fig = mne.viz.plot_topo_image_epochs(epochs, title=meeg.name, show=show_plots)
 
-        meeg.plot_save('epochs', subfolder='topo', trial=trial,
-                       matplotlib_figure=fig)
+        meeg.plot_save("epochs", subfolder="topo", trial=trial, matplotlib_figure=fig)
 
 
 def plot_epochs_drop_log(meeg, show_plots):
     epochs = meeg.load_epochs()
     fig = epochs.plot_drop_log(subject=meeg.name, show=show_plots)
 
-    meeg.plot_save('epochs', subfolder='drop_log', matplotlib_figure=fig)
+    meeg.plot_save("epochs", subfolder="drop_log", matplotlib_figure=fig)
 
 
 def plot_autoreject_log(meeg, show_plots):
     reject_log = meeg.load_reject_log()
     epochs = meeg.load_epochs()
 
     fig1 = reject_log.plot(show=show_plots)
-    meeg.plot_save('epochs', subfolder='autoreject_log', idx='reject',
-                   matplotlib_figure=fig1)
+    meeg.plot_save(
+        "epochs", subfolder="autoreject_log", idx="reject", matplotlib_figure=fig1
+    )
     try:
         fig2 = reject_log.plot_epochs(epochs)
-        meeg.plot_save('epochs', subfolder='autoreject_log', idx='epochs',
-                       matplotlib_figure=fig2)
+        meeg.plot_save(
+            "epochs", subfolder="autoreject_log", idx="epochs", matplotlib_figure=fig2
+        )
     except ValueError:
-        print(f'{meeg.name}: No epochs-plot for autoreject-log')
+        print(f"{meeg.name}: No epochs-plot for autoreject-log")
 
 
 def plot_evoked_topo(meeg, show_plots):
     evokeds = meeg.load_evokeds()
     fig = mne.viz.plot_evoked_topo(evokeds, title=meeg.name, show=show_plots)
 
-    meeg.plot_save('evokeds', subfolder='topo', matplotlib_figure=fig, dpi=800)
+    meeg.plot_save("evokeds", subfolder="topo", matplotlib_figure=fig, dpi=800)
 
 
 def plot_evoked_topomap(meeg, show_plots):
     evokeds = meeg.load_evokeds()
     for evoked in evokeds:
         fig = mne.viz.plot_evoked_topomap(
-            evoked, times='auto', title=meeg.name + '-' + evoked.comment,
-            show=show_plots)
-
-        meeg.plot_save('evokeds', subfolder='topomap', trial=evoked.comment,
-                       matplotlib_figure=fig)
+            evoked,
+            times="auto",
+            title=meeg.name + "-" + evoked.comment,
+            show=show_plots,
+        )
+
+        meeg.plot_save(
+            "evokeds", subfolder="topomap", trial=evoked.comment, matplotlib_figure=fig
+        )
 
 
 def plot_evoked_joint(meeg, show_plots):
     evokeds = meeg.load_evokeds()
 
     for evoked in evokeds:
         fig = mne.viz.plot_evoked_joint(
-            evoked, times='peaks', title=meeg.name + ' - ' + evoked.comment,
-            show=show_plots)
-
-        meeg.plot_save('evokeds', subfolder='joint', trial=evoked.comment,
-                       matplotlib_figure=fig)
+            evoked,
+            times="peaks",
+            title=meeg.name + " - " + evoked.comment,
+            show=show_plots,
+        )
+
+        meeg.plot_save(
+            "evokeds", subfolder="joint", trial=evoked.comment, matplotlib_figure=fig
+        )
 
 
 @pipeline_plot
 def plot_evoked_butterfly(meeg, apply_proj, show_plots):
     evokeds = meeg.load_evokeds()
     figs = list()
     for evoked in evokeds:
-        titles_dict = {cht: f'{cht}: {meeg.name}-{evoked.comment}'
-                       for cht in evoked.get_channel_types(unique=True,
-                                                           only_data_chs=True)}
-        fig = evoked.plot(spatial_colors=True, proj=apply_proj,
-                          titles=titles_dict,
-                          window_title=meeg.name + ' - ' + evoked.comment,
-                          selectable=True, gfp=True, zorder='std',
-                          show=show_plots)
+        titles_dict = {
+            cht: f"{cht}: {meeg.name}-{evoked.comment}"
+            for cht in evoked.get_channel_types(unique=True, only_data_chs=True)
+        }
+        fig = evoked.plot(
+            spatial_colors=True,
+            proj=apply_proj,
+            titles=titles_dict,
+            window_title=meeg.name + " - " + evoked.comment,
+            selectable=True,
+            gfp=True,
+            zorder="std",
+            show=show_plots,
+        )
         figs.append(fig)
-        meeg.plot_save('evokeds', subfolder='butterfly', trial=evoked.comment,
-                       matplotlib_figure=fig)
+        meeg.plot_save(
+            "evokeds",
+            subfolder="butterfly",
+            trial=evoked.comment,
+            matplotlib_figure=fig,
+        )
 
     return figs
 
 
 def plot_evoked_white(meeg, show_plots):
     evokeds = meeg.load_evokeds()
     noise_covariance = meeg.load_noise_covariance()
@@ -285,479 +342,781 @@
     for evoked in evokeds:
         # Check, if evokeds and noise covariance got the same channels
         channels = set(evoked.ch_names) & set(noise_covariance.ch_names)
         evoked.pick_channels(channels)
         noise_covariance.pick_channels(channels)
 
         fig = evoked.plot_white(noise_covariance, show=show_plots)
-        fig.suptitle(meeg.name + ' - ' + evoked.comment,
-                     horizontalalignment='center')
+        fig.suptitle(meeg.name + " - " + evoked.comment, horizontalalignment="center")
 
-        meeg.plot_save('evokeds', subfolder='white', trial=evoked.comment,
-                       matplotlib_figure=fig)
+        meeg.plot_save(
+            "evokeds", subfolder="white", trial=evoked.comment, matplotlib_figure=fig
+        )
 
 
 def plot_evoked_image(meeg, show_plots):
     evokeds = meeg.load_evokeds()
 
     for evoked in evokeds:
         fig = evoked.plot_image(show=show_plots)
-        fig.suptitle(meeg.name + ' - ' + evoked.comment,
-                     horizontalalignment='center')
+        fig.suptitle(meeg.name + " - " + evoked.comment, horizontalalignment="center")
 
-        meeg.plot_save('evokeds', subfolder='image', trial=evoked.comment,
-                       matplotlib_figure=fig)
+        meeg.plot_save(
+            "evokeds", subfolder="image", trial=evoked.comment, matplotlib_figure=fig
+        )
 
 
 def plot_compare_evokeds(meeg, show_plots):
     evokeds = meeg.load_evokeds()
 
-    evokeds = {evoked.comment: evoked for evoked in evokeds}
+    evokeds = {f"{evoked.comment}={evoked.nave}": evoked for evoked in evokeds}
 
     fig = mne.viz.plot_compare_evokeds(evokeds, show=show_plots)
 
-    meeg.plot_save('evokeds', subfolder='compare', matplotlib_figure=fig)
+    meeg.plot_save("evokeds", subfolder="compare", matplotlib_figure=fig)
 
 
 def plot_gfp(meeg, show_plots):
     evokeds = meeg.load_evokeds()
     for evoked in evokeds:
         gfp_dict = op.calculate_gfp(evoked)
         t = evoked.times
         trial = evoked.comment
 
         fig, ax = plt.subplots(len(gfp_dict), 1)
         for idx, ch_type in enumerate(gfp_dict):
             gfp = gfp_dict[ch_type]
             ax[idx].plot(t, gfp)
-            ax[idx].set_title(f'GFP of {meeg.name}-{trial}-{ch_type}')
+            ax[idx].set_title(f"GFP of {meeg.name}-{trial}-{ch_type}")
 
         if show_plots:
             fig.show()
 
-        meeg.plot_save('evokeds', subfolder='gfp', trial=trial,
-                       matplotlib_figure=fig)
+        meeg.plot_save("evokeds", subfolder="gfp", trial=trial, matplotlib_figure=fig)
 
 
-def plot_transformation(meeg):
+def _save_ica_on_close(_, meeg, ica):
+    meeg.set_ica_exclude(ica.exclude)
+    meeg.save_ica(ica)
+
+
+def plot_ica_components(meeg, show_plots, close_func=_save_ica_on_close):
+    ica = meeg.load_ica()
+    figs = ica.plot_components(title=meeg.name, show=show_plots)
+    if not isinstance(figs, list):
+        figs = [figs]
+    figs[0].canvas.mpl_connect("close_event", partial(close_func, meeg=meeg, ica=ica))
+    meeg.plot_save("ica", subfolder="components", matplotlib_figure=figs)
+
+
+def plot_ica_sources(meeg, ica_source_data, show_plots, close_func=_save_ica_on_close):
+    ica = meeg.load_ica()
+    data = meeg.load(ica_source_data)
+
+    fig = ica.plot_sources(data, title=meeg.name, show=show_plots)
+    if hasattr(fig, "canvas"):
+        # Connect to closing of Matplotlib-Figure
+        fig.canvas.mpl_connect("close_event", partial(close_func, meeg=meeg, ica=ica))
+        # Save plot as image
+        meeg.plot_save("ica", subfolder="sources", matplotlib_figure=fig)
+    else:
+        # Connect to closing of PyQt-Figure
+        fig.gotClosed.connect(partial(close_func, None, meeg=meeg, ica=ica))
+
+
+def plot_ica_overlay(meeg, ica_overlay_data, show_plots):
+    ica = meeg.load_ica()
+    data = meeg.load(ica_overlay_data)
+
+    overlay_figs = list()
+
+    if ica_overlay_data == "evoked":
+        for evoked in [e for e in data if e.comment in meeg.sel_trials]:
+            ovl_fig = ica.plot_overlay(
+                evoked, title=f"{meeg.name}-{evoked.comment}", show=show_plots
+            )
+            overlay_figs.append(ovl_fig)
+    else:
+        ovl_fig = ica.plot_overlay(data, title=meeg.name, show=show_plots)
+        overlay_figs.append(ovl_fig)
+
+    meeg.plot_save("ica", subfolder="overlay", matplotlib_figure=overlay_figs)
+
+    return overlay_figs
+
+
+def plot_ica_properties(meeg, ica_fitto, show_plots):
+    ica = meeg.load_ica()
+
+    eog_indices = meeg.load_json("eog_indices", default=list())
+    ecg_indices = meeg.load_json("ecg_indices", default=list())
+    psd_args = {"fmax": meeg.pa["lowpass"]}
+
+    if len(eog_indices) > 0:
+        eog_epochs = meeg.load_eog_epochs()
+        eog_prop_figs = ica.plot_properties(
+            eog_epochs, eog_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="eog", matplotlib_figure=eog_prop_figs
+        )
+
+    if len(ecg_indices) > 0:
+        ecg_epochs = meeg.load_ecg_epochs()
+        ecg_prop_figs = ica.plot_properties(
+            ecg_epochs, ecg_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="ecg", matplotlib_figure=ecg_prop_figs
+        )
+
+    remaining_indices = [
+        ix for ix in ica.exclude if ix not in eog_indices + ecg_indices
+    ]
+    if len(remaining_indices) > 0:
+        data = meeg.load(ica_fitto)
+        prop_figs = ica.plot_properties(
+            data, remaining_indices, psd_args=psd_args, show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="properties", trial="manually", matplotlib_figure=prop_figs
+        )
+
+
+def plot_ica_scores(meeg, show_plots):
+    eog_scores = meeg.load_json("eog_scores", default=list())
+    if len(eog_scores) > 1:
+        ica = meeg.load_ica()
+        eog_score_fig = ica.plot_scores(
+            eog_scores, title=f"{meeg.name}: EOG", show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="scores", trial="eog", matplotlib_figure=eog_score_fig
+        )
+    else:
+        eog_score_fig = None
+
+    ecg_scores = meeg.load_json("ecg_scores", default=list())
+    if len(ecg_scores) > 1:
+        ica = meeg.load_ica()
+        ecg_score_fig = ica.plot_scores(
+            ecg_scores, title=f"{meeg.name}: ECG", show=show_plots
+        )
+        meeg.plot_save(
+            "ica", subfolder="scores", trial="ecg", matplotlib_figure=ecg_score_fig
+        )
+    else:
+        ecg_score_fig = None
+
+    return eog_score_fig, ecg_score_fig
+
+
+def plot_transformation(meeg, backend_3d):
     info = meeg.load_info()
     trans = meeg.load_transformation()
 
-    mne.viz.plot_alignment(info, trans, meeg.fsmri.name, meeg.subjects_dir,
-                           surfaces=['head-dense', 'inner_skull', 'brain'],
-                           show_axes=True, dig=True)
+    with mne.viz.use_3d_backend(backend_3d):
+        mne.viz.plot_alignment(
+            info,
+            trans,
+            meeg.fsmri.name,
+            meeg.subjects_dir,
+            surfaces=["head-dense", "inner_skull", "brain"],
+            show_axes=True,
+            dig=True,
+        )
 
-    meeg.plot_save('transformation', mayavi=True)
 
-
-def plot_src(fsmri):
+def plot_src(fsmri, backend_3d):
     src = fsmri.load_source_space()
-    src.plot()
-
-    fsmri.plot_save('src', mayavi=True)
+    with mne.viz.use_3d_backend(backend_3d):
+        src.plot()
 
 
 def plot_bem(fsmri, show_plots):
     src = fsmri.load_source_space()
-    fig1 = mne.viz.plot_bem(fsmri.name, fsmri.subjects_dir, src=src,
-                            show=show_plots)
+    fig1 = mne.viz.plot_bem(fsmri.name, fsmri.subjects_dir, src=src, show=show_plots)
 
-    fsmri.plot_save('bem', subfolder='source-space', matplotlib_figure=fig1)
+    fsmri.plot_save("bem", subfolder="source-space", matplotlib_figure=fig1)
 
     try:
         vol_src = fsmri.load_volume_source_space()
-        fig2 = mne.viz.plot_bem(fsmri.name, fsmri.subjects_dir, src=vol_src,
-                                show=show_plots)
+        fig2 = mne.viz.plot_bem(
+            fsmri.name, fsmri.subjects_dir, src=vol_src, show=show_plots
+        )
 
-        fsmri.plot_save('bem', subfolder='volume-source-space',
-                        matplotlib_figure=fig2)
+        fsmri.plot_save("bem", subfolder="volume-source-space", matplotlib_figure=fig2)
 
     except FileNotFoundError:
         pass
 
 
 def plot_sensitivity_maps(meeg, ch_types):
     fwd = meeg.load_forward()
 
-    for ch_type in [ct for ct in ch_types if ct in ['grad', 'mag', 'eeg']]:
-        sens_map = mne.sensitivity_map(fwd, ch_type=ch_type, mode='fixed')
-        brain = sens_map.plot(title=f'{ch_type}-Sensitivity for {meeg.name}',
-                              subjects_dir=meeg.subjects_dir,
-                              clim=dict(lims=[0, 50, 100]))
+    for ch_type in [ct for ct in ch_types if ct in ["grad", "mag", "eeg"]]:
+        sens_map = mne.sensitivity_map(fwd, ch_type=ch_type, mode="fixed")
+        brain = sens_map.plot(
+            title=f"{ch_type}-Sensitivity for {meeg.name}",
+            subjects_dir=meeg.subjects_dir,
+            clim=dict(lims=[0, 50, 100]),
+        )
 
-        meeg.plot_save('sensitivity', trial=ch_type, brain=brain)
+        meeg.plot_save("sensitivity", trial=ch_type, brain=brain)
 
 
 def plot_noise_covariance(meeg, show_plots):
     noise_covariance = meeg.load_noise_covariance()
     info = meeg.load_info()
 
     fig1, fig2 = noise_covariance.plot(info, show_svd=False, show=show_plots)
 
-    meeg.plot_save('noise-covariance', subfolder='covariance',
-                   matplotlib_figure=fig1)
-    meeg.plot_save('noise-covariance', subfolder='svd-spectra',
-                   matplotlib_figure=fig2)
+    meeg.plot_save("noise-covariance", subfolder="covariance", matplotlib_figure=fig1)
+    meeg.plot_save("noise-covariance", subfolder="svd-spectra", matplotlib_figure=fig2)
 
 
-def _brain_plot(meeg, stcs, stc_surface, stc_hemi, stc_views,
-                stc_time, stc_clim, stc_background, target_labels,
-                label_colors, stc_roll, stc_azimuth, stc_elevation,
-                interactive=False, **brain_movie_kwargs):
-    labels = meeg.fsmri.get_labels(target_labels)
+def _brain_plot(
+    meeg,
+    stcs,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    target_labels,
+    label_colors,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    backend_3d="pyvistaqt",
+    interactive=False,
+    **brain_movie_kwargs,
+):
     for trial, stc in stcs.items():
-        title = f'{meeg.name}-{trial}'
-        brain = stc.plot(subject=meeg.fsmri.name, surface=stc_surface,
-                         subjects_dir=meeg.subjects_dir,
-                         hemi=stc_hemi, views=stc_views,
-                         clim=stc_clim,
-                         initial_time=stc_time, background=stc_background,
-                         title=title, time_viewer=interactive)
-        brain.show_view(roll=stc_roll, azimuth=stc_azimuth,
-                        elevation=stc_elevation)
-        brain.add_text(0, 0.9, title, 'title', font_size=14)
+        title = f"{meeg.name}-{trial}"
+        brain = stc.plot(
+            subject=meeg.fsmri.name,
+            surface=stc_surface,
+            subjects_dir=meeg.subjects_dir,
+            hemi=stc_hemi,
+            views=stc_views,
+            clim=stc_clim,
+            initial_time=stc_time,
+            title=title,
+            time_viewer=interactive,
+        )
+        brain.show_view(roll=stc_roll, azimuth=stc_azimuth, elevation=stc_elevation)
+        brain.add_text(0, 0.9, title, "title", color="w", font_size=14)
         if not interactive:
+            labels = meeg.fsmri.get_labels(target_labels)
             for label in labels:
                 color = label_colors.get(label.name)
                 brain.add_label(label, borders=True, color=color)
-            if brain_movie_kwargs is not None and 'stc_animation_dilat' \
-                    in brain_movie_kwargs:
-                img_format = '.mp4'
+            if (
+                brain_movie_kwargs is not None
+                and "stc_animation_dilat" in brain_movie_kwargs
+            ):
+                img_format = ".mp4"
             else:
-                img_format = '.jpg'
+                img_format = ".jpg"
                 brain_movie_kwargs = None
 
-            meeg.plot_save('source_estimates', trial=trial, brain=brain,
-                           brain_movie_kwargs=brain_movie_kwargs,
-                           img_format=img_format)
+            meeg.plot_save(
+                "source_estimates",
+                trial=trial,
+                brain=brain,
+                brain_movie_kwargs=brain_movie_kwargs,
+                img_format=img_format,
+            )
 
-            if not meeg.ct.settings['show_plots']:
+            if not meeg.ct.settings["show_plots"]:
                 brain.close()
 
 
-def plot_stc(meeg, target_labels, label_colors,
-             stc_surface, stc_hemi, stc_views, stc_time, stc_clim,
-             stc_background,
-             stc_roll, stc_azimuth, stc_elevation):
+def plot_stc(
+    meeg,
+    target_labels,
+    label_colors,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    backend_3d,
+):
     stcs = meeg.load_source_estimates()
-    _brain_plot(meeg=meeg, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=target_labels,
-                label_colors=label_colors, stc_roll=stc_roll,
-                stc_azimuth=stc_azimuth, stc_elevation=stc_elevation)
-
-
-def plot_stc_interactive(meeg, stc_surface, stc_hemi, stc_views, stc_time,
-                         stc_clim,
-                         stc_background, stc_roll, stc_azimuth, stc_elevation):
+    _brain_plot(
+        meeg=meeg,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=target_labels,
+        label_colors=label_colors,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        backend_3d=backend_3d,
+    )
+
+
+def plot_stc_interactive(
+    meeg,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    backend_3d,
+):
     stcs = meeg.load_source_estimates()
-    _brain_plot(meeg=meeg, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=None,
-                label_colors=None, stc_roll=stc_roll,
-                stc_azimuth=stc_azimuth, stc_elevation=stc_elevation,
-                interactive=True)
-
-
-def plot_animated_stc(meeg, target_labels, label_colors,
-                      stc_surface, stc_hemi, stc_views, stc_time, stc_clim,
-                      stc_background, stc_roll, stc_azimuth,
-                      stc_elevation, stc_animation_span, stc_animation_dilat):
+    _brain_plot(
+        meeg=meeg,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=None,
+        label_colors=None,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        backend_3d=backend_3d,
+        interactive=True,
+    )
+
+
+def plot_animated_stc(
+    meeg,
+    target_labels,
+    label_colors,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    stc_animation_span,
+    stc_animation_dilat,
+    backend_3d,
+):
     stcs = meeg.load_source_estimates()
-    _brain_plot(meeg=meeg, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=target_labels,
-                label_colors=label_colors, stc_roll=stc_roll,
-                stc_azimuth=stc_azimuth, stc_elevation=stc_elevation,
-                stc_animation_span=stc_animation_span,
-                stc_animation_dilat=stc_animation_dilat)
-
-
-def plot_labels(fsmri, target_labels, label_colors,
-                stc_hemi, stc_surface, stc_views):
-    Brain = mne.viz.get_brain_class()
-    brain = Brain(subject_id=fsmri.name, hemi=stc_hemi, surf=stc_surface,
-                  subjects_dir=fsmri.subjects_dir, views=stc_views)
-
-    labels = fsmri.get_labels(target_labels)
-    for label in labels:
-        color = label_colors.get(label.name)
-        brain.add_label(label, borders=False, color=color)
-    fsmri.plot_save('labels', brain=brain)
+    _brain_plot(
+        meeg=meeg,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=target_labels,
+        label_colors=label_colors,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        stc_animation_span=stc_animation_span,
+        stc_animation_dilat=stc_animation_dilat,
+        backend_3d=backend_3d,
+    )
+
+
+def plot_labels(
+    fsmri,
+    target_labels,
+    label_colors,
+    stc_hemi,
+    stc_surface,
+    stc_views,
+    backend_3d,
+):
+    with mne.viz.use_3d_backend(backend_3d):
+        Brain = mne.viz.get_brain_class()
+        brain = Brain(
+            subject=fsmri.name,
+            hemi=stc_hemi,
+            surf=stc_surface,
+            subjects_dir=fsmri.subjects_dir,
+            views=stc_views,
+        )
+
+        labels = fsmri.get_labels(target_labels)
+        y = 0.95
+        for label in labels:
+            color = label_colors.get(label.name)
+            if color is None:
+                color = label.color
+            brain.add_label(label, borders=False, color=color)
+            brain.add_text(x=0.05, y=y, text=label.name, color=color, font_size=14)
+            y -= 0.05
+
+        fsmri.plot_save("labels", brain=brain)
 
 
 def plot_ecd(meeg):
     ecd_dips = meeg.load_ecd()
     trans = meeg.load_transformation()
 
     for trial in ecd_dips:
         for dipole in ecd_dips[trial]:
-            fig = dipole.plot_locations(trans, meeg.fsmri.name,
-                                        meeg.subjects_dir,
-                                        mode='orthoview', idx='gof')
-            fig.suptitle(meeg.name, horizontalalignment='right')
+            fig = dipole.plot_locations(
+                trans, meeg.fsmri.name, meeg.subjects_dir, mode="orthoview", idx="gof"
+            )
+            fig.suptitle(meeg.name, horizontalalignment="right")
 
-            meeg.plot_save('ecd', subfolder=dipole, trial=trial,
-                           matplotlib_figure=fig)
+            meeg.plot_save("ecd", subfolder=dipole, trial=trial, matplotlib_figure=fig)
 
             # find time point with highest GOF to plot
             best_idx = np.argmax(dipole.gof)
             best_time = dipole.times[best_idx]
 
             print(
-                f'Highest GOF {dipole.gof[best_idx]:.2f}% at '
-                f't={best_time * 1000:.1f} ms with confidence volume'
-                f'{dipole.conf["vol"][best_idx] * 100 ** 3} cm^3')
-
-            mri_pos = mne.head_to_mri(dipole.pos, meeg.fsmri.name, trans,
-                                      meeg.subjects_dir)
-
-            save_path_anat = join(meeg.obj.figures_path, meeg.p_preset, 'ECD',
-                                  dipole, trial,
-                                  f'{meeg.name}-{trial}_{meeg.pr.p_preset}_'
-                                  f'ECD-{dipole}{meeg.img_format}')
-            t1_path = join(meeg.subjects_dir, meeg.fsmri.name, 'mri', 'T1.mgz')
-            plot_anat(t1_path, cut_coords=mri_pos[best_idx],
-                      output_file=save_path_anat,
-                      title=f'{meeg.name}-{trial}_{dipole}',
-                      annotate=True, draw_cross=True)
-
-            plot_anat(t1_path, cut_coords=mri_pos[best_idx],
-                      title=f'{meeg.name}-{trial}_{dipole}',
-                      annotate=True, draw_cross=True)
+                f"Highest GOF {dipole.gof[best_idx]:.2f}% at "
+                f"t={best_time * 1000:.1f} ms with confidence volume"
+                f'{dipole.conf["vol"][best_idx] * 100 ** 3} cm^3'
+            )
+
+            mri_pos = mne.head_to_mri(
+                dipole.pos, meeg.fsmri.name, trans, meeg.subjects_dir
+            )
+
+            save_path_anat = join(
+                meeg.obj.figures_path,
+                meeg.p_preset,
+                "ECD",
+                dipole,
+                trial,
+                f"{meeg.name}-{trial}_{meeg.pr.p_preset}_"
+                f"ECD-{dipole}{meeg.img_format}",
+            )
+            t1_path = join(meeg.subjects_dir, meeg.fsmri.name, "mri", "T1.mgz")
+            plot_anat(
+                t1_path,
+                cut_coords=mri_pos[best_idx],
+                output_file=save_path_anat,
+                title=f"{meeg.name}-{trial}_{dipole}",
+                annotate=True,
+                draw_cross=True,
+            )
+
+            plot_anat(
+                t1_path,
+                cut_coords=mri_pos[best_idx],
+                title=f"{meeg.name}-{trial}_{dipole}",
+                annotate=True,
+                draw_cross=True,
+            )
 
 
 def plot_snr(meeg, show_plots):
     evokeds = meeg.load_evokeds()
     inv = meeg.load_inverse_operator()
 
     for evoked in evokeds:
         trial = evoked.comment
         # data snr
         fig = mne.viz.plot_snr_estimate(evoked, inv, show=show_plots)
-        fig.suptitle(f'{meeg.name}-{evoked.comment}',
-                     horizontalalignment='center')
+        fig.suptitle(f"{meeg.name}-{evoked.comment}", horizontalalignment="center")
 
-        meeg.plot_save('snr', trial=trial, matplotlib_figure=fig)
+        meeg.plot_save("snr", trial=trial, matplotlib_figure=fig)
 
 
-def plot_label_time_course(meeg, show_plots):
+def plot_label_time_course(meeg, label_colors, show_plots):
     ltcs = meeg.load_ltc()
     for trial in ltcs:
-        for label in ltcs[trial]:
-            plt.figure()
-            plt.plot(ltcs[trial][label][1], ltcs[trial][label][0])
-            plt.title(f'{meeg.name}-{trial}-{label}\n'
-                      f'Extraction-Mode: {meeg.pa["extract_mode"]}')
-            plt.xlabel('Time in s')
-            plt.ylabel('Source amplitude')
-            if show_plots:
-                plt.show()
+        plt.figure()
+        plt.title(
+            f"{meeg.name}-{trial}\n" f'Extraction-Mode: {meeg.pa["extract_mode"]}'
+        )
+        plt.xlabel("Time in s")
+        plt.ylabel("Source amplitude")
+        for label_name, data in ltcs[trial].items():
+            color = label_colors.get(label_name, "black")
+            plt.plot(data[1], data[0], color=color, label=label_name)
+        plt.legend()
+        if show_plots:
+            plt.show()
+        meeg.plot_save("label-time-course", trial=trial)
 
-            meeg.plot_save('label-time-course', subfolder=label, trial=trial)
 
+def _get_n_subplots(n_items):
+    n_subplots = np.ceil(np.sqrt(n_items)).astype(int)
+    if n_items <= 2:
+        nrows = 1
+        ax_idxs = range(n_subplots)
+    else:
+        nrows = n_subplots
+        ax_idxs = itertools.product(range(n_subplots), repeat=2)
+    ncols = n_subplots
+
+    return nrows, ncols, ax_idxs
 
-def plot_src_connectivity(meeg, target_labels, con_fmin,
-                          con_fmax, show_plots):
-    con_dict = meeg.load_connectivity()
-    labels = meeg.fsmri.get_labels(target_labels)
-    if 'unknown-lh' in labels:
-        labels.pop('unknown-lh')
-    label_colors = [label.color for label in labels]
-    label_names = [label.name for label in labels]
-    lh_labels = [l_name for l_name in label_names if l_name.endswith('lh')]
-    rh_labels = [l_name for l_name in label_names if l_name.endswith('rh')]
-
-    # Get the y-location of the label
-    lh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
-                     if lb.name in lh_labels]
-    rh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
-                     if lb.name in rh_labels]
-
-    # Reorder the labels based on their location
-    lh_labels = [label for (yp, label) in
-                 sorted(zip(lh_label_ypos, lh_labels))]
-    rh_labels = [label for (yp, label) in
-                 sorted(zip(rh_label_ypos, rh_labels))]
-
-    # Save the plot order and create a circular layout
-    node_order = list()
-    node_order.extend(lh_labels[::-1])  # reverse the order
-    node_order.extend(rh_labels)
-
-    node_angles = mne.viz.circular_layout(
-        label_names, node_order, start_pos=90,
-        group_boundaries=[0, len(label_names) / 2])
 
-    # Plot the graph using node colors from the FreeSurfer parcellation.
-    # We only show the 300 strongest connections.
+def _plot_connectivity(obj, con_dict, label_colors, show_plots):
     for trial in con_dict:
-        for con_method in con_dict[trial]:
-            fig, axes = mne_connectivity.viz.plot_connectivity_circle(
-                con_dict[trial][con_method], label_names,
-                n_lines=100, node_angles=node_angles,
-                node_colors=label_colors,
-                title=f'{trial}: '
-                      f'{str(con_fmin)}-{str(con_fmax)}',
-                fontsize_names=8, show=show_plots)
+        for con_method, con in con_dict[trial].items():
+            labels = obj.fsmri.get_labels(con.names)
+            if "unknown-lh" in labels:
+                labels.pop("unknown-lh")
+            colors = list()
+            for label in labels:
+                color = label_colors.get(label.name)
+                if color is None:
+                    color = label.color
+                colors.append(color)
+            label_names = [label.name for label in labels]
+            lh_labels = [l_name for l_name in label_names if l_name.endswith("lh")]
+            rh_labels = [l_name for l_name in label_names if l_name.endswith("rh")]
+
+            # Get the y-location of the label
+            lh_label_ypos = [
+                np.mean(lb.pos[:, 1]) for lb in labels if lb.name in lh_labels
+            ]
+            rh_label_ypos = [
+                np.mean(lb.pos[:, 1]) for lb in labels if lb.name in rh_labels
+            ]
+
+            # Reorder the labels based on their location
+            lh_labels = [label for (yp, label) in sorted(zip(lh_label_ypos, lh_labels))]
+            rh_labels = [label for (yp, label) in sorted(zip(rh_label_ypos, rh_labels))]
+
+            # Save the plot order and create a circular layout
+            node_order = list()
+            node_order.extend(lh_labels[::-1])  # reverse the order
+            node_order.extend(rh_labels)
+
+            node_angles = mne.viz.circular_layout(
+                label_names,
+                node_order,
+                start_pos=90,
+                group_boundaries=[0, len(label_names) / 2],
+            )
+            con_data = con.get_data(output="dense")
+
+            nrows, ncols, ax_idxs = _get_n_subplots(len(con.freqs))
+            ax_idxs = list(ax_idxs)
+            fig, axes = plt.subplots(
+                nrows=nrows,
+                ncols=ncols,
+                subplot_kw={"projection": "polar"},
+                facecolor="black",
+                figsize=(8, 8),
+            )
+            # Remove extra axes
+            if nrows**2 > len(con.freqs):
+                fig.delaxes(axes[-1, -1])
+
+            for freq_idx, freq in enumerate(con.freqs):
+                if isinstance(axes, np.ndarray):
+                    ax = axes[ax_idxs[freq_idx]]
+                else:
+                    ax = axes
+                title = f"Frequency={freq:.1f} Hz"
+                mne_connectivity.viz.plot_connectivity_circle(
+                    con_data[:, :, freq_idx],
+                    label_names,
+                    n_lines=None,
+                    node_angles=node_angles,
+                    node_colors=colors,
+                    title=title,
+                    show=show_plots,
+                    ax=ax,
+                )
+            fig.suptitle(
+                f"{obj.name}-{trial}-{con_method}",
+                horizontalalignment="center",
+                color="white",
+            )
+            plt.tight_layout()
+            if isinstance(obj, MEEG):
+                plot_name = "connectivity"
+            else:
+                plot_name = "ga_connectivity"
+            obj.plot_save(
+                plot_name, subfolder=con_method, trial=trial, matplotlib_figure=fig
+            )
 
-            meeg.plot_save('connectivity', subfolder=con_method, trial=trial,
-                           matplotlib_figure=fig)
 
+def plot_src_connectivity(meeg, label_colors, show_plots):
+    con_dict = meeg.load_connectivity()
+    _plot_connectivity(meeg, con_dict, label_colors, show_plots)
 
-# %% Grand-Average Plots
 
+# %% Grand-Average Plots
 def plot_grand_avg_evokeds(group, show_plots):
     ga_evokeds = group.load_ga_evokeds()
 
     for trial in ga_evokeds:
-        fig = ga_evokeds[trial].plot(window_title=f'{group.name}-{trial}',
-                                     spatial_colors=True, gfp=True,
-                                     show=show_plots)
+        fig = ga_evokeds[trial].plot(
+            window_title=f"{group.name}-{trial}",
+            spatial_colors=True,
+            gfp=True,
+            show=show_plots,
+        )
 
-        group.plot_save('ga_evokeds', trial=trial, matplotlib_figure=fig)
+        group.plot_save("ga_evokeds", trial=trial, matplotlib_figure=fig)
 
 
 def plot_grand_avg_tfr(group, show_plots):
     ga_dict = group.load_ga_tfr()
 
     for trial in ga_dict:
         power = ga_dict[trial]
-        fig1 = power.plot(title=f'{group.name}-{power.comment}',
-                          show=show_plots)
-        fig2 = power.plot_topo(title=f'{group.name}-{power.comment}',
-                               show=show_plots)
-        fig3 = power.plot_joint(title=f'{group.name}-{power.comment}',
-                                show=show_plots)
-        fig4 = power.plot_topomap(title=f'{group.name}-{power.comment}',
-                                  show=show_plots)
-
-        group.plot_save('ga_tfr', subfolder='plot', trial=power.comment,
-                        matplotlib_figure=fig1)
-        group.plot_save('ga_tfr', subfolder='topo', trial=power.comment,
-                        matplotlib_figure=fig2)
-        group.plot_save('ga_tfr', subfolder='joint', trial=power.comment,
-                        matplotlib_figure=fig3)
-        group.plot_save('ga_tfr', subfolder='topomap', trial=power.comment,
-                        matplotlib_figure=fig4)
-
-
-def plot_grand_avg_stc(group, target_labels, label_colors,
-                       stc_surface, stc_hemi, stc_views, stc_time, stc_clim,
-                       stc_background, stc_roll, stc_azimuth, stc_elevation):
+        fig1 = power.plot(
+            title=f"{group.name}-{power.comment}", combine="mean", show=show_plots
+        )
+        fig2 = power.plot_topo(title=f"{group.name}-{power.comment}", show=show_plots)
+        fig3 = power.plot_joint(title=f"{group.name}-{power.comment}", show=show_plots)
+        fig4 = power.plot_topomap(show=show_plots)
+
+        group.plot_save(
+            "ga_tfr", subfolder="plot", trial=power.comment, matplotlib_figure=fig1
+        )
+        group.plot_save(
+            "ga_tfr", subfolder="topo", trial=power.comment, matplotlib_figure=fig2
+        )
+        group.plot_save(
+            "ga_tfr", subfolder="joint", trial=power.comment, matplotlib_figure=fig3
+        )
+        group.plot_save(
+            "ga_tfr", subfolder="topomap", trial=power.comment, matplotlib_figure=fig4
+        )
+
+
+def plot_grand_avg_stc(
+    group,
+    target_labels,
+    label_colors,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    backend_3d,
+):
     stcs = group.load_ga_stc()
-    _brain_plot(meeg=group, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=target_labels,
-                label_colors=label_colors, stc_roll=stc_roll,
-                stc_azimuth=stc_azimuth, stc_elevation=stc_elevation)
-
-
-def plot_grand_average_stc_interactive(group, stc_surface, stc_hemi,
-                                       stc_views, stc_time, stc_clim,
-                                       stc_background,
-                                       stc_roll, stc_azimuth, stc_elevation):
+    _brain_plot(
+        meeg=group,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=target_labels,
+        label_colors=label_colors,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        backend_3d=backend_3d,
+    )
+
+
+def plot_grand_average_stc_interactive(
+    group,
+    label_colors,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    backend_3d,
+):
     stcs = group.load_ga_stc()
-    _brain_plot(meeg=group, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=None,
-                stc_roll=stc_roll, stc_azimuth=stc_azimuth,
-                stc_elevation=stc_elevation, interactive=True)
-
-
-def plot_grand_avg_stc_anim(group, target_labels, label_colors,
-                            stc_surface, stc_hemi, stc_views, stc_time,
-                            stc_clim, stc_background,
-                            stc_roll, stc_azimuth, stc_elevation,
-                            stc_animation_span,
-                            stc_animation_dilat):
+    _brain_plot(
+        meeg=group,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=None,
+        label_colors=label_colors,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        backend_3d=backend_3d,
+        interactive=True,
+    )
+
+
+def plot_grand_avg_stc_anim(
+    group,
+    target_labels,
+    label_colors,
+    stc_surface,
+    stc_hemi,
+    stc_views,
+    stc_time,
+    stc_clim,
+    stc_roll,
+    stc_azimuth,
+    stc_elevation,
+    stc_animation_span,
+    stc_animation_dilat,
+    backend_3d,
+):
     stcs = group.load_ga_stc()
-    _brain_plot(meeg=group, stcs=stcs, stc_surface=stc_surface,
-                stc_hemi=stc_hemi, stc_views=stc_views, stc_time=stc_time,
-                stc_clim=stc_clim,
-                stc_background=stc_background, target_labels=target_labels,
-                label_colors=label_colors, stc_roll=stc_roll,
-                stc_azimuth=stc_azimuth, stc_elevation=stc_elevation,
-                stc_animation_span=stc_animation_span,
-                stc_animation_dilat=stc_animation_dilat)
+    _brain_plot(
+        meeg=group,
+        stcs=stcs,
+        stc_surface=stc_surface,
+        stc_hemi=stc_hemi,
+        stc_views=stc_views,
+        stc_time=stc_time,
+        stc_clim=stc_clim,
+        target_labels=target_labels,
+        label_colors=label_colors,
+        stc_roll=stc_roll,
+        stc_azimuth=stc_azimuth,
+        stc_elevation=stc_elevation,
+        stc_animation_span=stc_animation_span,
+        stc_animation_dilat=stc_animation_dilat,
+        backend_3d=backend_3d,
+    )
 
 
-def plot_grand_avg_ltc(group, show_plots):
+def plot_grand_avg_ltc(group, label_colors, show_plots):
     ga_ltc = group.load_ga_ltc()
     for trial in ga_ltc:
-        for label in ga_ltc[trial]:
-            plt.figure()
-            plt.plot(ga_ltc[trial][label][1], ga_ltc[trial][label][0])
-            plt.title(f'Label-Time-Course for {group.name}-{trial}-{label}\n'
-                      f'with Extraction-Mode: {group.pa["extract_mode"]}')
-            plt.xlabel('Time in ms')
-            plt.ylabel('Source amplitude')
-            if show_plots:
-                plt.show()
-
-            group.plot_save('ga_label-time-course', subfolder=label,
-                            trial=trial)
-
-
-def plot_grand_avg_connect(group, con_fmin, con_fmax, target_labels,
-                           morph_to, show_plots, connectivity_vmin,
-                           connectivity_vmax):
-    ga_dict = group.load_ga_con()
-
-    # Get labels for FreeSurfer 'aparc' cortical parcellation
-    # with 34 labels/hemi
-    fsmri = FSMRI(morph_to, group.ct)
-    labels = fsmri.get_labels(target_labels)
-    if 'unknown-lh' in labels:
-        labels.remove('unknown-lh')
-
-    label_colors = [label.color for label in labels]
-    label_names = [lb.name for lb in labels]
-
-    lh_labels = [l_name for l_name in label_names if l_name.endswith('lh')]
-    rh_labels = [l_name for l_name in label_names if l_name.endswith('rh')]
-
-    # Get the y-location of the label
-    lh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
-                     if lb.name in lh_labels]
-    rh_label_ypos = [np.mean(lb.pos[:, 1]) for lb in labels
-                     if lb.name in rh_labels]
-
-    # Reorder the labels based on their location
-    lh_labels = [label for (yp, label) in
-                 sorted(zip(lh_label_ypos, lh_labels))]
-    rh_labels = [label for (yp, label) in
-                 sorted(zip(rh_label_ypos, rh_labels))]
-
-    # Save the plot order and create a circular layout
-    node_order = list()
-    node_order.extend(lh_labels[::-1])  # reverse the order
-    node_order.extend(rh_labels)
-
-    node_angles = mne.viz.circular_layout(
-        label_names, node_order, start_pos=90,
-        group_boundaries=[0, len(label_names) / 2])
+        plt.figure()
+        plt.title(
+            f"Label-Time-Course for {group.name}-{trial}\n"
+            f'with Extraction-Mode: {group.pa["extract_mode"]}'
+        )
+        plt.xlabel("Time in ms")
+        plt.ylabel("Source amplitude")
+        for label_name, data in ga_ltc[trial].items():
+            color = label_colors.get(label_name, "black")
+            plt.plot(data[1], data[0], color=color, label=label_name)
+        plt.legend()
+        if show_plots:
+            plt.show()
 
-    for trial in ga_dict:
-        for method in ga_dict[trial]:
-            fig, axes = mne_connectivity.viz.plot_connectivity_circle(
-                ga_dict[trial][method],
-                label_names, n_lines=300,
-                node_angles=node_angles,
-                node_colors=label_colors,
-                title=f'{method}: {str(con_fmin)}-{str(con_fmax)}',
-                vmin=connectivity_vmin,
-                vmax=connectivity_vmax,
-                fontsize_names=16, show=show_plots)
-
-            group.plot_save('ga_connectivity', subfolder=method, trial=trial,
-                            matplotlib_figure=fig)
-
-
-def close_all():
-    plt.close('all')
-    gc.collect()
+        group.plot_save("ga_label-time-course", trial=trial)
+
+
+def plot_grand_avg_connect(
+    group,
+    label_colors,
+    show_plots,
+):
+    con_dict = group.load_ga_con()
+    _plot_connectivity(group, con_dict, label_colors, show_plots)
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/base_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/base_widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import itertools
+import re
 import sys
 
 import numpy as np
 import pandas
-from PyQt5.QtCore import QItemSelectionModel, QTimer, Qt, pyqtSignal
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
+from qtpy.QtCore import QItemSelectionModel, QTimer, Qt, Signal
+from qtpy.QtGui import QFont
+from qtpy.QtWidgets import (
     QAbstractItemView,
     QApplication,
     QDialog,
     QHBoxLayout,
     QLabel,
     QListView,
     QPushButton,
@@ -25,14 +26,15 @@
     QSpinBox,
     QTabWidget,
     QTableView,
     QTreeView,
     QVBoxLayout,
     QWidget,
     QComboBox,
+    QMessageBox,
 )
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.gui.gui_utils import get_user_input_string
 from mne_pipeline_hd.gui.models import (
     BaseDictModel,
     BaseListModel,
@@ -42,43 +44,45 @@
     CheckListModel,
     EditDictModel,
     EditListModel,
     EditPandasModel,
     FileManagementModel,
     TreeModel,
 )
-from mne_pipeline_hd.pipeline.pipeline_utils import QS
+from mne_pipeline_hd.pipeline.pipeline_utils import QS, logger
 
 
 class Base(QWidget):
-    currentChanged = pyqtSignal(object, object)
-    selectionChanged = pyqtSignal(object)
-    dataChanged = pyqtSignal(object, object)
+    currentChanged = Signal(object, object)
+    selectionChanged = Signal(object)
+    dataChanged = Signal(object, object)
 
-    def __init__(self, model, view, drag_drop, parent, title, verbose=False):
+    def __init__(self, model, view, drag_drop, parent, title):
         if parent:
             super().__init__(parent)
         else:
             super().__init__()
         self.title = title
-        self.verbose = verbose
 
         self.model = model
         self.view = view
         self.view.setModel(self.model)
 
         if drag_drop:
             self.view.setDragEnabled(True)
             self.view.setAcceptDrops(True)
             self.setDropIndicatorShown(True)
 
         # Connect to custom Selection-Signal
         self.view.selectionModel().currentChanged.connect(self._current_changed)
         self.view.selectionModel().selectionChanged.connect(self._selection_changed)
         self.model.dataChanged.connect(self._data_changed)
+        # Also send signal when rows are removed/added
+        self.model.rowsInserted.connect(self._data_changed)
+        self.model.rowsRemoved.connect(self._data_changed)
 
         self.init_ui()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         if self.title:
@@ -98,20 +102,21 @@
         except (KeyError, IndexError):
             current = None
 
         return current
 
     def _current_changed(self, current_idx, previous_idx):
         current = self.model.getData(current_idx)
+        # ToDo: For ListWidget after removal,
+        #  there is a bug when previous_idx is too high
         previous = self.model.getData(previous_idx)
 
         self.currentChanged.emit(current, previous)
 
-        if self.verbose:
-            print(f"Current changed from {previous} to {current}")
+        logger().debug(f"Current changed from {previous} to {current}")
 
     def get_selected(self):
         try:
             selected = [self.model.getData(idx) for idx in self.view.selectedIndexes()]
         except (KeyError, IndexError):
             selected = list()
 
@@ -121,23 +126,21 @@
         # Although the SelectionChanged-Signal sends
         # selected/deselected indexes, I don't use them here, because they
         # don't seem represent the selection.
         selected = self.get_selected()
 
         self.selectionChanged.emit(selected)
 
-        if self.verbose:
-            print(f"Selection changed to {selected}")
+        logger().debug(f"Selection changed to {selected}")
 
     def _data_changed(self, index, _):
         data = self.model.getData(index)
 
         self.dataChanged.emit(data, index)
-        if self.verbose:
-            print(f"{data} changed at {index}")
+        logger().debug(f"{data} changed at {index}")
 
     def content_changed(self):
         """Informs ModelView about external change made in data"""
         self.model.layoutChanged.emit()
 
     def replace_data(self, new_data):
         """Replaces model._data with new_data"""
@@ -150,17 +153,16 @@
         self,
         model,
         view,
         extended_selection=False,
         drag_drop=False,
         parent=None,
         title=None,
-        verbose=False,
     ):
-        super().__init__(model, view, drag_drop, parent, title, verbose=verbose)
+        super().__init__(model, view, drag_drop, parent, title)
 
         if extended_selection:
             self.view.setSelectionMode(QAbstractItemView.ExtendedSelection)
 
     def select(self, values, clear_selection=True):
         indices = [i for i, x in enumerate(self.model._data) if x in values]
 
@@ -185,16 +187,14 @@
         Set True if you want to display the list-index in front of each value.
     drag_drop: bool
         Set True to enable Drag&Drop.
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
-    verbose : bool
-        Set True to see debugging for signals.
 
     Notes
     -----
     If you change the contents of data outside of this class,
     call content_changed to update this widget.
     If you change the reference to data, call the appropriate replace_data.
     """
@@ -203,24 +203,22 @@
         self,
         data=None,
         extended_selection=False,
         show_index=False,
         drag_drop=False,
         parent=None,
         title=None,
-        verbose=False,
     ):
         super().__init__(
             model=BaseListModel(data, show_index, drag_drop),
             view=QListView(),
             extended_selection=extended_selection,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
 
 
 class EditList(BaseList):
     """An editable List-Widget to display and manipulate the content of a list.
 
     Parameters
@@ -238,16 +236,14 @@
         Set True to enable Drag&Drop.
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
     model : QAbstractItemModel
         Provide an alternative to EditListModel.
-    verbose : bool
-        Set True to see debugging for signals
 
     Notes
     -----
     If you change the contents of the list outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data.
     """
@@ -259,30 +255,28 @@
         ui_button_pos="right",
         extended_selection=False,
         show_index=False,
         drag_drop=False,
         parent=None,
         title=None,
         model=None,
-        verbose=False,
     ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         if model is None:
             model = EditListModel(data, show_index=show_index, drag_drop=drag_drop)
 
         super().__init__(
             model=model,
             view=QListView(),
             extended_selection=extended_selection,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
 
     def init_ui(self):
         if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
@@ -356,50 +350,46 @@
         Set True if you want to display the list-index in front of each value.
     drag_drop: bool
         Set True to enable Drag&Drop.
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title
-    verbose : bool
-        Set True to see debugging for signals
 
     Notes
     -----
     If you change the contents of data outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data or replace_checked.
     """
 
-    checkedChanged = pyqtSignal(list)
+    checkedChanged = Signal(list)
 
     def __init__(
         self,
         data=None,
         checked=None,
         ui_buttons=True,
         ui_button_pos="right",
         one_check=False,
         show_index=False,
         drag_drop=False,
         parent=None,
         title=None,
-        verbose=False,
     ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         super().__init__(
             model=CheckListModel(data, checked, one_check, show_index, drag_drop),
             view=QListView(),
             extended_selection=False,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
 
         self.model.dataChanged.connect(self._checked_changed)
 
     def init_ui(self):
         if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
@@ -434,19 +424,18 @@
             super_layout.addLayout(layout)
             self.setLayout(super_layout)
         else:
             self.setLayout(layout)
 
     def _checked_changed(self):
         self.checkedChanged.emit(self.model._checked)
-        if self.verbose:
-            print(f"Changed values: {self.model._checked}")
+        logger().debug(f"Changed values: {self.model._checked}")
 
     def replace_checked(self, new_checked):
-        """Replaces model._checked with new check_dict"""
+        """Replaces model._checked with new checked list"""
         self.model._checked = new_checked
         self.content_changed()
 
     def select_all(self):
         """Select all Items while leaving reference to model._checked intact"""
         for item in [i for i in self.model._data if i not in self.model._checked]:
             self.model._checked.append(item)
@@ -483,16 +472,14 @@
     no_bt: str
         Supply the name for a qt-standard-icon to mark the items
          not existing in check_dict.
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
-    verbose : bool
-        Set True to see debugging for signals.
 
     Notes
     -----
     If you change the contents of data outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data.
     If you change the reference to check_dict, call replace_check_dict.
@@ -508,26 +495,24 @@
         extended_selection=False,
         show_index=False,
         drag_drop=False,
         yes_bt=None,
         no_bt=None,
         parent=None,
         title=None,
-        verbose=False,
     ):
         super().__init__(
             model=CheckDictModel(
                 data, check_dict, show_index, drag_drop, yes_bt, no_bt
             ),
             view=QListView(),
             extended_selection=extended_selection,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
 
     def replace_check_dict(self, new_check_dict=None):
         """Replaces model.check_dict with new check_dict"""
         if new_check_dict:
             self.model._check_dict = new_check_dict
         self.content_changed()
@@ -558,16 +543,14 @@
         the items not existing in check_dict.
     drag_drop: bool
         Set True to enable Drag&Drop.
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
-    verbose : bool
-        Set True to see debugging for signals.
 
     Notes
     -----
     If you change the contents of data outside of this class,
      call content_changed to update this widget.
     If you change the reference to data, call replace_data.
     If you change the reference to check_dict, call replace_check_dict.
@@ -585,29 +568,27 @@
         extended_selection=False,
         show_index=False,
         yes_bt=None,
         no_bt=None,
         drag_drop=False,
         parent=None,
         title=None,
-        verbose=False,
     ):
         model = CheckDictEditModel(
             data, check_dict, show_index=show_index, yes_bt=yes_bt, no_bt=no_bt
         )
         super().__init__(
             data=data,
             ui_buttons=ui_buttons,
             ui_button_pos=ui_button_pos,
             extended_selection=extended_selection,
             show_index=show_index,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
             model=model,
         )
 
     def replace_check_dict(self, new_check_dict=None):
         """Replaces model.check_dict with new check_dict"""
         if new_check_dict:
             self.model._check_dict = new_check_dict
@@ -620,18 +601,16 @@
         model,
         view,
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
-        super().__init__(model, view, drag_drop, parent, title, verbose=verbose)
-        self.verbose = verbose
+        super().__init__(model, view, drag_drop, parent, title)
 
         if resize_rows:
             model.layoutChanged.connect(self.view.resizeRowsToContents)
             model.layoutChanged.emit()
         if resize_columns:
             model.layoutChanged.connect(self.view.resizeColumnsToContents)
             model.layoutChanged.emit()
@@ -663,16 +642,15 @@
 
     def _current_changed(self, current_idx, previous_idx):
         current_data = self.get_keyvalue_by_index(current_idx)
         previous_data = self.get_keyvalue_by_index(previous_idx)
 
         self.currentChanged.emit(current_data, previous_data)
 
-        if self.verbose:
-            print(f"Current changed from {current_data} to {previous_data}")
+        logger().debug(f"Current changed from {current_data} to {previous_data}")
 
     def _selected_keyvalue(self, indexes):
         try:
             return set([self.get_keyvalue_by_index(idx) for idx in indexes])
         except TypeError:
             return [self.get_keyvalue_by_index(idx) for idx in indexes]
 
@@ -680,16 +658,15 @@
         return self._selected_keyvalue(self.view.selectedIndexes())
 
     def _selection_changed(self):
         selected_data = self.get_selected()
 
         self.selectionChanged.emit(selected_data)
 
-        if self.verbose:
-            print(f"Selection to {selected_data}")
+        logger().debug(f"Selection to {selected_data}")
 
     def select(self, keys, values, clear_selection=True):
         key_indices = [i for i, x in enumerate(self.model._data.keys()) if x in keys]
         value_indices = [
             i for i, x in enumerate(self.model._data.values()) if x in values
         ]
 
@@ -718,41 +695,38 @@
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
     resize_rows : bool
         Set True to resize the rows to contents.
     resize_columns : bool
         Set True to resize the columns to contents.
-    verbose : bool
-        Set True to see debugging for signals.
 
     """
 
     def __init__(
         self,
         data=None,
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
         super().__init__(
             model=BaseDictModel(data),
             view=QTableView(),
             drag_drop=drag_drop,
             parent=parent,
             title=title,
             resize_rows=resize_rows,
             resize_columns=resize_columns,
-            verbose=verbose,
         )
 
 
+# ToDo: DataChanged somehow not emitted when row is removed
 class EditDict(BaseDict):
     """A Widget to display and edit a Dictionary
 
     Parameters
     ----------
     data : dict | None
         Input a pandas DataFrame with contents to display.
@@ -767,43 +741,39 @@
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title.
     resize_rows : bool
         Set True to resize the rows to contents.
     resize_columns : bool
         Set True to resize the columns to contents.
-    verbose : bool
-        Set True to see debugging for signals.
 
     """
 
     def __init__(
         self,
         data=None,
         ui_buttons=True,
         ui_button_pos="right",
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         super().__init__(
             model=EditDictModel(data),
             view=QTableView(),
             drag_drop=drag_drop,
             parent=parent,
             title=title,
             resize_rows=resize_rows,
             resize_columns=resize_columns,
-            verbose=verbose,
         )
 
     def init_ui(self):
         if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
@@ -868,38 +838,33 @@
     ----------
     model
         The model for the pandas DataFrame.
     view
         The view for the pandas DataFrame.
     title : str | None
         An optional title.
-    verbose : bool
-        Set True to see debugging for signals.
     """
 
     def __init__(
         self,
         model,
         view,
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
         super().__init__(
             model=model,
             view=view,
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
-        self.verbose = verbose
 
         if resize_rows:
             model.layoutChanged.connect(self.view.resizeRowsToContents)
             model.layoutChanged.emit()
         if resize_columns:
             model.layoutChanged.connect(self.view.resizeColumnsToContents)
             model.layoutChanged.emit()
@@ -941,32 +906,30 @@
         previous_list = list()
 
         self.get_rowcol_by_index(current_idx, current_list)
         self.get_rowcol_by_index(previous_idx, previous_list)
 
         self.currentChanged.emit(current_list, previous_list)
 
-        if self.verbose:
-            print(f"Current changed from {previous_list} to {current_list}")
+        logger().debug(f"Current changed from {previous_list} to {current_list}")
 
     def get_selected(self):
         # Somehow, the indexes got from selectionChanged
         # don't appear to be right (maybe some issue with QItemSelection?).
         selection_list = list()
         for idx in self.view.selectedIndexes():
             self.get_rowcol_by_index(idx, selection_list)
 
         return selection_list
 
     def _selection_changed(self):
         selection_list = self.get_selected()
         self.selectionChanged.emit(selection_list)
 
-        if self.verbose:
-            print(f"Selection changed to {selection_list}")
+        logger().debug(f"Selection changed to {selection_list}")
 
     def select(self, values=None, rows=None, columns=None, clear_selection=True):
         """
         Select items in Pandas DataFrame by value
         or select complete rows/columns.
 
         Parameters
@@ -1029,16 +992,14 @@
         Parent Widget (QWidget or inherited) or None if there is no parent
     title : str | None
         An optional title
     resize_rows : bool
         Set True to resize the rows to contents
     resize_columns : bool
         Set True to resize the columns to contents
-    verbose : bool
-        Set True to see debugging for signals
 
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
@@ -1046,25 +1007,23 @@
         self,
         data=None,
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
         super().__init__(
             model=BasePandasModel(data),
             view=QTableView(),
             drag_drop=drag_drop,
             parent=parent,
             title=title,
             resize_rows=resize_rows,
             resize_columns=resize_columns,
-            verbose=verbose,
         )
 
 
 class EditPandasTable(BasePandasTable):
     """A Widget to display and edit a pandas DataFrame
 
     Parameters
@@ -1082,16 +1041,14 @@
         Parent Widget (QWidget or inherited) or None if there is no parent.
     title : str | None
         An optional title
     resize_rows : bool
         Set True to resize the rows to contents.
     resize_columns : bool
         Set True to resize the columns to contents.
-    verbose : bool
-        Set True to see debugging for signals.
 
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
@@ -1101,28 +1058,26 @@
         ui_buttons=True,
         ui_button_pos="right",
         drag_drop=False,
         parent=None,
         title=None,
         resize_rows=False,
         resize_columns=False,
-        verbose=False,
     ):
         self.ui_buttons = ui_buttons
         self.ui_button_pos = ui_button_pos
 
         super().__init__(
             model=EditPandasModel(data),
             view=QTableView(),
             drag_drop=drag_drop,
             parent=parent,
             title=title,
             resize_rows=resize_rows,
             resize_columns=resize_columns,
-            verbose=verbose,
         )
 
     def init_ui(self):
         if self.ui_button_pos in ["top", "bottom"]:
             layout = QVBoxLayout()
             bt_layout = QHBoxLayout()
         else:
@@ -1273,44 +1228,40 @@
     ----------
     data : pandas.DataFrame | None
         Input a pandas DataFrame with contents to display
     parent : QWidget | None
         Parent Widget (QWidget or inherited) or None if there is no parent
     title : str | None
         An optional title
-    verbose : bool
-        Set True to see debugging for signals
 
     Notes
     -----
     If you change the Reference to data outside of this class,
     give the changed DataFrame to replace_data to update this widget
     """
 
-    def __init__(self, data=None, parent=None, title=None, verbose=False):
+    def __init__(self, data=None, parent=None, title=None):
         super().__init__(
             model=FileManagementModel(data),
             view=QTableView(),
             parent=parent,
             title=title,
             resize_rows=True,
             resize_columns=True,
-            verbose=verbose,
         )
 
 
 class DictTree(Base):
-    def __init__(self, data, drag_drop=False, parent=None, title=None, verbose=False):
+    def __init__(self, data, drag_drop=False, parent=None, title=None):
         super().__init__(
             model=TreeModel(data),
             view=QTreeView(),
             drag_drop=drag_drop,
             parent=parent,
             title=title,
-            verbose=verbose,
         )
 
 
 class ComboBox(QComboBox):
     def __init__(self, scrollable=False, **kwargs):
         self.scrollable = scrollable
         super().__init__(**kwargs)
@@ -1375,20 +1326,18 @@
         items,
         properties,
         assignments,
         properties_editable=False,
         parent=None,
         title=None,
         subtitles=None,
-        verbose=False,
     ):
         super().__init__(parent)
         self.title = title
         self.subtitles = subtitles
-        self.verbose = verbose
 
         self.items = items
         self.props = properties
         self.assignments = assignments
         self.props_editable = properties_editable
 
         self.init_ui()
@@ -1403,32 +1352,29 @@
             subtitle1, subtitle2 = None, None
 
         self.items_w = CheckDictList(
             self.items,
             self.assignments,
             extended_selection=True,
             title=subtitle1,
-            verbose=self.verbose,
         )
         self.items_w.selectionChanged.connect(self.items_selected)
         list_layout.addWidget(self.items_w)
 
         if self.props_editable:
             self.props_w = EditList(
                 self.props,
                 extended_selection=False,
                 title=subtitle2,
-                verbose=self.verbose,
             )
         else:
             self.props_w = SimpleList(
                 self.props,
                 extended_selection=False,
                 title=subtitle2,
-                verbose=self.verbose,
             )
         list_layout.addWidget(self.props_w)
         layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
         assign_bt = QPushButton("Assign")
         assign_bt.setSizePolicy(QSizePolicy.Fixed, QSizePolicy.Fixed)
@@ -1470,14 +1416,135 @@
         # Inform Model in CheckDict about change
         self.items_w.content_changed()
 
     def show_assignments(self):
         SimpleDialog(EditDict(self.assignments), parent=self, modal=False)
 
 
+class TimedMessageBox(QMessageBox):
+    def __init__(
+        self, timeout=10, step_length=1000, title=None, text=None, *args, **kwargs
+    ):
+        super().__init__(*args, **kwargs)
+
+        if title is not None:
+            self.setWindowTitle(title)
+        if text is not None:
+            self.setText(text)
+
+        self._got_clicked = False
+        self.buttonClicked.connect(lambda: setattr(self, "_got_clicked", True))
+
+        self.timeout = timeout
+        self._update_timeout_text()
+
+        # Start timer
+        self.timer = QTimer()
+        self.timer.timeout.connect(self.countdown)
+        self.timer.start(step_length)
+
+    def _update_timeout_text(self):
+        text = self.text()
+        match = re.match(r"(.*)\nTimeout: \d+", text)
+        if match:
+            text = match.group(1)
+        self.setText(f"{text}\nTimeout: {self.timeout}")
+
+    def countdown(self):
+        self._update_timeout_text()
+        self.timeout -= 1
+        if self.timeout <= 0:
+            self.timer.stop()
+            if self.defaultButton() is not None:
+                self.defaultButton().click()
+            else:
+                self.close()
+
+    def _static_setup(icon, timeout, parent, title, text, buttons, defaultButton):
+        cls = TimedMessageBox(
+            timeout=timeout,
+            title=title,
+            text=text,
+            icon=icon,
+            parent=parent,
+        )
+
+        cls._update_timeout_text()
+        cls.setStandardButtons(buttons)
+        cls.setDefaultButton(defaultButton)
+        ans = cls.exec()
+
+        # Make sure ans is the default button if timeout is reached
+        if not cls._got_clicked:
+            ans = cls.defaultButton()
+
+        return ans
+
+    @staticmethod
+    def critical(
+        timeout=10,
+        parent=None,
+        title=None,
+        text=None,
+        buttons=QMessageBox.Ok,
+        defaultButton=QMessageBox.NoButton,
+    ):
+        return TimedMessageBox._static_setup(
+            QMessageBox.Critical, timeout, parent, title, text, buttons, defaultButton
+        )
+
+    @staticmethod
+    def information(
+        timeout=10,
+        parent=None,
+        title=None,
+        text=None,
+        buttons=QMessageBox.Ok,
+        defaultButton=QMessageBox.NoButton,
+    ):
+        return TimedMessageBox._static_setup(
+            QMessageBox.Information,
+            timeout,
+            parent,
+            title,
+            text,
+            buttons,
+            defaultButton,
+        )
+
+    @staticmethod
+    def question(
+        timeout=10,
+        parent=None,
+        title=None,
+        text=None,
+        buttons=QMessageBox.Yes | QMessageBox.No,
+        defaultButton=QMessageBox.No,
+    ):
+        return TimedMessageBox._static_setup(
+            QMessageBox.Question, timeout, parent, title, text, buttons, defaultButton
+        )
+
+    @staticmethod
+    def warning(
+        timeout=10,
+        parent=None,
+        title=None,
+        text=None,
+        buttons=QMessageBox.Ok,
+        defaultButton=QMessageBox.NoButton,
+    ):
+        return TimedMessageBox._static_setup(
+            QMessageBox.Warning, timeout, parent, title, text, buttons, defaultButton
+        )
+
+
+# ToDo: Proper testing
+# Testing all signals properly emitted (also on row add/remove)
+# Testing when _data is empty and get-Data, what happens?
 class AllBaseWidgets(QWidget):
     def __init__(self):
         super().__init__()
 
         self.exlist = ["Athena", "Hephaistos", "Zeus", "Ares", "Aphrodite", "Poseidon"]
         self.exattributes = ["strong", "smart", "bossy", "fishy"]
         self.exassignments = {
@@ -1523,38 +1590,34 @@
             "AssignWidget": [self.exlist, self.exattributes, self.exassignments],
         }
 
         self.widget_kwargs = {
             "SimpleList": {
                 "extended_selection": True,
                 "title": "BaseList",
-                "verbose": True,
             },
             "EditList": {
                 "ui_button_pos": "bottom",
                 "extended_selection": True,
                 "title": "EditList",
-                "verbose": True,
             },
-            "CheckList": {"one_check": False, "title": "CheckList", "verbose": True},
+            "CheckList": {"one_check": False, "title": "CheckList"},
             "CheckDictList": {
                 "extended_selection": True,
                 "title": "CheckDictList",
-                "verbose": True,
             },
-            "CheckDictEditList": {"title": "CheckDictEditList", "verbose": True},
-            "SimpleDict": {"title": "BaseDict", "verbose": True},
-            "EditDict": {"ui_button_pos": "left", "title": "EditDict", "verbose": True},
-            "SimplePandasTable": {"title": "BasePandasTable", "verbose": True},
-            "EditPandasTable": {"title": "EditPandasTable", "verbose": True},
-            "DictTree": {"title": "BaseDictTree", "verbose": True},
+            "CheckDictEditList": {"title": "CheckDictEditList"},
+            "SimpleDict": {"title": "BaseDict"},
+            "EditDict": {"ui_button_pos": "left", "title": "EditDict"},
+            "SimplePandasTable": {"title": "BasePandasTable"},
+            "EditPandasTable": {"title": "EditPandasTable"},
+            "DictTree": {"title": "BaseDictTree"},
             "AssignWidget": {
                 "properties_editable": True,
                 "title": "AssignWidget",
-                "verbose": True,
             },
         }
 
         self.tab_widget = QTabWidget()
 
         self.init_ui()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/dialogs.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/dialogs.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from collections import Counter
 from importlib import resources
 from pathlib import Path
 
-import mne
-from PyQt5.QtWidgets import (
+from qtpy.QtWidgets import (
     QDialog,
     QGridLayout,
     QLabel,
     QListView,
     QPushButton,
     QSizePolicy,
     QTextEdit,
     QVBoxLayout,
     QWidget,
     QComboBox,
     QMessageBox,
 )
 
+from mne_pipeline_hd import extra
 from mne_pipeline_hd.gui.base_widgets import SimpleList, SimpleDialog
 from mne_pipeline_hd.gui.gui_utils import set_ratio_geometry
 from mne_pipeline_hd.gui.models import CheckListModel
 from mne_pipeline_hd.pipeline.loading import MEEG
 from mne_pipeline_hd.pipeline.project import Project
 
 
@@ -170,14 +170,15 @@
 
         close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
         layout.addWidget(close_bt, 1, 0, 1, 2)
 
         self.setLayout(layout)
 
+    # ToDo: Just parse/reformat repr(info) instead of rewriting all keys
     def meeg_selected(self, meeg_name):
         # Get size in Mebibytes of all files associated to this
         meeg = MEEG(meeg_name, self.mw.ct)
         info = meeg.load_info()
         fp = meeg.file_parameters
         meeg.get_existing_paths()
         other_infos = dict()
@@ -194,23 +195,21 @@
         if sizes_sum / 1024 < 1000:
             other_infos["size"] = f"{int(sizes_sum / 1024)}"
             size_unit = "KB"
         else:
             other_infos["size"] = f"{int(sizes_sum / 1024 ** 2)}"
             size_unit = "MB"
 
-        ch_type_counter = Counter(
-            [mne.io.pick.channel_type(info, idx) for idx in range(len(info["chs"]))]
-        )
+        ch_type_counter = Counter(info.get_channel_types())
         other_infos["ch_types"] = ", ".join(
             [f"{key}: {value}" for key, value in ch_type_counter.items()]
         )
 
         key_list = [
-            ("no_files", "Size of all associated files"),
+            ("no_files", "Number associated files"),
             ("size", "Size of all associated files", size_unit),
             ("proj_name", "Project-Name"),
             ("experimenter", "Experimenter"),
             ("line_freq", "Powerline-Frequency", "Hz"),
             ("sfreq", "Samplerate", "Hz"),
             ("highpass", "Highpass", "Hz"),
             ("lowpass", "Lowpass", "Hz"),
@@ -251,83 +250,109 @@
         layout.addWidget(QLabel("From:"), 0, 0)
         self.from_cmbx = QComboBox()
         self.from_cmbx.addItems(self.ct.projects)
         self.from_cmbx.currentTextChanged.connect(self.from_selected)
         layout.addWidget(self.from_cmbx, 1, 0)
         layout.addWidget(QLabel("Parameter-Preset:"), 2, 0)
         self.from_pp_cmbx = QComboBox()
+        self.from_pp_cmbx.currentTextChanged.connect(self.from_pp_selected)
         layout.addWidget(self.from_pp_cmbx, 3, 0)
 
         layout.addWidget(QLabel("To:"), 0, 1)
         self.to_cmbx = QComboBox()
         self.to_cmbx.currentTextChanged.connect(self.to_selected)
-        self.to_cmbx.setEnabled(False)
         layout.addWidget(self.to_cmbx, 1, 1)
         layout.addWidget(QLabel("Parameter-Preset:"), 2, 1)
         self.to_pp_cmbx = QComboBox()
         self.to_pp_cmbx.setEditable(True)
         layout.addWidget(self.to_pp_cmbx, 3, 1)
 
+        layout.addWidget(QLabel("Parameter:"), 4, 0, 1, 2)
+        self.param_cmbx = QComboBox()
+        layout.addWidget(self.param_cmbx, 5, 0, 1, 2)
+
         copy_bt = QPushButton("Copy")
         copy_bt.clicked.connect(self.copy_parameters)
-        layout.addWidget(copy_bt, 4, 0)
+        layout.addWidget(copy_bt, 6, 0)
         close_bt = QPushButton("Close")
         close_bt.clicked.connect(self.close)
-        layout.addWidget(close_bt, 4, 1)
+        layout.addWidget(close_bt, 6, 1)
 
         widget.setLayout(layout)
         super().__init__(
             widget,
             parent=main_win,
             title="Copy Parameters between Projects",
             window_title="Copy Parameters",
             show_close_bt=False,
         )
 
+        # Initialize with first from-entry
+        self.from_selected(self.from_cmbx.currentText())
+
     def _get_p_presets(self, pr_name):
         if self.ct.pr.name == pr_name:
             project = self.ct.pr
         else:
             project = Project(self.ct, pr_name)
 
         return list(project.parameters.keys())
 
+    def from_pp_selected(self, from_pp_name):
+        if from_pp_name:
+            self.param_cmbx.clear()
+            params = list(
+                Project(self.ct, self.from_cmbx.currentText())
+                .parameters[from_pp_name]
+                .keys()
+            )
+            params.insert(0, "<all>")
+            self.param_cmbx.addItems(params)
+
     def from_selected(self, from_name):
         if from_name:
-            self.to_cmbx.setEnabled(True)
             self.to_cmbx.clear()
             self.to_cmbx.addItems([p for p in self.ct.projects if p != from_name])
 
             self.from_pp_cmbx.clear()
             self.from_pp_cmbx.addItems(self._get_p_presets(from_name))
 
+            self.from_pp_selected(self.from_pp_cmbx.currentText())
+
     def to_selected(self, to_name):
         if to_name:
             self.to_pp_cmbx.clear()
             self.to_pp_cmbx.addItems(self._get_p_presets(to_name))
 
     def copy_parameters(self):
         from_name = self.from_cmbx.currentText()
         from_pp = self.from_pp_cmbx.currentText()
         to_name = self.to_cmbx.currentText()
         to_pp = self.to_pp_cmbx.currentText()
+        param = self.param_cmbx.currentText()
+        if param == "<all>":
+            param = None
         if from_name and to_name:
-            self.ct.copy_parameters_between_projects(from_name, from_pp, to_name, to_pp)
+            self.ct.copy_parameters_between_projects(
+                from_name, from_pp, to_name, to_pp, param
+            )
         if to_name == self.ct.pr.name:
             self.main_win.parameters_dock.redraw_param_widgets()
         QMessageBox().information(
-            self, "Finished", f"Parameters copied from {from_name} " f"to {to_name}!"
+            self,
+            "Finished",
+            f"Copied parameter '{param}' from {from_name} to {to_name}!",
         )
 
 
 class AboutDialog(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
-        with resources.open_text("mne_pipeline_hd.resource", "license.txt") as file:
+        with open(resources.files(extra) / "license.txt", "r") as file:
             license_text = file.read()
         license_text = license_text.replace("\n", "<br>")
         text = (
             "<h1>MNE-Pipeline HD</h1>"
             "<b>A Pipeline-GUI for MNE-Python</b><br>"
             "(originally developed for MEG-Lab Heidelberg)<br>"
             "<i>Development was initially inspired by: "
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/education_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/education_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 """
 
 import json
 from os import makedirs
 from os.path import isdir, join
 from shutil import copytree
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
+from qtpy import compat
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QFont
+from qtpy.QtWidgets import (
     QComboBox,
-    QFileDialog,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMainWindow,
     QSizePolicy,
     QTextBrowser,
@@ -234,15 +234,15 @@
         current_page = self.page_list.get_current()
         text = self.page_edit.toPlainText()
         self._set_page_display(text)
         if text != "":
             self.edu["tour"][current_page] = text
 
     def load_edu_file(self):
-        file_path = QFileDialog().getOpenFileName(self, directory=self.edu_folder)[0]
+        file_path = compat.getopenfilename(self, directory=self.edu_folder)[0]
         if file_path != "":
             with open(file_path, "r") as file:
                 self.edu = json.load(file)
 
         self.update_ui()
 
     def save_edu_file(self):
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/function_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/function_widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,33 +13,32 @@
 from importlib import util
 from os import mkdir
 from os.path import isdir, isfile, join
 from pathlib import Path
 from types import FunctionType
 
 import pandas as pd
-from PyQt5.QtCore import QSize, Qt
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
+from qtpy import compat
+from qtpy.QtCore import QSize, Qt
+from qtpy.QtGui import QFont, QTextDocument
+from qtpy.QtWidgets import (
     QButtonGroup,
     QComboBox,
     QDialog,
-    QFileDialog,
     QFormLayout,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QListView,
     QListWidget,
     QListWidgetItem,
     QMessageBox,
     QPushButton,
     QSizePolicy,
-    QStyle,
     QTabWidget,
     QVBoxLayout,
     QGridLayout,
     QProgressBar,
     QCheckBox,
 )
 
@@ -134,19 +133,16 @@
 
         self.restart_bt = QPushButton("Restart")
         self.restart_bt.setFont(QFont("AnyStyle", 14))
         self.restart_bt.setIcon(get_std_icon("SP_BrowserReload"))
         self.restart_bt.clicked.connect(self.restart)
         bt_layout.addWidget(self.restart_bt)
 
-        if QS().value("use_qthread"):
-            self.reload_chbx = None
-        else:
-            self.reload_chbx = QCheckBox("Reload Modules")
-            bt_layout.addWidget(self.reload_chbx)
+        self.reload_chbx = QCheckBox("Reload Modules")
+        bt_layout.addWidget(self.reload_chbx)
 
         self.autoscroll_bt = QPushButton("Auto-Scroll")
         self.autoscroll_bt.setCheckable(True)
         self.autoscroll_bt.setChecked(True)
         self.autoscroll_bt.setIcon(get_std_icon("SP_DialogOkButton"))
         self.autoscroll_bt.clicked.connect(self.toggle_autoscroll)
         bt_layout.addWidget(self.autoscroll_bt)
@@ -178,14 +174,16 @@
     def restart(self):
         # Reinitialize controller
         self.init_controller()
 
         # ToDo: MP
         # if self.reload_chbx and self.reload_chbx.isChecked():
         #     init_mp_pool()
+        if self.reload_chbx.isChecked():
+            self.mw.ct.reload_modules()
 
         # Clear Console-Widget
         self.console_widget.clear()
 
         # Redo References to display-widgets
         self.object_model._data = self.rc.all_objects
         self.object_model.layoutChanged.emit()
@@ -201,18 +199,24 @@
 
     def toggle_autoscroll(self, state):
         if state:
             self.console_widget.set_autoscroll(True)
         else:
             self.console_widget.set_autoscroll(False)
 
-    def show_error(self, current, _):
+    def show_error(self, current, previous):
         self.console_widget.set_autoscroll(False)
         self.autoscroll_bt.setChecked(False)
-        self.console_widget.scrollToAnchor(str(self.rc.errors[current][1]))
+        if current < previous:
+            self.console_widget.find(
+                f"Error-No. {self.rc.errors[current][1]} (above)",
+                QTextDocument.FindBackward,
+            )
+        else:
+            self.console_widget.find(f"Error-No. {self.rc.errors[current][1]} (above)")
 
     def closeEvent(self, event):
         self.mw.pipeline_running = False
         event.accept()
 
 
 class EditGuiArgsDlg(QDialog):
@@ -225,14 +229,15 @@
         if self.cf.current_parameter:
             covered_params = [
                 "data",
                 "name",
                 "alias",
                 "default",
                 "param_unit",
+                "none_select",
                 "description",
             ]
             # Get possible default GUI-Args additional to those
             # covered by the Main-GUI
             gui_type = self.cf.add_pd_params.loc[self.cf.current_parameter, "gui_type"]
             if pd.notna(gui_type):
                 gui_handle = getattr(parameter_widgets, gui_type)
@@ -906,28 +911,28 @@
         self.group_cmbx.insertItems(0, tab_set | tab_set2)
 
     def populate_guitype_cmbx(self):
         self.guitype_cmbx.insertItems(0, self.available_param_guis)
 
     def target_cmbx_changed(self, idx):
         if self.current_function:
-            self.add_pd_funcs.loc[
-                self.current_function, "target"
-            ] = self.target_cmbx.itemText(idx)
+            self.add_pd_funcs.loc[self.current_function, "target"] = (
+                self.target_cmbx.itemText(idx)
+            )
             self.target_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def tab_cmbx_changed(self, idx):
         # Insert changes from other functions if edited
         self.populate_tab_cmbx()
         self.tab_cmbx.setCurrentIndex(idx)
         if self.current_function:
-            self.add_pd_funcs.loc[
-                self.current_function, "tab"
-            ] = self.tab_cmbx.itemText(idx)
+            self.add_pd_funcs.loc[self.current_function, "tab"] = (
+                self.tab_cmbx.itemText(idx)
+            )
             self.tab_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
             self.check_func_setup()
 
     def tab_cmbx_edited(self, text):
         if self.current_function and text != "":
             self.add_pd_funcs.loc[self.current_function, "tab"] = text
             self.tab_chkl.setPixmap(self.yes_icon.pixmap(QSize(16, 16)))
@@ -1028,35 +1033,35 @@
         # Clear Function- and Parameter-DataFrame
         self.add_pd_funcs.drop(index=self.add_pd_funcs.index, inplace=True)
         self.add_pd_params.drop(index=self.add_pd_funcs.index, inplace=True)
         self.clear_func_items()
         self.clear_param_items()
 
         # Returns tuple of files-list and file-type
-        cf_path_string = QFileDialog.getOpenFileName(
+        cf_path_string = compat.getopenfilename(
             self,
             "Choose the Python-File containing your function to import",
-            filter="Python-File (*.py)",
+            filters="Python-File (*.py)",
         )[0]
         if cf_path_string:
             self.file_path = Path(cf_path_string)
             ImportFuncs(self)
 
     def edit_functions(self):
         # Clear Function- and Parameter-DataFrame
         self.add_pd_funcs.drop(index=self.add_pd_funcs.index, inplace=True)
         self.add_pd_params.drop(index=self.add_pd_funcs.index, inplace=True)
         self.clear_func_items()
         self.clear_param_items()
 
         # Returns tuple of files-list and file-type
-        cf_path_string = QFileDialog.getOpenFileName(
+        cf_path_string = compat.getopenfilename(
             self,
             "Choose the Python-File containing the functions to edit",
-            filter="Python-File (*.py)",
+            filters="Python-File (*.py)",
             directory=self.ct.custom_pkg_path,
         )[0]
         if cf_path_string:
             self.file_path = Path(cf_path_string)
             ImportFuncs(self, edit_existing=True)
 
     def test_param_gui(self, default_string, gui_type, gui_args=None):
@@ -1230,15 +1235,15 @@
             ErrorDialog(err, self)
         else:
             for func_key in self.module.__dict__:
                 func = self.module.__dict__[func_key]
                 # Only functions are allowed
                 # (Classes should be called from function!)
                 if (
-                    type(func) == FunctionType
+                    isinstance(func, FunctionType)
                     and func.__module__ == self.module.__name__
                 ):
                     # Check, if function is already existing
                     if func_key in self.cf.exst_functions:
                         if (
                             self.edit_existing
                             and func_key in self.cf.add_pd_funcs.index
@@ -1330,17 +1335,17 @@
                             if pd.notna(
                                 self.cf.add_pd_params.loc[param_key, "functions"]
                             ):
                                 self.cf.add_pd_params.loc[
                                     param_key, "functions"
                                 ] += func_key
                             else:
-                                self.cf.add_pd_params.loc[
-                                    param_key, "functions"
-                                ] = func_key
+                                self.cf.add_pd_params.loc[param_key, "functions"] = (
+                                    func_key
+                                )
                         else:
                             self.cf.add_pd_params.loc[param_key, "functions"] = func_key
                     else:
                         self.cf.add_pd_params.loc[param_key, "functions"] = func_key
 
             self.cf.param_exst_dict[func_key] = existing_parameters
 
@@ -1692,28 +1697,28 @@
         self.mw.redraw_func_and_param()
         event.accept()
 
 
 class AddKwargs(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
-        self.mw = main_win
+        self.ct = main_win.ct
         self.current_func = None
 
         self.init_ui()
         self.open()
 
     def init_ui(self):
         layout = QVBoxLayout()
 
         list_layout = QHBoxLayout()
         func_list = CheckDictList(
             self.ct.pd_funcs.index,
             self.ct.pr.add_kwargs,
-            no_bt=QStyle.SP_MessageBoxQuestion,
+            no_bt="SP_MessageBoxQuestion",
         )
         func_list.currentChanged.connect(self.func_selected)
         list_layout.addWidget(func_list)
 
         self.kwarg_dict = EditDict(
             dict(),
             title="Add Keyword-Arguments:",
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/gui_utils.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/gui_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,58 +6,59 @@
 """
 
 import io
 import logging
 import multiprocessing
 import sys
 import traceback
+from contextlib import contextmanager
 from inspect import signature
 
-from PyQt5.QtCore import (
+from qtpy.QtCore import (
     QObject,
     QProcess,
     QRunnable,
     QThreadPool,
     Qt,
-    pyqtSignal,
-    pyqtSlot,
+    Signal,
+    Slot,
     QTimer,
 )
-from PyQt5.QtGui import QFont, QTextCursor
-from PyQt5.QtWidgets import (
+from qtpy.QtGui import QFont, QTextCursor
+from qtpy.QtWidgets import (
     QApplication,
-    QDesktopWidget,
     QDialog,
     QHBoxLayout,
     QLabel,
     QMessageBox,
     QProgressBar,
     QPushButton,
     QTextEdit,
     QVBoxLayout,
     QStyle,
     QInputDialog,
+    QPlainTextEdit,
 )
 
 from mne_pipeline_hd import _object_refs
-from mne_pipeline_hd.pipeline.pipeline_utils import QS
+from mne_pipeline_hd.pipeline.pipeline_utils import QS, logger
 
 
 def center(widget):
     qr = widget.frameGeometry()
-    cp = QDesktopWidget().availableGeometry().center()
+    cp = QApplication.primaryScreen().availableGeometry().center()
     qr.moveCenter(cp)
     widget.move(qr.topLeft())
 
 
 def set_ratio_geometry(size_ratio, widget=None):
     if not isinstance(size_ratio, tuple):
         size_ratio = (size_ratio, size_ratio)
     wratio, hratio = size_ratio
-    desk_geometry = QApplication.instance().desktop().availableGeometry()
+    desk_geometry = QApplication.primaryScreen().availableGeometry()
     width = int(desk_geometry.width() * wratio)
     height = int(desk_geometry.height() * hratio)
     if widget:
         widget.resize(width, height)
 
     return width, height
 
@@ -146,23 +147,43 @@
     """Checks if a QApplication instance is available
     and shows the Error-Dialog.
      If unavailable (non-console application), log an additional notice.
     """
     if QApplication.instance() is not None:
         ErrorDialog(exc_str, title="A unexpected error occurred")
     else:
-        logging.debug("No QApplication instance available.")
+        logger().debug("No QApplication instance available.")
+
+
+def gui_error_decorator(func):
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except Exception:
+            exc_tuple = get_exception_tuple()
+            ErrorDialog(exc_tuple)
+
+    return wrapper
+
+
+@contextmanager
+def gui_error():
+    try:
+        yield
+    except Exception:
+        exc_tuple = get_exception_tuple()
+        ErrorDialog(exc_tuple)
 
 
 # ToDo: Test
 class UncaughtHook(QObject):
     """This class is a modified version
     of https://timlehr.com/python-exception-hooks-with-qt-message-box/"""
 
-    _exception_caught = pyqtSignal(object)
+    _exception_caught = Signal(object)
 
     def __init__(self, *args, **kwargs):
         super(UncaughtHook, self).__init__(*args, **kwargs)
 
         # connect signal to execute the message box function
         # always on main thread
         self._exception_caught.connect(show_error_dialog)
@@ -179,15 +200,15 @@
             traceback.print_exception(exc_type, exc_value, exc_traceback)
             exc_info = (exc_type, exc_value, exc_traceback)
             exc_str = (
                 exc_type.__name__,
                 exc_value,
                 "".join(traceback.format_tb(exc_traceback)),
             )
-            logging.critical(
+            logger().critical(
                 f"Uncaught exception:\n"
                 f"{exc_str[0]}: {exc_str[1]}\n"
                 f"{exc_str[2]}",
                 exc_info=exc_info,
             )
 
             # trigger showing of error-dialog
@@ -195,87 +216,86 @@
 
 
 class CodeEditor(QTextEdit):
     def __init__(self, parent=None):
         super().__init__(parent)
 
 
-def _html_compatible(text):
-    text = text.replace("<", "&lt;")
-    text = text.replace(">", "&gt;")
-    text = text.replace("\n", "<br>")
-    text = text.replace("\x1b", "")
-
-    return text
-
-
-class ConsoleWidget(QTextEdit):
+class ConsoleWidget(QPlainTextEdit):
     """A Widget displaying formatted stdout/stderr-output"""
 
     def __init__(self):
         super().__init__()
 
         self.setReadOnly(True)
         self.autoscroll = True
-
-        self.buffer_time = 10
+        self.is_progress = False
 
         # Buffer to avoid crash for too many inputs
         self.buffer = list()
+        self.buffer_time = 50
         self.buffer_timer = QTimer()
         self.buffer_timer.timeout.connect(self.write_buffer)
         self.buffer_timer.start(self.buffer_time)
 
-    def _add_html(self, text):
-        self.insertHtml(text)
-        if self.autoscroll:
-            self.ensureCursorVisible()
-
     def write_buffer(self):
+        if self.is_progress:
+            # Delete last line
+            cursor = self.textCursor()
+            # Avoid having no break between progress and text
+            # Remove last line
+            cursor.select(QTextCursor.LineUnderCursor)
+            cursor.removeSelectedText()
+            cursor.deletePreviousChar()
+            self.is_progress = False
+
         if len(self.buffer) > 0:
-            text, kind = self.buffer.pop(0)
-            if kind == "html":
-                self._add_html(text)
-
-            elif kind == "progress":
-                text = text.replace("\r", "")
-                text = _html_compatible(text)
-                text = f'<font color="green">{text}</font>'
-                # Delete last line
-                cursor = self.textCursor()
-                cursor.select(QTextCursor.LineUnderCursor)
-                cursor.removeSelectedText()
-                self._add_html(text)
-
-            elif kind == "stdout":
-                text = _html_compatible(text)
-                self._add_html(text)
-
-            elif kind == "stderr":
-                # weird characters in some progress are excluded
-                # (e.g. from autoreject)
-                if "\x1b" not in text:
-                    text = _html_compatible(text)
-                    text = f'<font color="red">{text}</font>'
-                    self._add_html(text)
+            text_list = self.buffer.copy()
+            self.buffer.clear()
+            text = "".join(text_list)
+            # Remove last break because of appendHtml above
+            if text[-4:] == "<br>":
+                text = text[:-4]
+            self.appendHtml(text)
+            if self.autoscroll:
+                self.ensureCursorVisible()
 
     def set_autoscroll(self, autoscroll):
         self.autoscroll = autoscroll
 
     def write_html(self, text):
-        self.buffer.append((text, "html"))
+        self.buffer.append(text)
+
+    def _html_compatible(self, text):
+        text = text.replace("<", "&lt;")
+        text = text.replace(">", "&gt;")
+        text = text.replace("\n", "<br>")
+        text = text.replace("\x1b", "")
+
+        if text[:1] == "\r":
+            self.is_progress = True
+            text = text.replace("\r", "")
+            # Avoid having no break between progress and text
+            text = f"<font color='green'>{text}</font>"
+            if len(self.buffer) > 0:
+                if self.buffer[-1][:20] == "<font color='green'>":
+                    self.buffer.pop(-1)
+        return text
 
     def write_stdout(self, text):
-        self.buffer.append((text, "stdout"))
+        text = self._html_compatible(text)
+        self.buffer.append(text)
 
     def write_stderr(self, text):
-        self.buffer.append((text, "stderr"))
-
-    def write_progress(self, text):
-        self.buffer.append((text, "progress"))
+        text = self._html_compatible(text)
+        if text[-4:] == "<br>":
+            text = f'<font color="red">{text[:-4]}</font><br>'
+        else:
+            text = f'<font color="red">{text}</font>'
+        self.buffer.append(text)
 
     # Make sure cursor is not moved
     def mousePressEvent(self, event):
         event.accept()
 
     def mouseDoubleClickEvent(self, event):
         event.accept()
@@ -287,66 +307,60 @@
 
     def __init__(self):
         super().__init__()
 
         # Connect custom stdout and stderr to display-function
         sys.stdout.signal.text_written.connect(self.write_stdout)
         sys.stderr.signal.text_written.connect(self.write_stderr)
-        # Handle progress-bars
-        sys.stdout.signal.text_updated.connect(self.write_progress)
-        sys.stderr.signal.text_updated.connect(self.write_progress)
 
 
 class StreamSignals(QObject):
-    text_updated = pyqtSignal(str)
-    text_written = pyqtSignal(str)
+    text_written = Signal(str)
 
 
-# ToDo: Buffering and halting signal-emission
-#  (continue writing to sys.__stdout__/__stderr__)
-#  when no accepted/printed-signal is coming back from receiving Widget
 class StdoutStderrStream(io.TextIOBase):
     def __init__(self, kind):
         super().__init__()
         self.signal = StreamSignals()
-        if kind == "stdout":
+        self.kind = kind
+        if self.kind == "stdout":
             self.original_stream = sys.__stdout__
-        else:
+        elif self.kind == "stderr":
             self.original_stream = sys.__stderr__
+        else:
+            self.original_stream = None
 
     def write(self, text):
-        # Still send output to the command-line
-        self.original_stream.write(text)
-
-        # Get progress-text with '\r' as prefix
-        if text[:1] == "\r":
-            self.signal.text_updated.emit(text)
-        else:
-            self.signal.text_written.emit(text)
+        if self.original_stream is not None:
+            # Still send output to the command-line
+            self.original_stream.write(text)
+        # Emit signal to display in GUI
+        self.signal.text_written.emit(text)
 
     def flush(self):
-        self.original_stream.flush()
+        if self.original_stream is not None:
+            self.original_stream.flush()
 
 
 class WorkerSignals(QObject):
     """Class for standard Worker-Signals"""
 
     # Emitted when the function finished and returns the return-value
-    finished = pyqtSignal(object)
+    finished = Signal(object)
 
     # Emitted when the function throws an error and returns
     # a tuple with information about the error
     # (see get_exception_tuple)
-    error = pyqtSignal(object)
+    error = Signal(object)
 
     # Can be passed to function to be emitted when a part
     # of the function progresses to update a Progress-Bar
-    pgbar_max = pyqtSignal(int)
-    pgbar_n = pyqtSignal(int)
-    pgbar_text = pyqtSignal(str)
+    pgbar_max = Signal(int)
+    pgbar_n = Signal(int)
+    pgbar_text = Signal(str)
 
     # Only an attribute which is stored here to maintain
     # reference when passing it to the function
     was_canceled = False
 
 
 class Worker(QRunnable):
@@ -370,15 +384,15 @@
 
         # Store constructor arguments (re-used for processing)
         self.function = function
         self.args = args
         self.kwargs = kwargs
         self.signals = WorkerSignals()
 
-    @pyqtSlot()
+    @Slot()
     def run(self):
         """
         Initialise the runner function with passed args, kwargs.
         """
         # Add signals to kwargs if in parameters of function
         if "worker_signals" in signature(self.function).parameters:
             self.kwargs["worker_signals"] = self.signals
@@ -399,32 +413,34 @@
         self.signals.was_canceled = True
 
 
 # ToDo: Make PyQt-independent with tqdm
 class WorkerDialog(QDialog):
     """A Dialog for a Worker doing a function"""
 
-    thread_finished = pyqtSignal(object)
+    thread_finished = Signal(object)
 
     def __init__(
         self,
         parent,
         function,
         show_buttons=False,
         show_console=False,
         close_directly=True,
         blocking=False,
+        return_exception=False,
         title=None,
         **kwargs,
     ):
         super().__init__(parent)
 
         self.show_buttons = show_buttons
         self.show_console = show_console
         self.close_directly = close_directly
+        self.return_exception = return_exception
         self.title = title
         self.is_finished = False
         self.return_value = None
 
         # Initialize worker
         self.worker = Worker(function, **kwargs)
         self.worker.signals.finished.connect(self.on_thread_finished)
@@ -477,14 +493,16 @@
 
             layout.addLayout(bt_layout)
 
         self.setLayout(layout)
 
     def on_thread_finished(self, return_value):
         # Store return value to send it when user closes the dialog
+        if type(return_value) == ExceptionTuple and not self.return_exception:
+            return_value = None
         self.return_value = return_value
         self.is_finished = True
         if self.show_buttons:
             self.close_bt.setEnabled(True)
         if self.close_directly:
             self.close()
 
@@ -510,26 +528,27 @@
             event.accept()
         else:
             QMessageBox.warning(
                 self,
                 "Closing not possible!",
                 "You can't close this Dialog before this Thread finished!",
             )
+            event.ignore()
 
 
 # ToDo: WIP
 class QProcessWorker(QObject):
     """A worker for QProcess."""
 
     # Send stdout from current process.
-    stdoutSignal = pyqtSignal(str)
+    stdoutSignal = Signal(str)
     # Send stderr from curren process.
-    stderrSignal = pyqtSignal(str)
+    stderrSignal = Signal(str)
     # Send when all processes from commands are finished.
-    finished = pyqtSignal()
+    finished = Signal()
 
     def __init__(self, commands, printtostd=True):
         """
         Parameters
         ----------
         commands : str, list
             Provide a command or a list of commands.
@@ -708,16 +727,16 @@
             if parent:
                 QMessageBox().warning(
                     parent,
                     "Input required!",
                     "You need to provide an appropriate input to proceed!",
                 )
             else:
-                print(
-                    "Warning: Input required! "
-                    "You need to provide an appropriate input to proceed!"
+                logger().warning(
+                    "Input required! You need to provide "
+                    "an appropriate input to proceed!"
                 )
             user_input = get_user_input_string(prompt, title, force)
         else:
             user_input = None
 
     return user_input
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/loading_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/loading_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
-
 import os
 import re
 import shutil
 import time
 from collections import Counter
 from functools import partial
 from os.path import exists, isfile, join
 from pathlib import Path
 
 import mne
 import numpy as np
 import pandas as pd
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QPixmap
-from PyQt5.QtWidgets import (
+from matplotlib import pyplot as plt
+from qtpy import compat
+from qtpy.QtCore import Qt
+from qtpy.QtWidgets import (
     QAbstractItemView,
     QCheckBox,
     QComboBox,
     QDialog,
     QDockWidget,
-    QFileDialog,
     QGridLayout,
     QHBoxLayout,
     QHeaderView,
     QLabel,
     QLineEdit,
     QListWidget,
     QListWidgetItem,
@@ -43,21 +42,22 @@
     QTreeWidget,
     QTreeWidgetItem,
     QVBoxLayout,
     QWidget,
     QWizard,
     QWizardPage,
 )
-from matplotlib import pyplot as plt
 
-from mne_pipeline_hd.functions.operations import (
+from mne_pipeline_hd.functions.operations import find_bads
+from mne_pipeline_hd.functions.plot import (
     plot_ica_components,
+    plot_ica_sources,
     plot_ica_overlay,
     plot_ica_properties,
-    plot_ica_sources,
+    plot_raw,
 )
 from mne_pipeline_hd.gui.base_widgets import (
     AssignWidget,
     CheckDictList,
     CheckList,
     EditDict,
     EditList,
@@ -67,39 +67,39 @@
     SimplePandasTable,
 )
 from mne_pipeline_hd.gui.gui_utils import (
     ErrorDialog,
     Worker,
     WorkerDialog,
     center,
-    get_exception_tuple,
     set_ratio_geometry,
     get_user_input_string,
+    gui_error,
 )
 from mne_pipeline_hd.gui.models import AddFilesModel
 from mne_pipeline_hd.gui.parameter_widgets import ComboGui
 from mne_pipeline_hd.pipeline.loading import FSMRI, Group, MEEG
-from mne_pipeline_hd.pipeline.pipeline_utils import compare_filep
+from mne_pipeline_hd.pipeline.pipeline_utils import compare_filep, QS, logger
 
 
-def index_parser(index, all_items):
+def index_parser(index, all_items, groups=None):
     """
     Parses indices from a index-string in all_items
 
     Parameters
     ----------
     index: str
         A string which contains information about indices
     all_items
         All items
     Returns
     -------
 
     """
-    run = list()
+    indices = list()
     rm = list()
 
     try:
         if index == "":
             return [], []
         elif "all" in index:
             if "," in index:
@@ -110,60 +110,64 @@
                         x = x[1:]
                         for n in range(int(x), int(y) + 1):
                             rm.append(n)
                     elif "!" in sp:
                         rm.append(int(sp[1:]))
                     elif "all" in sp:
                         for i in range(len(all_items)):
-                            run.append(i)
+                            indices.append(i)
             else:
-                run = [x for x in range(len(all_items))]
+                indices = [x for x in range(len(all_items))]
 
         elif "," in index and "-" in index:
             z = index.split(",")
             for i in z:
                 if "-" in i and "!" not in i:
                     x, y = i.split("-")
                     for n in range(int(x), int(y) + 1):
-                        run.append(n)
+                        indices.append(n)
                 elif "!" not in i:
-                    run.append(int(i))
+                    indices.append(int(i))
                 elif "!" in i and "-" in i:
                     x, y = i.split("-")
                     x = x[1:]
                     for n in range(int(x), int(y) + 1):
                         rm.append(n)
                 elif "!" in i:
                     rm.append(int(i[1:]))
 
         elif "-" in index and "," not in index:
             x, y = index.split("-")
-            run = [x for x in range(int(x), int(y) + 1)]
+            indices = [x for x in range(int(x), int(y) + 1)]
 
         elif "," in index and "-" not in index:
             splits = index.split(",")
             for sp in splits:
                 if "!" in sp:
                     rm.append(int(sp))
                 else:
-                    run.append(int(sp))
+                    indices.append(int(sp))
+
+        elif groups is not None and index in groups:
+            files = [x for x in all_items if x in groups[index]]
+            indices = [all_items.index(x) for x in files]
 
         else:
             if len(all_items) < int(index) or int(index) < 0:
-                run = []
+                indices = []
             else:
-                run = [int(index)]
+                indices = [int(index)]
 
-        run = [i for i in run if i not in rm]
-        files = [x for (i, x) in enumerate(all_items) if i in run]
+        indices = [i for i in indices if i not in rm]
+        files = np.asarray(all_items)[indices].tolist()
 
-        return files, run
+        return files
 
     except ValueError:
-        return [], []
+        return []
 
 
 class RemoveDialog(QDialog):
     def __init__(self, parentw, mode):
         super().__init__(parentw)
         self.pw = parentw
         self.pr = parentw.mw.ct.pr
@@ -227,15 +231,16 @@
             "Examples:\n"
             "'5' (One File)\n"
             "'1,7,28' (Several Files)\n"
             "'1-5' (From File x to File y)\n"
             "'1-4,7,20-26' (The last two combined)\n"
             "'1-20,!4-6' (1-20 except 4-6)\n"
             "'all' (All files in file_list.py)\n"
-            "'all,!4-6' (All files except 4-6)"
+            "'all,!4-6' (All files except 4-6)\n"
+            "<group-name> (All files in group)"
         )
 
         if self.meeg_view:
             # MEEG-List + Index-Line-Edit
             meeg_widget = QWidget()
             meeg_layout = QVBoxLayout()
             self.meeg_list = CheckList(
@@ -323,21 +328,23 @@
 
     def reload_dock(self):
         self.init_ui()
         self.central_widget.show()
 
     def select_meeg(self):
         index = self.meeg_ledit.text()
-        self.mw.ct.pr.sel_meeg, idxs = index_parser(index, self.mw.ct.pr.all_meeg)
+        self.mw.ct.pr.sel_meeg = index_parser(
+            index, self.mw.ct.pr.all_meeg, self.mw.ct.pr.all_groups
+        )
         # Replace _checked in CheckListModel because of rereferencing above
         self.meeg_list.replace_checked(self.mw.ct.pr.sel_meeg)
 
     def select_fsmri(self):
         index = self.fsmri_ledit.text()
-        self.mw.ct.pr.sel_fsmri, idxs = index_parser(index, self.mw.ct.pr.all_fsmri)
+        self.mw.ct.pr.sel_fsmri = index_parser(index, self.mw.ct.pr.all_fsmri)
         # Replace _checked in CheckListModel because of rereferencing above
         self.fsmri_list.replace_checked(self.mw.ct.pr.sel_fsmri)
 
     def _rename_meeg(self):
         current_meeg = self.meeg_list.get_current()
         if current_meeg is not None:
             meeg = MEEG(current_meeg, self.mw.ct)
@@ -688,33 +695,34 @@
     def get_files_path(self):
         filter_list = [
             f"{self.supported_file_types[key]} (*{key})"
             for key in self.supported_file_types
         ]
         filter_list.insert(0, "All Files (*.*)")
         filter_qstring = ";;".join(filter_list)
-        files_list = QFileDialog.getOpenFileNames(
-            self, "Choose raw-file/s to import", filter=filter_qstring
+        files_list = compat.getopenfilenames(
+            self, "Choose raw-file/s to import", filters=filter_qstring
         )[0]
         self.insert_files(files_list)
 
     def get_folder_path(self):
-        folder_path = QFileDialog.getExistingDirectory(
+        folder_path = compat.getexistingdirectory(
             self,
             "Choose a folder to import your raw-Files from " "(including subfolders)",
         )
         if folder_path != "":
             # create a list of file and obj directories
             # names in the given directory
             list_of_file = os.walk(folder_path)
             files_list = list()
+            file_types = [x for x in self.supported_file_types if x != ".*"]
             # Iterate over all the entries
             for dirpath, _, filenames in list_of_file:
                 for file in filenames:
-                    for file_type in self.supported_file_types:
+                    for file_type in file_types:
                         match = re.match(rf"(.+)({file_type})", file)
                         if match and len(match.group()) == len(file):
                             # Make sure, that no files from Pipeline-Analysis
                             # are included
                             if not any(
                                 x in file
                                 for x in [
@@ -765,15 +773,15 @@
             if not worker_signals.was_canceled:
                 worker_signals.pgbar_text.emit(f"Copying {name}")
                 file_path = self.pd_files.loc[idx, "Path"]
                 is_erm = self.pd_files.loc[idx, "Empty-Room?"]
                 self.pr.add_meeg(name, file_path, is_erm)
                 worker_signals.pgbar_n.emit(n + 1)
             else:
-                print("Canceled Loading")
+                logger().info("Canceled Loading")
                 break
 
     def add_files_starter(self):
         WorkerDialog(
             self, self.add_files, show_buttons=True, show_console=True, blocking=True
         )
 
@@ -912,49 +920,53 @@
             self.list_widget.edit(i)
             new_name = self.list_widget.item(i).text()
             repl_ind = self.files.index(old_name)
             self.folders[repl_ind] = new_name
             self.paths[new_name] = self.paths[old_name]
 
     def import_mri_subject(self):
-        folder_path = QFileDialog.getExistingDirectory(
+        folder_path = compat.getexistingdirectory(
             self, "Choose a folder with a subject's Freesurfe-Segmentation"
         )
 
         if folder_path != "":
             if exists(join(folder_path, "surf")):
                 fsmri = Path(folder_path).name
                 if fsmri not in self.pr.all_fsmri and fsmri not in self.folders:
                     self.folders.append(fsmri)
                     self.paths.update({fsmri: folder_path})
                     self.populate_list_widget()
                 else:
-                    print(f"{fsmri} already existing in {self.ct.subjects_dir}")
+                    logger().info(f"{fsmri} already existing in {self.ct.subjects_dir}")
             else:
-                print("Selected Folder doesn't seem to " "be a Freesurfer-Segmentation")
+                logger().warning(
+                    "Selected Folder doesn't seem to " "be a Freesurfer-Segmentation"
+                )
 
     def import_mri_subjects(self):
-        parent_folder = QFileDialog.getExistingDirectory(
+        parent_folder = compat.getexistingdirectory(
             self, "Choose a folder containting several " "Freesurfer-Segmentations"
         )
         folder_list = sorted(
             [f for f in os.listdir(parent_folder) if not f.startswith(".")],
             key=str.lower,
         )
 
         for fsmri in folder_list:
             folder_path = join(parent_folder, fsmri)
             if exists(join(folder_path, "surf")):
                 if fsmri not in self.pr.all_fsmri and fsmri not in self.folders:
                     self.folders.append(fsmri)
                     self.paths.update({fsmri: folder_path})
                 else:
-                    print(f"{fsmri} already existing in {self.ct.subjects_dir}")
+                    logger().info(f"{fsmri} already existing in {self.ct.subjects_dir}")
             else:
-                print("Selected Folder doesn't seem to be " "a Freesurfer-Segmentation")
+                logger().warning(
+                    "Selected Folder doesn't seem to be " "a Freesurfer-Segmentation"
+                )
         self.populate_list_widget()
 
     def add_mri_subjects(self, worker_signals):
         worker_signals.pgbar_max.emit(len(self.folders))
         for n, name in enumerate(self.folders):
             if not worker_signals.was_canceled:
                 worker_signals.pgbar_text.emit(f"Copying {name}")
@@ -1058,14 +1070,30 @@
 
         layout = QVBoxLayout()
         self.sub_dict_w = FileDictWidget(main_win, mode)
         layout.addWidget(self.sub_dict_w)
         self.setLayout(layout)
 
 
+class FindBadsDialog(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+        self.pw = parent
+
+        self.values
+
+        self.init_ui()
+        self.open()
+
+    def init_ui(self):
+        layout = QVBoxLayout()
+
+        self.setLayout(layout)
+
+
 class CopyBadsDialog(QDialog):
     def __init__(self, parent_w):
         super().__init__(parent_w)
 
         self.parent_w = parent_w
         self.all_files = parent_w.pr.all_meeg + parent_w.pr.all_erm
         self.bad_channels_dict = parent_w.pr.meeg_bad_channels
@@ -1130,14 +1158,15 @@
         :param main_win: The parent-window for the dialog
         """
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
         self.setWindowTitle("Assign bad_channels for your files")
+        self.all_files = self.pr.all_meeg + self.pr.all_erm
         self.bad_chkbts = dict()
         self.info_dict = dict()
         self.current_obj = None
         self.raw = None
         self.raw_fig = None
 
         self.init_ui()
@@ -1160,14 +1189,18 @@
         # Add Buttons
         self.bt_layout = QHBoxLayout()
 
         plot_bt = QPushButton("Plot raw")
         plot_bt.clicked.connect(self.plot_raw_bad)
         self.bt_layout.addWidget(plot_bt)
 
+        find_bads_bt = QPushButton("Find bads")
+        find_bads_bt.clicked.connect(self.find_bads)
+        self.bt_layout.addWidget(find_bads_bt)
+
         copy_bt = QPushButton("Copy Bads")
         copy_bt.clicked.connect(partial(CopyBadsDialog, self))
         self.bt_layout.addWidget(copy_bt)
 
         self.save_raw_annot = QCheckBox("Save Annotations")
         self.bt_layout.addWidget(self.save_raw_annot)
 
@@ -1249,73 +1282,65 @@
             if hasattr(self.raw_fig, "canvas"):
                 plt.close(self.raw_fig)
             else:
                 self.raw_fig.close()
 
         self.make_bad_chbxs()
 
-    def _assign_bad_channels(self, bad_channels):
-        # Directly replace value in bad_channels_dict
-        # (needed for first-time assignment)
-        self.current_obj.pr.meeg_bad_channels[self.current_obj.name] = bad_channels
-        # Restore/Establish reference to direct object-attribute
-        self.current_obj.bad_channels = bad_channels
-        self.files_widget.content_changed()
-
     def bad_ckbx_assigned(self):
         bad_channels = [ch for ch in self.bad_chkbts if self.bad_chkbts[ch].isChecked()]
-        self._assign_bad_channels(bad_channels)
+        self.current_obj.set_bad_channels(bad_channels)
 
     def set_chkbx_enable(self, enable):
         for chkbx in self.bad_chkbts:
             self.bad_chkbts[chkbx].setEnabled(enable)
 
-    def get_selected_bads(self, _):
-        # In-Place-Operations to maintain reference
-        # from current_obj to meeg_bad_channels
-        bad_channels = self.raw.info["bads"]
-        self._assign_bad_channels(bad_channels)
+    def get_selected_bads(self, _, meeg, raw, raw_type):
+        self.current_obj.set_bad_channels(raw.info["bads"])
         self.update_selection()
         self.set_chkbx_enable(True)
 
         if self.save_raw_annot.isChecked():
             WorkerDialog(
                 self,
-                self.current_obj.save_raw,
-                raw=self.raw,
+                meeg.save,
+                data_type=raw_type,
+                data=raw,
                 show_console=True,
                 title="Saving raw with Annotations",
             )
 
         self.raw_fig = None
 
     def plot_raw_bad(self):
         # Disable CheckBoxes to avoid confusion
         # (Bad-Selection only goes unidirectional from Plot>GUI)
         self.set_chkbx_enable(False)
 
         plot_dialog = QDialog(self)
         plot_dialog.setWindowTitle("Opening raw-Plot...")
         plot_dialog.open()
-        self.raw = self.current_obj.load_raw()
-        try:
-            events = self.current_obj.load_events()
-        except FileNotFoundError:
-            events = None
-        self.raw_fig = self.raw.plot(
-            events=events, n_channels=30, bad_color="red", title=self.current_obj.name
-        )
-        if hasattr(self.raw_fig, "canvas"):
-            # Connect Closing of Matplotlib-Figure
-            # to assignment of bad-channels
-            self.raw_fig.canvas.mpl_connect("close_event", self.get_selected_bads)
-        else:
-            self.raw_fig.gotClosed.connect(partial(self.get_selected_bads, None))
+
+        plot_raw(self.current_obj, show_plots=True, close_func=self.get_selected_bads)
         plot_dialog.close()
 
+    def find_bads(self):
+        wd = WorkerDialog(
+            self,
+            find_bads,
+            meeg=self.current_obj,
+            n_jobs=QS().value("n_jobs"),
+            show_console=True,
+            show_buttons=True,
+            close_directly=False,
+            return_exception=False,
+            title="Finding bads with maxwell filter...",
+        )
+        wd.thread_finished.connect(self.update_selection)
+
     def resizeEvent(self, event):
         if self.current_obj:
             self.make_bad_chbxs()
             self.update_selection()
         event.accept()
 
     def closeEvent(self, event):
@@ -1401,21 +1426,22 @@
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
 
         self.name = None
         self.event_id = dict()
+        self.queries = dict()
         self.labels = list()
         self.checked_labels = list()
 
         self.layout = QVBoxLayout()
         self.init_ui()
 
-        self.open()
+        self.show()
 
     def init_ui(self):
         list_layout = QHBoxLayout()
 
         self.files = CheckDictList(
             self.pr.all_meeg, self.pr.meeg_event_id, title="Files"
         )
@@ -1439,14 +1465,23 @@
         event_id_layout.addWidget(self.event_id_widget)
 
         self.event_id_label = QLabel()
         event_id_layout.addWidget(self.event_id_label)
 
         list_layout.addLayout(event_id_layout)
 
+        self.query_widget = EditDict(
+            self.queries, ui_buttons=True, title="Metadata-Queries"
+        )
+        self.query_widget.setToolTip(
+            "Add Metadata-Queries as value for trials which are named with key"
+        )
+        self.query_widget.dataChanged.connect(self.update_check_list)
+        list_layout.addWidget(self.query_widget)
+
         self.check_widget = CheckList(title="Select IDs")
         list_layout.addWidget(self.check_widget)
 
         self.layout.addLayout(list_layout)
 
         bt_layout = QHBoxLayout()
 
@@ -1470,64 +1505,96 @@
         """Get unique event-ids from events"""
         if self.name in self.pr.meeg_event_id:
             self.event_id = self.pr.meeg_event_id[self.name]
         else:
             self.event_id = dict()
         self.event_id_widget.replace_data(self.event_id)
 
+        meeg = MEEG(self.name, self.ct, suppress_warnings=True)
         try:
             # Load events from File
-            meeg = MEEG(self.name, self.ct, suppress_warnings=True)
             events = meeg.load_events()
         except FileNotFoundError:
-            self.event_id_label.setText(f"No events found for {self.name}")
+            label_text = f"No events found for {self.name}"
         else:
-            ids = np.unique(events[:, 2])
-            self.event_id_label.setText(f"events found: {ids}")
+            label_text = f"events found: {np.unique(events[:, 2])}"
+
+        try:
+            # Load epochs from File
+            epochs = meeg.load_epochs()
+            assert epochs.metadata is not None
+        except (FileNotFoundError, AssertionError):
+            self.query_widget.setEnabled(False)
+            label_text += "\nNo metadata found"
+        else:
+            self.query_widget.setEnabled(True)
+            label_text += "\nMetadata found"
+
+        self.event_id_label.setText(label_text)
 
     def save_event_id(self):
         if self.name:
             if len(self.event_id) > 0:
                 # Write Event-ID to Project
                 self.pr.meeg_event_id[self.name] = self.event_id
 
-                # Get selected Trials and write them to meeg.pr
-                self.pr.sel_event_id[self.name] = self.checked_labels
+                # Get selected Trials, add queries and write them to meeg.pr
+                sel_event_id = dict()
+                for label in self.checked_labels:
+                    if label in self.queries:
+                        sel_event_id[label] = self.queries[label]
+                    else:
+                        sel_event_id[label] = None
+                self.pr.sel_event_id[self.name] = sel_event_id
 
     def file_selected(self, current, _):
         """Called when File from file_widget is selected"""
         # Save event_id for previous file
         self.save_event_id()
 
         # Get event-id for selected file and update widget
         self.name = current
         self.get_event_id()
 
         # Load checked trials
         if self.name in self.pr.sel_event_id:
-            self.checked_labels = self.pr.sel_event_id[self.name]
+            # Update query-widget
+            if self.query_widget.isEnabled():
+                sel_trials = self.pr.sel_event_id[self.name]
+                if not isinstance(sel_trials, dict):
+                    sel_trials = {k: None for k in sel_trials}
+                self.queries = {k: v for k, v in sel_trials.items() if v is not None}
+                self.query_widget.replace_data(self.queries)
+            # Legacy to allow reading lists before
+            # they were changed to dicts for queries
+            self.checked_labels = list(self.pr.sel_event_id[self.name])
         else:
             self.checked_labels = list()
         self.update_check_list()
 
+    # ToDo: Make all combinations possible
     def update_check_list(self):
+        self.labels = [k for k in self.queries.keys()]
         # Get selectable trials and update widget
         prelabels = [i.split("/") for i in self.event_id.keys() if i != ""]
         if len(prelabels) > 0:
             # Concatenate all lists
             conc_labels = prelabels[0]
             if len(prelabels) > 1:
                 for item in prelabels[1:]:
                     conc_labels += item
             # Make sure that only unique labels exist
-            self.labels = list(set(conc_labels))
+            self.labels += list(set(conc_labels))
 
             # Make sure, that only trials, which exist in event_id exist
             for chk_label in self.checked_labels:
-                if not any(chk_label in key for key in self.event_id):
+                if (
+                    not any(chk_label in key for key in self.event_id)
+                    and chk_label not in self.queries
+                ):
                     self.checked_labels.remove(chk_label)
         else:
             self.labels = list()
 
         self.check_widget.replace_data(self.labels)
         self.check_widget.replace_checked(self.checked_labels)
 
@@ -1545,14 +1612,18 @@
         event.accept()
 
 
 class EvIDApply(QDialog):
     def __init__(self, parent):
         super().__init__(parent)
         self.p = parent
+
+        # Save to make sel_event_id available in apply_evid
+        self.p.save_event_id()
+
         self.apply_to = list()
 
         self.layout = QVBoxLayout()
         self.init_ui()
 
         self.open()
 
@@ -1576,16 +1647,16 @@
         self.layout.addLayout(bt_layout)
         self.setLayout(self.layout)
 
     def apply_evid(self):
         for file in self.apply_to:
             # Avoid with copy that CheckList-Model changes selected
             # for all afterwards (same reference)
-            self.p.pr.meeg_event_id[file] = self.p.event_id.copy()
-            self.p.pr.sel_event_id[file] = self.p.checked_labels.copy()
+            self.p.pr.meeg_event_id[file] = self.p.pr.meeg_event_id[self.p.name].copy()
+            self.p.pr.sel_event_id[file] = self.p.pr.sel_event_id[self.p.name].copy()
 
 
 class CopyTrans(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
@@ -1717,15 +1788,15 @@
             obj_pd_time = self.pd_fsmri_time
             obj_pd_size = self.pd_fsmri_size
         else:
             obj_list = self.pr.all_groups
             obj_pd = self.pd_group
             obj_pd_time = self.pd_group_time
             obj_pd_size = self.pd_group_size
-        print(f"Loading {kind}")
+        logger().debug(f"Loading {kind}")
 
         for obj_name in obj_list:
             if kind == "MEEG":
                 obj = MEEG(obj_name, self.ct)
             elif kind == "FSMRI":
                 obj = FSMRI(obj_name, self.ct)
             else:
@@ -1759,21 +1830,21 @@
                         self.param_results[obj_name][path_type] = result_dict
 
                         # Change status of path_type
                         # from object if there are conflicts
                         for parameter in result_dict:
                             if isinstance(result_dict[parameter], tuple):
                                 if result_dict[parameter][2]:
-                                    obj_pd.loc[
-                                        obj_name, path_type
-                                    ] = "critical_conflict"
+                                    obj_pd.loc[obj_name, path_type] = (
+                                        "critical_conflict"
+                                    )
                                 else:
-                                    obj_pd.loc[
-                                        obj_name, path_type
-                                    ] = "possible_conflict"
+                                    obj_pd.loc[obj_name, path_type] = (
+                                        "possible_conflict"
+                                    )
 
     def open_prog_dlg(self):
         # Create Progress-Dialog
         self.prog_bar = QProgressBar()
         self.prog_bar.setMinimum(0)
         self.prog_bar.setMaximum(3)
 
@@ -2051,33 +2122,26 @@
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
         self.pr = main_win.ct.pr
         self.current_obj = None
         self.parameters = dict()
         self.chkbxs = dict()
-        self.offline_plots = [
-            "plot_ica_components",
-            "plot_ica_sources",
-            "plot_ica_scores",
-            "plot_ica_overlay",
-        ]
-        self.selected_offline_plots = list()
 
         self.max_width, self.max_height = set_ratio_geometry(0.8)
         self.setMaximumSize(self.max_width, self.max_height)
 
         self.init_ui()
         self.show()
 
     def init_ui(self):
         self.main_layout = QVBoxLayout()
         list_layout = QHBoxLayout()
 
-        self.file_list = CheckDictList(self.pr.all_meeg, self.pr.ica_exclude)
+        self.file_list = CheckDictList(self.pr.all_meeg, self.pr.meeg_ica_exclude)
         self.file_list.currentChanged.connect(self.obj_selected)
         list_layout.addWidget(self.file_list)
 
         # Add Checkboxes for Components
         comp_scroll = QScrollArea()
         comp_widget = QWidget()
         self.comp_chkbx_layout = QGridLayout()
@@ -2090,59 +2154,53 @@
             self.chkbxs[idx] = chkbx
             self.comp_chkbx_layout.addWidget(chkbx, idx // 5, idx % 5)
 
         comp_widget.setLayout(self.comp_chkbx_layout)
         comp_scroll.setWidget(comp_widget)
         list_layout.addWidget(comp_scroll)
 
-        # Todo: Fix Offline-Plots Layout
-        # offline_plot_list = CheckList(self.offline_plots,
-        #                               self.selected_offline_plots,
-        #                               title='Offline-Plots to select')
-        # list_layout.addWidget(offline_plot_list)
-
         bt_layout = QVBoxLayout()
 
         plot_comp_bt = QPushButton("Plot Components")
         plot_comp_bt.clicked.connect(self.plot_components)
         bt_layout.addWidget(plot_comp_bt)
 
         # Create Parameter-GUI which stores parameter in dictionary
         # (not the same as project.parameters)
         ica_source_data_param = ComboGui(
-            self.parameters,
-            "ica_source_data",
-            options=[
-                "raw",
-                "raw_filtered",
-                "epochs",
-                "epochs_eog",
-                "epochs (ECG)",
-                "Evokeds",
-                "Evokeds (EOG)",
-                "Evokeds (ECG)",
-            ],
+            data=self.parameters,
+            name="ica_source_data",
+            options={
+                "raw": "Raw (unfiltered)",
+                "raw_filtered": "Raw (filtered)",
+                "epochs": "Epochs",
+                "epochs_eog": "Epochs (EOG)",
+                "epochs_ecg": "Epochs (ECG)",
+                "evoked": "Evoked",
+                "evoked_eog": "Evoked (EOG)",
+                "evoked_ecg": "Evoked (ECG)",
+            },
             default="raw_filtered",
         )
         bt_layout.addWidget(ica_source_data_param)
 
         plot_source_bt = QPushButton("Plot Source")
         plot_source_bt.clicked.connect(self.plot_sources)
         bt_layout.addWidget(plot_source_bt)
 
         ica_overlay_data_param = ComboGui(
-            self.parameters,
-            "ica_overlay_data",
-            options=[
-                "raw",
-                "raw_filtered",
-                "Evokeds",
-                "Evokeds (EOG)",
-                "Evokeds (ECG)",
-            ],
+            data=self.parameters,
+            name="ica_overlay_data",
+            options={
+                "raw": "Raw (unfiltered)",
+                "raw_filtered": "Raw (filtered)",
+                "evoked": "Evoked",
+                "evoked_eog": "Evoked (EOG)",
+                "evoked_ecg": "Evoked (ECG)",
+            },
             default="raw_filtered",
         )
         bt_layout.addWidget(ica_overlay_data_param)
 
         plot_overlay_bt = QPushButton("Plot Overlay")
         plot_overlay_bt.clicked.connect(self.plot_overlay)
         bt_layout.addWidget(plot_overlay_bt)
@@ -2162,190 +2220,112 @@
         list_layout.addLayout(bt_layout)
         self.main_layout.addLayout(list_layout)
 
         self.setLayout(self.main_layout)
 
     def update_chkbxs(self):
         # Check, if object is already in ica_exclude
-        if self.current_obj.name in self.pr.ica_exclude:
-            selected_components = self.pr.ica_exclude[self.current_obj.name]
+        if self.current_obj.name in self.pr.meeg_ica_exclude:
+            selected_components = self.pr.meeg_ica_exclude[self.current_obj.name]
         else:
             selected_components = list()
 
         # Clear all checkboxes
         for idx in self.chkbxs:
             self.chkbxs[idx].setChecked(False)
 
         # Select components
         for idx in selected_components:
             if idx in self.chkbxs:
                 self.chkbxs[idx].setChecked(True)
             else:
                 # Remove idx if not in range(n_components)
-                self.pr.ica_exclude[self.current_obj.name].remove(idx)
-
-    def update_plots(self):
-        # Remove old layout with plots
-        if self.main_layout.count() > 1:
-            old_layout = self.main_layout.itemAt(self.main_layout.count() - 1)
-            self.main_layout.removeItem(old_layout)
-            for sub_layout in [
-                old_layout.itemAt(idx).layout() for idx in range(old_layout.count())
-            ]:
-                for widget in [
-                    sub_layout.itemAt(idx).widget() for idx in range(sub_layout.count())
-                ]:
-                    widget.deleteLater()
-            del old_layout
-
-        plot_layout = QHBoxLayout()
-
-        for plot_func in self.selected_offline_plots:
-            sub_plot_layout = QVBoxLayout()
-            try:
-                plot_paths = self.current_obj.plot_files[plot_func]
-            except KeyError:
-                continue
-            else:
-                for plot_path in plot_paths:
-                    plot_path = join(self.pr.figures_path, plot_path)
-                    pixmap = QPixmap(plot_path)
-                    label = QLabel()
-                    label.setScaledContents(True)
-                    label.setPixmap(pixmap)
-                    sub_plot_layout.addWidget(label)
-            plot_layout.addLayout(sub_plot_layout)
-
-        self.main_layout.addLayout(plot_layout)
+                self.pr.meeg_ica_exclude[self.current_obj.name].remove(idx)
 
     def obj_selected(self, current_name):
         self.current_obj = MEEG(current_name, self.ct)
         self.update_chkbxs()
-        self.update_plots()
 
     def component_selected(self):
         if self.current_obj:
-            self.pr.ica_exclude[self.current_obj.name] = [
+            self.pr.meeg_ica_exclude[self.current_obj.name] = [
                 idx for idx in self.chkbxs if self.chkbxs[idx].isChecked()
             ]
         self.file_list.content_changed()
 
     def set_chkbx_enable(self, enable):
         for chkbx in self.chkbxs:
             self.chkbxs[chkbx].setEnabled(enable)
 
-    def get_selected_components(self, ica, _):
+    def get_selected_components(self, _, meeg, ica):
         self.set_chkbx_enable(True)
-        self.pr.ica_exclude[self.current_obj.name] = ica.exclude
+        meeg.set_ica_exclude(ica.exclude)
         self.update_chkbxs()
         self.file_list.content_changed()
 
     def plot_components(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
             dialog.setWindowTitle("Opening...")
             dialog.open()
-            try:
-                figs, ica = plot_ica_components(meeg=self.current_obj, show_plots=True)
-                if not isinstance(figs, list):
-                    figs = [figs]
-                for fig in figs:
-                    fig.canvas.mpl_connect(
-                        "close_event", partial(self.get_selected_components, ica)
-                    )
-            except Exception:
-                err_tuple = get_exception_tuple()
-                QMessageBox.critical(
-                    self,
-                    "An Error ocurred!",
-                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
+            with gui_error():
+                plot_ica_components(
+                    meeg=self.current_obj,
+                    show_plots=True,
+                    close_func=self.get_selected_components,
                 )
-                self.set_chkbx_enable(True)
-            finally:
-                dialog.close()
+            dialog.close()
 
     def plot_sources(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
             self.set_chkbx_enable(False)
             dialog = QDialog(self)
             dialog.setWindowTitle("Opening...")
             dialog.open()
-            try:
-                figs, ica = plot_ica_sources(
+
+            with gui_error():
+                plot_ica_sources(
                     meeg=self.current_obj,
                     ica_source_data=self.parameters["ica_source_data"],
                     show_plots=True,
+                    close_func=self.get_selected_components,
                 )
-                if not isinstance(figs, list):
-                    figs = [figs]
-                for fig in figs:
-                    fig.canvas.mpl_connect(
-                        "close_event", partial(self.get_selected_components, ica)
-                    )
-            except Exception:
-                err_tuple = get_exception_tuple()
-                QMessageBox.critical(
-                    self,
-                    "An Error ocurred!",
-                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
-                )
-                self.set_chkbx_enable(False)
-            finally:
-                dialog.close()
+            dialog.close()
 
     def plot_overlay(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
-            self.set_chkbx_enable(False)
             dialog = QDialog(self)
             dialog.setWindowTitle("Opening...")
             dialog.open()
-            try:
+
+            with gui_error():
                 plot_ica_overlay(
                     meeg=self.current_obj,
                     ica_overlay_data=self.parameters["ica_overlay_data"],
                     show_plots=True,
                 )
-            except Exception:
-                err_tuple = get_exception_tuple()
-                QMessageBox.critical(
-                    self,
-                    "An Error ocurred!",
-                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
-                )
-                self.set_chkbx_enable(False)
-            finally:
-                dialog.close()
+            dialog.close()
 
     def plot_properties(self):
         if self.current_obj:
             # Disable CheckBoxes to avoid confusion
             # (Bad-Selection only goes unidirectional from Plot>GUI)
-            self.set_chkbx_enable(False)
             dialog = QDialog(self)
             dialog.setWindowTitle("Opening...")
             dialog.open()
-            try:
+            with gui_error():
                 plot_ica_properties(meeg=self.current_obj, show_plots=True)
-            except Exception:
-                err_tuple = get_exception_tuple()
-                QMessageBox.critical(
-                    self,
-                    "An Error ocurred!",
-                    f"{err_tuple[0]}: {err_tuple[1]}\n" f"{err_tuple[2]}",
-                )
-                self.set_chkbx_enable(False)
-            finally:
-                dialog.close()
+            dialog.close()
 
 
 class ReloadRaw(QDialog):
     def __init__(self, main_win):
         super().__init__(main_win)
         self.mw = main_win
         self.ct = main_win.ct
@@ -2370,21 +2350,21 @@
 
         self.setLayout(layout)
 
     def reload_raw(self, selected_raw, raw_path):
         meeg = MEEG(selected_raw, self.ct)
         raw = mne.io.read_raw(raw_path, preload=True)
         meeg.save_raw(raw)
-        print(f"Reloaded raw for {selected_raw}")
+        logger().info(f"Reloaded raw for {selected_raw}")
 
     def start_reload(self):
         # Not with partial because otherwise the clicked-arg
         # from clicked goes into *args
         selected_raw = self.raw_list.get_current()
-        raw_path = QFileDialog.getOpenFileName(self, "Select raw for Reload")[0]
+        raw_path = compat.getopenfilename(self, "Select raw for Reload")[0]
         if raw_path:
             WorkerDialog(
                 self,
                 self.reload_raw,
                 selected_raw=selected_raw,
                 raw_path=raw_path,
                 show_console=True,
@@ -2414,15 +2394,15 @@
             if isinstance(self.common_types, list):
                 self.common_types = type_set
             else:
                 self.common_types = self.common_types & type_set
             self.export_paths[meeg_name] = meeg.existing_paths
 
     def _get_destination(self):
-        dest = QFileDialog.getExistingDirectory(self, "Select Destination-Folder")[0]
+        dest = compat.getexistingdirectory(self, "Select Destination-Folder")[0]
         if dest:
             self.dest_path = dest
 
     def _init_ui(self):
         layout = QVBoxLayout()
         self.dest_label = QLabel("<No Destination-Folder set>")
         layout.addWidget(self.dest_label)
@@ -2446,20 +2426,20 @@
         export_bt = QPushButton("Export")
         export_bt.clicked.connect(self.export_data)
         layout.addWidget(export_bt)
         self.setLayout(layout)
 
     def export_data(self):
         if self.dest_path:
-            print("Starting Export\n")
+            logger().info("Starting Export\n")
             for meeg_name, path_types in self.export_paths.items():
                 os.mkdir(join(self.dest_path, meeg_name))
                 for path_type in [pt for pt in path_types if pt in self.selected_types]:
                     paths = path_types[path_type]
                     for src_path in paths:
                         dest_name = Path(src_path).name
                         shutil.copy2(
                             src_path, join(self.dest_path, meeg_name, dest_name)
                         )
-                    print(f"\r{meeg_name}: Copying {path_type}...")
+                    logger().info(f"\r{meeg_name}: Copying {path_type}...")
         else:
             QMessageBox.warning(self, "Ups!", "Destination-Path not set!")
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/main_window.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
-
 import sys
 from functools import partial
 
 import mne
 import pandas as pd
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
+from qtpy import compat
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QFont
+from qtpy.QtWidgets import (
     QAction,
     QApplication,
     QComboBox,
-    QFileDialog,
     QGridLayout,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QMainWindow,
     QMessageBox,
     QPushButton,
@@ -28,15 +27,14 @@
     QSizePolicy,
     QTabWidget,
     QVBoxLayout,
     QWidget,
 )
 
 from mne_pipeline_hd import _object_refs
-from mne_pipeline_hd.functions.plot import close_all
 from mne_pipeline_hd.gui.dialogs import (
     QuickGuide,
     RawInfo,
     RemoveProjectsDlg,
     SysInfoMsg,
     AboutDialog,
     CopyParamsDialog,
@@ -75,28 +73,30 @@
     IntGui,
     ParametersDock,
     SettingsDlg,
 )
 from mne_pipeline_hd.gui.plot_widgets import PlotViewSelection
 from mne_pipeline_hd.gui.tools import DataTerminal
 from mne_pipeline_hd.pipeline.controller import Controller
+from mne_pipeline_hd.pipeline.function_utils import close_all
 from mne_pipeline_hd.pipeline.pipeline_utils import (
     restart_program,
     ismac,
     QS,
     _run_from_script,
     iswin,
+    logger,
 )
 
 
 class MainWindow(QMainWindow):
     # Define Main-Window-Signals to send into QThread
     # to control function execution
-    cancel_functions = pyqtSignal(bool)
-    plot_running = pyqtSignal(bool)
+    cancel_functions = Signal(bool)
+    plot_running = Signal(bool)
 
     def __init__(self, controller):
         super().__init__()
         _object_refs["main_window"] = self
         self.setWindowTitle("MNE-Pipeline HD")
 
         # Set QThread as default (ToDo: MP)
@@ -142,15 +142,15 @@
             f"Home-Path: {self.ct.home_path}, " f"Project: {self.pr.name}"
         )
 
     def change_home_path(self):
         # First save the former projects-data
         WorkerDialog(self, self.ct.save, blocking=True)
 
-        new_home_path = QFileDialog.getExistingDirectory(
+        new_home_path = compat.getexistingdirectory(
             self, "Change your Home-Path (top-level folder of Pipeline-Data)"
         )
         if new_home_path != "":
             try:
                 new_controller = Controller(new_home_path)
             except RuntimeError as err:
                 QMessageBox.critical(self, "Error with selected Home-Path", str(err))
@@ -198,14 +198,18 @@
         project = self.project_box.itemText(idx)
 
         # Change project
         self.pr = self.ct.change_project(project)
 
         self.update_project_ui()
 
+    def pr_rename(self):
+        self.ct.rename_project()
+        self.update_project_box()
+
     def pr_clean_fp(self):
         WorkerDialog(
             self,
             self.pr.clean_file_parameters,
             show_buttons=True,
             show_console=True,
             close_directly=False,
@@ -295,14 +299,15 @@
         prep_menu.addAction("MRI-Coregistration", mne.gui.coregistration)
         prep_menu.addAction("Copy Transformation", partial(CopyTrans, self))
 
         prep_menu.addSeparator()
 
         # Project
         project_menu = self.menuBar().addMenu("&Project")
+        project_menu.addAction("&Rename Project", self.pr_rename)
         project_menu.addAction("&Clean File-Parameters", self.pr_clean_fp)
         project_menu.addAction("&Clean Plot-Files", self.pr_clean_pf)
         project_menu.addAction(
             "&Copy Parameters between Projects", self.pr_copy_parameters
         )
 
         # Custom-Functions
@@ -549,15 +554,18 @@
                 self.tab_func_widget.addTab(tab, tab_name)
 
     def update_func_bts(self):
         # Remove tabs in tab_func_widget
         while self.tab_func_widget.count():
             tab = self.tab_func_widget.removeTab(0)
             if tab:
-                tab.deleteLater()
+                try:
+                    tab.deleteLater()
+                except RuntimeError:
+                    logger().debug("Tab already deleted")
         self.bt_dict = dict()
 
         self.add_func_bts()
 
     def redraw_func_and_param(self):
         self.update_func_bts()
         self.parameters_dock.redraw_param_widgets()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/models.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
-
 from ast import literal_eval
 from datetime import datetime
 
 import pandas as pd
-from PyQt5.QtCore import (
+from qtpy.QtCore import (
     QAbstractItemModel,
     QAbstractListModel,
     QAbstractTableModel,
     QModelIndex,
     Qt,
 )
-from PyQt5.QtGui import QBrush, QFont
+from qtpy.QtGui import QBrush, QFont
 
 from mne_pipeline_hd.gui.gui_utils import get_std_icon
+from mne_pipeline_hd.pipeline.pipeline_utils import logger
+
+
+# ToDo: Merge models and base widgets
 
 
 class BaseListModel(QAbstractListModel):
     """A basic List-Model
 
     Parameters
     ----------
@@ -40,14 +43,17 @@
         self.drag_drop = drag_drop
         if data is None:
             self._data = list()
         else:
             self._data = data
 
     def getData(self, index):
+        if len(self._data) == 0:
+            logger().debug("List is empty")
+            return None
         return self._data[index.row()]
 
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             if self.show_index:
                 return f"{index.row()}: {self.getData(index)}"
             else:
@@ -161,17 +167,14 @@
             self._data = data
 
         if checked is None:
             self._checked = list()
         else:
             self._checked = checked
 
-    def getChecked(self, index):
-        return self.checked[index.row()]
-
     def data(self, index, role=None):
         if role == Qt.DisplayRole:
             if self.show_index:
                 return f"{index.row()}: {self.getData(index)}"
             else:
                 return str(self.getData(index))
 
@@ -179,14 +182,16 @@
             if self.getData(index) in self._checked:
                 return Qt.Checked
             else:
                 return Qt.Unchecked
 
     def setData(self, index, value, role=None):
         if role == Qt.CheckStateRole:
+            # ToDo: This does not work under PySide6
+            #  since Qt.Checked returns no integer (only Qt.Checked.value)
             if value == Qt.Checked:
                 if self.one_check:
                     self._checked.clear()
                 self._checked.append(self.getData(index))
             else:
                 if self.getData(index) in self._checked:
                     self._checked.remove(self.getData(index))
@@ -349,14 +354,15 @@
     def rowCount(self, parent=None, *args, **kwargs):
         return len(self._data)
 
     def columnCount(self, parent=None, *args, **kwargs):
         return 2
 
 
+# ToDo: Somehow inputs are automatically sorted (annoyig, disable-toggle)
 class EditDictModel(BaseDictModel):
     """An editable model for Dictionaries
 
     Parameters
     ----------
     data : dict | OrderedDict | None
         Dictionary with keys and values to be displayed,
@@ -765,14 +771,16 @@
                     return Qt.Unchecked
 
     def setData(self, index, value, role=None):
         if (
             role == Qt.CheckStateRole
             and self._data.columns[index.column()] == "Empty-Room?"
         ):
+            # ToDo: This does not work under PySide6
+            #  since Qt.Checked returns no integer (only Qt.Checked.value)
             if value == Qt.Checked:
                 self._data.iloc[index.row(), index.column()] = 1
             else:
                 self._data.iloc[index.row(), index.column()] = 0
             self.dataChanged.emit(index, index, [role])
             return True
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/parameter_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/parameter_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 from ast import literal_eval
+from copy import copy
 from functools import partial
 
+import mne
 import numpy as np
 import pandas as pd
-from PyQt5.QtCore import Qt, pyqtSignal
-from PyQt5.QtGui import QFontDatabase, QFont, QPixmap
-from PyQt5.QtWidgets import (
+from mne_qt_browser._pg_figure import _get_color
+from qtpy import compat
+from qtpy.QtCore import Qt, Signal
+from qtpy.QtGui import QFontDatabase, QFont, QPixmap
+from qtpy.QtWidgets import (
     QCheckBox,
     QComboBox,
     QDialog,
     QDoubleSpinBox,
     QGridLayout,
     QGroupBox,
     QHBoxLayout,
@@ -29,16 +33,14 @@
     QWidget,
     QDockWidget,
     QTabWidget,
     QScrollArea,
     QMessageBox,
     QColorDialog,
 )
-from mne.viz import Brain
-from mne_qt_browser._pg_figure import _get_color
 from vtkmodules.vtkCommonCore import vtkCommand
 from vtkmodules.vtkRenderingCore import vtkCellPicker
 
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.gui.base_widgets import (
     CheckList,
     EditDict,
@@ -53,30 +55,31 @@
     WorkerDialog,
     get_exception_tuple,
     get_user_input_string,
     center,
 )
 from mne_pipeline_hd.pipeline.controller import Controller
 from mne_pipeline_hd.pipeline.loading import FSMRI
-from mne_pipeline_hd.pipeline.pipeline_utils import QS, iswin
+from mne_pipeline_hd.pipeline.pipeline_utils import QS, iswin, logger
 
 
+# ToDo: Unify None-select and more
 class Param(QWidget):
     """
     Base-Class Parameter-GUIs, not to be called directly
     Inherited Clases should have "Gui" in their name to get
     identified correctly.
 
     Attributes
     ----------
-    paramChanged : pyqtSignal
+    paramChanged : Signal
         This signal is emmited when the parameter changes.
     """
 
-    paramChanged = pyqtSignal(object)
+    paramChanged = Signal(object)
 
     def __init__(
         self,
         data,
         name,
         alias=None,
         default=None,
@@ -203,14 +206,18 @@
                 self.param_value = saved_value
                 self.save_param()
 
     def get_value(self):
         """This should be implemented for each widget"""
         pass
 
+    def set_value(self, value):
+        """This should be implemented for each widget"""
+        pass
+
     def _get_param(self):
         """Get current parameter value from gui."""
         self.param_value = self.get_value()
         self.paramChanged.emit(self.param_value)
         self.save_param()
 
     def _set_param(self):
@@ -225,39 +232,44 @@
         self._set_param()
         if value is not None:
             # Read from widget to get value e.g. inside min/max-bounds
             self._get_param()
 
     def _read_data(self, name):
         # get data from dictionary
-        if isinstance(self.data, dict):
-            if name in self.data:
-                value = self.data[name]
-            else:
-                value = self.default
+        if isinstance(self.data, dict) and name in self.data:
+            value = self.data[name]
 
         # get data from Parameters in Project in MainWindow
         # (depending on selected parameter-preset and selected Project)
-        elif isinstance(self.data, Controller):
-            if name in self.data.pr.parameters[self.data.pr.p_preset]:
-                value = self.data.pr.parameters[self.data.pr.p_preset][name]
-            else:
-                value = self.default
+        elif (
+            isinstance(self.data, Controller)
+            and name in self.data.pr.parameters[self.data.pr.p_preset]
+        ):
+            value = self.data.pr.parameters[self.data.pr.p_preset][name]
 
         # get data from QSettings
-        elif isinstance(self.data, QS):
-            if name in self.data.childKeys():
-                value = self.data.value(name)
-            else:
-                value = self.default
+        elif isinstance(self.data, QS) and name in self.data.childKeys():
+            value = self.data.value(name)
+        else:
+            value = self.default
 
         return value
 
     def read_param(self):
-        self.param_value = self._read_data(self.name)
+        data = self._read_data(self.name)
+        if not self.none_select:
+            if self.data_type != "multiple":
+                if not isinstance(data, self.data_type):
+                    logger().warning(
+                        f"Data for {self.name} has to be of type {self.data_type}, "
+                        f"but is of type {type(data)} instead!"
+                    )
+                    data = self.data_type()
+        self.param_value = data
 
     def _save_data(self, name, value):
         if isinstance(self.data, dict):
             self.data[name] = value
         elif isinstance(self.data, Controller):
             self.data.pr.parameters[self.data.pr.p_preset][name] = value
         elif isinstance(self.data, QS):
@@ -266,14 +278,16 @@
     def save_param(self):
         self._save_data(self.name, self.param_value)
 
 
 class IntGui(Param):
     """A GUI for Integer-Parameters"""
 
+    data_type = int
+
     def __init__(self, min_val=0, max_val=1000, special_value_text=None, **kwargs):
         """
         Parameters
         ----------
         min_val : int
             Set the minimumx value, defaults to 0.
         max_val : int
@@ -312,14 +326,16 @@
     def get_value(self):
         return self.param_widget.value()
 
 
 class FloatGui(Param):
     """A GUI for Float-Parameters"""
 
+    data_type = float
+
     def __init__(self, min_val=-1000.0, max_val=1000.0, step=0.1, decimals=2, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to -100..
         max_val : int | float
@@ -361,14 +377,16 @@
 
 
 class StringGui(Param):
     """
     A GUI for String-Parameters
     """
 
+    data_type = str
+
     def __init__(self, **kwargs):
         """
 
         Parameters
         ----------
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
@@ -403,14 +421,16 @@
     except (NameError, SyntaxError, ValueError, TypeError):
         return None
 
 
 class FuncGui(Param):
     """A GUI for Parameters defined by small functions, e.g from numpy"""
 
+    data_type = "multiple"
+
     def __init__(self, **kwargs):
         """
         Parameters
         ----------
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
@@ -490,14 +510,16 @@
         self.name = self.name[:-4]
         self.param_value = real_value
 
 
 class BoolGui(Param):
     """A GUI for Boolean-Parameters"""
 
+    data_type = bool
+
     def __init__(self, return_integer=False, **kwargs):
         """
         Parameters
         ----------
         return_integer : bool
             Set True to return an integer (0|1) instead of a boolean
             (e.g. useful for QSettings).
@@ -529,14 +551,16 @@
 
         return value
 
 
 class TupleGui(Param):
     """A GUI for Tuple-Parameters"""
 
+    data_type = tuple
+
     def __init__(self, min_val=-1000.0, max_val=1000.0, step=0.1, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to -100..
         max_val : int | float
@@ -545,25 +569,19 @@
             Set the amount, one step takes.
         **kwargs
             All the parameters fo :method:`~Param.__init__` go here.
         """
 
         super().__init__(**kwargs)
 
-        if step == 1:
-            self.param_widget1 = QSpinBox()
-            self.param_widget2 = QSpinBox()
-            min_val = int(min_val)
-            max_val = int(max_val)
-        else:
-            self.param_widget1 = QDoubleSpinBox()
-            self.param_widget2 = QDoubleSpinBox()
-            decimals = len(str(step)[str(step).find(".") :]) - 1
-            self.param_widget1.setDecimals(decimals)
-            self.param_widget2.setDecimals(decimals)
+        self.param_widget1 = QDoubleSpinBox()
+        self.param_widget2 = QDoubleSpinBox()
+        decimals = len(str(step)[str(step).find(".") :]) - 1
+        self.param_widget1.setDecimals(decimals)
+        self.param_widget2.setDecimals(decimals)
 
         self._external_set = False
 
         self.param_widget1.setToolTip(
             f"MinValue = {min_val}\nMaxVal = {max_val}\nStep = {step}\n"
         )
         self.param_widget2.setToolTip(
@@ -595,30 +613,34 @@
         tuple_layout.addWidget(self.param_widget2)
         self.init_ui(tuple_layout)
 
     def set_value(self, value):
         # Signal valueChanged is already emitted after first setValue,
         # which leads to second param_value being 0 without being
         # preserved in self.loaded_value
-        self._external_set = True
-        self.param_widget1.setValue(value[0])
-        self.param_widget2.setValue(value[1])
-        self._external_set = False
+        if len(value) == 2:
+            self._external_set = True
+            self.param_widget1.setValue(value[0])
+            self.param_widget2.setValue(value[1])
+            self._external_set = False
 
     def _get_param(self):
         if not self._external_set:
             super()._get_param()
 
     def get_value(self):
         return self.param_widget1.value(), self.param_widget2.value()
 
 
+# ToDo: make options replacable
 class ComboGui(Param):
     """A GUI for a Parameter with limited options"""
 
+    data_type = "multiple"
+
     def __init__(self, options, **kwargs):
         """
         Parameters
         ----------
         options : list | dict
             Supply a list or a dictionary with the options to choose from.
             If supplied a dictionary, dictionary-values are
@@ -692,14 +714,16 @@
         self.paramw.save_param()
         event.accept()
 
 
 class ListGui(Param):
     """A GUI for as list"""
 
+    data_type = list
+
     def __init__(self, value_string_length=30, **kwargs):
         """
         Parameters
         ----------
         value_string_length : int | None
             Set the limit of characters to which the value converted to a
             string will be displayed.
@@ -785,17 +809,20 @@
 
     def closeEvent(self, event):
         self.paramw._set_param()
         self.paramw.save_param()
         event.accept()
 
 
+# ToDo: make options replacable
 class CheckListGui(Param):
     """A GUI to select items from a list of options"""
 
+    data_type = list
+
     def __init__(self, options, value_string_length=30, one_check=False, **kwargs):
         """
         Parameters
         ----------
         options : list
             The items from which to choose
         value_string_length : int | None
@@ -886,14 +913,16 @@
         self.paramw.save_param()
         event.accept()
 
 
 class DictGui(Param):
     """A GUI for a dictionary"""
 
+    data_type = dict
+
     def __init__(self, value_string_length=30, **kwargs):
         """
 
         Parameters
         ----------
         value_string_length : int | None
             Set the limit of characters to which the value converted
@@ -961,14 +990,16 @@
 
         return value
 
 
 class SliderGui(Param):
     """A GUI to show a slider for Int/Float-Parameters"""
 
+    data_type = "multiple"
+
     def __init__(self, min_val=0, max_val=100, step=1, tracking=True, **kwargs):
         """
         Parameters
         ----------
         min_val : int | float
             Set the minimumx value, defaults to 0.
         max_val : int | float
@@ -1053,14 +1084,16 @@
 
         return value
 
 
 class MultiTypeGui(Param):
     """A GUI which accepts multiple types of values in a single LineEdit"""
 
+    data_type = "multiple"
+
     def __init__(self, type_selection=False, types=None, type_kwargs=None, **kwargs):
         """
         Parameters
         ----------
         type_selection : bool
             If True, the use can choose in a QComboBox which type they want
             to enter and then use the appropriate GUI.
@@ -1142,15 +1175,18 @@
         # Set Param-Value to None to avoid conflicts
         # whith values from other types
         self.param_value = None
         self.save_param()
 
         old_widget = self.type_layout.itemAt(1)
         self.type_layout.removeItem(old_widget)
-        old_widget.widget().deleteLater()
+        try:
+            old_widget.widget().deleteLater()
+        except RuntimeError:
+            logger().debug("Old widget already deleted")
         del old_widget, self.param_widget
 
         self.param_type = self.types[type_idx]
 
         self.add_type_gui()
 
     def _init_layout(self):
@@ -1191,50 +1227,74 @@
                 self.param_type = "error"
             self.type_display.setText(f"Type: {self.param_type}")
             self.save_param()
 
         return value
 
 
-class LabelPicker(Brain):
-    def __init__(self, paramdlg, *args, **kwargs):
-        try:
-            super().__init__(*args, **kwargs)
-        except TypeError:
-            # Backwards compatibility mne==0.24
-            kwargs.pop("block")
-            super().__init__(*args, **kwargs)
+class LabelPicker(mne.viz.Brain):
+    def __init__(
+        self, paramdlg, parcellation, surface, selected, list_changed_slot, title
+    ):
+        super().__init__(
+            paramdlg._fsmri.name,
+            surf=surface,
+            title=title,
+            subjects_dir=paramdlg.ct.subjects_dir,
+            background=(0, 0, 0),
+        )
+        self._renderer.plotter.show()
         self.paramdlg = paramdlg
         self.paramw = paramdlg.paramw
 
+        self.parcellation = parcellation
+        self.selected = selected
+        self.list_changed_slot = list_changed_slot
+
         self._shown_labels = list()
 
-        self._set_annotations()
+        # Title text
+        self.add_text(0, 0.9, "", color="w", font_size=14, name="title")
+
+        self._set_annotations(parcellation)
         self._init_picking()
-        self.add_text(0, 0.9, "Pick labels", "title", font_size=14)
 
-    def _set_annotations(self):
+        # Add selected labels
+        for label_name in selected:
+            hemi = label_name[-2:]
+            self._add_label_name(label_name, hemi)
+
+    def _set_annotations(self, parcellation):
         fsmri = self.paramdlg._fsmri
-        parcellation = self.paramdlg._parcellation
+        self.parcellation = parcellation
         self.clear_glyphs()
         self.remove_labels()
         self.remove_annotations()
-        self.add_annotation(parcellation, color="w", alpha=0.75)
+        labels = fsmri.get_labels(parcellation=parcellation)
+        if parcellation == "Other":
+            for label in labels:
+                self.add_label(label, borders=True, color="k", alpha=0.75)
+        else:
+            self.add_annotation(
+                parcellation, borders=True, color="k", alpha=0.75, remove_existing=True
+            )
 
-        for parc in [parcellation, "Other"]:
-            if parc in fsmri.labels:
-                labels = fsmri.labels[parc]
-                for hemi in self._hemis:
-                    hemi_labels = [lb for lb in labels if lb.hemi == hemi]
-                    self._vertex_to_label_id[hemi] = np.full(
-                        self.geo[hemi].coords.shape[0], -1
-                    )
-                    self._annotation_labels[hemi] = hemi_labels
-                    for idx, label in enumerate(hemi_labels):
-                        self._vertex_to_label_id[hemi][label.vertices] = idx
+        # Add label coordinates to dictionary to allow selection
+        for hemi in self._hemis:
+            hemi_labels = [lb for lb in labels if lb.hemi == hemi]
+            self._vertex_to_label_id[hemi] = np.full(self.geo[hemi].coords.shape[0], -1)
+            self._annotation_labels[hemi] = hemi_labels
+            for idx, hemi_label in enumerate(hemi_labels):
+                self._vertex_to_label_id[hemi][hemi_label.vertices] = idx
+
+        # Update text
+        self._actors["text"]["title"].SetInput(
+            f"Subject={self.paramdlg._fsmri.name}, Parcellation={parcellation}\n"
+            f"Select labels by clicking on them"
+        )
 
     def _init_picking(self):
         self._mouse_no_mvt = -1
         add_obs = self._renderer.plotter.iren.add_observer
         add_obs(vtkCommand.RenderEvent, self._on_mouse_move)
         add_obs(vtkCommand.LeftButtonPressEvent, self._on_button_press)
         add_obs(vtkCommand.EndInteractionEvent, self._on_button_release)
@@ -1259,199 +1319,284 @@
             vertices = mesh.points[cell]
             idx = np.argmin(abs(vertices - pos), axis=0)
             vertex_id = cell[idx[0]]
 
             label_id = self._vertex_to_label_id[hemi][vertex_id]
             label = self._annotation_labels[hemi][label_id]
 
-            if label.name in self.paramdlg._selected_labels:
+            if label.name in self.selected:
                 self._remove_label_name(label.name, hemi)
-                self.paramdlg._selected_labels.remove(label.name)
+                self.selected.remove(label.name)
             else:
                 self._add_label_name(label.name, hemi, label)
-                self.paramdlg._selected_labels.append(label.name)
-            self.paramdlg.label_list.content_changed()
+                self.selected.append(label.name)
+            self.list_changed_slot()
+            self.paramdlg.update_selected_display()
+
+            # Update label text
+            if "label" in self._actors["text"]:
+                self.remove_text("label")
+            if label.color is not None:
+                color = label.color[:3]
+                opacity = label.color[-1]
+            else:
+                color = "w"
+                opacity = 1
+            self.add_text(
+                0,
+                0.05,
+                label.name,
+                color=color,
+                opacity=opacity,
+                font_size=12,
+                name="label",
+            )
 
     def _add_label_name(self, label_name, hemi, label=None):
         if label is None:
             for lb in self._annotation_labels[hemi]:
                 if lb.name == label_name:
                     label = lb
                     break
         if label is not None:
-            self.add_label(label, borders=False, reset_camera=False)
+            self.add_label(label, borders=False)
             self._shown_labels.append(label_name)
 
     def _remove_label_name(self, label_name, hemi):
         self._layered_meshes[hemi].remove_overlay(label_name)
         self._shown_labels.remove(label_name)
         self._renderer._update()
 
-    def closeEvent(self, event):
-        self.paramdlg._label_picker = None
-        super().closeEvent(event)
+    def isclosed(self):
+        if self.plotter is None:
+            self._closed = True
+        return self._closed
+
+    def close(self):
+        if self.plotter is not None:
+            super().close()
+        self._closed = True
 
 
 class LabelDialog(SimpleDialog):
     def __init__(self, paramw):
         self.main_widget = QWidget()
         super().__init__(
             self.main_widget,
             parent=paramw,
             title="Choose a label!",
             window_title="Label Picker",
             modal=False,
         )
         self.paramw = paramw
         self.ct = paramw.data
-        self.params = self.ct.pr.parameters[self.ct.pr.p_preset]
         self.param_value = paramw.param_value
 
-        self._label_picker = None
+        self._parc_picker = None
+        self._extra_picker = None
         self._fsmri = None
         self._parcellation = None
-        self._all_label_names = list()
-        self._selected_labels = list()
+        self._surface = None
+        # Put selected labels from LabelGui in both parc and extra,
+        # since they get removed if not fitting later anyway
+        self._parc_labels = list()
+        self._selected_parc_labels = copy(paramw.param_value) or list()
+        self._extra_labels = list()
+        self._selected_extra_labels = copy(paramw.param_value) or list()
 
         self.resize(400, 800)
         center(self)
 
         self._init_layout()
+
+        # Initialize with first items
+        self._subject_changed()
+        self._surface_changed()
+
         self.open()
 
     def _init_layout(self):
         layout = QVBoxLayout(self.main_widget)
 
+        layout.addWidget(QLabel("Choose a subject:"))
         self.fsmri_cmbx = QComboBox()
         self.fsmri_cmbx.addItems(self.ct.pr.all_fsmri)
         self.fsmri_cmbx.activated.connect(self._subject_changed)
         layout.addWidget(self.fsmri_cmbx)
 
+        layout.addWidget(QLabel("Choose a parcellation:"))
         self.parcellation_cmbx = QComboBox()
         self.parcellation_cmbx.activated.connect(self._parc_changed)
         layout.addWidget(self.parcellation_cmbx)
 
-        self.label_list = CheckList(
-            data=self._all_label_names,
-            checked=self._selected_labels,
+        layout.addWidget(QLabel("Choose a surface:"))
+        self.surface_cmbx = QComboBox()
+        self.surface_cmbx.addItems(["inflated", "pial", "white"])
+        self.surface_cmbx.activated.connect(self._surface_changed)
+        layout.addWidget(self.surface_cmbx)
+
+        self.selected_display = SimpleList(
+            data=self._selected_parc_labels + self._selected_extra_labels,
+            title="Selected Labels",
+        )
+        layout.addWidget(self.selected_display)
+
+        self.parc_label_list = CheckList(
+            data=self._parc_labels,
+            checked=self._selected_parc_labels,
             ui_buttons=True,
             ui_button_pos="bottom",
+            title="Parcellation Labels",
+        )
+        self.parc_label_list.checkedChanged.connect(
+            partial(self._labels_changed, picker_name="parcellation")
         )
-        self.label_list.checkedChanged.connect(self._labels_changed)
-        layout.addWidget(self.label_list)
+        layout.addWidget(self.parc_label_list)
 
-        # ToDo: fix Brain-Picker (errors and somehow all labels are selected)
-        # slider_kwargs = {'max_val': 360, 'tracking': False}
-        # self.elevation_slider = SliderGui(data=self.paramw.data,
-        #                                   name='stc_elevation',
-        #                                   **slider_kwargs)
-        # self.elevation_slider.paramChanged.connect(self._slider_changed)
-        # layout.addWidget(self.elevation_slider)
-        #
-        # self.roll_slider = SliderGui(data=self.paramw.data,
-        #                              name='stc_roll',
-        #                              **slider_kwargs)
-        # self.roll_slider.paramChanged.connect(self._slider_changed)
-        # layout.addWidget(self.roll_slider)
-        #
-        # self.azimuth_slider = SliderGui(data=self.paramw.data,
-        #                                 name='stc_azimuth',
-        #                                 **slider_kwargs)
-        # self.azimuth_slider.paramChanged.connect(self._slider_changed)
-        # layout.addWidget(self.azimuth_slider)
-        #
-        # choose_bt = QPushButton('Choose Labels')
-        # choose_bt.clicked.connect(self._open_label_picker)
-        # layout.addWidget(choose_bt)
+        self.extra_label_list = CheckList(
+            data=self._extra_labels,
+            checked=self._selected_extra_labels,
+            ui_buttons=True,
+            ui_button_pos="bottom",
+            title="Extra Labels",
+        )
+        self.extra_label_list.checkedChanged.connect(
+            partial(self._labels_changed, picker_name="extra")
+        )
+        layout.addWidget(self.extra_label_list)
 
-        # Initialize with first items
-        self._subject_changed()
-        self._parc_changed()
+        self.choose_parc_bt = QPushButton("Choose Parcellation Labels")
+        self.choose_parc_bt.clicked.connect(self._open_parc_picker)
+        layout.addWidget(self.choose_parc_bt)
+
+        self.choose_extra_bt = QPushButton("Choose Extra Labels")
+        self.choose_extra_bt.clicked.connect(self._open_extra_picker)
+        layout.addWidget(self.choose_extra_bt)
 
     def _subject_changed(self):
         self._fsmri = FSMRI(self.fsmri_cmbx.currentText(), self.ct, load_labels=True)
 
         self.parcellation_cmbx.clear()
         self.parcellation_cmbx.addItems(self._fsmri.parcellations)
+
+        # Update extra labels
+        self._extra_labels.clear()
+        self._extra_labels += [lb.name for lb in self._fsmri.labels["Other"]]
+        self.extra_label_list.content_changed()
+
+        old_selected_extra = self._selected_extra_labels.copy()
+        self._selected_extra_labels.clear()
+        self._selected_extra_labels += [
+            lb for lb in old_selected_extra if lb in self._extra_labels
+        ]
+        self.extra_label_list.content_changed()
+
+        # Update selected parcellation labels
+        all_labels_exept_other = list()
+        for parc_name, labels in self._fsmri.labels.items():
+            if parc_name != "Other":
+                all_labels_exept_other += [lb.name for lb in labels]
+        old_selected_parc = self._selected_parc_labels.copy()
+        self._selected_parc_labels.clear()
+        self._selected_parc_labels += [
+            lb for lb in old_selected_parc if lb in all_labels_exept_other
+        ]
+
+        # Update pickers if open
+        if self._parc_picker is not None and not self._parc_picker.isclosed():
+            self._parc_picker.close()
+            self._open_parc_picker()
+        if self._extra_picker is not None and not self._extra_picker.isclosed():
+            self._extra_picker.close()
+            self._open_extra_picker()
+
+        # Update parcellation labels
         self._parc_changed()
 
     def _parc_changed(self):
         # Keep reference for inplace change
-        self._all_label_names.clear()
-        self._selected_labels.clear()
-
-        # Add single labels
-        self._all_label_names += [lb.name for lb in self._fsmri.labels["Other"]]
+        self._parc_labels.clear()
 
         # Add parcellation labels
         self._parcellation = self.parcellation_cmbx.currentText()
         if self._parcellation in self._fsmri.labels:
-            self._all_label_names += [
+            self._parc_labels += [
                 lb.name for lb in self._fsmri.labels[self._parcellation]
             ]
 
-        # get selected
-        self._selected_labels += [
-            lb for lb in self.paramw.param_value if lb in self._all_label_names
-        ]
-        self.label_list.content_changed()
+        self.parc_label_list.content_changed()
 
-        if self._label_picker is not None:
-            self._label_picker._set_annotations()
+        if self._parc_picker is not None and not self._parc_picker.isclosed():
+            self._parc_picker._set_annotations(self._parcellation)
+            for label_name in [
+                lb for lb in self._selected_parc_labels if lb in self._parc_labels
+            ]:
+                hemi = label_name[-2:]
+                self._parc_picker._add_label_name(label_name, hemi)
+
+    def _surface_changed(self):
+        self._surface = self.surface_cmbx.currentText()
+        if self._parc_picker is not None and not self._parc_picker.isclosed():
+            self._parc_picker.close()
+            self._open_parc_picker()
+
+    def update_selected_display(self):
+        self.selected_display.replace_data(
+            self._selected_parc_labels + self._selected_extra_labels
+        )
 
-    def _labels_changed(self, labels):
-        if self._label_picker is not None:
-            shown_labels = self._label_picker._shown_labels
+    def _labels_changed(self, labels, picker_name):
+        picker = (
+            self._parc_picker if picker_name == "parcellation" else self._extra_picker
+        )
+        if picker is not None:
+            shown_labels = picker._shown_labels
             for add_name in [lb for lb in labels if lb not in shown_labels]:
                 hemi = add_name[-2:]
-                self._label_picker._add_label_name(add_name, hemi)
+                picker._add_label_name(add_name, hemi)
             for remove_name in [lb for lb in shown_labels if lb not in labels]:
                 hemi = remove_name[-2:]
-                self._label_picker._remove_label_name(remove_name, hemi)
-
-    def _slider_changed(self, _):
-        if self._label_picker is not None:
-            roll = self.roll_slider.param_value
-            elevation = self.elevation_slider.param_value
-            azimuth = self.azimuth_slider.param_value
-            for row, col in [(0, 0), (0, 1), (1, 0), (1, 1)]:
-                self._label_picker.show_view(
-                    roll=roll, elevation=elevation, azimuth=azimuth, row=row, col=col
-                )
-
-    def _open_label_picker(self):
-        background = self.params["stc_background"]
+                picker._remove_label_name(remove_name, hemi)
+        # Update display
+        self.update_selected_display()
+
+    # Keep pickers on top
+    def _open_parc_picker(self):
+        self._parc_picker = LabelPicker(
+            self,
+            self._parcellation,
+            self._surface,
+            self._selected_parc_labels,
+            self.parc_label_list.content_changed,
+            title="Pick parcellation labels",
+        )
 
-        self._label_picker = LabelPicker(
+    def _open_extra_picker(self):
+        self._extra_picker = LabelPicker(
             self,
-            self._fsmri.name,
-            hemi="split",
-            views=["lat", "med"],
-            surf="inflated",
-            title="Pick labels",
-            subjects_dir=self.ct.subjects_dir,
-            block=False,
-            background=background,
+            "Other",
+            self._surface,
+            self._selected_extra_labels,
+            self.extra_label_list.content_changed,
+            title="Pick extra labels",
         )
-        self._slider_changed(None)
 
     def closeEvent(self, event):
-        event.accept()
-        self.paramw.param_value = self._selected_labels
-        self.paramw._get_param()
-        self.paramw._set_param()
-        if self._label_picker is not None:
-            if self._label_picker.plotter is not None:
-                self._label_picker.plotter.close()
-        # ToDo: Update slider across all instances
+        self.paramw.set_param(self._selected_parc_labels + self._selected_extra_labels)
+        for picker in [self._parc_picker, self._extra_picker]:
+            if picker is not None and not picker.isclosed():
+                picker.close()
+        self.hide()
 
 
 class LabelGui(Param):
     """This GUI lets the user pick labels from a brain."""
 
+    data_type = list
+
     def __init__(self, value_string_length=30, **kwargs):
         """
         Parameters
         ----------
         value_string_length : int | None
             Set the limit of characters to which the value converted to a
             string will be displayed.
@@ -1462,32 +1607,41 @@
         super().__init__(**kwargs)
         self.value_string_length = value_string_length
         if not isinstance(self.data, Controller):
             raise RuntimeError(
                 "LabelGui can only used with an instance of "
                 "Controller passed as data."
             )
+
+        self._dialog = None
+
         self.read_param()
         self._init_layout()
         self._set_param()
         self.save_param()
 
     def _init_layout(self):
         check_list_layout = QHBoxLayout()
 
         self.value_label = QLabel()
         check_list_layout.addWidget(self.value_label)
 
         self.param_widget = QPushButton("Edit")
         self.param_widget.setSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
-        self.param_widget.clicked.connect(partial(LabelDialog, self))
+        self.param_widget.clicked.connect(self.show_dialog)
         check_list_layout.addWidget(self.param_widget)
 
         self.init_ui(check_list_layout)
 
+    def show_dialog(self):
+        if self._dialog is None:
+            self._dialog = LabelDialog(self)
+        else:
+            self._dialog.show()
+
     def set_value(self, value):
         if value is not None:
             self.cached_value = value
         self.check_groupbox_state()
         if isinstance(value, list):
             if self.param_unit:
                 val_str = ", ".join([f"{item}" for item in value])
@@ -1512,14 +1666,16 @@
 
         return value
 
 
 class ColorGui(Param):
     """A GUI to pick a color and returns a dictionary with HexRGBA-Strings."""
 
+    data_type = dict
+
     def __init__(self, keys, **kwargs):
         """
         Parameters
         ----------
         keys : dict | str | None
             If you supply a dictionary with keys, you can set a color
             for each key. If you supply the string name of another parameter
@@ -1591,14 +1747,64 @@
             )
         self._cached_value[key] = color.name()
         self._change_display_color()
         self._set_param()
         self._get_param()
 
 
+# ToDo: Own testable QFileDialog-Implementations
+class PathGui(Param):
+    """A GUI to pick a path."""
+
+    data_type = str
+
+    def __init__(self, pick_mode="file", **kwargs):
+        """
+        Parameters
+        ----------
+        pick_mode : str
+            Can be either "file" or "directory".
+        **kwargs
+            All the parameters for :method:`Param.__init__` go here.
+        """
+
+        super().__init__(**kwargs)
+
+        self.pick_mode = pick_mode
+
+        self.read_param()
+        self._init_layout()
+        self._set_param()
+        self.save_param()
+
+    def _init_layout(self):
+        layout = QHBoxLayout()
+        self.display_widget = QLabel()
+        layout.addWidget(self.display_widget)
+        self.param_widget = QPushButton("Pick Path")
+        self.param_widget.clicked.connect(self._pick_path)
+        layout.addWidget(self.param_widget)
+
+        self.init_ui(layout)
+
+    def _pick_path(self):
+        if self.pick_mode == "file":
+            path = compat.getopenfilename(self, self.description)[0]
+        else:
+            path = compat.getexistingdirectory(self, self.description)
+        self.set_value(path)
+        self._get_param()
+
+    def set_value(self, value):
+        self.display_widget.setText(value)
+
+    def get_value(self):
+        return self.display_widget.text()
+
+
 # Todo: Ordering Parameters in Tabs and add Find-Command
 class ResetDialog(QDialog):
     def __init__(self, p_dock):
         super().__init__(p_dock)
         self.pd = p_dock
         self.selected_params = list()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/plot_widgets.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/plot_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
-import logging
 from functools import partial
 from importlib import import_module
 from os.path import join, isfile
 
-from PyQt5.QtCore import Qt, QThreadPool
-from PyQt5.QtGui import QPixmap, QFont
-from PyQt5.QtWidgets import (
+from matplotlib import pyplot as plt
+from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg
+from matplotlib.figure import Figure
+from mne.viz import Brain
+from mne_qt_browser._pg_figure import MNEQtBrowser
+from qtpy.QtCore import Qt, QThreadPool
+from qtpy.QtGui import QPixmap, QFont
+from qtpy.QtWidgets import (
     QMainWindow,
     QWidget,
     QGridLayout,
     QComboBox,
     QTabWidget,
     QVBoxLayout,
     QDialog,
@@ -25,19 +29,16 @@
     QMessageBox,
     QProgressDialog,
     QLabel,
     QScrollArea,
     QToolBar,
     QSpinBox,
 )
-from matplotlib import pyplot as plt
-from matplotlib.backends.backend_qtagg import FigureCanvasQTAgg
-from matplotlib.figure import Figure
-from mne.viz import Brain
-from mne_qt_browser._pg_figure import MNEQtBrowser
+
+from mne_pipeline_hd.pipeline.pipeline_utils import logger
 
 try:
     from mne.viz import Figure3D
 except ImportError:
     Figure3D = None
 from mne_pipeline_hd import _object_refs
 from mne_pipeline_hd.gui.base_widgets import SimpleList, CheckList
@@ -106,15 +107,15 @@
             elif isinstance(subplot, MNEQtBrowser):
                 plot_widget = subplot
             elif isinstance(subplot, Brain):
                 plot_widget = subplot
             elif isinstance(subplot, Figure3D):
                 plot_widget = subplot
             else:
-                logging.error(
+                logger().error(
                     f'Unrecognized type "{type(subplot)}" ' f'for "{func_name}"'
                 )
                 plot_widget = QWidget()
 
             self.plots[name][func_name].append(plot_widget)
 
             if (
@@ -283,15 +284,15 @@
                     else:
                         break
 
                     # Replace Parameter-Preset for the loaded object
                     # and reload load/save-paths
                     if p_preset != obj.p_preset:
                         obj.p_preset = p_preset
-                        obj.init_parameters()
+                        obj.init_plot_files()
                         obj.init_paths()
 
                     # Load Matplotlib-Plots
                     if self.interactive_chkbx.isChecked():
                         # Get module of plot_function
                         module_name = self.ct.pd_funcs.loc[self.selected_func, "module"]
                         module = import_module(module_name)
@@ -314,15 +315,15 @@
 
                         worker.signals.finished.connect(finished_func)
 
                         def error_func(err_tuple, o_name=obj_name, ppreset=p_preset):
                             self.thread_error(err_tuple, o_name, ppreset, "plot")
 
                         worker.signals.error.connect(error_func)
-                        print(
+                        logger().info(
                             f"Starting Thread for Object= {obj_name} "
                             f"and Parameter-Preset= {p_preset}"
                         )
                         QThreadPool.globalInstance().start(worker)
 
                     # Load Plot-Images
                     else:
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/tools.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/tools.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from functools import partial
 
-from PyQt5.QtGui import QFont
-from PyQt5.QtWidgets import (
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QFont
+from qtpy.QtWidgets import (
     QComboBox,
     QDialog,
     QGridLayout,
     QHBoxLayout,
     QPushButton,
     QSizePolicy,
     QVBoxLayout,
@@ -208,26 +209,26 @@
         else:
             # Reset globals to default
             for key in [
                 k for k in self.t_globals.keys() if k not in self.default_t_globals
             ]:
                 self.t_globals.pop(key)
             self.t_globals["obj"] = self.obj
-            self.displayw.insertHtml(f"<b>Subject: {self.obj.name} loaded</b><br>")
+            self.displayw.appendHtml(f"<b>Subject: {self.obj.name} loaded</b><br>")
             self.displayw.ensureCursorVisible()
 
     def load_bt_pressed(self, bt_name):
         worker_dialog = WorkerDialog(
             self, self.start_load, title=f"Loading {bt_name}...", bt_name=bt_name
         )
         worker_dialog.thread_finished.connect(self.finished_handling)
 
     def finished_handling(self, result_msg):
         if isinstance(result_msg, str):
-            self.displayw.insertHtml(result_msg)
+            self.displayw.appendHtml(result_msg)
             self.displayw.ensureCursorVisible()
 
     def start_load(self, bt_name):
         try:
             load_fn = getattr(self.obj, self.load_mapping[bt_name])
             self.t_globals[bt_name] = load_fn()
         except OSError:
@@ -239,15 +240,15 @@
             )
 
         return result_msg
 
     def start_execution(self):
         command = self.inputw.toPlainText()
         command_html = command.replace("\n", "<br>")
-        self.displayw.insertHtml(
+        self.displayw.appendHtml(
             f'<font color="blue"><b><i>{command_html}</i></b></font><br>'
         )
         self.displayw.ensureCursorVisible()
         self.history.insert(0, command)
 
         try:
             print(eval(command, self.t_globals))
@@ -258,7 +259,12 @@
                 get_exception_tuple()
             else:
                 self.inputw.clear()
         except Exception:
             get_exception_tuple()
         else:
             self.inputw.clear()
+
+    def keyPressEvent(self, event):
+        if event.key() == Qt.Key_Up:
+            self.inputw.insertPlainText(self.history[0])
+            self.inputw.ensureCursorVisible()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/gui/welcome_window.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/gui/welcome_window.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,30 @@
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 from importlib import resources
 from os import listdir
 from os.path import isdir, join
 
-from PyQt5.QtCore import Qt
-from PyQt5.QtGui import QFont, QPixmap
-from PyQt5.QtWidgets import (
+from qtpy import compat
+from qtpy.QtCore import Qt
+from qtpy.QtGui import QFont, QPixmap
+from qtpy.QtWidgets import (
     QComboBox,
-    QFileDialog,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
     QVBoxLayout,
     QWidget,
 )
 
-from mne_pipeline_hd import _object_refs
+from mne_pipeline_hd import _object_refs, extra
 from mne_pipeline_hd.gui.base_widgets import SimpleList
-from mne_pipeline_hd.gui.gui_utils import center, WorkerDialog, \
-    get_user_input_string
+from mne_pipeline_hd.gui.gui_utils import center, WorkerDialog, get_user_input_string
 from mne_pipeline_hd.gui.main_window import MainWindow
 from mne_pipeline_hd.pipeline.controller import Controller
 from mne_pipeline_hd.pipeline.pipeline_utils import QS
 
 
 class WelcomeWindow(QWidget):
     def __init__(self, controller=None):
@@ -52,18 +51,16 @@
     def init_ui(self):
         layout = QVBoxLayout()
         title_label = QLabel("Welcome to MNE-Pipeline!")
         title_label.setFont(QFont(QS().value("app_font"), 20))
         layout.addWidget(title_label)
 
         image_label = QLabel()
-        with resources.path(
-            "mne_pipeline_hd.resource", "mne_pipeline_logo_evee_smaller.jpg"
-        ) as img_path:
-            image_label.setPixmap(QPixmap(str(img_path)))
+        img_path = resources.files(extra) / "mne_pipeline_logo_evee_smaller.jpg"
+        image_label.setPixmap(QPixmap(str(img_path)))
         layout.addWidget(image_label)
 
         home_layout = QHBoxLayout()
         self.home_path_label = QLabel()
         home_layout.addWidget(self.home_path_label, stretch=4)
         self.home_path_bt = QPushButton("Set Home-Folder")
         self.home_path_bt.clicked.connect(self.set_home_path)
@@ -130,15 +127,15 @@
             self.add_pr_bt.setEnabled(False)
             self.start_bt.setEnabled(False)
             self.home_path_label.setText("No Home-Path selected")
 
     def set_home_path(self):
         if self.ct is not None:
             self.ct.save()
-        loaded_home_path = QFileDialog.getExistingDirectory(
+        loaded_home_path = compat.getexistingdirectory(
             self, "Select a folder as Home-Path"
         )
         if loaded_home_path != "":
             try:
                 self.ct = Controller(str(loaded_home_path))
             except RuntimeError as err:
                 self.home_path_label.setText(str(err))
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/controller.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,18 @@
 from os import listdir
 from os.path import isdir, join
 from pathlib import Path
 
 import mne
 import pandas as pd
 
-from mne_pipeline_hd import functions
+from mne_pipeline_hd import functions, extra
 from mne_pipeline_hd.gui.gui_utils import get_user_input_string
-from mne_pipeline_hd.pipeline.legacy import \
-    transfer_file_params_to_single_subject
-from mne_pipeline_hd.pipeline.pipeline_utils import QS
+from mne_pipeline_hd.pipeline.legacy import transfer_file_params_to_single_subject
+from mne_pipeline_hd.pipeline.pipeline_utils import QS, logger
 from mne_pipeline_hd.pipeline.project import Project
 
 home_dirs = ["custom_packages", "freesurfer", "projects"]
 project_dirs = ["_pipeline_scripts", "data", "figures"]
 
 
 class Controller:
@@ -47,18 +46,22 @@
 
         # Check, if path is writable
         elif not os.access(self.home_path, os.W_OK):
             raise RuntimeError(f"{self.home_path} not writable!")
 
         # Initialize log-file
         self.logging_path = join(self.home_path, "_pipeline.log")
+        file_handlers = [h for h in logger().handlers if h.name == "file"]
+        if len(file_handlers) > 0:
+            logger().removeHandler(file_handlers[0])
         file_handler = logging.FileHandler(self.logging_path, "w")
-        logging.getLogger().addHandler(file_handler)
+        file_handler.set_name("file")
+        logger().addHandler(file_handler)
 
-        logging.info(f"Home-Path: {self.home_path}")
+        logger().info(f"Home-Path: {self.home_path}")
         QS().setValue("home_path", self.home_path)
         # Create subdirectories if not existing for a valid home_path
         for subdir in [d for d in home_dirs if not isdir(join(self.home_path, d))]:
             os.mkdir(join(self.home_path, subdir))
 
         # Get Project-Folders (recognized by distinct sub-folders)
         self.projects_path = join(self.home_path, "projects")
@@ -76,51 +79,44 @@
         self.custom_pkg_path = join(self.home_path, "custom_packages")
 
         # Initialize educational programs
         self.edu_program_name = edu_program_name
         self.edu_program = None
 
         # Load default settings
-        with resources.open_text(
-            "mne_pipeline_hd.resource", "default_settings.json"
-        ) as file:
+        default_path = join(resources.files(extra), "default_settings.json")
+        with open(default_path, "r") as file:
             self.default_settings = json.load(file)
 
         # Load settings (which are stored as .json-file in home_path)
         # settings=<everything, that's OS-independent>
         self.load_settings()
 
         self.all_modules = dict()
         self.all_pd_funcs = None
 
         # Pandas-DataFrame for contextual data of basic functions
         # (included with program)
-        with resources.path(
-            "mne_pipeline_hd.resource", "functions.csv"
-        ) as pd_funcs_path:
-            self.pd_funcs = pd.read_csv(
-                str(pd_funcs_path),
-                sep=";",
-                index_col=0,
-                na_values=[""],
-                keep_default_na=False,
-            )
+        self.pd_funcs = pd.read_csv(
+            resources.files(extra) / "functions.csv",
+            sep=";",
+            index_col=0,
+            na_values=[""],
+            keep_default_na=False,
+        )
 
         # Pandas-DataFrame for contextual data of parameters
         # for basic functions (included with program)
-        with resources.path(
-            "mne_pipeline_hd.resource", "parameters.csv"
-        ) as pd_params_path:
-            self.pd_params = pd.read_csv(
-                str(pd_params_path),
-                sep=";",
-                index_col=0,
-                na_values=[""],
-                keep_default_na=False,
-            )
+        self.pd_params = pd.read_csv(
+            resources.files(extra) / "parameters.csv",
+            sep=";",
+            index_col=0,
+            na_values=[""],
+            keep_default_na=False,
+        )
 
         # Import the basic- and custom-function-modules
         self.import_custom_modules()
 
         # Check Project
         if selected_project is None:
             selected_project = self.settings["selected_project"]
@@ -173,15 +169,15 @@
     def save_settings(self):
         try:
             with open(
                 join(self.home_path, "mne_pipeline_hd-settings.json"), "w"
             ) as file:
                 json.dump(self.settings, file, indent=4)
         except FileNotFoundError:
-            print("Settings could not be saved!")
+            logger().warning("Settings could not be saved!")
 
         # Sync QSettings with other instances
         QS().sync()
 
     def get_setting(self, setting):
         try:
             value = self.settings[setting]
@@ -191,15 +187,15 @@
         return value
 
     def change_project(self, new_project):
         self.pr = Project(self, new_project)
         self.settings["selected_project"] = new_project
         if new_project not in self.projects:
             self.projects.append(new_project)
-        logging.info(f"Selected-Project: {self.pr.name}")
+        logger().info(f"Selected-Project: {self.pr.name}")
         # Legacy
         transfer_file_params_to_single_subject(self)
 
         return self.pr
 
     def remove_project(self, project):
         self.projects.remove(project)
@@ -213,28 +209,66 @@
             self.change_project(new_project)
 
         # Remove Project-Folder
         try:
             shutil.rmtree(join(self.projects_path, project))
         except OSError as error:
             print(error)
-            logging.warning(
+            logger().warning(
                 f"The folder of {project} can't be deleted "
                 f"and has to be deleted manually!"
             )
 
+    def rename_project(self):
+        check_writable = os.access(self.pr.project_path, os.W_OK)
+        if check_writable:
+            new_project_name = get_user_input_string(
+                f'Change the name of project "{self.pr.name}" to:',
+                "Rename Project",
+                force=False,
+            )
+            if new_project_name is not None:
+                try:
+                    old_name = self.pr.name
+                    self.pr.rename(new_project_name)
+                except PermissionError:
+                    # ToDo: Warning-Function for GUI with dialog and non-GUI
+                    logger().critical(
+                        f"Can't rename {old_name} to {new_project_name}. "
+                        f"Probably a file from inside the project is still opened. "
+                        f"Please close all files and try again."
+                    )
+                else:
+                    self.projects.remove(old_name)
+                    self.projects.append(new_project_name)
+        else:
+            logger().warning(
+                "The project-folder seems to be not writable at the moment, "
+                "maybe some files inside are still in use?"
+            )
+
     def copy_parameters_between_projects(
-        self, from_name, from_p_preset, to_name, to_p_preset
+        self,
+        from_name,
+        from_p_preset,
+        to_name,
+        to_p_preset,
+        parameter=None,
     ):
         from_project = Project(self, from_name)
         if to_name == self.pr.name:
             to_project = self.pr
         else:
             to_project = Project(self, to_name)
-        to_project.parameters[to_p_preset] = from_project.parameters[from_p_preset]
+        if parameter is not None:
+            from_param = from_project.parameters[from_p_preset][parameter]
+            to_project.parameters[to_p_preset][parameter] = from_param
+        else:
+            from_param = from_project.parameters[from_p_preset]
+            to_project.parameters[to_p_preset] = from_param
         to_project.save()
 
     def save(self, worker_signals=None):
         if self.pr is not None:
             # Save Project
             self.pr.save(worker_signals)
             self.settings["selected_project"] = self.pr.name
@@ -366,15 +400,15 @@
                         ]
                         self.pd_params = pd.concat(
                             [self.pd_params, pd_params_to_append]
                         )
 
             else:
                 missing_files = [key for key in file_dict if file_dict[key] is None]
-                logging.warning(
+                logger().warning(
                     f"Files for import of {pkg_name} " f"are missing: {missing_files}"
                 )
 
     def reload_modules(self):
         for pkg_name in self.all_modules:
             for module_name in self.all_modules[pkg_name]:
                 module = import_module(module_name)
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/function_utils.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/function_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,82 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
+from __future__ import print_function
 
+import gc
 import inspect
 import io
-import logging
 import sys
 from collections import OrderedDict
 from importlib import import_module
 from multiprocessing import Pipe
 
-from PyQt5.QtCore import QThreadPool, QRunnable, pyqtSlot, QObject, pyqtSignal
-from PyQt5.QtWidgets import QAbstractItemView
+from matplotlib import pyplot as plt
+from qtpy.QtCore import QThreadPool, QRunnable, Slot, QObject, Signal
+from qtpy.QtWidgets import QAbstractItemView
 
-from mne_pipeline_hd.gui.gui_utils import get_exception_tuple, ExceptionTuple, \
-    Worker
+from mne_pipeline_hd.gui.base_widgets import TimedMessageBox
+from mne_pipeline_hd.gui.gui_utils import get_exception_tuple, ExceptionTuple, Worker
 from mne_pipeline_hd.pipeline.loading import BaseLoading, FSMRI, Group, MEEG
-from mne_pipeline_hd.pipeline.pipeline_utils import shutdown, ismac, QS
+from mne_pipeline_hd.pipeline.pipeline_utils import shutdown, ismac, QS, logger
 
 
 def get_func(func_name, obj):
     # Get module- and package-name, has to specified in pd_funcs
     # (which imports from functions.csv or the <custom_package>.csv)
     module_name = obj.ct.pd_funcs.loc[func_name, "module"]
     module = import_module(module_name)
     func = getattr(module, func_name)
 
     return func
 
 
 def get_arguments(func, obj):
-    keyword_arguments = {}
-    project_attributes = vars(obj.pr)
-
     # Get arguments from function signature
-    arg_names = list(inspect.signature(func).parameters)
+    arguments = {
+        arg_name: arg.default
+        for arg_name, arg in inspect.signature(func).parameters.items()
+    }
 
     # Remove args/kwargs
-    if "args" in arg_names:
-        arg_names.remove("args")
-    if "kwargs" in arg_names:
-        arg_names.remove("kwargs")
+    for pop_item in ["args", "kwargs"]:
+        arguments.pop(pop_item, None)
+
+    # Set data-objects
+    for obj_name, obj in [
+        ("ct", obj.ct),
+        ("controller", obj.ct),
+        ("pr", obj.pr),
+        ("project", obj.pr),
+        ("meeg", obj),
+        ("fsmri", obj),
+        ("group", obj),
+    ]:
+        if obj_name in arguments:
+            arguments[obj_name] = obj
 
     # Get the values for parameter-names
-    for arg_name in arg_names:
-        if arg_name == "ct":
-            keyword_arguments.update({"ct": obj.ct})
-        elif arg_name == "controller":
-            keyword_arguments.update({"controller": obj.ct})
-        elif arg_name == "pr":
-            keyword_arguments.update({"pr": obj.pr})
-        elif arg_name == "project":
-            keyword_arguments.update({"project": obj.pr})
-        elif arg_name == "meeg":
-            keyword_arguments.update({"meeg": obj})
-        elif arg_name == "fsmri":
-            keyword_arguments.update({"fsmri": obj})
-        elif arg_name == "group":
-            keyword_arguments.update({"group": obj})
-        elif arg_name in project_attributes:
-            keyword_arguments.update({arg_name: project_attributes[arg_name]})
-        elif arg_name in obj.pr.parameters[obj.pr.p_preset]:
-            keyword_arguments.update(
-                {arg_name: obj.pr.parameters[obj.pr.p_preset][arg_name]}
-            )
+    for arg_name in arguments:
+        if arg_name in obj.pa:
+            arguments[arg_name] = obj.pa[arg_name]
         elif arg_name in obj.ct.settings:
-            keyword_arguments.update({arg_name: obj.ct.settings[arg_name]})
+            arguments[arg_name] = obj.ct.settings[arg_name]
         elif arg_name in QS().childKeys():
-            keyword_arguments.update({arg_name: QS().value(arg_name)})
-        else:
-            raise RuntimeError(
-                f"{arg_name} could not be found " f"in Subject, Project or Parameters"
-            )
+            arguments[arg_name] = QS().value(arg_name)
 
     # Add additional keyword-arguments if added for function by user
     if func.__name__ in obj.pr.add_kwargs:
         for kwarg in obj.pr.add_kwargs[func.__name__]:
-            keyword_arguments[kwarg] = obj.pr.add_kwargs[func.__name__][kwarg]
+            arguments[kwarg] = obj.pr.add_kwargs[func.__name__][kwarg]
 
-    return keyword_arguments
+    return arguments
 
 
 class StreamManager:
     def __init__(self, pipe):
         self.pipe_busy = False
         self.stdout_sender = StreamSender(self, "stdout", pipe)
         self.stderr_sender = StreamSender(self, "stderr", pipe)
@@ -105,48 +96,42 @@
     def write(self, text):
         # Still send output to the command-line
         self.original_stream.write(text)
         # Wait until pipe is free
         while self.manager.pipe_busy:
             pass
         self.manager.pipe_busy = True
-        if text[:1] == "\r":
-            kind = "progress"
-        else:
-            kind = self.kind
+        kind = self.kind
         self.pipe.send((text, kind))
         self.manager.pipe_busy = False
 
 
 class StreamRcvSignals(QObject):
-    stdout_received = pyqtSignal(str)
-    stderr_received = pyqtSignal(str)
-    progress_received = pyqtSignal(str)
+    stdout_received = Signal(str)
+    stderr_received = Signal(str)
 
 
 class StreamReceiver(QRunnable):
     def __init__(self, pipe):
         super().__init__()
         self.pipe = pipe
         self.signals = StreamRcvSignals()
 
-    @pyqtSlot()
+    @Slot()
     def run(self):
         while True:
             try:
                 text, kind = self.pipe.recv()
             except EOFError:
                 break
             else:
-                if kind == "stdout":
-                    self.signals.stdout_received.emit(text)
-                elif kind == "stderr":
+                if kind == "stderr":
                     self.signals.stderr_received.emit(text)
                 else:
-                    self.signals.progress_received.emit(text)
+                    self.signals.stdout_received.emit(text)
 
 
 def run_func(func, keywargs, pipe=None):
     if pipe is not None:
         stream_manager = StreamManager(pipe)
         sys.stdout = stream_manager.stdout_sender
         sys.stderr = stream_manager.stderr_sender
@@ -164,15 +149,17 @@
         self.thread_idx_count = 0
         self.all_objects = OrderedDict()
         self.current_all_funcs = dict()
         self.current_obj_name = None
         self.current_object = None
         self.loaded_fsmri = None
         self.current_func = None
+
         self.prog_count = 0
+        self.errors = list()
 
         self.init_lists()
 
     def init_lists(self):
         # Lists dividing the
         self.meeg_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "MEEG"]
         self.fsmri_funcs = self.ct.pd_funcs[self.ct.pd_funcs["target"] == "FSMRI"]
@@ -275,25 +262,29 @@
 
             elif self.current_type == "Other":
                 self.current_object = BaseLoading(self.current_obj_name, self.ct)
 
     def process_finished(self, result):
         # ToDo: tqdm-progressbar for headless-mode
         self.prog_count += 1
-        self.start()
+        if len(self.all_steps) > 0:
+            self.start()
+        else:
+            self.finished()
 
     def finished(self):
-        pass
+        for name, func, error in self.errors:
+            logger().critical(f"Error in {name} <- {func}: {error}")
 
     def prepare_start(self):
         # Take first step of all_steps until there are no steps left.
         if len(self.all_steps) > 0:
             # Getting information as encoded in init_lists
             self.current_obj_name, self.current_func = self.all_steps.pop(0)
-            logging.debug(
+            logger().debug(
                 f"Running {self.current_func} for " f"{self.current_obj_name}"
             )
             # Get current object
             self.get_object()
 
             # Mark current object and current function
             self.mark_current_items(2)
@@ -305,21 +296,37 @@
 
             return kwds
 
         else:
             self.finished()
 
     def start(self):
-        kwds = self.prepare_start()
-        if kwds is not None:
-            run_func(**kwds)
+        """No-Gui start method."""
+        for name, func in self.all_steps:
+            self.current_obj_name = name
+            self.current_func = func
+            self.get_object()
+            kwds = dict()
+            kwds["func"] = get_func(self.current_func, self.current_object)
+            kwds["keywargs"] = get_arguments(kwds["func"], self.current_object)
+            logger().info(
+                f"########################################\n"
+                f"Running {self.current_func} for {self.current_obj_name}\n"
+                f"########################################\n"
+            )
+            result = run_func(**kwds)
+
+            if isinstance(result, ExceptionTuple):
+                self.errors.append(
+                    (self.current_object.name, self.current_func, result)
+                )
             # ToDo: MP
             # self.pool.apply_async(func=run_func, kwds=kwds,
             #                       callback=self.process_finished)
-            self.process_finished(None)
+        self.finished()
 
 
 class QRunController(RunController):
     def __init__(self, run_dialog, controller):
         super().__init__(controller)
         self.rd = run_dialog
         self.errors = dict()
@@ -387,16 +394,15 @@
                 self.errors[error_cause] = (result, self.error_count)
                 # Update Error-Widget
                 self.rd.error_widget.replace_data(list(self.errors.keys()))
 
                 # Insert Error-Number into console-widget as an anchor
                 # for later inspection
                 self.rd.console_widget.write_html(
-                    f'<a name="{self.error_count}" href={self.error_count}>'
-                    f"<i>Error No.{self.error_count}</i><br></a>"
+                    f"<b>Error-No. {self.error_count} (above)</b><br>"
                 )
                 # Increase Error-Count by one
                 self.error_count += 1
 
             # Continue with next object
             self.start()
 
@@ -404,17 +410,28 @@
         self.rd.console_widget.write_html("<b><big>Finished</big></b><br>")
         # Enable/Disable Buttons
         self.rd.continue_bt.setEnabled(False)
         self.rd.pause_bt.setEnabled(False)
         self.rd.restart_bt.setEnabled(True)
         self.rd.close_bt.setEnabled(True)
 
+        if not self.ct.get_setting("show_plots"):
+            close_all()
+
         if self.ct.get_setting("shutdown"):
             self.ct.save()
-            shutdown()
+            ans = TimedMessageBox.information(
+                timeout=60,
+                parent=self.rd,
+                title="Shutdown",
+                text="The PC is about to shutdown. Cancel?",
+                buttons=TimedMessageBox.Cancel,
+            )
+            if not ans == TimedMessageBox.Cancel:
+                shutdown()
 
     def start(self):
         kwds = self.prepare_start()
         if kwds:
             # Plot functions with interactive plots currently can't
             # run in a separate thread, so they
             #  excuted in the main thread
@@ -423,37 +440,39 @@
             show_plots = self.ct.get_setting("show_plots")
             use_qthread = QS().value("use_qthread")
             if (
                 ismayavi
                 or (ismpl and show_plots and use_qthread)
                 or (ismpl and not show_plots and use_qthread and ismac)
             ):
-                logging.info("Starting in Main-Thread.")
+                logger().info("Starting in Main-Thread.")
                 result = run_func(**kwds)
                 self.process_finished(result)
 
             elif QS().value("use_qthread"):
-                logging.info("Starting in separate Thread.")
+                logger().info("Starting in separate Thread.")
                 worker = Worker(function=run_func, **kwds)
                 worker.signals.error.connect(self.process_finished)
                 worker.signals.finished.connect(self.process_finished)
                 QThreadPool.globalInstance().start(worker)
 
             else:
-                logging.info("Starting in process from multiprocessing.")
+                logger().info("Starting in process from multiprocessing.")
                 recv_pipe, send_pipe = Pipe(False)
                 kwds["pipe"] = send_pipe
                 stream_rcv = StreamReceiver(recv_pipe)
                 stream_rcv.signals.stdout_received.connect(
                     self.rd.console_widget.write_stdout
                 )
                 stream_rcv.signals.stderr_received.connect(
                     self.rd.console_widget.write_stderr
                 )
-                stream_rcv.signals.progress_received.connect(
-                    self.rd.console_widget.write_progress
-                )
                 QThreadPool.globalInstance().start(stream_rcv)
                 # ToDO: MP
                 self.pool.apply_async(
                     func=run_func, kwds=kwds, callback=self.process_finished
                 )
+
+
+def close_all():
+    plt.close("all")
+    gc.collect()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/legacy.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/legacy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 import json
-import logging
 import os
 import subprocess
 import sys
 from os.path import isdir, join, isfile
 
 from mne_pipeline_hd.pipeline.loading import MEEG, FSMRI, Group
-from mne_pipeline_hd.pipeline.pipeline_utils import type_json_hook
+from mne_pipeline_hd.pipeline.pipeline_utils import type_json_hook, logger
 
 renamed_parameters = {
     "filter_target": {"Raw": "raw", "Epochs": "epochs", "Evoked": "evoked"},
     "bad_interpolation": {
         "Raw (Filtered)": "raw_filtered",
         "Epochs": "epochs",
         "Evoked": "evoked",
@@ -47,24 +46,24 @@
 }
 
 # New packages with {import_name: install_name} (can be the same)
 new_packages = {"qdarktheme": "pyqtdarktheme"}
 
 
 def install_package(package_name):
-    print(f"Installing {package_name}...")
+    logger().info(f"Installing {package_name}...")
     print(
         subprocess.check_output(
             [sys.executable, "-m", "pip", "install", package_name], text=True
         )
     )
 
 
 def uninstall_package(package_name):
-    print(f"Uninstalling {package_name}...")
+    logger().info(f"Uninstalling {package_name}...")
     print(
         subprocess.check_output(
             [sys.executable, "-m", "pip", "uninstall", "-y", package_name], text=True
         )
     )
 
 
@@ -77,35 +76,37 @@
     if test_package is not None:
         new_packages[test_package] = test_package
 
     for import_name, install_name in new_packages.items():
         try:
             __import__(import_name)
         except ImportError:
-            print(f"The package {import_name} " f"is required for this application.\n")
+            logger().info(
+                f"The package {import_name} " f"is required for this application.\n"
+            )
             ans = input("Do you want to install the " "new package now? [y/n]").lower()
             if ans == "y":
                 try:
                     install_package(install_name)
                 except subprocess.CalledProcessError:
-                    print("Installation failed!")
+                    logger().critical("Installation failed!")
                 else:
                     return
-            print(
+            logger().info(
                 f"Please install the new package {import_name} "
                 f"manually with:\n\n"
                 f"> pip install {install_name}"
             )
             sys.exit(1)
 
 
 def transfer_file_params_to_single_subject(ct):
     old_fp_path = join(ct.pr.pscripts_path, f"file_parameters_{ct.pr.name}.json")
     if isfile(old_fp_path):
-        logging.info("Transfering File-Parameters to single files...")
+        logger().info("Transfering File-Parameters to single files...")
         with open(old_fp_path, "r") as file:
             file_parameters = json.load(file, object_hook=type_json_hook)
             for obj_name in file_parameters:
                 if obj_name in ct.pr.all_meeg:
                     obj = MEEG(obj_name, ct)
                 elif obj_name in ct.pr.all_fsmri:
                     obj = FSMRI(obj_name, ct)
@@ -116,8 +117,8 @@
                 if obj is not None:
                     if not isdir(obj.save_dir):
                         continue
                     obj.file_parameters = file_parameters[obj_name]
                     obj.save_file_parameter_file()
                     obj.clean_file_parameters()
         os.remove(old_fp_path)
-        logging.info("Done!")
+        logger().info("Done!")
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/loading.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/loading.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,46 +7,36 @@
 
 from __future__ import print_function
 
 import functools
 import inspect
 import itertools
 import json
-import logging
 import os
 import pickle
 import shutil
 from datetime import datetime
-from os import listdir, makedirs, remove
+from os import listdir, makedirs
 from os.path import exists, getsize, isdir, isfile, join
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import mne
+import mne_connectivity
 import numpy as np
-
-# =============================================================================
-# LOADING FUNCTIONS
-# =============================================================================
 from tqdm import tqdm
 
 from mne_pipeline_hd.pipeline.pipeline_utils import (
     TypedJSONEncoder,
     type_json_hook,
     QS,
     _test_run,
+    logger,
 )
 
-sample_paths = {
-    "raw": "sample_audvis_raw.fif",
-    "erm": "ernoise_raw.fif",
-    "events": "sample_audvis_raw-eve.fif",
-    "trans": "sample_audvis_raw-trans.fif",
-}
-
 
 def _get_data_type_from_func(self, func, method):
     # Get matching data-type from IO-Dict
     func_name = func.__name__
     data_type = None
     for dt in self.io_dict:
         io_func = self.io_dict[dt][method]
@@ -60,57 +50,62 @@
 
 
 def load_decorator(load_func):
     @functools.wraps(load_func)
     def load_wrapper(self, *args, **kwargs):
         # Get matching data-type from IO-Dict
         data_type = _get_data_type_from_func(self, load_func, "load")
-        print(f"Loading {data_type} for {self.name}")
+        logger().info(f"Loading {data_type} for {self.name}")
 
         if data_type in self.data_dict:
             data = self.data_dict[data_type]
         else:
             # Todo: Dependencies!
             try:
                 data = load_func(self, *args, **kwargs)
-            except OSError as err:
-                deprc_path = self.deprecated_paths.get(data_type, "")
-                if isfile(deprc_path):
-                    new_path = self.io_dict[data_type]["path"]
-                    self.io_dict[data_type]["path"] = deprc_path
-                    data = load_func(self, *args, **kwargs)
-                    self.io_dict[data_type]["path"] = new_path
-                    logging.info(
-                        f"Deprecated path: Saving file for "
-                        f"{data_type} in updated path..."
-                    )
-                    # Save data with new path
-                    save_func = self.io_dict[data_type]["save"]
-                    # Does only support save-functions with no extra args
-                    save_func(self, data)
-                    # Remove deprecated path
-                    os.remove(deprc_path)
-
-                elif self.p_preset != "Default":
-                    print(
-                        f"No File for {data_type} from {self.name}"
-                        f" with Parameter-Preset={self.p_preset} found,"
-                        f" trying Default"
-                    )
-
-                    actual_p_preset = self.p_preset
-                    self.p_preset = "Default"
-                    self.init_paths()
-
-                    data = load_func(*args, **kwargs)
-
-                    self.p_preset = actual_p_preset
-                    self.init_paths()
+            except (OSError, FileNotFoundError) as err:
+                deprc_paths = self.deprecated_paths.get(data_type, "")
+                if isinstance(deprc_paths, dict):
+                    deprc_paths = deprc_paths.values()
                 else:
-                    raise err
+                    deprc_paths = [deprc_paths]
+                for dp in deprc_paths:
+                    if isfile(dp):
+                        new_path = self.io_dict[data_type]["path"]
+                        self.io_dict[data_type]["path"] = dp
+                        data = load_func(self, *args, **kwargs)
+                        self.io_dict[data_type]["path"] = new_path
+                        logger().info(
+                            f"Deprecated path: Saving file for "
+                            f"{data_type} in updated path..."
+                        )
+                        # Save data with new path
+                        save_func = self.io_dict[data_type]["save"]
+                        # Does only support save-functions with no extra args
+                        save_func(data)
+                        # Remove deprecated path
+                        os.remove(dp)
+
+                    elif self.p_preset != "Default":
+                        logger().info(
+                            f"No File for {data_type} from {self.name}"
+                            f" with Parameter-Preset={self.p_preset} found,"
+                            f" trying Default"
+                        )
+
+                        actual_p_preset = self.p_preset
+                        self.p_preset = "Default"
+                        self.init_paths()
+
+                        data = load_func(self, *args, **kwargs)
+
+                        self.p_preset = actual_p_preset
+                        self.init_paths()
+                    else:
+                        raise err
 
         # Save data in data-dict for machines with big RAM
         if not QS().value("save_ram"):
             self.data_dict[data_type] = data
 
         return data
 
@@ -132,74 +127,83 @@
             data = None
 
         # Make sure, that parent-directory exists
         paths = self._return_path_list(data_type)
         for path in [p for p in paths if not isdir(Path(p).parent)]:
             makedirs(Path(path).parent, exist_ok=True)
 
-        print(f"Saving {data_type} for {self.name}")
+        logger().info(f"Saving {data_type} for {self.name}")
         save_func(self, *args, **kwargs)
 
         # Save data in data-dict for machines with big RAM
         if not QS().value("save_ram"):
             self.data_dict[data_type] = data
 
         # Save File-Parameters
         paths = self._return_path_list(data_type)
         for path in paths:
             self.save_file_params(path)
 
     return save_wrapper
 
 
+# ToDo: Unify all objects to one loading-class
+# For example Group and MEEG can have the same load-method for Source-Estimates then
 class BaseLoading:
     """Base-Class for Sub (The current File/MRI-File/Grand-Average-Group,
     which is executed)"""
 
     def __init__(self, name, controller):
         # Basic Attributes (partly taking parameters or main-win-attributes
         # for easier access)
         self.name = name
         self.ct = controller
         self.pr = controller.pr
         self.p_preset = self.pr.p_preset
+        self.pa = self.pr.parameters[self.p_preset]
         self.subjects_dir = self.ct.subjects_dir
         self.save_plots = self.ct.get_setting("save_plots")
         self.figures_path = self.pr.figures_path
         self.img_format = self.ct.get_setting("img_format")
         self.dpi = self.ct.get_setting("dpi")
 
         self.data_dict = dict()
         self.existing_paths = dict()
 
+        self.init_attributes()
         if name is not None:
-            self.init_parameters()
-            self.init_attributes()
+            self.init_plot_files()
             self.init_paths()
             self.load_file_parameter_file()
 
-    def init_parameters(self):
-        self.pa = self.pr.parameters[self.p_preset]
-
+    def init_plot_files(self):
         # Prepare plot-files-dictionary for Loading-Object
         if self.name not in self.pr.plot_files:
             self.pr.plot_files[self.name] = dict()
         if self.p_preset not in self.pr.plot_files[self.name]:
             self.pr.plot_files[self.name][self.p_preset] = dict()
         self.plot_files = self.pr.plot_files[self.name][self.p_preset]
 
+    def get_parameter(self, parameter_name):
+        """Get parameter from parameter-dictionary"""
+
+        if parameter_name in self.pa:
+            return self.pa[parameter_name]
+        else:
+            raise KeyError(f"Parameter {parameter_name} not found in parameters")
+
     def init_attributes(self):
         """Initialization of additional attributes, should be overridden
         in inherited classes"""
         pass
 
     def init_paths(self):
         """Initialization of all paths and the io_dict, should be overridden
         in inherited classes"""
-        self.save_dir = None
+        self.save_dir = ""
         self.io_dict = dict()
         self.deprecated_paths = dict()
 
     def _return_path_list(self, data_type):
         paths = self.io_dict[data_type]["path"]
         # Convert paths to list
         if not isinstance(paths, list):
@@ -313,27 +317,28 @@
                 for param in remove_params:
                     self.file_parameters[file_name].pop(param)
 
                 n_remove_params += len(remove_params)
 
         for file_name in remove_files:
             self.file_parameters.pop(file_name)
-        print(
+        logger().info(
             f"Removed {len(remove_files)} Files " f"and {n_remove_params} Parameters."
         )
         self.save_file_parameter_file()
 
     # Todo: Type recognition
     def plot_save(
         self,
         plot_name,
         subfolder=None,
         trial=None,
         idx=None,
         matplotlib_figure=None,
+        pyvista_figure=None,
         brain=None,
         brain_movie_kwargs=None,
         dpi=None,
         img_format=None,
     ):
         """
         Save a plot with this method either by letting the figure be detected
@@ -351,14 +356,16 @@
             An optinal name of the trial if you have several trials from the
              same run.
         idx : int | str | None
             An optional index as enumerator for multiple plots.
         matplotlib_figure : matplotlib.figure.Figure | None
             Supply a matplotlib-figure here (if none is given,
              the current-figure will be taken with plt.savefig()).
+        pyvista_figure: pyvista.Plotter
+            Supply a pyvista-plotter here.
         brain : mne.viz.Brain | None
             Supply a Brain-instance here.
         brain_movie_kwargs : dict
             Supply keyword-arguments for brain.save_movie() here.
         dpi :
             Set the dpi-setting if you want another than specified
              in the MainWindow-Settings.
@@ -413,74 +420,105 @@
                         # (easier with removesuffix when moving to 3.9)
                         idx_file_name = (
                             f"{file_name[:-len(self.img_format)]}"
                             f"--{ix}{self.img_format}"
                         )
                         idx_file_path = join(dir_path, idx_file_name)
                         figure.savefig(idx_file_path)
-                        print(f"figure: {idx_file_path} has been saved")
+                        logger().info(f"figure: {idx_file_path} has been saved")
                         # Only store relative path to be compatible across OS
                         plot_files_save_path = os.path.relpath(
                             idx_file_path, self.figures_path
                         )
                         # Add Plot-Save-Path to plot_files
                         # if not already contained
                         if plot_files_save_path not in self.plot_files[calling_func]:
                             self.plot_files[calling_func].append(plot_files_save_path)
                 else:
                     matplotlib_figure.savefig(save_path, dpi=dpi)
+            elif pyvista_figure:
+                if self.img_format != ".svg":
+                    file_name = file_name.strip(self.img_format) + ".svg"
+                    save_path = join(dir_path, file_name)
+                    logger().info("Pyvista-Plots are saved as .svg")
+                pyvista_figure.plotter.save_graphics(save_path, title=file_name)
             elif brain:
                 if brain_movie_kwargs is not None:
                     time_dilation = brain_movie_kwargs["stc_animation_dilat"]
                     tmin, tmax = brain_movie_kwargs["stc_animation_span"]
                     brain.save_movie(
                         save_path, time_dilation=time_dilation, tmin=tmin, tmax=tmax
                     )
                 else:
                     brain.save_image(save_path)
             else:
                 plt.savefig(save_path, dpi=dpi)
-            print(f"figure: {save_path} has been saved")
+            logger().info(f"figure: {save_path} has been saved")
 
             if not isinstance(matplotlib_figure, list):
                 # Only store relative path to be compatible across OS
                 plot_files_save_path = os.path.relpath(save_path, self.figures_path)
                 # Add Plot-Save-Path to plot_files if not already contained
                 if plot_files_save_path not in self.plot_files[calling_func]:
                     self.plot_files[calling_func].append(plot_files_save_path)
         else:
-            print('Not saving plots; set "save_plots" to "True" to save')
+            logger().info('Not saving plots; set "save_plots" to "True" to save')
+
+    # ToDo: Should have load-decorator!
+    def load(self, data_type, **kwargs):
+        """General load function with data_type as parameter."""
+        load_func = self.io_dict[data_type]["load"]
+        if load_func is not None:
+            return load_func(**kwargs)
+
+    # Should have save-decorator!
+    def save(self, data_type, data, **kwargs):
+        """General save function with data_type as parameter."""
+        save_func = self.io_dict[data_type]["save"]
+        if save_func is not None:
+            save_func(data, **kwargs)
 
     def load_json(self, file_name, default=None):
         file_path = join(self.save_dir, f"{self.name}_{self.p_preset}_{file_name}.json")
         try:
             with open(file_path, "r") as file:
                 data = json.load(file, object_hook=type_json_hook)
         except json.JSONDecodeError:
-            print(f"{file_path} could not be loaded")
+            logger().warning(f"{file_path} could not be loaded")
             data = default
         except FileNotFoundError:
-            print(f"{file_path} could not be found")
+            logger().warning(f"{file_path} could not be found")
             data = default
 
         return data
 
     def save_json(self, file_name, data):
         # If file-ending is supplied, remove it to avoid doubling
         if file_name[-5:] == ".json":
             file_name = file_name[:-5]
         file_path = join(self.save_dir, f"{self.name}_{self.p_preset}_{file_name}.json")
         try:
             with open(file_path, "w") as file:
                 json.dump(data, file, cls=TypedJSONEncoder, indent=4)
         except json.JSONDecodeError:
-            print(f"{file_path} could not be saved")
+            logger().warning(f"{file_path} could not be saved")
 
         self.save_file_params(file_path)
 
+    def remove_json(self, file_name):
+        file_path = join(self.save_dir, f"{self.name}_{self.p_preset}_{file_name}.json")
+        try:
+            os.remove(file_path)
+        except FileNotFoundError:
+            logger().warning(f"{file_path} was not found")
+        except OSError as err:
+            logger().warning(f"{file_path} could not be removed due to {err}")
+        else:
+            logger().warning(f"{file_path} was removed")
+
     def get_existing_paths(self):
         """Get existing paths and add the mapped File-Type
         to existing_paths (set)"""
         self.existing_paths.clear()
         for data_type in self.io_dict:
             paths = self._return_path_list(data_type)
             if paths:
@@ -509,35 +547,52 @@
                 # Accounting for Source-Estimate naming-conventions
                 try:
                     p_name_lh = p_name + "-lh.stc"
                     p_name_rh = p_name + "-rh.stc"
                     for pn in [p_name_lh, p_name_rh]:
                         self.file_parameters.pop(pn)
                 except KeyError:
-                    print(f"{Path(p).name} not in file-parameters")
+                    logger().warning(f"{Path(p).name} not in file-parameters")
             try:
-                remove(p)
+                os.remove(p)
             except FileNotFoundError:
                 # Accounting for Source-Estimate naming-conventions
                 try:
                     p_lh = p + "-lh.stc"
                     p_rh = p + "-rh.stc"
                     for ps in [p_lh, p_rh]:
                         os.remove(ps)
                 except FileNotFoundError:
-                    print(f"{p} was not found")
+                    logger().warning(f"{p} was not found")
             except IsADirectoryError:
                 try:
                     shutil.rmtree(p)
                 except OSError as err:
-                    print(f"{p} could not be removed due to {err}")
+                    logger().warning(f"{p} could not be removed due to {err}")
             except OSError as err:
-                print(f"{p} could not be removed due to {err}")
+                logger().warning(f"{p} could not be removed due to {err}")
+            else:
+                logger().warning(f"{p} was removed")
+
+
+sample_paths = {
+    "raw": "sample_audvis_raw.fif",
+    "erm": "ernoise_raw.fif",
+    "events": "sample_audvis_raw-eve.fif",
+    "evoked": "sample_audvis-ave.fif",
+    "noise_cov": "sample_audvis-cov.fif",
+    "forward": "sample_audvis-meg-eeg-oct-6-fwd.fif",
+    "inverse": "sample_audvis-meg-eeg-oct-6-meg-eeg-inv.fif",
+    "stcs": "sample_audvis-meg-eeg",
+}
 
 
+# ToDo: Currently there is duplication with attribute for Path and io_dict['path'].
+#  In the future there should be only one,
+#  favor io_dict (better than attribute since easier to set from config-files)
 class MEEG(BaseLoading):
     """Class for File-Data in File-Loop"""
 
     def __init__(self, name, controller, fsmri=None, suppress_warnings=True):
         self.fsmri = fsmri
         self.suppress_warnings = suppress_warnings
         super().__init__(name, controller)
@@ -547,15 +602,15 @@
 
     def init_attributes(self):
         """Initialize additional attributes for MEEG"""
         # The assigned Empty-Room-Measurement if existing
         if self.name not in self.pr.meeg_to_erm:
             self.erm = None
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No Empty-Room-Measurement assigned for {self.name},"
                     f' defaulting to "None"'
                 )
         else:
             # Transition from 'None' to None (placed 30.01.2021,
             # can be removed soon)
             if self.pr.meeg_to_erm[self.name] == "None":
@@ -567,56 +622,66 @@
             if self.fsmri and self.fsmri.name == self.pr.meeg_to_fsmri[self.name]:
                 pass
             else:
                 self.fsmri = FSMRI(self.pr.meeg_to_fsmri[self.name], self.ct)
         else:
             self.fsmri = FSMRI(None, self.ct)
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No Freesurfer-MRI-Subject assigned for {self.name},"
                     f' defaulting to "None"'
                 )
 
         # The assigned bad-channels
         if self.name not in self.pr.meeg_bad_channels:
             self.bad_channels = list()
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No bad channels assigned for {self.name},"
                     f" defaulting to empty list"
                 )
         else:
             self.bad_channels = self.pr.meeg_bad_channels[self.name]
 
         # The selected trials from the event-id
         if self.name not in self.pr.sel_event_id:
-            self.sel_trials = list()
+            self.sel_trials = dict()
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No Trials selected for {self.name}," f" defaulting to empty list"
                 )
         else:
             self.sel_trials = self.pr.sel_event_id[self.name]
+            # Legacy for before when sel_event_id was a list
+            if isinstance(self.sel_trials, list):
+                self.sel_trials = {k: None for k in self.sel_trials}
+                self.pr.sel_event_id[self.name] = self.sel_trials
 
         # The assigned event-id
         if self.name not in self.pr.meeg_event_id:
             self.event_id = dict()
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No EventID assigned for {self.name},"
                     f" defaulting to empty dictionary"
                 )
         else:
             # Only inlcude event-ids which are selected
             self.event_id = {
                 key: value
                 for key, value in self.pr.meeg_event_id[self.name].items()
                 if any([k in self.sel_trials for k in key.split("/")])
             }
 
+        # The excluded ica-components
+        if self.name not in self.pr.meeg_ica_exclude:
+            self.ica_exclude = list()
+        else:
+            self.ica_exclude = self.pr.meeg_ica_exclude[self.name]
+
     def init_paths(self):
         """Load Paths as attributes
         (depending on which Parameter-Preset is selected)"""
 
         # Main save directory
         self.save_dir = join(self.pr.data_path, self.name)
         if not isdir(self.save_dir):
@@ -649,14 +714,20 @@
         self.eog_epochs_path = join(
             self.save_dir, f"{self.name}_{self.p_preset}-eog-epo.fif"
         )
         self.ecg_epochs_path = join(
             self.save_dir, f"{self.name}_{self.p_preset}-ecg-epo.fif"
         )
         self.evokeds_path = join(self.save_dir, f"{self.name}_{self.p_preset}-ave.fif")
+        self.psd_raw_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-raw-psd.h5"
+        )
+        self.psd_epochs_path = join(
+            self.save_dir, f"{self.name}_{self.p_preset}-epo-psd.h5"
+        )
         self.power_tfr_epochs_path = join(
             self.save_dir,
             f"{self.name}_{self.p_preset}_" f'#{self.pa["tfr_method"]}-epo-pw-tfr.h5',
         )
         self.itc_tfr_epochs_path = join(
             self.save_dir,
             f"{self.name}_{self.p_preset}_" f'{self.pa["tfr_method"]}-epo-itc-tfr.h5',
@@ -716,15 +787,16 @@
             }
             for trial in self.sel_trials
         }
         self.con_paths = {
             trial: {
                 con_method: join(
                     self.save_dir,
-                    f"{self.name}_{trial}_{self.p_preset}_{con_method}-con.npy",
+                    "connectivity",
+                    f"{self.name}_{trial}_{self.p_preset}_{con_method}-con.nc",
                 )
                 for con_method in self.pa["con_methods"]
             }
             for trial in self.sel_trials
         }
 
         # This dictionary contains entries for each data-type
@@ -777,14 +849,26 @@
                 "save": self.save_ecg_epochs,
             },
             "evoked": {
                 "path": self.evokeds_path,
                 "load": self.load_evokeds,
                 "save": self.save_evokeds,
             },
+            "evoked_eog": {"path": None, "load": self.load_eog_evokeds, "save": None},
+            "evoked_ecg": {"path": None, "load": self.load_ecg_evokeds, "save": None},
+            "psd_raw": {
+                "path": self.psd_raw_path,
+                "load": self.load_psd_raw,
+                "save": self.save_psd_raw,
+            },
+            "psd_epochs": {
+                "path": self.psd_epochs_path,
+                "load": self.load_psd_epochs,
+                "save": self.save_psd_epochs,
+            },
             "tf_power_epochs": {
                 "path": self.power_tfr_epochs_path,
                 "load": self.load_power_tfr_epochs,
                 "save": self.save_power_tfr_epochs,
             },
             "tf_itc_epochs": {
                 "path": self.itc_tfr_epochs_path,
@@ -800,15 +884,15 @@
                 "path": self.itc_tfr_average_path,
                 "load": self.load_itc_tfr_average,
                 "save": self.save_itc_tfr_average,
             },
             "trans": {
                 "path": self.trans_path,
                 "load": self.load_transformation,
-                "save": None,
+                "save": self.save_transformation,
             },
             "forward": {
                 "path": self.forward_path,
                 "load": self.load_forward,
                 "save": self.save_forward,
             },
             "morph": {
@@ -861,33 +945,65 @@
         }
 
     def init_sample(self):
         # Add _sample_ to project and update attributes
         self.pr.all_erm.append("ernoise")
         self.erm = "ernoise"
         self.pr.meeg_to_erm[self.name] = self.erm
+
+        self.pr.meeg_to_fsmri[self.name] = "fsaverage"
+        self.fsmri = FSMRI("fsaverage", self.ct)
+
+        # Add event_id
+        if self.name not in self.pr.meeg_event_id:
+            self.event_id = {
+                "auditory/left": 1,
+                "auditory/right": 2,
+                "visual/left": 3,
+                "visual/right": 4,
+                "face": 5,
+                "buttonpress": 32,
+            }
+            self.pr.meeg_event_id[self.name] = self.event_id
+        else:
+            self.event_id = self.pr.meeg_event_id[self.name]
+
+        # ToDo: Here is problem, since there is no way
+        #  to select "auditory/left" from the gui.
+        if self.name not in self.pr.sel_event_id:
+            self.sel_trials = {"auditory": None}
+            self.pr.sel_event_id[self.name] = self.sel_trials
+        else:
+            self.sel_trials = self.pr.sel_event_id[self.name]
+
+        # init paths again
         self.init_paths()
 
         # Load sample
         test_data_folder = join(mne.datasets.sample.data_path(), "MEG", "sample")
-        test_file_dict = sample_paths
 
-        for data_type in test_file_dict:
-            test_file_name = test_file_dict[data_type]
+        for data_type in sample_paths:
+            test_file_name = sample_paths[data_type]
             test_file_path = join(test_data_folder, test_file_name)
             file_path = self.io_dict[data_type]["path"]
-
-            if isfile(test_file_path) and not isfile(file_path):
-                print(f"Copying {data_type} from sample-dataset...")
+            if data_type == "stcs":
+                file_path = file_path["auditory"]
+                if not isfile(file_path + "-lh.stc"):
+                    logger().debug(f"Copying {data_type} from sample-dataset...")
+                    stcs = mne.source_estimate.read_source_estimate(test_file_path)
+                    stcs.save(file_path)
+            elif isfile(test_file_path) and not isfile(file_path):
+                logger().debug(f"Copying {data_type} from sample-dataset...")
                 folder = Path(file_path).parent
                 if not isdir(folder):
                     os.mkdir(folder)
                 shutil.copy2(test_file_path, file_path)
-                print("Done!")
+                logger().debug("Done!")
 
+        # Add bad_channels
         self.bad_channels = self.load_info()["bads"]
         self.pr.meeg_bad_channels[self.name] = self.bad_channels
 
     def rename(self, new_name):
         # Stor old name
         old_name = self.name
         all_old_paths = dict()
@@ -918,14 +1034,22 @@
         for data_type in self.io_dict:
             new_paths = self._return_path_list(data_type)
             old_paths = all_old_paths[data_type]
             for new_path, old_path in zip(new_paths, old_paths):
                 if isfile(old_path):
                     os.renames(old_path, new_path)
 
+    def set_bad_channels(self, bad_channels):
+        self.bad_channels = bad_channels
+        self.pr.meeg_bad_channels[self.name] = self.bad_channels
+
+    def set_ica_exclude(self, ica_exclude):
+        self.ica_exclude = ica_exclude
+        self.pr.meeg_ica_exclude[self.name] = self.ica_exclude
+
     ###########################################################################
     # Load- & Save-Methods
     ###########################################################################
 
     def load_info(self):
         return mne.io.read_info(self.raw_path)
 
@@ -938,15 +1062,14 @@
     @save_decorator
     def save_raw(self, raw):
         raw.save(self.raw_path, fmt=raw.orig_format, overwrite=True)
 
     @load_decorator
     def load_filtered(self):
         raw = mne.io.read_raw_fif(self.raw_filtered_path, preload=True)
-        raw.info["bads"] = [bc for bc in self.bad_channels if bc in raw.ch_names]
         return raw
 
     @save_decorator
     def save_filtered(self, raw_filtered):
         raw_filtered.save(
             self.raw_filtered_path, fmt=raw_filtered.orig_format, overwrite=True
         )
@@ -982,14 +1105,27 @@
             self.epochs_path, proj=self.pa["apply_proj"], preload=True
         )
 
     @save_decorator
     def save_epochs(self, epochs):
         epochs.save(self.epochs_path, overwrite=True)
 
+    def get_trial_epochs(self):
+        """Return epochs for each trial in self.sel_trials"""
+        epochs = self.load_epochs()
+        for trial, meta_query in self.sel_trials.items():
+            epoch_trial = meta_query or trial
+            # ToDo: Make this optional (at own risk) and not for normal trials
+            try:
+                epoch_trial = eval(epoch_trial)
+            except (NameError, SyntaxError, ValueError, TypeError):
+                pass
+
+            yield trial, epochs[epoch_trial]
+
     @load_decorator
     def load_reject_log(self):
         with open(self.reject_log_path, "rb") as file:
             return pickle.load(file)
 
     @save_decorator
     def save_reject_log(self, reject_log):
@@ -997,16 +1133,16 @@
             pickle.dump(reject_log, file)
 
     @load_decorator
     def load_ica(self):
         ica = mne.preprocessing.read_ica(self.ica_path)
         # Change ica.exclude to indices stored in ica_exclude.py
         # for this MEEG-Object
-        if self.name in self.pr.ica_exclude:
-            ica.exclude = self.pr.ica_exclude[self.name]
+        if self.name in self.pr.meeg_ica_exclude:
+            ica.exclude = self.pr.meeg_ica_exclude[self.name]
         return ica
 
     @save_decorator
     def save_ica(self, ica):
         ica.save(self.ica_path, overwrite=True)
 
     @load_decorator
@@ -1030,14 +1166,38 @@
         return mne.read_evokeds(self.evokeds_path, proj=self.pa["apply_proj"])
 
     @save_decorator
     def save_evokeds(self, evokeds):
         mne.evoked.write_evokeds(self.evokeds_path, evokeds, overwrite=True)
 
     @load_decorator
+    def load_eog_evokeds(self):
+        return self.load_eog_epochs().average()
+
+    @load_decorator
+    def load_ecg_evokeds(self):
+        return self.load_ecg_epochs().average()
+
+    @load_decorator
+    def load_psd_raw(self):
+        return mne.time_frequency.read_spectrum(self.psd_raw_path)
+
+    @save_decorator
+    def save_psd_raw(self, psd_raw):
+        psd_raw.save(self.psd_raw_path, overwrite=True)
+
+    @load_decorator
+    def load_psd_epochs(self):
+        return mne.time_frequency.read_spectrum(self.psd_epochs_path)
+
+    @save_decorator
+    def save_psd_epochs(self, psd_epochs):
+        psd_epochs.save(self.psd_epochs_path, overwrite=True)
+
+    @load_decorator
     def load_power_tfr_epochs(self):
         return mne.time_frequency.read_tfrs(self.power_tfr_epochs_path)
 
     @save_decorator
     def save_power_tfr_epochs(self, powers):
         mne.time_frequency.write_tfrs(
             self.power_tfr_epochs_path, powers, overwrite=True
@@ -1067,16 +1227,23 @@
 
     @save_decorator
     def save_itc_tfr_average(self, itcs):
         mne.time_frequency.write_tfrs(self.itc_tfr_average_path, itcs, overwrite=True)
 
     @load_decorator
     def load_transformation(self):
+        # Load built-in transformation for fsaverage
+        if self.fsmri.name == "fsaverage":
+            return "fsaverage"
         return mne.read_trans(self.trans_path)
 
+    @save_decorator
+    def save_transformation(self, trans):
+        mne.write_trans(self.trans_path, trans, overwrite=True)
+
     @load_decorator
     def load_forward(self):
         return mne.read_forward_solution(self.forward_path, verbose="WARNING")
 
     @save_decorator
     def save_forward(self, forward):
         mne.write_forward_solution(self.forward_path, forward, overwrite=True)
@@ -1149,25 +1316,25 @@
                     self.save_dir,
                     "mixn_dipoles",
                     f"{self.name}_{trial}_" f"{self.p_preset}-mixn-dip{idx}.dip",
                 )
                 dip_list.append(mne.read_dipole(mixn_dip_path))
                 idx += 1
             mixn_dips[trial] = dip_list
-            print(f"{idx + 1} dipoles read for {self.name}-{trial}")
+            logger().info(f"{idx + 1} dipoles read for {self.name}-{trial}")
 
         return mixn_dips
 
     def save_mixn_dipoles(self, mixn_dips):
         # Remove old dipoles
         if not exists(join(self.save_dir, "mixn_dipoles")):
             makedirs(join(self.save_dir, "mixn_dipoles"))
         old_dipoles = listdir(join(self.save_dir, "mixn_dipoles"))
         for file in old_dipoles:
-            remove(join(self.save_dir, "mixn_dipoles", file))
+            os.remove(join(self.save_dir, "mixn_dipoles", file))
 
         for trial in mixn_dips:
             for idx, dip in enumerate(mixn_dips[trial]):
                 mxn_dip_path = join(
                     self.save_dir,
                     "mixn_dipoles",
                     f"{self.name}_{trial}_" f"{self.p_preset}-mixn-dip{idx}.dip",
@@ -1194,14 +1361,17 @@
     def load_ecd(self):
         ecd_dipoles = dict()
         for trial in self.ecd_paths:
             ecd_dipoles[trial] = dict()
             for dip in self.ecd_paths[trial]:
                 ecd_dipoles[trial][dip] = mne.read_dipole(self.ecd_paths[trial][dip])
 
+        if all([len(ecd_dipoles[trial]) == 0 for trial in ecd_dipoles]):
+            raise FileNotFoundError(f"No ECD-Dipoles found for {self.name}!")
+
         return ecd_dipoles
 
     @save_decorator
     def save_ecd(self, ecd_dips):
         for trial in ecd_dips:
             for dip in ecd_dips[trial]:
                 ecd_dips[trial][dip].save(self.ecd_paths[trial][dip], overwrite=True)
@@ -1218,60 +1388,61 @@
                 else:
                     raise FileNotFoundError(
                         f"No Label-Time-Course found "
                         f"for trial {trial} "
                         f"in label {label}!"
                     )
 
+        if all([len(ltcs[trial]) == 0 for trial in ltcs]):
+            raise FileNotFoundError(f"No Label-Time-Courses found for {self.name}!")
+
         return ltcs
 
     @save_decorator
     def save_ltc(self, ltcs):
         for trial in ltcs:
             for label in ltcs[trial]:
                 np.save(self.ltc_paths[trial][label], ltcs[trial][label])
 
     @load_decorator
     def load_connectivity(self):
         con_dict = dict()
         for trial in self.con_paths:
             con_dict[trial] = dict()
-            for con_method in self.con_paths[trial]:
-                con_dict[trial][con_method] = np.load(self.con_paths[trial][con_method])
+            for con_method, con_path in self.con_paths[trial].items():
+                con_dict[trial][con_method] = mne_connectivity.read_connectivity(
+                    con_path
+                )
 
         return con_dict
 
     @save_decorator
     def save_connectivity(self, con_dict):
+        # Write info about label and parcellation into json
         for trial in con_dict:
-            for con_method in con_dict[trial]:
-                np.save(self.con_paths[trial][con_method], con_dict[trial][con_method])
+            for con_method, con in con_dict[trial].items():
+                con.save(self.con_paths[trial][con_method])
+
+
+fsaverage_paths = {
+    "src": "bem/fsaverage-ico-5-src.fif",
+    "bem_model": "bem/fsaverage-5120-5120-5120-bem.fif",
+    "bem_solution": "bem/fsaverage-5120-5120-5120-bem-sol.fif",
+    "volume_src": "bem/fsaverage-vol-5-src.fif",
+}
 
 
 class FSMRI(BaseLoading):
     def __init__(self, name, controller, load_labels=False):
-        if name == "fsaverage" and not isfile(
-            join(controller.subjects_dir, "fsaverage/mri/T1.mgz")
-        ):
-            if _test_run():
-                test_data_folder = join(
-                    mne.datasets.sample.data_path(), "subjects", "fsaverage"
-                )
-                shutil.copytree(test_data_folder, join(controller.subjects_dir, name))
-            else:
-                try:
-                    logging.info("Downloading fsaverage...")
-                    mne.datasets.fetch_fsaverage(subjects_dir=controller.subjects_dir)
-                # Not working on macOS for mne<=0.24
-                except ValueError:
-                    logging.warning("fsaverage could not be downloaded!")
-
         self.load_labels = load_labels
         super().__init__(name, controller)
 
+        if name == "fsaverage":
+            self.init_fsaverage()
+
     def init_attributes(self):
         """Initialize additional attributes for FSMRI"""
         self.fs_path = QS().value("fs_path")
         self.mne_path = QS().value("mne_path")
 
         # Initialize Parcellations and Labels
         if self.load_labels:
@@ -1281,183 +1452,223 @@
             self.parcellations = None
             self.labels = None
 
     def init_paths(self):
         # Main Path
         self.save_dir = join(self.subjects_dir, self.name)
 
-        # Data-Paths
-        self.src_path = join(
-            self.save_dir,
-            "bem",
-            f'{self.name}_{self.p_preset}_{self.pa["src_spacing"]}-src.fif',
-        )
-        self.bem_model_path = join(
-            self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem.fif"
-        )
-        self.bem_solution_path = join(
-            self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem-sol.fif"
-        )
-        self.vol_src_path = join(
-            self.save_dir, "bem", f"{self.name}_{self.p_preset}-vol-src.fif"
-        )
-
         # This dictionary contains entries for each data-type
         # which is loaded to/saved from disk
         self.io_dict = {
             "src": {
-                "path": self.src_path,
+                "path": join(
+                    self.save_dir,
+                    "bem",
+                    f'{self.name}_{self.p_preset}_{self.pa["src_spacing"]}-src.fif',
+                ),
                 "load": self.load_source_space,
                 "save": self.save_source_space,
             },
             "bem_model": {
-                "path": self.bem_model_path,
+                "path": join(
+                    self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem.fif"
+                ),
                 "load": self.load_bem_model,
                 "save": self.save_bem_model,
             },
             "bem_solution": {
-                "path": self.bem_solution_path,
+                "path": join(
+                    self.save_dir, "bem", f"{self.name}_{self.p_preset}-bem-sol.fif"
+                ),
                 "load": self.load_bem_solution,
                 "save": self.save_bem_solution,
             },
             "volume_src": {
-                "path": self.vol_src_path,
+                "path": join(
+                    self.save_dir, "bem", f"{self.name}_{self.p_preset}-vol-src.fif"
+                ),
                 "load": self.load_volume_source_space,
                 "save": self.save_volume_source_space,
             },
         }
 
         self.deprecated_paths = {
             "src": join(
                 self.save_dir, "bem", f'{self.name}_{self.pa["src_spacing"]}-src.fif'
             ),
             "bem_model": join(self.save_dir, "bem", f"{self.name}-bem.fif"),
             "bem_solution": join(self.save_dir, "bem", f"{self.name}-bem-sol.fif"),
             "volume_src": join(self.save_dir, "bem", f"{self.name}-vol-src.fif"),
         }
 
+    def init_fsaverage(self):
+        # Set SUBJECTS_DIR in config to None for test case,
+        # so fsaverage will be downloaded to "~/mne_data/MNE-fsaverage-data"
+        if _test_run():
+            mne.set_config("SUBJECTS_DIR", None)
+        logger().info("Downloading fsaverage...")
+        fsaverage_dir = mne.datasets.fetch_fsaverage(subjects_dir=None)
+        if _test_run():
+            mne.set_config("SUBJECTS_DIR", self.ct.subjects_dir)
+            new_dir = join(self.ct.subjects_dir, "fsaverage")
+            if not isdir(new_dir):
+                shutil.copytree(fsaverage_dir, new_dir)
+
+        # Rename files to match naming convention
+        for data_type, from_path in fsaverage_paths.items():
+            from_path = join(self.save_dir, from_path)
+            to_path = self.io_dict[data_type]["path"]
+            if not isfile(to_path):
+                os.rename(from_path, to_path)
+                logger().info(f"Renamed {from_path} to {to_path}")
+
     def _get_available_parc(self):
         annot_dir = join(self.subjects_dir, self.name, "label")
         try:
             files = os.listdir(annot_dir)
-            annotations = [file[3:-6] for file in files if file[-6:] == ".annot"]
+            annotations = set([file[3:-6] for file in files if file[-6:] == ".annot"])
         except FileNotFoundError:
-            annotations = list()
+            annotations = set()
 
         return annotations
 
     def _get_available_labels(self):
         labels = dict()
         labels["Other"] = list()
         label_dir = join(self.subjects_dir, self.name, "label")
         try:
             files = os.listdir(label_dir)
             for label_path in tqdm(
                 [str(lp) for lp in files if lp[-6:] == ".label"],
                 desc="Loading labels...",
                 ascii=True,
             ):
-                label = mne.read_label(join(label_dir, label_path), self.name)
+                try:
+                    label = mne.read_label(join(label_dir, label_path), self.name)
+                except ValueError:
+                    logger().warning(f"Label {label_path} could not be loaded!")
                 labels["Other"].append(label)
         except FileNotFoundError:
-            logging.warning(f"No label directory found for {self.name}!")
+            logger().warning(f"No label directory found for {self.name}!")
 
         if self.parcellations is None:
             self.parcellations = self._get_available_parc()
 
         for parcellation in tqdm(
             self.parcellations, desc="Loading parcellations...", ascii=True
         ):
             try:
                 labels[parcellation] = mne.read_labels_from_annot(
                     self.name,
                     parcellation,
                     subjects_dir=self.subjects_dir,
                     verbose="warning",
                 )
-            except RuntimeError:
-                print(f"Parcellation {parcellation} could not be loaded!")
+            except (RuntimeError, OSError):
+                logger().warning(f"Parcellation {parcellation} could not be loaded!")
 
         return labels
 
-    def get_labels(self, target_labels):
+    def get_labels(self, target_labels=None, parcellation=None):
         labels = list()
-        if target_labels is not None:
+        if self.name is None:
+            logger().warning("FSMRI-Object has no name and is empty!")
+        else:
+            # Get available parcellations
             if self.labels is None:
                 self.labels = self._get_available_labels()
-            for label_list in self.labels.values():
-                labels += [lb for lb in label_list if lb.name in target_labels]
+
+            # Subselect labels with parcellation
+            if parcellation is None:
+                search_labels = list()
+                for parcellation in self.labels:
+                    search_labels += self.labels[parcellation]
+            else:
+                if parcellation in self.labels:
+                    search_labels = self.labels[parcellation]
+                else:
+                    raise RuntimeError(
+                        f"Parcellation '{parcellation}' not found for {self.name}!"
+                    )
+
+            if target_labels is not None:
+                labels += [lb for lb in search_labels if lb.name in target_labels]
+            else:
+                labels = search_labels
 
         return labels
 
     ###########################################################################
     # Load- & Save-Methods
     ###########################################################################
     @load_decorator
     def load_source_space(self):
-        return mne.read_source_spaces(self.src_path)
+        return mne.read_source_spaces(self.io_dict["src"]["path"])
 
     @save_decorator
     def save_source_space(self, src):
-        src.save(self.src_path, overwrite=True)
+        src.save(self.io_dict["src"]["path"], overwrite=True)
 
     @load_decorator
     def load_bem_model(self):
-        return mne.read_bem_surfaces(self.bem_model_path)
+        return mne.read_bem_surfaces(self.io_dict["bem_model"]["path"])
 
     @save_decorator
     def save_bem_model(self, bem_model):
-        mne.write_bem_surfaces(self.bem_model_path, bem_model, overwrite=True)
+        mne.write_bem_surfaces(
+            self.io_dict["bem_model"]["path"], bem_model, overwrite=True
+        )
 
     @load_decorator
     def load_bem_solution(self):
-        return mne.read_bem_solution(self.bem_solution_path)
+        return mne.read_bem_solution(self.io_dict["bem_solution"]["path"])
 
     @save_decorator
     def save_bem_solution(self, bem_solution):
-        mne.write_bem_solution(self.bem_solution_path, bem_solution, overwrite=True)
+        mne.write_bem_solution(
+            self.io_dict["bem_solution"]["path"], bem_solution, overwrite=True
+        )
 
     @load_decorator
     def load_volume_source_space(self):
-        return mne.read_source_spaces(self.vol_src_path)
+        return mne.read_source_spaces(self.io_dict["volume_src"]["path"])
 
     @save_decorator
     def save_volume_source_space(self, vol_src):
-        vol_src.save(self.vol_src_path, overwrite=True)
+        vol_src.save(self.io_dict["volume_src"]["path"], overwrite=True)
 
 
 class Group(BaseLoading):
     def __init__(self, name, controller, suppress_warnings=True):
         self.suppress_warnings = suppress_warnings
         super().__init__(name, controller)
 
     def init_attributes(self):
         """Initialize additional attributes for Group"""
         if self.name not in self.pr.all_groups:
             self.group_list = []
             if not self.suppress_warnings:
-                print(
+                logger().warning(
                     f"No objects assigned for {self.name}," f" defaulting to empty list"
                 )
         else:
             self.group_list = self.pr.all_groups[self.name]
 
         # The assigned event-id
         self.event_id = dict()
         for group_item in [
             gi for gi in self.group_list if gi in self.ct.pr.meeg_event_id
         ]:
             self.event_id = {**self.event_id, **self.ct.pr.meeg_event_id[group_item]}
 
-        # The selected trials from the event-id
-        self.sel_trials = set()
-        for group_item in [
-            gi for gi in self.group_list if gi in self.ct.pr.sel_event_id
-        ]:
-            self.sel_trials = self.sel_trials | set(self.ct.pr.sel_event_id[group_item])
+        # The selected trials from the event-id (assume first to allow meta-queries)
+        if len(self.group_list) > 0:
+            self.sel_trials = MEEG(self.group_list[0], self.ct).sel_trials
+        else:
+            self.sel_trials = dict()
 
         # The fsmri where all group members are morphed to
         self.fsmri = FSMRI(self.pa["morph_to"], self.ct)
 
     def init_paths(self):
         # Main Path
         self.save_dir = self.pr.save_dir_averages
@@ -1501,15 +1712,15 @@
             for trial in self.sel_trials
         }
         self.ga_con_paths = {
             trial: {
                 con_method: join(
                     self.save_dir,
                     "connectivity",
-                    f"{self.name}_{trial}_" f"{self.p_preset}_{con_method}.npy",
+                    f"{self.name}_{trial}_" f"{self.p_preset}_{con_method}.nc",
                 )
                 for con_method in self.pa["con_methods"]
             }
             for trial in self.sel_trials
         }
 
         # This dictionary contains entries for each data-type
@@ -1551,23 +1762,23 @@
         """Returns a generator for group items."""
         for obj_name in self.group_list:
             if obj_type == "MEEG":
                 obj = MEEG(obj_name, self.ct)
             elif obj_type == "FSMRI":
                 obj = FSMRI(obj_name, self.ct)
             else:
-                logging.error(f"The object-type {obj_type} is not valid!")
+                logger().error(f"The object-type {obj_type} is not valid!")
                 continue
             if data_type is None:
                 yield obj
             elif data_type in obj.io_dict:
                 data = obj.io_dict[data_type]["load"]()
                 yield data, obj
             else:
-                logging.error(f"{data_type} is not valid for {obj_type}")
+                logger().error(f"{data_type} is not valid for {obj_type}")
 
     @load_decorator
     def load_ga_evokeds(self):
         ga_evokeds = dict()
         for trial in self.sel_trials:
             ga_evokeds[trial] = mne.read_evokeds(self.ga_evokeds_paths[trial])[0]
 
@@ -1623,19 +1834,19 @@
                 np.save(self.ga_ltc_paths[trial][label], ga_ltc[trial][label])
 
     @load_decorator
     def load_ga_con(self):
         ga_connect = dict()
         for trial in self.ga_con_paths:
             ga_connect[trial] = {}
-            for con_method in self.ga_con_paths[trial]:
-                ga_connect[trial][con_method] = np.load(
-                    self.ga_con_paths[trial][con_method]
+            for con_method, con_path in self.ga_con_paths[trial].items():
+                ga_connect[trial][con_method] = mne_connectivity.read_connectivity(
+                    con_path
                 )
 
         return ga_connect
 
     @save_decorator
-    def save_ga_con(self, ga_con):
-        for trial in ga_con:
-            for con_method in ga_con[trial]:
-                np.save(self.ga_con_paths[trial][con_method], ga_con[trial][con_method])
+    def save_ga_con(self, ga_con_dict):
+        for trial in ga_con_dict:
+            for con_method, ga_con in ga_con_dict[trial].items():
+                ga_con.save(self.ga_con_paths[trial][con_method])
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/pipeline_utils.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/pipeline_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,73 @@
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import inspect
 import json
 import logging
+import multiprocessing
 import os
 import sys
 from ast import literal_eval
 from copy import deepcopy
 from datetime import datetime
 from importlib import resources
 from os.path import join, isfile
 from pathlib import Path
 
 import numpy as np
 import psutil
 
+from mne_pipeline_hd import extra
+
 datetime_format = "%d.%m.%Y %H:%M:%S"
 
 ismac = sys.platform.startswith("darwin")
 iswin = sys.platform.startswith("win32")
 islin = not ismac and not iswin
 
+_logger = None
+
+
+def init_logging(debug_mode=False):
+    global _logger
+    # Initialize Logger
+    _logger = logging.getLogger("mne_pipeline_hd")
+    if debug_mode:
+        _logger.setLevel(logging.DEBUG)
+    else:
+        _logger.setLevel(QS().value("log_level", defaultValue=logging.INFO))
+    if debug_mode:
+        fmt = "[%(levelname)s] %(module)s.%(funcName)s(): %(message)s"
+    else:
+        fmt = "[%(levelname)s] %(message)s"
+    formatter = logging.Formatter(fmt)
+    console_handler = logging.StreamHandler()
+    console_handler.set_name("console")
+    console_handler.setFormatter(formatter)
+    _logger.addHandler(console_handler)
+
+
+def logger():
+    global _logger
+    if _logger is None:
+        _logger = logging.getLogger("mne_pipeline_hd")
+    return _logger
+
+
+def get_n_jobs(n_jobs):
+    """Get the number of jobs to use for parallel processing"""
+    if n_jobs == -1 or n_jobs in ["auto", "max"]:
+        n_cores = multiprocessing.cpu_count()
+    else:
+        n_cores = int(n_jobs)
+
+    return n_cores
+
 
 def encode_tuples(input_dict):
     """Encode tuples in a dictionary, because JSON does not recognize them
     (CAVE: input_dict is changed in place)"""
     for key, value in input_dict.items():
         if isinstance(value, dict):
             encode_tuples(value)
@@ -120,40 +161,40 @@
         try:
             previous_value = obj.file_parameters[file_name][param]
             current_value = obj.pa[param]
 
             if str(previous_value) == str(current_value):
                 result_dict[param] = "equal"
                 if verbose:
-                    print(f"{param} equal for {file_name}")
+                    logger().debug(f"{param} equal for {file_name}")
             else:
                 if param in critical_params:
                     result_dict[param] = (previous_value, current_value, True)
                     if verbose:
-                        print(
+                        logger().debug(
                             f"{param} changed from {previous_value} to "
                             f"{current_value} for {file_name} "
                             f"and is probably crucial for {function}"
                         )
                 else:
                     result_dict[param] = (previous_value, current_value, False)
                     if verbose:
-                        print(
+                        logger().debug(
                             f"{param} changed from {previous_value} to "
                             f"{current_value} for {file_name}"
                         )
         except KeyError:
             result_dict[param] = "missing"
             if verbose:
-                print(f"{param} is missing in records for {file_name}")
+                logger().warning(f"{param} is missing in records for {file_name}")
 
     if obj.ct.settings["overwrite"]:
         result_dict[param] = "overwrite"
         if verbose:
-            print(
+            logger().info(
                 f"{file_name} will be overwritten anyway"
                 f" because Overwrite=True (Settings)"
             )
 
     return result_dict
 
 
@@ -193,21 +234,21 @@
     if ismac:
         os.system("sudo shutdown -h now")
 
 
 def restart_program():
     """Restarts the current program, with file objects and descriptors
     cleanup."""
-    logging.info("Restarting")
+    logger().info("Restarting")
     try:
         p = psutil.Process(os.getpid())
         for handler in p.open_files() + p.connections():
             os.close(handler.fd)
     except Exception as e:
-        logging.error(e)
+        logger().error(e)
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
 
 def _get_func_param_kwargs(func, params):
     kwargs = {
@@ -217,73 +258,38 @@
 
     return kwargs
 
 
 class BaseSettings:
     def __init__(self):
         # Load default settings
-        with resources.open_text(
-            "mne_pipeline_hd.resource", "default_settings.json"
-        ) as file:
+        default_settings_path = join(resources.files(extra), "default_settings.json")
+        with open(default_settings_path, "r") as file:
             self.default_qsettings = json.load(file)["qsettings"]
 
     def get_default(self, name):
         if name in self.default_qsettings:
             return self.default_qsettings[name]
         else:
             raise RuntimeError(
                 f"{name} not in default_settings.json! "
                 f"Please add it or fix the bug."
             )
 
 
-class QSettingsDummy(BaseSettings):
-    def __init__(self):
-        super().__init__()
-
-        self.settings_path = join(Path.home(), ".mnephd_settings.json")
-
-    def _load_settings(self):
-        if isfile(self.settings_path):
-            with open(self.settings_path, "r") as file:
-                self.settings = json.load(file)
-        else:
-            self.settings = deepcopy(self.default_qsettings)
-
-    def _write_settings(self):
-        with open(self.settings_path, "w") as file:
-            json.dump(self.settings, file)
-
-    def value(self, setting, defaultValue=None):
-        self._load_settings()
-        if setting in self.settings:
-            return self.settings[setting]
-
-        if defaultValue is None:
-            return self.get_default(setting)
-        else:
-            return defaultValue
-
-    def setValue(self, setting, value):
-        self._load_settings()
-        self.settings[setting] = value
-        self._write_settings()
-
-
 # Import QSettings or provide Dummy-Class to be independent from PyQt/PySide
 try:
-    from PyQt5.QtCore import QSettings
+    from qtpy.QtCore import QSettings
 
-    class ModQSettings(QSettings, BaseSettings):
+    class QS(BaseSettings):
         def __init__(self):
-            super(QSettings, self).__init__()
-            super(BaseSettings, self).__init__()
+            super().__init__()
 
         def value(self, setting, defaultValue=None):
-            loaded_value = super().value(setting, defaultValue=defaultValue)
+            loaded_value = QSettings().value(setting, defaultValue=defaultValue)
             # Type-Conversion for UNIX-Systems
             # (ini-File does not preserve type, converts to strings)
             if not isinstance(loaded_value, type(self.get_default(setting))):
                 try:
                     loaded_value = literal_eval(loaded_value)
                 except (SyntaxError, ValueError):
                     return self.get_default(setting)
@@ -291,24 +297,73 @@
                 if defaultValue is None:
                     return self.get_default(setting)
                 else:
                     return defaultValue
             else:
                 return loaded_value
 
-    class QS(ModQSettings):
-        def __init__(self):
-            super().__init__()
+        def setValue(self, setting, value):
+            QSettings().setValue(setting, value)
+
+        def sync(self):
+            QSettings().sync()
+
+        def childKeys(self):
+            return QSettings().childKeys()
+
+        def remove(self, setting):
+            QSettings().remove(setting)
 
 except ImportError:
 
-    class QS(QSettingsDummy):
+    class QS(BaseSettings):
         def __init__(self):
             super().__init__()
 
+            self.settings_path = join(Path.home(), ".mnephd_settings.json")
+
+        def _load_settings(self):
+            if isfile(self.settings_path):
+                with open(self.settings_path, "r") as file:
+                    self.settings = json.load(file)
+            else:
+                self.settings = deepcopy(self.default_qsettings)
+
+        def _write_settings(self):
+            with open(self.settings_path, "w") as file:
+                json.dump(self.settings, file)
+
+        def value(self, setting, defaultValue=None):
+            self._load_settings()
+            if setting in self.settings:
+                return self.settings[setting]
+
+            if defaultValue is None:
+                return self.get_default(setting)
+            else:
+                return defaultValue
+
+        def setValue(self, setting, value):
+            self._load_settings()
+            self.settings[setting] = value
+            self._write_settings()
+
+        def sync(self):
+            self._write_settings()
+            self._load_settings()
+
+        def childKeys(self):
+            self._load_settings()
+            return self.settings.keys()
+
+        def remove(self, setting):
+            self._load_settings()
+            self._settings.pop(setting)
+            self._write_settings()
+
 
 def _set_test_run():
     os.environ["TEST_RUN"] = "True"
 
 
 def _test_run():
     if "TEST_RUN" in os.environ:
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/plot_utils.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/pipeline/project.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/pipeline/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 import json
-import logging
 import os
 import shutil
 from ast import literal_eval
 from copy import deepcopy
 from os import listdir, makedirs
 from os.path import exists, getsize, isfile, join, isdir
 from pathlib import Path
@@ -21,14 +20,15 @@
 from mne_pipeline_hd.pipeline.legacy import renamed_parameters
 from mne_pipeline_hd.pipeline.loading import MEEG, FSMRI, Group
 from mne_pipeline_hd.pipeline.pipeline_utils import (
     TypedJSONEncoder,
     count_dict_keys,
     encode_tuples,
     type_json_hook,
+    logger,
 )
 
 
 class Project:
     """
     A class with attributes for all the paths, file-lists/dicts
     and parameters of the selected project
@@ -68,15 +68,15 @@
             self.figures_path,
         ]
 
         # Create or check existence of main_paths
         for path in self.main_paths:
             if not exists(path):
                 makedirs(path)
-                logging.debug(f"{path} created")
+                logger().debug(f"{path} created")
 
     def init_attributes(self):
         # Stores the names of all MEG/EEG-Files
         self.all_meeg = list()
         # Stores selected MEG/EEG-Files
         self.sel_meeg = list()
         # Stores Bad-Channels for each MEG/EEG-File
@@ -93,15 +93,15 @@
         # in Subjects-Dir
         self.all_fsmri = list()
         # Stores selected Freesurfer-Segmentations
         self.sel_fsmri = list()
         # Maps each MEG/EEG-File to a Freesurfer-Segmentation or None
         self.meeg_to_fsmri = dict()
         # Stores the ICA-Components to be excluded
-        self.ica_exclude = dict()
+        self.meeg_ica_exclude = dict()
         # Groups MEG/EEG-Files e.g. for Grand-Average
         self.all_groups = dict()
         # Stores selected Grand-Average-Groups
         self.sel_groups = list()
         # Stores paths of saved plots
         self.plot_files = dict()
         # Stores functions and if they are selected
@@ -167,24 +167,41 @@
             self.meeg_event_id_path: "meeg_event_id",
             self.sel_event_id_path: "sel_event_id",
             self.all_erm_path: "all_erm",
             self.meeg_to_erm_path: "meeg_to_erm",
             self.all_fsmri_path: "all_fsmri",
             self.sel_fsmri_path: "sel_fsmri",
             self.meeg_to_fsmri_path: "meeg_to_fsmri",
-            self.ica_exclude_path: "ica_exclude",
+            self.ica_exclude_path: "meeg_ica_exclude",
             self.all_groups_path: "all_groups",
             self.sel_groups_path: "sel_groups",
             self.plot_files_path: "plot_files",
             self.sel_functions_path: "sel_functions",
             self.add_kwargs_path: "add_kwargs",
             self.parameters_path: "parameters",
             self.sel_p_preset_path: "p_preset",
         }
 
+    def rename(self, new_name):
+        # Rename folder
+        old_name = self.name
+        os.rename(self.project_path, join(self.ct.projects_path, new_name))
+        self.name = new_name
+        self.init_main_paths()
+        # Rename project-files
+        old_paths = [Path(p).name for p in self.path_to_attribute]
+        self.init_pipeline_scripts()
+        new_paths = [Path(p).name for p in self.path_to_attribute]
+        for old_path, new_path in zip(old_paths, new_paths):
+            os.rename(
+                join(self.pscripts_path, old_path), join(self.pscripts_path, new_path)
+            )
+            logger().info(f"Renamed project-script {old_path} to {new_path}")
+        logger().info(f'Finished renaming project "{old_name}" to "{new_name}"')
+
     def load_lists(self):
         # Old Paths to allow transition (22.11.2020)
         self.old_all_meeg_path = join(self.pscripts_path, "file_list.json")
         self.old_sel_meeg_path = join(self.pscripts_path, "selected_files.json")
         self.old_meeg_bad_channels_path = join(
             self.pscripts_path, "bad_channels_dict.json"
         )
@@ -262,15 +279,15 @@
                         p
                         for p in loaded_parameters[p_preset]
                         if p not in self.ct.pd_params.index
                     ]:
                         if "_exp" not in param:
                             loaded_parameters[p_preset].pop(param)
 
-                    # Add parameters, which exist in resource/parameters.csv,
+                    # Add parameters, which exist in extra/parameters.csv,
                     # but not in loaded-parameters
                     # (e.g. added with custom-module)
                     for param in [
                         p
                         for p in self.ct.pd_params.index
                         if p not in loaded_parameters[p_preset]
                     ]:
@@ -360,15 +377,15 @@
                 encode_tuples(attribute)
 
             try:
                 with open(path, "w") as file:
                     json.dump(attribute, file, cls=TypedJSONEncoder, indent=4)
 
             except json.JSONDecodeError as err:
-                print(f"There is a problem with path:\n" f"{err}")
+                logger().warning(f"There is a problem with path:\n" f"{err}")
 
     def add_meeg(self, name, file_path=None, is_erm=False):
         if is_erm:
             # Organize Empty-Room-FIles
             self.all_erm.append(name)
         else:
             # Organize other files
@@ -391,58 +408,58 @@
 
     def remove_meeg(self, remove_files):
         for meeg in self.sel_meeg:
             try:
                 # Remove MEEG from Lists/Dictionaries
                 self.all_meeg.remove(meeg)
             except ValueError:
-                logging.warning(f"{meeg} already removed!")
+                logger().warning(f"{meeg} already removed!")
             self.meeg_to_erm.pop(meeg, None)
             self.meeg_to_fsmri.pop(meeg, None)
             self.meeg_bad_channels.pop(meeg, None)
             self.meeg_event_id.pop(meeg, None)
             if remove_files:
                 try:
                     remove_path = join(self.data_path, meeg)
                     shutil.rmtree(remove_path)
-                    print(f"Succesful removed {remove_path}")
+                    logger().info(f"Succesful removed {remove_path}")
                 except FileNotFoundError:
-                    print(join(self.data_path, meeg) + " not found!")
+                    logger().critical(join(self.data_path, meeg) + " not found!")
         self.sel_meeg.clear()
 
     def add_fsmri(self, name, src_dir=None):
         self.all_fsmri.append(name)
         # Initialize FSMRI
         fsmri = FSMRI(name, self.ct)
         if src_dir is not None:
             dst_dir = join(self.ct.subjects_dir, name)
             if not isdir(dst_dir):
-                print(f"Copying Folder from {src_dir}...")
+                logger().debug(f"Copying Folder from {src_dir}...")
                 try:
                     shutil.copytree(src_dir, dst_dir)
                 # surfaces with .H and .K at the end can't be copied
                 except shutil.Error:
                     pass
-                print(f"Finished Copying to {dst_dir}")
+                logger().debug(f"Finished Copying to {dst_dir}")
             else:
-                print(f"{dst_dir} already exists")
+                logger().info(f"{dst_dir} already exists")
 
         return fsmri
 
     def remove_fsmri(self, remove_files):
         for fsmri in self.sel_fsmri:
             try:
                 self.all_fsmri.remove(fsmri)
             except ValueError:
-                logging.warning(f"{fsmri} already deleted!")
+                logger().warning(f"{fsmri} already deleted!")
             if remove_files:
                 try:
                     shutil.rmtree(join(self.ct.subjects_dir, fsmri))
                 except FileNotFoundError:
-                    print(join(self.ct.subjects_dir, fsmri) + " not found!")
+                    logger().info(join(self.ct.subjects_dir, fsmri) + " not found!")
         self.sel_fsmri.clear()
 
     def add_group(self):
         pass
 
     def remove_group(self):
         pass
@@ -484,37 +501,37 @@
             meeg = MEEG(meeg, self.ct)
             worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {meeg}")
             meeg.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print("Cleaning was canceled by the user!")
+                    logger().info("Cleaning was canceled by the user!")
                     return
 
         for fsmri in self.all_fsmri:
             fsmri = FSMRI(fsmri, self.ct)
             worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {fsmri}")
             fsmri.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print("Cleaning was canceled by the user!")
+                    logger().info("Cleaning was canceled by the user!")
                     return
 
         for group in self.all_groups:
             group = Group(group, self.ct)
             worker_signals.pgbar_text.emit(f"Cleaning File-Parameters for {group}")
             group.clean_file_parameters()
             count += 1
             if worker_signals is not None:
                 worker_signals.pgbar_n.emit(count)
                 if worker_signals.was_canceled:
-                    print("Cleaning was canceled by the user!")
+                    logger().info("Cleaning was canceled by the user!")
                     return
 
     def clean_plot_files(self, worker_signals=None):
         all_image_paths = list()
         # Remove object-keys which no longer exist
         remove_obj = list()
         n_remove_ppreset = 0
@@ -557,15 +574,15 @@
                                 worker_signals.pgbar_n.emit(key_count)
 
                             # Cancel if canceled
                             if (
                                 worker_signals is not None
                                 and worker_signals.was_canceled
                             ):
-                                print("Cleaning was canceled by user")
+                                logger().info("Cleaning was canceled by user")
                                 return
 
                             if func not in self.ct.pd_funcs.index:
                                 remove_funcs.append(func)
                             else:
                                 # Remove image-paths which no longer exist
                                 for rel_image_path in self.plot_files[obj_key][
@@ -592,47 +609,47 @@
                             self.plot_files[obj_key][p_preset].pop(remove_func_key)
                         n_remove_funcs += len(remove_funcs)
 
                 for remove_preset_key in remove_p_preset:
                     self.plot_files[obj_key].pop(remove_preset_key)
                 n_remove_ppreset += len(remove_p_preset)
 
-            print(
+            logger().info(
                 f"Removed {n_remove_ppreset} Parameter-Presets and "
                 f"{n_remove_funcs} from {obj_key}"
             )
 
         for remove_key in remove_obj:
             self.plot_files.pop(remove_key)
-        print(f"Removed {len(remove_obj)} Objects from Plot-Files")
+        logger().info(f"Removed {len(remove_obj)} Objects from Plot-Files")
 
         # Remove image-files, which aren't listed in plot_files.
         free_space = 0
-        print("Removing unregistered images...")
+        logger().info("Removing unregistered images...")
         n_removed_images = 0
         for root, _, files in os.walk(self.figures_path):
             files = [join(root, f) for f in files]
             for file_path in [
                 fp for fp in files if str(Path(fp)) not in all_image_paths
             ]:
                 free_space += getsize(file_path)
                 n_removed_images += 1
                 os.remove(file_path)
-        print(f"Removed {n_removed_images} images")
+        logger().info(f"Removed {n_removed_images} images")
 
         # Remove empty folders (loop until all empty folders are removed)
-        print("Removing empty folders...")
+        logger().info("Removing empty folders...")
         n_removed_folders = 0
         folder_loop = True
         # Redo the file-walk because folders can get empty
         # by deleting folders inside
         while folder_loop:
             folder_loop = False
             for root, folders, _ in os.walk(self.figures_path):
                 folders = [join(root, fd) for fd in folders]
                 for folder in [fdp for fdp in folders if len(listdir(fdp)) == 0]:
                     os.rmdir(folder)
                     n_removed_folders += 1
                     folder_loop = True
-        print(f"Removed {n_removed_folders} folders")
+        logger().info(f"Removed {n_removed_folders} folders")
 
-        print(f"{round(free_space / (1024 ** 2), 2)} MB of space was freed!")
+        logger().info(f"{round(free_space / (1024 ** 2), 2)} MB of space was freed!")
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/default_settings.json` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/default_settings.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 1.0%*

 * *Differences: {}*

```diff
@@ -2,15 +2,15 @@
     "qsettings": {
         "app_font": "AnyStyle",
         "app_font_size": 10,
         "app_style": "auto",
         "education": 0,
         "enable_cuda": 0,
         "fs_path": "",
-        "gui": true,
+        "gui": 1,
         "home_path": "",
         "log_level": 20,
         "mne_path": "",
         "n_jobs": -1,
         "n_parallel": 1,
         "save_ram": 1,
         "use_qthread": 1
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/functions.csv` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/functions.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 ;alias;target;tab;group;matplotlib;mayavi;dependencies;module;pkg_name;func_args
+find_bads;Find Bad Channels;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,n_jobs
 filter_data;Filter;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,filter_target,highpass,lowpass,filter_length,l_trans_bandwidth,h_trans_bandwidth,filter_method,iir_params,fir_phase,fir_window,fir_design,skip_by_annotation,fir_pad,n_jobs,enable_cuda,erm_t_limit,bad_interpolation
+notch_filter;Notch Filter;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,notch_frequencies,n_jobs
+interpolate_bads;Interpolate Bads;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,bad_interpolation
 add_erm_ssp;Empty-Room SSP;MEEG;Compute;Preprocessing;True;False;;operations;basic;meeg,erm_ssp_duration,erm_n_grad,erm_n_mag,erm_n_eeg,n_jobs,show_plots
 eeg_reference_raw;Set EEG Reference;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,ref_channels
 find_events;Find events;MEEG;Compute;events;False;False;;operations;basic;meeg,stim_channels,min_duration,shortest_event,adjust_timeline_by_msec
 find_6ch_binary_events;Find events HD;MEEG;Compute;events;False;False;;operations;basic;meeg,min_duration,shortest_event,adjust_timeline_by_msec
 epoch_raw;Get Epochs;MEEG;Compute;events;False;False;;operations;basic;meeg,ch_types,ch_names,t_epoch,baseline,apply_proj,reject,flat,reject_by_annotation,bad_interpolation,use_autoreject,consensus_percs,n_interpolates,overwrite_ar,decim,n_jobs
 estimate_noise_covariance;Noise-Covariance;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,baseline,n_jobs,noise_cov_mode,noise_cov_method
-run_ica;Run ICA;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,ica_method,ica_fitto,n_components,ica_noise_cov,ica_remove_proj,ica_reject,ica_autoreject,ch_types,ch_names,reject_by_annotation,ica_eog,eog_channel,ica_ecg,ecg_channel
-apply_ica;Apply ICA;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,n_pca_components
+run_ica;Run ICA;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,ica_method,ica_fitto,n_components,ica_noise_cov,ica_remove_proj,ica_reject,ica_autoreject,overwrite_ar,ch_types,ch_names,reject_by_annotation,ica_eog,eog_channel,ica_ecg,ecg_channel
+apply_ica;Apply ICA;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,ica_apply_target,n_pca_components
 get_evokeds;Get Evokeds;MEEG;Compute;events;False;False;;operations;basic;meeg
-interpolate_bads;Interpolate Bads;MEEG;Compute;Preprocessing;False;False;;operations;basic;meeg,bad_interpolation
+compute_psd_raw;Compute PSD (Raw);MEEG;Compute;Time-Frequency;False;False;;operations;basic;meeg,psd_method,n_jobs
+compute_psd_epochs;Compute PSD (Epochs);MEEG;Compute;Time-Frequency;False;False;;operations;basic;meeg,psd_method,n_jobs
 tfr;Time-Frequency;MEEG;Compute;Time-Frequency;False;False;;operations;basic;meeg,tfr_freqs,tfr_n_cycles,tfr_average,tfr_use_fft,tfr_baseline,tfr_baseline_mode,tfr_method,multitaper_bandwidth,stockwell_width,n_jobs
 apply_watershed;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri
 prepare_bem;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri,bem_spacing,bem_conductivity
 setup_src;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri,src_spacing,surface,n_jobs
 compute_src_distances;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri,n_jobs
 make_dense_scalp_surfaces;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri
 setup_vol_src;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri,vol_src_spacing
+create_forward_solution;;MEEG;Compute;Forward;False;False;;operations;basic;meeg,n_jobs,ch_types
 morph_fsmri;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,morph_to
 morph_labels_from_fsaverage;;FSMRI;Compute;MRI-Preprocessing;False;False;;operations;basic;fsmri
-create_forward_solution;;MEEG;Compute;Forward;False;False;;operations;basic;meeg,n_jobs,ch_types
 create_inverse_operator;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg
 source_estimate;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,inverse_method,pick_ori,lambda2
 apply_morph;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,morph_to
 label_time_course;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,target_labels,extract_mode
 ecd_fit;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,ecd_times,ecd_positions,ecd_orientations,t_epoch
-src_connectivity;;MEEG;Compute;Inverse;False;False;;operations;basic;meeg,target_labels,inverse_method,lambda2,con_methods,con_fmin,con_fmax,n_jobs
+src_connectivity;;MEEG;Compute;Time-Frequency;False;False;;operations;basic;meeg,target_labels,inverse_method,lambda2,con_methods,con_fmin,con_fmax,con_time_window,n_jobs
 grand_avg_evokeds;;Group;Compute;Grand-Average;False;False;;operations;basic;group,ga_interpolate_bads,ga_drop_bads
 grand_avg_tfr;;Group;Compute;Grand-Average;False;False;;operations;basic;group
 grand_avg_morphed;;Group;Compute;Grand-Average;False;False;;operations;basic;group,morph_to
 grand_avg_ltc;;Group;Compute;Grand-Average;False;False;;operations;basic;group
 grand_avg_connect;;Group;Compute;Grand-Average;False;False;;operations;basic;group
-plot_src;;FSMRI;Plot;MRI-Preprocessing;True;True;;plot;basic;fsmri
+plot_src;;FSMRI;Plot;MRI-Preprocessing;True;True;;plot;basic;fsmri,backend_3d
 plot_bem;;FSMRI;Plot;MRI-Preprocessing;True;False;;plot;basic;fsmri,show_plots
 plot_noise_covariance;;MEEG;Plot;Inverse;True;False;;plot;basic;meeg,show_plots
-plot_transformation;;MEEG;Plot;Forward;True;True;;plot;basic;meeg
+plot_transformation;;MEEG;Plot;Forward;True;True;;plot;basic;meeg,backend_3d
 plot_sensitivity_maps;;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,ch_types
 plot_sensors;;MEEG;Plot;Forward;True;False;;plot;basic;meeg,plot_sensors_kind,ch_types,show_plots
-plot_raw;;MEEG;Plot;Raw;True;False;;plot;basic;meeg,show_plots
-plot_filtered;;MEEG;Plot;Raw;True;False;;plot;basic;meeg,show_plots
+plot_raw;;MEEG;Plot;Raw;True;False;;plot;basic;meeg,show_plots,close_func
+plot_filtered;;MEEG;Plot;Raw;True;False;;plot;basic;meeg,show_plots,close_func
 plot_events;;MEEG;Plot;events;True;False;;plot;basic;meeg,show_plots
-plot_power_spectra;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots,n_jobs
-plot_power_spectra_topo;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots,n_jobs
-plot_power_spectra_epochs;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots,n_jobs
-plot_power_spectra_epochs_topo;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots,n_jobs
+plot_power_spectra;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots
+plot_power_spectra_topomap;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,psd_topomap_bands,show_plots
+plot_power_spectra_epochs;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots
+plot_power_spectra_epochs_topomap;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,psd_topomap_bands,show_plots
 plot_tfr;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,show_plots
 plot_epochs;;MEEG;Plot;Epochs;True;False;;plot;basic;meeg,show_plots
 plot_epochs_image;;MEEG;Plot;Epochs;True;False;;plot;basic;meeg,show_plots
 plot_epochs_topo;;MEEG;Plot;Epochs;True;False;;plot;basic;meeg,show_plots
 plot_epochs_drop_log;;MEEG;Plot;Epochs;True;False;;plot;basic;meeg,show_plots
 plot_autoreject_log;;MEEG;Plot;Epochs;True;False;;plot;basic;meeg,show_plots
 plot_evoked_topo;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_evoked_topomap;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_evoked_butterfly;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,apply_proj,show_plots
 plot_evoked_joint;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_evoked_white;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_evoked_image;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_compare_evokeds;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
 plot_gfp;;MEEG;Plot;Evoked;True;False;;plot;basic;meeg,show_plots
-plot_stc;Plot Source-Estimate;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
-plot_stc_interactive;;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
-plot_labels;;FSMRI;Plot;Inverse;True;True;;plot;basic;fsmri,target_labels,label_colors,stc_hemi,stc_surface,stc_views
-plot_animated_stc;Plot Source-Estimate Video;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation,stc_animation_span,stc_animation_dilat
+plot_stc;Plot Source-Estimate;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,backend_3d
+plot_stc_interactive;;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,backend_3d
+plot_labels;;FSMRI;Plot;Inverse;True;True;;plot;basic;fsmri,target_labels,label_colors,stc_hemi,stc_surface,stc_views,backend_3d
+plot_animated_stc;Plot Source-Estimate Video;MEEG;Plot;Inverse;True;True;;plot;basic;meeg,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,stc_animation_span,stc_animation_dilat,backend_3d
 plot_snr;;MEEG;Plot;Inverse;True;False;;plot;basic;meeg,show_plots
-plot_label_time_course;;MEEG;Plot;Inverse;True;False;;plot;basic;meeg,show_plots
+plot_label_time_course;;MEEG;Plot;Inverse;True;False;;plot;basic;meeg,label_colors,show_plots
 plot_ecd;;MEEG;Plot;Inverse;True;True;;plot;basic;meeg
-plot_src_connectivity;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,target_labels,con_fmin,con_fmax,show_plots
+plot_src_connectivity;;MEEG;Plot;Time-Frequency;True;False;;plot;basic;meeg,label_colors,show_plots
 plot_grand_avg_evokeds;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
 plot_grand_avg_tfr;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
-plot_grand_avg_stc;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
-plot_grand_avg_stc_anim;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation,stc_animation_span,stc_animation_dilat
-plot_grand_average_stc_interactive;;Group;Plot;Grand-Average;True;True;;plot;basic;group,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_background,stc_roll,stc_azimuth,stc_elevation
-plot_grand_avg_ltc;;Group;Plot;Grand-Average;True;False;;plot;basic;group,show_plots
-plot_grand_avg_connect;;Group;Plot;Grand-Average;True;False;;plot;basic;group,con_fmin,con_fmax,target_labels,morph_to,show_plots,connectivity_vmin,connectivity_vmax
-plot_ica_components;Plot ICA-Components;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
-plot_ica_sources;Plot ICA-Sources;MEEG;Plot;ICA;True;False;;operations;basic;meeg,ica_source_data,show_plots
-plot_ica_overlay;Plot ICA-Overlay;MEEG;Plot;ICA;True;False;;operations;basic;meeg,ica_overlay_data,show_plots
-plot_ica_properties;Plot ICA-Properties;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
-plot_ica_scores;Plot ICA-Scores;MEEG;Plot;ICA;True;False;;operations;basic;meeg,show_plots
+plot_grand_avg_stc;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,backend_3d
+plot_grand_avg_stc_anim;;Group;Plot;Grand-Average;True;True;;plot;basic;group,target_labels,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,stc_animation_span,stc_animation_dilat,backend_3d
+plot_grand_average_stc_interactive;;Group;Plot;Grand-Average;True;True;;plot;basic;group,label_colors,stc_surface,stc_hemi,stc_views,stc_time,stc_clim,stc_roll,stc_azimuth,stc_elevation,backend_3d
+plot_grand_avg_ltc;;Group;Plot;Grand-Average;True;False;;plot;basic;group,label_colors,show_plots
+plot_grand_avg_connect;;Group;Plot;Grand-Average;True;False;;plot;basic;group,label_colors,show_plots
+plot_ica_components;Plot ICA-Components;MEEG;Plot;ICA;True;False;;plot;basic;meeg,show_plots,close_func
+plot_ica_sources;Plot ICA-Sources;MEEG;Plot;ICA;True;False;;plot;basic;meeg,ica_source_data,show_plots,close_func
+plot_ica_overlay;Plot ICA-Overlay;MEEG;Plot;ICA;True;False;;plot;basic;meeg,ica_overlay_data,show_plots
+plot_ica_properties;Plot ICA-Properties;MEEG;Plot;ICA;True;False;;plot;basic;meeg,ica_fitto,show_plots
+plot_ica_scores;Plot ICA-Scores;MEEG;Plot;ICA;True;False;;plot;basic;meeg,show_plots
 print_info;Print Info;MEEG;Plot;Raw;False;False;;operations;basic;meeg
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/license.txt` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/license.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_license.txt` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_license.txt`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_dark.png` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_icon_dark.png`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_icon_light.png` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_icon_light.png`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/mne_pipeline_logo_evee_smaller.jpg`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/resource/parameters.csv` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/extra/parameters.csv`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 n_interpolates;;epochs;np.array([1, 4, 32]);;p-values for autoreject;FuncGui;
 consensus_percs;;epochs;np.linspace(0, 1.0, 11);;k-values for autoreject;FuncGui;
 overwrite_ar;Overwrite Autoreject(Threshold);epochs;False;;if to calculate new threshold or use the previously calculated;BoolGui;
 reject;;epochs;{'mag':3000e-15, 'grad':3000e-13, 'eeg':100e-6, 'eog':200e-6};;Chose reject-thresholds if not reject with autoreject_threshold;DictGui;{'none_select': True}
 flat;;epochs;{'mag': 1e-15, 'grad':1e-13, 'eeg': 1e-6};;Chose flat-thresholds;DictGui;{'none_select': True}
 decim;;epochs;1;;Downsampling-Factor for epochs;IntGui;
 ica_method;ICA-Method;ICA;fastica;;The method for calculating ICA;ComboGui;{'options': ['fastica', 'infomax', 'picard']}
-ica_fitto;Fit ICA to:;ICA;'raw_filtered';;The data to fit the ICA to;ComboGui;{'options': ['raw', 'raw_filtered', 'epochs']}
+ica_fitto;Fit ICA to:;ICA;'raw_filtered';;The data to fit the ICA to;ComboGui;{'options': {'raw': 'Raw (unfiltered)', 'raw_filtered': 'Raw (filtered)', 'epochs': 'Epochs'}}
+ica_apply_target;Apply ICA to:;ICA;raw_filtered;;The target object (Raw, Epochs or Evoked) to apply ICA and remove the selected components from;ComboGui;{'options': {'raw_filtered': 'Raw (filtered)', 'epochs': 'Epochs', 'evoked': 'Evoked'}}
 n_components;;ICA;25;;The number of components for ICA;IntGui;
 max_pca_components;;ICA;None;;;IntGui;{'none_select': True}
 n_pca_components;;ICA;None;;;IntGui;{'none_select': True}
 ica_noise_cov;Use Noise-Covariance;ICA;False;;If to use a noise-covariance for pre-whitening;BoolGui;
 ica_remove_proj;Remove projections;ICA;False;;If to remove projections from the data before fitting;BoolGui;
 ica_reject;Reject-Parameters;ICA;{'mag':3000e-15, 'grad':3000e-13, 'eeg':100e-6, 'eog':200e-6};;Reject-Parameters for ICA;DictGui;{'none_select': True}
 ica_autoreject;Autoreject;ICA;False;;If to use Autoreject for ICA;BoolGui;
@@ -67,32 +68,36 @@
 stc_surface;;Inverse;inflated;;Select the surface type for Source Estimate Plots;ComboGui;{'options':['inflated', 'white', 'pial']}
 stc_hemi;;Inverse;'split';;Select the hemispheres for Source Estimate Plots;ComboGui;{'options':['lh', 'rh', 'both', 'split']}
 stc_views;;Inverse;['med', 'lat'];;Select the views for Source Estimate Plots;MultiTypeGui;{'type_selection': True, 'types': ['str', 'list']}
 stc_time;;Inverse;0;;Initial time for Source Estimate Plots;FloatGui;
 stc_clim;;Inverse;'auto';;Colorbar Limits for Source Estimate Plots;MultiTypeGui;{'type_selection': True, 'types': ['str', 'dict']}
 stc_background;;Inverse;'black';;Background for Source Estimate Plots;MultiTypeGui;{'type_selection': False}
 stc_roll;;Inverse;0;;Roll for view in for Source Estimate Plots;IntGui;{'max_val': 360}
-stc_azimuth;;Inverse;0;;Azimuth for view for Source Estimate Plots;IntGui;{'max_val': 360}
-stc_elevation;;Inverse;0;;Elevation for view for Source Estimate Plots;IntGui;{'max_val': 360}
+stc_azimuth;;Inverse;70;;Azimuth for view for Source Estimate Plots;IntGui;{'max_val': 360}
+stc_elevation;;Inverse;60;;Elevation for view for Source Estimate Plots;IntGui;{'max_val': 360}
 stc_animation_span;;Inverse;(0,0.5);s;time-span for stc-animation[s];TupleGui;
 stc_animation_dilat;;Inverse;20;;time-dilation for stc-animation;IntGui;
-target_labels;;Inverse;[];;;LabelGui;
+target_labels;Target Labels;Inverse;[];;;LabelGui;
 label_colors;;Inverse;{};;Set custom colors for labels.;ColorGui;{'keys': 'target_labels', 'none_select':True}
-extract_mode;Label-Extraction-Mode;Inverse;mean_flip;;mode for extracting label-time-course from Source-Estimate;ComboGui;{'options': ['max', 'mean', 'mean_flip', 'pca_flip']}
-con_methods;;Connectivity;['coh'];;methods for connectivity plots;CheckListGui;{'options': ['coh', 'cohy', 'imcoh', 'plv', 'ciplv', 'ppc', 'pli', 'pli2_unbiased', 'wpli', 'wpli2_debiased']}
-con_fmin;;Connectivity;30;;fmin for connectivity plot;IntGui;
-con_fmax;;Connectivity;80;;fmax for connectivity plot;IntGui;
+extract_mode;Label-Extraction-Mode;Inverse;auto;;mode for extracting label-time-course from Source-Estimate;ComboGui;{'options': ['auto', 'max', 'mean', 'mean_flip', 'pca_flip']}
+con_methods;;Connectivity;['coh'];;methods for connectivity;CheckListGui;{'options': ['coh', 'cohy', 'imcoh', 'plv', 'ciplv', 'ppc', 'pli', 'pli2_unbiased', 'wpli', 'wpli2_debiased']}
+con_fmin;;Connectivity;30;;lower frequency/frequencies for connectivity;MultiTypeGui;{'type_selection': True, 'types': ['float', 'list']}
+con_fmax;;Connectivity;80;;upper frequency/frequencies for connectivity;MultiTypeGui;{'type_selection': True, 'types': ['float', 'list']}
+con_time_window;;Connectivity;(0, 0.5);;time-window for connectivity;TupleGui;{'none_select': True, 'step': 0.001}
 ecd_times;;Inverse;{};;;DictGui;
 ecd_positions;;Inverse;{};;;DictGui;
 ecd_orientations;;Inverse;{};;;DictGui;
 morph_to;;Grand-Average;fsaverage;;name of the freesurfer subject to be morphed to;StringGui;
-ica_source_data;;ICA;raw_filtered;;Which data to plot in sources-plot from ICA;ComboGui;{'options':['raw', 'raw_filtered', 'epochs', 'epochs_eog', 'epochs_ecg',  'evoked', 'evoked (EOG)', 'evoked (ECG)']}
-ica_overlay_data;;ICA;Evokeds;;Which data to plot in overlay-plot from ICA;ComboGui;{'options':['raw', 'raw_filtered', 'evoked', 'evoked (EOG)', 'evoked (ECG)']}
-plot_sensors_kind;;Plot;'topomap';;The kind of plot for plot_sensors;ComboGui;{'options':['topomap', '3d', 'select']}
+ica_source_data;;ICA;raw_filtered;;Which data to plot in sources-plot from ICA;ComboGui;{'options': {'raw': 'Raw (unfiltered)', 'raw_filtered': 'Raw (filtered)', 'epochs': 'Epochs', 'epochs_eog': 'Epochs (EOG)', 'epochs_ecg': 'Epochs (ECG)', 'evoked': 'Evoked', 'evoked_eog': 'Evoked (EOG)', 'evoked_ecg': 'Evoked (ECG)'}}
+ica_overlay_data;;ICA;evoked;;Which data to plot in overlay-plot from ICA;ComboGui;{'options': {'raw': 'Raw (unfiltered)', 'raw_filtered': 'Raw (filtered)', 'evoked': 'Evoked', 'evoked_eog': 'Evoked (EOG)', 'evoked_ecg': 'Evoked (ECG)'}}
+plot_sensors_kind;;Plot;'topomap';;The kind of plot for plot_sensors;ComboGui;{'options': ['topomap', '3d', 'select']}
 erm_ssp_duration;;Preprocessing;1;s;The time-chunk to use for ssp;IntGui;
 erm_n_grad;;Preprocessing;2;;The number of projections for Gradiometer;IntGui;
 erm_n_mag;;Preprocessing;2;;The number of projections for Magnetometer;IntGui;
 erm_n_eeg;;Preprocessing;0;;The number of projections for EEG;IntGui;
 ga_interpolate_bads;;Grand-Average;True;;If to interpolate bad channels for the Grand-Average;BoolGui;
 ga_drop_bads;;Grand-Average;True;;If to drop bad channels for the Grand-Average;BoolGui;
-connectivity_vmin;;Connectivity;None;;Minimum value for colormap;FloatGui;{'step': 0.01, 'none_select':True}
-connectivity_vmax;;Connectivity;None;;Maximum value for colormap;FloatGui;{'step': 0.01, 'none_select':True}
+psd_method;;Time-Frequency;welch;;The method for spectral estimation;ComboGui;{'options': ['welch', 'multitaper']}
+psd_topomap_bands;;Time-Frequency;None;;The frequency bands for the topomap-plot;DictGui;{'none_select': True}
+backend_3d;3D-Backend;Plot;pyvistaqt;;Choose the 3D-Backend for Brain-plots.;ComboGui;{'options': ['pyvistaqt', 'notebook']}
+con_group_boundaries;;Connectivity;None;;Set group-boundaries for circular plot.;FuncGui;{'none_select': True}
+notch_frequencies;;Preprocessing;50;;Set frequencies for Notch filtering;FuncGui;""
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_app.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_concurrent.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_concurrent.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 
 # def test_blocking_worker_dialog(qtbot):
 #     def _test_func():
 #         time.sleep(2)
-#         print('Finished Test-Func')
+#         logger().info('Finished Test-Func')
 #
 #     time1 = time.time()
 #     dlg = WorkerDialog(None, _test_func, blocking=True)
 #     qtbot.addWidget(dlg)
 #     time2 = time.time()
 #
-#     print(f'Worker-Dialog took {round(time2 - time1, 2)} s')
+#     logger().info(f'Worker-Dialog took {round(time2 - time1, 2)} s')
 #     assert time2 - time1 >= 2
 
 # def test_qprocess_worker(qtbot):
 #     commands = ['conda', 'quatsch']
 #     pw = QProcessWorker(commands, printtostd=False)
 #     output = list()
 #     errors = list()
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_controller.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_functions.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd/tests/test_param_guis.py` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd/tests/test_parameter_widgets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,22 @@
 # -*- coding: utf-8 -*-
 """
 Authors: Martin Schulz <dev@mgschulz.de>
 License: BSD 3-Clause
 Github: https://github.com/marsipu/mne-pipeline-hd
 """
 import inspect
-import sys
-from ast import literal_eval
 
 import pytest
-from PyQt5.QtWidgets import (
-    QVBoxLayout,
-    QGridLayout,
-    QPushButton,
-    QLineEdit,
-    QDialog,
-    QApplication,
-    QWidget,
-    QHBoxLayout,
-    QComboBox,
-)
+from qtpy.QtCore import Qt
 from numpy.testing import assert_allclose
 
 from mne_pipeline_hd.gui import parameter_widgets
-from mne_pipeline_hd.gui.base_widgets import SimpleDict
-from mne_pipeline_hd.gui.parameter_widgets import Param, _eval_param
+from mne_pipeline_hd.gui.parameter_widgets import Param, _eval_param, LabelGui
+from mne_pipeline_hd.tests._test_utils import toggle_checked_list_model
 
 parameters = {
     "IntGui": 1,
     "FloatGui": 5.3,
     "StringGui": "postcentral-lh",
     "MultiTypeGui": 42,
     "FuncGui": "np.arange(10) * np.pi",
@@ -36,14 +24,15 @@
     "TupleGui": (45, 6),
     "ComboGui": "a",
     "ListGui": [1, 454.33, "postcentral-lh", 5],
     "CheckListGui": ["postcentral-lh"],
     "DictGui": {"A": "B", "C": 58.144, 3: [1, 2, 3, 4], "D": {"A": 1, "B": 2}},
     "SliderGui": 5,
     "ColorGui": {"C": "#98765432", "3": "#97867564"},
+    "PathGui": "C:/test",
 }
 
 alternative_parameters = {
     "IntGui": 5,
     "FloatGui": 8.45,
     "StringGui": "precentral-lh",
     "MultiTypeGui": 32,
@@ -52,14 +41,15 @@
     "TupleGui": (2, 23),
     "ComboGui": "b",
     "ListGui": [33, 2234.33, "precentral-lh", 3],
     "CheckListGui": ["precentral-lh"],
     "DictGui": {"B": "V", "e": 11.333, 5: [65, 3, 11], "F": {"C": 1, "D": 2}},
     "SliderGui": 2,
     "ColorGui": {"A": "#12345678", "B": "#13243546"},
+    "PathGui": "D:/test",
 }
 
 gui_kwargs = {
     "none_select": True,
     "min_val": -40,
     "max_val": 100,
     "step": 0.5,
@@ -124,117 +114,131 @@
             min_val = kwargs["min_val"]
         gui.set_param(value)
         assert parameters[gui_name] == max_val
         # less than min
         gui.set_param(neg_value)
         assert parameters[gui_name] == min_val
 
+    # Test return integer for BoolGui
     if "return_integer" in gui_parameters:
         gui.return_integer = True
         gui.set_param(True)
         assert gui.get_value() == 1
 
+    # Test ComboGui
     if gui_name == "ComboGui":
         # Don't set values which are not in options
         with pytest.raises(KeyError):
             gui.set_param("d")
 
+        # Test option-aliases
+        gui.set_param("a")
+        assert gui.param_widget.currentText() == "A"
+        gui.param_widget.setCurrentText("B")
+        assert gui.get_value() == "b"
+
+    # Test MultiTypeGui
     if gui_name == "MultiTypeGui":
-        for gui_type, gui_name in gui.gui_types.items():
-            gui.set_param(parameters[gui_name])
-            assert gui.get_value() == parameters[gui_name]
+        for gui_type, type_gui_name in gui.gui_types.items():
+            gui.set_param(parameters[type_gui_name])
+            assert gui.get_value() == parameters[type_gui_name]
             assert type(gui.get_value()).__name__ == gui_type
         kwargs["type_selection"] = True
         kwargs["type_kwargs"] = dict()
-        for gui_name in gui.gui_types.values():
-            type_class = getattr(parameter_widgets, gui_name)
+        for type_gui_name in gui.gui_types.values():
+            type_class = getattr(parameter_widgets, type_gui_name)
             gui_parameters = list(inspect.signature(type_class).parameters) + list(
                 inspect.signature(Param).parameters
             )
             t_kwargs = {
                 key: value for key, value in gui_kwargs.items() if key in gui_parameters
             }
-            kwargs["type_kwargs"][gui_name] = t_kwargs
+            kwargs["type_kwargs"][type_gui_name] = t_kwargs
         gui = gui_class(data=parameters, name=gui_name, **kwargs)
-        for gui_type, gui_name in gui.gui_types.items():
-            type_idx = gui.types.index(gui_type)
+        for type_idx, (gui_type, type_gui_name) in enumerate(gui.gui_types.items()):
             gui.change_type(type_idx)
-            gui.set_param(parameters[gui_name])
-            assert gui.get_value() == parameters[gui_name]
+            gui.set_param(parameters[type_gui_name])
+            assert gui.get_value() == parameters[type_gui_name]
             assert type(gui.get_value()).__name__ == gui_type
 
 
-class ParamGuis(QWidget):
-    def __init__(self):
-        super().__init__()
-
-        self.gui_dict = dict()
-
-        self.init_ui()
-
-    def init_ui(self):
-        test_layout = QVBoxLayout()
-        grid_layout = QGridLayout()
-        max_cols = 4
-        set_none_select = True
-        set_groupbox_layout = False
-        set_alias = False
-
-        for idx, gui_nm in enumerate(gui_kwargs):
-            kw_args = gui_kwargs[gui_nm]
-            kw_args["data"] = parameters
-            kw_args["name"] = gui_nm
-            kw_args["none_select"] = set_none_select
-            kw_args["groupbox_layout"] = set_groupbox_layout
-            if set_alias:
-                kw_args["alias"] = gui_nm + "-alias"
-            kw_args["description"] = gui_nm + "-description"
-            gui = getattr(parameter_widgets, gui_nm)(**kw_args)
-            grid_layout.addWidget(gui, idx // max_cols, idx % max_cols)
-            self.gui_dict[gui_nm] = gui
-
-        test_layout.addLayout(grid_layout)
-
-        set_layout = QHBoxLayout()
-        self.gui_cmbx = QComboBox()
-        self.gui_cmbx.addItems(self.gui_dict.keys())
-        set_layout.addWidget(self.gui_cmbx)
-
-        self.set_le = QLineEdit()
-        set_layout.addWidget(self.set_le)
-
-        set_bt = QPushButton("Set")
-        set_bt.clicked.connect(self.set_param)
-        set_layout.addWidget(set_bt)
-
-        show_bt = QPushButton("Show Parameters")
-        show_bt.clicked.connect(self.show_parameters)
-        set_layout.addWidget(show_bt)
-
-        test_layout.addLayout(set_layout)
-
-        self.setLayout(test_layout)
-
-    def set_param(self):
-        current_gui = self.gui_cmbx.currentText()
-        try:
-            value = literal_eval(self.set_le.text())
-        except (SyntaxError, ValueError):
-            value = self.set_le.text()
-        parameters[current_gui] = value
-        p_gui = self.gui_dict[current_gui]
-        p_gui.read_param()
-        p_gui._set_param()
-
-    def show_parameters(self):
-        dlg = QDialog(self)
-        layout = QVBoxLayout()
-        layout.addWidget(SimpleDict(parameters))
-        dlg.setLayout(layout)
-        dlg.open()
-
-
-def show_param_guis():
-    app = QApplication.instance() or QApplication(sys.argv)
-    test_widget = ParamGuis()
-    test_widget.show()
-    sys.exit(app.exec())
+def test_label_gui(qtbot, controller):
+    """Test opening label-gui without error"""
+    # Add fsaverage
+    controller.pr.add_fsmri("fsaverage")
+
+    # Add start labels
+    controller.pr.parameters["Default"]["test_labels"] = [
+        "insula-lh",
+        "postcentral-lh",
+        "lh.BA1-lh",
+    ]
+
+    label_gui = LabelGui(data=controller, name="test_labels", default=[])
+    qtbot.addWidget(label_gui)
+
+    # Check start labels
+    assert label_gui.param_value == ["insula-lh", "postcentral-lh", "lh.BA1-lh"]
+
+    # Push edit button
+    label_gui.param_widget.click()
+    dlg = label_gui._dialog
+
+    # Test start labels in checked
+    assert ["insula-lh", "postcentral-lh"] == dlg._selected_parc_labels
+    assert "lh.BA1-lh" in dlg._selected_extra_labels
+
+    # Open Parc-Picker
+    dlg.choose_parc_bt.click()
+    parc_plot = dlg._parc_picker._renderer.plotter
+    # Select "aparc" parcellation
+    dlg.parcellation_cmbx.setCurrentText("aparc")
+    dlg._parc_changed()  # Only triggered by mouse click with .activated
+    # Check if start labels are shown
+    assert "insula-lh" in dlg._parc_picker._shown_labels
+    assert "postcentral-lh" in dlg._parc_picker._shown_labels
+    # Add label by clicking on plot
+    qtbot.mouseClick(parc_plot, Qt.LeftButton, pos=parc_plot.rect().center(), delay=100)
+    assert "supramarginal-rh" in dlg._selected_parc_labels
+    # Remove label by clicking on plot
+    qtbot.mouseClick(parc_plot, Qt.LeftButton, pos=parc_plot.rect().center(), delay=100)
+    assert "superiorfrontal-rh" not in dlg._selected_parc_labels
+    # Add label by selecting from list
+    toggle_checked_list_model(dlg.parc_label_list.model, value=1, row=5)
+    assert "caudalmiddlefrontal-rh" in dlg._parc_picker._shown_labels
+    toggle_checked_list_model(dlg.parc_label_list.model, value=0, row=5)
+    assert "caudalmiddlefrontal-rh" not in dlg._parc_picker._shown_labels
+
+    # Trigger subject changed (only fsaverage available), should not change anything
+    dlg._subject_changed()
+    parc_plot = dlg._parc_picker._renderer.plotter
+    assert ["insula-lh", "postcentral-lh"] == dlg._selected_parc_labels
+    assert "lh.BA1-lh" in dlg._selected_extra_labels
+
+    # Open Extra-Picker
+    dlg.choose_extra_bt.click()
+    # Check if start labels are shown
+    assert "lh.BA1-lh" in dlg._extra_picker._shown_labels
+
+    # Change parcellation
+    dlg.parcellation_cmbx.setCurrentText("aparc_sub")
+    dlg._parc_changed()  # Only triggered by mouse click with .activated
+    # Add label by clicking on plot
+    qtbot.mouseClick(parc_plot, Qt.LeftButton, pos=parc_plot.rect().center(), delay=100)
+    assert "supramarginal_9-rh" in dlg._selected_parc_labels
+    # Add label by selecting from list
+    toggle_checked_list_model(dlg.parc_label_list.model, value=1, row=0)
+    assert "bankssts_1-lh" in dlg._selected_parc_labels
+
+    final_selection = [
+        "insula-lh",
+        "postcentral-lh",
+        "supramarginal_9-rh",
+        "bankssts_1-lh",
+        "lh.BA1-lh",
+    ]
+    # Check display widget
+    assert dlg.selected_display.model._data == final_selection
+
+    # Add all labels
+    dlg.close()
+    assert label_gui.param_value == final_selection
```

### Comparing `mne-pipeline-hd-0.3.3a0/mne_pipeline_hd.egg-info/SOURCES.txt` & `mne_pipeline_hd-0.3.3a0.dev0/mne_pipeline_hd.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,25 @@
 mne_pipeline_hd.egg-info/SOURCES.txt
 mne_pipeline_hd.egg-info/dependency_links.txt
 mne_pipeline_hd.egg-info/entry_points.txt
 mne_pipeline_hd.egg-info/requires.txt
 mne_pipeline_hd.egg-info/top_level.txt
 mne_pipeline_hd/development/__init__.py
 mne_pipeline_hd/development/check_ressources.py
+mne_pipeline_hd/development/console_widget_speed.py
 mne_pipeline_hd/development/dev_utils.py
+mne_pipeline_hd/extra/__init__.py
+mne_pipeline_hd/extra/default_settings.json
+mne_pipeline_hd/extra/functions.csv
+mne_pipeline_hd/extra/license.txt
+mne_pipeline_hd/extra/mne_license.txt
+mne_pipeline_hd/extra/mne_pipeline_icon_dark.png
+mne_pipeline_hd/extra/mne_pipeline_icon_light.png
+mne_pipeline_hd/extra/mne_pipeline_logo_evee_smaller.jpg
+mne_pipeline_hd/extra/parameters.csv
 mne_pipeline_hd/functions/__init__.py
 mne_pipeline_hd/functions/operations.py
 mne_pipeline_hd/functions/plot.py
 mne_pipeline_hd/gui/__init__.py
 mne_pipeline_hd/gui/base_widgets.py
 mne_pipeline_hd/gui/dialogs.py
 mne_pipeline_hd/gui/education_widgets.py
@@ -37,28 +47,21 @@
 mne_pipeline_hd/pipeline/function_utils.py
 mne_pipeline_hd/pipeline/legacy.py
 mne_pipeline_hd/pipeline/loading.py
 mne_pipeline_hd/pipeline/parallel.py
 mne_pipeline_hd/pipeline/pipeline_utils.py
 mne_pipeline_hd/pipeline/plot_utils.py
 mne_pipeline_hd/pipeline/project.py
-mne_pipeline_hd/resource/__init__.py
-mne_pipeline_hd/resource/default_settings.json
-mne_pipeline_hd/resource/functions.csv
-mne_pipeline_hd/resource/license.txt
-mne_pipeline_hd/resource/mne_license.txt
-mne_pipeline_hd/resource/mne_pipeline_icon_dark.png
-mne_pipeline_hd/resource/mne_pipeline_icon_light.png
-mne_pipeline_hd/resource/mne_pipeline_logo_evee_smaller.jpg
-mne_pipeline_hd/resource/parameters.csv
 mne_pipeline_hd/tests/__init__.py
 mne_pipeline_hd/tests/_test_utils.py
 mne_pipeline_hd/tests/test_app.py
+mne_pipeline_hd/tests/test_base_widgets.py
 mne_pipeline_hd/tests/test_concurrent.py
+mne_pipeline_hd/tests/test_console.py
 mne_pipeline_hd/tests/test_controller.py
 mne_pipeline_hd/tests/test_functions.py
 mne_pipeline_hd/tests/test_loading.py
 mne_pipeline_hd/tests/test_main_window.py
-mne_pipeline_hd/tests/test_param_guis.py
+mne_pipeline_hd/tests/test_parameter_widgets.py
 mne_pipeline_hd/tests/test_project.py
 mne_pipeline_hd/tests/test_qsettings.py
 mne_pipeline_hd/tests/test_welcome_window.py
```

