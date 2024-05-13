# Comparing `tmp/sbn-95.tar.gz` & `tmp/sbn-96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-95.tar", last modified: Sun May 12 05:56:48 2024, max compression
+gzip compressed data, was "sbn-96.tar", last modified: Mon May 13 02:46:23 2024, max compression
```

## Comparing `sbn-95.tar` & `sbn-96.tar`

### file list

```diff
@@ -1,79 +1,74 @@
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.304195 sbn-95/
--rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-12 05:56:48.304195 sbn-95/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1932 2024-05-12 05:45:59.000000 sbn-95/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/
--rw-r--r--   0 bart      (1000) bart      (1001)   180711 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAabilify.png
--rw-r--r--   0 bart      (1000) bart      (1001)   193757 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAclozapine.png
--rw-r--r--   0 bart      (1000) bart      (1001)   197697 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAhaldol.png
--rw-r--r--   0 bart      (1000) bart      (1001)   232313 2024-05-12 05:07:36.000000 sbn-95/docs/ECHAzyprexa.png
--rw-r--r--   0 bart      (1000) bart      (1001)   245670 2024-05-12 05:07:36.000000 sbn-95/docs/OTP1.png
--rw-r--r--   0 bart      (1000) bart      (1001)   238095 2024-05-12 05:07:36.000000 sbn-95/docs/OTP2.png
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/_static/
--rw-r--r--   0 bart      (1000) bart      (1001)     1000 2024-05-12 05:07:36.000000 sbn-95/docs/_static/sbn.css
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/_templates/
--rw-r--r--   0 bart      (1000) bart      (1001)      291 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/base.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      543 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/class.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/mine.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-95/docs/_templates/module.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     1178 2024-05-12 05:17:00.000000 sbn-95/docs/about.rst
--rw-r--r--   0 bart      (1000) bart      (1001)   130021 2024-05-12 05:07:36.000000 sbn-95/docs/arrest.png
--rw-r--r--   0 bart      (1000) bart      (1001)   256520 2024-05-12 05:07:36.000000 sbn-95/docs/banner.png
--rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-05-12 05:07:36.000000 sbn-95/docs/bevestigd.jpg
--rw-r--r--   0 bart      (1000) bart      (1001)     3644 2024-05-12 05:18:53.000000 sbn-95/docs/conf.py
--rw-r--r--   0 bart      (1000) bart      (1001)      600 2024-05-12 05:17:00.000000 sbn-95/docs/evidence.rst
--rw-r--r--   0 bart      (1000) bart      (1001)    47740 2024-05-12 05:07:36.000000 sbn-95/docs/genocide.png
--rw-r--r--   0 bart      (1000) bart      (1001)      364 2024-05-12 05:17:00.000000 sbn-95/docs/guilty.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     2153 2024-05-12 05:17:00.000000 sbn-95/docs/index.rst
--rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-05-12 05:07:36.000000 sbn-95/docs/informed.jpg
--rw-r--r--   0 bart      (1000) bart      (1001)   228393 2024-05-12 05:07:36.000000 sbn-95/docs/kamer.png
--rw-r--r--   0 bart      (1000) bart      (1001)     3457 2024-05-12 05:49:11.000000 sbn-95/docs/manual.rst
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/docs/pdf/
--rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_Ack_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_T04_OTP-CR-117_19.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)    41559 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/Kamer.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)   323490 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/Rome-Statute.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-05-12 05:07:36.000000 sbn-95/docs/pdf/bevestigd.pdf
--rw-r--r--   0 bart      (1000) bart      (1001)     2196 2024-05-12 05:17:00.000000 sbn-95/docs/request.rst
--rw-r--r--   0 bart      (1000) bart      (1001)   179869 2024-05-12 05:07:36.000000 sbn-95/docs/skull.jpg
--rw-r--r--   0 bart      (1000) bart      (1001)   287102 2024-05-12 05:07:36.000000 sbn-95/docs/skull3.png
--rw-r--r--   0 bart      (1000) bart      (1001)      841 2024-05-12 05:20:24.000000 sbn-95/docs/source.rst
--rw-r--r--   0 bart      (1000) bart      (1001)      176 2024-05-12 05:17:00.000000 sbn-95/docs/verbatim.rst
--rw-r--r--   0 bart      (1000) bart      (1001)   256611 2024-05-12 05:51:27.000000 sbn-95/docs/verbatim6.png
--rw-r--r--   0 bart      (1000) bart      (1001)    46476 2024-05-12 05:07:36.000000 sbn-95/docs/wallpaper.png
--rw-r--r--   0 bart      (1000) bart      (1001)     1183 2024-05-12 05:17:00.000000 sbn-95/docs/writings.rst
--rw-r--r--   0 bart      (1000) bart      (1001)     2102 2024-05-12 05:55:43.000000 sbn-95/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/sbn/
--rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:08:36.000000 sbn-95/sbn/__init__.py
--rwxr-xr-x   0 bart      (1000) bart      (1001)     3913 2024-05-12 05:37:03.000000 sbn-95/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:08:36.000000 sbn-95/sbn/broker.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:08:36.000000 sbn-95/sbn/client.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:08:36.000000 sbn-95/sbn/disk.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:08:36.000000 sbn-95/sbn/find.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:08:36.000000 sbn-95/sbn/handler.py
--rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:08:36.000000 sbn-95/sbn/log.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.304195 sbn-95/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1001)      355 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-12 05:08:41.000000 sbn-95/sbn/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:08:36.000000 sbn-95/sbn/object.py
--rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:08:36.000000 sbn-95/sbn/run.py
--rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:08:36.000000 sbn-95/sbn/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-12 05:56:48.300195 sbn-95/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1001)     1327 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1001)       74 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-12 05:56:48.000000 sbn-95/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-12 05:56:48.304195 sbn-95/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1001)      192 2024-05-12 05:07:36.000000 sbn-95/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 02:46:23.707057 sbn-96/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1932 2024-05-12 05:45:59.000000 sbn-96/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/
+-rw-r--r--   0 bart      (1000) bart      (1001)   180711 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   193757 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   197697 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   232313 2024-05-12 05:07:36.000000 sbn-96/docs/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   245670 2024-05-12 05:07:36.000000 sbn-96/docs/OTP1.png
+-rw-r--r--   0 bart      (1000) bart      (1001)   238095 2024-05-12 05:07:36.000000 sbn-96/docs/OTP2.png
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/_static/
+-rw-r--r--   0 bart      (1000) bart      (1001)     1000 2024-05-12 05:07:36.000000 sbn-96/docs/_static/sbn.css
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/_templates/
+-rw-r--r--   0 bart      (1000) bart      (1001)      291 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/base.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      543 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/class.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/mine.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)      879 2024-05-12 05:07:36.000000 sbn-96/docs/_templates/module.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1208 2024-05-13 02:30:34.000000 sbn-96/docs/about.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)  1685507 2024-05-12 05:07:36.000000 sbn-96/docs/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)     3603 2024-05-13 02:13:01.000000 sbn-96/docs/conf.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      600 2024-05-12 05:17:00.000000 sbn-96/docs/evidence.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    47740 2024-05-13 02:42:11.000000 sbn-96/docs/genocide.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      364 2024-05-12 05:17:00.000000 sbn-96/docs/guilty.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     2068 2024-05-13 02:15:41.000000 sbn-96/docs/index.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)    69979 2024-05-12 05:07:36.000000 sbn-96/docs/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1001)   228393 2024-05-12 05:07:36.000000 sbn-96/docs/kamer.png
+-rw-r--r--   0 bart      (1000) bart      (1001)     3457 2024-05-12 05:49:11.000000 sbn-96/docs/manual.rst
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.703057 sbn-96/docs/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1001)   225470 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   238330 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   236671 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    41559 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)   323490 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)    50044 2024-05-12 05:07:36.000000 sbn-96/docs/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1001)     2196 2024-05-12 05:17:00.000000 sbn-96/docs/request.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)       23 2024-05-12 05:07:36.000000 sbn-96/docs/robots.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)   287102 2024-05-12 05:07:36.000000 sbn-96/docs/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1001)      841 2024-05-12 05:20:24.000000 sbn-96/docs/source.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1183 2024-05-12 05:17:00.000000 sbn-96/docs/writings.rst
+-rw-r--r--   0 bart      (1000) bart      (1001)     1980 2024-05-13 02:44:16.000000 sbn-96/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1001)       62 2024-05-12 05:08:36.000000 sbn-96/sbn/__init__.py
+-rwxr-xr-x   0 bart      (1000) bart      (1001)     3913 2024-05-13 02:19:42.000000 sbn-96/sbn/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      704 2024-05-12 05:08:36.000000 sbn-96/sbn/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4219 2024-05-12 05:08:36.000000 sbn-96/sbn/client.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2328 2024-05-12 05:08:36.000000 sbn-96/sbn/disk.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1954 2024-05-12 05:08:36.000000 sbn-96/sbn/find.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2110 2024-05-12 05:08:36.000000 sbn-96/sbn/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      490 2024-05-12 05:08:36.000000 sbn-96/sbn/log.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1001)      355 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      190 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      351 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    18777 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      694 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      385 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     2354 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1001)    10762 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1123 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1001)      991 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     5163 2024-05-12 05:08:41.000000 sbn-96/sbn/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     6168 2024-05-12 05:08:36.000000 sbn-96/sbn/object.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     1421 2024-05-12 05:08:36.000000 sbn-96/sbn/run.py
+-rw-r--r--   0 bart      (1000) bart      (1001)     4209 2024-05-12 05:08:36.000000 sbn-96/sbn/thread.py
+drwxr-xr-x   0 bart      (1000) bart      (1001)        0 2024-05-13 02:46:23.707057 sbn-96/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1001)     2494 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1001)     1240 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)       74 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        7 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        4 2024-05-13 02:46:23.000000 sbn-96/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1001)        1 2024-05-13 02:46:03.000000 sbn-96/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1001)       38 2024-05-13 02:46:23.707057 sbn-96/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1001)      192 2024-05-12 05:07:36.000000 sbn-96/setup.py
```

### Comparing `sbn-95/PKG-INFO` & `sbn-96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 95
+Version: 96
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-95/README.rst` & `sbn-96/README.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/ECHAabilify.png` & `sbn-96/docs/ECHAabilify.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/ECHAclozapine.png` & `sbn-96/docs/ECHAclozapine.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/ECHAhaldol.png` & `sbn-96/docs/ECHAhaldol.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/ECHAzyprexa.png` & `sbn-96/docs/ECHAzyprexa.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/OTP1.png` & `sbn-96/docs/OTP1.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/OTP2.png` & `sbn-96/docs/OTP2.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/_static/sbn.css` & `sbn-96/docs/_static/sbn.css`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/_templates/class.rst` & `sbn-96/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/_templates/mine.rst` & `sbn-96/docs/_templates/mine.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/_templates/module.rst` & `sbn-96/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/about.rst` & `sbn-96/docs/about.rst`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 Using poison makes the care laws used in the netherlands to provide
 care to elderly and handicapped, criminals and psychiatric patients
 not care laws but genocide laws with which the king is killing groups
 of the population by giving them poison instead of medicine in
 the "care" they are forced to undergo.
 
 I wrote the prosecutor asking for an arrest of the king (make him
-stop), the prosecutor decided to call it a "no basis to proceed".
+stop), the prosecutor decided to call it a "no basis to proceed", reference
+``OTP-CR-117/19``.
+
 
 .. raw:: html
 
     <br><br>
     <center>
     <b>
