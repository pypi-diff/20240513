# Comparing `tmp/backpipe-0.5.1.tar.gz` & `tmp/backpipe-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backpipe-0.5.1.tar", last modified: Sat Apr 27 13:25:55 2024, max compression
+gzip compressed data, was "backpipe-0.6.0.tar", last modified: Mon May 13 21:23:42 2024, max compression
```

## Comparing `backpipe-0.5.1.tar` & `backpipe-0.6.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.461519 backpipe-0.5.1/
--rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.5.1/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.5.1/MANIFEST.in
--rw-r--r--   0 simon     (1000) simon     (1000)     3513 2024-04-27 13:25:55.461519 backpipe-0.5.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     2860 2024-04-15 19:20:17.000000 backpipe-0.5.1/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.455519 backpipe-0.5.1/backpipe/
--rw-r--r--   0 simon     (1000) simon     (1000)      490 2024-04-27 13:25:44.000000 backpipe-0.5.1/backpipe/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.5.1/backpipe/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6095 2024-04-14 09:49:40.000000 backpipe-0.5.1/backpipe/app.py
--rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.5.1/backpipe/builder.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1257 2024-03-28 19:06:16.000000 backpipe-0.5.1/backpipe/config.py
--rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.5.1/backpipe/defaults.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-03-30 04:22:44.000000 backpipe-0.5.1/backpipe/host.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.456519 backpipe-0.5.1/backpipe/presets/
--rw-r--r--   0 simon     (1000) simon     (1000)      522 2024-04-26 19:42:58.000000 backpipe-0.5.1/backpipe/presets/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1468 2024-04-27 13:25:44.000000 backpipe-0.5.1/backpipe/presets/file.py
--rw-r--r--   0 simon     (1000) simon     (1000)      459 2024-04-27 13:25:44.000000 backpipe-0.5.1/backpipe/presets/ipaddr.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-04-14 09:53:29.000000 backpipe-0.5.1/backpipe/rq.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6476 2024-03-30 04:30:41.000000 backpipe-0.5.1/backpipe/server.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.457519 backpipe-0.5.1/backpipe/tools/
--rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.5.1/backpipe/tools/__init__.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.457519 backpipe-0.5.1/backpipe/tools/base64/
--rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.5.1/backpipe/tools/base64/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.5.1/backpipe/tools/base64/decode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.5.1/backpipe/tools/base64/encode.py
--rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.5.1/backpipe/tools/check_type.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.458519 backpipe-0.5.1/backpipe/tools/file/
--rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.5.1/backpipe/tools/file/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.5.1/backpipe/tools/file/append.py
--rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.5.1/backpipe/tools/file/create.py
--rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.5.1/backpipe/tools/file/delete.py
--rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.5.1/backpipe/tools/file/write.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.459519 backpipe-0.5.1/backpipe/tools/hash/
--rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.5.1/backpipe/tools/hash/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.5.1/backpipe/tools/hash/md5.py
--rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.5.1/backpipe/tools/hash/sha1.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.5.1/backpipe/tools/hash/sha224.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.5.1/backpipe/tools/hash/sha256.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.5.1/backpipe/tools/hash/sha384.py
--rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.5.1/backpipe/tools/hash/sha512.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.460519 backpipe-0.5.1/backpipe/tools/html/
--rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.5.1/backpipe/tools/html/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.5.1/backpipe/tools/html/addMeta.py
--rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.5.1/backpipe/tools/html/addStyle.py
--rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.5.1/backpipe/tools/html/addTag.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.5.1/backpipe/tools/html/html.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.461519 backpipe-0.5.1/backpipe/tools/json/
--rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.5.1/backpipe/tools/json/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      184 2024-04-15 14:42:14.000000 backpipe-0.5.1/backpipe/tools/json/deserialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.5.1/backpipe/tools/json/serialize.py
--rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.5.1/backpipe/uptime.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-04-27 13:25:55.456519 backpipe-0.5.1/backpipe.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     3513 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     1266 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-04-27 13:25:55.000000 backpipe-0.5.1/backpipe.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-04-27 13:25:55.461519 backpipe-0.5.1/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.5.1/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.991404 backpipe-0.6.0/
+-rw-r--r--   0 simon     (1000) simon     (1000)    35129 2023-11-04 20:14:40.000000 backpipe-0.6.0/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)      176 2024-04-22 18:38:17.000000 backpipe-0.6.0/MANIFEST.in
+-rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-13 21:23:42.991404 backpipe-0.6.0/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     2872 2024-05-09 11:06:37.000000 backpipe-0.6.0/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.986405 backpipe-0.6.0/backpipe/
+-rw-r--r--   0 simon     (1000) simon     (1000)      537 2024-05-09 10:29:17.000000 backpipe-0.6.0/backpipe/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5172 2024-04-26 15:29:12.000000 backpipe-0.6.0/backpipe/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5798 2024-05-09 11:35:16.000000 backpipe-0.6.0/backpipe/app.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     3244 2024-03-30 02:36:58.000000 backpipe-0.6.0/backpipe/builder.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1027 2024-05-09 11:37:15.000000 backpipe-0.6.0/backpipe/config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      364 2024-03-29 01:51:22.000000 backpipe-0.6.0/backpipe/defaults.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1916 2024-05-09 19:47:37.000000 backpipe-0.6.0/backpipe/host.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/presets/
+-rw-r--r--   0 simon     (1000) simon     (1000)      627 2024-05-09 14:02:28.000000 backpipe-0.6.0/backpipe/presets/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1468 2024-04-27 13:29:04.000000 backpipe-0.6.0/backpipe/presets/file.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      459 2024-04-27 13:29:04.000000 backpipe-0.6.0/backpipe/presets/ipaddr.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      870 2024-05-09 15:37:55.000000 backpipe-0.6.0/backpipe/presets/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      589 2024-05-11 09:44:30.000000 backpipe-0.6.0/backpipe/redirect.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1233 2024-05-09 10:28:38.000000 backpipe-0.6.0/backpipe/rq.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     7185 2024-05-10 12:09:45.000000 backpipe-0.6.0/backpipe/server.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/tools/
+-rw-r--r--   0 simon     (1000) simon     (1000)      178 2024-04-22 17:36:44.000000 backpipe-0.6.0/backpipe/tools/__init__.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.988404 backpipe-0.6.0/backpipe/tools/base64/
+-rw-r--r--   0 simon     (1000) simon     (1000)       95 2024-04-15 14:45:34.000000 backpipe-0.6.0/backpipe/tools/base64/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:45:00.000000 backpipe-0.6.0/backpipe/tools/base64/decode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      177 2024-04-15 14:43:40.000000 backpipe-0.6.0/backpipe/tools/base64/encode.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      398 2024-04-15 15:05:34.000000 backpipe-0.6.0/backpipe/tools/check_type.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.989405 backpipe-0.6.0/backpipe/tools/file/
+-rw-r--r--   0 simon     (1000) simon     (1000)      181 2024-04-22 17:06:34.000000 backpipe-0.6.0/backpipe/tools/file/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      464 2024-04-22 17:03:16.000000 backpipe-0.6.0/backpipe/tools/file/append.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      301 2024-04-22 16:26:18.000000 backpipe-0.6.0/backpipe/tools/file/create.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      388 2024-04-22 16:51:25.000000 backpipe-0.6.0/backpipe/tools/file/delete.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      463 2024-04-22 16:39:25.000000 backpipe-0.6.0/backpipe/tools/file/write.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.990404 backpipe-0.6.0/backpipe/tools/hash/
+-rw-r--r--   0 simon     (1000) simon     (1000)      265 2024-04-22 17:45:34.000000 backpipe-0.6.0/backpipe/tools/hash/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      284 2024-04-22 17:41:35.000000 backpipe-0.6.0/backpipe/tools/hash/md5.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      286 2024-04-22 17:41:54.000000 backpipe-0.6.0/backpipe/tools/hash/sha1.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:44.000000 backpipe-0.6.0/backpipe/tools/hash/sha224.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:42:57.000000 backpipe-0.6.0/backpipe/tools/hash/sha256.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:00.000000 backpipe-0.6.0/backpipe/tools/hash/sha384.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      290 2024-04-22 17:44:07.000000 backpipe-0.6.0/backpipe/tools/hash/sha512.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.990404 backpipe-0.6.0/backpipe/tools/html/
+-rw-r--r--   0 simon     (1000) simon     (1000)       41 2024-04-14 18:21:28.000000 backpipe-0.6.0/backpipe/tools/html/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      212 2024-04-14 20:54:18.000000 backpipe-0.6.0/backpipe/tools/html/addMeta.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      130 2024-04-14 20:54:11.000000 backpipe-0.6.0/backpipe/tools/html/addStyle.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      346 2024-04-27 09:07:22.000000 backpipe-0.6.0/backpipe/tools/html/addTag.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1176 2024-04-27 09:10:21.000000 backpipe-0.6.0/backpipe/tools/html/html.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.991404 backpipe-0.6.0/backpipe/tools/json/
+-rw-r--r--   0 simon     (1000) simon     (1000)      107 2024-04-14 16:06:07.000000 backpipe-0.6.0/backpipe/tools/json/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      184 2024-04-15 14:42:14.000000 backpipe-0.6.0/backpipe/tools/json/deserialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      262 2024-04-15 14:42:48.000000 backpipe-0.6.0/backpipe/tools/json/serialize.py
+-rw-r--r--   0 simon     (1000) simon     (1000)      137 2023-11-14 15:08:41.000000 backpipe-0.6.0/backpipe/uptime.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2024-05-13 21:23:42.987404 backpipe-0.6.0/backpipe.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     3525 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     1316 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       52 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       19 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        9 2024-05-13 21:23:42.000000 backpipe-0.6.0/backpipe.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2024-05-13 21:23:42.991404 backpipe-0.6.0/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)     1532 2024-04-26 16:49:47.000000 backpipe-0.6.0/setup.py
```

### Comparing `backpipe-0.5.1/LICENSE` & `backpipe-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/PKG-INFO` & `backpipe-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.5.1
+Version: 0.6.0
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -51,51 +51,51 @@
 ### Hello World!
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def hello_world(r: backpipe.Request):
     return (200, "Hello World")
 
 server.run()
 ```
 
 ### What is my IP address?
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def my_ip_address(r: backpipe.Request):
     return (200, r.address)
 
 server.run()
 ```
 
 ### Complex Example
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.any
+@server.any()
 def wrong_method(r: backpipe.Request):
     return (405, f"Wrong method: {r.method}, use POST.")
 
