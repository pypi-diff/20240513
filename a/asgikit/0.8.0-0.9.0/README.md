# Comparing `tmp/asgikit-0.8.0.tar.gz` & `tmp/asgikit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgikit-0.8.0.tar", max compression
+gzip compressed data, was "asgikit-0.9.0.tar", max compression
```

## Comparing `asgikit-0.8.0.tar` & `asgikit-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2024-04-17 20:43:08.455555 asgikit-0.8.0/LICENSE
--rw-r--r--   0        0        0     2361 2024-04-17 20:43:08.455555 asgikit-0.8.0/README.md
--rw-r--r--   0        0        0     1853 2024-04-17 20:43:23.015546 asgikit-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      131 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/__init__.py
--rw-r--r--   0        0        0      426 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/asgi.py
--rw-r--r--   0        0        0      484 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/constants.py
--rw-r--r--   0        0        0        0 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/errors/__init__.py
--rw-r--r--   0        0        0       37 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/errors/asgi.py
--rw-r--r--   0        0        0      132 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/errors/http.py
--rw-r--r--   0        0        0      398 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/errors/websocket.py
--rw-r--r--   0        0        0     2622 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/headers.py
--rw-r--r--   0        0        0        0 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/py.typed
--rw-r--r--   0        0        0     1139 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/query.py
--rw-r--r--   0        0        0     7694 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/requests.py
--rw-r--r--   0        0        0    10593 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/responses.py
--rw-r--r--   0        0        0        0 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/util/__init__.py
--rw-r--r--   0        0        0     1252 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/util/async_file.py
--rw-r--r--   0        0        0      523 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/util/callable_proxy.py
--rw-r--r--   0        0        0     1817 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/util/multi_value_dict.py
--rw-r--r--   0        0        0     2978 2024-04-17 20:43:08.455555 asgikit-0.8.0/src/asgikit/websockets.py
--rw-r--r--   0        0        0     3436 1970-01-01 00:00:00.000000 asgikit-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 18:03:02.772483 asgikit-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2816 2024-05-13 18:03:02.776483 asgikit-0.9.0/README.md
+-rw-r--r--   0        0        0     1906 2024-05-13 18:03:15.292514 asgikit-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      119 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/_json.py
+-rw-r--r--   0        0        0      426 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/asgi.py
+-rw-r--r--   0        0        0      484 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/constants.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/errors/__init__.py
+-rw-r--r--   0        0        0       37 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/errors/asgi.py
+-rw-r--r--   0        0        0      132 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/errors/http.py
+-rw-r--r--   0        0        0      398 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/errors/websocket.py
+-rw-r--r--   0        0        0     2622 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/headers.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/py.typed
+-rw-r--r--   0        0        0     1139 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/query.py
+-rw-r--r--   0        0        0     7723 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/requests.py
+-rw-r--r--   0        0        0    10701 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/responses.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/util/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/util/async_file.py
+-rw-r--r--   0        0        0      523 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/util/callable_proxy.py
+-rw-r--r--   0        0        0     1817 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/util/multi_value_dict.py
+-rw-r--r--   0        0        0     2978 2024-05-13 18:03:02.776483 asgikit-0.9.0/src/asgikit/websockets.py
+-rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 asgikit-0.9.0/PKG-INFO
```

### Comparing `asgikit-0.8.0/LICENSE` & `asgikit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/README.md` & `asgikit-0.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,27 @@
 to read form data from the request and write json to the response.
 
 This strategy allows for simpler extensibility. For example, to parse json from the request
 using an alternative json parser, you just need to write a function that reads the request.
 Similarly, to write another data format into the response, you just write a function that
 writes to the response.
 
+## Custom JSON encoder and decoder
+
+By default, asgikit uses `json.dumps` and `json.loads` for dealing with JSON. If
+you want to use other libraries like `orjson`, just define the environment variable
+`ASGIKIT_JSON_ENCODER` of the module compatible with `json`, or the full path to
+the functions that perform encoding and decoding, in that order:
+
+```dotenv
+ASGIKIT_JSON_ENCODER=orjson
+# or
+ASGIKIT_JSON_ENCODER=msgspc.json.encode,msgspc.json.encode
+```
+
 ## Example request and response
 
 ```python
 from asgikit.requests import Request, read_json
 from asgikit.responses import respond_json
```

