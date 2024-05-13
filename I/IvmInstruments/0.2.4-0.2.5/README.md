# Comparing `tmp/ivminstruments-0.2.4.tar.gz` & `tmp/ivminstruments-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivminstruments-0.2.4.tar", last modified: Mon May 13 14:32:57 2024, max compression
+gzip compressed data, was "ivminstruments-0.2.5.tar", last modified: Mon May 13 14:40:04 2024, max compression
```

## Comparing `ivminstruments-0.2.4.tar` & `ivminstruments-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:32:57.605599 ivminstruments-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:32:57.605599 ivminstruments-0.2.4/Instruments/
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/DigitalScope.py
--rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/KeySight_N670x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/KeySight_RP7954.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/Keysight_34461.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/Keysight_E362x.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/Instruments/multimeter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:32:57.605599 ivminstruments-0.2.4/IvmInstruments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 14:32:57.000000 ivminstruments-0.2.4/IvmInstruments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 14:32:57.000000 ivminstruments-0.2.4/IvmInstruments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:32:57.000000 ivminstruments-0.2.4/IvmInstruments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:32:57.000000 ivminstruments-0.2.4/IvmInstruments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-13 14:32:57.605599 ivminstruments-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:32:57.605599 ivminstruments-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 14:32:49.000000 ivminstruments-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/Instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/DigitalScope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/KeySight_N670x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/KeySight_RP7954.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/Keysight_34461.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/Keysight_E362x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/multimeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/IvmInstruments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/setup.py
```

### Comparing `ivminstruments-0.2.4/Instruments/DigitalScope.py` & `ivminstruments-0.2.5/Instruments/DigitalScope.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/Instruments/KeySight_N670x.py` & `ivminstruments-0.2.5/Instruments/KeySight_N670x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/Instruments/KeySight_RP7954.py` & `ivminstruments-0.2.5/Instruments/KeySight_RP7954.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/Instruments/Keysight_34461.py` & `ivminstruments-0.2.5/Instruments/Keysight_34461.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/Instruments/Keysight_E362x.py` & `ivminstruments-0.2.5/Instruments/Keysight_E362x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/Instruments/multimeter.py` & `ivminstruments-0.2.5/Instruments/multimeter.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.4/LICENSE` & `ivminstruments-0.2.5/LICENSE`

 * *Files identical despite different names*

