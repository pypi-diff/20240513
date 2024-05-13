# Comparing `tmp/kaas_cli-0.1.6.tar.gz` & `tmp/kaas_cli-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaas_cli-0.1.6.tar", max compression
+gzip compressed data, was "kaas_cli-0.1.7.tar", max compression
```

## Comparing `kaas_cli-0.1.6.tar` & `kaas_cli-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/LICENSE
--rw-r--r--   0        0        0     1639 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/README.md
--rw-r--r--   0        0        0     1628 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       48 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/__init__.py
--rw-r--r--   0        0        0     1253 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/__main__.py
--rw-r--r--   0        0        0     7916 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/cli.py
--rw-r--r--   0        0        0    23212 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/client.py
--rw-r--r--   0        0        0     1139 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/config.py
--rw-r--r--   0        0        0      945 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/constants.py
--rw-r--r--   0        0        0       58 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/hello.py
--rw-r--r--   0        0        0        0 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/py.typed
--rw-r--r--   0        0        0      884 2024-05-10 21:42:32.832005 kaas_cli-0.1.6/src/kaas_cli/types.py
--rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 kaas_cli-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-13 20:07:50.268646 kaas_cli-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1639 2024-05-13 20:07:50.268646 kaas_cli-0.1.7/README.md
+-rw-r--r--   0        0        0     1628 2024-05-13 20:07:50.268646 kaas_cli-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-05-13 20:07:50.268646 kaas_cli-0.1.7/src/kaas_cli/__init__.py
+-rw-r--r--   0        0        0     1253 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/__main__.py
+-rw-r--r--   0        0        0     7916 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/cli.py
+-rw-r--r--   0        0        0    23212 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/client.py
+-rw-r--r--   0        0        0     1139 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/config.py
+-rw-r--r--   0        0        0      945 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/constants.py
+-rw-r--r--   0        0        0       58 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/hello.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/py.typed
+-rw-r--r--   0        0        0      884 2024-05-13 20:07:50.272646 kaas_cli-0.1.7/src/kaas_cli/types.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 kaas_cli-0.1.7/PKG-INFO
```

### Comparing `kaas_cli-0.1.6/LICENSE` & `kaas_cli-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/README.md` & `kaas_cli-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/pyproject.toml` & `kaas_cli-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kaas-cli"
-version = "0.1.6"
+version = "0.1.7"
 description = "Command line utility for K as a Service"
 authors = [
     "Runtime Verification, Inc. <contact@runtimeverification.com>",
 ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `kaas_cli-0.1.6/src/kaas_cli/__main__.py` & `kaas_cli-0.1.7/src/kaas_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/src/kaas_cli/cli.py` & `kaas_cli-0.1.7/src/kaas_cli/cli.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/src/kaas_cli/client.py` & `kaas_cli-0.1.7/src/kaas_cli/client.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/src/kaas_cli/config.py` & `kaas_cli-0.1.7/src/kaas_cli/config.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/src/kaas_cli/constants.py` & `kaas_cli-0.1.7/src/kaas_cli/constants.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/src/kaas_cli/types.py` & `kaas_cli-0.1.7/src/kaas_cli/types.py`

 * *Files identical despite different names*

### Comparing `kaas_cli-0.1.6/PKG-INFO` & `kaas_cli-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaas-cli
-Version: 0.1.6
+Version: 0.1.7
 Summary: Command line utility for K as a Service
 Author: Runtime Verification, Inc.
 Author-email: contact@runtimeverification.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```
