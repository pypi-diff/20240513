# Comparing `tmp/dash_express_components-0.0.92.tar.gz` & `tmp/dash_express_components-0.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express_components-0.0.92.tar", last modified: Wed May  1 15:17:16 2024, max compression
+gzip compressed data, was "dash_express_components-0.0.94.tar", last modified: Mon May 13 15:06:47 2024, max compression
```

## Comparing `dash_express_components-0.0.92.tar` & `dash_express_components-0.0.94.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:17:16.534504 dash_express_components-0.0.92/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 15:16:08.000000 dash_express_components-0.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-01 15:16:08.000000 dash_express_components-0.0.92/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-01 15:17:16.534504 dash_express_components-0.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-01 15:16:08.000000 dash_express_components-0.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:17:16.534504 dash_express_components-0.0.92/dash_express_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/AggrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/AsType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/BarCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/BinTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/CategoryLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/CombinecatTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/ConfigReceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/CoreGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/DropnaTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/EvalTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/FilterIqrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/GroupedSample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/HistogramLine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Localstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/MeltTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/MetaCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/PlotterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/RenameTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/ScatterMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/StrSplitTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/SubComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/Violin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/WideToLong.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/ZerosToNanTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/async-excel.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/async-excel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   711489 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/dash_express_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/dash_express_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    91991 2024-05-01 15:17:15.000000 dash_express_components-0.0.92/dash_express_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-01 15:17:14.000000 dash_express_components-0.0.92/dash_express_components/package-info.json
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-01 15:17:13.000000 dash_express_components-0.0.92/dash_express_components/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 15:17:16.534504 dash_express_components-0.0.92/dash_express_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-01 15:17:16.000000 dash_express_components-0.0.92/dash_express_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-01 15:17:16.000000 dash_express_components-0.0.92/dash_express_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 15:17:16.000000 dash_express_components-0.0.92/dash_express_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 15:17:16.000000 dash_express_components-0.0.92/dash_express_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 15:17:16.000000 dash_express_components-0.0.92/dash_express_components.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-01 15:16:08.000000 dash_express_components-0.0.92/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 15:17:16.534504 dash_express_components-0.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-01 15:16:08.000000 dash_express_components-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:06:47.255476 dash_express_components-0.0.94/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:05:39.000000 dash_express_components-0.0.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-13 15:05:39.000000 dash_express_components-0.0.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-13 15:06:47.255476 dash_express_components-0.0.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-13 15:05:39.000000 dash_express_components-0.0.94/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:06:47.255476 dash_express_components-0.0.94/dash_express_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/AggrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/AsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/BarCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/BinTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/CategoryLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/CombinecatTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/ConfigReceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/CoreGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/DropnaTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/EvalTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/FilterIqrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/GroupedSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/HistogramLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Localstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/MeltTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/MetaCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/PlotterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/RenameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/ScatterMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/StrSplitTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/SubComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/Violin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/WideToLong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/ZerosToNanTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/async-excel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/async-excel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   711576 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/dash_express_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/dash_express_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    91991 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 15:06:45.000000 dash_express_components-0.0.94/dash_express_components/package-info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-05-13 15:06:44.000000 dash_express_components-0.0.94/dash_express_components/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:06:47.255476 dash_express_components-0.0.94/dash_express_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-13 15:06:47.000000 dash_express_components-0.0.94/dash_express_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 15:06:46.000000 dash_express_components-0.0.94/dash_express_components.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-13 15:05:39.000000 dash_express_components-0.0.94/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:06:47.255476 dash_express_components-0.0.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 15:05:39.000000 dash_express_components-0.0.94/setup.py
```

### Comparing `dash_express_components-0.0.92/PKG-INFO` & `dash_express_components-0.0.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_express_components
-Version: 0.0.92
+Version: 0.0.94
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.92/README.md` & `dash_express_components-0.0.94/README.md`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/AggrTransform.py` & `dash_express_components-0.0.94/dash_express_components/AggrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/AsType.py` & `dash_express_components-0.0.94/dash_express_components/AsType.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Bar.py` & `dash_express_components-0.0.94/dash_express_components/Bar.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/BarCount.py` & `dash_express_components-0.0.94/dash_express_components/BarCount.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Base.py` & `dash_express_components-0.0.94/dash_express_components/Base.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/BinTransform.py` & `dash_express_components-0.0.94/dash_express_components/BinTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Box.py` & `dash_express_components-0.0.94/dash_express_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/CategoryLookup.py` & `dash_express_components-0.0.94/dash_express_components/CategoryLookup.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/CombinecatTransform.py` & `dash_express_components-0.0.94/dash_express_components/CombinecatTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/ConfigReceiver.py` & `dash_express_components-0.0.94/dash_express_components/ConfigReceiver.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Configurator.py` & `dash_express_components-0.0.94/dash_express_components/Configurator.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/CoreGraph.py` & `dash_express_components-0.0.94/dash_express_components/CoreGraph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/DropnaTransform.py` & `dash_express_components-0.0.94/dash_express_components/DropnaTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/EvalTransform.py` & `dash_express_components-0.0.94/dash_express_components/EvalTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Filter.py` & `dash_express_components-0.0.94/dash_express_components/Filter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/FilterIqrTransform.py` & `dash_express_components-0.0.94/dash_express_components/FilterIqrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Graph.py` & `dash_express_components-0.0.94/dash_express_components/Graph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/GroupedSample.py` & `dash_express_components-0.0.94/dash_express_components/GroupedSample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/HistogramLine.py` & `dash_express_components-0.0.94/dash_express_components/HistogramLine.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Imshow.py` & `dash_express_components-0.0.94/dash_express_components/Imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Localstore.py` & `dash_express_components-0.0.94/dash_express_components/Localstore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/MeltTransform.py` & `dash_express_components-0.0.94/dash_express_components/MeltTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/MetaCheck.py` & `dash_express_components-0.0.94/dash_express_components/MetaCheck.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Parameterize.py` & `dash_express_components-0.0.94/dash_express_components/Parameterize.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Plotter.py` & `dash_express_components-0.0.94/dash_express_components/Plotter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/PlotterBase.py` & `dash_express_components-0.0.94/dash_express_components/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Probability.py` & `dash_express_components-0.0.94/dash_express_components/Probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/RenameTransform.py` & `dash_express_components-0.0.94/dash_express_components/RenameTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Scatter.py` & `dash_express_components-0.0.94/dash_express_components/Scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/ScatterMatrix.py` & `dash_express_components-0.0.94/dash_express_components/ScatterMatrix.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/StrSplitTransform.py` & `dash_express_components-0.0.94/dash_express_components/StrSplitTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/SubComponentBase.py` & `dash_express_components-0.0.94/dash_express_components/SubComponentBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Table.py` & `dash_express_components-0.0.94/dash_express_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Transform.py` & `dash_express_components-0.0.94/dash_express_components/Transform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/Violin.py` & `dash_express_components-0.0.94/dash_express_components/Violin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/WideToLong.py` & `dash_express_components-0.0.94/dash_express_components/WideToLong.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/ZerosToNanTransform.py` & `dash_express_components-0.0.94/dash_express_components/ZerosToNanTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/__init__.py` & `dash_express_components-0.0.94/dash_express_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/_imports_.py` & `dash_express_components-0.0.94/dash_express_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/async-excel.js` & `dash_express_components-0.0.94/dash_express_components/async-excel.js`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/dash_express_components.min.js` & `dash_express_components-0.0.94/dash_express_components/dash_express_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(l()),
                 n = c(e);
             if (!t) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_92m1714576616"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v0_0_94m1715612787"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     var u = window.webpackJsonpdash_express_components = window.webpackJsonpdash_express_components || [],
         s = u.push.bind(u);
     u.push = t, u = u.slice();
     for (var f = 0; f < u.length; f++) t(u[f]);
     var p = s;
