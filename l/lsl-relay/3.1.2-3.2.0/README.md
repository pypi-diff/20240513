# Comparing `tmp/lsl_relay-3.1.2.tar.gz` & `tmp/lsl_relay-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsl_relay-3.1.2.tar", last modified: Thu Jun  1 07:10:52 2023, max compression
+gzip compressed data, was "lsl_relay-3.2.0.tar", last modified: Mon May 13 12:22:16 2024, max compression
```

## Comparing `lsl_relay-3.1.2.tar` & `lsl_relay-3.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.425257 lsl_relay-3.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.429257 lsl_relay-3.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/conda-env.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.429257 lsl_relay-3.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/device_sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/guides/time_alignment.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.433257 lsl_relay-3.1.2/examples/cloud_recordings/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/cloud_recordings/time_alignment_parameters.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/examples/companion_app_exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.437257 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/
--rw-r--r--   0 runner    (1001) docker     (123)   163603 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv
--rw-r--r--   0 runner    (1001) docker     (123)   167691 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_1/time_alignment_parameters.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.437257 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/
--rw-r--r--   0 runner    (1001) docker     (123)   165227 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv
--rw-r--r--   0 runner    (1001) docker     (123)   162539 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/companion_app_exports/subject_2/time_alignment_parameters.json
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/device_vs_lsl_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/linear_time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/examples/time_mapping_from_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.441257 lsl_relay-3.1.2/src/lsl_relay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 07:10:52.000000 lsl_relay-3.1.2/src/lsl_relay.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.417257 lsl_relay-3.1.2/src/pupil_labs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.445257 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/linear_time_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/outlets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10535 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.445257 lsl_relay-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tests/test_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:10:52.449257 lsl_relay-3.1.2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/extract_eye_video_illuminance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/monitor_relay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/print_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tools/show_relay_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-01 07:10:27.000000 lsl_relay-3.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.397381 lsl_relay-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 12:22:16.397381 lsl_relay-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/conda-env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/guides/device_sync.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/guides/time_alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/examples/cloud_recordings/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/cloud_recordings/time_alignment_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.385381 lsl_relay-3.2.0/examples/companion_app_exports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.389381 lsl_relay-3.2.0/examples/companion_app_exports/subject_1/
+-rw-r--r--   0 runner    (1001) docker     (127)   163603 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   167691 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_1/time_alignment_parameters.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.393381 lsl_relay-3.2.0/examples/companion_app_exports/subject_2/
+-rw-r--r--   0 runner    (1001) docker     (127)   165227 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   162539 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/companion_app_exports/subject_2/time_alignment_parameters.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/device_vs_lsl_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/linear_time_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/examples/time_mapping_from_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-13 12:22:16.397381 lsl_relay-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.385381 lsl_relay-3.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.397381 lsl_relay-3.2.0/src/lsl_relay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 12:22:16.000000 lsl_relay-3.2.0/src/lsl_relay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.385381 lsl_relay-3.2.0/src/pupil_labs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.393381 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/linear_time_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/outlets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10551 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.393381 lsl_relay-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:22:16.397381 lsl_relay-3.2.0/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tools/extract_eye_video_illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tools/monitor_relay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tools/print_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tools/show_relay_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-13 12:21:55.000000 lsl_relay-3.2.0/tox.ini
```

### Comparing `lsl_relay-3.1.2/.github/workflows/main.yml` & `lsl_relay-3.2.0/.github/workflows/main.yml`

 * *Files 11% similar despite different names*

```diff
@@ -8,19 +8,17 @@
   workflow_dispatch:
 
 jobs:
   test:
     strategy:
       matrix:
         python:
-          - 3.7
-          - 3.8
-          - 3.9
           - "3.10"
           - "3.11"
+          - "3.12"
         platform:
           - ubuntu-latest
           - macos-latest
           - windows-latest
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
```

### Comparing `lsl_relay-3.1.2/.gitignore` & `lsl_relay-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/.pre-commit-config.yaml` & `lsl_relay-3.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/CHANGES.rst` & `lsl_relay-3.2.0/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+3.1.1 (2024-05-09)
+##################
+- Bumps real-time API to support Pupillometry & Eye state in real-time.
+
 3.1.0 (2023-05-25)
 ##################
 - Adds official support for Neon modules
 - New project name pupil-labs-lsl-relay
 
 3.0.2 (2022-11-09)
 ##################
