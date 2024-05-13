# Comparing `tmp/stac_model-0.1.3a1.tar.gz` & `tmp/stac_model-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_model-0.1.3a1.tar", max compression
+gzip compressed data, was "stac_model-0.1.4.tar", max compression
```

## Comparing `stac_model-0.1.3a1.tar` & `stac_model-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-01 23:25:28.057036 stac_model-0.1.3a1/LICENSE
--rw-r--r--   0        0        0    56030 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/README.md
--rw-r--r--   0        0        0     7476 2024-05-02 20:48:44.991630 stac_model-0.1.3a1/pyproject.toml
--rw-r--r--   0        0        0      265 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/__init__.py
--rw-r--r--   0        0        0     1215 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/__main__.py
--rw-r--r--   0        0        0     3035 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/base.py
--rw-r--r--   0        0        0     7036 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/examples.py
--rw-r--r--   0        0        0     2026 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/input.py
--rw-r--r--   0        0        0     3007 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/output.py
--rw-r--r--   0        0        0     1476 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/runtime.py
--rw-r--r--   0        0        0     9408 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/schema.py
--rw-r--r--   0        0        0    57733 1970-01-01 00:00:00.000000 stac_model-0.1.3a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 16:59:06.677350 stac_model-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3688 2024-05-13 16:59:06.677350 stac_model-0.1.4/README_STAC_MODEL.md
+-rw-r--r--   0        0        0     8013 2024-05-13 16:59:06.677350 stac_model-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/__init__.py
+-rw-r--r--   0        0        0     1215 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/__main__.py
+-rw-r--r--   0        0        0     3035 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/base.py
+-rw-r--r--   0        0        0     7036 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/examples.py
+-rw-r--r--   0        0        0     2026 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/input.py
+-rw-r--r--   0        0        0     3007 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/output.py
+-rw-r--r--   0        0        0     1476 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/runtime.py
+-rw-r--r--   0        0        0     9408 2024-05-13 16:59:06.677350 stac_model-0.1.4/stac_model/schema.py
+-rw-r--r--   0        0        0     5481 1970-01-01 00:00:00.000000 stac_model-0.1.4/PKG-INFO
```

### Comparing `stac_model-0.1.3a1/LICENSE` & `stac_model-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/pyproject.toml` & `stac_model-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,44 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "stac-model"
-version = "0.1.3-alpha.1"
+version = "0.1.4"
 description = "A PydanticV2 validation and serialization libary for the STAC ML Model Extension"
-readme = "README.md"
-authors = ["Ryan Avery <ryan@wherobots.com>"]
+readme = "README_STAC_MODEL.md"
+authors = [
+  "Ryan Avery <ryan@wherobots.com>",
+  "Francis Charette-Migneault <francis.charette-migneault@crim.ca>"
+]
 license = "Apache Software License 2.0"
-repository = "https://github.com/rbavery/stac-model"
-homepage = "https://github.com/rbavery/stac-model"
+repository = "https://github.com/crim-ca/mlm-extension"
+homepage = "https://github.com/crim-ca/mlm-extension/blob/main/README_STAC_MODEL.md"
 packages = [
   {include = "stac_model"}
 ]
 
 
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
 keywords = []  # UPDATEME with relevant keywords
 
 
 # Pypi classifiers: https://pypi.org/classifiers/
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 4 - Beta",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3 :: Only",
   "Framework :: Pydantic",
   "Framework :: Pydantic :: 2",
   "Intended Audience :: Developers",
   "Intended Audience :: Information Technology",
   "Intended Audience :: Science/Research",
   "Topic :: File Formats :: JSON :: JSON Schema",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
@@ -81,14 +86,19 @@
 pytest-click = "^1.1.0"
 pytest-pikachu = "^1.0.0"
 coverage = "^7.3.0"
 ruff = "^0.2.2"
 bump-my-version = "^0.21"
 
 [tool.bumpversion]
+# NOTE:
+#   Although these definitions are provided in this 'stac-model' project file,
+#   they are actually intented for versioning the MLM specification itself.
+#   To version 'stac-model', use the 'poetry version' operations.
+#   See also https://github.com/crim-ca/mlm-extension/blob/main/CONTRIBUTING.md#building-and-releasing
 current_version = "1.1.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = true
```

### Comparing `stac_model-0.1.3a1/stac_model/__main__.py` & `stac_model-0.1.4/stac_model/__main__.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/base.py` & `stac_model-0.1.4/stac_model/base.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/examples.py` & `stac_model-0.1.4/stac_model/examples.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/input.py` & `stac_model-0.1.4/stac_model/input.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/output.py` & `stac_model-0.1.4/stac_model/output.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/runtime.py` & `stac_model-0.1.4/stac_model/runtime.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.3a1/stac_model/schema.py` & `stac_model-0.1.4/stac_model/schema.py`

 * *Files identical despite different names*

