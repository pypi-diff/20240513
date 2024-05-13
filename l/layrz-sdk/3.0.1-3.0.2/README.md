# Comparing `tmp/layrz_sdk-3.0.1.tar.gz` & `tmp/layrz_sdk-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layrz_sdk-3.0.1.tar", last modified: Sat May 11 19:57:07 2024, max compression
+gzip compressed data, was "layrz_sdk-3.0.2.tar", last modified: Mon May 13 14:50:15 2024, max compression
```

## Comparing `layrz_sdk-3.0.1.tar` & `layrz_sdk-3.0.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/
--rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      628 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.351812 layrz_sdk-3.0.1/layrz_sdk/
--rw-rw-r--   0 root         (0) root         (0)       28 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.351812 layrz_sdk-3.0.1/layrz_sdk/entities/
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.355812 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/
--rw-rw-r--   0 root         (0) root         (0)      215 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      566 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/request.py
--rw-rw-r--   0 root         (0) root         (0)      586 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/response.py
--rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/result.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/service.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.355812 layrz_sdk-3.0.1/layrz_sdk/entities/cases/
--rw-rw-r--   0 root         (0) root         (0)      135 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/case.py
--rw-rw-r--   0 root         (0) root         (0)      902 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/comment.py
--rw-rw-r--   0 root         (0) root         (0)      629 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/cases/trigger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/charts/
--rw-rw-r--   0 root         (0) root         (0)      753 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      438 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/alignment.py
--rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/bar.py
--rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/column.py
--rw-rw-r--   0 root         (0) root         (0)      514 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/configuration.py
--rw-rw-r--   0 root         (0) root         (0)      447 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/data_type.py
--rw-rw-r--   0 root         (0) root         (0)      558 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)      995 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/html.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/line.py
--rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/map.py
--rw-rw-r--   0 root         (0) root         (0)      811 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/number.py
--rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/pie.py
--rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/radar.py
--rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/radial_bar.py
--rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/scatter.py
--rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie.py
--rw-rw-r--   0 root         (0) root         (0)      463 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie_type.py
--rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/table.py
--rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/charts/timeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/
--rw-rw-r--   0 root         (0) root         (0)      126 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/checkpoint.py
--rw-rw-r--   0 root         (0) root         (0)      653 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/geofence.py
--rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/waypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/events/
--rw-rw-r--   0 root         (0) root         (0)       49 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/events/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/events/event.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/
--rw-rw-r--   0 root         (0) root         (0)       66 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      467 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/formatting/text_align.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/general/
--rw-rw-r--   0 root         (0) root         (0)      218 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/asset.py
--rw-rw-r--   0 root         (0) root         (0)      569 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/asset_operation_mode.py
--rw-rw-r--   0 root         (0) root         (0)      606 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/custom_field.py
--rw-rw-r--   0 root         (0) root         (0)      973 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/device.py
--rw-rw-r--   0 root         (0) root         (0)      615 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/sensor.py
--rw-rw-r--   0 root         (0) root         (0)      527 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/general/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.359812 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/
--rw-rw-r--   0 root         (0) root         (0)       61 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/repcom/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/entities/reports/
--rw-rw-r--   0 root         (0) root         (0)      249 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/col.py
--rw-rw-r--   0 root         (0) root         (0)      442 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/format.py
--rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/header.py
--rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/page.py
--rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/report.py
--rw-rw-r--   0 root         (0) root         (0)      881 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/reports/row.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/
--rw-rw-r--   0 root         (0) root         (0)       87 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      789 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/message.py
--rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/position.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/helpers/
--rw-rw-r--   0 root         (0) root         (0)       72 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/helpers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/helpers/color.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk/lcl/
--rw-rw-r--   0 root         (0) root         (0)       67 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/lcl/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    22683 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/layrz_sdk/lcl/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/layrz_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1458 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2523 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-11 19:57:07.000000 layrz_sdk-3.0.1/layrz_sdk.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-11 19:57:07.363812 layrz_sdk-3.0.1/tests/
--rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-11 19:56:16.000000 layrz_sdk-3.0.1/tests/test_lcl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/
+-rw-rw-r--   0 root         (0) root         (0)     1057 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      628 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/entities/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.311596 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/
+-rw-rw-r--   0 root         (0) root         (0)      215 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      566 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/request.py
+-rw-rw-r--   0 root         (0) root         (0)      586 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/response.py
+-rw-rw-r--   0 root         (0) root         (0)     1291 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/result.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/service.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.315596 layrz_sdk-3.0.2/layrz_sdk/entities/cases/
+-rw-rw-r--   0 root         (0) root         (0)      135 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/case.py
+-rw-rw-r--   0 root         (0) root         (0)      902 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/comment.py
+-rw-rw-r--   0 root         (0) root         (0)      629 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/cases/trigger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.315596 layrz_sdk-3.0.2/layrz_sdk/entities/charts/
+-rw-rw-r--   0 root         (0) root         (0)      753 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      438 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/alignment.py
+-rw-rw-r--   0 root         (0) root         (0)     3867 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4928 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/column.py
+-rw-rw-r--   0 root         (0) root         (0)      514 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)      447 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/data_type.py
+-rw-rw-r--   0 root         (0) root         (0)      558 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)      995 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/html.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/line.py
+-rw-rw-r--   0 root         (0) root         (0)     4230 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/map.py
+-rw-rw-r--   0 root         (0) root         (0)      811 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/number.py
+-rw-rw-r--   0 root         (0) root         (0)     2972 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/pie.py
+-rw-rw-r--   0 root         (0) root         (0)     3155 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/radar.py
+-rw-rw-r--   0 root         (0) root         (0)     3011 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/radial_bar.py
+-rw-rw-r--   0 root         (0) root         (0)     4871 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/scatter.py
+-rw-rw-r--   0 root         (0) root         (0)     1509 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie.py
+-rw-rw-r--   0 root         (0) root         (0)      463 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie_type.py
+-rw-rw-r--   0 root         (0) root         (0)     1344 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/table.py
+-rw-rw-r--   0 root         (0) root         (0)     3985 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/charts/timeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/
+-rw-rw-r--   0 root         (0) root         (0)      126 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1040 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/checkpoint.py
+-rw-rw-r--   0 root         (0) root         (0)      653 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/geofence.py
+-rw-rw-r--   0 root         (0) root         (0)     1236 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/waypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/events/
+-rw-rw-r--   0 root         (0) root         (0)       49 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/events/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1175 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/events/event.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/
+-rw-rw-r--   0 root         (0) root         (0)       66 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      467 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/formatting/text_align.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/general/
+-rw-rw-r--   0 root         (0) root         (0)      218 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1786 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/asset.py
+-rw-rw-r--   0 root         (0) root         (0)      569 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/asset_operation_mode.py
+-rw-rw-r--   0 root         (0) root         (0)      606 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/custom_field.py
+-rw-rw-r--   0 root         (0) root         (0)      973 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/device.py
+-rw-rw-r--   0 root         (0) root         (0)      615 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/sensor.py
+-rw-rw-r--   0 root         (0) root         (0)      527 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/general/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.319596 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1461 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/repcom/transaction.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/entities/reports/
+-rw-rw-r--   0 root         (0) root         (0)      249 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1961 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/col.py
+-rw-rw-r--   0 root         (0) root         (0)      442 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/format.py
+-rw-rw-r--   0 root         (0) root         (0)     1408 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/header.py
+-rw-rw-r--   0 root         (0) root         (0)     1574 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/page.py
+-rw-rw-r--   0 root         (0) root         (0)     6444 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/report.py
+-rw-rw-r--   0 root         (0) root         (0)      881 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/reports/row.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/
+-rw-rw-r--   0 root         (0) root         (0)       87 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      789 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/message.py
+-rw-rw-r--   0 root         (0) root         (0)     1327 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/position.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/helpers/
+-rw-rw-r--   0 root         (0) root         (0)       72 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/helpers/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1102 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/helpers/color.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk/lcl/
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/lcl/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    22987 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/layrz_sdk/lcl/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/layrz_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1458 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-13 14:50:15.000000 layrz_sdk-3.0.2/layrz_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     7589 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 14:50:15.323596 layrz_sdk-3.0.2/tests/
+-rw-rw-r--   0 root         (0) root         (0)    28784 2024-05-13 14:49:19.000000 layrz_sdk-3.0.2/tests/test_lcl.py
```

### Comparing `layrz_sdk-3.0.1/LICENSE` & `layrz_sdk-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/PKG-INFO` & `layrz_sdk-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.1/README.md` & `layrz_sdk-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/__init__.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/request.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/request.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/response.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/response.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/result.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/result.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/service.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/service.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/broadcasts/status.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/broadcasts/status.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/cases/case.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/cases/case.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/cases/comment.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/cases/comment.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/cases/trigger.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/cases/trigger.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/__init__.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/bar.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/column.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/column.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/configuration.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/configuration.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/exceptions.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/exceptions.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/html.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/html.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/line.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/line.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/map.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/map.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/number.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/number.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/pie.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/pie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/radar.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/radar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/radial_bar.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/radial_bar.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/scatter.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/scatter.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/serie.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/serie.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/table.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/table.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/charts/timeline.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/charts/timeline.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/checkpoint.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/checkpoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/geofence.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/geofence.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/checkpoints/waypoint.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/checkpoints/waypoint.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/events/event.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/events/event.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/asset.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/asset.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/asset_operation_mode.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/asset_operation_mode.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/custom_field.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/custom_field.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/device.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/device.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/sensor.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/sensor.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/general/user.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/general/user.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/repcom/transaction.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/repcom/transaction.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/reports/col.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/reports/col.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/reports/header.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/reports/header.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/reports/page.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/reports/page.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/reports/report.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/reports/report.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/reports/row.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/reports/row.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/message.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/message.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/entities/telemetry/position.py` & `layrz_sdk-3.0.2/layrz_sdk/entities/telemetry/position.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/helpers/color.py` & `layrz_sdk-3.0.2/layrz_sdk/helpers/color.py`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/layrz_sdk/lcl/core.py` & `layrz_sdk-3.0.2/layrz_sdk/lcl/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         'NOT': self.NOT,
         'CONTAINS': self.CONTAINS,
         'STARTS_WITH': self.STARTS_WITH,
         'ENDS_WITH': self.ENDS_WITH,
         'PRIMARY_DEVICE': self.PRIMARY_DEVICE,
         'SUBSTRING': self.SUBSTRING,
         'UNIX_TO_STR': self.UNIX_TO_STR,
+        'VERSION': self.VERSION,
       }
       global_functions.update(additional_globals)
 
       import json
       result = json.dumps(eval(self._script, global_functions, local_variables))  # pylint: disable=eval-used
 
       return result
@@ -612,15 +613,15 @@
     return self._asset_constants.get('timeElapsed', 0)
 
   def IF(self, *args: list[Any]) -> Any:
     """ IF Function """
     if len(args) != 3:
       return INVALID_NUMBER_OF_PARAMS.format(expected=3, received=len(args))
 
-    if args[0] is None or args[1] is None or args[2] is None:
+    if args[0] is None:
       return None
 
     return args[1] if args[0] else args[2]
 
   def NOW(self, *args: list[Any]) -> float:  # pylint: disable=unused-argument
     """ NOW Function """
     import zoneinfo
@@ -757,7 +758,17 @@
       except zoneinfo.ZoneInfoNotFoundError:
         tz = zoneinfo.ZoneInfo('UTC')
 
     return datetime\
           .fromtimestamp(int(args[0]), tz=zoneinfo.ZoneInfo('UTC'))\
           .astimezone(tz)\
           .strftime(args[1])
+
+  def VERSION(self, *args: list[Any]) -> str:
+    """ VERSION function """
+    if len(args) > 0:
+      return INVALID_NUMBER_OF_PARAMS.format(expected=0, received=len(args))
+
+    import importlib.metadata
+    version = importlib.metadata.version('layrz_sdk')
+
+    return f'LCL {version} - Layrz SDK Runtime'
```

