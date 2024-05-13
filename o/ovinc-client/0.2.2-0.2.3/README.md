# Comparing `tmp/ovinc_client-0.2.2.tar.gz` & `tmp/ovinc_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovinc_client-0.2.2.tar", last modified: Wed May  8 03:15:49 2024, max compression
+gzip compressed data, was "ovinc_client-0.2.3.tar", last modified: Mon May 13 11:17:03 2024, max compression
```

## Comparing `ovinc_client-0.2.2.tar` & `ovinc_client-0.2.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.730029 ovinc_client-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-08 03:15:49.730029 ovinc_client-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.722030 ovinc_client-0.2.2/ovinc_client/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.722030 ovinc_client-0.2.2/ovinc_client/account/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.726029 ovinc_client-0.2.2/ovinc_client/account/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/account/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.726029 ovinc_client-0.2.2/ovinc_client/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/components/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/components/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/components/notice.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/components/tcaptcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.726029 ovinc_client-0.2.2/ovinc_client/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/paginations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/core/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.730029 ovinc_client-0.2.2/ovinc_client/trace/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/exporters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/instrumentors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/ovinc_client/trace/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 03:15:49.730029 ovinc_client-0.2.2/ovinc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-08 03:15:49.000000 ovinc_client-0.2.2/ovinc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-08 03:15:49.000000 ovinc_client-0.2.2/ovinc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 03:15:49.000000 ovinc_client-0.2.2/ovinc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-08 03:15:49.000000 ovinc_client-0.2.2/ovinc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 03:15:49.000000 ovinc_client-0.2.2/ovinc_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 03:15:49.730029 ovinc_client-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-08 03:15:40.000000 ovinc_client-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.584232 ovinc_client-0.2.3/ovinc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.588232 ovinc_client-0.2.3/ovinc_client/account/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.588232 ovinc_client-0.2.3/ovinc_client/account/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/account/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.588232 ovinc_client-0.2.3/ovinc_client/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/components/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/components/notice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/components/tcaptcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/ovinc_client/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/paginations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/core/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/ovinc_client/trace/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/instrumentors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/ovinc_client/trace/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/ovinc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 11:17:03.000000 ovinc_client-0.2.3/ovinc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-13 11:17:03.000000 ovinc_client-0.2.3/ovinc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:17:03.000000 ovinc_client-0.2.3/ovinc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 11:17:03.000000 ovinc_client-0.2.3/ovinc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 11:17:03.000000 ovinc_client-0.2.3/ovinc_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:17:03.592232 ovinc_client-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-13 11:16:59.000000 ovinc_client-0.2.3/setup.py
```

### Comparing `ovinc_client-0.2.2/LICENSE` & `ovinc_client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/PKG-INFO` & `ovinc_client-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django<5,>=4.2.11
-Requires-Dist: django_environ==0.10.0
-Requires-Dist: djangorestframework==3.14.0
-Requires-Dist: mysqlclient==2.1.1
-Requires-Dist: django-cors-headers==3.10.1
-Requires-Dist: pytz==2021.3
-Requires-Dist: django-sslserver==0.22
-Requires-Dist: pyOpenSSL==22.1.0
-Requires-Dist: django-simpleui==2023.8.28
-Requires-Dist: redis==4.5.4
-Requires-Dist: django-redis==5.2.0
-Requires-Dist: python_json_logger==2.0.4
-Requires-Dist: requests==2.31.0
-Requires-Dist: protobuf==3.19.5
+Requires-Dist: django<5,>=4
+Requires-Dist: django_environ<1,>=0.10.0
+Requires-Dist: djangorestframework<4,>=3.14.0
+Requires-Dist: mysqlclient<3,>=2.1.1
+Requires-Dist: django-cors-headers<4,>=3.11.0
+Requires-Dist: pytz<2025,>=2022.4
+Requires-Dist: django-sslserver<1,>=0.22
+Requires-Dist: pyOpenSSL<25,>=22.1.0
+Requires-Dist: django-simpleui<2025,>=2023.8.28
+Requires-Dist: redis<6,>=5.0.0
+Requires-Dist: django-redis<6,>=5.0.0
+Requires-Dist: python_json_logger<3,>=2.0.3
+Requires-Dist: httpx[http2]<1,>=0.23.2
+Requires-Dist: requests<3,>=2.28.0
+Requires-Dist: protobuf<6,>=3.19.5
 Requires-Dist: opentelemetry-api==1.24.0
 Requires-Dist: opentelemetry-sdk==1.24.0
 Requires-Dist: opentelemetry-exporter-jaeger==1.21.0
 Requires-Dist: opentelemetry-exporter-otlp==1.24.0
 Requires-Dist: opentelemetry-instrumentation==0.45b0
 Requires-Dist: opentelemetry-instrumentation-django==0.45b0
 Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
 Requires-Dist: opentelemetry-instrumentation-redis==0.45b0
 Requires-Dist: opentelemetry-instrumentation-requests==0.45b0
 Requires-Dist: opentelemetry-instrumentation-celery==0.45b0
 Requires-Dist: opentelemetry-instrumentation-logging==0.45b0
