# Comparing `tmp/ddeutil-0.3.2.tar.gz` & `tmp/ddeutil-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil-0.3.2.tar", last modified: Sun May  5 07:13:16 2024, max compression
+gzip compressed data, was "ddeutil-0.3.3.tar", last modified: Sun May  5 09:27:37 2024, max compression
```

## Comparing `ddeutil-0.3.2.tar` & `ddeutil-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.713090 ddeutil-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 07:13:12.000000 ddeutil-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 07:13:16.713090 ddeutil-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-05 07:13:12.000000 ddeutil-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-05 07:13:12.000000 ddeutil-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 07:13:16.713090 ddeutil-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.705090 ddeutil-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.705090 ddeutil-0.3.2/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/src/ddeutil/core/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-05 07:13:12.000000 ddeutil-0.3.2/src/ddeutil/core/threader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/src/ddeutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 07:13:16.000000 ddeutil-0.3.2/src/ddeutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 07:13:16.709090 ddeutil-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_dtutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-05 07:13:12.000000 ddeutil-0.3.2/tests/test_randomly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.836744 ddeutil-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 09:27:29.000000 ddeutil-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 09:27:37.836744 ddeutil-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-05 09:27:29.000000 ddeutil-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-05 09:27:29.000000 ddeutil-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 09:27:37.836744 ddeutil-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.828744 ddeutil-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.828744 ddeutil-0.3.3/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.832744 ddeutil-0.3.3/src/ddeutil/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.836744 ddeutil-0.3.3/src/ddeutil/core/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/base/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-05 09:27:29.000000 ddeutil-0.3.3/src/ddeutil/core/threader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.836744 ddeutil-0.3.3/src/ddeutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-05 09:27:37.000000 ddeutil-0.3.3/src/ddeutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-05 09:27:37.000000 ddeutil-0.3.3/src/ddeutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 09:27:37.000000 ddeutil-0.3.3/src/ddeutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-05 09:27:37.000000 ddeutil-0.3.3/src/ddeutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 09:27:37.000000 ddeutil-0.3.3/src/ddeutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 09:27:37.836744 ddeutil-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-05 09:27:29.000000 ddeutil-0.3.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-05 09:27:29.000000 ddeutil-0.3.3/tests/test_dtutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-05 09:27:29.000000 ddeutil-0.3.3/tests/test_randomly.py
```

### Comparing `ddeutil-0.3.2/LICENSE` & `ddeutil-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/PKG-INFO` & `ddeutil-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil-0.3.2/README.md` & `ddeutil-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/pyproject.toml` & `ddeutil-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "ddeutil.core.__about__.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
-include = ["ddeutil.core"]
 
 [tool.shelf.version]
 version = "./src/ddeutil/core/__about__.py"
 changelog = "CHANGELOG.md"
 
 [tool.coverage.run]
 branch = true
@@ -119,33 +118,35 @@
     | build
     | dist
 )/
 """
 
 [tool.ruff]
 line-length = 80
+# Exclude a variety of commonly ignored directories.
+exclude = [
+    ".git",
+    ".mypy_cache",
+    ".ruff_cache",
+    "__pypackages__",
+    "build",
+    "dist",
+    "venv",
+]
+
+[tool.ruff.lint]
 select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
 ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".git",
-    ".mypy_cache",
-    ".ruff_cache",
-    "__pypackages__",
-    "build",
-    "dist",
-    "venv",
-]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `ddeutil-0.3.2/src/ddeutil/core/__init__.py` & `ddeutil-0.3.3/src/ddeutil/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/src/ddeutil/core/decorator.py` & `ddeutil-0.3.3/src/ddeutil/core/decorator.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/src/ddeutil/core/dtutils.py` & `ddeutil-0.3.3/src/ddeutil/core/dtutils.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/src/ddeutil/core/threader.py` & `ddeutil-0.3.3/src/ddeutil/core/threader.py`

 * *Files identical despite different names*

### Comparing `ddeutil-0.3.2/src/ddeutil.egg-info/PKG-INFO` & `ddeutil-0.3.3/src/ddeutil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil
-Version: 0.3.2
+Version: 0.3.3
 Summary: Data Developer & Engineer Core Utility Objects
 Author-email: korawica <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/ddeutils/ddeutil/
 Project-URL: Source Code, https://github.com/ddeutils/ddeutil/
 Keywords: data,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil-0.3.2/tests/test_randomly.py` & `ddeutil-0.3.3/tests/test_randomly.py`

 * *Files identical despite different names*