### Comparing `layrz_sdk-3.0.1/layrz_sdk.egg-info/PKG-INFO` & `layrz_sdk-3.0.2/layrz_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layrz-sdk
-Version: 3.0.1
+Version: 3.0.2
 Summary: Layrz SDK for Python
 Author-email: "Golden M, Inc." <software@goldenm.com>
 Maintainer-email: Kenny Mochizuki <kenny@goldenm.com>, Luis Reyes <lreyes@goldenm.com>, Kasen Li <kli@goldenm.com>
 License: MIT License
 Project-URL: Repository, https://github.com/goldenm-software/layrz-sdk
 Project-URL: Changelog, https://github.com/goldenm-software/layrz-sdk/blob/main/CHANGELOG.md
 Keywords: sdk,goldenm,lcl,layrz compute language,layrz
```

### Comparing `layrz_sdk-3.0.1/layrz_sdk.egg-info/SOURCES.txt` & `layrz_sdk-3.0.2/layrz_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layrz_sdk-3.0.1/pyproject.toml` & `layrz_sdk-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "layrz-sdk"
-version = "3.0.1"
+version = "3.0.2"
 description = "Layrz SDK for Python"
 authors = [
   {name = "Golden M, Inc.", email = "software@goldenm.com"}
 ]
 requires-python = ">=3.10"
 
 maintainers = [
```

### Comparing `layrz_sdk-3.0.1/tests/test_lcl.py` & `layrz_sdk-3.0.2/tests/test_lcl.py`

 * *Files identical despite different names*

