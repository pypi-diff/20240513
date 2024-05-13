# Comparing `tmp/rra_tools-1.0.3.tar.gz` & `tmp/rra_tools-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.3.tar", max compression
+gzip compressed data, was "rra_tools-1.0.4.tar", max compression
```

## Comparing `rra_tools-1.0.3.tar` & `rra_tools-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-13 15:39:14.347159 rra_tools-1.0.3/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-13 15:39:14.347159 rra_tools-1.0.3/README.md
--rw-r--r--   0        0        0     3749 2024-05-13 15:39:14.347159 rra_tools-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 15:39:14.347159 rra_tools-1.0.3/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      601 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     4816 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0     4635 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3082 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-13 15:39:14.351158 rra_tools-1.0.3/src/rra_tools/translate.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-13 15:49:49.970944 rra_tools-1.0.4/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-13 15:49:49.970944 rra_tools-1.0.4/README.md
+-rw-r--r--   0        0        0     3749 2024-05-13 15:49:49.970944 rra_tools-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      681 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     5299 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0     4635 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-13 15:49:49.970944 rra_tools-1.0.4/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.4/PKG-INFO
```

### Comparing `rra_tools-1.0.3/LICENSE` & `rra_tools-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/README.md` & `rra_tools-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/pyproject.toml` & `rra_tools-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.3"
+version = "1.0.4"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rra_tools-1.0.3/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.4/src/rra_tools/cli_tools/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from rra_tools.cli_tools.exceptions import handle_exceptions
 from rra_tools.cli_tools.importers import (
     import_module_from_info,
 )
 from rra_tools.cli_tools.options import (
+    process_choices,
+    with_choice,
     with_debugger,
     with_dry_run,
     with_input_directory,
     with_num_cores,
     with_output_directory,
     with_progress_bar,
     with_queue,
@@ -20,8 +22,10 @@
     "with_dry_run",
     "with_input_directory",
     "with_num_cores",
     "with_output_directory",
     "with_progress_bar",
     "with_queue",
     "with_verbose",
+    "process_choices",
+    "with_choice",
 ]
```

### Comparing `rra_tools-1.0.3/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.4/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/cli_tools/options.py` & `rra_tools-1.0.4/src/rra_tools/cli_tools/options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from collections.abc import Callable, Sequence
 from pathlib import Path
-from typing import ParamSpec, TypeVar
+from typing import Any, ParamSpec, TypeVar
 
 import click
 
 _T = TypeVar("_T")
 _P = ParamSpec("_P")
 _EntryPoint = Callable[_P, _T]
 ClickOption = Callable[[_EntryPoint[_P, _T]], _EntryPoint[_P, _T]]
@@ -64,28 +64,47 @@
         else:
             default = choices[-1]
         option_type = click.Choice(choices)
     show_default = default is not None
     return option_type, default, show_default
 
 
-def with_year(
+def with_choice(
+    name: str,
+    short_name: str | None = None,
     *,
     allow_all: bool = True,
     choices: Sequence[str] | None = None,
+    **kwargs: Any,
 ) -> ClickOption[_P, _T]:
+    """Create an option with a set of choices.
+
+    Parameters
+    ----------
+    name
+        The name of the option.
+    short_name
+        An optional short name for the option.
+    allow_all
+        Whether to allow the special value "ALL", which represents all choices.
+    choices
+        The set of choices to allow.
+
+    """
+    names = [name.replace("_", "-")]
+    if short_name is not None:
+        names.append(short_name)
     option_type, default, show_default = process_choices(allow_all, choices)
 
     return click.option(
-        "--year",
-        "-y",
+        *names,
         type=option_type,
         default=default,
-        help="Year to run.",
         show_default=show_default,
+        **kwargs,
     )
 
 
 def with_verbose() -> ClickOption[_P, _T]:
     return click.option(
         "-v",
         "verbose",
```

### Comparing `rra_tools-1.0.3/src/rra_tools/jobmon.py` & `rra_tools-1.0.4/src/rra_tools/jobmon.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/logging/config.py` & `rra_tools-1.0.4/src/rra_tools/logging/config.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/logging/performance.py` & `rra_tools-1.0.4/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.4/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/parallel.py` & `rra_tools-1.0.4/src/rra_tools/parallel.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/shell_tools.py` & `rra_tools-1.0.4/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/src/rra_tools/translate.py` & `rra_tools-1.0.4/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.3/PKG-INFO` & `rra_tools-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.3
+Version: 1.0.4
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