### Comparing `asgikit-0.8.0/pyproject.toml` & `asgikit-0.9.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "asgikit"
-version = "0.8.0"
+version = "0.9.0"
 description = "Toolkit for building ASGI applications and libraries"
 authors = ["Livio Ribeiro <livioribeiro@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/livioribeiro/asgikit"
 keywords = ["asgi", "toolkit", "asyncio", "web"]
 classifiers = [
@@ -36,31 +36,34 @@
 aiofiles = "^23.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 uvicorn = { version = "^0.29", extras = ["standard"] }
+granian = "^1.3"
 pylint = "^3.1"
 flake8 = "^7.0"
-mypy = "^1.9"
+mypy = "^1.10"
 isort = "^5.13"
-black = "^24.3"
-ruff = "^0.3"
+black = "^24.4"
+ruff = "^0.4"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^8.1"
+pytest = "^8.2"
 pytest-asyncio = "^0.23"
 pytest-cov = "^5.0"
-coverage = { version = "^7.4", extras = ["toml"] }
+coverage = { version = "^7.5", extras = ["toml"] }
 httpx = "^0.27"
 asgiref = "^3.8"
+orjson = "^3.10"
+msgspec = "^0.18"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
```

### Comparing `asgikit-0.8.0/src/asgikit/headers.py` & `asgikit-0.9.0/src/asgikit/headers.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/src/asgikit/query.py` & `asgikit-0.9.0/src/asgikit/query.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/src/asgikit/requests.py` & `asgikit-0.9.0/src/asgikit/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import asyncio
-import json
 import re
 from collections.abc import AsyncIterable, Awaitable, Callable
 from http import HTTPMethod
 from http.cookies import SimpleCookie
 from typing import Any
 from urllib.parse import parse_qs, unquote_plus
 
 from multipart import multipart
 
+from asgikit._json import JSON_DECODER
 from asgikit.asgi import AsgiProtocol, AsgiReceive, AsgiScope, AsgiSend
 from asgikit.constants import (
     SCOPE_ASGIKIT,
     SCOPE_REQUEST,
     SCOPE_REQUEST_ATTRIBUTES,
     SCOPE_REQUEST_IS_CONSUMED,
 )
@@ -229,15 +229,15 @@
 
 
 async def read_json(request: Request) -> dict | list:
     body = await read_body(request)
     if not body:
         return {}
 
-    return json.loads(body)
+    return JSON_DECODER(body)
 
 
 def _is_form_multipart(content_type: str) -> bool:
     return content_type.startswith(FORM_MULTIPART_CONTENT_TYPE)
 
 
 async def read_form(request: Request) -> dict[str, str | multipart.File]:
```

### Comparing `asgikit-0.8.0/src/asgikit/responses.py` & `asgikit-0.9.0/src/asgikit/responses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
-import json
 import mimetypes
 import os
 from collections.abc import AsyncIterable
 from contextlib import asynccontextmanager
 from email.utils import formatdate
 from enum import StrEnum
 from http import HTTPStatus
 from http.cookies import SimpleCookie
 from os import PathLike
 from typing import Any
 
 import aiofiles
 import aiofiles.os
 
+from asgikit._json import JSON_ENCODER
 from asgikit.asgi import AsgiProtocol, AsgiReceive, AsgiScope, AsgiSend
 from asgikit.constants import (
     SCOPE_ASGIKIT,
     SCOPE_RESPONSE,
     SCOPE_RESPONSE_CONTENT_LENGTH,
     SCOPE_RESPONSE_CONTENT_TYPE,
     SCOPE_RESPONSE_COOKIES,
@@ -54,14 +54,18 @@
     ENCODING = "utf-8"
 
     __slots__ = ("asgi",)
 
     def __init__(self, scope: AsgiScope, receive: AsgiReceive, send: AsgiSend):
         scope.setdefault(SCOPE_ASGIKIT, {})
         scope[SCOPE_ASGIKIT].setdefault(SCOPE_RESPONSE, {})
+
+        scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].setdefault(
+            SCOPE_RESPONSE_STATUS, HTTPStatus.OK
+        )
         scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].setdefault(
             SCOPE_RESPONSE_HEADERS, MutableHeaders()
         )
         scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].setdefault(
             SCOPE_RESPONSE_COOKIES, SimpleCookie()
         )
         scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].setdefault(
@@ -73,14 +77,22 @@
         scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].setdefault(
             SCOPE_RESPONSE_IS_FINISHED, False
         )
 
         self.asgi = AsgiProtocol(scope, receive, send)
 
     @property