-@server.unknown
+@server.unknown()
 def unknown_method(r: backpipe.Request):
     return (405, f"Unknown method: {r.method}, use POST.")
 
-@server.post
+@server.post()
 def login(r: backpipe.Request):
     try:
         if r.headers["key"] == "password1234":
             return (200, "Password correct!")
         else:
             return (304, "Password wrong!")
     except KeyError:
@@ -107,15 +107,15 @@
 ### Using Request Bodies
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.post
+@server.post()
 def respond(r: backpipe.Request):
     return (200, r.body) # Returns the clients's request body
 
 server.run()
 ```
 
 ## Known issues
```

### Comparing `backpipe-0.5.1/README.md` & `backpipe-0.6.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -32,51 +32,51 @@
 ### Hello World!
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def hello_world(r: backpipe.Request):
     return (200, "Hello World")
 
 server.run()
 ```
 
 ### What is my IP address?
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def my_ip_address(r: backpipe.Request):
     return (200, r.address)
 
 server.run()
 ```
 
 ### Complex Example
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.any
+@server.any()
 def wrong_method(r: backpipe.Request):
     return (405, f"Wrong method: {r.method}, use POST.")
 
-@server.unknown
+@server.unknown()
 def unknown_method(r: backpipe.Request):
     return (405, f"Unknown method: {r.method}, use POST.")
 
