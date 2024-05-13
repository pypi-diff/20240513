# Comparing `tmp/fastapi_file_router-0.1.0.tar.gz` & `tmp/fastapi_file_router-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_file_router-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_file_router-0.1.1.tar", max compression
```

## Comparing `fastapi_file_router-0.1.0.tar` & `fastapi_file_router-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.0/README.md
--rw-r--r--   0        0        0     2423 2024-05-12 19:40:56.699994 fastapi_file_router-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.0/router/__init__.py
--rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.0/router/router.py
--rw-r--r--   0        0        0        0 2024-05-12 19:24:33.998945 fastapi_file_router-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.1/README.md
+-rw-r--r--   0        0        0     2471 2024-05-13 04:29:22.310563 fastapi_file_router-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.1/router/__init__.py
+-rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.1/router/router.py
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:33.998945 fastapi_file_router-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.1/PKG-INFO
```

### Comparing `fastapi_file_router-0.1.0/pyproject.toml` & `fastapi_file_router-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "fastapi-file-router"
-version = "0.1.0"
+version = "0.1.1"
 description = "File-based routing for FastAPI"
 authors = ["Bewinxed <bewinxed@gmail.com>"]
 license = "WhoCares"
 readme = "README.md"
 packages = [
     { include = "router", from = "." },
     { include = "tests", from = "." },
+    { include = "router/router.py", from = "."}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.12"
+python = "^3.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
```

### Comparing `fastapi_file_router-0.1.0/router/router.py` & `fastapi_file_router-0.1.1/router/router.py`

 * *Files identical despite different names*

