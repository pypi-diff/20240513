# Comparing `tmp/pytest_aws_apigateway-0.1.0.tar.gz` & `tmp/pytest_aws_apigateway-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_aws_apigateway-0.1.0.tar", last modified: Fri May 10 14:19:09 2024, max compression
+gzip compressed data, was "pytest_aws_apigateway-0.2.0.tar", last modified: Mon May 13 08:48:43 2024, max compression
```

## Comparing `pytest_aws_apigateway-0.1.0.tar` & `pytest_aws_apigateway-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.046190 pytest_aws_apigateway-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.046190 pytest_aws_apigateway-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.046190 pytest_aws_apigateway-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.046190 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-10 14:19:09.000000 pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tasks/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 14:19:09.050190 pytest_aws_apigateway-0.1.0/tests/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tests/examples/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-10 14:18:59.000000 pytest_aws_apigateway-0.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.128115 pytest_aws_apigateway-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.120115 pytest_aws_apigateway-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/changes/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/changes/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:48:43.128115 pytest_aws_apigateway-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.120115 pytest_aws_apigateway-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 08:48:43.000000 pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tasks/release.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:48:43.124115 pytest_aws_apigateway-0.2.0/tests/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/examples/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-13 08:48:36.000000 pytest_aws_apigateway-0.2.0/tox.ini
```

### Comparing `pytest_aws_apigateway-0.1.0/.github/workflows/main.yml` & `pytest_aws_apigateway-0.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.1.0/LICENSE` & `pytest_aws_apigateway-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.1.0/PKG-INFO` & `pytest_aws_apigateway-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.1.0
+Version: 0.2.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.1.0/README.md` & `pytest_aws_apigateway-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.1.0/pyproject.toml` & `pytest_aws_apigateway-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway/apigateway.py` & `pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway/apigateway.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,32 +1,58 @@
+import json
+import re
 from typing import Callable
+from typing import Union
+
 import httpx
 import pytest_httpx
-import re
 
-from pytest_aws_apigateway.event import request_to_event, transform_response
+from pytest_aws_apigateway.context import LambdaContext, create_context
+from pytest_aws_apigateway.event import OutputFormatError
+from pytest_aws_apigateway.event import request_to_event
+from pytest_aws_apigateway.event import transform_response
+
+__all__ = ["ApiGateway"]
 
 
 class ApiGateway:
     def __init__(self, httpx_mock: pytest_httpx.HTTPXMock):
         self.httpx_mock = httpx_mock
         ...
 
     def add_integration(
-        self, resource: str, method: str, handler: Callable, endpoint: str
+        self,
+        resource: str,
+        method: str,
+        endpoint: str,
+        handler: Callable[[dict, LambdaContext], Union[dict, httpx.Response]],
     ):
-        p = re.compile(r"\{([^\/]+)\}")
-        res = re.subn(p, r"([^\/]+)", resource)
-        if res[1] > 0:
-            newp = re.compile(f"{endpoint}/{res[0]}")
-        else:
-            newp = endpoint
+        resource = self._normalize_resource(resource)
 
-        resource = resource.lstrip("/")
-        resource = f"/{resource}"
+        url = self._url_expression(endpoint, resource)
 
         def integration(request: httpx.Request) -> httpx.Response:
             event = request_to_event(request, resource)
-            resp = handler(event, None)
-            return transform_response(resp)
+            context = create_context(handler)
+            resp = handler(event, context)
+            try:
+                return transform_response(resp)
+            except OutputFormatError:
+                return httpx.Response(
+                    status_code=500,
+                    json=json.dumps({"message": "Internal server error"}),
+                )
+
+        self.httpx_mock.add_callback(callback=integration, url=url, method=method)
+
+    def _normalize_resource(self, resource: str) -> str:
+        resource = resource.lstrip("/")
+        resource = f"/{resource}"
+        return resource
 
-        self.httpx_mock.add_callback(callback=integration, url=newp, method=method)
+    def _url_expression(self, endpoint: str, resource: str) -> Union[re.Pattern, str]:
+        p = re.compile(r"\{([^\/]+)\}")
+        res = re.subn(p, r"([^\/]+)", resource)
+        if res[1] > 0:
+            return re.compile(f"{endpoint}/{res[0]}")
+        else:
+            return endpoint
```

### Comparing `pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/PKG-INFO` & `pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-aws-apigateway
-Version: 0.1.0
+Version: 0.2.0
 Summary: pytest plugin for AWS ApiGateway
 Author-email: Felix Scherz <felixwscherz@gmail.com>
 License: MIT License
         
         Copyright (c) 2024-present Felix Scherz <felixwscherz@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytest_aws_apigateway-0.1.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt` & `pytest_aws_apigateway-0.2.0/src/pytest_aws_apigateway.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 requirements-dev.txt
 tox.ini
 .github/workflows/main.yml
+changes/.gitignore
 src/pytest_aws_apigateway/__init__.py
 src/pytest_aws_apigateway/apigateway.py
+src/pytest_aws_apigateway/context.py
 src/pytest_aws_apigateway/event.py
 src/pytest_aws_apigateway/plugin.py
 src/pytest_aws_apigateway.egg-info/PKG-INFO
 src/pytest_aws_apigateway.egg-info/SOURCES.txt
 src/pytest_aws_apigateway.egg-info/dependency_links.txt
 src/pytest_aws_apigateway.egg-info/entry_points.txt
 src/pytest_aws_apigateway.egg-info/requires.txt
 src/pytest_aws_apigateway.egg-info/top_level.txt
 tasks/release.py
 tests/__init__.py
 tests/conftest.py
 tests/test_event.py
 tests/test_plugin.py
+tests/test_response.py
 tests/examples/test_handler.py
```

### Comparing `pytest_aws_apigateway-0.1.0/tasks/release.py` & `pytest_aws_apigateway-0.2.0/tasks/release.py`

 * *Files identical despite different names*

### Comparing `pytest_aws_apigateway-0.1.0/tests/test_event.py` & `pytest_aws_apigateway-0.2.0/tests/test_event.py`

 * *Files identical despite different names*

