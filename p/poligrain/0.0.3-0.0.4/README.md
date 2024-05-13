# Comparing `tmp/poligrain-0.0.3.tar.gz` & `tmp/poligrain-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poligrain-0.0.3.tar", max compression
+gzip compressed data, was "poligrain-0.0.4.tar", max compression
```

## Comparing `poligrain-0.0.3.tar` & `poligrain-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1526 2024-01-31 14:30:46.860852 poligrain-0.0.3/LICENSE
--rw-r--r--   0        0        0     1561 2024-01-31 14:30:46.860852 poligrain-0.0.3/README.md
--rw-r--r--   0        0        0     4497 2024-01-31 14:31:05.260983 poligrain-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      568 2024-01-31 14:31:05.260983 poligrain-0.0.3/src/poligrain/__init__.py
--rw-r--r--   0        0        0      672 2024-01-31 14:30:46.860852 poligrain-0.0.3/src/poligrain/plot_map.py
--rw-r--r--   0        0        0        0 2024-01-31 14:30:46.860852 poligrain-0.0.3/src/poligrain/py.typed
--rw-r--r--   0        0        0     4123 2024-01-31 14:30:46.860852 poligrain-0.0.3/src/poligrain/spatial.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 poligrain-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1530 2024-05-13 07:02:23.463062 poligrain-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1779 2024-05-13 07:02:23.463062 poligrain-0.0.4/README.md
+-rw-r--r--   0        0        0     4934 2024-05-13 07:02:26.899070 poligrain-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-05-13 07:02:26.899070 poligrain-0.0.4/src/poligrain/__init__.py
+-rw-r--r--   0        0        0     7157 2024-05-13 07:02:23.467062 poligrain-0.0.4/src/poligrain/plot_map.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:02:23.467062 poligrain-0.0.4/src/poligrain/py.typed
+-rw-r--r--   0        0        0    21335 2024-05-13 07:02:23.467062 poligrain-0.0.4/src/poligrain/spatial.py
+-rw-r--r--   0        0        0     2298 2024-05-13 07:02:23.467062 poligrain-0.0.4/src/poligrain/xarray.py
+-rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 poligrain-0.0.4/PKG-INFO
```

### Comparing `poligrain-0.0.3/LICENSE` & `poligrain-0.0.4/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2023, Christian Chwala.
+Copyright (c) 2023, poligrain developers.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `poligrain-0.0.3/README.md` & `poligrain-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,20 @@
 
 <!-- SPHINX-START -->
 
 `poligrain` is a Python package developed within the COST Action OPENSENSE to
 simplify common tasks for working with **po**int, **li**ne and **gr**idded
 sensor data, focusing on **rain**fall observations.
 
-This is currently an early draft of the package and no, or only preliminary
-functionality, is there...
+This is package is currently in an early stage of development. There are already
+useful functionalities there, but beware that their usage and naming might still
+change.
+
+Checkout the [docs](https://poligrain.readthedocs.io/en/latest/index.html) to
+explore the package. The examples can also be run as notebooks locally.
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/OpenSenseAction/poligrain/workflows/CI/badge.svg
 [actions-link]:             https://github.com/OpenSenseAction/poligrain/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/poligrain
 [conda-link]:               https://github.com/conda-forge/poligrain-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
```

### Comparing `poligrain-0.0.3/pyproject.toml` & `poligrain-0.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 
 [tool.poetry]
 name = "poligrain"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   "Christian Chwala <christian.chwala@kit.edu>",
 ]
 homepage = "https://github.com/OpenSenseAction/poligrain"
 repository = "https://github.com/OpenSenseAction/poligrain"
 license = "BSD-3-Clause"
 description = "Effortlessly plot and compare (rainfall) sensor data with point, line and grid geometry."
@@ -21,30 +21,34 @@
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Scientific/Engineering",
   "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10, <3.12"