```

### Comparing `sbn-95/docs/bevestigd.jpg` & `sbn-96/docs/bevestigd.jpg`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/conf.py` & `sbn-96/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     'link': '#000',
     'link_hover': '#000',
     'nosidebar': True,
     'show_powered_by': False,
     'show_relbar_top': False,
     'sidebar_width': 10,
 }
-html_favicon = "skull.jpg"
+html_favicon = "skull3.png"
 html_extra_path = []
 html_last_updated_fmt = '%Y-%b-%d'
 html_additional_pages = {}
 html_domain_indices = False
 html_use_index = False
 html_split_index = False
 html_show_sourcelink = False
@@ -132,20 +132,18 @@
     </i>
     </center>
 '''
 
 rst_epilog = '''.. raw:: html
 
     <br>
-    <br>
-    <br>
     <center>
     <b>
 
-:ref:`about <about>` - :ref:`writings <writings>` - :ref:`evidence <evidence>` - :ref:`guilty <guilty>` - :ref:`reconsider <reconsider>` - :ref:`manual <manual>`
+:ref:`about <about>`  - :ref:`evidence <evidence>` - :ref:`guilty <guilty>` - :ref:`writings <writings>` - :ref:`reconsider <reconsider>`
 
 
 .. raw:: html
 
     </b>
     </center>
```