-@server.post
+@server.post()
 def login(r: backpipe.Request):
     try:
         if r.headers["key"] == "password1234":
             return (200, "Password correct!")
         else:
             return (304, "Password wrong!")
     except KeyError:
@@ -88,15 +88,15 @@
 ### Using Request Bodies
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.post
+@server.post()
 def respond(r: backpipe.Request):
     return (200, r.body) # Returns the clients's request body
 
 server.run()
 ```
 
 ## Known issues
```

### Comparing `backpipe-0.5.1/backpipe/__main__.py` & `backpipe-0.6.0/backpipe/__main__.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe/app.py` & `backpipe-0.6.0/backpipe/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .builder import BackPipeBuilder
 from .config import config
 from .uptime import _uptime
+from backpipe.tools.check_type import check
 
 class BackPipe():
     """
     The class, that is the instance of your API server.
     """
     def __init__(self, address = None, port = None) -> None:
         if address == None:
@@ -17,14 +18,16 @@
             set_port = port
             
         self.__builder__ = BackPipeBuilder(set_address, set_port)
     def __str__(self) -> str:
         return f"BackPipe(address={self.__builder__.addr.__repr__()}, port={self.__builder__.port})"
     def __repr__(self) -> str:
         return self.__str__()
+    def __eq__(self, other) -> bool:
+        return isinstance(other, BackPipe) and self.__dict__ == other.__dict__
     # HTTPS support still in Development, uncomment it, if you want to test it.
     #def enable_https(self, certfile, keyfile):
     #    """
     #    Offers integrated SSL support.
     #    Certfiles and Keyfiles can be generated using OpenSSL.
     #    Tools such as CURL or your web browser will raise warnings, that the connection is unsafe if you self-sign your certificate.
     #    """
