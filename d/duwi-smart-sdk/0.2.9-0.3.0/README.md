# Comparing `tmp/duwi_smart_sdk-0.2.9.tar.gz` & `tmp/duwi_smart_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duwi_smart_sdk-0.2.9.tar", last modified: Sat May 11 05:01:36 2024, max compression
+gzip compressed data, was "duwi_smart_sdk-0.3.0.tar", last modified: Mon May 13 09:14:06 2024, max compression
```

## Comparing `duwi_smart_sdk-0.2.9.tar` & `duwi_smart_sdk-0.3.0.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.738691 duwi_smart_sdk-0.2.9/
--rw-rw-rw-   0        0        0      900 2024-05-11 05:01:36.737692 duwi_smart_sdk-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.673745 duwi_smart_sdk-0.2.9/duwi_smart_sdk/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.698571 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/__init__.py
--rw-rw-rw-   0        0        0     2404 2024-05-11 05:00:46.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/account.py
--rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/control.py
--rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/discover.py
--rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/floor.py
--rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/house.py
--rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/refresh_token.py
--rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/room.py
--rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/ws.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.704090 duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/__init__.py
--rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/const.py
--rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/status.py
--rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/type_map.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.705084 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.708090 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/req/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/req/__init__.py
--rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/req/device_control.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.717596 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/__init__.py
--rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/auth.py
--rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/control.py
--rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/device.py
--rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/floor.py
--rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/house.py
--rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/room.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.722165 duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/http.py
--rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/sign.py
--rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/timestamp.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.736734 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1421 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-11 05:01:36.000000 duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 05:01:36.738691 duwi_smart_sdk-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      936 2024-05-11 05:01:08.000000 duwi_smart_sdk-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.723175 duwi_smart_sdk-0.2.9/test/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.733695 duwi_smart_sdk-0.2.9/test/api/
--rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.2.9/test/api/__init__.py
--rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.2.9/test/api/test_account.py
--rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.2.9/test/api/test_control.py
--rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.2.9/test/api/test_discover.py
--rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.2.9/test/api/test_floor.py
--rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.2.9/test/api/test_house.py
--rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.2.9/test/api/test_login.py
--rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.2.9/test/api/test_room.py
--rw-rw-rw-   0        0        0     1020 2024-05-07 07:13:14.000000 duwi_smart_sdk-0.2.9/test/api/test_ws.py
-drwxrwxrwx   0        0        0        0 2024-05-11 05:01:36.735737 duwi_smart_sdk-0.2.9/test/util/
--rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.2.9/test/util/__init__.py
--rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.2.9/test/util/test_http.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.837572 duwi_smart_sdk-0.3.0/
+-rw-rw-rw-   0        0        0      900 2024-05-13 09:14:06.836596 duwi_smart_sdk-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-10 01:36:43.000000 duwi_smart_sdk-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.768917 duwi_smart_sdk-0.3.0/duwi_smart_sdk/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.788649 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/__init__.py
+-rw-rw-rw-   0        0        0     2404 2024-05-11 05:00:46.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/account.py
+-rw-rw-rw-   0        0        0     1739 2024-05-10 00:48:21.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/control.py
+-rw-rw-rw-   0        0        0     4512 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/discover.py
+-rw-rw-rw-   0        0        0     2623 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/floor.py
+-rw-rw-rw-   0        0        0     2651 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/house.py
+-rw-rw-rw-   0        0        0     2121 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/refresh_token.py
+-rw-rw-rw-   0        0        0     2731 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/room.py
+-rw-rw-rw-   0        0        0     3098 2024-05-13 09:12:17.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/terminal.py
+-rw-rw-rw-   0        0        0     4768 2024-05-10 01:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/ws.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.794828 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/const.py
+-rw-rw-rw-   0        0        0      599 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/status.py
+-rw-rw-rw-   0        0        0     1154 2024-05-07 06:05:58.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/type_map.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.795887 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.798044 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/__init__.py
+-rw-rw-rw-   0        0        0      926 2024-05-10 01:12:19.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/device_control.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.809473 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/__init__.py
+-rw-rw-rw-   0        0        0     1050 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/auth.py
+-rw-rw-rw-   0        0        0      217 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/control.py
+-rw-rw-rw-   0        0        0     2977 2024-05-09 05:13:50.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/device.py
+-rw-rw-rw-   0        0        0      901 2024-05-10 01:13:17.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/floor.py
+-rw-rw-rw-   0        0        0     1722 2024-05-10 01:15:23.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/house.py
+-rw-rw-rw-   0        0        0      609 2024-05-09 07:11:19.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/room.py
+-rw-rw-rw-   0        0        0     1146 2024-05-13 09:11:16.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/terminal.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.815911 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     1848 2024-05-10 01:19:10.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/http.py
+-rw-rw-rw-   0        0        0      522 2024-05-10 01:19:53.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/sign.py
+-rw-rw-rw-   0        0        0      118 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/timestamp.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.835620 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1516 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 09:14:06.000000 duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 09:14:06.837572 duwi_smart_sdk-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      936 2024-05-13 09:14:04.000000 duwi_smart_sdk-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.817864 duwi_smart_sdk-0.3.0/test/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.831703 duwi_smart_sdk-0.3.0/test/api/
+-rw-rw-rw-   0        0        0        0 2024-05-07 06:10:48.000000 duwi_smart_sdk-0.3.0/test/api/__init__.py
+-rw-rw-rw-   0        0        0      723 2024-05-11 03:19:03.000000 duwi_smart_sdk-0.3.0/test/api/test_account.py
+-rw-rw-rw-   0        0        0      948 2024-05-08 01:12:43.000000 duwi_smart_sdk-0.3.0/test/api/test_control.py
+-rw-rw-rw-   0        0        0      813 2024-05-09 03:37:26.000000 duwi_smart_sdk-0.3.0/test/api/test_discover.py
+-rw-rw-rw-   0        0        0      780 2024-05-09 07:45:49.000000 duwi_smart_sdk-0.3.0/test/api/test_floor.py
+-rw-rw-rw-   0        0        0      687 2024-05-07 06:29:35.000000 duwi_smart_sdk-0.3.0/test/api/test_house.py
+-rw-rw-rw-   0        0        0      640 2024-05-07 08:44:11.000000 duwi_smart_sdk-0.3.0/test/api/test_login.py
+-rw-rw-rw-   0        0        0      724 2024-05-09 07:16:53.000000 duwi_smart_sdk-0.3.0/test/api/test_room.py
+-rw-rw-rw-   0        0        0      732 2024-05-13 09:10:46.000000 duwi_smart_sdk-0.3.0/test/api/test_terminal.py
+-rw-rw-rw-   0        0        0     1220 2024-05-13 01:32:37.000000 duwi_smart_sdk-0.3.0/test/api/test_ws.py
+drwxrwxrwx   0        0        0        0 2024-05-13 09:14:06.833662 duwi_smart_sdk-0.3.0/test/util/
+-rw-rw-rw-   0        0        0        0 2024-05-06 05:48:31.000000 duwi_smart_sdk-0.3.0/test/util/__init__.py
+-rw-rw-rw-   0        0        0     1222 2024-05-07 06:12:53.000000 duwi_smart_sdk-0.3.0/test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.9/PKG-INFO` & `duwi_smart_sdk-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/account.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/control.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/discover.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/floor.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/house.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/refresh_token.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/refresh_token.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/room.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/api/ws.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/api/ws.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/status.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/status.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/const/type_map.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/const/type_map.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/req/device_control.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/req/device_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/auth.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/auth.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/device.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/device.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/floor.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/house.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/model/resp/room.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/model/resp/room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/http.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/http.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk/util/sign.py` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk/util/sign.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/PKG-INFO` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duwi_smart_sdk
-Version: 0.2.9
+Version: 0.3.0
 Summary: sdk for duwi third platform
 Home-page: https://github.com/Ledgerbiggg/duwi_smart_sdk
 Author: ledger
 Author-email: ledgerbiggg@gmail.com
 License: MIT
 Keywords: python,duwi,sdk,third,platform
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `duwi_smart_sdk-0.2.9/duwi_smart_sdk.egg-info/SOURCES.txt` & `duwi_smart_sdk-0.3.0/duwi_smart_sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 duwi_smart_sdk/api/account.py
 duwi_smart_sdk/api/control.py
 duwi_smart_sdk/api/discover.py
 duwi_smart_sdk/api/floor.py
 duwi_smart_sdk/api/house.py
 duwi_smart_sdk/api/refresh_token.py
 duwi_smart_sdk/api/room.py
+duwi_smart_sdk/api/terminal.py
 duwi_smart_sdk/api/ws.py
 duwi_smart_sdk/const/__init__.py
 duwi_smart_sdk/const/const.py
 duwi_smart_sdk/const/status.py
 duwi_smart_sdk/const/type_map.py
 duwi_smart_sdk/model/__init__.py
 duwi_smart_sdk/model/req/__init__.py
@@ -26,23 +27,25 @@
 duwi_smart_sdk/model/resp/__init__.py
 duwi_smart_sdk/model/resp/auth.py
 duwi_smart_sdk/model/resp/control.py
 duwi_smart_sdk/model/resp/device.py
 duwi_smart_sdk/model/resp/floor.py
 duwi_smart_sdk/model/resp/house.py
 duwi_smart_sdk/model/resp/room.py
+duwi_smart_sdk/model/resp/terminal.py
 duwi_smart_sdk/util/__init__.py
 duwi_smart_sdk/util/http.py
 duwi_smart_sdk/util/sign.py
 duwi_smart_sdk/util/timestamp.py
 test/__init__.py
 test/api/__init__.py
 test/api/test_account.py
 test/api/test_control.py
 test/api/test_discover.py
 test/api/test_floor.py
 test/api/test_house.py
 test/api/test_login.py
 test/api/test_room.py
+test/api/test_terminal.py
 test/api/test_ws.py
 test/util/__init__.py
 test/util/test_http.py
```