### Comparing `sbn-95/docs/evidence.rst` & `sbn-96/docs/evidence.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/genocide.png` & `sbn-96/docs/genocide.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/index.rst` & `sbn-96/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,23 @@
 .. raw:: html
 
     <br>
 
 .. title:: Reconsider
 
 
-.. raw:: html
-
-    <center><b>RECONSIDER</b></center>
-    <br>
-
-
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands** 
 |
 
 
-Hello Office of the Prosecutor, ``OTP-CR-117/19``
+Hello Office of the Prosecutor,
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute. 
 
 The dutch government has introduced three new forced care laws, the Wfz 
@@ -66,13 +60,12 @@
 were aware that these medicine are poison at the time they voted for this law
 and the day the Wfz law took effect (1-1-2019), i ask the prosecutor to
 prosecute the king for making the commiting of the above mentioned crimes
 (killing, torture and impotent making) possible here in the netherlands in
 the hope that it stops the mass torture with poison the king of the 
 netherlands and his government are doing.
 
-
 .. toctree::
     :hidden:
     :glob:
 
-    *
+    *
```

### Comparing `sbn-95/docs/informed.jpg` & `sbn-96/docs/informed.jpg`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/kamer.png` & `sbn-96/docs/kamer.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/manual.rst` & `sbn-96/docs/manual.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/EM_Ack_OTP-CR-117_19.pdf` & `sbn-96/docs/pdf/EM_Ack_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/EM_T04_OTP-CR-117_19.pdf` & `sbn-96/docs/pdf/EM_T04_OTP-CR-117_19.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf` & `sbn-96/docs/pdf/EM_T07_OTP-CR-117_19_001.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/Kamer.pdf` & `sbn-96/docs/pdf/Kamer.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/Rome-Statute.pdf` & `sbn-96/docs/pdf/Rome-Statute.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/pdf/bevestigd.pdf` & `sbn-96/docs/pdf/bevestigd.pdf`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/request.rst` & `sbn-96/docs/request.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/skull3.png` & `sbn-96/docs/skull3.png`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/source.rst` & `sbn-96/docs/source.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/docs/writings.rst` & `sbn-96/docs/writings.rst`

 * *Files identical despite different names*

