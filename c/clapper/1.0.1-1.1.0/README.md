# Comparing `tmp/clapper-1.0.1.tar.gz` & `tmp/clapper-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clapper-1.0.1.tar", last modified: Tue Feb 28 20:27:49 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `clapper-1.0.1.tar` & `clapper-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,43 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.256079 clapper-1.0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.248079 clapper-1.0.1/LICENSES/
--rw-rw-rw-   0 root         (0) root         (0)     1459 2023-02-28 17:13:15.000000 clapper-1.0.1/LICENSES/BSD-3-Clause.txt
--rw-rw-rw-   0 root         (0) root         (0)      228 2023-02-28 20:00:38.000000 clapper-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2003 2023-02-28 20:27:49.256079 clapper-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-02-28 20:25:58.000000 clapper-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.252079 clapper-1.0.1/doc/
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     9113 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/click.rst
--rw-rw-rw-   0 root         (0) root         (0)     3529 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5382 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/config.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.252079 clapper-1.0.1/doc/data/
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/data/basic_config.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/data/second_config.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_alias.py
--rw-rw-rw-   0 root         (0) root         (0)     1763 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      463 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_config.py
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)      319 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_logging.py
--rw-rw-rw-   0 root         (0) root         (0)      186 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/example_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1101 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-02-28 17:59:46.000000 clapper-1.0.1/doc/install.rst
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/links.rst
--rw-rw-rw-   0 root         (0) root         (0)     4503 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/logging.rst
--rw-rw-rw-   0 root         (0) root         (0)      147 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/nitpick-exceptions.txt
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-02-28 17:13:15.000000 clapper-1.0.1/doc/rc.rst
--rw-rw-rw-   0 root         (0) root         (0)     2254 2023-02-28 20:25:58.000000 clapper-1.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-28 20:27:49.256079 clapper-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-02-28 17:13:15.000000 clapper-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.248079 clapper-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.252079 clapper-1.0.1/src/clapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 17:13:15.000000 clapper-1.0.1/src/clapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30544 2023-02-28 17:13:15.000000 clapper-1.0.1/src/clapper/click.py
--rw-rw-rw-   0 root         (0) root         (0)    12534 2023-02-28 17:13:15.000000 clapper-1.0.1/src/clapper/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3711 2023-02-28 17:13:15.000000 clapper-1.0.1/src/clapper/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     6883 2023-02-28 17:13:15.000000 clapper-1.0.1/src/clapper/rc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.252079 clapper-1.0.1/src/clapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2003 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1118 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      385 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      205 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-02-28 20:27:49.000000 clapper-1.0.1/src/clapper.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-28 20:27:48.000000 clapper-1.0.1/src/clapper.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.256079 clapper-1.0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2276 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-28 20:27:49.256079 clapper-1.0.1/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/basic_config.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/complex.py
--rw-rw-rw-   0 root         (0) root         (0)      170 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/oldjson.cfg
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/second_config.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/test_dump_config.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/test_dump_config2.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/userdefaults_ex1.cfg
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/data/verbose_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9499 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/test_click.py
--rw-rw-rw-   0 root         (0) root         (0)     5909 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     4890 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-02-28 17:13:15.000000 clapper-1.0.1/tests/test_rc.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 clapper-1.1.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/api.rst
+-rw-r--r--   0        0        0     9113 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/click.rst
+-rw-r--r--   0        0        0     3585 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/conf.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/config.rst
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_alias.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_cli.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_config.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_defaults.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_logging.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/example_options.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/index.rst
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/install.rst
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/links.rst
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/logging.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/nitpick-exceptions.txt
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/rc.rst
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/data/basic_config.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 clapper-1.1.0/doc/data/second_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clapper-1.1.0/src/clapper/__init__.py
+-rw-r--r--   0        0        0    30636 2020-02-02 00:00:00.000000 clapper-1.1.0/src/clapper/click.py
+-rw-r--r--   0        0        0    11712 2020-02-02 00:00:00.000000 clapper-1.1.0/src/clapper/config.py
+-rw-r--r--   0        0        0     3705 2020-02-02 00:00:00.000000 clapper-1.1.0/src/clapper/logging.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 clapper-1.1.0/src/clapper/rc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/test_click.py
+-rw-r--r--   0        0        0     5854 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/test_logging.py
+-rw-r--r--   0        0        0    10578 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/test_rc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/__init__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/basic_config.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/complex.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/oldjson.cfg
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/second_config.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/test_dump_config.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/test_dump_config2.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/userdefaults_ex1.cfg
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 clapper-1.1.0/tests/data/verbose_config.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 clapper-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 clapper-1.1.0/README.md
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 clapper-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 clapper-1.1.0/PKG-INFO
```

### Comparing `clapper-1.0.1/LICENSES/BSD-3-Clause.txt` & `clapper-1.1.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/PKG-INFO` & `clapper-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,52 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: clapper
-Version: 1.0.1
+Version: 1.1.0
 Summary: Configuration Support for Python Packages and CLIs
-Author-email: Andre Anjos <andre.anjos@idiap.ch>
-License: BSD 3-Clause License
-Project-URL: documentation, https://clapper.readthedocs.io/en/v1.0.1/
+Project-URL: documentation, https://clapper.readthedocs.io/en/v1.1.0/
 Project-URL: homepage, https://pypi.org/project/clapper
 Project-URL: repository, https://gitlab.idiap.ch/software/clapper
 Project-URL: changelog, https://gitlab.idiap.ch/software/clapper/-/releases
+Author-email: Andre Anjos <andre.anjos@idiap.ch>
+License-Expression: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: qa
+Requires-Python: >=3.10
+Requires-Dist: click>=8
+Requires-Dist: tomli
+Requires-Dist: tomli-w
+Requires-Dist: xdg
 Provides-Extra: doc