### Comparing `duwi_smart_sdk-0.2.9/setup.py` & `duwi_smart_sdk-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.9'
+VERSION = '0.3.0'
 DESCRIPTION = 'sdk for duwi third platform'
 
 setup(
     name="duwi_smart_sdk",
     version=VERSION,
     author="ledger",
     author_email="ledgerbiggg@gmail.com",
```

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_account.py` & `duwi_smart_sdk-0.3.0/test/api/test_account.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_control.py` & `duwi_smart_sdk-0.3.0/test/api/test_control.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_discover.py` & `duwi_smart_sdk-0.3.0/test/api/test_discover.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_floor.py` & `duwi_smart_sdk-0.3.0/test/api/test_floor.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_house.py` & `duwi_smart_sdk-0.3.0/test/api/test_house.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_login.py` & `duwi_smart_sdk-0.3.0/test/api/test_login.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_room.py` & `duwi_smart_sdk-0.3.0/test/api/test_room.py`

 * *Files identical despite different names*

### Comparing `duwi_smart_sdk-0.2.9/test/api/test_ws.py` & `duwi_smart_sdk-0.3.0/test/api/test_ws.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+import logging
 from unittest import TestCase
 from duwi_smart_sdk.api.ws import DeviceSynchronizationWS
 import asyncio
 
+_LOGGER = logging.getLogger(__name__)
 
 class TestDeviceSynchronizationWS(TestCase):
     def test_device_synchronization(self):
         async def run_test():
             async def on_callback(x: str):
                 print(f"on_callback: {x}")
-
+            # 测试房屋
             ws = DeviceSynchronizationWS(
                 on_callback=on_callback,
                 app_key="2e479831-1fb7-751e-7017-7534f7f99fc1",
                 app_secret="26af4883a943083a4c34083897fcea10",
                 access_token="715d1c63-85c0-4d74-9a89-5a0aa4806f74",
                 refresh_token="c539ec1b-99d9-44f2-8bb0-b942545c0aca",
-                house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
+                # house_no="c7bf567d-225a-4533-ab72-5dc080b794f5",
+                house_no="cd56eba8-d63c-4676-b09e-9bffae64076e",
                 app_version="0.0.1",
                 client_version="0.0.1",
                 client_model="homeassistant",
             )
-
+            _LOGGER.warning('connect ws server...')
             await ws.reconnect()
             await ws.listen()
             await ws.keep_alive()
 
         asyncio.run(run_test())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `duwi_smart_sdk-0.2.9/test/util/test_http.py` & `duwi_smart_sdk-0.3.0/test/util/test_http.py`

 * *Files identical despite different names*

