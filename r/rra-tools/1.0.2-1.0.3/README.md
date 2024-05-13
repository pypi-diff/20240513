# Comparing `tmp/rra_tools-1.0.2.tar.gz` & `tmp/rra_tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.2.tar", max compression
+gzip compressed data, was "rra_tools-1.0.3.tar", max compression
```

## Comparing `rra_tools-1.0.2.tar` & `rra_tools-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-10 21:37:33.437084 rra_tools-1.0.2/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-10 21:37:33.437084 rra_tools-1.0.2/README.md
--rw-r--r--   0        0        0     3749 2024-05-10 21:37:33.437084 rra_tools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      601 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     2087 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0     4635 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3082 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-10 21:37:33.437084 rra_tools-1.0.2/src/rra_tools/translate.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-13 15:39:14.347159 rra_tools-1.0.3/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-13 15:39:14.347159 rra_tools-1.0.3/README.md
+-rw-r--r--   0        0        0     3749 2024-05-13 15:39:14.347159 rra_tools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:14.347159 rra_tools-1.0.3/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     4816 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0     4635 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.3/PKG-INFO
```

### Comparing `rra_tools-1.0.2/LICENSE` & `rra_tools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/README.md` & `rra_tools-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/pyproject.toml` & `rra_tools-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.2"
+version = "1.0.3"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rra_tools-1.0.2/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.3/src/rra_tools/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.3/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/jobmon.py` & `rra_tools-1.0.3/src/rra_tools/jobmon.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/logging/config.py` & `rra_tools-1.0.3/src/rra_tools/logging/config.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/logging/performance.py` & `rra_tools-1.0.3/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.3/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/parallel.py` & `rra_tools-1.0.3/src/rra_tools/parallel.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/shell_tools.py` & `rra_tools-1.0.3/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/src/rra_tools/translate.py` & `rra_tools-1.0.3/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.2/PKG-INFO` & `rra_tools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

