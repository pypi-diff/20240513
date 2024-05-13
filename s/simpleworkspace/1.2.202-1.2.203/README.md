# Comparing `tmp/simpleworkspace-1.2.202.tar.gz` & `tmp/simpleworkspace-1.2.203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleworkspace-1.2.202.tar", last modified: Fri May 10 12:06:45 2024, max compression
+gzip compressed data, was "simpleworkspace-1.2.203.tar", last modified: Mon May 13 19:54:50 2024, max compression
```

## Comparing `simpleworkspace-1.2.202.tar` & `simpleworkspace-1.2.203.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.189924 simpleworkspace-1.2.202/
--rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.202/MANIFEST.in
--rw-rw-rw-   0        0        0      148 2024-05-10 12:06:45.187055 simpleworkspace-1.2.202/PKG-INFO
--rw-rw-rw-   0        0        0      313 2024-05-10 12:05:21.000000 simpleworkspace-1.2.202/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-10 12:06:45.191014 simpleworkspace-1.2.202/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.791517 simpleworkspace-1.2.202/src/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.878572 simpleworkspace-1.2.202/src/simpleworkspace/
--rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.202/src/simpleworkspace/__init__.py
--rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.202/src/simpleworkspace/__lazyimporter__.py
--rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.202/src/simpleworkspace/app.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.904575 simpleworkspace-1.2.202/src/simpleworkspace/assets/
--rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.913676 simpleworkspace-1.2.202/src/simpleworkspace/assets/__pycache__/
--rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.800359 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.917547 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/alarms/
--rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/alarms/Siren.wav
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.930636 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/notifications/
--rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/notifications/Completed.wav
--rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/notifications/Error.wav
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.948022 simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/
--rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/ErrorCircle.png
--rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/InfoCircle.png
--rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/QuestionCircle.png
--rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/WarningCircle.png
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.958657 simpleworkspace-1.2.202/src/simpleworkspace/collections/
--rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/collections/__init__.py
--rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/collections/loader.py
--rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.202/src/simpleworkspace/collections/observables.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.973991 simpleworkspace-1.2.202/src/simpleworkspace/db/
--rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.202/src/simpleworkspace/db/__init__.py
--rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.202/src/simpleworkspace/db/dbfactory.py
--rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.202/src/simpleworkspace/db/fluentsqlbuilder.py
--rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/db/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.983307 simpleworkspace-1.2.202/src/simpleworkspace/gui/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/gui/__init__.py
--rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.202/src/simpleworkspace/gui/dialogs.py
--rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.202/src/simpleworkspace/gui/loader.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.999227 simpleworkspace-1.2.202/src/simpleworkspace/io/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.008524 simpleworkspace-1.2.202/src/simpleworkspace/io/audio/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/audio/__init__.py
--rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/audio/loader.py
--rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/audio/play.py
--rw-rw-rw-   0        0        0     5574 2024-05-10 07:59:18.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/directory.py
--rw-rw-rw-   0        0        0     2999 2024-05-09 18:37:59.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/file.py
--rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/loader.py
--rw-rw-rw-   0        0        0     6180 2024-05-10 07:32:00.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/path.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.024139 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/__init__.py
--rw-rw-rw-   0        0        0    13750 2024-05-10 12:05:01.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/archive.py
--rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/csvreader.py
--rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/loader.py
--rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.202/src/simpleworkspace/io/readers/logreader.py
--rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.202/src/simpleworkspace/loader.py
--rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.202/src/simpleworkspace/logproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.841981 simpleworkspace-1.2.202/src/simpleworkspace/packages/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.027563 simpleworkspace-1.2.202/src/simpleworkspace/packages/debug/
--rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/debug/profiler.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.831756 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:44.832750 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.034844 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/
--rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.038994 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/model/
--rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
--rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/server.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.041828 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.045671 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/
--rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.090591 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
--rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
--rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
--rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
--rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
--rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
--rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.098147 simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/
--rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/__init__.py
--rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/manager.py
--rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/model.py
--rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.202/src/simpleworkspace/settingsproviders.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.136087 simpleworkspace-1.2.202/src/simpleworkspace/types/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/__init__.py
--rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/byte.py
--rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/iunit.py
--rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/loader.py
--rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/measurement.py
--rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/os.py
--rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.202/src/simpleworkspace/types/time.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.177309 simpleworkspace-1.2.202/src/simpleworkspace/utility/
--rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/__init__.py
--rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/bytes.py
--rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/cache.py
--rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/console.py
--rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/linq.py
--rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/loader.py
--rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/module.py
--rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/parallel.py
--rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/progressbar.py
--rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/regex.py
--rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/strings.py
--rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.202/src/simpleworkspace/utility/time.py
-drwxrwxrwx   0        0        0        0 2024-05-10 12:06:45.179495 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/
--rw-rw-rw-   0        0        0      148 2024-05-10 12:06:44.000000 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2024-05-10 12:06:44.000000 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 12:06:44.000000 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-10 12:06:44.000000 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-10 12:06:44.000000 simpleworkspace-1.2.202/src/simpleworkspace.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.115351 simpleworkspace-1.2.203/
+-rw-rw-rw-   0        0        0       22 2024-01-29 16:35:42.000000 simpleworkspace-1.2.203/MANIFEST.in
+-rw-rw-rw-   0        0        0      148 2024-05-13 19:54:50.115351 simpleworkspace-1.2.203/PKG-INFO
+-rw-rw-rw-   0        0        0      313 2024-05-13 19:53:28.000000 simpleworkspace-1.2.203/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 19:54:50.128867 simpleworkspace-1.2.203/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.667208 simpleworkspace-1.2.203/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.754600 simpleworkspace-1.2.203/src/simpleworkspace/
+-rw-rw-rw-   0        0        0        0 2024-01-22 08:55:41.000000 simpleworkspace-1.2.203/src/simpleworkspace/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-12-11 19:38:16.000000 simpleworkspace-1.2.203/src/simpleworkspace/__lazyimporter__.py
+-rw-rw-rw-   0        0        0     2458 2024-02-05 17:50:15.000000 simpleworkspace-1.2.203/src/simpleworkspace/app.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.779943 simpleworkspace-1.2.203/src/simpleworkspace/assets/
+-rw-rw-rw-   0        0        0      561 2024-02-24 14:57:44.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.789185 simpleworkspace-1.2.203/src/simpleworkspace/assets/__pycache__/
+-rw-rw-rw-   0        0        0      658 2024-01-24 15:01:20.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      876 2024-02-24 15:09:13.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.678105 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.796406 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/alarms/
+-rw-rw-rw-   0        0        0   115582 2024-02-24 14:31:08.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/alarms/Siren.wav
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.825894 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/notifications/
+-rw-rw-rw-   0        0        0   168352 2024-02-24 14:26:13.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/notifications/Completed.wav
+-rw-rw-rw-   0        0        0   159276 2021-05-30 12:26:50.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/notifications/Error.wav
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.848028 simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/
+-rw-rw-rw-   0        0        0      864 2024-01-22 08:25:22.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/ErrorCircle.png
+-rw-rw-rw-   0        0        0      738 2024-01-22 09:30:40.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/InfoCircle.png
+-rw-rw-rw-   0        0        0      913 2024-01-22 08:25:22.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/QuestionCircle.png
+-rw-rw-rw-   0        0        0      643 2024-01-22 08:25:22.000000 simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/WarningCircle.png
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.860615 simpleworkspace-1.2.203/src/simpleworkspace/collections/
+-rw-rw-rw-   0        0        0        0 2023-12-06 00:49:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/collections/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-12-11 19:38:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/collections/loader.py
+-rw-rw-rw-   0        0        0     8357 2024-03-10 18:15:07.000000 simpleworkspace-1.2.203/src/simpleworkspace/collections/observables.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.869703 simpleworkspace-1.2.203/src/simpleworkspace/db/
+-rw-rw-rw-   0        0        0        0 2023-09-27 17:03:43.000000 simpleworkspace-1.2.203/src/simpleworkspace/db/__init__.py
+-rw-rw-rw-   0        0        0     1961 2023-11-10 09:43:08.000000 simpleworkspace-1.2.203/src/simpleworkspace/db/dbfactory.py
+-rw-rw-rw-   0        0        0    26868 2024-01-15 18:01:58.000000 simpleworkspace-1.2.203/src/simpleworkspace/db/fluentsqlbuilder.py
+-rw-rw-rw-   0        0        0      356 2023-12-11 19:38:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/db/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.897585 simpleworkspace-1.2.203/src/simpleworkspace/gui/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/gui/__init__.py
+-rw-rw-rw-   0        0        0    19745 2024-02-03 10:18:03.000000 simpleworkspace-1.2.203/src/simpleworkspace/gui/dialogs.py
+-rw-rw-rw-   0        0        0      199 2024-01-15 19:55:06.000000 simpleworkspace-1.2.203/src/simpleworkspace/gui/loader.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.918375 simpleworkspace-1.2.203/src/simpleworkspace/io/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.949683 simpleworkspace-1.2.203/src/simpleworkspace/io/audio/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/audio/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-02-24 14:54:39.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/audio/loader.py
+-rw-rw-rw-   0        0        0      720 2024-02-24 19:58:16.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/audio/play.py
+-rw-rw-rw-   0        0        0     5574 2024-05-10 07:59:18.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/directory.py
+-rw-rw-rw-   0        0        0     2999 2024-05-09 18:37:59.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/file.py
+-rw-rw-rw-   0        0        0      603 2024-05-09 18:37:59.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/loader.py
+-rw-rw-rw-   0        0        0     6180 2024-05-10 07:32:00.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/path.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.965026 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/__init__.py
+-rw-rw-rw-   0        0        0    13750 2024-05-12 06:37:39.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/archive.py
+-rw-rw-rw-   0        0        0     6265 2024-02-12 21:01:46.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/csvreader.py
+-rw-rw-rw-   0        0        0      423 2024-05-09 18:37:59.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/loader.py
+-rw-rw-rw-   0        0        0     2637 2024-02-25 08:00:45.000000 simpleworkspace-1.2.203/src/simpleworkspace/io/readers/logreader.py
+-rw-rw-rw-   0        0        0     1256 2024-01-19 14:38:39.000000 simpleworkspace-1.2.203/src/simpleworkspace/loader.py
+-rw-rw-rw-   0        0        0     6464 2024-01-27 23:46:02.000000 simpleworkspace-1.2.203/src/simpleworkspace/logproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.721064 simpleworkspace-1.2.203/src/simpleworkspace/packages/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.965026 simpleworkspace-1.2.203/src/simpleworkspace/packages/debug/
+-rw-rw-rw-   0        0        0     2163 2024-01-31 16:09:17.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/debug/profiler.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.707893 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.709898 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.980638 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/
+-rw-rw-rw-   0        0        0       71 2024-04-21 07:34:26.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:49.996245 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/model/
+-rw-rw-rw-   0        0        0     3293 2024-04-21 13:55:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py
+-rw-rw-rw-   0        0        0     9530 2024-04-21 14:05:03.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/server.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.011263 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.013063 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/
+-rw-rw-rw-   0        0        0        0 2024-01-27 17:48:10.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.031401 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/
+-rw-rw-rw-   0        0        0      717 2024-01-27 17:30:09.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py
+-rw-rw-rw-   0        0        0    38758 2024-01-27 17:30:16.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py
+-rw-rw-rw-   0        0        0     9974 2024-01-27 17:30:31.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py
+-rw-rw-rw-   0        0        0      348 2024-01-27 17:30:45.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/ordered.py
+-rw-rw-rw-   0        0        0      768 2023-10-11 00:54:10.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py
+-rw-rw-rw-   0        0        0     4889 2024-02-12 20:16:17.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.045628 simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/
+-rw-rw-rw-   0        0        0       79 2023-09-27 18:18:53.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/__init__.py
+-rw-rw-rw-   0        0        0     8955 2024-04-22 19:17:15.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/manager.py
+-rw-rw-rw-   0        0        0     5067 2024-04-22 19:17:15.000000 simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/model.py
+-rw-rw-rw-   0        0        0     7383 2024-02-12 20:00:46.000000 simpleworkspace-1.2.203/src/simpleworkspace/settingsproviders.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.069929 simpleworkspace-1.2.203/src/simpleworkspace/types/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/__init__.py
+-rw-rw-rw-   0        0        0     2996 2024-02-14 19:40:14.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/byte.py
+-rw-rw-rw-   0        0        0     5736 2023-09-27 18:18:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/iunit.py
+-rw-rw-rw-   0        0        0      471 2023-12-11 19:38:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/loader.py
+-rw-rw-rw-   0        0        0      932 2023-09-27 18:18:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/measurement.py
+-rw-rw-rw-   0        0        0      556 2024-03-09 13:42:06.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/os.py
+-rw-rw-rw-   0        0        0     8342 2024-04-22 19:22:13.000000 simpleworkspace-1.2.203/src/simpleworkspace/types/time.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.115351 simpleworkspace-1.2.203/src/simpleworkspace/utility/
+-rw-rw-rw-   0        0        0        0 2023-09-26 16:36:19.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-09-27 18:18:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/bytes.py
+-rw-rw-rw-   0        0        0     1916 2024-04-22 19:17:15.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/cache.py
+-rw-rw-rw-   0        0        0     7735 2024-02-08 17:57:55.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/console.py
+-rw-rw-rw-   0        0        0     3157 2024-05-13 19:52:32.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/encryption.py
+-rw-rw-rw-   0        0        0    14504 2024-04-25 16:58:27.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/linq.py
+-rw-rw-rw-   0        0        0      984 2023-12-11 19:38:54.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/loader.py
+-rw-rw-rw-   0        0        0     4548 2024-02-28 20:36:05.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/module.py
+-rw-rw-rw-   0        0        0     1798 2024-01-23 23:38:57.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/parallel.py
+-rw-rw-rw-   0        0        0    11207 2024-04-25 16:08:18.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/progressbar.py
+-rw-rw-rw-   0        0        0     7218 2024-02-20 06:25:57.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/regex.py
+-rw-rw-rw-   0        0        0     1897 2024-05-08 10:41:26.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/strings.py
+-rw-rw-rw-   0        0        0     6760 2024-04-22 19:17:15.000000 simpleworkspace-1.2.203/src/simpleworkspace/utility/time.py
+drwxrwxrwx   0        0        0        0 2024-05-13 19:54:50.115351 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/
+-rw-rw-rw-   0        0        0      148 2024-05-13 19:54:49.000000 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3514 2024-05-13 19:54:49.000000 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 19:54:49.000000 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 19:54:49.000000 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-13 19:54:49.000000 simpleworkspace-1.2.203/src/simpleworkspace.egg-info/top_level.txt
```

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/app.py` & `simpleworkspace-1.2.203/src/simpleworkspace/app.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/__init__.py` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/__pycache__/__init__.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/alarms/Siren.wav` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/alarms/Siren.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/notifications/Completed.wav` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/notifications/Completed.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/audio/notifications/Error.wav` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/audio/notifications/Error.wav`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/ErrorCircle.png` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/ErrorCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/InfoCircle.png` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/InfoCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/QuestionCircle.png` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/QuestionCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/assets/icons/WarningCircle.png` & `simpleworkspace-1.2.203/src/simpleworkspace/assets/icons/WarningCircle.png`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/collections/observables.py` & `simpleworkspace-1.2.203/src/simpleworkspace/collections/observables.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/db/dbfactory.py` & `simpleworkspace-1.2.203/src/simpleworkspace/db/dbfactory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/db/fluentsqlbuilder.py` & `simpleworkspace-1.2.203/src/simpleworkspace/db/fluentsqlbuilder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/gui/dialogs.py` & `simpleworkspace-1.2.203/src/simpleworkspace/gui/dialogs.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/audio/play.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/audio/play.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/directory.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/directory.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/file.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/file.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/loader.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/path.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/path.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/readers/archive.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/readers/archive.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/readers/csvreader.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/readers/csvreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/io/readers/logreader.py` & `simpleworkspace-1.2.203/src/simpleworkspace/io/readers/logreader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/loader.py` & `simpleworkspace-1.2.203/src/simpleworkspace/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/logproviders.py` & `simpleworkspace-1.2.203/src/simpleworkspace/logproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/debug/profiler.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/debug/profiler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/model/commobjects.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/network/servers/basicserver/server.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/network/servers/basicserver/server.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/__init__.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/decoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/encoder.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/dependecy/toml/tz.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/pythonbundlers/setuptoolsbundler.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/manager.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/manager.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/packages/taskscheduler/model.py` & `simpleworkspace-1.2.203/src/simpleworkspace/packages/taskscheduler/model.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/settingsproviders.py` & `simpleworkspace-1.2.203/src/simpleworkspace/settingsproviders.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/types/byte.py` & `simpleworkspace-1.2.203/src/simpleworkspace/types/byte.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/types/iunit.py` & `simpleworkspace-1.2.203/src/simpleworkspace/types/iunit.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/types/measurement.py` & `simpleworkspace-1.2.203/src/simpleworkspace/types/measurement.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/types/os.py` & `simpleworkspace-1.2.203/src/simpleworkspace/types/os.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/types/time.py` & `simpleworkspace-1.2.203/src/simpleworkspace/types/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/cache.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/cache.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/console.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/console.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/linq.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/linq.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/loader.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/loader.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/module.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/module.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/parallel.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/parallel.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/progressbar.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/progressbar.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/regex.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/regex.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/strings.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/strings.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace/utility/time.py` & `simpleworkspace-1.2.203/src/simpleworkspace/utility/time.py`

 * *Files identical despite different names*

### Comparing `simpleworkspace-1.2.202/src/simpleworkspace.egg-info/SOURCES.txt` & `simpleworkspace-1.2.203/src/simpleworkspace.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 src/simpleworkspace/types/measurement.py
 src/simpleworkspace/types/os.py
 src/simpleworkspace/types/time.py
 src/simpleworkspace/utility/__init__.py
 src/simpleworkspace/utility/bytes.py
 src/simpleworkspace/utility/cache.py
 src/simpleworkspace/utility/console.py
+src/simpleworkspace/utility/encryption.py
 src/simpleworkspace/utility/linq.py
 src/simpleworkspace/utility/loader.py
 src/simpleworkspace/utility/module.py
 src/simpleworkspace/utility/parallel.py
 src/simpleworkspace/utility/progressbar.py
 src/simpleworkspace/utility/regex.py
 src/simpleworkspace/utility/strings.py
```