### Comparing `sbn-95/pyproject.toml` & `sbn-96/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=43.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "sbn"
 description = "Skull, Bones and Number (OTP-CR-117/19)"
-version = "95"
+version = "96"
 authors = [
     {name = "Bart Thate", email = "bthate@dds.nl" },
 ]
 readme = "README.rst"
 license = { text="Public Domain"}
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -41,40 +41,35 @@
 ]
 zip-safe = true
 
 
 [tool.setuptools.data-files]
 "share/doc/sbn" = [
     "README.rst",
+    "docs/genocide.png",
     "docs/about.rst",
-    "docs/arrest.png",
     "docs/conf.py",
     "docs/ECHAhaldol.png",
     "docs/evidence.rst",
-    "docs/genocide.png",
     "docs/informed.jpg",
     "docs/OTP1.png",
-    "docs/skull.jpg",
     "docs/source.rst",
-    "docs/verbatim6.png",
-    "docs/banner.png",
     "docs/ECHAabilify.png",
     "docs/ECHAzyprexa.png",
     "docs/guilty.rst",
     "docs/kamer.png",
     "docs/OTP2.png",
     "docs/request.rst",
     "docs/skull3.png",
-    "docs/verbatim.rst",
     "docs/writings.rst",
     "docs/bevestigd.jpg",
     "docs/ECHAclozapine.png",
-    "docs/wallpaper.png",
     "docs/index.rst",
-    "docs/manual.rst"
+    "docs/manual.rst",
+    "docs/robots.txt"
 ]
 
 "share/doc/sbn/_static" = [
     "docs/_static/sbn.css",
 ]
 
 "share/doc/sbn/pdf" =  [
```

### Comparing `sbn-95/sbn/__main__.py` & `sbn-96/sbn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 Cfg             = Default()
 Cfg.dis         = ""
 Cfg.mod         = "cmd,err,log,mod,req,tdo,thr,tmr"
 Cfg.opts        = ""
 Cfg.name        = "sbn"
-Cfg.version     = "95"
+Cfg.version     = "96"
 Cfg.wdr         = os.path.expanduser(f"~/.{Cfg.name}")
 Cfg.pidfile     = os.path.join(Cfg.wdr, f"{Cfg.name}.pid")
 
 
 Workdir.workdir = Cfg.wdr
```

### Comparing `sbn-95/sbn/broker.py` & `sbn-96/sbn/broker.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/client.py` & `sbn-96/sbn/client.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/disk.py` & `sbn-96/sbn/disk.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/find.py` & `sbn-96/sbn/find.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/handler.py` & `sbn-96/sbn/handler.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/irc.py` & `sbn-96/sbn/modules/irc.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/log.py` & `sbn-96/sbn/modules/log.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/req.py` & `sbn-96/sbn/modules/req.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/rss.py` & `sbn-96/sbn/modules/rss.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/tdo.py` & `sbn-96/sbn/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/thr.py` & `sbn-96/sbn/modules/thr.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/modules/tmr.py` & `sbn-96/sbn/modules/tmr.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/object.py` & `sbn-96/sbn/object.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/run.py` & `sbn-96/sbn/run.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn/thread.py` & `sbn-96/sbn/thread.py`

 * *Files identical despite different names*

### Comparing `sbn-95/sbn.egg-info/PKG-INFO` & `sbn-96/sbn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 95
+Version: 96
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-95/sbn.egg-info/SOURCES.txt` & `sbn-96/sbn.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,27 @@
 docs/ECHAabilify.png
 docs/ECHAclozapine.png
 docs/ECHAhaldol.png
 docs/ECHAzyprexa.png
 docs/OTP1.png
 docs/OTP2.png
 docs/about.rst
-docs/arrest.png
-docs/banner.png
 docs/bevestigd.jpg
 docs/conf.py
 docs/evidence.rst
 docs/genocide.png
 docs/guilty.rst
 docs/index.rst
 docs/informed.jpg
 docs/kamer.png
 docs/manual.rst
 docs/request.rst
-docs/skull.jpg
+docs/robots.txt
 docs/skull3.png
 docs/source.rst
-docs/verbatim.rst
-docs/verbatim6.png
-docs/wallpaper.png
 docs/writings.rst
 docs/_static/sbn.css
 docs/_templates/base.rst
 docs/_templates/class.rst
 docs/_templates/mine.rst
 docs/_templates/module.rst
 docs/pdf/EM_Ack_OTP-CR-117_19.pdf
```

