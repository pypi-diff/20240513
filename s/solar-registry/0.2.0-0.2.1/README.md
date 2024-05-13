# Comparing `tmp/solar_registry-0.2.0.tar.gz` & `tmp/solar_registry-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.0.tar", last modified: Mon May 13 03:40:13 2024, max compression
+gzip compressed data, was "solar_registry-0.2.1.tar", last modified: Mon May 13 06:24:35 2024, max compression
```

## Comparing `solar_registry-0.2.0.tar` & `solar_registry-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-05-13 03:39:53.074143 solar_registry-0.2.0/LICENSE
--rw-r--r--   0        0        0      682 2024-05-13 03:39:53.074143 solar_registry-0.2.0/README.md
--rw-r--r--   0        0        0      835 2024-05-13 03:40:13.958150 solar_registry-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     1418 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4789 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2051 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-13 03:39:53.074143 solar_registry-0.2.0/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-13 03:39:53.074143 solar_registry-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      680 2024-05-13 03:39:53.074143 solar_registry-0.2.0/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-13 03:39:53.074143 solar_registry-0.2.0/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-13 03:39:53.074143 solar_registry-0.2.0/tests/test_testtool.py
--rw-r--r--   0        0        0      731 2024-05-13 03:39:53.074143 solar_registry-0.2.0/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-13 03:39:53.078143 solar_registry-0.2.0/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2820 2024-05-13 03:39:53.078143 solar_registry-0.2.0/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 solar_registry-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 06:24:10.323039 solar_registry-0.2.1/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-13 06:24:10.323039 solar_registry-0.2.1/README.md
+-rw-r--r--   0        0        0     1182 2024-05-13 06:24:35.175118 solar_registry-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     1418 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4789 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2051 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     2517 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-13 06:24:10.327039 solar_registry-0.2.1/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      680 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/test_testtool.py
+-rw-r--r--   0        0        0      731 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2820 2024-05-13 06:24:10.327039 solar_registry-0.2.1/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     1462 1970-01-01 00:00:00.000000 solar_registry-0.2.1/PKG-INFO
```

### Comparing `solar_registry-0.2.0/LICENSE` & `solar_registry-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/README.md` & `solar_registry-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/cli.py` & `solar_registry-0.2.1/src/solar_registry/cli.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.1/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.1/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/service/generator.py` & `solar_registry-0.2.1/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.1/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/src/solar_registry/util/file.py` & `solar_registry-0.2.1/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/tests/test_merger.py` & `solar_registry-0.2.1/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/tests/test_testtool.py` & `solar_registry-0.2.1/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.1/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.1/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.0/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.1/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

