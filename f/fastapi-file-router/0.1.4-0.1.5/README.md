# Comparing `tmp/fastapi_file_router-0.1.4.tar.gz` & `tmp/fastapi_file_router-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_file_router-0.1.4.tar", max compression
+gzip compressed data, was "fastapi_file_router-0.1.5.tar", max compression
```

## Comparing `fastapi_file_router-0.1.4.tar` & `fastapi_file_router-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.4/README.md
--rw-r--r--   0        0        0     2427 2024-05-13 04:48:30.717782 fastapi_file_router-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.4/src/router/__init__.py
--rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.4/src/router/router.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-12 19:24:46.691424 fastapi_file_router-0.1.5/README.md
+-rw-r--r--   0        0        0     2422 2024-05-13 04:51:56.441516 fastapi_file_router-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-12 19:23:28.924492 fastapi_file_router-0.1.5/src/fastapi-file-router/router/__init__.py
+-rw-r--r--   0        0        0     3410 2024-05-12 19:30:34.476536 fastapi_file_router-0.1.5/src/fastapi-file-router/router/router.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 fastapi_file_router-0.1.5/PKG-INFO
```

### Comparing `fastapi_file_router-0.1.4/pyproject.toml` & `fastapi_file_router-0.1.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "fastapi-file-router"
-version = "0.1.4"
+version = "0.1.5"
 description = "File-based routing for FastAPI"
 authors = ["Bewinxed <bewinxed@gmail.com>"]
 license = "WhoCares"
 readme = "README.md"
 packages = [
     # include the router in src
-    { include = "src/router" },
+    { include = "src/*" },
 
 ]
 package-mode=true
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `fastapi_file_router-0.1.4/src/router/router.py` & `fastapi_file_router-0.1.5/src/fastapi-file-router/router/router.py`

 * *Files identical despite different names*