@@ -34,136 +37,132 @@
         Set a rate limit for how many requests from one IP address are allowed per minute.
         Set it to a number below 0 to disable rate limiting.
         Default rate limit is -1 (No limit.).
         """
         if not isinstance(limit, int):
             raise TypeError(f"given rate limit must be 'int' not '{type(limit).__name__}'")
         self.__builder__.ratelimit = limit
-    def ratelimit(self, function):
+    def ratelimit(self):
         """
         Set a message, that gets responded, when a client is rate limited.
         Default is 'Too many requests from the same client.'
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.ratelimit_message = function
-        return wrapper()
+        return wrapper
     def set_ratelimit_reset_interval(self, time):
         """
         Set a time, that determines how long it takes until the ratelimits are reset.
         Default is 60.
         """
-        if not isinstance(time, (int, float)):
-            raise TypeError(f"specified time must be 'int' or 'float' not '{type(time).__name__}'")
-        else:
-            self.__builder__.ratelimit_reset = time
+        check(time, (int, float), "time")
+            
+        self.__builder__.ratelimit_reset = time
     def ratelimit_exception_ipaddr(self, *addresses):
         """
         Set an exception for ratelimiting based on the clients IP address.
         """
         for a in addresses:
-            if not isinstance(a, str):
-                raise TypeError(f"all addresses must be 'str' not '{type(a).__name__}'")
-        else:
-            self.__builder__.ratelimit_exc_addrs.extend(addresses)
+            check(a, str, "all addresses")
+
+        self.__builder__.ratelimit_exc_addrs.extend(addresses)
     def ratelimit_exception_paths(self, *paths):
         """
         Set an exception for ratelimiting based on the requested path.
         """
         for p in paths:
-            if not isinstance(p, str):
-                raise TypeError(f"all addresses must be 'str' not '{type(p).__name__}'")
-        else:
-            self.__builder__.ratelimit_exc_paths.extend(paths)
+            check(p, str, "all paths")
+
+        self.__builder__.ratelimit_exc_paths.extend(paths)
     def uptime(self):
         """
         Uptime counter starts when the server is started.
         """
         return _uptime(self.__builder__)
     def set_uri_limit(self, amount):
         """
         Set the URI limit, which can't be exceeded by the client.
         If the URI limit was exceeded the client gets a special message.
         Default is 65536.
         """
-        if not isinstance(amount, int):
-            raise TypeError(f"specified amount must be 'int' not {type(amount).__name__}")
-        else:
-            self.__builder__.uri_limit = amount
+        check(amount, int, "amount")
+        
+        self.__builder__.uri_limit = amount
     def uri_limit_message(self, message):
         """
         Set the returned message when the client exceeded the URI limit.
         """
         if isinstance(message, str):
             message = message.encode()
         elif isinstance(message, bytes):
             pass
         else:
             raise TypeError(f"message parameter must be 'str' not '{type(message).__name__}'")
         self.__builder__.uri_limit_msg(message)
