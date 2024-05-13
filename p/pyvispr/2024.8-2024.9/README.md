# Comparing `tmp/pyvispr-2024.8.tar.gz` & `tmp/pyvispr-2024.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvispr-2024.8.tar", last modified: Thu Apr 25 12:14:17 2024, max compression
+gzip compressed data, was "pyvispr-2024.9.tar", last modified: Tue May  7 14:02:23 2024, max compression
```

## Comparing `pyvispr-2024.8.tar` & `pyvispr-2024.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/
--rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.8/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-25 12:14:17.818999 pyvispr-2024.8/PKG-INFO
--rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.8/README-COPYRIGHT-utf8.txt
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.8/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4434 2024-04-22 09:35:02.000000 pyvispr-2024.8/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     2421 2024-04-19 15:02:26.000000 pyvispr-2024.8/documentation/wiki/description.asciidoc
--rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.8/pyproject.toml
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/
--rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.8/pyvispr/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/catalog/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/catalog/factory/
--rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_256.py
--rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_loader.py
--rwx------   0 eric      (1000) users      (984)    15998 2024-04-25 12:10:02.000000 pyvispr-2024.8/pyvispr/catalog/factory/image_viewer.py
--rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.8/pyvispr/catalog/factory/numexpr_calculator.py
--rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.8/pyvispr/catalog/factory/value.py
--rwx------   0 eric      (1000) users      (984)     5939 2024-04-21 14:27:40.000000 pyvispr-2024.8/pyvispr/catalog/factory/value_viewer.py
--rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.8/pyvispr/catalog/installer.py
--rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.8/pyvispr/catalog/parser.py
--rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.8/pyvispr/catalog/type.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.802332 pyvispr-2024.8/pyvispr/config/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/config/appearance/
--rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.8/pyvispr/config/appearance/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.8/pyvispr/config/appearance/behavior.py
--rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.8/pyvispr/config/appearance/color.py
--rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.8/pyvispr/config/appearance/geometry.py
--rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/config/path.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/constant/
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.8/pyvispr/constant/app.py
--rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.8/pyvispr/constant/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.8/pyvispr/constant/function.py
--rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.8/pyvispr/constant/path.py
--rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.8/pyvispr/constant/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.805666 pyvispr-2024.8/pyvispr/constant/widget/
--rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/constant/widget/function_header.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.8/pyvispr/constant/widget/list.py
--rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.8/pyvispr/constant/widget/node.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.808999 pyvispr-2024.8/pyvispr/extension/
--rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.8/pyvispr/extension/function.py
--rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.8/pyvispr/extension/module.py
--rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.8/pyvispr/extension/qt6.py
--rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.8/pyvispr/extension/string_.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/pyvispr/flow/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.808999 pyvispr-2024.8/pyvispr/flow/descriptive/
--rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.8/pyvispr/flow/descriptive/node.py
--rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.8/pyvispr/flow/descriptive/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.812332 pyvispr-2024.8/pyvispr/flow/functional/
--rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.8/pyvispr/flow/functional/graph.py
--rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.8/pyvispr/flow/functional/link.py
--rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.8/pyvispr/flow/functional/node_isolated.py
--rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.8/pyvispr/flow/functional/node_linked.py
--rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.8/pyvispr/flow/functional/socket.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.812332 pyvispr-2024.8/pyvispr/flow/visual/
--rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.8/pyvispr/flow/visual/graph.py
--rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.8/pyvispr/flow/visual/ii_value.py
--rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.8/pyvispr/flow/visual/link.py
--rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.8/pyvispr/flow/visual/node.py
--rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/flow/visual/socket.py
--rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.8/pyvispr/flow/visual/whiteboard.py
--rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/install.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.798999 pyvispr-2024.8/pyvispr/interface/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.815666 pyvispr-2024.8/pyvispr/interface/storage/
--rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.8/pyvispr/interface/storage/loading.py
--rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.8/pyvispr/interface/storage/stowing.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.815666 pyvispr-2024.8/pyvispr/interface/window/
--rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.8/pyvispr/interface/window/installer.py
--rwx------   0 eric      (1000) users      (984)     7880 2024-04-18 07:10:06.000000 pyvispr-2024.8/pyvispr/interface/window/runner.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr/interface/window/widget/
--rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.8/pyvispr/interface/window/widget/function_header.py
--rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list.py
--rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_file.py
--rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_function.py
--rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_module.py
--rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.8/pyvispr/interface/window/widget/list_node.py
--rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.8/pyvispr/interface/window/widget/menu.py
--rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.8/pyvispr/run.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr/runtime/
--rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.8/pyvispr/runtime/backend.py
--rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.8/pyvispr/runtime/catalog.py
--rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.8/pyvispr/runtime/socket.py
--rwx------   0 eric      (1000) users      (984)     1577 2024-04-25 12:13:54.000000 pyvispr-2024.8/pyvispr/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-04-25 12:14:17.818999 pyvispr-2024.8/pyvispr.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5492 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)     2224 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)       87 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/entry_points.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)        8 2024-04-25 12:14:17.000000 pyvispr-2024.8/pyvispr.egg-info/top_level.txt
--rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.8/requirements.txt
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-04-25 12:14:17.818999 pyvispr-2024.8/setup.cfg
--rwx------   0 eric      (1000) users      (984)     8530 2024-04-11 11:30:02.000000 pyvispr-2024.8/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.945397 pyvispr-2024.9/
+-rwx------   0 eric      (1000) users      (984)      139 2024-04-05 18:00:47.000000 pyvispr-2024.9/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5492 2024-05-07 14:02:23.945397 pyvispr-2024.9/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      642 2024-02-07 09:03:58.000000 pyvispr-2024.9/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 pyvispr-2024.9/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4434 2024-04-22 09:35:02.000000 pyvispr-2024.9/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.938731 pyvispr-2024.9/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.938731 pyvispr-2024.9/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     2421 2024-04-19 15:02:26.000000 pyvispr-2024.9/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      112 2024-02-07 08:56:45.000000 pyvispr-2024.9/pyproject.toml
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.938731 pyvispr-2024.9/pyvispr/
+-rwx------   0 eric      (1000) users      (984)     1594 2023-11-17 11:20:29.000000 pyvispr-2024.9/pyvispr/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/catalog/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/catalog/factory/
+-rwx------   0 eric      (1000) users      (984)     1715 2024-04-19 07:34:07.000000 pyvispr-2024.9/pyvispr/catalog/factory/image_256.py
+-rwx------   0 eric      (1000) users      (984)     1804 2024-01-19 10:13:27.000000 pyvispr-2024.9/pyvispr/catalog/factory/image_loader.py
+-rwx------   0 eric      (1000) users      (984)    15776 2024-05-07 13:41:30.000000 pyvispr-2024.9/pyvispr/catalog/factory/image_viewer.py
+-rwx------   0 eric      (1000) users      (984)     1975 2024-01-19 10:13:27.000000 pyvispr-2024.9/pyvispr/catalog/factory/numexpr_calculator.py
+-rwx------   0 eric      (1000) users      (984)     1818 2024-01-19 10:18:15.000000 pyvispr-2024.9/pyvispr/catalog/factory/value.py
+-rwx------   0 eric      (1000) users      (984)     5853 2024-05-07 13:41:46.000000 pyvispr-2024.9/pyvispr/catalog/factory/value_viewer.py
+-rwx------   0 eric      (1000) users      (984)     7691 2024-04-11 08:05:54.000000 pyvispr-2024.9/pyvispr/catalog/installer.py
+-rwx------   0 eric      (1000) users      (984)     4160 2024-04-19 07:40:32.000000 pyvispr-2024.9/pyvispr/catalog/parser.py
+-rwx------   0 eric      (1000) users      (984)     2226 2024-04-10 14:04:29.000000 pyvispr-2024.9/pyvispr/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/config/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/config/appearance/
+-rwx------   0 eric      (1000) users      (984)     1584 2024-04-10 13:34:33.000000 pyvispr-2024.9/pyvispr/config/appearance/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1611 2024-04-10 13:52:01.000000 pyvispr-2024.9/pyvispr/config/appearance/behavior.py
+-rwx------   0 eric      (1000) users      (984)     2662 2024-04-19 14:06:18.000000 pyvispr-2024.9/pyvispr/config/appearance/color.py
+-rwx------   0 eric      (1000) users      (984)     1727 2024-04-19 14:06:38.000000 pyvispr-2024.9/pyvispr/config/appearance/geometry.py
+-rwx------   0 eric      (1000) users      (984)     1788 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/config/path.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 14:04:29.000000 pyvispr-2024.9/pyvispr/constant/app.py
+-rwx------   0 eric      (1000) users      (984)     1961 2024-01-22 14:35:46.000000 pyvispr-2024.9/pyvispr/constant/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1654 2024-04-10 13:34:03.000000 pyvispr-2024.9/pyvispr/constant/function.py
+-rw-r--r--   0 eric      (1000) users      (984)     1618 2024-04-10 13:51:28.000000 pyvispr-2024.9/pyvispr/constant/path.py
+-rw-r--r--   0 eric      (1000) users      (984)     1610 2024-04-10 15:59:22.000000 pyvispr-2024.9/pyvispr/constant/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/constant/widget/
+-rw-r--r--   0 eric      (1000) users      (984)     1873 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/constant/widget/function_header.py
+-rw-r--r--   0 eric      (1000) users      (984)     1575 2024-04-10 13:59:48.000000 pyvispr-2024.9/pyvispr/constant/widget/list.py
+-rw-r--r--   0 eric      (1000) users      (984)     1969 2024-04-11 12:23:33.000000 pyvispr-2024.9/pyvispr/constant/widget/node.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/extension/
+-rwx------   0 eric      (1000) users      (984)    11886 2024-04-19 06:09:59.000000 pyvispr-2024.9/pyvispr/extension/function.py
+-rwx------   0 eric      (1000) users      (984)     2907 2024-04-19 07:15:15.000000 pyvispr-2024.9/pyvispr/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     1986 2024-01-19 10:18:15.000000 pyvispr-2024.9/pyvispr/extension/qt6.py
+-rwx------   0 eric      (1000) users      (984)     1723 2023-12-14 14:25:13.000000 pyvispr-2024.9/pyvispr/extension/string_.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.938731 pyvispr-2024.9/pyvispr/flow/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/flow/descriptive/
+-rwx------   0 eric      (1000) users      (984)     7948 2024-04-19 07:15:25.000000 pyvispr-2024.9/pyvispr/flow/descriptive/node.py
+-rwx------   0 eric      (1000) users      (984)     4489 2024-04-11 12:50:13.000000 pyvispr-2024.9/pyvispr/flow/descriptive/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/flow/functional/
+-rwx------   0 eric      (1000) users      (984)     4471 2024-04-19 13:44:55.000000 pyvispr-2024.9/pyvispr/flow/functional/graph.py
+-rwx------   0 eric      (1000) users      (984)     4508 2024-04-19 14:19:48.000000 pyvispr-2024.9/pyvispr/flow/functional/link.py
+-rwx------   0 eric      (1000) users      (984)    10587 2024-04-19 14:36:55.000000 pyvispr-2024.9/pyvispr/flow/functional/node_isolated.py
+-rwx------   0 eric      (1000) users      (984)     5179 2024-04-19 14:41:22.000000 pyvispr-2024.9/pyvispr/flow/functional/node_linked.py
+-rwx------   0 eric      (1000) users      (984)     2548 2024-04-19 14:19:48.000000 pyvispr-2024.9/pyvispr/flow/functional/socket.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/flow/visual/
+-rwx------   0 eric      (1000) users      (984)    18596 2024-04-19 13:37:01.000000 pyvispr-2024.9/pyvispr/flow/visual/graph.py
+-rw-r--r--   0 eric      (1000) users      (984)     1858 2024-04-10 15:51:00.000000 pyvispr-2024.9/pyvispr/flow/visual/ii_value.py
+-rwx------   0 eric      (1000) users      (984)     6200 2024-04-11 08:06:24.000000 pyvispr-2024.9/pyvispr/flow/visual/link.py
+-rwx------   0 eric      (1000) users      (984)    13289 2024-04-19 13:42:58.000000 pyvispr-2024.9/pyvispr/flow/visual/node.py
+-rwx------   0 eric      (1000) users      (984)     1879 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/flow/visual/socket.py
+-rwx------   0 eric      (1000) users      (984)     7879 2024-04-19 13:11:30.000000 pyvispr-2024.9/pyvispr/flow/visual/whiteboard.py
+-rwx------   0 eric      (1000) users      (984)     1917 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/install.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.938731 pyvispr-2024.9/pyvispr/interface/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/interface/storage/
+-rwx------   0 eric      (1000) users      (984)     3187 2024-04-19 06:39:34.000000 pyvispr-2024.9/pyvispr/interface/storage/loading.py
+-rwx------   0 eric      (1000) users      (984)     3592 2024-04-19 14:39:57.000000 pyvispr-2024.9/pyvispr/interface/storage/stowing.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.942064 pyvispr-2024.9/pyvispr/interface/window/
+-rwx------   0 eric      (1000) users      (984)    16232 2024-04-19 06:27:12.000000 pyvispr-2024.9/pyvispr/interface/window/installer.py
+-rwx------   0 eric      (1000) users      (984)     8116 2024-05-07 13:40:42.000000 pyvispr-2024.9/pyvispr/interface/window/runner.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.945397 pyvispr-2024.9/pyvispr/interface/window/widget/
+-rwx------   0 eric      (1000) users      (984)    16183 2024-04-18 07:10:09.000000 pyvispr-2024.9/pyvispr/interface/window/widget/function_header.py
+-rwx------   0 eric      (1000) users      (984)     4147 2024-04-18 07:06:06.000000 pyvispr-2024.9/pyvispr/interface/window/widget/list.py
+-rwx------   0 eric      (1000) users      (984)     2533 2024-01-16 14:25:32.000000 pyvispr-2024.9/pyvispr/interface/window/widget/list_file.py
+-rwx------   0 eric      (1000) users      (984)     2710 2024-04-18 11:56:51.000000 pyvispr-2024.9/pyvispr/interface/window/widget/list_function.py
+-rwx------   0 eric      (1000) users      (984)     1925 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/interface/window/widget/list_module.py
+-rwx------   0 eric      (1000) users      (984)     3942 2024-04-19 14:11:04.000000 pyvispr-2024.9/pyvispr/interface/window/widget/list_node.py
+-rwx------   0 eric      (1000) users      (984)     2412 2024-04-18 07:06:19.000000 pyvispr-2024.9/pyvispr/interface/window/widget/menu.py
+-rwx------   0 eric      (1000) users      (984)     1908 2024-04-11 10:07:56.000000 pyvispr-2024.9/pyvispr/run.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.945397 pyvispr-2024.9/pyvispr/runtime/
+-rw-r--r--   0 eric      (1000) users      (984)     1713 2024-04-10 14:04:53.000000 pyvispr-2024.9/pyvispr/runtime/backend.py
+-rw-r--r--   0 eric      (1000) users      (984)     1625 2024-04-10 13:44:05.000000 pyvispr-2024.9/pyvispr/runtime/catalog.py
+-rw-r--r--   0 eric      (1000) users      (984)     1718 2024-04-10 14:44:38.000000 pyvispr-2024.9/pyvispr/runtime/socket.py
+-rwx------   0 eric      (1000) users      (984)     1577 2024-05-07 13:42:27.000000 pyvispr-2024.9/pyvispr/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-07 14:02:23.945397 pyvispr-2024.9/pyvispr.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5492 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)     2224 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)       87 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/entry_points.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)        8 2024-05-07 14:02:23.000000 pyvispr-2024.9/pyvispr.egg-info/top_level.txt
+-rw-r--r--   0 eric      (1000) users      (984)      113 2024-04-17 16:13:58.000000 pyvispr-2024.9/requirements.txt
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-07 14:02:23.945397 pyvispr-2024.9/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     8308 2024-05-07 14:01:59.000000 pyvispr-2024.9/setup.py
```

### Comparing `pyvispr-2024.8/PKG-INFO` & `pyvispr-2024.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.8
+Version: 2024.9
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
```

### Comparing `pyvispr-2024.8/README-COPYRIGHT-utf8.txt` & `pyvispr-2024.9/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/README-LICENCE-utf8.txt` & `pyvispr-2024.9/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/README.rst` & `pyvispr-2024.9/README.rst`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/documentation/wiki/description.asciidoc` & `pyvispr-2024.9/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/__init__.py` & `pyvispr-2024.9/pyvispr/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/image_256.py` & `pyvispr-2024.9/pyvispr/catalog/factory/image_256.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/image_loader.py` & `pyvispr-2024.9/pyvispr/catalog/factory/image_loader.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/image_viewer.py` & `pyvispr-2024.9/pyvispr/catalog/factory/image_viewer.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,66 +25,56 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from os.path import dirname as DetermineFolder
-from os.path import expanduser as ExpandTildeBasePath
+from pathlib import Path as path_t
 
 import numpy
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
-from pyvispr.extension.qt6 import ExecuteApp, QtApp
+from pyvispr.interface.window.runner import RunnerWindow
 from pyvispr.runtime.backend import SCREEN_BACKEND
 
+DEFAULT_SAVE_EXTENSION = "png"  # lowercase
+
 _IMG_FORMAT = {
     1: qtui.QImage.Format.Format_Indexed8,
     3: qtui.QImage.Format.Format_RGB888,
     4: qtui.QImage.Format.Format_RGBA8888,
 }
 _IMG_FORMAT_AS_STR = {1: "Grayscale 8 bits", 3: "RGB 8 bits", 4: "RGBA 8 bits"}
 
-
-class _image_container(wdgt.QLabel):
-    def __init__(self, image: numpy.ndarray, depth: int, status_bar: wdgt.QStatusBar, *args, **kwargs) -> None:
-        """"""
-        wdgt.QLabel.__init__(self, *args, **kwargs)
-        self.image = image
-        self.row_width = str(self.image.shape[0]).__len__()
-        self.col_width = str(self.image.shape[1]).__len__()
-        self.scale = 1.0
-        self.status_bar = status_bar
-        self.should_color_sb = (depth > 2) and numpy.issubdtype(image.dtype, numpy.integer) and (
-            not numpy.any(image < 0)) and (not numpy.any(image > 255))
-        self.setMouseTracking(True)
-
-    def mouseMoveEvent(self, event: qtui.QMoveEvent, /) -> None:
-        """"""
-        position = event.pos()
-        if self.scale > 0.0:
-            row = int(round(position.y() / self.scale))
-            col = int(round(position.x() / self.scale))
-        else:
-            row = int(round(position.y() * ((self.image.shape[0] - 1) / (self.height() - 1))))
-            col = int(round(position.x() * ((self.image.shape[1] - 1) / (self.width() - 1))))
-        color = self.image[row, col, ...]
-        if self.should_color_sb:
-            self.status_bar.setStyleSheet(
-                f"font-weight: bold; "
-                f"background-color: rgb({color[0]}, {color[1]}, {color[2]}); "
-                f"color: rgb({255 - color[0]}, {255 - color[1]}, {255 - color[2]})")
-        self.status_bar.showMessage(f"ROWxCOL:{row:{self.row_width}}x{col:{self.col_width}} = {color}")
+# Action name {...}_action, menu text, shortcut, method name
+_MENU_ENTRIES = (
+    ("quit", "&Quit", qtui.QKeySequence.StandardKey.Quit, "close"),
+    (
+        "save",
+        "&Save",
+        qtui.QKeySequence.StandardKey.Save,
+        "SaveImage",
+    ),
+    ("copy", "&Copy", qtui.QKeySequence.StandardKey.Copy, "CopyImage"),
+    ("zoom_in", "Zoom &In (25%)", "Ctrl++", "ZoomImageIn"),
+    ("zoom_out", "Zoom &Out (25%)", "Ctrl+-", "ZoomImageOut"),
+    ("original_size", "Original Si&ze", "Ctrl+=", "RevertImageToOriginalSize"),
+    ("fit_to_window", "&Fit to Window", "Ctrl+/", "FitImageToWindow"),
+)
 
 
 def pyVisprImageViewer(image: numpy.ndarray, /) -> None:
     """"""
-    if (not isinstance(image, numpy.ndarray)) or (image.size < 1) or numpy.any(numpy.isnan(image)) or numpy.any(
-        numpy.isinf(image)):
+    if (
+        (not isinstance(image, numpy.ndarray))
+        or (image.size < 1)
+        or numpy.any(numpy.isnan(image))
+        or numpy.any(numpy.isinf(image))
+    ):
         wdgt.QMessageBox.critical(
             None,
             f"{pyVisprImageViewer.__name__}: Error",
             f"Image is empty or contains NaN or Inf.",
         )
         return
 
@@ -107,50 +97,45 @@
         wdgt.QMessageBox.critical(
             None,
             f"{pyVisprImageViewer.__name__}: Error",
             "Input must be a 2D or 3D numpy array",
         )
         return
 
-    app, should_exec = QtApp()
     viewer = viewer_t(
         image,
         width,
         height,
         depth,
-        wdgt.QApplication.activeWindow(),
     )
     viewer.show()
-    ExecuteApp(app, should_exec)
 
 
 class viewer_t(wdgt.QMainWindow):
-    DEFAULT_SAVE_EXTENSION = "png"  # lowercase
-
     def __init__(
         self,
         image: numpy.ndarray,
         width: int,
         height: int,
         depth: int,
-        wdw: wdgt.QWidget,
     ):
         """"""
-        super().__init__(wdw)
+        wdgt.QMainWindow.__init__(self, RunnerWindow())
         self.setWindowTitle("pyVispr Image Viewer")
 
-        self.quit_action = None
-        self.save_action = None
-        self.copy_action = None
-        self.zoom_in_action = None
-        self.zoom_out_action = None
-        self.original_size_action = None
-        self.fit_to_window_action = None
+        self.quit_action: qtui.QAction | None = None
+        self.save_action: qtui.QAction | None = None
+        self.copy_action: qtui.QAction | None = None
+        self.zoom_in_action: qtui.QAction | None = None
+        self.zoom_out_action: qtui.QAction | None = None
+        self.original_size_action: qtui.QAction | None = None
+        self.fit_to_window_action: qtui.QAction | None = None
+        self._CreateActions()
 
-        self.last_save_location = ExpandTildeBasePath("~")
+        self.last_save_location = path_t.home()
 
         screen_size = self.screen().availableGeometry()
         wdw_width = min(width, int(0.75 * screen_size.width()))
         wdw_height = min(height, int(0.75 * screen_size.height()))
         self.resize(wdw_width, wdw_height)
 
         min_value, max_value, mean_value, median_value = _ImageStatistics(image, depth)
@@ -188,27 +173,44 @@
         image_0_255, depth_0_255 = _NewNImage_0_255(image, min_value, max_value, depth)
         self.q_img, self.np_img = _NewQImage(image_0_255, width, height, depth_0_255)
         self.image_container.setPixmap(qtui.QPixmap.fromImage(self.q_img))
         self.fit_to_window_action.setEnabled(True)
         if not self.fit_to_window_action.isChecked():
             self.image_container.adjustSize()
 
+    def _CreateActions(self) -> None:
+        """"""
+        for action_name, entry, shortcut, method_name in _MENU_ENTRIES:
+            action = qtui.QAction(entry, self)
+            action.setShortcut(shortcut)
+            setattr(self, f"{action_name}_action", action)
+
+            method = getattr(self, method_name)
+
+            SCREEN_BACKEND.CreateMessageCanal(action, "triggered", method)
+
+        self.fit_to_window_action.setCheckable(True)
+
+    def _UpdateActions(self) -> None:
+        """"""
+        self.zoom_in_action.setEnabled(not self.fit_to_window_action.isChecked())
+        self.zoom_out_action.setEnabled(not self.fit_to_window_action.isChecked())
+        self.original_size_action.setEnabled(not self.fit_to_window_action.isChecked())
+
     def _CreateMenus(
         self,
         width,
         height,
         depth,
         min_value,
         max_value,
         mean_value,
         median_value,
     ) -> None:
         """"""
-        self._CreateActions()
-
         numpy.set_printoptions(precision=1, floatmode="fixed")
 
         menu_bar = self.menuBar()
 
         menu = wdgt.QMenu("&Viewer", self)
         menu.addAction(self.quit_action)
         menu_bar.addMenu(menu)
@@ -235,71 +237,14 @@
         menu.addAction(f"median: {median_value}")
         for action in menu.actions():
             action.setEnabled(False)
         menu_bar.addMenu(menu)
 
         self._UpdateActions()
 
-    def _CreateActions(self) -> None:
-        """"""
-        attributes = (
-            "quit",
-            "save",
-            "copy",
-            "zoom_in",
-            "zoom_out",
-            "original_size",
-            "fit_to_window",
-        )
-        entries = (
-            "&Quit",
-            "&Save",
-            "&Copy",
-            "Zoom &In (25%)",
-            "Zoom &Out (25%)",
-            "Original Si&ze",
-            "&Fit to Window",
-        )
-        shortcuts = (
-            qtui.QKeySequence.StandardKey.Quit,
-            qtui.QKeySequence.StandardKey.Save,
-            qtui.QKeySequence.StandardKey.Copy,
-            "Ctrl++",
-            "Ctrl+-",
-            "Ctrl+=",
-            "Ctrl+/",
-        )
-        Functions = (
-            self.close,
-            self.SaveImage,
-            self.CopyImage,
-            self.ZoomImageIn,
-            self.ZoomImageOut,
-            self.RevertImageToOriginalSize,
-            self.FitImageToWindow,
-        )
-        for attribute, entry, shortcut, Function in zip(
-            attributes,
-            entries,
-            shortcuts,
-            Functions,
-        ):
-            action = qtui.QAction(entry, self)
-            action.setShortcut(shortcut)
-            SCREEN_BACKEND.CreateMessageCanal(action, "triggered", Function)
-            setattr(self, f"{attribute}_action", action)
-
-        self.fit_to_window_action.setCheckable(True)
-
-    def _UpdateActions(self) -> None:
-        """"""
-        self.zoom_in_action.setEnabled(not self.fit_to_window_action.isChecked())
-        self.zoom_out_action.setEnabled(not self.fit_to_window_action.isChecked())
-        self.original_size_action.setEnabled(not self.fit_to_window_action.isChecked())
-
     def ZoomImageIn(self) -> None:
         """"""
         self._ScaleImage(1.25)
 
     def ZoomImageOut(self) -> None:
         """"""
         self._ScaleImage(0.8)
@@ -343,46 +288,93 @@
             map(
                 lambda elm: bytearray(elm).decode().lower(),
                 qtui.QImageWriter.supportedImageFormats(),
             )
         )
         supported_formats.sort()
 
-        default_save_extension = viewer_t.DEFAULT_SAVE_EXTENSION
+        default_save_extension = DEFAULT_SAVE_EXTENSION
         if default_save_extension not in supported_formats:
             default_save_extension = supported_formats[0]
-        default_save_format = _MakeImageFilterFromExtension(default_save_extension)
+        default_save_format = _NewFileFormatFilter(default_save_extension)
 
-        supported_formats = ";;".join(
-            map(_MakeImageFilterFromExtension, supported_formats)
-        )
+        supported_formats = ";;".join(map(_NewFileFormatFilter, supported_formats))
 
         filename = wdgt.QFileDialog.getSaveFileName(
             self,
             "Save Image",
-            self.last_save_location,
+            str(self.last_save_location),
             supported_formats,
             default_save_format,
         )
         if (filename is None) or (len(filename[0]) == 0):
             return
         filename = filename[0]
 
-        self.last_save_location = DetermineFolder(filename)
+        self.last_save_location = path_t(filename).parent
 
         img_writer = qtui.QImageWriter(filename)
 
         if not img_writer.write(self.q_img):
             wdgt.QMessageBox.critical(
                 self,
                 f"{pyVisprImageViewer.__name__}: Error",
                 f"Failure in saving image to '{filename}': {img_writer.errorString()}",
             )
 
 
+class _image_container(wdgt.QLabel):
+    def __init__(
+        self,
+        image: numpy.ndarray,
+        depth: int,
+        status_bar: wdgt.QStatusBar,
+        *args,
+        **kwargs,
+    ) -> None:
+        """"""
+        wdgt.QLabel.__init__(self, *args, **kwargs)
+        self.image = image
+        self.row_width = str(self.image.shape[0]).__len__()
+        self.col_width = str(self.image.shape[1]).__len__()
+        self.scale = 1.0
+        self.status_bar = status_bar
+        self.should_color_sb = (
+            (depth > 2)
+            and numpy.issubdtype(image.dtype, numpy.integer)
+            and (not numpy.any(image < 0))
+            and (not numpy.any(image > 255))
+        )
+        self.setMouseTracking(True)
+
+    def mouseMoveEvent(self, event: qtui.QMoveEvent, /) -> None:
+        """"""
+        position = event.pos()
+        if self.scale > 0.0:
+            row = int(round(position.y() / self.scale))
+            col = int(round(position.x() / self.scale))
+        else:
+            row = int(
+                round(position.y() * ((self.image.shape[0] - 1) / (self.height() - 1)))
+            )
+            col = int(
+                round(position.x() * ((self.image.shape[1] - 1) / (self.width() - 1)))
+            )
+        color = self.image[row, col, ...]
+        if self.should_color_sb:
+            self.status_bar.setStyleSheet(
+                f"font-weight: bold; "
+                f"background-color: rgb({color[0]}, {color[1]}, {color[2]}); "
+                f"color: rgb({255 - color[0]}, {255 - color[1]}, {255 - color[2]})"
+            )
+        self.status_bar.showMessage(
+            f"ROWxCOL:{row:{self.row_width}}x{col:{self.col_width}} = {color}"
+        )
+
+
 def _ImageStatistics(image: numpy.ndarray, depth: int, /) -> tuple[
     int | float | numpy.ndarray,
     int | float | numpy.ndarray,
     int | float | numpy.ndarray,
     int | float | numpy.ndarray,
 ]:
     """"""
@@ -465,10 +457,10 @@
 def _AdjustScrollBarPosition(scroll_bar: wdgt.QScrollBar, factor: float, /) -> None:
     """"""
     scroll_bar.setValue(
         int(factor * scroll_bar.value() + ((factor - 1) * scroll_bar.pageStep() / 2))
     )
 
 
-def _MakeImageFilterFromExtension(extension: str, /) -> str:
+def _NewFileFormatFilter(extension: str, /) -> str:
     """"""
     return f"{extension.upper()} Images (*.{extension})"
```

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/numexpr_calculator.py` & `pyvispr-2024.9/pyvispr/catalog/factory/numexpr_calculator.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/value.py` & `pyvispr-2024.9/pyvispr/catalog/factory/value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/factory/value_viewer.py` & `pyvispr-2024.9/pyvispr/catalog/factory/value_viewer.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,24 +35,22 @@
 
 import numpy
 import PyQt6.QtCore as core
 import PyQt6.QtGui as qtui
 import PyQt6.QtWidgets as wdgt
 from PyQt6.QtCore import QRunnable as task_base_t
 from PyQt6.QtCore import QThreadPool as thread_manager_t
