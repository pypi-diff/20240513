# Comparing `tmp/qt-data-extractor-0.2.2.tar.gz` & `tmp/qt_data_extractor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qt-data-extractor-0.2.2.tar", last modified: Wed Dec 27 22:16:02 2023, max compression
+gzip compressed data, was "qt_data_extractor-0.3.0.tar", last modified: Mon May 13 16:10:33 2024, max compression
```

## Comparing `qt-data-extractor-0.2.2.tar` & `qt_data_extractor-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.857429 qt-data-extractor-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.845429 qt-data-extractor-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.849429 qt-data-extractor-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     9885 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-12-27 22:16:02.857429 qt-data-extractor-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/data-extractor.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.849429 qt-data-extractor-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.849429 qt-data-extractor-0.2.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      346 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2023-12-27 22:16:02.857429 qt-data-extractor-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.845429 qt-data-extractor-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.853428 qt-data-extractor-0.2.2/src/qt_data_extractor/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.853428 qt-data-extractor-0.2.2/src/qt_data_extractor/design/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/copy-progress.ui
--rw-r--r--   0 runner    (1001) docker     (127)     8391 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/copy-prompt.ui
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/create_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    27560 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/main-window.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/manage-connections.ui
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/design/pandas_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.853428 qt-data-extractor-0.2.2/src/qt_data_extractor/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/hooks/hook-qt_data_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    34026 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/mainwindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/src/qt_data_extractor/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.857429 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-27 22:16:02.000000 qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.853428 qt-data-extractor-0.2.2/static/
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/static/logo-256.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9662 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/static/logo-48.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 22:16:02.853428 qt-data-extractor-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-27 22:15:32.000000 qt-data-extractor-0.2.2/wix.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.949024 qt_data_extractor-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.953024 qt_data_extractor-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     9885 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/data-extractor.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.949024 qt_data_extractor-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/src/qt_data_extractor/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.957024 qt_data_extractor-0.3.0/src/qt_data_extractor/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-progress.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     8391 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-prompt.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/create_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27560 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/main-window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/manage-connections.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/design/pandas_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/src/qt_data_extractor/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/hooks/hook-qt_data_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33419 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/mainwindow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/src/qt_data_extractor/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:10:33.000000 qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/static/logo-256.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9662 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/static/logo-48.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:10:33.961024 qt_data_extractor-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-13 16:10:08.000000 qt_data_extractor-0.3.0/wix.json
```

### Comparing `qt-data-extractor-0.2.2/.coveragerc` & `qt_data_extractor-0.3.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/.github/workflows/ci.yml` & `qt_data_extractor-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/.gitignore` & `qt_data_extractor-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/.pre-commit-config.yaml` & `qt_data_extractor-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/.readthedocs.yml` & `qt_data_extractor-0.3.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/CONTRIBUTING.md` & `qt_data_extractor-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/LICENSE.txt` & `qt_data_extractor-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/PKG-INFO` & `qt_data_extractor-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-data-extractor
-Version: 0.2.2
+Version: 0.3.0
 Summary: Extract data from industrial historians
 Home-page: https://github.com/imubit/qt-data-extractor/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/qt-data-extractor/
 Project-URL: Source, https://github.com/imubit/qt-data-extractor/
