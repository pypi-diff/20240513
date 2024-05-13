# Comparing `tmp/netsim_tools-1.8.1.post1.tar.gz` & `tmp/netsim_tools-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsim_tools-1.8.1.post1.tar", last modified: Wed Apr 24 08:34:00 2024, max compression
+gzip compressed data, was "netsim_tools-1.8.2.tar", last modified: Mon May 13 14:43:01 2024, max compression
```

## Comparing `netsim_tools-1.8.1.post1.tar` & `netsim_tools-1.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-24 08:33:44.000000 netsim_tools-1.8.1.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:34:00.698518 netsim_tools-1.8.1.post1/netsim_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:34:00.000000 netsim_tools-1.8.1.post1/netsim_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:34:00.702518 netsim_tools-1.8.1.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 08:33:44.000000 netsim_tools-1.8.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:43:01.348746 netsim_tools-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 14:43:01.348746 netsim_tools-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-13 14:42:41.000000 netsim_tools-1.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:43:01.348746 netsim_tools-1.8.2/netsim_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 14:43:01.000000 netsim_tools-1.8.2/netsim_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 14:43:01.000000 netsim_tools-1.8.2/netsim_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:43:01.000000 netsim_tools-1.8.2/netsim_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 14:43:01.000000 netsim_tools-1.8.2/netsim_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:43:01.000000 netsim_tools-1.8.2/netsim_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:43:01.348746 netsim_tools-1.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-13 14:42:41.000000 netsim_tools-1.8.2/setup.py
```

### Comparing `netsim_tools-1.8.1.post1/PKG-INFO` & `netsim_tools-1.8.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.1.post1
+Version: 1.8.2
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
-Requires-Dist: networklab>=1.8.1-post1
+Requires-Dist: networklab>=1.8.2
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim_tools-1.8.1.post1/netsim_tools.egg-info/PKG-INFO` & `netsim_tools-1.8.2/netsim_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: netsim-tools
-Version: 1.8.1.post1
+Version: 1.8.2
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Requires-Python: >=3.8
-Requires-Dist: networklab>=1.8.1-post1
+Requires-Dist: networklab>=1.8.2
 
 netsim-tools has been renamed to netlab in August 2022.
 
 The Python package netsim-tools has been renamed to networklab and is
 installed as a dependency of netsim-tools every time you install or
 upgrade netsim-tools, but we won't keep that dependency active foreer.
```

### Comparing `netsim_tools-1.8.1.post1/setup.py` & `netsim_tools-1.8.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ redirect netsim-tools to networklab """
 import sys
 from setuptools import setup, find_packages
 from pathlib import Path
 
 sys.path.append('..')
 
-version="1.8.1-post1"
+version="1.8.2"
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
   name="netsim-tools",
   version=version,
   packages=[],
```

