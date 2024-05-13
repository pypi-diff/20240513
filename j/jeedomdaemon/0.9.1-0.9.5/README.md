# Comparing `tmp/jeedomdaemon-0.9.1.tar.gz` & `tmp/jeedomdaemon-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeedomdaemon-0.9.1.tar", last modified: Mon May 13 08:37:58 2024, max compression
+gzip compressed data, was "jeedomdaemon-0.9.5.tar", last modified: Mon May 13 09:13:29 2024, max compression
```

## Comparing `jeedomdaemon-0.9.1.tar` & `jeedomdaemon-0.9.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/jeedomdaemon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/jeedomdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/jeedomdaemon/aio_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/jeedomdaemon/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/jeedomdaemon/base_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/jeedomdaemon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 08:37:58.000000 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 08:37:58.000000 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:37:58.000000 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 08:37:58.000000 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 08:37:58.000000 jeedomdaemon-0.9.1/jeedomdaemon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:58.162813 jeedomdaemon-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/tests/base_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-13 08:37:52.000000 jeedomdaemon-0.9.1/tests/base_daemon_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/jeedomdaemon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/aio_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/base_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/jeedomdaemon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-13 09:13:29.000000 jeedomdaemon-0.9.5/jeedomdaemon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:29.418749 jeedomdaemon-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/base_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-13 09:13:25.000000 jeedomdaemon-0.9.5/tests/base_daemon_test.py
```

### Comparing `jeedomdaemon-0.9.1/LICENSE` & `jeedomdaemon-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/PKG-INFO` & `jeedomdaemon-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.9.1
+Version: 0.9.5
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.9.1/README.md` & `jeedomdaemon-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/jeedomdaemon/aio_connector.py` & `jeedomdaemon-0.9.5/jeedomdaemon/aio_connector.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/jeedomdaemon/base_config.py` & `jeedomdaemon-0.9.5/jeedomdaemon/base_config.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/jeedomdaemon/base_daemon.py` & `jeedomdaemon-0.9.5/jeedomdaemon/base_daemon.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/jeedomdaemon/utils.py` & `jeedomdaemon-0.9.5/jeedomdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/jeedomdaemon.egg-info/PKG-INFO` & `jeedomdaemon-0.9.5/jeedomdaemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeedomdaemon
-Version: 0.9.1
+Version: 0.9.5
 Summary: A base to implement Jeedom daemon in python
 Home-page: https://github.com/Mips2648/jeedom-daemon-py
 Author: Mips
 License: MIT
 Keywords: JEEDOM,DAEMON,ASYNCIO
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `jeedomdaemon-0.9.1/setup.py` & `jeedomdaemon-0.9.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # pylint: disable=missing-module-docstring
+
 from setuptools import setup, find_packages
 
-__version__ = "0.9.1"
+__version__ = "0.9.5"
 
 setup(
     # Needed to silence warnings (and to be a worthwhile package)
     name='jeedomdaemon',
     url='https://github.com/Mips2648/jeedom-daemon-py',
     author='Mips',
     # author_email='',
```

### Comparing `jeedomdaemon-0.9.1/tests/base_config_test.py` & `jeedomdaemon-0.9.5/tests/base_config_test.py`

 * *Files identical despite different names*

### Comparing `jeedomdaemon-0.9.1/tests/base_daemon_test.py` & `jeedomdaemon-0.9.5/tests/base_daemon_test.py`

 * *Files identical despite different names*

