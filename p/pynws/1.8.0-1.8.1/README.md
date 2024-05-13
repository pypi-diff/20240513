# Comparing `tmp/pynws-1.8.0.tar.gz` & `tmp/pynws-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynws-1.8.0.tar", last modified: Wed May  8 10:03:20 2024, max compression
+gzip compressed data, was "pynws-1.8.1.tar", last modified: Mon May 13 18:53:21 2024, max compression
```

## Comparing `pynws-1.8.0.tar` & `pynws-1.8.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-08 10:03:13.000000 pynws-1.8.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/postcreatecommand.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.devcontainer/python3.9/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-08 10:03:13.000000 pynws-1.8.0/.devcontainer/python3.9/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 10:03:13.000000 pynws-1.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-08 10:03:13.000000 pynws-1.8.0/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-08 10:03:13.000000 pynws-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-08 10:03:13.000000 pynws-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-08 10:03:13.000000 pynws-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-08 10:03:13.000000 pynws-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-08 10:03:20.705052 pynws-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-08 10:03:13.000000 pynws-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-08 10:03:13.000000 pynws-1.8.0/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-08 10:03:13.000000 pynws-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-08 10:03:13.000000 pynws-1.8.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:03:20.705052 pynws-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.693053 pynws-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/src/pynws/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.697053 pynws-1.8.0/src/pynws/backports/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/backports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/backports/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/nws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/raw_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    18146 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/simple_nws.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-08 10:03:13.000000 pynws-1.8.0/src/pynws/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/src/pynws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-08 10:03:20.000000 pynws-1.8.0/src/pynws.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.701053 pynws-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:03:20.705052 pynws-1.8.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/alerts_active_zone.json
--rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/alerts_active_zone_second.json
--rw-r--r--   0 runner    (1001) docker     (127)   132083 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/detailed_forecast.json
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast.json
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_empty.json
--rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly.json
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly_empty.json
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_forecast_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)    45128 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/gridpoints_stations.json
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/points.json
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations.json
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_alternate_units.json
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_empty.json
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_latest.json
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_metar.json
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_metar_noparse.json
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_missing_value.json
--rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_multiple.json
--rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_multiple_unsorted.json
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_noprop.json
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_other_unitcode.json
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/fixtures/stations_observations_strings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_nws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-05-08 10:03:13.000000 pynws-1.8.0/tests/test_simple_nws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.400106 pynws-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:53:16.000000 pynws-1.8.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.388106 pynws-1.8.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-13 18:53:16.000000 pynws-1.8.1/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (127)      212 2024-05-13 18:53:16.000000 pynws-1.8.1/.devcontainer/postcreatecommand.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.388106 pynws-1.8.1/.devcontainer/python3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-13 18:53:16.000000 pynws-1.8.1/.devcontainer/python3.9/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 18:53:16.000000 pynws-1.8.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.388106 pynws-1.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 18:53:16.000000 pynws-1.8.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.388106 pynws-1.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 18:53:16.000000 pynws-1.8.1/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 18:53:16.000000 pynws-1.8.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 18:53:16.000000 pynws-1.8.1/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 18:53:16.000000 pynws-1.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 18:53:16.000000 pynws-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 18:53:16.000000 pynws-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 18:53:16.000000 pynws-1.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-13 18:53:21.396106 pynws-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-13 18:53:16.000000 pynws-1.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-13 18:53:16.000000 pynws-1.8.1/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-13 18:53:16.000000 pynws-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-13 18:53:16.000000 pynws-1.8.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:53:21.400106 pynws-1.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.384106 pynws-1.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.392106 pynws-1.8.1/src/pynws/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.392106 pynws-1.8.1/src/pynws/backports/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/backports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/backports/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/raw_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/simple_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-13 18:53:16.000000 pynws-1.8.1/src/pynws/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.396106 pynws-1.8.1/src/pynws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 18:53:21.000000 pynws-1.8.1/src/pynws.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.392106 pynws-1.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:53:21.396106 pynws-1.8.1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7715 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/alerts_active_zone.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14878 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/alerts_active_zone_second.json
+-rw-r--r--   0 runner    (1001) docker     (127)   132083 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/detailed_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_forecast.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_forecast_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_forecast_hourly.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_forecast_hourly_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_forecast_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    45128 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/gridpoints_stations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/points.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_alternate_units.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_empty.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_latest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_metar.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_metar_noparse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_missing_value.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10288 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_multiple.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10282 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_multiple_unsorted.json
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_noprop.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_other_unitcode.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/fixtures/stations_observations_strings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/test_nws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19901 2024-05-13 18:53:16.000000 pynws-1.8.1/tests/test_simple_nws.py
```

### Comparing `pynws-1.8.0/.devcontainer/devcontainer.json` & `pynws-1.8.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/.github/dependabot.yml` & `pynws-1.8.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/.github/workflows/pytest.yml` & `pynws-1.8.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/.github/workflows/pythonpublish.yml` & `pynws-1.8.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/.github/workflows/typing.yml` & `pynws-1.8.1/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/LICENSE` & `pynws-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/PKG-INFO` & `pynws-1.8.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pynws
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
 Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynws-1.8.0/README.md` & `pynws-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/example.py` & `pynws-1.8.1/example.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/pyproject.toml` & `pynws-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/backports/enum.py` & `pynws-1.8.1/src/pynws/backports/enum.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/const.py` & `pynws-1.8.1/src/pynws/const.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/forecast.py` & `pynws-1.8.1/src/pynws/forecast.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/nws.py` & `pynws-1.8.1/src/pynws/nws.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/raw_data.py` & `pynws-1.8.1/src/pynws/raw_data.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/simple_nws.py` & `pynws-1.8.1/src/pynws/simple_nws.py`

 * *Files 3% similar despite different names*

```diff
@@ -259,24 +259,28 @@
             self._observation = obs
             self._metar_obs = [self.extract_metar(iobs) for iobs in self._observation]
         elif raise_no_data:
             raise NwsNoDataError("Observation received with no data.")
 
     async def update_forecast(self: SimpleNWS, *, raise_no_data: bool = False) -> None:
         """Update forecast."""
