# Comparing `tmp/ivminstruments-0.2.5.tar.gz` & `tmp/ivminstruments-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivminstruments-0.2.5.tar", last modified: Mon May 13 14:40:04 2024, max compression
+gzip compressed data, was "ivminstruments-0.2.7.tar", last modified: Mon May 13 14:43:15 2024, max compression
```

## Comparing `ivminstruments-0.2.5.tar` & `ivminstruments-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/Instruments/
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/DigitalScope.py
--rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/KeySight_N670x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/KeySight_RP7954.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/Keysight_34461.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/Keysight_E362x.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/Instruments/multimeter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/IvmInstruments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:40:04.000000 ivminstruments-0.2.5/IvmInstruments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:40:04.376784 ivminstruments-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 14:39:56.000000 ivminstruments-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:43:15.114216 ivminstruments-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:43:15.110216 ivminstruments-0.2.7/Instruments/
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/DigitalScope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23077 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/KeySight_N670x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/KeySight_RP7954.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/Keysight_34461.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/Keysight_E362x.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/Instruments/multimeter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:43:15.110216 ivminstruments-0.2.7/IvmInstruments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:43:15.000000 ivminstruments-0.2.7/IvmInstruments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 14:43:15.000000 ivminstruments-0.2.7/IvmInstruments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:43:15.000000 ivminstruments-0.2.7/IvmInstruments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:43:15.000000 ivminstruments-0.2.7/IvmInstruments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 14:43:15.114216 ivminstruments-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:43:01.000000 ivminstruments-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:43:15.114216 ivminstruments-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-13 14:43:02.000000 ivminstruments-0.2.7/setup.py
```

### Comparing `ivminstruments-0.2.5/Instruments/DigitalScope.py` & `ivminstruments-0.2.7/Instruments/DigitalScope.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/Instruments/KeySight_N670x.py` & `ivminstruments-0.2.7/Instruments/KeySight_N670x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/Instruments/KeySight_RP7954.py` & `ivminstruments-0.2.7/Instruments/KeySight_RP7954.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/Instruments/Keysight_34461.py` & `ivminstruments-0.2.7/Instruments/Keysight_34461.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/Instruments/Keysight_E362x.py` & `ivminstruments-0.2.7/Instruments/Keysight_E362x.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/Instruments/multimeter.py` & `ivminstruments-0.2.7/Instruments/multimeter.py`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/LICENSE` & `ivminstruments-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ivminstruments-0.2.5/setup.py` & `ivminstruments-0.2.7/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 AUTHOR_USER_NAME = 'HarishKumarSedu'
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'Instruments'
 setup(
     name=f'Ivm{REPO_NAME}',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.2.5',
+    version='0.2.7',
     py_modules=['Instruments'],
-    description=[ 'text/x-rst','text/markdown'],
+    description=[ 'text/markdown','text/x-rst',],
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     long_description=long_description,
     packages=find_packages(),
     include_dirs=['Instruments'],
```

