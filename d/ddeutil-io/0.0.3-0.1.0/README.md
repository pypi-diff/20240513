# Comparing `tmp/ddeutil-io-0.0.3.tar.gz` & `tmp/ddeutil_io-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil-io-0.0.3.tar", last modified: Tue Sep 26 06:18:17 2023, max compression
+gzip compressed data, was "ddeutil_io-0.1.0.tar", last modified: Sun May  5 10:02:19 2024, max compression
```

## Comparing `ddeutil-io-0.0.3.tar` & `ddeutil_io-0.1.0.tar`

### file list

```diff
@@ -1,34 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.746486 ddeutil-io-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.746486 ddeutil-io-0.0.3/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.746486 ddeutil-io-0.0.3/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/src/ddeutil/io/base/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/base/pathutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/base/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13387 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7164 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    22473 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)    10113 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2023-09-26 06:18:17.000000 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2023-09-26 06:18:17.000000 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 06:18:17.000000 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-26 06:18:17.000000 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-26 06:18:17.000000 ddeutil-io-0.0.3/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 06:18:17.750486 ddeutil-io-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2023-09-26 06:18:05.000000 ddeutil-io-0.0.3/tests/test_register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.689370 ddeutil_io-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.689370 ddeutil_io-0.1.0/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.693369 ddeutil_io-0.1.0/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.693369 ddeutil_io-0.1.0/src/ddeutil/io/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/base/pathutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/base/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13387 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7164 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22212 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10113 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/src/ddeutil/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/src/ddeutil/node/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28819 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/base/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/base/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35564 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/datasets_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11029 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15743 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/src/ddeutil/node/vendors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/vendors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6279 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/vendors/boto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/vendors/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-05 10:02:15.000000 ddeutil_io-0.1.0/src/ddeutil/node/vendors/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 10:02:19.697369 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-05-05 10:02:19.000000 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-05 10:02:19.000000 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 10:02:19.000000 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-05 10:02:19.000000 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-05 10:02:19.000000 ddeutil_io-0.1.0/src/ddeutil_io.egg-info/top_level.txt
```

### Comparing `ddeutil-io-0.0.3/LICENSE` & `ddeutil_io-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/pyproject.toml` & `ddeutil_io-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 [project]
 name = "ddeutil-io"
 description = "Data Developer & Engineer IO Utility Objects"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {text = "MIT"}
-authors = [{ name = "korawica", email = "korawich.anu@gmail.com" }]
+authors = [{ name = "ddeutils", email = "korawich.anu@gmail.com" }]
 keywords = ['data', 'config', 'utility']
 classifiers = [
     "Topic :: Utilities",
     "Natural Language :: English",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.8.10"
 dependencies = [
     "ddeutil",
     "fmtutil",
     "pydantic==2.3.0",
     "deepdiff==6.3.1",
     "pyyaml==6.0.1",
+    "sqlalchemy==2.0.20",
+    "pandas==2.0.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/korawica/ddeutil-io/"
 "Source Code" = "https://github.com/korawica/ddeutil-io/"
 
 [project.optional-dependencies]
 dev = [
     "clishelf",
+    "python-dotenv==1.0.0",
+]
+s3 = [
+    "boto3>=1.28.49",
+]
+sftp = [
+    "sshtunnel==0.4.0",
 ]
 
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "ddeutil.io.__about__.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
-[tool.utils.version]
+[tool.shelf.version]
 version = "./src/ddeutil/io/__about__.py"
 changelog = "CHANGELOG.md"
 
 [tool.coverage.run]
 branch = true
 concurrency = ["thread", "multiprocessing"]
 source = ["ddeutil", "tests"]
@@ -73,15 +82,15 @@
 addopts = [
     "--strict-config",
     "--strict-markers",
 ]
 filterwarnings = ["error"]
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.9"
 files = ["ddeutil"]
 show_error_codes = true
 pretty = true
 strict = true
 local_partial_types = true
 warn_unreachable = true
 
@@ -93,15 +102,15 @@
 [[tool.mypy.overrides]]
 module = "tests.*"
 ignore_missing_imports = true
 check_untyped_defs = true
 
 [tool.black]
 line-length = 80
-target-version = ['py38']
+target-version = ['py39']
 exclude = """
 /(
     \\.git
     | \\.__pycache__
     | \\.idea
     | \\.ruff_cache
     | \\.mypy_cache
```

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/base/files.py` & `ddeutil_io-0.1.0/src/ddeutil/io/base/files.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/base/pathutils.py` & `ddeutil_io-0.1.0/src/ddeutil/io/base/pathutils.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/base/settings.py` & `ddeutil_io-0.1.0/src/ddeutil/io/base/settings.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/base/utils.py` & `ddeutil_io-0.1.0/src/ddeutil/io/base/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/config.py` & `ddeutil_io-0.1.0/src/ddeutil/io/config.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.0/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/models.py` & `ddeutil_io-0.1.0/src/ddeutil/io/models.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/register.py` & `ddeutil_io-0.1.0/src/ddeutil/io/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     List,
     NoReturn,
     Optional,
     Type,
     TypedDict,
 )
 
-import packaging.version
+# import packaging.version
 from dateutil.relativedelta import relativedelta
 from ddeutil.core import (
     concat,
     hash_all,
     merge_dict,
     rsplit,
 )
@@ -32,14 +32,15 @@
 from fmtutil import (
     ConstantType,
     Datetime,
     FormatterArgumentError,
     FormatterGroup,
     FormatterGroupType,
     Naming,
+    VerPackage,
     Version,
     make_const,
     make_group,
 )
 
 from .base.pathutils import remove_file
 from .config import ConfFile, OpenFile
@@ -415,35 +416,31 @@
         elif _dt := self.data().get("updt"):
             return datetime.datetime.strptime(
                 _dt,
                 self.params.engine.values.datetime_fmt,
             )
         return self.updt
 
-    def version(self, _next: bool = False) -> packaging.version.Version:
+    def version(self, _next: bool = False) -> VerPackage:
         """Generate version value from the pick method. If version value does
         not exist from configuration data, this property will return the
         default, `v0.0.1`. If the initialization process tracking some change
         from configuration data between metadata and the latest data in the
         stage, the _next will be generated.
 
-        :return: packaging.version.Version
+        :return: VerPackage
         """
-        _vs = packaging.version.parse(self.data().get("version", "v0.0.1"))
-        if not _next or _vs == 0:
-            return packaging.version.parse(self.data().get("version", "v0.0.1"))
+        _vs = VerPackage.parse(self.data().get("version", "v0.0.1"))
+        if not _next or self.changed == 0:
+            return _vs
         elif self.changed >= 3:
-            return packaging.version.parse(f"v{str(_vs.major + 1)}.0.0")
+            return _vs.bump_major()
         elif self.changed == 2:
-            return packaging.version.parse(
-                f"v{_vs.major}.{str(_vs.minor + 1)}.0"
-            )
-        return packaging.version.parse(
-            f"v{_vs.major}.{_vs.minor}.{str(_vs.micro + 1)}"
-        )
+            return _vs.bump_minor()
+        return _vs.bump_patch()
 
     def fmt(self, update: Optional[Dict[str, Any]] = None):
         return self.fmt_group(
             {
                 "timestamp": self.timestamp,
                 "version": self.version(),
                 **(update or {}),
```

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/tracking.py` & `ddeutil_io-0.1.0/src/ddeutil/io/tracking.py`

 * *Files identical despite different names*

### Comparing `ddeutil-io-0.0.3/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.0/src/ddeutil/io/utils.py`

 * *Files identical despite different names*