-from pyvispr.extension.qt6 import ExecuteApp, QtApp
+from pyvispr.interface.window.runner import RunnerWindow
 from pyvispr.runtime.backend import SCREEN_BACKEND
 
 
 def pyVisprValueViewer(value: h.Any, /) -> None:
     """"""
-    app, should_exec = QtApp()
-    value_viewer = value_viewer_t(value, wdgt.QApplication.activeWindow())
+    value_viewer = value_viewer_t(value)
     value_viewer.show()
-    ExecuteApp(app, should_exec)
     # TODO: Solve the following error:
     #     QBasicTimer::stop: Failed. Possibly trying to stop from a different thread
     #     The code below makes it disappear, but the table is not correctly populated then.
     # if value_viewer.thread_manager is not None:
     #     value_viewer.thread_manager.waitForDone()
     # Test also somewhere (not here though; it does not work):
     # value_viewer.thread_manager.moveToThread(wdgt.QApplication.instance().thread())
@@ -110,17 +108,17 @@
 
         self.viewer.setEnabled(True)
 
         self.value = None
 
 
 class value_viewer_t(wdgt.QMainWindow):
-    def __init__(self, value: h.Any, wdw: wdgt.QWidget, /) -> None:
+    def __init__(self, value: h.Any, /) -> None:
         """"""