-        self._forecast = await self.get_gridpoints_forecast()
-        if not self.forecast and raise_no_data:
+        forecast = await self.get_gridpoints_forecast()
+        if self._filter_forecast(forecast):
+            self._forecast = forecast
+        elif raise_no_data:
             raise NwsNoDataError("Forecast received with no data.")
 
     async def update_forecast_hourly(
         self: SimpleNWS, *, raise_no_data: bool = False
     ) -> None:
         """Update forecast hourly."""
-        self._forecast_hourly = await self.get_gridpoints_forecast_hourly()
-        if not self.forecast_hourly and raise_no_data:
+        forecast_hourly = await self.get_gridpoints_forecast_hourly()
+        if self._filter_forecast(forecast_hourly):
+            self._forecast_hourly = forecast_hourly
+        elif raise_no_data:
             raise NwsNoDataError("Forecast hourly received with no data.")
 
     async def update_detailed_forecast(
         self: SimpleNWS, *, raise_no_data: bool = False
     ) -> None:
         """Update forecast.
 
@@ -438,50 +442,57 @@
             data["iconTime"] = None
             data["iconWeather"] = None
         return data
 
     @property
     def forecast(self: SimpleNWS) -> Optional[List[Dict[str, Any]]]:
         """Return forecast."""
-        return self._convert_forecast(self._forecast, self.filter_forecast)
+        forecast = self._filter_forecast(self._forecast)
+        return self._convert_forecast(forecast)
 
     @property
     def forecast_hourly(self: SimpleNWS) -> Optional[List[Dict[str, Any]]]:
         """Return forecast hourly."""
-        return self._convert_forecast(self._forecast_hourly, self.filter_forecast)
+        forecast = self._filter_forecast(self._forecast_hourly)
+        return self._convert_forecast(forecast)
 
     @property
     def detailed_forecast(self: SimpleNWS) -> Optional[DetailedForecast]:
         """Return detailed forecast.
 
         Returns:
             Optional[DetailedForecast]: Returns None if update_detailed_forecast
             hasn't been called.
         """
         return self._detailed_forecast
 
-    @staticmethod
-    def _convert_forecast(
+    def _filter_forecast(
+        self,
         input_forecast: Optional[List[Dict[str, Any]]],
-        filter_forecast: bool,
     ) -> List[Dict[str, Any]]:
-        """Converts forecast to common dict."""
         if not input_forecast:
             return []
-        forecast = []
+        if not self.filter_forecast:
+            return input_forecast
+        forecast: List[Dict[str, Any]] = []
         now = datetime.now(timezone.utc)
         for forecast_entry in input_forecast:
-            # get weather
-            if filter_forecast:
-                end_time = forecast_entry.get("endTime")
-                if not end_time:
-                    continue
-                if now > datetime.fromisoformat(end_time):
-                    continue
+            end_time = forecast_entry.get("endTime")
+            if not end_time or now > datetime.fromisoformat(end_time):
+                continue
+            forecast.append(forecast_entry)
+        return forecast
 
+    @staticmethod
+    def _convert_forecast(
+        input_forecast: List[Dict[str, Any]],
+    ) -> List[Dict[str, Any]]:
+        """Converts forecast to common dict."""
+        forecast = []
+        for forecast_entry in input_forecast:
             if (value := forecast_entry.get("temperature")) is not None:
                 forecast_entry["temperature"] = int(value)
 
             temp_unit = forecast_entry.get("temperatureUnit")
 
             for key in ("probabilityOfPrecipitation", "dewpoint", "relativeHumidity"):
                 extracted = SimpleNWS.extract_value(forecast_entry, key)
```

### Comparing `pynws-1.8.0/src/pynws/units.py` & `pynws-1.8.1/src/pynws/units.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws/urls.py` & `pynws-1.8.1/src/pynws/urls.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/src/pynws.egg-info/PKG-INFO` & `pynws-1.8.1/src/pynws.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynws
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python library to retrieve observations and forecasts from NWS/NOAA
 Author-email: Matthew Flamm <matthewhflamm0@gmail.com>
 License: MIT License
 Project-URL: Repository, https://github.com/MatthewFlamm/pynws
 Project-URL: Bug Tracker, https://github.com/MatthewFlamm/pynws/issues
 Keywords: nws,weather
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pynws-1.8.0/src/pynws.egg-info/SOURCES.txt` & `pynws-1.8.1/src/pynws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/conftest.py` & `pynws-1.8.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/alerts_active_zone.json` & `pynws-1.8.1/tests/fixtures/alerts_active_zone.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/alerts_active_zone_second.json` & `pynws-1.8.1/tests/fixtures/alerts_active_zone_second.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/detailed_forecast.json` & `pynws-1.8.1/tests/fixtures/detailed_forecast.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_forecast.json` & `pynws-1.8.1/tests/fixtures/gridpoints_forecast.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_forecast_empty.json` & `pynws-1.8.1/tests/fixtures/gridpoints_forecast_empty.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly.json` & `pynws-1.8.1/tests/fixtures/gridpoints_forecast_hourly.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_forecast_hourly_empty.json` & `pynws-1.8.1/tests/fixtures/gridpoints_forecast_hourly_empty.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_forecast_strings.json` & `pynws-1.8.1/tests/fixtures/gridpoints_forecast_strings.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/gridpoints_stations.json` & `pynws-1.8.1/tests/fixtures/gridpoints_stations.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/points.json` & `pynws-1.8.1/tests/fixtures/points.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations.json` & `pynws-1.8.1/tests/fixtures/stations_observations.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_alternate_units.json` & `pynws-1.8.1/tests/fixtures/stations_observations_alternate_units.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_empty.json` & `pynws-1.8.1/tests/fixtures/stations_observations_empty.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_latest.json` & `pynws-1.8.1/tests/fixtures/stations_observations_latest.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_metar.json` & `pynws-1.8.1/tests/fixtures/stations_observations_metar.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_metar_noparse.json` & `pynws-1.8.1/tests/fixtures/stations_observations_metar_noparse.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_missing_value.json` & `pynws-1.8.1/tests/fixtures/stations_observations_missing_value.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_multiple.json` & `pynws-1.8.1/tests/fixtures/stations_observations_multiple.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_multiple_unsorted.json` & `pynws-1.8.1/tests/fixtures/stations_observations_multiple_unsorted.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_other_unitcode.json` & `pynws-1.8.1/tests/fixtures/stations_observations_other_unitcode.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/fixtures/stations_observations_strings.json` & `pynws-1.8.1/tests/fixtures/stations_observations_strings.json`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/helpers.py` & `pynws-1.8.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/test_nws.py` & `pynws-1.8.1/tests/test_nws.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/test_raw.py` & `pynws-1.8.1/tests/test_raw.py`

 * *Files identical despite different names*

### Comparing `pynws-1.8.0/tests/test_simple_nws.py` & `pynws-1.8.1/tests/test_simple_nws.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,32 @@
     nws = SimpleNWS(*LATLON, USERID, client)
     await nws.set_station(STATION)
 
     await call_with_retry(nws.update_observation, 0, 5, retry_no_data=True)
     assert nws.observation is not None
 
 
+async def test_nws_observation_cache(aiohttp_client, mock_urls):
+    app = setup_app(
+        stations_observations=[
+            "stations_observations.json",
+            "stations_observations_noprop.json",
+        ]
+    )
+    client = await aiohttp_client(app)
+    nws = SimpleNWS(*LATLON, USERID, client)
+    await nws.set_station(STATION)
+    await nws.update_observation()
+    observation = nws.observation
+    assert observation
+
+    await nws.update_observation()
+    assert observation
+
+
 async def test_nws_observation_missing_value(aiohttp_client, mock_urls):
     app = setup_app(stations_observations="stations_observations_missing_value.json")
     client = await aiohttp_client(app)
     nws = SimpleNWS(*LATLON, USERID, client)
     await nws.set_station(STATION)
     await nws.update_observation()
     observation = nws.observation
@@ -310,14 +328,32 @@
     app = setup_app(gridpoints_forecast="gridpoints_forecast_empty.json")
     client = await aiohttp_client(app)
     nws = SimpleNWS(*LATLON, USERID, client)
     with pytest.raises(NwsNoDataError, match="Forecast received with no data"):
         await nws.update_forecast(raise_no_data=True)
 
 
+@freeze_time("2019-10-13T14:30:00-04:00")
+async def test_nws_forecast_cache(aiohttp_client, mock_urls):
+    app = setup_app(
+        gridpoints_forecast=[
+            "gridpoints_forecast.json",
+            "gridpoints_forecast_empty.json",
+        ]
+    )
+    client = await aiohttp_client(app)
+    nws = SimpleNWS(*LATLON, USERID, client)
+    await nws.update_forecast()
+    forecast = nws.forecast
+    assert forecast
+
+    await nws.update_forecast()
+    assert forecast
+
+
 @freeze_time("2019-10-14T20:30:00-04:00")
 async def test_nws_forecast_hourly_empty(aiohttp_client, mock_urls):
     app = setup_app(gridpoints_forecast_hourly="gridpoints_forecast_hourly_empty.json")
     client = await aiohttp_client(app)
     nws = SimpleNWS(*LATLON, USERID, client)
     await nws.update_forecast_hourly()
     forecast_hourly = nws.forecast_hourly
@@ -330,14 +366,31 @@
     app = setup_app(gridpoints_forecast_hourly="gridpoints_forecast_hourly_empty.json")
     client = await aiohttp_client(app)
     nws = SimpleNWS(*LATLON, USERID, client)
     with pytest.raises(NwsNoDataError, match="Forecast hourly received with no data"):
         await nws.update_forecast_hourly(raise_no_data=True)
 
 
+@freeze_time("2019-10-14T20:30:00-04:00")
+async def test_nws_forecast_hourly_cache(aiohttp_client, mock_urls):
+    app = setup_app(
+        gridpoints_forecast_hourly=[
+            "gridpoints_forecast_hourly.json",
+            "gridpoints_forecast_hourly_empty.json",
+        ]
+    )
+    client = await aiohttp_client(app)
+    nws = SimpleNWS(*LATLON, USERID, client)
+    await nws.update_forecast_hourly()
+    assert nws.forecast_hourly
+
+    await nws.update_forecast_hourly()
+    assert nws.forecast_hourly
+
+
 async def test_nws_unimplemented_retry_no_data(aiohttp_client, mock_urls):
     app = setup_app(gridpoints_forecast="gridpoints_forecast_empty.json")
     client = await aiohttp_client(app)
     nws = SimpleNWS(*LATLON, USERID, client)
     with pytest.raises(
         NotImplementedError,
         match="raise_no_data=True not implemented for update_detailed_forecast",
```