-    def get(self, function):
+    def get(self):
         """
         Set the GET request handler.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_get(function)
-        return wrapper()
-    def post(self, function):
+        return wrapper
+    def post(self):
         """
         Set the POST request handler.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_post(function)
-        return wrapper()
-    def put(self, function):
+        return wrapper
+    def put(self):
         """
         Set the PUT request handler.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_put(function)
-        return wrapper()
-    def patch(self, function):
+        return wrapper
+    def patch(self):
         """
         Set the PATCH request handler.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_patch(function)
-        return wrapper()
-    def delete(self, function):
+        return wrapper
+    def delete(self):
         """
         Set the DELETE request handler.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_delete(function)
-        return wrapper()
-    def unknown(self, function):
+        return wrapper
+    def unknown(self):
         """
         If an unknown method is used, the set function will handle it.
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_unknown(function)
-        return wrapper()
-    def any(self, function):
+        return wrapper
+    def any(self):
         """
         Set the handler for GET, POST, PUT, PATCH, DELETE.
         Can be overwritten using the normal way:
 
         @{server_instance_name}.{method}
 
         def foo(r):
             return (200, "Blah.")
 
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.set_all(function)
-        return wrapper()
-    def block(self, function):
+        return wrapper
+    def block(self):
         """
         Set the request handler for client's with blocked IP addresses.
         Block an IP address by using {server_instance_name}.block_address("addr1", "addr2") ...
         """
-        def wrapper():
+        def wrapper(function):
             self.__builder__.blocked_msg = function
-        return wrapper()
+        return wrapper
     def block_address(self, *addresses):
         self.__builder__.block_address(addresses)
     def run(self):
         self.__builder__.run()
```

### Comparing `backpipe-0.5.1/backpipe/builder.py` & `backpipe-0.6.0/backpipe/builder.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe/host.py` & `backpipe-0.6.0/backpipe/host.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe/presets/file.py` & `backpipe-0.6.0/backpipe/presets/file.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe/rq.py` & `backpipe-0.6.0/backpipe/rq.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe/server.py` & `backpipe-0.6.0/backpipe/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from socketserver import *
 from colorama import Back, Fore , init
 from typing import Any
 
 from .rq import Request
 from .host import Server as BackPipeHoster
 from .config import config
+from .redirect import BackPipeRedirect
 
 init()
 
 class BackPipeServer(SimpleHTTPRequestHandler):
     def __init__(self, request, client_address, server: BackPipeHoster, *, directory: str | None = None) -> None:
         super().__init__(request, client_address, server=server, directory=directory)
     def log_message(self, format: str, *args: Any) -> None:
@@ -68,14 +69,25 @@
                 pass
 
             if not self.client_address[0] in self.server.ratelimit_exc_addr and not self.path in self.server.ratelimit_exc_path:
                 self.server.add_ip_ratelimiter(self.client_address[0])
 
             if not hasattr(self, mname):
                 answer = self.server.unknown(Request(self.client_address, self.path, self.headers, self.command, self.body))
+                if isinstance(answer, BackPipeRedirect):
+                    self.send_response(301)
+                    self.send_header("Location", answer.location)
+                    if config.use_html_header:
+                        self.send_header("Content-Type", "text/html")
+                    self.end_headers()
+                    if isinstance(answer.message, str):
+                        self.wfile.write(answer.message.encode())
+                    else:
+                        self.wfile.write(answer.message)
+                    return
                 if not isinstance(answer[0], int):
                     raise TypeError(f"HTTP status code must be 'int' not '{type(answer[0]).__name__}'")
                 self.send_response(answer[0])
                 self.end_headers()
                 if isinstance(answer[1], str):
                     self.wfile.write(answer[1].encode())
                 elif isinstance(answer[1], bytes):
@@ -87,22 +99,25 @@
             method()
             self.wfile.flush()
         except TimeoutError as e:
             self.log_error("Request timed out: %r", e)
             self.close_connection = True
             return
     def handlerq(self, answer):
-        """TODO
-        if self.server.https != None:
-            if self.headers.get("X-Forwarded-Proto", "http") == "http":
-                print("YES")
-                self.send_response(301)
-                self.send_header('Location', 'https://{}{}'.format(self.server.server_address[0], self.path))
-                self.end_headers()
-        """
+        if isinstance(answer, BackPipeRedirect):
+            self.send_response(301)
+            self.send_header("Location", answer.location)
+            if config.use_html_header:
+                self.send_header("Content-Type", "text/html")
+            self.end_headers()
+            if isinstance(answer.message, str):
+                self.wfile.write(answer.message.encode())
+            else:
+                self.wfile.write(answer.message)
+            return
         if not isinstance(answer[0], int):
             raise TypeError(f"HTTP status code must be 'int' not '{type(answer[0]).__name__}'")
         self.send_response(answer[0])
         if config.use_html_header:
             self.send_header("Content-Type", "text/html")
         self.end_headers()
         if isinstance(answer[1], str):
```

### Comparing `backpipe-0.5.1/backpipe/tools/html/html.py` & `backpipe-0.6.0/backpipe/tools/html/html.py`

 * *Files identical despite different names*

### Comparing `backpipe-0.5.1/backpipe.egg-info/PKG-INFO` & `backpipe-0.6.0/backpipe.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backpipe
-Version: 0.5.1
+Version: 0.6.0
 Summary: A backend HTTP framework for Python.
 Home-page: https://github.com/Simoso68/backpipe
 Author: Simoso68
 Maintainer: Simoso68
 License: GNU GPL v3
 Keywords: framework,http,web,api,server
 Classifier: Development Status :: 4 - Beta
@@ -51,51 +51,51 @@
 ### Hello World!
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def hello_world(r: backpipe.Request):
     return (200, "Hello World")
 
 server.run()
 ```
 
 ### What is my IP address?
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.get
+@server.get()
 def my_ip_address(r: backpipe.Request):
     return (200, r.address)
 
 server.run()
 ```
 
 ### Complex Example
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.any
+@server.any()
 def wrong_method(r: backpipe.Request):
     return (405, f"Wrong method: {r.method}, use POST.")
 
-@server.unknown
+@server.unknown()
 def unknown_method(r: backpipe.Request):
     return (405, f"Unknown method: {r.method}, use POST.")
 
-@server.post
+@server.post()
 def login(r: backpipe.Request):
     try:
         if r.headers["key"] == "password1234":
             return (200, "Password correct!")
         else:
             return (304, "Password wrong!")
     except KeyError:
@@ -107,15 +107,15 @@
 ### Using Request Bodies
 
 ```python
 import backpipe
 
 server = backpipe.BackPipe()
 
-@server.post
+@server.post()
 def respond(r: backpipe.Request):
     return (200, r.body) # Returns the clients's request body
 
 server.run()
 ```
 
 ## Known issues
```

### Comparing `backpipe-0.5.1/backpipe.egg-info/SOURCES.txt` & `backpipe-0.6.0/backpipe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,26 +5,28 @@
 backpipe/__init__.py
 backpipe/__main__.py
 backpipe/app.py
 backpipe/builder.py
 backpipe/config.py
 backpipe/defaults.py
 backpipe/host.py
+backpipe/redirect.py
 backpipe/rq.py
 backpipe/server.py
 backpipe/uptime.py
 backpipe.egg-info/PKG-INFO
 backpipe.egg-info/SOURCES.txt
 backpipe.egg-info/dependency_links.txt
 backpipe.egg-info/entry_points.txt
 backpipe.egg-info/requires.txt
 backpipe.egg-info/top_level.txt
 backpipe/presets/__init__.py
 backpipe/presets/file.py
 backpipe/presets/ipaddr.py
+backpipe/presets/redirect.py
 backpipe/tools/__init__.py
 backpipe/tools/check_type.py
 backpipe/tools/base64/__init__.py
 backpipe/tools/base64/decode.py
 backpipe/tools/base64/encode.py
 backpipe/tools/file/__init__.py
 backpipe/tools/file/append.py
```

### Comparing `backpipe-0.5.1/setup.py` & `backpipe-0.6.0/setup.py`

 * *Files identical despite different names*