-        super().__init__(wdw)
+        wdgt.QMainWindow.__init__(self, RunnerWindow())
 
         try:
             as_array = numpy.array(value)
         except:
             as_array = None
         if (
             (as_array is not None)
```

### Comparing `pyvispr-2024.8/pyvispr/catalog/installer.py` & `pyvispr-2024.9/pyvispr/catalog/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/parser.py` & `pyvispr-2024.9/pyvispr/catalog/parser.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/catalog/type.py` & `pyvispr-2024.9/pyvispr/catalog/type.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/config/appearance/backend.py` & `pyvispr-2024.9/pyvispr/config/appearance/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/config/appearance/behavior.py` & `pyvispr-2024.9/pyvispr/config/appearance/behavior.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/config/appearance/color.py` & `pyvispr-2024.9/pyvispr/config/appearance/color.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/config/appearance/geometry.py` & `pyvispr-2024.9/pyvispr/config/appearance/geometry.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/config/path.py` & `pyvispr-2024.9/pyvispr/config/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/app.py` & `pyvispr-2024.9/pyvispr/constant/app.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/catalog.py` & `pyvispr-2024.9/pyvispr/constant/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/function.py` & `pyvispr-2024.9/pyvispr/constant/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/path.py` & `pyvispr-2024.9/pyvispr/constant/path.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/socket.py` & `pyvispr-2024.9/pyvispr/constant/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/widget/function_header.py` & `pyvispr-2024.9/pyvispr/constant/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/widget/list.py` & `pyvispr-2024.9/pyvispr/constant/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/constant/widget/node.py` & `pyvispr-2024.9/pyvispr/constant/widget/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/extension/function.py` & `pyvispr-2024.9/pyvispr/extension/function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/extension/module.py` & `pyvispr-2024.9/pyvispr/extension/module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/extension/qt6.py` & `pyvispr-2024.9/pyvispr/extension/qt6.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/extension/string_.py` & `pyvispr-2024.9/pyvispr/extension/string_.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/descriptive/node.py` & `pyvispr-2024.9/pyvispr/flow/descriptive/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/descriptive/socket.py` & `pyvispr-2024.9/pyvispr/flow/descriptive/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/functional/graph.py` & `pyvispr-2024.9/pyvispr/flow/functional/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/functional/link.py` & `pyvispr-2024.9/pyvispr/flow/functional/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/functional/node_isolated.py` & `pyvispr-2024.9/pyvispr/flow/functional/node_isolated.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/functional/node_linked.py` & `pyvispr-2024.9/pyvispr/flow/functional/node_linked.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/functional/socket.py` & `pyvispr-2024.9/pyvispr/flow/functional/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/graph.py` & `pyvispr-2024.9/pyvispr/flow/visual/graph.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/ii_value.py` & `pyvispr-2024.9/pyvispr/flow/visual/ii_value.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/link.py` & `pyvispr-2024.9/pyvispr/flow/visual/link.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/node.py` & `pyvispr-2024.9/pyvispr/flow/visual/node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/socket.py` & `pyvispr-2024.9/pyvispr/flow/visual/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/flow/visual/whiteboard.py` & `pyvispr-2024.9/pyvispr/flow/visual/whiteboard.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/install.py` & `pyvispr-2024.9/pyvispr/install.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/storage/loading.py` & `pyvispr-2024.9/pyvispr/interface/storage/loading.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/storage/stowing.py` & `pyvispr-2024.9/pyvispr/interface/storage/stowing.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/installer.py` & `pyvispr-2024.9/pyvispr/interface/window/installer.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/runner.py` & `pyvispr-2024.9/pyvispr/interface/window/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -203,14 +203,23 @@
             cast(wdgt.QWidget, self),
             "About Workflow",
             f"Nodes:{self.whiteboard.graph.nodes.__len__()}/{self.whiteboard.graph.functional.__len__()}\n"
             f"Links:{self.whiteboard.graph.links.__len__()}",
         )
 
 
