# Comparing `tmp/fastapi_file_router-0.1.6.tar.gz` & `tmp/fastapi_file_router-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_file_router-0.1.6.tar", max compression
+gzip compressed data, was "fastapi_file_router-0.1.7.tar", max compression
```

## Comparing `fastapi_file_router-0.1.6.tar` & `fastapi_file_router-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.6/README.md
--rw-r--r--   0        0        0     2452 2024-05-13 04:53:09.012244 fastapi_file_router-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.6/src/fastapi-file-router/router/__init__.py
--rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.6/src/fastapi-file-router/router/router.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.7/README.md
+-rw-r--r--   0        0        0     2452 2024-05-13 04:54:52.144352 fastapi_file_router-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.7/src/fastapi_file_router/router/__init__.py
+-rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.7/src/fastapi_file_router/router/router.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.7/PKG-INFO
```

### Comparing `fastapi_file_router-0.1.6/pyproject.toml` & `fastapi_file_router-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "fastapi-file-router"
-version = "0.1.6"
+version = "0.1.7"
 description = "File-based routing for FastAPI"
 authors = ["Bewinxed <bewinxed@gmail.com>"]
 license = "WhoCares"
 readme = "README.md"
 packages = [
     # include the router in src
-    { include = "fastapi-file-router", from = "./src" },
+    { include = "fastapi_file_router", from = "./src" },
 
 ]
 package-mode=true
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fastapi_file_router-0.1.6/src/fastapi-file-router/router/router.py` & `fastapi_file_router-0.1.7/src/fastapi_file_router/router/router.py`

 * *Files identical despite different names*

