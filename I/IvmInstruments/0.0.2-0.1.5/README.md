# Comparing `tmp/IvmInstruments-0.0.2.tar.gz` & `tmp/IvmInstruments-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IvmInstruments-0.0.2.tar", last modified: Mon May 13 11:20:12 2024, max compression
+gzip compressed data, was "IvmInstruments-0.1.5.tar", last modified: Mon May 13 11:27:01 2024, max compression
```

## Comparing `IvmInstruments-0.0.2.tar` & `IvmInstruments-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 11:20:12.063717 IvmInstruments-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-13 11:20:12.019045 IvmInstruments-0.0.2/IvmInstruments.egg-info/
--rw-rw-rw-   0        0        0      525 2024-05-13 11:20:11.000000 IvmInstruments-0.0.2/IvmInstruments.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-05-13 11:20:11.000000 IvmInstruments-0.0.2/IvmInstruments.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 11:20:11.000000 IvmInstruments-0.0.2/IvmInstruments.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-13 11:20:11.000000 IvmInstruments-0.0.2/IvmInstruments.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-13 11:20:11.000000 IvmInstruments-0.0.2/IvmInstruments.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1103 2024-05-09 13:09:14.000000 IvmInstruments-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      525 2024-05-13 11:20:12.063717 IvmInstruments-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-09 13:09:14.000000 IvmInstruments-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 11:20:12.063717 IvmInstruments-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      895 2024-05-13 11:19:30.000000 IvmInstruments-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 11:20:12.057093 IvmInstruments-0.0.2/src/
--rw-rw-rw-   0        0        0     4894 2024-05-07 08:11:02.000000 IvmInstruments-0.0.2/src/DigitalScope.py
--rw-rw-rw-   0        0        0    23545 2024-05-07 08:11:02.000000 IvmInstruments-0.0.2/src/KeySight_N670x.py
--rw-rw-rw-   0        0        0     2777 2024-05-07 08:11:02.000000 IvmInstruments-0.0.2/src/KeySight_RP7954.py
--rw-rw-rw-   0        0        0    12743 2024-05-07 08:11:02.000000 IvmInstruments-0.0.2/src/Keysight_34461.py
--rw-rw-rw-   0        0        0     3139 2024-05-07 08:11:02.000000 IvmInstruments-0.0.2/src/Keysight_E362x.py
--rw-rw-rw-   0        0        0      214 2024-05-13 10:49:43.000000 IvmInstruments-0.0.2/src/__init__.py
--rw-rw-rw-   0        0        0     5261 2024-05-09 13:15:43.000000 IvmInstruments-0.0.2/src/multimeter.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:27:01.143573 IvmInstruments-0.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-13 11:27:01.118099 IvmInstruments-0.1.5/Instruments/
+-rw-rw-rw-   0        0        0     4894 2024-05-07 08:11:02.000000 IvmInstruments-0.1.5/Instruments/DigitalScope.py
+-rw-rw-rw-   0        0        0    23545 2024-05-07 08:11:02.000000 IvmInstruments-0.1.5/Instruments/KeySight_N670x.py
+-rw-rw-rw-   0        0        0     2777 2024-05-07 08:11:02.000000 IvmInstruments-0.1.5/Instruments/KeySight_RP7954.py
+-rw-rw-rw-   0        0        0    12743 2024-05-07 08:11:02.000000 IvmInstruments-0.1.5/Instruments/Keysight_34461.py
+-rw-rw-rw-   0        0        0     3139 2024-05-07 08:11:02.000000 IvmInstruments-0.1.5/Instruments/Keysight_E362x.py
+-rw-rw-rw-   0        0        0      214 2024-05-13 10:49:43.000000 IvmInstruments-0.1.5/Instruments/__init__.py
+-rw-rw-rw-   0        0        0     5261 2024-05-09 13:15:43.000000 IvmInstruments-0.1.5/Instruments/multimeter.py
+drwxrwxrwx   0        0        0        0 2024-05-13 11:27:01.137181 IvmInstruments-0.1.5/IvmInstruments.egg-info/
+-rw-rw-rw-   0        0        0       84 2024-05-13 11:27:00.000000 IvmInstruments-0.1.5/IvmInstruments.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-05-13 11:27:00.000000 IvmInstruments-0.1.5/IvmInstruments.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 11:27:00.000000 IvmInstruments-0.1.5/IvmInstruments.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 11:27:00.000000 IvmInstruments-0.1.5/IvmInstruments.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1103 2024-05-09 13:09:14.000000 IvmInstruments-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       84 2024-05-13 11:27:01.140430 IvmInstruments-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2024-05-09 13:09:14.000000 IvmInstruments-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 11:27:01.143573 IvmInstruments-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      211 2024-05-13 11:26:31.000000 IvmInstruments-0.1.5/setup.py
```

### Comparing `IvmInstruments-0.0.2/LICENSE` & `IvmInstruments-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/DigitalScope.py` & `IvmInstruments-0.1.5/Instruments/DigitalScope.py`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/KeySight_N670x.py` & `IvmInstruments-0.1.5/Instruments/KeySight_N670x.py`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/KeySight_RP7954.py` & `IvmInstruments-0.1.5/Instruments/KeySight_RP7954.py`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/Keysight_34461.py` & `IvmInstruments-0.1.5/Instruments/Keysight_34461.py`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/Keysight_E362x.py` & `IvmInstruments-0.1.5/Instruments/Keysight_E362x.py`

 * *Files identical despite different names*

### Comparing `IvmInstruments-0.0.2/src/multimeter.py` & `IvmInstruments-0.1.5/Instruments/multimeter.py`

 * *Files identical despite different names*

