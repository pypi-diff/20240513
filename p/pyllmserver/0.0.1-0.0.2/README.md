# Comparing `tmp/pyllmserver-0.0.1.tar.gz` & `tmp/pyllmserver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllmserver-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyllmserver-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyllmserver-0.0.1.tar` & `pyllmserver-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1063 2024-05-12 14:02:19.081410 pyllmserver-0.0.1/LICENSE
--rw-r--r--   0        0        0       13 2024-05-12 14:03:49.208667 pyllmserver-0.0.1/README.md
--rw-r--r--   0        0        0       56 2024-05-12 14:03:36.256121 pyllmserver-0.0.1/llmserver/__init__.py
--rw-r--r--   0        0        0      810 2024-05-12 14:05:10.947489 pyllmserver-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      346 1970-01-01 00:00:00.000000 pyllmserver-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-12 14:02:19.081410 pyllmserver-0.0.2/LICENSE
+-rw-r--r--   0        0        0       13 2024-05-12 14:03:49.208667 pyllmserver-0.0.2/README.md
+-rw-r--r--   0        0        0       56 2024-05-13 00:26:18.135278 pyllmserver-0.0.2/llmserver/__init__.py
+-rw-r--r--   0        0        0      705 2024-05-13 00:25:44.398766 pyllmserver-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 pyllmserver-0.0.2/PKG-INFO
```

### Comparing `pyllmserver-0.0.1/LICENSE` & `pyllmserver-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllmserver-0.0.1/pyproject.toml` & `pyllmserver-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -8,20 +8,14 @@
 readme = "README.md"
 requires-python = ">=3.12"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = []
 
-[project.optional-dependencies]
-dev = []
-
-[project.urls]
-Home = "https://github.com/yansh97/llm-server"
-
 [tool.flit.module]
 name = "llmserver"
 
 [tool.coverage.report]
 exclude_also = ["@abstractmethod", "raise", "except"]
 
 [tool.pytest.ini_options]
```