```

### Comparing `lsl_relay-3.1.2/LICENSE` & `lsl_relay-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/README.rst` & `lsl_relay-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/docs/conf.py` & `lsl_relay-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/docs/guides/device_sync.rst` & `lsl_relay-3.2.0/docs/guides/device_sync.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/docs/guides/overview.rst` & `lsl_relay-3.2.0/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/docs/guides/time_alignment.rst` & `lsl_relay-3.2.0/docs/guides/time_alignment.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/docs/index.rst` & `lsl_relay-3.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv` & `lsl_relay-3.2.0/examples/companion_app_exports/subject_1/PI left v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv` & `lsl_relay-3.2.0/examples/companion_app_exports/subject_1/PI right v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv` & `lsl_relay-3.2.0/examples/companion_app_exports/subject_2/PI left v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv` & `lsl_relay-3.2.0/examples/companion_app_exports/subject_2/PI right v1 ps1.illuminance.csv`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/device_vs_lsl_sync.py` & `lsl_relay-3.2.0/examples/device_vs_lsl_sync.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/linear_time_model.py` & `lsl_relay-3.2.0/examples/linear_time_model.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/examples/time_mapping_from_parameters.py` & `lsl_relay-3.2.0/examples/time_mapping_from_parameters.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/setup.cfg` & `lsl_relay-3.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 	Pupil Labs Realtime Network API=https://github.com/pupil-labs/realtime-network-api
 	LabStreamingLayer=https://labstreaminglayer.readthedocs.io/
 
 [options]
 packages = find_namespace:
 install_requires = 
 	click>=7.0
-	pupil-labs-realtime-api>=1.1.0
+	pupil-labs-realtime-api>=1.2.1
 	pylsl>=1.12.2
 	rich
 	typing-extensions
 	importlib-metadata;python_version<"3.8"
-python_requires = >=3.7
+python_requires = >=3.10
 include_package_data = true
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
 exclude =
```

### Comparing `lsl_relay-3.1.2/src/lsl_relay.egg-info/SOURCES.txt` & `lsl_relay-3.2.0/src/lsl_relay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/channels.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/channels.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/cli.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/cli.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/linear_time_model.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/linear_time_model.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/outlets.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/outlets.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/relay.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/relay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import logging
 import uuid
 from typing import Iterable, List, NoReturn, Optional
 
 from pupil_labs.realtime_api import Device, StatusUpdateNotifier, receive_gaze_data
 from pupil_labs.realtime_api.models import Component, Event, Sensor
-from pupil_labs.realtime_api.streaming import GazeData
+from pupil_labs.realtime_api.simple.models import GazeDataType
 from pupil_labs.realtime_api.time_echo import TimeOffsetEstimator
 
 from pupil_labs.lsl_relay import outlets
 
 logger = logging.getLogger(__name__)
 logging.getLogger("pupil_labs.realtime_api.time_echo").setLevel("WARNING")
 
@@ -80,15 +80,15 @@
 
     async def receive_gaze_sample(self):
         while True:
             if self.receiver.gaze_sensor_url:
                 async for gaze in receive_gaze_data(
                     self.receiver.gaze_sensor_url, run_loop=True, log_level=30
                 ):
-                    if isinstance(gaze, GazeData):
+                    if isinstance(gaze, GazeDataType):
                         await self.gaze_sample_queue.put(
                             GazeAdapter(gaze, self.receiver.clock_offset_ns)
                         )
                     else:
                         logger.warning(f"Dropping unknown gaze data type: {gaze}")
             else:
                 logger.debug("The gaze sensor was not yet identified.")
@@ -225,15 +225,15 @@
 
     async def cleanup(self):
         if self.notifier is not None:
             await self.notifier.receive_updates_stop()
 
 
 class GazeAdapter:
-    def __init__(self, sample: GazeData, clock_offset_ns: int):
+    def __init__(self, sample: GazeDataType, clock_offset_ns: int):
         self.x = sample.x
         self.y = sample.y
         self.timestamp_unix_seconds = (
             sample.timestamp_unix_seconds + clock_offset_ns * 1e-9
         )
```

### Comparing `lsl_relay-3.1.2/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py` & `lsl_relay-3.2.0/src/pupil_labs/lsl_relay/xdf_cloud_time_sync.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/tools/extract_eye_video_illuminance.py` & `lsl_relay-3.2.0/tools/extract_eye_video_illuminance.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/tools/monitor_relay.py` & `lsl_relay-3.2.0/tools/monitor_relay.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/tools/print_events.py` & `lsl_relay-3.2.0/tools/print_events.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/tools/show_relay_metadata.py` & `lsl_relay-3.2.0/tools/show_relay_metadata.py`

 * *Files identical despite different names*

### Comparing `lsl_relay-3.1.2/tox.ini` & `lsl_relay-3.2.0/tox.ini`

 * *Files identical despite different names*

