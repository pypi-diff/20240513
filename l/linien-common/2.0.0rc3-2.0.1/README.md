# Comparing `tmp/linien-common-2.0.0rc3.tar.gz` & `tmp/linien_common-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linien-common-2.0.0rc3.tar", last modified: Fri Apr  5 14:08:55 2024, max compression
+gzip compressed data, was "linien_common-2.0.1.tar", last modified: Mon May 13 15:17:57 2024, max compression
```

## Comparing `linien-common-2.0.0rc3.tar` & `linien_common-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:08:55.578033 linien-common-2.0.0rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 14:08:55.578033 linien-common-2.0.0rc3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:08:55.574032 linien-common-2.0.0rc3/linien_common/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/linien_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/linien_common/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/linien_common/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/linien_common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/linien_common/influxdb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:08:55.578033 linien-common-2.0.0rc3/linien_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-05 14:08:55.000000 linien-common-2.0.0rc3/linien_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-05 14:08:55.000000 linien-common-2.0.0rc3/linien_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:08:55.000000 linien-common-2.0.0rc3/linien_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 14:08:55.000000 linien-common-2.0.0rc3/linien_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 14:08:55.000000 linien-common-2.0.0rc3/linien_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-05 14:08:46.000000 linien-common-2.0.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:08:55.578033 linien-common-2.0.0rc3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:17:57.801398 linien_common-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 15:17:57.801398 linien_common-2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:17:57.801398 linien_common-2.0.1/linien_common/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-13 15:17:51.000000 linien_common-2.0.1/linien_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9767 2024-05-13 15:17:51.000000 linien_common-2.0.1/linien_common/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-13 15:17:51.000000 linien_common-2.0.1/linien_common/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-13 15:17:51.000000 linien_common-2.0.1/linien_common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-05-13 15:17:51.000000 linien_common-2.0.1/linien_common/influxdb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:17:57.801398 linien_common-2.0.1/linien_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 15:17:57.000000 linien_common-2.0.1/linien_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-13 15:17:57.000000 linien_common-2.0.1/linien_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:17:57.000000 linien_common-2.0.1/linien_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-13 15:17:57.000000 linien_common-2.0.1/linien_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 15:17:57.000000 linien_common-2.0.1/linien_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-05-13 15:17:51.000000 linien_common-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:17:57.801398 linien_common-2.0.1/setup.cfg
```

### Comparing `linien-common-2.0.0rc3/PKG-INFO` & `linien_common-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.0rc3
+Version: 2.0.1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien-common-2.0.0rc3/linien_common/__init__.py` & `linien_common-2.0.1/linien_common/__init__.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc3/linien_common/common.py` & `linien_common-2.0.1/linien_common/common.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc3/linien_common/communication.py` & `linien_common-2.0.1/linien_common/communication.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc3/linien_common/config.py` & `linien_common-2.0.1/linien_common/config.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc3/linien_common/influxdb.py` & `linien_common-2.0.1/linien_common/influxdb.py`

 * *Files identical despite different names*

### Comparing `linien-common-2.0.0rc3/linien_common.egg-info/PKG-INFO` & `linien_common-2.0.1/linien_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linien-common
-Version: 2.0.0rc3
+Version: 2.0.1
 Summary: Shared components of the Linien spectroscopy lock application.
 Author-email: Benjamin Wiegand <benjamin.wiegand@physik.hu-berlin.de>, Bastian Leykauf <leykauf@physik.hu-berlin.de>, Robert Jördens <rj@quartiq.de>, Christian Freier <christian.freier@gmail.com>, Doron Behar <doron.behar@gmail.com>
 Maintainer-email: Bastian Leykauf <leykauf@physik.hu-berlin.de>
 Project-URL: Homepage, https://github.com/linien-org/linien
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `linien-common-2.0.0rc3/pyproject.toml` & `linien_common-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linien-common"
-version = "2.0.0rc3"
+version = "2.0.1"
 authors = [
     { name = "Benjamin Wiegand", email = "benjamin.wiegand@physik.hu-berlin.de" },
     { name = "Bastian Leykauf", email = "leykauf@physik.hu-berlin.de" },
     { name = "Robert Jördens", email = "rj@quartiq.de" },
     { name = "Christian Freier", email = "christian.freier@gmail.com" },
     { name = "Doron Behar", email = "doron.behar@gmail.com" },
 ]
```