+python = ">=3.9, <3.12"
 
 furo = { version = ">=2023.08.17", optional = true }
 myst_parser = { version = ">=0.13", optional = true }
 pytest = { version = ">=6", optional = true }
 pytest-cov = { version = ">=3", optional = true }
 sphinx = { version = ">=7.0", optional = true }
 sphinx_copybutton = { version = ">=0.3.0", optional = true }
 sphinx-autodoc-typehints = { version = "*", optional = true }
 nbsphinx = { version = "*", optional = true }
+pypandoc-binary = { version = "*", optional = true }
+ipython = { version = "*", optional = true }
 netcdf4 = "^1.6.5"
 xarray = "^2023.12.0"
 matplotlib = "^3.8.2"
 nbmake = "^1.4.6"
 pyproj = "^3.6.1"
 scipy = "^1.12.0"
+sparse = "*"
+shapely = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = ">= 6"
 pytest-cov = ">= 3"
 jupyterlab = "^4.0.10"
 nbmake = "^1.4.6"
 
@@ -54,14 +58,16 @@
 docs = [
   "furo",
   "myst_parser",
   "sphinx",
   "sphinx_autodoc_typehints",
   "sphinx_copybutton",
   "nbsphinx",
+  "pypandoc-binary",
+  "ipython",
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 substitution.files = ["src/poligrain/__init__.py"]
 
 
@@ -87,15 +93,15 @@
 report.exclude_also = [
   '\.\.\.',
   'if typing.TYPE_CHECKING:',
 ]
 
 [tool.mypy]
 files = ["src", "tests"]
-python_version = "3.10"
+python_version = "3.9"
 warn_unused_configs = true
 strict = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 disallow_untyped_defs = false
 disallow_incomplete_defs = false
 
@@ -108,57 +114,67 @@
 # below when its usage is fixed. But I keep this section for now.
 #[[tool.mypy.overrides]]
 #module = "numpy,numpy.testing,xarray,matplotlib,matplotlib.pyplot,matplotlib.collections,netCDF4,poligrain"
 #ignore_missing_imports = true
 
 [tool.ruff]
 src = ["src"]
-target-version = "py310"
+line-length = 88
+target-version = "py39"
 extend-include = ["*.ipynb"]
 
 [tool.ruff.lint]
 extend-select = [
   "B",        # flake8-bugbear
   "I",        # isort
   "ARG",      # flake8-unused-arguments
   "C4",       # flake8-comprehensions
   "EM",       # flake8-errmsg
   "ICN",      # flake8-import-conventions
   "G",        # flake8-logging-format
   "PGH",      # pygrep-hooks
   "PIE",      # flake8-pie
   "PL",       # pylint
+  "A001",     # flake8-builtins
   "PT",       # flake8-pytest-style
   "PTH",      # flake8-use-pathlib
   "RET",      # flake8-return
   "RUF",      # Ruff-specific
   "SIM",      # flake8-simplify
   "T20",      # flake8-print
   "UP",       # pyupgrade
   "YTT",      # flake8-2020
   "EXE",      # flake8-executable
   "NPY",      # NumPy specific rules
   "PD",       # pandas-vet
+  "E",        # style errors
+  "W",        # style warnings
+  "F",        # flakes
+  "D",        # pydocstyle
+  "U",        # pyupgrade
 ]
 ignore = [
   "PLR09",    # Too many <...>
   "PLR2004",  # Magic value used in comparison
   "ISC001",   # Conflicts with formatter
 ]
 # Disabled because this would also be forced in notebooks where
 # it does not make sense. We also do not require it now in module
 # files. We do currently not do type checking anyway...
 #isort.required-imports = ["from __future__ import annotations"]
 # Uncomment if using a _compat.typing backport
 # typing-modules = ["poligrain._compat.typing"]
 
 [tool.ruff.lint.per-file-ignores]
-"tests/**" = ["T20"]
-"noxfile.py" = ["T20"]
+"tests/**" = ["T20", "D"]
+"noxfile.py" = ["T20", "D100"]
+"docs/conf.py" = ["D100", "A001"]
 
+[tool.ruff.lint.pydocstyle]
+convention = "numpy"
 
 [tool.pylint]
 py-version = "3.10"
 ignore-paths = [".*/_version.py"]
 reports.output-format = "colorized"
 similarities.ignore-imports = "yes"
 messages_control.disable = [
```

### Comparing `poligrain-0.0.3/src/poligrain/__init__.py` & `poligrain-0.0.4/src/poligrain/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""
-Copyright (c) 2023 Christian Chwala. All rights reserved.
+"""Copyright (c) 2023 Christian Chwala. All rights reserved.
 
-poligrain: Effortlessly plot and compare (rainfall) sensor data with point, line and grid geometry.
+poligrain: Effortlessly plot and compare (rainfall) sensor data
+           with point, line and grid geometry.
 """
 
 
 from __future__ import annotations
 
 # This is only here to suppress the bug described in
 # https://github.com/pydata/xarray/issues/7259
 # We have to make sure that netcdf4 is imported before
 # numpy is imported for the first time, e.g. also via
 # importing xarray
 import netCDF4  # noqa: F401
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
-from . import plot_map, spatial
+from . import plot_map, spatial, xarray
 
-__all__ = ["__version__", "plot_map", "spatial"]
+__all__ = ["__version__", "plot_map", "spatial", "xarray"]
```

### Comparing `poligrain-0.0.3/PKG-INFO` & `poligrain-0.0.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: poligrain
-Version: 0.0.3
+Version: 0.0.4
 Summary: Effortlessly plot and compare (rainfall) sensor data with point, line and grid geometry.
 Home-page: https://github.com/OpenSenseAction/poligrain
 License: BSD-3-Clause
 Author: Christian Chwala
 Author-email: christian.chwala@kit.edu
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 Requires-Dist: furo (>=2023.08.17) ; extra == "docs"
+Requires-Dist: ipython ; extra == "docs"
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: myst_parser (>=0.13) ; extra == "docs"
 Requires-Dist: nbmake (>=1.4.6,<2.0.0) ; extra == "test" or extra == "dev"
 Requires-Dist: nbsphinx ; extra == "docs"
 Requires-Dist: netcdf4 (>=1.6.5,<2.0.0)
+Requires-Dist: pypandoc-binary ; extra == "docs"
 Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Requires-Dist: pytest (>=6) ; extra == "test" or extra == "dev"
 Requires-Dist: pytest-cov (>=3) ; extra == "test" or extra == "dev"
 Requires-Dist: scipy (>=1.12.0,<2.0.0)
+Requires-Dist: shapely
+Requires-Dist: sparse
 Requires-Dist: sphinx (>=7.0) ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ; extra == "docs"
 Requires-Dist: sphinx_copybutton (>=0.3.0) ; extra == "docs"
 Requires-Dist: xarray (>=2023.12.0,<2024.0.0)
 Project-URL: Repository, https://github.com/OpenSenseAction/poligrain
 Description-Content-Type: text/markdown
 
@@ -48,16 +53,20 @@
 
 <!-- SPHINX-START -->
 
 `poligrain` is a Python package developed within the COST Action OPENSENSE to
 simplify common tasks for working with **po**int, **li**ne and **gr**idded
 sensor data, focusing on **rain**fall observations.
 
-This is currently an early draft of the package and no, or only preliminary
-functionality, is there...
+This is package is currently in an early stage of development. There are already
+useful functionalities there, but beware that their usage and naming might still
+change.
+
+Checkout the [docs](https://poligrain.readthedocs.io/en/latest/index.html) to
+explore the package. The examples can also be run as notebooks locally.
 
 <!-- prettier-ignore-start -->
 [actions-badge]:            https://github.com/OpenSenseAction/poligrain/workflows/CI/badge.svg
 [actions-link]:             https://github.com/OpenSenseAction/poligrain/actions
 [conda-badge]:              https://img.shields.io/conda/vn/conda-forge/poligrain
 [conda-link]:               https://github.com/conda-forge/poligrain-feedstock
 [github-discussions-badge]: https://img.shields.io/static/v1?label=Discussions&message=Ask&color=blue&logo=github
```

