# Comparing `tmp/fastapi_problem-0.7.3.tar.gz` & `tmp/fastapi_problem-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_problem-0.7.3.tar", max compression
+gzip compressed data, was "fastapi_problem-0.7.4.tar", max compression
```

## Comparing `fastapi_problem-0.7.3.tar` & `fastapi_problem-0.7.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11307 2024-05-13 06:57:54.209846 fastapi_problem-0.7.3/LICENSE
--rw-r--r--   0        0        0     1905 2024-05-13 06:57:54.209846 fastapi_problem-0.7.3/README.md
--rw-r--r--   0        0        0     2228 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/__init__.py
--rw-r--r--   0        0        0      220 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/cors.py
--rw-r--r--   0        0        0     3407 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/error.py
--rw-r--r--   0        0        0        0 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/handler/__init__.py
--rw-r--r--   0        0        0     5955 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/handler/base.py
--rw-r--r--   0        0        0     3094 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/handler/fastapi.py
--rw-r--r--   0        0        0     2225 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/handler/starlette.py
--rw-r--r--   0        0        0      297 2024-05-13 06:57:54.213846 fastapi_problem-0.7.3/src/fastapi_problem/handler/util.py
--rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 fastapi_problem-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/LICENSE
+-rw-r--r--   0        0        0     1905 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/README.md
+-rw-r--r--   0        0        0     2228 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/cors.py
+-rw-r--r--   0        0        0     3407 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/error.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/handler/__init__.py
+-rw-r--r--   0        0        0     5955 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/handler/base.py
+-rw-r--r--   0        0        0     3094 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/handler/fastapi.py
+-rw-r--r--   0        0        0     2225 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/handler/starlette.py
+-rw-r--r--   0        0        0      297 2024-05-13 07:18:59.621401 fastapi_problem-0.7.4/src/fastapi_problem/handler/util.py
+-rw-r--r--   0        0        0     2602 1970-01-01 00:00:00.000000 fastapi_problem-0.7.4/PKG-INFO
```

### Comparing `fastapi_problem-0.7.3/LICENSE` & `fastapi_problem-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.3/README.md` & `fastapi_problem-0.7.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# FastAPI Problems v0.7.3
+# FastAPI Problems v0.7.4
 [![image](https://img.shields.io/pypi/v/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/l/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/pyversions/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 ![style](https://github.com/NRWLDev/fastapi-problem/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/fastapi-problem/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/fastapi-problem/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/fastapi-problem)
```

### Comparing `fastapi_problem-0.7.3/pyproject.toml` & `fastapi_problem-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-problem"
-version = "0.7.3"
+version = "0.7.4"
 description = "FastAPI support for RFC9457 problems."
 authors = ["Daniel Edgecombe <edgy.edgemond@gmail.com>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/fastapi-problem/"
 homepage="https://github.com/NRWLDev/fastapi-problem/"
 readme = "README.md"
 
@@ -23,15 +23,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3.0"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.7.3"
+current_version = "0.7.4"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "README.md"
 
 [[tool.bumpversion.files]]
```

### Comparing `fastapi_problem-0.7.3/src/fastapi_problem/error.py` & `fastapi_problem-0.7.4/src/fastapi_problem/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         **kwargs,
     ) -> None:
         warn(
             "HttpException use is deprecated, use `Problem` subclasses instead.",
             FutureWarning,
             stacklevel=2,
         )
-        super().__init__(title, core=code, details=details, status=status, **kwargs)
+        super().__init__(title, code=code, details=details, status=status, **kwargs)
 
 
 class StatusProblem(Problem):
     code = None
     title = "Base http exception."
     status = 500
```

### Comparing `fastapi_problem-0.7.3/src/fastapi_problem/handler/base.py` & `fastapi_problem-0.7.4/src/fastapi_problem/handler/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.3/src/fastapi_problem/handler/fastapi.py` & `fastapi_problem-0.7.4/src/fastapi_problem/handler/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.3/src/fastapi_problem/handler/starlette.py` & `fastapi_problem-0.7.4/src/fastapi_problem/handler/starlette.py`

 * *Files identical despite different names*

### Comparing `fastapi_problem-0.7.3/PKG-INFO` & `fastapi_problem-0.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-problem
-Version: 0.7.3
+Version: 0.7.4
 Summary: FastAPI support for RFC9457 problems.
 Home-page: https://github.com/NRWLDev/fastapi-problem/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: edgy.edgemond@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/NRWLDev/fastapi-problem/
 Description-Content-Type: text/markdown
 
-# FastAPI Problems v0.7.3
+# FastAPI Problems v0.7.4
 [![image](https://img.shields.io/pypi/v/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/l/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 [![image](https://img.shields.io/pypi/pyversions/fastapi_problem.svg)](https://pypi.org/project/fastapi-problem/)
 ![style](https://github.com/NRWLDev/fastapi-problem/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/fastapi-problem/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/fastapi-problem/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/fastapi-problem)
```

