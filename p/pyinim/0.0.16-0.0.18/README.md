# Comparing `tmp/pyinim-0.0.16.tar.gz` & `tmp/pyinim-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinim-0.0.16.tar", last modified: Sat May 11 19:34:14 2024, max compression
+gzip compressed data, was "pyinim-0.0.18.tar", last modified: Mon May 13 21:58:58 2024, max compression
```

## Comparing `pyinim-0.0.16.tar` & `pyinim-0.0.18.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.927485 pyinim-0.0.16/
--rw-r--r--   0 bertulla (1473677006) 52240112    35149 2024-04-27 20:46:49.000000 pyinim-0.0.16/LICENSE
--rw-r--r--   0 bertulla (1473677006) 52240112     3471 2024-05-11 19:34:14.927403 pyinim-0.0.16/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112     2846 2024-05-11 19:32:04.000000 pyinim-0.0.16/README.md
--rw-r--r--   0 bertulla (1473677006) 52240112      621 2024-05-11 19:33:17.000000 pyinim-0.0.16/pyproject.toml
--rw-r--r--   0 bertulla (1473677006) 52240112      418 2024-05-11 19:34:14.927745 pyinim-0.0.16/setup.cfg
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.924408 pyinim-0.0.16/src/
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.925346 pyinim-0.0.16/src/pyinim/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/__init__.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.926376 pyinim-0.0.16/src/pyinim/cloud/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/cloud/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2465 2024-05-11 19:32:04.000000 pyinim-0.0.16/src/pyinim/cloud/abc.py
--rw-r--r--   0 bertulla (1473677006) 52240112      195 2024-05-11 19:32:04.000000 pyinim-0.0.16/src/pyinim/cloud/exceptions.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2599 2024-05-11 19:32:04.000000 pyinim-0.0.16/src/pyinim/cloud/resolver.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.926713 pyinim-0.0.16/src/pyinim/cloud/types/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/cloud/types/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     2304 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/cloud/types/devices.py
--rw-r--r--   0 bertulla (1473677006) 52240112      489 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/cloud/types/token.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.926935 pyinim-0.0.16/src/pyinim/examples/
--rw-r--r--   0 bertulla (1473677006) 52240112        0 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/examples/__init__.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1390 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/examples/poc.py
--rw-r--r--   0 bertulla (1473677006) 52240112     1584 2024-05-07 10:55:00.000000 pyinim-0.0.16/src/pyinim/inim_cloud.py
-drwxr-xr-x   0 bertulla (1473677006) 52240112        0 2024-05-11 19:34:14.927100 pyinim-0.0.16/src/pyinim.egg-info/
--rw-r--r--   0 bertulla (1473677006) 52240112     3471 2024-05-11 19:34:14.000000 pyinim-0.0.16/src/pyinim.egg-info/PKG-INFO
--rw-r--r--   0 bertulla (1473677006) 52240112      532 2024-05-11 19:34:14.000000 pyinim-0.0.16/src/pyinim.egg-info/SOURCES.txt
--rw-r--r--   0 bertulla (1473677006) 52240112        1 2024-05-11 19:34:14.000000 pyinim-0.0.16/src/pyinim.egg-info/dependency_links.txt
--rw-r--r--   0 bertulla (1473677006) 52240112       53 2024-05-11 19:34:14.000000 pyinim-0.0.16/src/pyinim.egg-info/requires.txt
--rw-r--r--   0 bertulla (1473677006) 52240112        7 2024-05-11 19:34:14.000000 pyinim-0.0.16/src/pyinim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.012733 pyinim-0.0.18/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 21:58:53.000000 pyinim-0.0.18/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-13 21:58:58.012733 pyinim-0.0.18/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 21:58:53.000000 pyinim-0.0.18/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-13 21:58:53.000000 pyinim-0.0.18/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 21:58:58.012733 pyinim-0.0.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.008733 pyinim-0.0.18/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.008733 pyinim-0.0.18/src/pyinim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.012733 pyinim-0.0.18/src/pyinim/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.012733 pyinim-0.0.18/src/pyinim/cloud/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/types/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/cloud/types/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.012733 pyinim-0.0.18/src/pyinim/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/examples/poc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 21:58:53.000000 pyinim-0.0.18/src/pyinim/inim_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:58:58.012733 pyinim-0.0.18/src/pyinim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-13 21:58:58.000000 pyinim-0.0.18/src/pyinim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-13 21:58:58.000000 pyinim-0.0.18/src/pyinim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:58:58.000000 pyinim-0.0.18/src/pyinim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 21:58:58.000000 pyinim-0.0.18/src/pyinim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 21:58:58.000000 pyinim-0.0.18/src/pyinim.egg-info/top_level.txt
```

### Comparing `pyinim-0.0.16/LICENSE` & `pyinim-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/PKG-INFO` & `pyinim-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.16
+Version: 0.0.18
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyinim-0.0.16/README.md` & `pyinim-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/pyproject.toml` & `pyinim-0.0.18/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyinim"
-version = "0.0.16"
+version = "0.0.18"
 authors = [
   { name="Antonino Bertulla", email="abertulla@email.address" },
 ]
 description = "A Inim Cloud API client"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `pyinim-0.0.16/src/pyinim/cloud/abc.py` & `pyinim-0.0.18/src/pyinim/cloud/abc.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/src/pyinim/cloud/resolver.py` & `pyinim-0.0.18/src/pyinim/cloud/resolver.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/src/pyinim/cloud/types/devices.py` & `pyinim-0.0.18/src/pyinim/cloud/types/devices.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/src/pyinim/examples/poc.py` & `pyinim-0.0.18/src/pyinim/examples/poc.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/src/pyinim/inim_cloud.py` & `pyinim-0.0.18/src/pyinim/inim_cloud.py`

 * *Files identical despite different names*

### Comparing `pyinim-0.0.16/src/pyinim.egg-info/PKG-INFO` & `pyinim-0.0.18/src/pyinim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinim
-Version: 0.0.16
+Version: 0.0.18
 Summary: A Inim Cloud API client
 Home-page: https://github.com/nidble/pyinim
 Author: Antonino Bertulla
 Author-email: Antonino Bertulla <abertulla@email.address>
 Project-URL: Homepage, https://github.com/nidble/pyinim
 Project-URL: Issues, https://github.com/nidble/pyinim/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyinim-0.0.16/src/pyinim.egg-info/SOURCES.txt` & `pyinim-0.0.18/src/pyinim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