+    def status(self) -> HTTPStatus | None:
+        return self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][SCOPE_RESPONSE_STATUS]
+
+    @status.setter
+    def status(self, status: HTTPStatus):
+        self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][SCOPE_RESPONSE_STATUS] = status
+
+    @property
     def headers(self) -> MutableHeaders:
         return self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][SCOPE_RESPONSE_HEADERS]
 
     @property
     def cookies(self) -> SimpleCookie:
         return self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][SCOPE_RESPONSE_COOKIES]
 
@@ -130,21 +142,14 @@
         ]
 
     def __set_finished(self):
         self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][
             SCOPE_RESPONSE_IS_FINISHED
         ] = True
 
-    @property
-    def status(self) -> HTTPStatus | None:
-        return self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE].get(SCOPE_RESPONSE_STATUS)
-
-    def __set_status(self, status: HTTPStatus):
-        self.asgi.scope[SCOPE_ASGIKIT][SCOPE_RESPONSE][SCOPE_RESPONSE_STATUS] = status
-
     def header(self, name: str, value: str):
         self.headers.set(name, value)
 
     def cookie(
         self,
         name: str,
         value: str,
@@ -180,25 +185,26 @@
             self.header("content-type", content_type)
 
         if self.content_length is not None:
             self.header("content-length", str(self.content_length))
 
         return self.headers.encode()
 
-    async def start(self, status=HTTPStatus.OK):
+    async def start(self):
         if self.is_started:
             raise RuntimeError("response has already started")
 
         if self.is_finished:
             raise RuntimeError("response has already ended")
 
         self.__set_started()
-        self.__set_status(status)
 
+        status = self.status
         headers = self.__build_headers()
+
         await self.asgi.send(
             {
                 "type": "http.response.start",
                 "status": status,
                 "headers": headers,
             }
         )
@@ -226,29 +232,32 @@
 
         if self.is_finished:
             raise RuntimeError("response is already finished")
 
         await self.write(b"", more_body=False)
 
 
-async def respond_text(
-    response: Response, content: str | bytes, *, status: HTTPStatus = HTTPStatus.OK
-):
-    data = content.encode(response.encoding) if isinstance(content, str) else content
+async def respond_text(response: Response, content: str | bytes):
+    if isinstance(content, str):
+        data = content.encode(response.encoding)
+    else:
+        data = content
+
     if not response.content_type:
         response.content_type = "text/plain"
 
     response.content_length = len(data)
 
-    await response.start(status)
+    await response.start()
     await response.write(data, more_body=False)
 
 
 async def respond_status(response: Response, status: HTTPStatus):
-    await response.start(status)
+    response.status = status
+    await response.start()
     await response.end()
 
 
 async def respond_redirect(response: Response, location: str, permanent: bool = False):
     status = (
         HTTPStatus.TEMPORARY_REDIRECT
         if not permanent
@@ -260,33 +269,34 @@
 
 
 async def respond_redirect_post_get(response: Response, location: str):
     response.header("location", location)
     await respond_status(response, HTTPStatus.SEE_OTHER)
 
 
-async def respond_json(response: Response, content: Any, status=HTTPStatus.OK):
-    data = json.dumps(content).encode(response.encoding)
+async def respond_json(response: Response, content: Any):
+    data = JSON_ENCODER(content)
+    if isinstance(data, str):
+        data = data.encode(response.encoding)
 
     response.content_type = "application/json"
-    response.content_length = len(data)
-
-    await response.start(status)
-    await response.write(data, more_body=False)
+    await respond_text(response, data)
 
 
 async def __listen_for_disconnect(receive):
     while True:
         message = await receive()
         if message["type"] == "http.disconnect":
             return
 
 
 @asynccontextmanager
 async def stream_writer(response: Response):
+    await response.start()
+
     client_disconect = asyncio.create_task(
         __listen_for_disconnect(response.asgi.receive)
     )
 
     async def write(data: bytes | str):
         if client_disconect.done():
             raise ClientDisconnectError()
@@ -295,19 +305,15 @@
     try:
         yield write
     finally:
         await response.end()
         client_disconect.cancel()
 
 
-async def respond_stream(
-    response: Response, stream: AsyncIterable[bytes | str], *, status=HTTPStatus.OK
-):
-    await response.start(status)
-
+async def respond_stream(response: Response, stream: AsyncIterable[bytes | str]):
     async with stream_writer(response) as write:
         async for chunk in stream:
             await write(chunk)
 
 
 def __file_last_modified(stat: os.stat_result) -> str:
     return formatdate(stat.st_mtime, usegmt=True)
@@ -322,41 +328,44 @@
     return "extensions" in scope and "http.response.pathsend" in scope["extensions"]
 
 
 def __supports_zerocopysend(scope):
     return "extensions" in scope and "http.response.zerocopysend" in scope["extensions"]
 
 
-async def respond_file(
-    response: Response, path: str | PathLike[str], status=HTTPStatus.OK
-):
+async def respond_file(response: Response, path: str | PathLike[str]):
     if not response.content_type:
         response.content_type = __guess_mimetype(path)
 
-    stat = await asyncio.to_thread(os.stat, path)
+    stat = await aiofiles.os.stat(path)
     content_length = stat.st_size
     last_modified = __file_last_modified(stat)
 
     response.content_length = content_length
     response.headers.set("last-modified", last_modified)
 
+    if not isinstance(path, str):
+        path = str(path)
+
     if __supports_pathsend(response.asgi.scope):
+        await response.start()
         await response.asgi.send(
             {
                 "type": "http.response.pathsend",
                 "path": path,
             }
         )
         return
 
     if __supports_zerocopysend(response.asgi.scope):
+        await response.start()
         file = await asyncio.to_thread(open, path, "rb")
         await response.asgi.send(
             {
                 "type": "http.response.zerocopysend",
                 "file": file.fileno(),
             }
         )
         return
 
     async with aiofiles.open(path, "rb") as stream:
-        await respond_stream(response, stream, status=status)
+        await respond_stream(response, stream)
```

### Comparing `asgikit-0.8.0/src/asgikit/util/async_file.py` & `asgikit-0.9.0/src/asgikit/util/async_file.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/src/asgikit/util/callable_proxy.py` & `asgikit-0.9.0/src/asgikit/util/callable_proxy.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/src/asgikit/util/multi_value_dict.py` & `asgikit-0.9.0/src/asgikit/util/multi_value_dict.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/src/asgikit/websockets.py` & `asgikit-0.9.0/src/asgikit/websockets.py`

 * *Files identical despite different names*

### Comparing `asgikit-0.8.0/PKG-INFO` & `asgikit-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgikit
-Version: 0.8.0
+Version: 0.9.0
 Summary: Toolkit for building ASGI applications and libraries
 Home-page: https://github.com/livioribeiro/asgikit
 License: MIT
 Keywords: asgi,toolkit,asyncio,web
 Author: Livio Ribeiro
 Author-email: livioribeiro@outlook.com
 Requires-Python: >=3.11,<4.0
@@ -58,14 +58,27 @@
 to read form data from the request and write json to the response.
 
 This strategy allows for simpler extensibility. For example, to parse json from the request
 using an alternative json parser, you just need to write a function that reads the request.
 Similarly, to write another data format into the response, you just write a function that
 writes to the response.
 
+## Custom JSON encoder and decoder
+
+By default, asgikit uses `json.dumps` and `json.loads` for dealing with JSON. If
+you want to use other libraries like `orjson`, just define the environment variable
+`ASGIKIT_JSON_ENCODER` of the module compatible with `json`, or the full path to
+the functions that perform encoding and decoding, in that order:
+
+```dotenv
+ASGIKIT_JSON_ENCODER=orjson
+# or
+ASGIKIT_JSON_ENCODER=msgspc.json.encode,msgspc.json.encode
+```
+
 ## Example request and response
 
 ```python
 from asgikit.requests import Request, read_json
 from asgikit.responses import respond_json
```

