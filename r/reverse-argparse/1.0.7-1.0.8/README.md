# Comparing `tmp/reverse_argparse-1.0.7.tar.gz` & `tmp/reverse_argparse-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reverse_argparse-1.0.7.tar", max compression
+gzip compressed data, was "reverse_argparse-1.0.8.tar", max compression
```

## Comparing `reverse_argparse-1.0.7.tar` & `reverse_argparse-1.0.8.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1711 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/LICENSE.md
--rw-r--r--   0        0        0     5453 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/README.md
--rw-r--r--   0        0        0     3340 2024-04-22 22:04:19.297584 reverse_argparse-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      537 2024-04-22 22:04:19.297584 reverse_argparse-1.0.7/reverse_argparse/__init__.py
--rw-r--r--   0        0        0    19292 2024-04-22 22:04:18.129580 reverse_argparse-1.0.7/reverse_argparse/reverse_argparse.py
--rw-r--r--   0        0        0     7123 1970-01-01 00:00:00.000000 reverse_argparse-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1711 2024-05-13 13:50:06.207356 reverse_argparse-1.0.8/LICENSE.md
+-rw-r--r--   0        0        0     5538 2024-05-13 13:50:06.207356 reverse_argparse-1.0.8/README.md
+-rw-r--r--   0        0        0     3129 2024-05-13 13:50:07.371359 reverse_argparse-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      545 2024-05-13 13:50:07.371359 reverse_argparse-1.0.8/reverse_argparse/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:50:06.207356 reverse_argparse-1.0.8/reverse_argparse/py.typed
+-rw-r--r--   0        0        0    19292 2024-05-13 13:50:06.207356 reverse_argparse-1.0.8/reverse_argparse/reverse_argparse.py
+-rw-r--r--   0        0        0     7208 1970-01-01 00:00:00.000000 reverse_argparse-1.0.8/PKG-INFO
```

### Comparing `reverse_argparse-1.0.7/LICENSE.md` & `reverse_argparse-1.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `reverse_argparse-1.0.7/README.md` & `reverse_argparse-1.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+![Lines of code](https://sloc.xyz/github/sandialabs/reverse_argparse/?category=code)
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
 [![CodeFactor](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/badge/master)](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/overview/master)
 [![CodeQL](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql)
 [![Conda Version](https://img.shields.io/conda/v/conda-forge/reverse-argparse?label=conda-forge)](https://anaconda.org/conda-forge/reverse-argparse)
 ![Conda Downloads](https://img.shields.io/conda/d/conda-forge/reverse-argparse?label=conda-forge%20downloads)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
```

### Comparing `reverse_argparse-1.0.7/pyproject.toml` & `reverse_argparse-1.0.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
-[tool.bandit.assert_used]
-skips = ["**/test_*.py"]
-
-
-[tool.commitizen]
-name = "cz_customize"
-
-
-[tool.commitizen.customize]
-schema_pattern = "(?s)(build|chore|ci|docs|feat|fix|minor|patch|perf|refactor|style|test|revert)(\\(\\S+\\))?!?:( [^\\n\\r]+)((\\n\\n.*)|(\\s*))?$"
-
-
 [tool.poetry]
 name = "reverse_argparse"
-version = "1.0.7"
+version = "1.0.8"
 license = "LICENSE.md"
 readme = "README.md"
 keywords = ["argparse", "argument", "parse", "parsing", "command line"]
 repository = "https://github.com/sandialabs/reverse_argparse"
 description = "Generate the effective command line invocation for a script."
 documentation = "https://reverse-argparse.readthedocs.io"
 authors = [
@@ -99,14 +87,18 @@
     "W",
 ]
 ignore = [
     "D212",
 ]
 
 
+[tool.ruff.lint.per-file-ignores]
+"**/test_*.py" = ["S101"]
+
+
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 
 [tool.semantic_release]
 build_command = "python3 -m pip install poetry && poetry build"
 commit_message = """
```

### Comparing `reverse_argparse-1.0.7/reverse_argparse/__init__.py` & `reverse_argparse-1.0.8/reverse_argparse/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 The ``reverse_argparse`` package.
 
 Provide the :class:`ReverseArgumentParser` class and
 :func:`quote_arg_if_necessary` helper function.
+"""
 
-© 2024 National Technology & Engineering Solutions of Sandia, LLC
-(NTESS).  Under the terms of Contract DE-NA0003525 with NTESS, the U.S.
-Government retains certain rights in this software.
+# © 2024 National Technology & Engineering Solutions of Sandia, LLC
+# (NTESS).  Under the terms of Contract DE-NA0003525 with NTESS, the
+# U.S. Government retains certain rights in this software.
 
-SPDX-License-Identifier: BSD-3-Clause
-"""
+# SPDX-License-Identifier: BSD-3-Clause
 
 from .reverse_argparse import ReverseArgumentParser, quote_arg_if_necessary
 
 __all__ = ["ReverseArgumentParser", "quote_arg_if_necessary"]
-__version__ = "1.0.7"
+__version__ = "1.0.8"
```

### Comparing `reverse_argparse-1.0.7/reverse_argparse/reverse_argparse.py` & `reverse_argparse-1.0.8/reverse_argparse/reverse_argparse.py`

 * *Files identical despite different names*

### Comparing `reverse_argparse-1.0.7/PKG-INFO` & `reverse_argparse-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reverse_argparse
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate the effective command line invocation for a script.
 Home-page: https://github.com/sandialabs/reverse_argparse
 License: LICENSE.md
 Keywords: argparse,argument,parse,parsing,command line
 Author: Jason M. Gates
 Author-email: jmgate@sandia.gov
 Requires-Python: >=3.8
@@ -30,14 +30,15 @@
 Classifier: Typing :: Typed
 Project-URL: CI, https://github.com/sandialabs/reverse_argparse/actions
 Project-URL: Documentation, https://reverse-argparse.readthedocs.io
 Project-URL: Issues, https://github.com/sandialabs/reverse_argparse/issues
 Project-URL: Repository, https://github.com/sandialabs/reverse_argparse
 Description-Content-Type: text/markdown
 
+![Lines of code](https://sloc.xyz/github/sandialabs/reverse_argparse/?category=code)
 [![codecov](https://codecov.io/gh/sandialabs/reverse_argparse/branch/master/graph/badge.svg?token=FmDStZ6FVR)](https://codecov.io/gh/sandialabs/reverse_argparse)
 [![CodeFactor](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/badge/master)](https://www.codefactor.io/repository/github/sandialabs/reverse_argparse/overview/master)
 [![CodeQL](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/github-code-scanning/codeql)
 [![Conda Version](https://img.shields.io/conda/v/conda-forge/reverse-argparse?label=conda-forge)](https://anaconda.org/conda-forge/reverse-argparse)
 ![Conda Downloads](https://img.shields.io/conda/d/conda-forge/reverse-argparse?label=conda-forge%20downloads)
 [![Continuous Integration](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/sandialabs/reverse_argparse/actions/workflows/continuous-integration.yml)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
```