@@ -14620,15 +14620,15 @@
                             var r = {
                                 filterIndex: o,
                                 selectedColumn: t[o].col,
                                 selectedType: "type" in n[t[o].col] ? n[t[o].col].type : "",
                                 filterType: t[o].type,
                                 filterNumber: t[o].value
                             };
-                            "categorical" === n[t[o].col].type && (r.selectedCategories = t[o].value, r.manualCategories = t[o].value.join("\n"), "large" in n[t[o].col] && n[t[o].col].large ? r.categoryOptionsLarge = !0 : (r.categoryOptionsLarge = !1, r.categoryOptions = te(n[t[o].col].cat.map((function(e) {
+                            "categorical" === n[t[o].col].type && (r.selectedCategories = t[o].value, Array.isArray(t[o].value) ? r.manualCategories = t[o].value.join("\n") : "string" == typeof t[o].value && (r.manualCategories = t[o].value), "large" in n[t[o].col] && n[t[o].col].large ? r.categoryOptionsLarge = !0 : (r.categoryOptionsLarge = !1, r.categoryOptions = te(n[t[o].col].cat.map((function(e) {
                                 return {
                                     label: String(e),
                                     value: e
                                 }
                             }))))), e.setState(r, (function() {
                                 e.handleShow()
                             }))
```

### Comparing `dash_express_components-0.0.92/dash_express_components/metadata.json` & `dash_express_components-0.0.94/dash_express_components/metadata.json`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/dash_express_components/package-info.json` & `dash_express_components-0.0.94/dash_express_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.94'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.92"
+    "version": "0.0.94"
 }
```

### Comparing `dash_express_components-0.0.92/dash_express_components/utils.py` & `dash_express_components-0.0.94/dash_express_components/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,16 @@
 
 def get_plot(inputDataFrame, config, apply_parameterization=True, compute_types=["custom", "dask", "mongodf", "pyspark"], meta="compute"):
     errorResult = "Empty plot"
     import pandas as _pd
     import numpy as _np
     import plotly.express as _px
     import plotly.graph_objects as _go
+    from . import plottypes
+    from . import transformationtypes
 
     if meta == "compute":
         meta = get_meta_if_possible(inputDataFrame)
     if meta == False:
         meta = None
```

### Comparing `dash_express_components-0.0.92/dash_express_components.egg-info/PKG-INFO` & `dash_express_components-0.0.94/dash_express_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-express-components
-Version: 0.0.92
+Version: 0.0.94
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.92/dash_express_components.egg-info/SOURCES.txt` & `dash_express_components-0.0.94/dash_express_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.92/package.json` & `dash_express_components-0.0.94/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.94'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.92"
+    "version": "0.0.94"
 }
```

### Comparing `dash_express_components-0.0.92/setup.py` & `dash_express_components-0.0.94/setup.py`

 * *Files identical despite different names*

