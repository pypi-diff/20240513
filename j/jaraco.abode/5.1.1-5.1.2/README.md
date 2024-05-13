# Comparing `tmp/jaraco.abode-5.1.1.tar.gz` & `tmp/jaraco_abode-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.abode-5.1.1.tar", last modified: Sun Mar 24 01:01:03 2024, max compression
+gzip compressed data, was "jaraco_abode-5.1.2.tar", last modified: Mon May 13 01:10:43 2024, max compression
```

## Comparing `jaraco.abode-5.1.1.tar` & `jaraco_abode-5.1.2.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.682520 jaraco.abode-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.666520 jaraco.abode-5.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.666520 jaraco.abode-5.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-03-24 01:01:03.682520 jaraco.abode-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.666520 jaraco.abode-5.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.662521 jaraco.abode-5.1.1/jaraco/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.670521 jaraco.abode-5.1.1/jaraco/abode/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/automation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.670521 jaraco.abode-5.1.1/jaraco/abode/devices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/cover.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/light.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/switch.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/devices/valve.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/event_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.670521 jaraco.abode-5.1.1/jaraco/abode/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/helpers/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/helpers/events.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/helpers/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/helpers/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/socketio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/jaraco/abode/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.678521 jaraco.abode-5.1.1/jaraco.abode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11309 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-24 01:01:03.000000 jaraco.abode-5.1.1/jaraco.abode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-24 01:01:03.682520 jaraco.abode-5.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.674521 jaraco.abode-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.674521 jaraco.abode-5.1.1/tests/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/automation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 01:01:03.678521 jaraco.abode-5.1.1/tests/mock/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/door_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/door_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/glass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/hue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/ipcam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/ir_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/keypad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/pir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/power_switch_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/power_switch_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/remote_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/secure_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/siren.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/status_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/valve.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/devices/water_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/login.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/oauth_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/mock/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    20393 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_abode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_automation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13234 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_dimmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_door_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_event_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_hue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_power_switch_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_power_switch_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_secure_barrier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tests/test_valve.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-03-24 01:00:37.000000 jaraco.abode-5.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.510747 jaraco_abode-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.490747 jaraco_abode-5.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.490747 jaraco_abode-5.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-13 01:10:43.510747 jaraco_abode-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.494747 jaraco_abode-5.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.490747 jaraco_abode-5.1.2/jaraco/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.498747 jaraco_abode-5.1.2/jaraco/abode/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/automation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9979 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.502747 jaraco_abode-5.1.2/jaraco/abode/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5458 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/devices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/event_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.502747 jaraco_abode-5.1.2/jaraco/abode/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/helpers/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/helpers/events.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/helpers/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/helpers/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/socketio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/jaraco/abode/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.506747 jaraco_abode-5.1.2/jaraco.abode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 01:10:43.000000 jaraco_abode-5.1.2/jaraco.abode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 01:10:43.510747 jaraco_abode-5.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.502747 jaraco_abode-5.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.502747 jaraco_abode-5.1.2/tests/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/automation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:10:43.506747 jaraco_abode-5.1.2/tests/mock/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/door_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/door_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/glass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/ipcam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/ir_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/keypad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/pir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/power_switch_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/power_switch_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/remote_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/secure_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/siren.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/status_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/devices/water_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/oauth_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/mock/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20393 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_abode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11979 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_automation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13234 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14943 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_dimmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_door_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18433 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_event_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9382 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_hue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_power_switch_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_power_switch_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_secure_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-13 01:10:24.000000 jaraco_abode-5.1.2/tox.ini
```

### Comparing `jaraco.abode-5.1.1/.github/workflows/main.yml` & `jaraco_abode-5.1.2/.github/workflows/main.yml`

 * *Files 9% similar despite different names*

```diff
@@ -27,32 +27,34 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
-    continue-on-error: ${{ matrix.python == '3.13' }}
+    continue-on-error: ${{ matrix.python == '3.13' || (matrix.python == '3.8' || matrix.python == '3.9') && matrix.platform == 'macos-latest' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
           allow-prereleases: true
```

### Comparing `jaraco.abode-5.1.1/LICENSE` & `jaraco_abode-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/NEWS.rst` & `jaraco_abode-5.1.2/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.1.2
+======
+
+Bugfixes
+--------
+
+- Restore support for details in SocketIOException, used in socketio module. (#27)
+
+
 v5.1.1
 ======
 
 No significant changes.
 
 
 v5.1.0
```

### Comparing `jaraco.abode-5.1.1/PKG-INFO` & `jaraco_abode-5.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: jaraco.abode
-Version: 5.1.1
+Version: 5.1.2
 Summary: A library interfacing to the Abode home security system
-Home-page: https://github.com/jaraco/jaraco.abode
-Author: Wil Schrader
-Author-email: wilrader@gmail.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
+Author-email: Wil Schrader <wilrader@gmail.com>
+Maintainer-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.abode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests>=2.12.4
 Requires-Dist: lomond>=0.3.3
 Requires-Dist: colorlog>=3.0.1
 Requires-Dist: keyring
 Requires-Dist: requests_toolbelt
 Requires-Dist: jaraco.collections
@@ -26,15 +25,15 @@
 Requires-Dist: more_itertools
 Requires-Dist: importlib_resources>=5.10
 Requires-Dist: bx_py_utils
 Requires-Dist: platformdirs
 Requires-Dist: jaraco.itertools
 Requires-Dist: jaraco.functools>=3.6
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: requests_mock; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
```

### Comparing `jaraco.abode-5.1.1/README.rst` & `jaraco_abode-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/conftest.py` & `jaraco_abode-5.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/docs/api.rst` & `jaraco_abode-5.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/docs/conf.py` & `jaraco_abode-5.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/automation.py` & `jaraco_abode-5.1.2/jaraco/abode/automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/cli.py` & `jaraco_abode-5.1.2/jaraco/abode/cli.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/client.py` & `jaraco_abode-5.1.2/jaraco/abode/client.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/alarm.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/alarm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/base.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/base.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/binary_sensor.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/camera.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/cover.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/cover.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/light.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/light.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/lock.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/sensor.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/status.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/status.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/switch.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/switch.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/devices/valve.py` & `jaraco_abode-5.1.2/jaraco/abode/devices/valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/event_controller.py` & `jaraco_abode-5.1.2/jaraco/abode/event_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/helpers/errors.py` & `jaraco_abode-5.1.2/jaraco/abode/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/helpers/events.csv` & `jaraco_abode-5.1.2/jaraco/abode/helpers/events.csv`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/helpers/timeline.py` & `jaraco_abode-5.1.2/jaraco/abode/helpers/timeline.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/helpers/urls.py` & `jaraco_abode-5.1.2/jaraco/abode/helpers/urls.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/settings.py` & `jaraco_abode-5.1.2/jaraco/abode/settings.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/socketio.py` & `jaraco_abode-5.1.2/jaraco/abode/socketio.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco/abode/state.py` & `jaraco_abode-5.1.2/jaraco/abode/state.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/jaraco.abode.egg-info/PKG-INFO` & `jaraco_abode-5.1.2/jaraco.abode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: jaraco.abode
-Version: 5.1.1
+Version: 5.1.2
 Summary: A library interfacing to the Abode home security system
-Home-page: https://github.com/jaraco/jaraco.abode
-Author: Wil Schrader
-Author-email: wilrader@gmail.com
-Maintainer: Jason R. Coombs
-Maintainer-email: jaraco@jaraco.com
+Author-email: Wil Schrader <wilrader@gmail.com>
+Maintainer-email: "Jason R. Coombs" <jaraco@jaraco.com>
+Project-URL: Homepage, https://github.com/jaraco/jaraco.abode
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: requests>=2.12.4
 Requires-Dist: lomond>=0.3.3
 Requires-Dist: colorlog>=3.0.1
 Requires-Dist: keyring
 Requires-Dist: requests_toolbelt
 Requires-Dist: jaraco.collections
@@ -26,15 +25,15 @@
 Requires-Dist: more_itertools
 Requires-Dist: importlib_resources>=5.10
 Requires-Dist: bx_py_utils
 Requires-Dist: platformdirs
 Requires-Dist: jaraco.itertools
 Requires-Dist: jaraco.functools>=3.6
 Provides-Extra: testing
-Requires-Dist: pytest>=6; extra == "testing"
+Requires-Dist: pytest!=8.1.*,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-mypy; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "testing"
 Requires-Dist: requests_mock; extra == "testing"
 Requires-Dist: types-requests; extra == "testing"
```

### Comparing `jaraco.abode-5.1.1/jaraco.abode.egg-info/SOURCES.txt` & `jaraco_abode-5.1.2/jaraco.abode.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 NEWS.rst
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
-setup.cfg
 towncrier.toml
 tox.ini
 .github/dependabot.yml
 .github/workflows/main.yml
 docs/api.rst
 docs/conf.py
 docs/history.rst
```

### Comparing `jaraco.abode-5.1.1/tests/mock/__init__.py` & `jaraco_abode-5.1.2/tests/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/automation.py` & `jaraco_abode-5.1.2/tests/mock/automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/__init__.py` & `jaraco_abode-5.1.2/tests/mock/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/dimmer.py` & `jaraco_abode-5.1.2/tests/mock/devices/dimmer.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/door_contact.py` & `jaraco_abode-5.1.2/tests/mock/devices/door_contact.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/door_lock.py` & `jaraco_abode-5.1.2/tests/mock/devices/door_lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/glass.py` & `jaraco_abode-5.1.2/tests/mock/devices/glass.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/hue.py` & `jaraco_abode-5.1.2/tests/mock/devices/hue.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/ipcam.py` & `jaraco_abode-5.1.2/tests/mock/devices/ipcam.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/ir_camera.py` & `jaraco_abode-5.1.2/tests/mock/devices/ir_camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/keypad.py` & `jaraco_abode-5.1.2/tests/mock/devices/keypad.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/lm.py` & `jaraco_abode-5.1.2/tests/mock/devices/lm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/pir.py` & `jaraco_abode-5.1.2/tests/mock/devices/pir.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/power_switch_meter.py` & `jaraco_abode-5.1.2/tests/mock/devices/power_switch_meter.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/power_switch_sensor.py` & `jaraco_abode-5.1.2/tests/mock/devices/power_switch_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/remote_controller.py` & `jaraco_abode-5.1.2/tests/mock/devices/remote_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/secure_barrier.py` & `jaraco_abode-5.1.2/tests/mock/devices/secure_barrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/siren.py` & `jaraco_abode-5.1.2/tests/mock/devices/siren.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/status_display.py` & `jaraco_abode-5.1.2/tests/mock/devices/status_display.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/unknown.py` & `jaraco_abode-5.1.2/tests/mock/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/valve.py` & `jaraco_abode-5.1.2/tests/mock/devices/valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/devices/water_sensor.py` & `jaraco_abode-5.1.2/tests/mock/devices/water_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/login.py` & `jaraco_abode-5.1.2/tests/mock/login.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/panel.py` & `jaraco_abode-5.1.2/tests/mock/panel.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/mock/user.py` & `jaraco_abode-5.1.2/tests/mock/user.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_abode.py` & `jaraco_abode-5.1.2/tests/test_abode.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_alarm.py` & `jaraco_abode-5.1.2/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_automation.py` & `jaraco_abode-5.1.2/tests/test_automation.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_binary_sensor.py` & `jaraco_abode-5.1.2/tests/test_binary_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_camera.py` & `jaraco_abode-5.1.2/tests/test_camera.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_device.py` & `jaraco_abode-5.1.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_dimmer.py` & `jaraco_abode-5.1.2/tests/test_dimmer.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_door_lock.py` & `jaraco_abode-5.1.2/tests/test_door_lock.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_event_controller.py` & `jaraco_abode-5.1.2/tests/test_event_controller.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_hue.py` & `jaraco_abode-5.1.2/tests/test_hue.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_lm.py` & `jaraco_abode-5.1.2/tests/test_lm.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_power_switch_meter.py` & `jaraco_abode-5.1.2/tests/test_power_switch_meter.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_power_switch_sensor.py` & `jaraco_abode-5.1.2/tests/test_power_switch_sensor.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_secure_barrier.py` & `jaraco_abode-5.1.2/tests/test_secure_barrier.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tests/test_valve.py` & `jaraco_abode-5.1.2/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `jaraco.abode-5.1.1/tox.ini` & `jaraco_abode-5.1.2/tox.ini`

 * *Files identical despite different names*