+Requires-Dist: auto-intersphinx; extra == 'doc'
+Requires-Dist: furo; extra == 'doc'
+Requires-Dist: sphinx; extra == 'doc'
+Requires-Dist: sphinx-autodoc-typehints; extra == 'doc'
+Requires-Dist: sphinx-copybutton; extra == 'doc'
+Requires-Dist: sphinx-inline-tabs; extra == 'doc'
+Requires-Dist: sphinxcontrib-programoutput; extra == 'doc'
+Provides-Extra: qa
+Requires-Dist: pre-commit; extra == 'qa'
 Provides-Extra: test
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.1-orange.svg)](https://clapper.readthedocs.io/en/v1.0.1/)
-[![build](https://gitlab.idiap.ch/software/clapper/badges/v1.0.1/pipeline.svg)](https://gitlab.idiap.ch/software/clapper/commits/v1.0.1)
-[![coverage](https://gitlab.idiap.ch/software/clapper/badges/v1.0.1/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/clapper/v1.0.1/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.1.0-orange.svg)](https://clapper.readthedocs.io/en/v1.1.0/)
+[![build](https://gitlab.idiap.ch/software/clapper/badges/v1.1.0/pipeline.svg)](https://gitlab.idiap.ch/software/clapper/commits/v1.1.0)
+[![coverage](https://gitlab.idiap.ch/software/clapper/badges/v1.1.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/clapper/v1.1.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/clapper)
 
 
 # Configuration Support for Python Packages and CLIs
 
 This package provides a way to define command-line-interface (CLI) applications
 such that user options can be stored in Python-based configuration files and
```

### Comparing `clapper-1.0.1/README.md` & `clapper-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
 SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 
 SPDX-License-Identifier: BSD-3-Clause
 -->
 
-[![latest-docs](https://img.shields.io/badge/docs-v1.0.1-orange.svg)](https://clapper.readthedocs.io/en/v1.0.1/)
-[![build](https://gitlab.idiap.ch/software/clapper/badges/v1.0.1/pipeline.svg)](https://gitlab.idiap.ch/software/clapper/commits/v1.0.1)
-[![coverage](https://gitlab.idiap.ch/software/clapper/badges/v1.0.1/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/clapper/v1.0.1/coverage/index.html)
+[![latest-docs](https://img.shields.io/badge/docs-v1.1.0-orange.svg)](https://clapper.readthedocs.io/en/v1.1.0/)
+[![build](https://gitlab.idiap.ch/software/clapper/badges/v1.1.0/pipeline.svg)](https://gitlab.idiap.ch/software/clapper/commits/v1.1.0)
+[![coverage](https://gitlab.idiap.ch/software/clapper/badges/v1.1.0/coverage.svg)](https://www.idiap.ch/software/biosignal/docs/software/clapper/v1.1.0/coverage/index.html)
 [![repository](https://img.shields.io/badge/gitlab-project-0000c0.svg)](https://gitlab.idiap.ch/software/clapper)
 
 
 # Configuration Support for Python Packages and CLIs
 
 This package provides a way to define command-line-interface (CLI) applications
 such that user options can be stored in Python-based configuration files and
```

### Comparing `clapper-1.0.1/doc/click.rst` & `clapper-1.1.0/doc/click.rst`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/doc/conf.py` & `clapper-1.1.0/doc/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
-import os
+import pathlib
 import time
 
 from importlib.metadata import distribution
 
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
@@ -31,16 +31,17 @@
 # Be picky about warnings
 nitpicky = True
 
 # Ignores stuff we can't easily resolve on other project's sphinx manuals
 nitpick_ignore = []
 
 # Allows the user to override warnings from a separate file
-if os.path.exists("nitpick-exceptions.txt"):
-    for line in open("nitpick-exceptions.txt"):
+nitpick_path = pathlib.Path("nitpick-exceptions.txt")
+if nitpick_path.exists():
+    for line in nitpick_path.open():
         if line.strip() == "" or line.startswith("#"):
             continue
         dtype, target = line.split(None, 1)
         target = target.strip()
         nitpick_ignore.append((dtype, target))
 
 # Always includes todos
@@ -49,16 +50,16 @@
 # Generates auto-summary automatically
 autosummary_generate = True
 
 # Create numbers on figures with captions
 numfig = True
 
 # If we are on OSX, the 'dvipng' path maybe different
-dvipng_osx = "/Library/TeX/texbin/dvipng"
-if os.path.exists(dvipng_osx):
+dvipng_osx = pathlib.Path("/Library/TeX/texbin/dvipng")
+if dvipng_osx.exists():
     pngmath_dvipng = dvipng_osx
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
@@ -66,15 +67,15 @@
 # The main toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "clapper"
 package = distribution(project)
 
-copyright = "%s, Idiap Research Institute" % time.strftime("%Y")
+copyright = f"{time.strftime('%Y')}, Idiap Research Institute"  # noqa: A001
 
 # The short X.Y version.
 version = package.version
 # The full version, including alpha/beta/rc tags.
 release = version
 
 # List of patterns, relative to source directory, that match files and
@@ -114,12 +115,12 @@
     "show-inheritance": True,
 }
 
 auto_intersphinx_packages = [("python", "3"), "click"]
 auto_intersphinx_catalog = "catalog.json"
 
 # Doctest global setup
-sphinx_source_dir = os.path.abspath(".")
+sphinx_source_dir = pathlib.Path.cwd().resolve()
 doctest_global_setup = f"""
 import os
 data = os.path.join('{sphinx_source_dir}', 'data')
 """
```

### Comparing `clapper-1.0.1/doc/config.rst` & `clapper-1.1.0/doc/config.rst`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/doc/example_alias.py` & `clapper-1.1.0/doc/example_alias.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """An example script to demonstrate config-file option readout."""
 
 # To improve loading performance, we recommend you only import the very
 # essential packages needed to start the CLI.  Defer all other imports to
 # within the function implementing the command.
 
-import click
-
 import clapper.click
+import click
 
 
 @click.group(cls=clapper.click.AliasedGroup)
 def main():
+    """Declare main command-line application."""
     pass
 
 
 @main.command()
 def push():
+    """Push subcommand."""
     click.echo("push was called")
 
 
 @main.command()
 def pop():
+    """Pop subcommand."""
     click.echo("pop was called")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `clapper-1.0.1/doc/example_cli.py` & `clapper-1.1.0/doc/example_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """An example script to demonstrate config-file option readout."""
 
 # To improve loading performance, we recommend you only import the very
 # essential packages needed to start the CLI.  Defer all other imports to
 # within the function implementing the command.
 
 import click
@@ -39,15 +38,15 @@
     type=click.Choice(["red", "green", "blue"]),
     cls=ResourceOption,
 )
 @verbosity_option(logger=logger)
 @click.version_option(package_name="clapper")
 @click.pass_context
 def main(ctx, **_):
-    """Tests our Click interfaces."""
+    """Test our Click interfaces."""
     # Add imports needed for your code here, and avoid spending time loading!
 
     # In this example, we just print the loaded options to demonstrate loading
     # from config files actually works!
     for k, v in ctx.params.items():
         if k in ("dump_config", "config"):
             continue
```

### Comparing `clapper-1.0.1/doc/example_defaults.py` & `clapper-1.1.0/doc/example_defaults.py`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/doc/index.rst` & `clapper-1.1.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/doc/links.rst` & `clapper-1.1.0/doc/links.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 .. SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 ..
 .. SPDX-License-Identifier: BSD-3-Clause
 
 .. _python: http://www.python.org
 .. _pip: https://pip.pypa.io/en/stable/
+.. _uv: https://github.com/astral-sh/uv
+.. _rye: https://github.com/astral-sh/rye
+.. _poetry: https://python-poetry.org
+.. _pixi: https://pixi.sh
 .. _mamba: https://mamba.readthedocs.io/en/latest/index.html
 .. _toml: https://toml.io
 .. _tomli: https://pypi.org/project/tomli/
 .. _package entry-points: https://packaging.python.org/en/latest/specifications/entry-points/
 .. _click: http://click.pocoo.org/
 .. _click-plugins: https://github.com/click-contrib/click-plugins
 .. _logging-tree module: https://pypi.org/project/logging_tree/
```

### Comparing `clapper-1.0.1/doc/logging.rst` & `clapper-1.1.0/doc/logging.rst`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/doc/rc.rst` & `clapper-1.1.0/doc/rc.rst`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/src/clapper/click.py` & `clapper-1.1.0/src/clapper/click.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Helpers to build command-line interfaces (CLI) via :py:mod:`click`."""
 
-from __future__ import annotations
-
 import functools
 import inspect
 import logging
+import pathlib
 import pprint
 import shutil
 import time
 import typing
 
 from importlib.metadata import EntryPoint
 
@@ -72,34 +70,32 @@
 
         dlft: The default verbosity level to use (defaults to 0).
 
         **kwargs: Further keyword-arguments to be forwarded to the underlying
             :py:func:`click.option`
 
 
-    Returns:
-
+    Returns
+    -------
         A callable, that follows the :py:mod:`click`-framework policy for
         option decorators.  Use it accordingly.
     """
 
     def custom_verbosity_option(f):
         def callback(ctx, param, value):
             ctx.meta[name] = value
-            log_level: int = {
+            log_level: int = {  # type: ignore
                 0: logging.ERROR,
                 1: logging.WARNING,
                 2: logging.INFO,
                 3: logging.DEBUG,
             }[value]
 
             logger.setLevel(log_level)
-            logger.debug(
-                f'Level of Logger("{logger.name}") was set to {log_level}'
-            )
+            logger.debug(f'Level of Logger("{logger.name}") was set to {log_level}')
             return value
 
         return click.option(
             f"-{short_name}",
             f"--{name}",
             count=True,
             type=click.IntRange(min=0, max=3, clamp=True),
@@ -148,35 +144,33 @@
     entry_point_group: str
     """The name of entry point that will be used to load the config files."""
 
     def __init__(
         self,
         name: str,
         *args: tuple,
-        help: str | None = None,
+        help: str | None = None,  # noqa: A002
         entry_point_group: str | None = None,
         **kwargs: typing.Any,
     ) -> None:
         self.entry_point_group = entry_point_group
         configs_argument_name = "CONFIG"
 
         # Augment help for the config file argument
         self.extra_help = f"""\n\nIt is possible to pass one or several Python
 files (or names of ``{entry_point_group}`` entry points or module names) as
 {configs_argument_name} arguments to the command line which contain the parameters listed below as Python variables. The options through the command-line (see below)
 will override the values of configuration files. You can run this command with
 ``<COMMAND> -H example_config.py`` to create a template config file."""
-        help = (help or "").rstrip() + self.extra_help
+        help = (help or "").rstrip() + self.extra_help  # noqa: A001
         super().__init__(name, *args, help=help, **kwargs)
 
         # Add the config argument to the command
         def configs_argument_callback(ctx, param, value):
-            config_context = load(
-                value, entry_point_group=self.entry_point_group
-            )
+            config_context = load(value, entry_point_group=self.entry_point_group)
 
             config_context = mod_to_context(config_context)
             ctx.config_context = config_context
             module_logger.debug("Augmenting click context with config context")
             return value
 
         click.argument(
@@ -244,17 +238,15 @@
                 begin, dflt = "Required parameter", ""
             else:
                 begin, dflt = (
                     "Optional parameter",
                     f" [default: {param.default}]",
                 )
 
-            config_file.write(
-                f"{begin}: {param.name} ({', '.join(param.opts)}){dflt}"
-            )
+            config_file.write(f"{begin}: {param.name} ({', '.join(param.opts)}){dflt}")
 
             if param.help is not None:
                 config_file.write(f"\n{param.help}")
 
             if (
                 isinstance(param, ResourceOption)
                 and param.entry_point_group is not None
@@ -262,25 +254,24 @@
                 config_file.write(
                     f"\nRegistered entries are: "
                     f"{resource_keys(param.entry_point_group)}"
                 )
 
             config_file.write('"""\n')
 
-        click.echo(
-            f"Configuration file `{config_file.name}' was written; exiting"
-        )
+        click.echo(f"Configuration file `{config_file.name}' was written; exiting")
 
         config_file.close()
         ctx.exit()
 
 
 class CustomParamType(click.ParamType):
     """Custom parameter class allowing click to receive complex Python types as
-    parameters."""
+    parameters.
+    """
 
     name = "custom"
 
 
 class ResourceOption(click.Option):
     """An extended :py:class:`click.Option` that automatically loads resources
     from config files.
@@ -305,17 +296,14 @@
     2. Using this class (with :py:class:`ConfigCommand`) AND (providing
        `entry_point_group`).
     3. Using this class (with :py:class:`ConfigCommand`) AND (without providing
        `entry_point_group`).
 
     Using this class without :py:class:`ConfigCommand` and without providing
     `entry_point_group` does nothing and is not allowed.
-
-
-    Attributes:
     """
 
     entry_point_group: str | None
     """If provided, the strings values to this option are assumed to be entry
     points from ``entry_point_group`` that need to be loaded.
 
     This may be different than the wrapping :py:class:`ConfigCommand`.
@@ -334,16 +322,16 @@
         confirmation_prompt=False,
         hide_input=False,
         is_flag=None,
         flag_value=None,
         multiple=False,
         count=False,
         allow_from_autoenv=True,
-        type=None,
-        help=None,
+        type=None,  # noqa: A002
+        help=None,  # noqa: A002
         entry_point_group=None,
         required=False,
         string_exceptions=None,
         **kwargs,
     ) -> None:
         # By default, if unspecified, click options are converted to strings.
         # By using ResourceOption's, however, we allow for complex user types
@@ -352,27 +340,25 @@
         # "custom" parameter type, and do not convert values to strings.
         if (
             (type is None)
             and (kwargs.get("default") is None)
             and (count is False)
             and (is_flag is None)
         ):
-            type = CustomParamType()
+            type = CustomParamType()  # noqa: A001
 
         self.entry_point_group = entry_point_group
         if entry_point_group is not None:
-            name, _, _ = self._parse_decls(
-                param_decls, kwargs.get("expose_value")
-            )
-            help = help or ""
-            help += (
+            name, _, _ = self._parse_decls(param_decls, kwargs.get("expose_value"))
+            help = help or ""  # noqa: A001
+            help += (  # noqa: A001
                 f" Can be a `{entry_point_group}' entry point, a module name, or "
                 f"a path to a Python file which contains a variable named `{name}'."
             )
-            help = help.format(entry_point_group=entry_point_group, name=name)
+            help = help.format(entry_point_group=entry_point_group, name=name)  # noqa: A001
 
         super().__init__(
             param_decls=param_decls,
             show_default=show_default,
             prompt=prompt,
             confirmation_prompt=confirmation_prompt,
             hide_input=hide_input,
@@ -387,36 +373,34 @@
             **kwargs,
         )
         self.string_exceptions = string_exceptions or []
 
     def consume_value(
         self, ctx: click.Context, opts: dict
     ) -> tuple[typing.Any, ParameterSource]:
-        """Retrieves value for parameter from appropriate context.
+        """Retrieve value for parameter from appropriate context.
 
         This method will retrive the value of its own parameter from the
         appropriate context, by trying various sources.
 
+        Parameters
+        ----------
+        ctx
+            The click context to retrieve the value from
+        opts
+            command-line options, eventually passed by the user
 
-        Arguments:
-
-            ctx: The click context to retrieve the value from
-
-            opts: command-line options, eventually passed by the user
-
-
-        Returns:
 
+        Returns
+        -------
             A tuple containing the parameter value (of any type) and the source
             it used to retrieve it.
         """
 
-        if (
-            not hasattr(ctx, "config_context")
-        ) and self.entry_point_group is None:
+        if (not hasattr(ctx, "config_context")) and self.entry_point_group is None:
             raise TypeError(
                 "The ResourceOption class is not meant to be used this way. "
                 "See package documentation for details."
             )
 
         module_logger.debug(f"consuming resource option for {self.name}")
         value = opts.get(self.name)
@@ -442,41 +426,37 @@
 
         if value is None:
             value = self.get_default(ctx)
             source = ParameterSource.DEFAULT
 
         return value, source
 
-    def type_cast_value(
-        self, ctx: click.Context, value: typing.Any
-    ) -> typing.Any:
+    def type_cast_value(self, ctx: click.Context, value: typing.Any) -> typing.Any:
         """Convert and validate a value against the option's type.
 
         This method considers the option's ``type``, ``multiple``, and ``nargs``.
         Furthermore, if the an ``entry_point_group`` is provided, it will load
         it.
 
         Arguments:
 
             ctx: The click context to be used for casting the value
 
             value: The actual value, that needs to be cast
 
 
-        Returns:
-
+        Returns
+        -------
             The cast value
         """
         value = super().type_cast_value(ctx, value)
 
         # if the value is a string and an entry_point_group is provided, load it
         if self.entry_point_group is not None:
-            while (
-                isinstance(value, str) and value not in self.string_exceptions
-            ):
+            while isinstance(value, str) and value not in self.string_exceptions:
                 value = load(
                     [value],
                     entry_point_group=self.entry_point_group,
                     attribute_name=self.name,
                 )
 
         return value
@@ -498,113 +478,115 @@
         """get_command with prefix aliasing."""
         rv = click.Group.get_command(self, ctx, cmd_name)
         if rv is not None:
             return rv
         matches = [x for x in self.list_commands(ctx) if x.startswith(cmd_name)]
         if not matches:
             return None
-        elif len(matches) == 1:
+
+        if len(matches) == 1:
             return click.Group.get_command(self, ctx, matches[0])
-        ctx.fail("Too many matches: %s" % ", ".join(sorted(matches)))
+
+        ctx.fail(f"Too many matches: {', '.join(sorted(matches))}")  # noqa: RET503
 
 
 def user_defaults_group(
     logger: logging.Logger,
     config: UserDefaults,
 ) -> typing.Callable[..., typing.Any]:
-    """Decorator to add a command group to read/write RC configuration.
+    """Add a command group to read/write RC configuration.
 
     This decorator adds a whole command group to a user predefined function
     which is part of the user's CLI.  The command group allows the user to get
-    and set options
-    through the command-line interface:
+    and set options through the command-line interface:
 
     .. code-block:: python
 
        import logging
        from expose.rc import UserDefaults
        from expose.click import user_defaults_group
 
        logger = logging.getLogger(__name__)
        user_defaults = UserDefaults("~/.myapprc")
        ...
 
+
        @user_defaults_group(logger=logger, config=user_defaults)
        def rc(**kwargs):
-            '''Use this command to affect the global user configuration.'''
-            pass
+           '''Use this command to affect the global user configuration.'''
+           pass
 
 
     Then use it like this:
 
     .. code-block:: shell
 
        $ user-cli rc --help
        usage: ...
     """
 
     def group_decorator(
-        func: typing.Callable[..., typing.Any]
+        func: typing.Callable[..., typing.Any],
     ) -> typing.Callable[..., typing.Any]:
         @click.group(
             cls=AliasedGroup,
             no_args_is_help=True,
             context_settings=_COMMON_CONTEXT_SETTINGS,
         )
         @verbosity_option(logger=logger)
         @functools.wraps(func)
         def group_wrapper(**kwargs):
             return func(**kwargs)
 
         @group_wrapper.command(context_settings=_COMMON_CONTEXT_SETTINGS)
         @verbosity_option(logger=logger)
         def show(**_: typing.Any) -> None:
-            """Shows the user-defaults file contents."""
+            """Show the user-defaults file contents."""
             click.echo(str(config).strip())
 
         @group_wrapper.command(
-            no_args_is_help=True, context_settings=_COMMON_CONTEXT_SETTINGS
+            no_args_is_help=True,
+            context_settings=_COMMON_CONTEXT_SETTINGS,
         )
         @click.argument("key")
         @verbosity_option(logger=logger)
         def get(key: str, **_: typing.Any) -> None:
-            """Prints a key from the user-defaults file.
+            """Print a key from the user-defaults file.
 
-            Retrieves the value of the requested KEY and displays it.
-            The KEY may contain dots (``.``) to access values from
-            subsections in the TOML_ document.
+            Retrieves the value of the requested KEY and displays it. The KEY
+            may contain dots (``.``) to access values from subsections in the
+            TOML_ document.
             """
             try:
                 click.echo(config[key])
             except KeyError:
                 raise click.ClickException(
                     f"Cannot find object named `{key}' at `{config.path}'",
                 )
 
         @group_wrapper.command(
-            no_args_is_help=True, context_settings=_COMMON_CONTEXT_SETTINGS
+            name="set",
+            no_args_is_help=True,
+            context_settings=_COMMON_CONTEXT_SETTINGS,
         )
         @click.argument("key")
         @click.argument("value")
         @verbosity_option(logger=logger)
-        def set(key: str, value: str, **_: typing.Any) -> None:
-            """Sets the value for a key on the user-defaults file.
+        def set_(key: str, value: str, **_: typing.Any) -> None:
+            """Set the value for a key on the user-defaults file.
 
-            If ``key`` contains dots (``.``), then this sets nested
-            subsection
+            If ``key`` contains dots (``.``), then this sets nested subsection
             variables on the configuration file.  Values are parsed and
             translated following the rules of TOML_.
 
             .. warning::
 
-            This command will override the current configuration file
-            and my
-            erase any user comments added by hand.  To avoid this,
-            simply
-            edit your configuration file by hand.
+               This command will override the current configuration file and my
+               erase any user comments added by hand.  To avoid this, simply
+               edit your configuration file by hand.
             """
             try:
                 tmp = tomli.loads(f"v = {value}")
                 value = tmp["v"]
             except tomli.TOMLDecodeError:
                 pass
 
@@ -622,29 +604,25 @@
 
         @group_wrapper.command(
             no_args_is_help=True, context_settings=_COMMON_CONTEXT_SETTINGS
         )
         @click.argument("key")
         @verbosity_option(logger=logger)
         def rm(key: str, **_: typing.Any) -> None:
-            """Removes the given key from the configuration file.
+            """Remove the given key from the configuration file.
 
-            This command will remove the KEY from the configuration
-            file.  If
-            the input key corresponds to a section in the configuration
-            file,
+            This command will remove the KEY from the configuration file.  If
+            the input key corresponds to a section in the configuration file,
             then the whole configuration section will be removed.
 
             .. warning::
 
-            This command will override the current configuration file
-            and my
-            erase any user comments added by hand.  To avoid this,
-            simply
-            edit your configuration file by hand.
+               This command will override the current configuration file and my
+               erase any user comments added by hand.  To avoid this, simply
+               edit your configuration file by hand.
             """
             try:
                 del config[key]
                 config.write()
             except KeyError:
                 logger.error(
                     f"Cannot delete object named `{key}' at `{config.path}'",
@@ -659,16 +637,15 @@
     return group_decorator
 
 
 def config_group(
     logger: logging.Logger,
     entry_point_group: str,
 ) -> typing.Callable[..., typing.Any]:
-    """Decorator to add a command group to list/describe/copy job
-    configurations.
+    """Add a command group to list/describe/copy job configurations.
 
     This decorator adds a whole command group to a user predefined function
     which is part of the user's CLI.  The command group provdes an interface to
     list, fully describe or locally copy configuration files distributed with
     the package.  Commands accept both entry-point or module names to be
     provided as input.
 
@@ -676,69 +653,71 @@
 
        import logging
        from expose.click import config_group
 
        logger = logging.getLogger(__name__)
        ...
 
+
        @config_group(logger=logger, entry_point_group="mypackage.config")
        def config(**kwargs):
-            '''Use this command to list/describe/copy config files.'''
-            pass
+           '''Use this command to list/describe/copy config files.'''
+           pass
 
 
     Then use it like this:
 
     .. code-block:: shell
 
        $ user-cli config --help
        usage: ...
     """
 
     def group_decorator(
-        func: typing.Callable[..., typing.Any]
+        func: typing.Callable[..., typing.Any],
     ) -> typing.Callable[..., typing.Any]:
-        @click.group(
-            cls=AliasedGroup, context_settings=_COMMON_CONTEXT_SETTINGS
-        )
+        @click.group(cls=AliasedGroup, context_settings=_COMMON_CONTEXT_SETTINGS)
         @verbosity_option(logger=logger)
         @functools.wraps(func)
         def group_wrapper(**kwargs):
             return func(**kwargs)
 
-        @group_wrapper.command(context_settings=_COMMON_CONTEXT_SETTINGS)
+        @group_wrapper.command(
+            name="list",
+            context_settings=_COMMON_CONTEXT_SETTINGS,
+        )
         @click.pass_context
         @verbosity_option(logger=logger)
-        def list(ctx, **_: typing.Any):
-            """Lists installed configuration resources."""
-            from .config import _retrieve_entry_points
+        def list_(ctx, **_: typing.Any):
+            """List installed configuration resources."""
+            from importlib.metadata import entry_points  # type: ignore
 
-            entry_points: dict[str, EntryPoint] = {
-                e.name: e for e in _retrieve_entry_points(entry_point_group)
+            entry_points: dict[str, EntryPoint] = {  # type: ignore
+                e.name: e for e in entry_points(group=entry_point_group)
             }
 
             # all modules with configuration resources
             modules: set[str] = {
                 # note: k.module does not exist on Python < 3.9
                 k.value.split(":")[0].rsplit(".", 1)[0]
-                for k in entry_points.values()
+                for k in entry_points.values()  # type: ignore
             }
             keep_modules: set[str] = set()
             for k in sorted(modules):
                 if k not in keep_modules and not any(
                     k.startswith(to_keep) for to_keep in keep_modules
                 ):
                     keep_modules.add(k)
             modules = keep_modules
 
             # sort data entries by originating module
             entry_points_by_module: dict[str, dict[str, EntryPoint]] = {}
             for k in modules:
                 entry_points_by_module[k] = {}
-                for name, ep in entry_points.items():
+                for name, ep in entry_points.items():  # type: ignore
                     # note: ep.module does not exist on Python < 3.9
                     module = ep.value.split(":", 1)[0]  # works on Python 3.8
                     if module.startswith(k):
                         entry_points_by_module[k][name] = ep
 
             for config_type in sorted(entry_points_by_module):
                 # calculates the longest config name so we offset the printing
@@ -749,41 +728,38 @@
                 # set-up printing options
                 print_string = "    %%-%ds   %%s" % (longest_name_length,)
                 # 79 - 4 spaces = 75 (see string above)
                 description_leftover = 75 - longest_name_length
 
                 click.echo(f"module: {config_type}")
                 for name in sorted(entry_points_by_module[config_type]):
-                    ep = entry_points[name]
+                    ep = entry_points[name]  # type: ignore
 
                     if (ctx.parent.params["verbose"] >= 1) or (
                         ctx.params["verbose"] >= 1
                     ):
                         try:
                             obj = ep.load()
 
                             if ":" in ep.value:  # it's an object
                                 summary = (
-                                    f"[{type(obj).__name__}] "
-                                    f"{pprint.pformat(obj)}"
+                                    f"[{type(obj).__name__}] {pprint.pformat(obj)}"
                                 )
                                 summary = summary.replace("\n", " ")
                             else:  # it's a whole module
                                 summary = "[module] "
                                 doc = inspect.getdoc(obj)
                                 if doc is not None:
                                     summary += doc.split("\n\n")[0]
                                     summary = summary.replace("\n", " ")
                                 else:
                                     summary += "[undocumented]"
 
                         except Exception as ex:
-                            summary = (
-                                "(cannot be loaded; add another -v for details)"
-                            )
+                            summary = "(cannot be loaded; add another -v for details)"
                             if (ctx.parent.params["verbose"] >= 2) or (
                                 ctx.params["verbose"] >= 2
                             ):
                                 logger.exception(ex)
 
                     else:
                         summary = ""
@@ -803,38 +779,38 @@
         @click.argument(
             "name",
             required=True,
             nargs=-1,
         )
         @verbosity_option(logger=logger)
         def describe(ctx, name, **_: typing.Any):
-            """Describes a specific configuration resource."""
-            from .config import _retrieve_entry_points
+            """Describe a specific configuration resource."""
+            from importlib.metadata import entry_points  # type: ignore
 
-            entry_points: dict[str, EntryPoint] = {
-                e.name: e for e in _retrieve_entry_points(entry_point_group)
+            entry_points: dict[str, EntryPoint] = {  # type: ignore
+                e.name: e for e in entry_points(group=entry_point_group)
             }
 
             for k in name:
-                if k not in entry_points:
+                if k not in entry_points:  # type: ignore
                     logger.error(f"Cannot find configuration resource `{k}'")
                     continue
-                ep = entry_points[k]
+                ep = entry_points[k]  # type: ignore
                 click.echo(f"Configuration: {ep.name}")
                 click.echo(f"Python object: {ep.value}")
                 click.echo("")
                 mod = ep.load()
 
                 if ":" not in ep.value:
                     if (ctx.parent.params["verbose"] >= 1) or (
                         ctx.params["verbose"] >= 1
                     ):
                         fname = inspect.getfile(mod)
                         click.echo("Contents:")
-                        with open(fname) as f:
+                        with pathlib.Path(fname).open() as f:
                             click.echo(f.read())
                     else:  # only output documentation, if module
                         doc = inspect.getdoc(mod)
                         if doc and doc.strip():
                             click.echo("Documentation:")
                             click.echo(doc)
 
@@ -849,47 +825,48 @@
         @click.argument(
             "destination",
             required=True,
             nargs=1,
         )
         @verbosity_option(logger=logger)
         def copy(source, destination, **_: typing.Any):
-            """Copies a specific configuration resource so it can be modified
-            locally."""
-
-            from .config import _retrieve_entry_points
+            """Copy a specific configuration resource so it can be modified
+            locally.
+            """
+            from importlib.metadata import entry_points  # type: ignore
 
-            entry_points: dict[str, EntryPoint] = {
-                e.name: e for e in _retrieve_entry_points(entry_point_group)
+            entry_points: dict[str, EntryPoint] = {  # type: ignore
+                e.name: e for e in entry_points(group=entry_point_group)
             }
 
-            if source not in entry_points:
+            if source not in entry_points:  # type: ignore
                 logger.error(f"Cannot find configuration resource `{source}'")
                 return 1
-            ep = entry_points[source]
+            ep = entry_points[source]  # type: ignore
             mod = ep.load()
             src_name = inspect.getfile(mod)
             logger.info(f"cp {src_name} -> {destination}")
             shutil.copyfile(src_name, destination)
 
+            return None
+
         return group_wrapper
 
     return group_decorator
 
 
-def log_parameters(
-    logger_handle: logging.Logger, ignore: tuple[str] | None = None
-):
-    """Logs the click parameters with the logging module.
-
-    Arguments:
-
-        logger: The :py:class:`logging.Logger` handle to write debug information into.
+def log_parameters(logger_handle: logging.Logger, ignore: tuple[str] | None = None):
+    """Log the click parameters with the logging module.
 
-        ignore : List of the parameters to ignore when logging. (Tuple)
+    Parameters
+    ----------
+    logger
+        The :py:class:`logging.Logger` handle to write debug information into.
+    ignore
+        List of the parameters to ignore when logging. (Tuple)
     """
     ignore = ignore or tuple()
     ctx = click.get_current_context()
     # do not sort the ctx.params dict. The insertion order is kept in Python 3
     # and is useful (but not necessary so works on Python 2 too).
     for k, v in ctx.params.items():
         if k in ignore:
```

### Comparing `clapper-1.0.1/src/clapper/config.py` & `clapper-1.1.0/src/clapper/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Functionality to implement python-based config file parsing and loading."""
 
-from __future__ import annotations
-
 import logging
-import os.path
 import pathlib
 import pkgutil
-import sys
 import types
 import typing
 
 from importlib.abc import FileLoader
 from importlib.metadata import EntryPoint, entry_points
 
 logger = logging.getLogger(__name__)
 
 _LOADED_CONFIGS = []
 """Small gambiarra (https://www.urbandictionary.com/define.php?term=Gambiarra)
 to avoid the garbage collector to collect some already imported modules."""
 
 
 def _load_context(path: str, mod: types.ModuleType) -> types.ModuleType:
-    """Loads the Python file as module, returns a resolved context.
+    """Load the Python file as module, returns a resolved context.
 
     This function is implemented in a way that is both Python 2 and Python 3
     compatible. It does not directly load the python file, but reads its
     contents in memory before Python-compiling it. It leaves no traces on the
     file system.
 
     Arguments:
@@ -45,40 +40,40 @@
                m = types.ModuleType("name")
                m.__dict__.update(ctxt)
 
             ``ctxt`` is a python dictionary mapping strings to object values
             representing the contents of the module to be created.
 
 
-    Returns:
-
+    Returns
+    -------
         A python module with the fully resolved context
     """
     # executes the module code on the context of previously imported modules
-    with open(path, "rb") as f:
+    with pathlib.Path(path).open("rb") as f:
         exec(compile(f.read(), path, "exec"), mod.__dict__)
 
     return mod
 
 
 def _get_module_filename(module_name: str) -> str | None:
-    """Resolves a module name to an actual Python file.
+    """Resolve a module name to an actual Python file.
 
     This function will return the path to the file containing the module named
     at ``module_name``.  Values for this parameter are dot-separated module
     names such as ``expose.config``.
 
 
     Arguments:
 
         module_name: The name of the module to search
 
 
-    Returns:
-
+    Returns
+    -------
         The path that corresponds to file implementing the provided module name
     """
     try:
         loader = pkgutil.get_loader(module_name)
         if isinstance(loader, FileLoader):
             return str(loader.path)
         return None
@@ -92,122 +87,96 @@
     if isinstance(path, pathlib.Path):
         path = str(path)
 
     r = path.rsplit(":", 1)
     return r[0], (common_name if len(r) < 2 else r[1])
 
 
-def _retrieve_entry_points(group: str) -> typing.Iterable[EntryPoint]:
-    """Wraps various entry-point retrieval mechanisms.
-
-    For Python 3.9 and 3.10,
-    :py:func:`importlib.metadata.entry_points()`
-    returns a dictionary keyed by entry-point group names.  From Python
-    3.10
-    onwards, one may pass the ``group`` keyword to that function to
-    enable
-    pre-filtering, or use the ``select()`` method on the returned value,
-    which
-    is no longer a dictionary.
-
-    For anything before Python 3.8, you must use the backported library
-    ``importlib_metadata``.
-    """
-    if sys.version_info[:2] < (3, 10):
-        all_entry_points = entry_points()
-        return all_entry_points.get(group, [])  # Python 3.9
-
-    return entry_points(group=group)  # Python 3.10 and above
-
-
 def _resolve_entry_point_or_modules(
     paths: list[str | pathlib.Path],
     entry_point_group: str | None = None,
     common_name: str | None = None,
 ) -> tuple[list[str], list[str], list[str]]:
-    """Resolves a mixture of paths, entry point names, and module names to
+    """Resolve a mixture of paths, entry point names, and module names to
     path.
 
     This function can resolve actual file system paths, ``setup.py``
     entry-point names and module names to a set of file system paths.
 
     Examples of things that can be resolved by this function are:
     ``["/tmp/config.py", "my-config", "expose.config"]`` (an actualy filesystem
     path, an entry-point described in a ``setup.py`` file, or the name of a
     python module.
 
-
-    Arguments:
-
-        paths: An iterable strings that either point to actual files, are entry
-            point names, or are module names.
-
-        entry_point_group: The entry point group name to search in entry
-            points.
-
-        common_name: It will be used as a default name for object names. See
-            the ``attribute_name`` parameter from :py:func:`load`.
+    Parameters
+    ----------
+    paths
+        An iterable strings that either point to actual files, are entry point
+        names, or are module names.
+    entry_point_group
+        The entry point group name to search in entry points.
+    common_name
+        It will be used as a default name for object names. See the
+        ``attribute_name`` parameter from :py:func:`load`.
 
 
-    Returns:
-
+    Returns
+    -------
         A tuple containing three lists of strings with:
 
         * The resolved paths pointing to existing files
         * The valid python module names to bind each of the files to, and
           finally,
         * The name of objects that are supposed to be picked from paths
 
 
-    Raises:
-
-        ValueError: If one of the paths cannot be resolved to an actual path to
-            a file.
+    Raises
+    ------
+    ValueError
+        If one of the paths cannot be resolved to an actual path to a file.
     """
 
     if entry_point_group is not None:
         entry_point_dict: dict[str, EntryPoint] = {
-            e.name: e for e in _retrieve_entry_points(entry_point_group)
+            e.name: e for e in entry_points(group=entry_point_group)
         }
     else:
         entry_point_dict = {}
 
     files = []
     module_names = []
     object_names = []
 
     for path in paths:
-        module_name = (
-            "user_config"  # fixed module name for files with full paths
-        )
+        module_name = "user_config"  # fixed module name for files with full paths
         resolved_path, object_name = _object_name(path, common_name)
 
         # if it already points to a file, then do nothing
-        if os.path.isfile(resolved_path):
+        if pathlib.Path(resolved_path).is_file():
             pass
 
         # If it is an entry point name, collect path and module name
         elif resolved_path in entry_point_dict:
             entry = entry_point_dict[resolved_path]
             module_name = entry.module
             object_name = entry.attr if entry.attr else common_name
 
             resolved_path = _get_module_filename(module_name)
-            if resolved_path is None or not os.path.isfile(resolved_path):
+            if resolved_path is None or not pathlib.Path(resolved_path).is_file():
                 raise ValueError(
                     f"The specified entry point `{path}' pointing to module "
                     f"`{module_name}' and resolved to `{resolved_path}' does "
                     f"not point to an existing file."
                 )
 
         # If it is not a path nor an entry point name, it is a module name then?
         else:
             # if we have gotten here so far then path must resolve as a module
             resolved_path = _get_module_filename(resolved_path)
-            if resolved_path is None or not os.path.isfile(resolved_path):
+            if resolved_path is None or not pathlib.Path(resolved_path).is_file():
                 raise ValueError(
                     f"The specified path `{path}' is not a file, a entry "
                     f"point name, or a known-module name"
                 )
 
         files.append(resolved_path)
         module_names.append(module_name)
@@ -218,57 +187,55 @@
 
 def load(
     paths: list[str | pathlib.Path],
     context: dict[str, typing.Any] | None = None,
     entry_point_group: str | None = None,
     attribute_name: str | None = None,
 ) -> types.ModuleType | typing.Any:
-    """Loads a set of configuration files, in sequence.
+    """Load a set of configuration files, in sequence.
 
     This method will load one or more configuration files. Every time a
     configuration file is loaded, the context (variables) loaded from the
     previous file is made available, so the new configuration file can override
     or modify this context.
 
+    Parameters
+    ----------
+    paths
+        A list or iterable containing paths (relative or absolute) of
+        configuration files that need to be loaded in sequence. Each
+        configuration file is loaded by creating/modifying the context
+        generated after each file readout.
+    context
+        If provided, start the readout of the first configuration file with the
+        given context. Otherwise, create a new internal context.
+    entry_point_group
+        If provided, it will treat non-existing file paths as entry point names
+        under the ``entry_point_group`` name.
+    attribute_name
+        If provided, will look for the ``attribute_name`` variable inside the
+        loaded files. Paths ending with ``some_path:variable_name`` can
+        override the ``attribute_name``. The ``entry_point_group`` must
+        provided as well ``attribute_name`` is not ``None``.
 
-    Arguments:
-
-        paths: A list or iterable containing paths (relative or absolute) of
-            configuration files that need to be loaded in sequence. Each
-            configuration file is loaded by creating/modifying the context
-            generated after each file readout.
-
-        context: If provided, start the readout of the first configuration file
-            with the given context. Otherwise, create a new internal context.
-
-        entry_point_group: If provided, it will treat non-existing file paths
-            as entry point names under the ``entry_point_group`` name.
-
-        attribute_name: If provided, will look for the ``attribute_name`` variable
-            inside the loaded files. Paths ending with
-            ``some_path:variable_name`` can override the ``attribute_name``. The
-            ``entry_point_group`` must provided as well ``attribute_name`` is
-            not ``None``.
-
-
-    Returns:
 
+    Returns
+    -------
         A module representing the resolved context, after loading the provided
         modules and resolving all variables. If ``attribute_name`` is given,
         the object with the given ``attribute_name`` name (or the name provided
         by user) is returned instead of the module.
 
 
-    Raises:
-
-        ImportError: If attribute_name is given but the object does not exist
-            in the paths.
-
-        ValueError: If attribute_name is given but entry_point_group is not
-            given.
+    Raises
+    ------
+    ImportError
+        If attribute_name is given but the object does not exist in the paths.
+    ValueError
+        If attribute_name is given but entry_point_group is not given.
     """
 
     # resolve entry points to paths
     resolved_paths, names, object_names = _resolve_entry_point_or_modules(
         paths, entry_point_group, attribute_name
     )
 
@@ -288,17 +255,15 @@
     for k, n in zip(resolved_paths, names):
         logger.debug("Loading configuration file `%s'...", k)
         mod = types.ModuleType(n)
         # remove the keys that might break the loading of the next config file.
         ctxt.__dict__.pop("__name__", None)
         ctxt.__dict__.pop("__package__", None)
         # do not propogate __ variables
-        context = {
-            k: v for k, v in ctxt.__dict__.items() if not k.startswith("__")
-        }
+        context = {k: v for k, v in ctxt.__dict__.items() if not k.startswith("__")}
         mod.__dict__.update(context)
         _LOADED_CONFIGS.append(mod)
         ctxt = _load_context(k, mod)
 
     if not attribute_name:
         return mod
 
@@ -311,26 +276,25 @@
             f"your configuration files: {', '.join(resolved_paths)}"
         )
 
     return getattr(mod, attribute_name)
 
 
 def mod_to_context(mod: types.ModuleType) -> dict[str, typing.Any]:
-    """Converts the loaded module of :py:func:`load` to a dictionary context.
+    """Convert the loaded module of :py:func:`load` to a dictionary context.
 
     This function removes all the variables that start and end with ``__``.
 
+    Parameters
+    ----------
+    mod
+        a Python module, e.g., as returned by :py:func:`load`.
 
-    Arguments:
-
-        mod: a Python module, e.g., as returned by :py:func:`load`.
-
-
-    Returns:
-
+    Returns
+    -------
         The context that was in ``mod``, as a dictionary mapping strings to
         objects.
     """
     return {
         k: v
         for k, v in mod.__dict__.items()
         if not (k.startswith("__") and k.endswith("__"))
@@ -338,43 +302,43 @@
 
 
 def resource_keys(
     entry_point_group: str,
     exclude_packages: tuple[str, ...] = tuple(),
     strip: tuple[str, ...] = ("dummy",),
 ) -> list[str]:
-    """Reads and returns all resources that are registered on a entry-point
+    """Read and returns all resources that are registered on a entry-point
     group.
 
     Entry points from the given ``exclude_packages`` list are ignored.  Notice
     we are using :py:mod:`importlib.metadata` to load entry-points, and that
     that entry point distribution (``.dist`` attribute) was only added to
     Python in version 3.10.  We therefore currently only verify if the named
     resource does not start with any of the strings provided in
     `exclude_package``.
 
+    Parameters
+    ----------
+    entry_point_group
+        The entry point group name.
+    exclude_packages
+        List of packages to exclude when finding resources.
+    strip
+        Entrypoint names that start with any value in ``strip`` will be
+        ignored.
 
-    Arguments:
-
-        entry_point_group: The entry point group name.
-
-        exclude_packages: List of packages to exclude when finding resources.
-
-        strip: Entrypoint names that start with any value in ``strip`` will be
-            ignored.
-
-
-    Returns:
 
+    Returns
+    -------
         Alphabetically sorted list of resources matching your query
     """
 
     ret_list = [
         k.name
-        for k in _retrieve_entry_points(entry_point_group)
+        for k in entry_points(group=entry_point_group)
         if (
             (not k.name.strip().startswith(exclude_packages))
             and (not k.name.startswith(strip))
         )
     ]
     ret_list = list(dict.fromkeys(ret_list))  # order-preserving uniq
     return sorted(ret_list)
```

### Comparing `clapper-1.0.1/src/clapper/logging.py` & `clapper-1.1.0/src/clapper/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
-""":py:class:`logging.Logger` setup and stream separation"""
+""":py:class:`logging.Logger` setup and stream separation."""
 
 import logging
 import sys
 import typing
 
 
 # debug and info messages are written to sys.stdout
@@ -20,19 +19,19 @@
 
     def filter(self, record):
         return record.levelno <= logging.INFO
 
 
 def setup(
     logger_name: str,
-    format: str = "[%(levelname)s] %(message)s (%(name)s, %(asctime)s)",
+    format: str = "[%(levelname)s] %(message)s (%(name)s, %(asctime)s)",  # noqa: A002
     low_level_stream: typing.TextIO = sys.stdout,
     high_level_stream: typing.TextIO = sys.stderr,
 ) -> logging.Logger:
-    """This function returns a logger object that is ready for console logging.
+    """Return a logger object that is ready for console logging.
 
     Retrieves (as with :py:func:`logging.getLogger()`) the given logger, and
     then attaches 2 handlers (defined on the module) to it:
 
     1. A :py:class:`logging.StreamHandler` to output messages with level equal
        or lower than ``logging.INFO`` to the text-I/O stream
        ``low_level_stream``.  This is implemented by attaching a filter to the
@@ -42,62 +41,58 @@
        level set to ``logging.WARNING``.
 
     A new formatter, with the format string as defined by the ``format``
     argument is set on both handlers.  In this way, the global logger level can
     still be controlled from one single place.  If output is generated, then it
     is sent to the right stream.
 
+    Parameters
+    ----------
+    logger_name
+        The name of the module to generate logs for
+    format
+        The format of the logs, see :py:class:`logging.LogRecord` for more
+        details. By default, the log contains the logger name, the log time,
+        the log level and the massage.
+    low_level_stream
+        The stream where to output info messages and below
+    high_level_stream
+        The stream where to output warning messages and above
 
-    Arguments:
-
-        logger_name: The name of the module to generate logs for
-
-        format: The format of the logs, see :py:class:`logging.LogRecord` for
-            more details. By default, the log contains the logger name, the log
-            time, the log level and the massage.
-
-        low_level_stream: The stream where to output info messages and below
-
-        high_level_stream: The stream where to output warning messages and
-            above
-
-
-    Returns:
-
+    Returns
+    -------
         The configured logger. The same logger can be retrieved using the
         :py:func:`logging.getLogger` function.
     """
 
     logger = logging.getLogger(logger_name)
 
     formatter = logging.Formatter(format)
 
     handlers_installed = {k.name: k for k in logger.handlers}
     debug_logger_name = f"debug_info+{logger_name}"
 
     # First check that logger with a matching name or stream is not already
     # there before attaching a new one.
     if (debug_logger_name not in handlers_installed) or (
-        getattr(handlers_installed[debug_logger_name], "stream")
-        != low_level_stream
+        getattr(handlers_installed[debug_logger_name], "stream") != low_level_stream
     ):
         debug_info = logging.StreamHandler(low_level_stream)
         debug_info.setLevel(logging.DEBUG)
         debug_info.setFormatter(formatter)
         debug_info.addFilter(_InfoFilter())
         debug_info.name = debug_logger_name
         logger.addHandler(debug_info)
 
     error_logger_name = f"warn_err+{logger_name}"
 
     # First check that logger with a matching name or stream is not already
     # there before attaching a new one.
     if (error_logger_name not in handlers_installed) or (
-        getattr(handlers_installed[error_logger_name], "stream")
-        != high_level_stream
+        getattr(handlers_installed[error_logger_name], "stream") != high_level_stream
     ):
         warn_err = logging.StreamHandler(high_level_stream)
         warn_err.setLevel(logging.WARNING)
         warn_err.setFormatter(formatter)
         warn_err.name = error_logger_name
         logger.addHandler(warn_err)
```

### Comparing `clapper-1.0.1/src/clapper/rc.py` & `clapper-1.1.0/src/clapper/rc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
-
 """Implements a global configuration system setup and readout."""
 
-from __future__ import annotations
-
 import collections.abc
 import io
 import json
 import logging
 import pathlib
 import typing
 
@@ -28,35 +25,33 @@
     operating system dependent, c.f. `XDG defaults`_).
 
     This object may be used (with limited functionality) like a dictionary.  In
     this mode, objects of this class read and write values to the ``DEFAULT``
     section.  The ``len()`` method will also return the number of variables set
     at the ``DEFAULT`` section as well.
 
-
-    Arguments:
-
-        path: The path, absolute or relative, to the file containing the user
-            defaults to read.  If `path` is a relative path, then it is
-            considered relative to the directory defined by the environment
-            variable ``${XDG_CONFIG_HOME}`` (read `XDG defaults`_ for details on
-            the default location of this directory in the various operating
-            systems).  The tilde (`~`) character may be used to represent the
-            user home, and is automatically expanded.
-
-        logger: A logger to use for messaging operations.  If not set, use this
-            module's logger.
-
-
-    Attributes:
-
-        path: The current path to the user defaults base file.
-
-
-    .. _XDG defaults: https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
+    Parameters
+    ----------
+    path
+        The path, absolute or relative, to the file containing the user
+        defaults to read.  If `path` is a relative path, then it is considered
+        relative to the directory defined by the environment variable
+        ``${XDG_CONFIG_HOME}`` (read `XDG defaults
+        <https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html>`_
+        for details on the default location of this directory in the various
+        operating systems).  The tilde (`~`) character may be used to represent
+        the user home, and is automatically expanded.
+    logger
+        A logger to use for messaging operations.  If not set, use this
+        module's logger.
+
+    Attributes
+    ----------
+    path
+        The current path to the user defaults base file.
     """
 
     def __init__(
         self,
         path: str | pathlib.Path,
         logger: logging.Logger | None = None,
     ) -> None:
@@ -68,19 +63,17 @@
             self.path = xdg.xdg_config_home() / self.path
 
         self.logger.info(f"User configuration file set to `{str(self.path)}'")
         self.data: dict[str, typing.Any] = {}
         self.read()
 
     def read(self) -> None:
-        """Reads configuration file, replaces any internal values."""
+        """Read configuration file, replaces any internal values."""
         if self.path.exists():
-            self.logger.debug(
-                "User configuration file exists, reading contents..."
-            )
+            self.logger.debug("User configuration file exists, reading contents...")
             self.data.clear()
 
             with self.path.open("rb") as f:
                 contents = f.read()
 
             # Support for legacy JSON file format.  Remove after sometime
             # FYI: today is September 16, 2022
@@ -101,15 +94,15 @@
 
             self.data.update(tomli.load(io.BytesIO(contents)))
 
         else:
             self.logger.debug("Initializing empty user configuration...")
 
     def write(self) -> None:
-        """Stores any modifications done on the user configuration."""
+        """Store any modifications done on the user configuration."""
         if self.path.exists():
             backup = pathlib.Path(str(self.path) + "~")
             self.logger.debug(f"Backing-up {str(self.path)} -> {str(backup)}")
             self.path.rename(backup)
 
         with self.path.open("wb") as f:
             tomli_w.dump(self.data, f)
@@ -121,15 +114,15 @@
         tomli_w.dump(self.data, t)
         return t.getvalue().decode(encoding="utf-8")
 
     def __getitem__(self, k: str) -> typing.Any:
         if k in self.data:
             return self.data[k]
 
-        elif "." in k:
+        if "." in k:
             # search for a key with a matching name after the "."
             parts = k.split(".")
             base = self.data
             for n in range(len(parts)):
                 if parts[n] in base:
                     base = base[parts[n]]
                     if (not isinstance(base, dict)) and (n < (len(parts) - 1)):
@@ -153,15 +146,15 @@
             parts = k.split(".")
             base = self.data
             for n in range(len(parts) - 1):
                 base = base.setdefault(parts[n], {})
                 if not isinstance(base, dict):
                     raise KeyError(
                         f"You are trying to set configuration key "
-                        f"{k}, but {'.'.join(parts[:(n+1)])} is already a "
+                        f"{k}, but {'.'.join(parts[:(n + 1)])} is already a "
                         f"variable set in the file, and not a section"
                     )
             base[parts[-1]] = v
             return v
 
         # otherwise, defaults to the default behaviour
         return self.data.__setitem__(k, v)
@@ -181,15 +174,15 @@
                         # should not as we have more parts to go
                         break
                 else:
                     break
                 subkey = ".".join(parts[(n + 1) :])
                 if subkey in base:
                     del base[subkey]
-                    return
+                    return None
 
         # otherwise, defaults to the default behaviour
         return self.data.__delitem__(k)
 
     def __iter__(self) -> typing.Iterator[str]:
         return self.data.__iter__()
```

### Comparing `clapper-1.0.1/tests/conftest.py` & `clapper-1.1.0/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,24 +54,24 @@
     def invoke(self, cli, args=None, **kwargs):
         params = kwargs.copy()
         if self._in_pdb:
             params["catch_exceptions"] = False
 
         return super().invoke(cli, args=args, **params)
 
-    def isolation(self, input=None, env=None, color=False):
+    def isolation(self, input_=None, env=None, color=False):
         if self._in_pdb:
-            if input or env or color:
+            if input_ or env or color:
                 warnings.warn(
                     "CliRunner PDB un-isolation doesn't work if input/env/color are passed"
                 )
             else:
                 return self.isolation_pdb()
 
-        return super().isolation(input=input, env=env, color=color)
+        return super().isolation(input=input_, env=env, color=color)
 
     @contextlib.contextmanager
     def isolation_pdb(self):
         s = io.BytesIO(b"{stdout not captured because --pdb-trace}")
         yield (s, not self.mix_stderr and s)
```

### Comparing `clapper-1.0.1/tests/data/test_dump_config.py` & `clapper-1.1.0/tests/data/test_dump_config.py`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/tests/data/test_dump_config2.py` & `clapper-1.1.0/tests/data/test_dump_config2.py`

 * *Files identical despite different names*

### Comparing `clapper-1.0.1/tests/test_click.py` & `clapper-1.1.0/tests/test_click.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 import difflib
 import logging
 
 import click
 
-from click.testing import CliRunner
-
 from clapper.click import (
     AliasedGroup,
     ConfigCommand,
     ResourceOption,
     log_parameters,
     verbosity_option,
 )
+from click.testing import CliRunner
 
 
 def test_prefix_aliasing():
     @click.group(cls=AliasedGroup)
     def cli():
         pass
 
@@ -59,15 +58,15 @@
 
 
 def test_commands_with_config_2():
     # test option with valid default value
     @click.command(cls=ConfigCommand, entry_point_group="clapper.test.config")
     @click.option("-a", type=click.INT, cls=ResourceOption)
     def cli(a, **_):
-        assert type(a) == int, (type(a), a)
+        assert isinstance(a, int), (type(a), a)
         click.echo(f"{a}")
 
     runner = CliRunner()
 
     result = runner.invoke(cli, ["first"])
     assert result.exit_code == 0
     assert result.output.strip() == "1"
@@ -111,15 +110,15 @@
 
     result = runner.invoke(cli, ["first", "-a", "3"])
     assert result.exit_code == 0
     assert result.output.strip() == "3"
 
 
 def _assert_config_dump(output, ref, ref_date):
-    with output.open("rt") as f, open(ref) as f2:
+    with output.open("rt") as f, ref.open() as f2:
         diff = difflib.ndiff(f.readlines(), f2.readlines())
         important_diffs = [k for k in diff if k.startswith(("+", "-"))]
 
         # check and remove differences on the generation date
         if (
             len(important_diffs) >= 2
             and important_diffs[0].startswith(
@@ -221,28 +220,24 @@
 
         [CONFIG]...           BLA BLA BLA BLA
         """
         pass
 
     runner = CliRunner()
     output = tmp_path / "test_dump.py"
-    result = runner.invoke(
-        test, ["test", "-H", str(output)], catch_exceptions=False
-    )
+    result = runner.invoke(test, ["test", "-H", str(output)], catch_exceptions=False)
 
     ref = datadir / "test_dump_config2.py"
     assert result.exit_code == 0
     _assert_config_dump(output, ref, "10/09/2022")
 
 
 def test_config_command_with_callback_options():
     @click.command(cls=ConfigCommand, entry_point_group="clapper.test.config")
-    @verbosity_option(
-        logging.getLogger(__name__), envvar="VERBOSE", cls=ResourceOption
-    )
+    @verbosity_option(logging.getLogger(__name__), envvar="VERBOSE", cls=ResourceOption)
     @click.pass_context
     def cli(ctx, **_):
         verbose = ctx.meta["verbose"]
         assert verbose == 2
 
     runner = CliRunner()
     result = runner.invoke(cli, ["verbose-config"])
@@ -302,15 +297,15 @@
 
 def test_log_parameter():
     # Fake logger that checks if log_parameters accesses it
     class DummyLogger:
         def __init__(self):
             self.accessed = False
 
-        def debug(self, str, k, v):
+        def debug(self, s, k, v):
             self.accessed = True
 
     @click.command()
     @click.option(
         "-a",
         "--a",
     )
@@ -323,15 +318,15 @@
     result = runner.invoke(cli_log, ["-a", "aparam"])
     assert result.exit_code == 0
 
 
 def test_log_parameter_with_ignore():
     # Fake logger that ensures that the parameter 'a' is ignored
     class DummyLogger:
-        def debug(self, str, k, v):
+        def debug(self, s, k, v):
             assert "a" not in k
 
     @click.command()
     @click.option("-a", "--a")
     @click.option(
         "-b",
         "--b",
```

### Comparing `clapper-1.0.1/tests/test_config.py` & `clapper-1.1.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 # SPDX-License-Identifier: BSD-3-Clause
 
 import filecmp
 import io
 
 import pytest
 
-from click.testing import CliRunner
-
 from clapper.click import config_group
 from clapper.config import load, mod_to_context
 from clapper.logging import setup as logger_setup
+from click.testing import CliRunner
 
 
 def test_basic(datadir):
     c = load([datadir / "basic_config.py"])
     assert hasattr(c, "a") and c.a == 1
     assert hasattr(c, "b") and c.b == 3
 
@@ -54,17 +53,15 @@
     )
     assert hasattr(c, "a") and c.a == 1
     assert hasattr(c, "b") and c.b == 6
     assert hasattr(c, "cplx") and isinstance(c.cplx, dict)
 
 
 def test_config_with_entry_point():
-    c = load(
-        ["first", "second", "complex"], entry_point_group="clapper.test.config"
-    )
+    c = load(["first", "second", "complex"], entry_point_group="clapper.test.config")
     assert hasattr(c, "a") and c.a == 1
     assert hasattr(c, "b") and c.b == 6
     assert hasattr(c, "cplx") and isinstance(c.cplx, dict)
 
 
 def test_config_with_entry_point_file_missing():
     with pytest.raises(ValueError):
@@ -170,17 +167,15 @@
 
 
 def test_config_click_describe_error(cli_messages):
     cli, messages = cli_messages
     runner = CliRunner()
     result = runner.invoke(cli, ["describe", "not-found"])
     assert result.exit_code == 0
-    assert (
-        "Cannot find configuration resource `not-found'" in messages.getvalue()
-    )
+    assert "Cannot find configuration resource `not-found'" in messages.getvalue()
 
 
 def test_config_click_copy(cli_messages, datadir, tmp_path):
     cli = cli_messages[0]
     runner = CliRunner()
     dest = tmp_path / "file.py"
     result = runner.invoke(cli, ["copy", "first", str(dest)])
@@ -190,11 +185,8 @@
 
 def test_config_click_copy_error(cli_messages, datadir, tmp_path):
     cli, messages = cli_messages
     runner = CliRunner()
     dest = tmp_path / "file.py"
     result = runner.invoke(cli, ["copy", "firstx", str(dest)])
     assert result.exit_code == 0
-    assert (
-        "[ERROR] Cannot find configuration resource `firstx'"
-        in messages.getvalue()
-    )
+    assert "[ERROR] Cannot find configuration resource `firstx'" in messages.getvalue()
```

### Comparing `clapper-1.0.1/tests/test_logging.py` & `clapper-1.1.0/tests/test_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import io
 import logging
 
-import click
-
-from click.testing import CliRunner
-
 import clapper.logging
+import click
 
 from clapper.click import verbosity_option
+from click.testing import CliRunner
 
 
 def test_logger_setup():
     lo = io.StringIO()
     hi = io.StringIO()
 
     logger = clapper.logging.setup(
```

### Comparing `clapper-1.0.1/tests/test_rc.py` & `clapper-1.1.0/tests/test_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-FileCopyrightText: Copyright © 2022 Idiap Research Institute <contact@idiap.ch>
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import filecmp
 import logging
 import os
+import pathlib
 import shutil
 
 import pytest
 
-from click.testing import CliRunner
-
 from clapper.click import user_defaults_group
 from clapper.rc import UserDefaults
+from click.testing import CliRunner
 
 
 def _check_userdefaults_ex1_contents(rc):
     # checks that it matches the contents of that file
 
     assert rc["string"] == "this is a string"
     assert rc["integer"] == 42
@@ -153,15 +153,15 @@
     rc = UserDefaults("does-not-exist")
     assert not rc
 
     rc["section2.another_int"] = 42
     rc.clear()
 
     assert not rc
-    assert not os.path.exists("does-not-exist")
+    assert not pathlib.Path("does-not-exist").exists()
 
 
 def test_rc_reload(tmp_path):
     rc = UserDefaults(tmp_path / "new-rc")
     rc["section1.foo"] = "bar"
     rc["section1.an_int"] = 15
     rc.write()
@@ -181,15 +181,15 @@
 
 def test_rc_str(tmp_path):
     rc = UserDefaults(tmp_path / "new-rc")
     rc["foo"] = "bar"
     rc["section1.an_int"] = 15
     rc.write()
 
-    assert open(tmp_path / "new-rc").read() == str(rc)
+    assert (tmp_path / "new-rc").open().read() == str(rc)
 
 
 def test_rc_json_legacy(datadir, tmp_path):
     shutil.copy(datadir / "oldjson.cfg", tmp_path)
     rc = UserDefaults(tmp_path / "oldjson.cfg")
 
     assert rc["string"] == "this is a string"
```