+def RunnerWindow() -> runner_wdw_t:
+    """"""
+    for widget in wdgt.QApplication.topLevelWidgets():
+        if isinstance(widget, runner_wdw_t):
+            return widget
+
+    raise RuntimeError(f"No runner window currently open.")
+
+
 def _AddMenu(
     name: str,
     entries: tuple,
     parent_menu: wdgt.QMenuBar | wdgt.QMenu | None,
     parent_widget: wdgt.QWidget,
     /,
 ) -> wdgt.QMenu:
```

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/function_header.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/function_header.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/list.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/list.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/list_file.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/list_file.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/list_function.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/list_function.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/list_module.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/list_module.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/list_node.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/list_node.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/interface/window/widget/menu.py` & `pyvispr-2024.9/pyvispr/interface/window/widget/menu.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/run.py` & `pyvispr-2024.9/pyvispr/run.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/runtime/backend.py` & `pyvispr-2024.9/pyvispr/runtime/backend.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/runtime/catalog.py` & `pyvispr-2024.9/pyvispr/runtime/catalog.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/runtime/socket.py` & `pyvispr-2024.9/pyvispr/runtime/socket.py`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/pyvispr/version.py` & `pyvispr-2024.9/pyvispr/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.8"
+__version__ = "2024.9"
```

### Comparing `pyvispr-2024.8/pyvispr.egg-info/PKG-INFO` & `pyvispr-2024.9/pyvispr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvispr
-Version: 2024.8
+Version: 2024.9
 Summary: Visual Programming App for Python
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/pyvispr//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/pyvispr/
```

### Comparing `pyvispr-2024.8/pyvispr.egg-info/SOURCES.txt` & `pyvispr-2024.9/pyvispr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyvispr-2024.8/setup.py` & `pyvispr-2024.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,28 +113,25 @@
                 return folder / DESCRIPTION["IMPORT_NAME"]
         return None
 
     def run(self) -> None:
         """"""
         install_base_t.run(self)
 
-        if DESCRIPTION["CONFIG_FOLDER"] != "None":
-            config_folder = fldr.user_config_path(
-                appname=DESCRIPTION["CONFIG_FOLDER"], ensure_exists=True
-            )
-        else:
-            config_folder = None
         installation_folder = install_t.InstallationFolder()
         if installation_folder is None:
-            raise RuntimeError("Setup process cannot determine the package "
-                               "installation folder.")
+            return
 
+        config_folder = fldr.user_config_path(
+            appname=DESCRIPTION["CONFIG_FOLDER"], ensure_exists=True
+        )
         if config_folder is None:
             raise RuntimeError("Setup process cannot create the package "
                                "config folder.")
+
         catalog_folder = config_folder / "catalog"
         for node in (installation_folder / "catalog" / "factory").glob("*.py"):
             now = date_time_t.now().isoformat(sep="-", timespec="microseconds")
             now = "".join(filter(str.isdigit, now))
             found_s = catalog_folder.glob(f"{node.stem}_[0-9][0-9]*.py")
             for found in found_s:
                 if found.is_symlink():
```