```

### Comparing `qt-data-extractor-0.2.2/README.md` & `qt_data_extractor-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/data-extractor.spec` & `qt_data_extractor-0.3.0/data-extractor.spec`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/docs/Makefile` & `qt_data_extractor-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/docs/conf.py` & `qt_data_extractor-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/docs/index.md` & `qt_data_extractor-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/setup.cfg` & `qt_data_extractor-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/setup.py` & `qt_data_extractor-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/__init__.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/copy-progress.ui` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-progress.ui`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/copy-prompt.ui` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/copy-prompt.ui`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/create_connection.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/create_connection.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/main-window.ui` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/main-window.ui`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/manage-connections.ui` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/manage-connections.ui`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/design/pandas_model.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/design/pandas_model.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/main.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/main.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/mainwindow.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/mainwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,17 +110,23 @@
 
     def _get_selected_tags(self):
         return [
             self._w.treeSelectedTags.topLevelItem(i).data(0, QtCore.Qt.UserRole)
             for i in range(0, self._w.treeSelectedTags.topLevelItemCount())
         ]
 
+    @property
+    def _current_connection(self):
+        return self._w.comboLeftConnection.currentData()
+
+    # SLOTS
+
     @QtCore.Slot(str)
     def on_connection_change(self):
-        current_conn = self._w.comboLeftConnection.currentData()
+        current_conn = self._current_connection
         if not current_conn:
             self._refresh_current_connection_view(current_conn=None)
             return
 
         if current_conn == "add_new":
             self._w.comboLeftConnection.setCurrentIndex(-1)
             self.on_create_new_connection()
@@ -270,14 +276,24 @@
             dlg = DataTableDialog(df, parent=self._w)
             dlg.show()
 
         except Exception as e:
             QMessageBox.critical(self._w, self._w.windowTitle(), str(e))
 
     @QtCore.Slot()
+    def on_selected_tags_change(self):
+        selected_items = len(self._w.treeSelectedTags.selectedItems())
+        total_items = self._w.treeSelectedTags.topLevelItemCount()
+        self._w.labelRightPanelStatus.setText(
+            f"{selected_items} / {total_items} tags"
+            if selected_items > 0
+            else f"{total_items} tags"
+        )
+
+    @QtCore.Slot()
     def on_add_selected_tags(self):
         source_items = self._w.treeLeftTagHierarchy.selectedItems()
 
         source_tags = {
             i.data(0, QtCore.Qt.UserRole): i.data(1, QtCore.Qt.UserRole)
             for i in source_items
         }
@@ -294,26 +310,15 @@
             item.setData(0, QtCore.Qt.UserRole, (tag_name))
             item.setData(1, QtCore.Qt.UserRole, (source_tags[tag_name]))
 
             self._w.treeSelectedTags.addTopLevelItem(item)
 
         self._mark_selected_tags()
 
-        @QtCore.Slot()
-        def on_tree_selection_changed():
-            selected_items = len(self._w.treeSelectedTags.selectedItems())
-            total_items = self._w.treeSelectedTags.topLevelItemCount()
-            self._w.labelRightPanelStatus.setText(
-                f"{selected_items} / {total_items} tags"
-                if selected_items > 0
-                else f"{total_items} tags"
-            )
-
-        self._w.treeSelectedTags.itemSelectionChanged.connect(on_tree_selection_changed)
-        on_tree_selection_changed()
+        self.on_selected_tags_change()
 
     @QtCore.Slot()
     def on_remove_selected_tags(self, all):
         if all:
             self._w.treeSelectedTags.clear()
             self._mark_selected_tags()
             return
@@ -543,15 +548,67 @@
 
             tag_name = item.data(0, QtCore.Qt.UserRole)
             for i in range(item.columnCount()):
                 item.setFont(
                     i, font_selected if tag_name in selected_tags else font_deselected
                 )
 
-    def _refresh_tags_tree(self, filter, conn_name, display_attributes):
+    # Dynamic tree expansion
+    @QtCore.Slot(QTreeWidgetItem)
+    def on_tree_expanded(self, clicked_item):
+        conn_name = self._current_connection["name"]
+        display_attributes = OrderedDict(self._current_connection["default_attributes"])
+
+        tag = clicked_item.data(1, QtCore.Qt.UserRole)
+        if tag["HasChildren"]:
+            # Reload children
+            for i in reversed(range(clicked_item.childCount())):
+                clicked_item.removeChild(clicked_item.child(i))
+
+            children = self._api.list_tags(
+                conn_name,
+                filter=tag["Name"],
+                include_attributes=True,
+                max_results=MAX_TAGS_TO_LOAD,
+            )
+
+            for i, child_name in enumerate(children):
+                row = [
+                    str(children[child_name][key])
+                    if key in children[child_name]
+                    else ""
+                    for j, key in enumerate(display_attributes.keys())
+                ]
+
+                child_item = QTreeWidgetItem(row)
+                child_item.setData(0, QtCore.Qt.UserRole, (child_name))
+                child_item.setData(1, QtCore.Qt.UserRole, (children[child_name]))
+
+                clicked_item.addChild(child_item)
+
+    @QtCore.Slot()
+    def on_tree_selection_changed(self):
+        total_items = self._w.treeLeftTagHierarchy.topLevelItemCount()
+        selected_items = len(self._w.treeLeftTagHierarchy.selectedItems())
+        too_many_tags_msg = (
+            " (Too Many Tags to Display - Narrow Your Search)"
+            if total_items >= MAX_TAGS_TO_LOAD
+            else ""
+        )
+        self._w.labelLeftPanelStatus.setText(
+            f"{selected_items} / {total_items} tags {too_many_tags_msg}"
+            if selected_items > 0
+            else f"{total_items} tags {too_many_tags_msg}"
+        )
+
+    @QtCore.Slot()
+    def on_refresh_tags_tree(self, filter):
+        conn_name = self._current_connection["name"]
+        display_attributes = OrderedDict(self._current_connection["default_attributes"])
+
         # Prepare headers
         self._w.treeLeftTagHierarchy.clear()
         self._w.treeLeftTagHierarchy.setColumnCount(len(display_attributes))
         self._w.treeLeftTagHierarchy.setHeaderLabels(
             [a["Name"] for a in display_attributes.values()]
         )
 
@@ -589,64 +646,42 @@
             self._show_msg_box(
                 f"Cannot find {len(missing_tags)} tag(s): {', '.join(missing_tags)}"[
                     :2000
                 ],
                 icon=QMessageBox.Icon.Warning,
             )
 
-        # Dynamic tree expansion
-        @QtCore.Slot(QTreeWidgetItem)
-        def on_tree_expanded(clicked_item):
-            tag = clicked_item.data(1, QtCore.Qt.UserRole)
-            if tag["HasChildren"]:
-                # Reload children
-                for i in reversed(range(clicked_item.childCount())):
-                    clicked_item.removeChild(clicked_item.child(i))
-
-                children = self._api.list_tags(
-                    conn_name,
-                    filter=tag["Name"],
-                    include_attributes=True,
-                    max_results=MAX_TAGS_TO_LOAD,
-                )
-
-                for i, child_name in enumerate(children):
-                    row = [
-                        str(children[child_name][key])
-                        if key in children[child_name]
-                        else ""
-                        for j, key in enumerate(display_attributes.keys())
-                    ]
-
-                    child_item = QTreeWidgetItem(row)
-                    child_item.setData(0, QtCore.Qt.UserRole, (child_name))
-                    child_item.setData(1, QtCore.Qt.UserRole, (children[child_name]))
-
-                    clicked_item.addChild(child_item)
-
-        self._w.treeLeftTagHierarchy.itemExpanded.connect(on_tree_expanded)
-
-        @QtCore.Slot()
-        def on_tree_selection_changed():
-            selected_items = len(self._w.treeLeftTagHierarchy.selectedItems())
-            too_many_tags_msg = (
-                " (Too Many Tags to Display - Narrow Your Search)"
-                if len(tags) >= MAX_TAGS_TO_LOAD
-                else ""
-            )
-            self._w.labelLeftPanelStatus.setText(
-                f"{selected_items} / {len(tags)} tags {too_many_tags_msg}"
-                if selected_items > 0
-                else f"{len(tags)} tags {too_many_tags_msg}"
-            )
+        self.on_tree_selection_changed()
 
-        self._w.treeLeftTagHierarchy.itemSelectionChanged.connect(
-            on_tree_selection_changed
+    @QtCore.Slot(str)
+    def on_tags_file_select(self):
+        filename, filter = QFileDialog.getOpenFileName(
+            parent=self._w,
+            caption="Select Tags File",
+            dir=".",
+            # filter='*.xls, *.xlsx, *.xlsm, *.xlsb, *.odf, *.ods, *.odt')
+            filter="*.xlsx",
         )
-        on_tree_selection_changed()
+        if not filename:
+            return
+
+        try:
+            df = pd.read_excel(filename, header=None)
+            df = df.dropna()
+            tags_to_find = df.iloc[:, 0].tolist()
+
+            self.on_refresh_tags_tree(filter=tags_to_find)
+            self._w.comboLeftTagFilter.clear()
+
+        except Exception as e:
+            mb = QMessageBox(self._w)
+            # mb.setIcon(QMessageBox.Icon.Error)
+            mb.setWindowTitle(self._w.windowTitle())
+            mb.setText(f"Error reading excel file: {str(e)}")
+            mb.exec_()
 
     def _refresh_connections(self):
         """ """
         self._w.comboLeftConnection.clear()
 
         self._existing_connections = self._api.list_connections()
 
@@ -717,64 +752,19 @@
             return
 
         self._w.labelLeftConnectionDetails.setText(conn_info["OneLiner"])
 
         # - Filters configuration -
         self._w.comboLeftTagFilter.setCurrentText(TAGS_FILTER_DEFAULT_PLACEHOLDER)
 
-        # Update panel on filter change
-        @QtCore.Slot(str)
-        def on_name_filter_changed(text):
-            self._refresh_tags_tree(
-                filter=text,
-                conn_name=current_conn["name"],
-                display_attributes=OrderedDict(current_conn["default_attributes"]),
-            )
-
-        self._w.comboLeftTagFilter.textActivated.connect(on_name_filter_changed)
-        self._w.comboLeftTagFilter.installEventFilter(self._filterWidgetEventInspector)
-
         if "name" in current_conn["supported_filters"]:
             self._w.comboLeftTagFilter.show()
         else:
             self._w.comboLeftTagFilter.hide()
 
-        @QtCore.Slot(str)
-        def on_tags_file_select():
-            filename, filter = QFileDialog.getOpenFileName(
-                parent=self._w,
-                caption="Select Tags File",
-                dir=".",
-                # filter='*.xls, *.xlsx, *.xlsm, *.xlsb, *.odf, *.ods, *.odt')
-                filter="*.xlsx",
-            )
-            if not filename:
-                return
-
-            try:
-                df = pd.read_excel(filename, header=None)
-                df = df.dropna()
-                tags_to_find = df.iloc[:, 0].tolist()
-
-                self._refresh_tags_tree(
-                    filter=tags_to_find,
-                    conn_name=current_conn["name"],
-                    display_attributes=OrderedDict(current_conn["default_attributes"]),
-                )
-                self._w.comboLeftTagFilter.clear()
-
-            except Exception as e:
-                mb = QMessageBox(self._w)
-                # mb.setIcon(QMessageBox.Icon.Error)
-                mb.setWindowTitle(self._w.windowTitle())
-                mb.setText(f"Error reading excel file: {str(e)}")
-                mb.exec_()
-
-        self._w.buttonLeftTagsFileSelect.clicked.connect(on_tags_file_select)
-
         if "tags_file" in current_conn["supported_filters"]:
             self._w.buttonLeftTagsFileSelect.show()
         else:
             self._w.buttonLeftTagsFileSelect.hide()
 
         # Selection dates
         if "time" in current_conn["supported_filters"]:
@@ -785,39 +775,56 @@
             self._w.dateTimeLeftTo.setDateTime(end_time)
             self._w.widgetLeftTimeFilter.show()
 
         else:
             self._w.widgetLeftTimeFilter.hide()
 
         # Tag tree
-        # self._refreshTagsTree(filter=filter, conn_name=current_conn['name'],
-        #                       display_attributes=OrderedDict(current_conn['default_attributes']))
+        # self.on_refresh_tags_tree(filter=filter)
+
+    def setup(self):
+        self._w.setWindowTitle(f"{WINDOW_DEFAULT_TITLE} - v{__version__}")
 
-    def _setup_panel(self):
         # Connection list
         self._refresh_connections()
 
         self._w.comboLeftConnection.currentTextChanged.connect(
             self.on_connection_change
         )
 
-        @QtCore.Slot()
-        def on_connect():
-            self._enable_current_connection()
-
-        self._w.buttonLeftConnect.clicked.connect(on_connect)
+        self._w.buttonLeftConnect.clicked.connect(self._enable_current_connection)
 
         self.on_connection_change()
 
-    def _setup_manipulation_controls(self):
+        # Menu Bar
+        self._w.actionAddNewConnection.triggered.connect(self.on_create_new_connection)
+        self._w.actionManageConnections.triggered.connect(self.on_manage_connections)
+
+        # Display
+
+        self._w.comboLeftTagFilter.textActivated.connect(self.on_refresh_tags_tree)
+        self._w.comboLeftTagFilter.installEventFilter(self._filterWidgetEventInspector)
+
+        self._w.treeLeftTagHierarchy.itemExpanded.connect(self.on_tree_expanded)
+        self._w.treeLeftTagHierarchy.itemSelectionChanged.connect(
+            self.on_tree_selection_changed
+        )
+
+        self._w.treeSelectedTags.itemSelectionChanged.connect(
+            self.on_selected_tags_change
+        )
+
+        # Controls
         self._w.buttonLeftView.clicked.connect(lambda: self.on_view_tags(left=True))
         # shortcut_view = QtGui.QShortcut(QtGui.QKeySequence("F3"), self._w)
         # shortcut_view.activated.connect(self.on_view_tags)
         self._w.buttonRightView.clicked.connect(lambda: self.on_view_tags(left=False))
 
+        self._w.buttonLeftTagsFileSelect.clicked.connect(self.on_tags_file_select)
+
         self._w.buttonAddSelectedTags.clicked.connect(self.on_add_selected_tags)
 
         self._w.buttonRemoveAllSelected.clicked.connect(
             lambda: self.on_remove_selected_tags(all=True)
         )
         self._w.buttonRemoveSelected.clicked.connect(
             lambda: self.on_remove_selected_tags(all=False)
@@ -853,20 +860,9 @@
         # shortcutRefresh.activated.connect(QtWidgets.QApplication.instance().quit)
 
         # Exit
         self._w.buttonExit.clicked.connect(QtWidgets.QApplication.instance().quit)
         shortcut_quit = QtGui.QShortcut(QtGui.QKeySequence("Alt+F4"), self._w)
         shortcut_quit.activated.connect(QtWidgets.QApplication.instance().quit)
 
-    def _setup_menu_bar(self):
-        self._w.actionAddNewConnection.triggered.connect(self.on_create_new_connection)
-        self._w.actionManageConnections.triggered.connect(self.on_manage_connections)
-
-    def setup(self):
-        self._w.setWindowTitle(f"{WINDOW_DEFAULT_TITLE} - v{__version__}")
-
-        self._setup_panel()
-        self._setup_menu_bar()
-        self._setup_manipulation_controls()
-
     def show(self):
         self._w.show()
```

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor/worker_thread.py` & `qt_data_extractor-0.3.0/src/qt_data_extractor/worker_thread.py`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/PKG-INFO` & `qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qt-data-extractor
-Version: 0.2.2
+Version: 0.3.0
 Summary: Extract data from industrial historians
 Home-page: https://github.com/imubit/qt-data-extractor/
 Author: Meir Tseitlin
 Author-email: meir@imubit.com
 License: LGPLv3
 Project-URL: Documentation, https://github.com/imubit/qt-data-extractor/
 Project-URL: Source, https://github.com/imubit/qt-data-extractor/
```

### Comparing `qt-data-extractor-0.2.2/src/qt_data_extractor.egg-info/SOURCES.txt` & `qt_data_extractor-0.3.0/src/qt_data_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/static/logo-256.ico` & `qt_data_extractor-0.3.0/static/logo-256.ico`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/static/logo-48.ico` & `qt_data_extractor-0.3.0/static/logo-48.ico`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/tox.ini` & `qt_data_extractor-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `qt-data-extractor-0.2.2/wix.json` & `qt_data_extractor-0.3.0/wix.json`

 * *Files identical despite different names*