+Requires-Dist: opentelemetry-instrumentation-httpx==0.45b0
 
 ## OVINC Union Api Client
 
 ### Init
 
 Init: `APP_CODE` `APP_SECRET` `OVINC_API_URL`
```

### Comparing `ovinc_client-0.2.2/ovinc_client/account/constants.py` & `ovinc_client-0.2.3/ovinc_client/account/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/account/migrations/0001_initial.py` & `ovinc_client-0.2.3/ovinc_client/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/account/models.py` & `ovinc_client-0.2.3/ovinc_client/account/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/account/serializers.py` & `ovinc_client-0.2.3/ovinc_client/account/serializers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/account/views.py` & `ovinc_client-0.2.3/ovinc_client/account/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/client.py` & `ovinc_client-0.2.3/ovinc_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from json import JSONDecodeError
 
-import requests
-from requests import HTTPError, Response
+import httpx
+from httpx import HTTPStatusError, Response
 
 from ovinc_client.components.auth import Auth
 from ovinc_client.components.notice import Notice
 from ovinc_client.components.tcaptcha import TCaptcha
 from ovinc_client.constants import (
     APP_AUTH_HEADER_KEY,
     APP_AUTH_ID_KEY,
@@ -35,23 +35,24 @@
         self.tcaptcha = TCaptcha(self, self._union_api_url)
 
     def call_api(self, method: str, url: str, params: dict, timeout: float = OVINC_CLIENT_TIMEOUT) -> ResponseData:
         """
         call union api
         """
 
-        # init kwargs
-        kwargs = {"headers": self._build_headers(), "verify": bool(strtobool(os.getenv("OVINC_API_VERIFY", "True")))}
-        if method == RequestMethodEnum.GET.value:
-            kwargs["params"] = params
-        else:
-            kwargs["json"] = params
-
         # request
-        response = requests.request(method=method, url=url, timeout=timeout, **kwargs)
+        client = httpx.Client(
+            http2=True,
+            headers=self._build_headers(),
+            verify=bool(strtobool(os.getenv("OVINC_API_VERIFY", "True"))),
+        )
+        if method == RequestMethodEnum.GET:
+            response = client.request(method=method, url=url, timeout=timeout, params=params)
+        else:
+            response = client.request(method=method, url=url, timeout=timeout, json=params)
 
         # parse response
         return self._parse_response(response)
 
     def _build_headers(self) -> dict:
         """
         build request header
@@ -71,15 +72,15 @@
     def _parse_response(cls, response: Response) -> ResponseData:
         """
         parse response to json
         """
 
         try:
             response.raise_for_status()
-        except HTTPError as err:
+        except HTTPStatusError as err:
             logger.error("[ResponseCheckFailed] %s", err)
             return ResponseData(result=False)
 
         try:
             data = response.json()
         except (TypeError, ValueError, JSONDecodeError) as err:
             logger.error("[ResponseParseFailed] %s", err)
```

### Comparing `ovinc_client-0.2.2/ovinc_client/components/base.py` & `ovinc_client-0.2.3/ovinc_client/components/base.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/components/notice.py` & `ovinc_client-0.2.3/ovinc_client/components/notice.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/auth.py` & `ovinc_client-0.2.3/ovinc_client/core/auth.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/cache.py` & `ovinc_client-0.2.3/ovinc_client/core/cache.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/constants.py` & `ovinc_client-0.2.3/ovinc_client/core/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/exceptions.py` & `ovinc_client-0.2.3/ovinc_client/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/lock.py` & `ovinc_client-0.2.3/ovinc_client/core/lock.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/logger.py` & `ovinc_client-0.2.3/ovinc_client/core/logger.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/middlewares.py` & `ovinc_client-0.2.3/ovinc_client/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/models.py` & `ovinc_client-0.2.3/ovinc_client/core/models.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/paginations.py` & `ovinc_client-0.2.3/ovinc_client/core/paginations.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/renderers.py` & `ovinc_client-0.2.3/ovinc_client/core/renderers.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/utils.py` & `ovinc_client-0.2.3/ovinc_client/core/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/core/viewsets.py` & `ovinc_client-0.2.3/ovinc_client/core/viewsets.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/constants.py` & `ovinc_client-0.2.3/ovinc_client/trace/constants.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/exporters.py` & `ovinc_client-0.2.3/ovinc_client/trace/exporters.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/instrumentors.py` & `ovinc_client-0.2.3/ovinc_client/trace/instrumentors.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from django.http import HttpResponse
 from opentelemetry.instrumentation.celery import CeleryInstrumentor
 from opentelemetry.instrumentation.dbapi import (
     DatabaseApiIntegration,
     trace_integration,
 )
 from opentelemetry.instrumentation.django import DjangoInstrumentor
+from opentelemetry.instrumentation.httpx import HTTPXClientInstrumentor
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
 from opentelemetry.instrumentation.redis import RedisInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.trace import Span, Status, StatusCode, format_trace_id
 from requests import Response
 
@@ -122,14 +123,15 @@
 
     def _instrument(self, **kwargs):
         LoggingInstrumentor().instrument()
         RequestsInstrumentor().instrument(span_callback=requests_callback)
         DjangoInstrumentor().instrument(request_hook=django_request_hook, response_hook=django_response_hook)
         CeleryInstrumentor().instrument()
         RedisInstrumentor().instrument(request_hook=RedisRequestHook())
+        HTTPXClientInstrumentor().instrument()
         trace_integration(MySQLdb, "connect", "mysql", db_api_integration_factory=DBApiIntegration)
 
     def _uninstrument(self, **kwargs):
         if getattr(self, "instrumentors", None) is None:
             return
         for instrumentor in self.instrumentors:  # pylint: disable=E1101
             instrumentor.uninstrument()
```

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/setup.py` & `ovinc_client-0.2.3/ovinc_client/trace/setup.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/utils.py` & `ovinc_client-0.2.3/ovinc_client/trace/utils.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client/trace/views.py` & `ovinc_client-0.2.3/ovinc_client/trace/views.py`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client.egg-info/PKG-INFO` & `ovinc_client-0.2.3/ovinc_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 Metadata-Version: 2.1
 Name: ovinc_client
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Tool for OVINC Union API
 Home-page: https://www.ovinc.cn/
 Author: OVINC
 Author-email: contact@ovinc.cn
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Django<5,>=4.2.11
-Requires-Dist: django_environ==0.10.0
-Requires-Dist: djangorestframework==3.14.0
-Requires-Dist: mysqlclient==2.1.1
-Requires-Dist: django-cors-headers==3.10.1
-Requires-Dist: pytz==2021.3
-Requires-Dist: django-sslserver==0.22
-Requires-Dist: pyOpenSSL==22.1.0
-Requires-Dist: django-simpleui==2023.8.28
-Requires-Dist: redis==4.5.4
-Requires-Dist: django-redis==5.2.0
-Requires-Dist: python_json_logger==2.0.4
-Requires-Dist: requests==2.31.0
-Requires-Dist: protobuf==3.19.5
+Requires-Dist: django<5,>=4
+Requires-Dist: django_environ<1,>=0.10.0
+Requires-Dist: djangorestframework<4,>=3.14.0
+Requires-Dist: mysqlclient<3,>=2.1.1
+Requires-Dist: django-cors-headers<4,>=3.11.0
+Requires-Dist: pytz<2025,>=2022.4
+Requires-Dist: django-sslserver<1,>=0.22
+Requires-Dist: pyOpenSSL<25,>=22.1.0
+Requires-Dist: django-simpleui<2025,>=2023.8.28
+Requires-Dist: redis<6,>=5.0.0
+Requires-Dist: django-redis<6,>=5.0.0
+Requires-Dist: python_json_logger<3,>=2.0.3
+Requires-Dist: httpx[http2]<1,>=0.23.2
+Requires-Dist: requests<3,>=2.28.0
+Requires-Dist: protobuf<6,>=3.19.5
 Requires-Dist: opentelemetry-api==1.24.0
 Requires-Dist: opentelemetry-sdk==1.24.0
 Requires-Dist: opentelemetry-exporter-jaeger==1.21.0
 Requires-Dist: opentelemetry-exporter-otlp==1.24.0
 Requires-Dist: opentelemetry-instrumentation==0.45b0
 Requires-Dist: opentelemetry-instrumentation-django==0.45b0
 Requires-Dist: opentelemetry-instrumentation-dbapi==0.45b0
 Requires-Dist: opentelemetry-instrumentation-redis==0.45b0
 Requires-Dist: opentelemetry-instrumentation-requests==0.45b0
 Requires-Dist: opentelemetry-instrumentation-celery==0.45b0
 Requires-Dist: opentelemetry-instrumentation-logging==0.45b0
+Requires-Dist: opentelemetry-instrumentation-httpx==0.45b0
 
 ## OVINC Union Api Client
 
 ### Init
 
 Init: `APP_CODE` `APP_SECRET` `OVINC_API_URL`
```

### Comparing `ovinc_client-0.2.2/ovinc_client.egg-info/SOURCES.txt` & `ovinc_client-0.2.3/ovinc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovinc_client-0.2.2/ovinc_client.egg-info/requires.txt` & `ovinc_client-0.2.3/ovinc_client.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-Django<5,>=4.2.11
-django_environ==0.10.0
-djangorestframework==3.14.0
-mysqlclient==2.1.1
-django-cors-headers==3.10.1
-pytz==2021.3
-django-sslserver==0.22
-pyOpenSSL==22.1.0
-django-simpleui==2023.8.28
-redis==4.5.4
-django-redis==5.2.0
-python_json_logger==2.0.4
-requests==2.31.0
-protobuf==3.19.5
+django<5,>=4
+django_environ<1,>=0.10.0
+djangorestframework<4,>=3.14.0
+mysqlclient<3,>=2.1.1
+django-cors-headers<4,>=3.11.0
+pytz<2025,>=2022.4
+django-sslserver<1,>=0.22
+pyOpenSSL<25,>=22.1.0
+django-simpleui<2025,>=2023.8.28
+redis<6,>=5.0.0
+django-redis<6,>=5.0.0
+python_json_logger<3,>=2.0.3
+httpx[http2]<1,>=0.23.2
+requests<3,>=2.28.0
+protobuf<6,>=3.19.5
 opentelemetry-api==1.24.0
 opentelemetry-sdk==1.24.0
 opentelemetry-exporter-jaeger==1.21.0
 opentelemetry-exporter-otlp==1.24.0
 opentelemetry-instrumentation==0.45b0
 opentelemetry-instrumentation-django==0.45b0
 opentelemetry-instrumentation-dbapi==0.45b0
 opentelemetry-instrumentation-redis==0.45b0
 opentelemetry-instrumentation-requests==0.45b0
 opentelemetry-instrumentation-celery==0.45b0
 opentelemetry-instrumentation-logging==0.45b0
+opentelemetry-instrumentation-httpx==0.45b0
```

### Comparing `ovinc_client-0.2.2/setup.py` & `ovinc_client-0.2.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,50 +3,52 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="ovinc_client",
-    version="0.2.2",
+    version="0.2.3",
     author="OVINC",
     url="https://www.ovinc.cn/",
     author_email="contact@ovinc.cn",
     description="A Tool for OVINC Union API",
     packages=[
         "ovinc_client",
         "ovinc_client.account",
         "ovinc_client.account.migrations",
         "ovinc_client.components",
         "ovinc_client.core",
         "ovinc_client.trace",
     ],
     install_requires=[
-        "Django>=4.2.11,<5",
-        "django_environ==0.10.0",
-        "djangorestframework==3.14.0",
-        "mysqlclient==2.1.1",
-        "django-cors-headers==3.10.1",
-        "pytz==2021.3",
-        "django-sslserver==0.22",
-        "pyOpenSSL==22.1.0",
-        "django-simpleui==2023.8.28",
-        "redis==4.5.4",
-        "django-redis==5.2.0",
-        "python_json_logger==2.0.4",
-        "requests==2.31.0",
-        "protobuf==3.19.5",
+        "django>=4,<5",
+        "django_environ>=0.10.0,<1",
+        "djangorestframework>=3.14.0,<4",
+        "mysqlclient>=2.1.1,<3",
+        "django-cors-headers>=3.11.0,<4",
+        "pytz>=2022.4,<2025",
+        "django-sslserver>=0.22,<1",
+        "pyOpenSSL>=22.1.0,<25",
+        "django-simpleui>=2023.8.28,<2025",
+        "redis>=5.0.0,<6",
+        "django-redis>=5.0.0,<6",
+        "python_json_logger>=2.0.3,<3",
+        "httpx[http2]>=0.23.2,<1",
+        "requests>=2.28.0,<3",
+        "protobuf>=3.19.5,<6",
         "opentelemetry-api==1.24.0",
         "opentelemetry-sdk==1.24.0",
         "opentelemetry-exporter-jaeger==1.21.0",
         "opentelemetry-exporter-otlp==1.24.0",
         "opentelemetry-instrumentation==0.45b0",
         "opentelemetry-instrumentation-django==0.45b0",
         "opentelemetry-instrumentation-dbapi==0.45b0",
         "opentelemetry-instrumentation-redis==0.45b0",
         "opentelemetry-instrumentation-requests==0.45b0",
         "opentelemetry-instrumentation-celery==0.45b0",
         "opentelemetry-instrumentation-logging==0.45b0",
+        "opentelemetry-instrumentation-httpx==0.45b0",
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

