# Comparing `tmp/rra_tools-1.0.4.tar.gz` & `tmp/rra_tools-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.4.tar", max compression
+gzip compressed data, was "rra_tools-1.0.5.tar", max compression
```

## Comparing `rra_tools-1.0.4.tar` & `rra_tools-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-13 15:49:49.970944 rra_tools-1.0.4/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-13 15:49:49.970944 rra_tools-1.0.4/README.md
--rw-r--r--   0        0        0     3749 2024-05-13 15:49:49.970944 rra_tools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      681 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     5299 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0     4635 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3082 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/translate.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-13 16:01:18.911015 rra_tools-1.0.5/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-13 16:01:18.915015 rra_tools-1.0.5/README.md
+-rw-r--r--   0        0        0     3749 2024-05-13 16:01:18.915015 rra_tools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     5299 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0     4635 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-13 16:01:18.915015 rra_tools-1.0.5/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.5/PKG-INFO
```

### Comparing `rra_tools-1.0.4/LICENSE` & `rra_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/README.md` & `rra_tools-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/pyproject.toml` & `rra_tools-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.4"
+version = "1.0.5"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rra_tools-1.0.4/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.5/src/rra_tools/cli_tools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from rra_tools.cli_tools.exceptions import handle_exceptions
 from rra_tools.cli_tools.importers import (
     import_module_from_info,
 )
 from rra_tools.cli_tools.options import (
+    RUN_ALL,
+    ClickOption,
     process_choices,
     with_choice,
     with_debugger,
     with_dry_run,
     with_input_directory,
     with_num_cores,
     with_output_directory,
@@ -24,8 +26,10 @@
     "with_num_cores",
     "with_output_directory",
     "with_progress_bar",
     "with_queue",
     "with_verbose",
     "process_choices",
     "with_choice",
+    "RUN_ALL",
+    "ClickOption",
 ]
```

### Comparing `rra_tools-1.0.4/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.5/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/cli_tools/options.py` & `rra_tools-1.0.5/src/rra_tools/cli_tools/options.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/jobmon.py` & `rra_tools-1.0.5/src/rra_tools/jobmon.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/logging/config.py` & `rra_tools-1.0.5/src/rra_tools/logging/config.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/logging/performance.py` & `rra_tools-1.0.5/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.5/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/parallel.py` & `rra_tools-1.0.5/src/rra_tools/parallel.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/shell_tools.py` & `rra_tools-1.0.5/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/src/rra_tools/translate.py` & `rra_tools-1.0.5/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.4/PKG-INFO` & `rra_tools-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

