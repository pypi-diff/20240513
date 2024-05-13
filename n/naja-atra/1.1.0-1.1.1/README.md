# Comparing `tmp/naja_atra-1.1.0.tar.gz` & `tmp/naja_atra-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naja_atra-1.1.0.tar", last modified: Sat May 11 09:58:35 2024, max compression
+gzip compressed data, was "naja_atra-1.1.1.tar", last modified: Mon May 13 03:11:49 2024, max compression
```

## Comparing `naja_atra-1.1.0.tar` & `naja_atra-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,38 @@
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.282536 naja_atra-1.1.0/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2023-01-29 02:07:01.000000 naja_atra-1.1.0/LICENSE
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-11 09:58:35.282536 naja_atra-1.1.0/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-04-02 02:23:04.000000 naja_atra-1.1.0/README.md
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.270536 naja_atra-1.1.0/naja_atra/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-05-11 09:57:23.000000 naja_atra-1.1.0/naja_atra/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-04-02 11:35:53.000000 naja_atra-1.1.0/naja_atra/__main__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-04-01 10:12:01.000000 naja_atra-1.1.0/naja_atra/app_conf.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.274536 naja_atra-1.1.0/naja_atra/http_servers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-04-16 12:02:34.000000 naja_atra-1.1.0/naja_atra/http_servers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-03-11 09:12:30.000000 naja_atra-1.1.0/naja_atra/http_servers/coroutine_http_server.py
--rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-03-12 01:27:45.000000 naja_atra-1.1.0/naja_atra/http_servers/http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-03-11 09:43:12.000000 naja_atra-1.1.0/naja_atra/http_servers/routing_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-03-11 09:15:29.000000 naja_atra-1.1.0/naja_atra/http_servers/threading_http_server.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    18456 2024-05-11 06:54:42.000000 naja_atra-1.1.0/naja_atra/models.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra/request_handlers/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:12:14.000000 naja_atra-1.1.0/naja_atra/request_handlers/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    30633 2024-05-11 09:50:45.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    17638 2024-05-11 09:07:29.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_request_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/http_session_local_impl.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    14419 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/model_bindings.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-03-11 09:39:40.000000 naja_atra-1.1.0/naja_atra/request_handlers/websocket_controller_handler.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-04-16 12:02:50.000000 naja_atra-1.1.0/naja_atra/server.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra/utils/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-03-07 02:23:26.000000 naja_atra-1.1.0/naja_atra/utils/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     7276 2024-05-11 09:46:24.000000 naja_atra-1.1.0/naja_atra/utils/http_utils.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-03-07 03:33:13.000000 naja_atra-1.1.0/naja_atra/utils/logger.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/naja_atra.egg-info/
--rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/PKG-INFO
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1077 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/SOURCES.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/dependency_links.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/requires.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-05-11 09:58:35.000000 naja_atra-1.1.0/naja_atra.egg-info/top_level.txt
--rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-03-08 09:12:59.000000 naja_atra-1.1.0/pyproject.toml
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-05-11 09:58:35.282536 naja_atra-1.1.0/setup.cfg
--rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2023-01-29 02:07:01.000000 naja_atra-1.1.0/setup.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/tests/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja_atra-1.1.0/tests/__init__.py
-drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-11 09:58:35.278536 naja_atra-1.1.0/tests/ctrls/
--rw-rw-r--   0 keijack   (1000) keijack   (1000)        0 2023-01-29 02:07:01.000000 naja_atra-1.1.0/tests/ctrls/__init__.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)    10132 2024-05-11 09:30:50.000000 naja_atra-1.1.0/tests/ctrls/my_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     1890 2024-03-11 08:58:23.000000 naja_atra-1.1.0/tests/ctrls/my_controllers_model_binding.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     3538 2024-03-07 03:14:28.000000 naja_atra-1.1.0/tests/ctrls/ws_controllers.py
--rw-rw-r--   0 keijack   (1000) keijack   (1000)     8064 2024-03-08 02:52:49.000000 naja_atra-1.1.0/tests/test_all_ctrls.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.047187 naja_atra-1.1.1/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1066 2024-05-11 10:09:28.000000 naja_atra-1.1.1/LICENSE
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-13 03:11:49.043189 naja_atra-1.1.1/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1031 2024-05-11 10:09:28.000000 naja_atra-1.1.1/README.md
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.031195 naja_atra-1.1.1/naja_atra/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1172 2024-05-13 03:05:33.000000 naja_atra-1.1.1/naja_atra/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     2049 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/__main__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    28716 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/app_conf.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.035193 naja_atra-1.1.1/naja_atra/http_servers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/http_servers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3740 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/http_servers/coroutine_http_server.py
+-rwxrwxr-x   0 keijack   (1000) keijack   (1000)     5587 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/http_servers/http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17237 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/http_servers/routing_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     3337 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/http_servers/threading_http_server.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    18476 2024-05-13 01:35:42.000000 naja_atra-1.1.1/naja_atra/models.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.035193 naja_atra-1.1.1/naja_atra/request_handlers/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/request_handlers/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    31289 2024-05-13 02:57:09.000000 naja_atra-1.1.1/naja_atra/request_handlers/http_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    17619 2024-05-13 02:49:16.000000 naja_atra-1.1.1/naja_atra/request_handlers/http_request_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     5914 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/request_handlers/http_session_local_impl.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    14392 2024-05-13 01:32:06.000000 naja_atra-1.1.1/naja_atra/request_handlers/model_bindings.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)    23851 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/request_handlers/websocket_controller_handler.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     8848 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/server.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.035193 naja_atra-1.1.1/naja_atra/utils/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     1087 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/utils/__init__.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     7276 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/utils/http_utils.py
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     6668 2024-05-11 10:09:28.000000 naja_atra-1.1.1/naja_atra/utils/logger.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.043189 naja_atra-1.1.1/naja_atra.egg-info/
+-rw-r--r--   0 keijack   (1000) keijack   (1000)     3012 2024-05-13 03:11:48.000000 naja_atra-1.1.1/naja_atra.egg-info/PKG-INFO
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      931 2024-05-13 03:11:49.000000 naja_atra-1.1.1/naja_atra.egg-info/SOURCES.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)        1 2024-05-13 03:11:49.000000 naja_atra-1.1.1/naja_atra.egg-info/dependency_links.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       56 2024-05-13 03:11:49.000000 naja_atra-1.1.1/naja_atra.egg-info/requires.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       10 2024-05-13 03:11:49.000000 naja_atra-1.1.1/naja_atra.egg-info/top_level.txt
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)      929 2024-05-11 10:09:28.000000 naja_atra-1.1.1/pyproject.toml
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       38 2024-05-13 03:11:49.047187 naja_atra-1.1.1/setup.cfg
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)       62 2024-05-11 10:09:28.000000 naja_atra-1.1.1/setup.py
+drwxrwxr-x   0 keijack   (1000) keijack   (1000)        0 2024-05-13 03:11:49.043189 naja_atra-1.1.1/tests/
+-rw-rw-r--   0 keijack   (1000) keijack   (1000)     9112 2024-05-13 03:03:45.000000 naja_atra-1.1.1/tests/test_all_ctrls.py
```

### Comparing `naja_atra-1.1.0/LICENSE` & `naja_atra-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/PKG-INFO` & `naja_atra-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja_atra-1.1.0/README.md` & `naja_atra-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/__init__.py` & `naja_atra-1.1.1/naja_atra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 SOFTWARE.
 """
 
 from .app_conf import *
 from .models import *
 
 name = "naja-atra"
-version = "1.1.0"
+version = "1.1.1"
```

### Comparing `naja_atra-1.1.0/naja_atra/__main__.py` & `naja_atra-1.1.1/naja_atra/__main__.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/app_conf.py` & `naja_atra-1.1.1/naja_atra/app_conf.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/http_servers/__init__.py` & `naja_atra-1.1.1/naja_atra/http_servers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/http_servers/coroutine_http_server.py` & `naja_atra-1.1.1/naja_atra/http_servers/coroutine_http_server.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/http_servers/http_server.py` & `naja_atra-1.1.1/naja_atra/http_servers/http_server.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/http_servers/routing_server.py` & `naja_atra-1.1.1/naja_atra/http_servers/routing_server.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/http_servers/threading_http_server.py` & `naja_atra-1.1.1/naja_atra/http_servers/threading_http_server.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/models.py` & `naja_atra-1.1.1/naja_atra/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 
 class RequestBodyReader:
 
     @abstractmethod
     async def read(self, n: int = -1) -> bytes:
         return NotImplemented
 
+    @abstractmethod
     async def read_to_end(self) -> bytes:
         return NotImplemented
 
 
 class Request:
     """Request"""
```

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/__init__.py` & `naja_atra-1.1.1/naja_atra/request_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/http_controller_handler.py` & `naja_atra-1.1.1/naja_atra/request_handlers/http_controller_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,110 +46,124 @@
 from .http_session_local_impl import LocalSessionFactory
 from ..utils.logger import get_logger
 from ..utils.http_utils import get_function_args, get_function_kwargs
 
 _logger = get_logger("naja_atra.request_handlers.http_request_handler")
 
 
+class RequestBodyReaderDumpWrapper(RequestBodyReader):
+
+    def __init__(self, reader: StreamReader) -> None:
+        self._reader = reader
+
+    async def read(self, n: int = -1) -> bytes:
+        _logger.warning(
+            "`Content-Length` and `Transfer-Encoding` are both not set in request, so we can't read the body.")
+        return b''
+
+    async def read_to_end(self) -> bytes:
+        _logger.warning(
+            "`Content-Length` and `Transfer-Encoding` are both not set in request, so we can't read the body.")
+        raise b''
+
+
 class RequestBodyReaderWrapper(RequestBodyReader):
 
-    def __init__(self, reader: StreamReader, content_length: int = None) -> None:
+    def __init__(self, reader: StreamReader, content_length: int) -> None:
+        if content_length is None or content_length < 0:
+            raise HttpError(400, "Invalid content length")
         self._content_length: int = content_length
         self._remain_length: int = content_length
         self._reader: StreamReader = reader
+        self._lock = asyncio.Lock()
 
     async def read(self, n: int = -1) -> bytes:
-        data = b''
-        if not n:
-            return data
-        if self._remain_length is not None and self._remain_length <= 0:
-            return data
-        if n < 0:
-            if self._remain_length:
-                data = await self._reader.read(self._remain_length)
-            else:
-                data = await self._reader.read()
-        else:
-            if self._remain_length and n > self._remain_length:
+        async with self._lock:
+            if not n or self._remain_length <= 0:
+                return b''
+            if n < 0:
                 data = await self._reader.read(self._remain_length)
             else:
-                data = await self._reader.read(n)
+                data = await self._reader.read(min(n, self._remain_length))
 
-        if self._remain_length and self._remain_length > 0:
             self._remain_length -= len(data)
 
-        return data
+            return data
 
     async def read_to_end(self) -> bytes:
-        return await self.read(self._remain_length)
+        data = b''
+        while self._remain_length > 0:
+            data += await self.read()
+        return data
 
 
 class RequestBodyReaderChunkedReader(RequestBodyReader):
 
     def __init__(self, reader: StreamReader) -> None:
         self._reader = reader
         self._current_chunk_len: int = -1
         self._buffer: bytes = b''
         self._eof: bool = False
         self._lock = asyncio.Lock()
 
     async def _fill_buffer(self):
         if self._eof:
+            _logger.warning("The body or this request has been all read. ")
             return
         if self._buffer:
+            _logger.debug(
+                f"There is still data in buffer. length: {len(self._buffer)}")
             return
 
         if self._current_chunk_len > 0:
             self._buffer = await self._reader.read(self._current_chunk_len)
             self._current_chunk_len -= len(self._buffer)
             return
 
         if self._current_chunk_len == 0:
             # Read \r\n at the end of a chunk
-            self._reader.read(2)
+            rn = await self._reader.read(2)
+            if rn != b'\r\n':
+                raise HttpError(400, f"Invalid chunk end: {rn}")
 
         chunk_len = await self._reader.readline()
         chunk_len = chunk_len.rstrip(b'\r\n')
         self._current_chunk_len = int(chunk_len, 16)
         _logger.debug(f"current chunk length: {self._current_chunk_len}")
         if self._current_chunk_len == 0:
             # Read \r\n at the end of the final chunk
-            await self._reader.read(2)
+            rn = await self._reader.read(2)
+            if rn != b'\r\n':
+                raise HttpError(400, f"Invalid chunk end: {rn}")
             self._eof = True
             return
         if self._current_chunk_len < 0:
             raise HttpError(400, "Invalid chunk length")
         self._buffer = await self._reader.read(self._current_chunk_len)
         self._current_chunk_len -= len(self._buffer)
 
-    async def _read(self, n: int = -1) -> bytes:
+    async def read(self, n: int = -1) -> bytes:
         async with self._lock:
             if not n:
                 return b''
             await self._fill_buffer()
-            if len(self._buffer) > n:
-                data = self._buffer[:n]
-                self._buffer = self._buffer[n:]
-                return data
-            else:
+            if n < 0 or n >= len(self._buffer):
                 data = self._buffer
                 self._buffer = b''
                 return data
-
-    async def read(self, n: int = -1) -> bytes:
-        if n >= 0:
-            return await self._read(n)
-        else:
-            data = b''
-            while not self._eof:
-                data += await self._read()
-            return data
+            else:
+                data = self._buffer[:n]
+                self._buffer = self._buffer[n:]
+                return data
 
     async def read_to_end(self) -> bytes:
-        return await self._read(-1)
+        data = b''
+        while not self._eof:
+            data += await self.read()
+        return data
 
 
 class RequestWrapper(Request):
 
     def __init__(self):
         super().__init__()
         self._headers_keys_in_lowcase = {}
@@ -576,15 +590,15 @@
         if "content-length" in _headers_keys_in_lowers.keys():
             content_length = int(_headers_keys_in_lowers["content-length"])
             req.reader = RequestBodyReaderWrapper(self.reader, content_length)
         elif _headers_keys_in_lowers.get("transfer-encoding", "").lower() == "chunked":
             _logger.debug("chunked encoding")
             req.reader = RequestBodyReaderChunkedReader(self.reader)
         else:
-            req.reader = RequestBodyReaderWrapper(self.reader)
+            req.reader = RequestBodyReaderDumpWrapper(self.reader)
 
         content_type = _headers_keys_in_lowers.get("content-type", "")
         if content_type.lower().startswith("application/x-www-form-urlencoded"):
             charset = http_utils.get_charset(content_type)
             req._body = await req.reader.read_to_end()
             body_decoded_params = http_utils.decode_query_string(
                 req._body.decode(charset))
```

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/http_request_handler.py` & `naja_atra-1.1.1/naja_atra/request_handlers/http_request_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         except socket.timeout as e:
             # a read or a write timed out.  Discard this connection
             self.log_error("Request timed out: %r", e)
             self.close_connection = True
             return
 
 
-class SocketServerStreamRequestHandlerWraper(socketserver.StreamRequestHandler, RequestBodyReader):
+class SocketServerStreamRequestHandlerWraper(socketserver.StreamRequestHandler):
 
     server_version = HttpRequestHandler.server_version
 
     # Wrapper method for readline
     async def readline(self):
         return self.rfile.readline(_LINE_MAX_BYTES)
```

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/http_session_local_impl.py` & `naja_atra-1.1.1/naja_atra/request_handlers/http_session_local_impl.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/model_bindings.py` & `naja_atra-1.1.1/naja_atra/request_handlers/model_bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,43 +213,41 @@
 class RegGroupModelBinding(ModelBinding):
 
     async def bind(self) -> RegGroup:
         return self.__build_reg_group(**self._kws)
 
     def __build_reg_group(self, val: RegGroup = RegGroup(group=0)):
         if val.group >= len(self.request.reg_groups):
-            raise HttpError(
-                400, None, f"RegGroup required an element at {val.group}, but the reg length is only {len(self.request.reg_groups)}")
+            raise HttpError(400, None, f"RegGroup required an element at {val.group}, but the reg length is only {len(self.request.reg_groups)}")
         return RegGroup(group=val.group, _value=self.request.reg_groups[val.group])
 
 
 class JSONBodyModelBinding(ModelBinding):
 
     async def bind(self) -> Any:
         return self.__build_json_body()
 
     def __build_json_body(self):
         if "content-type" not in self.request._headers_keys_in_lowcase.keys() or \
                 not self.request._headers_keys_in_lowcase["content-type"].lower().startswith("application/json"):
-            raise HttpError(
-                400, None, 'The content type of this request must be "application/json"')
+            raise HttpError(400, None, 'The content type of this request must be "application/json"')
         return JSONBody(self.request.json)
 
 
 class RequestBodyReaderModelBinding(ModelBinding):
 
     async def bind(self) -> Any:
         return self.request.reader
 
 
 class BytesBodyModelBinding(ModelBinding):
 
     async def bind(self) -> Any:
         if not self.request._body:
-            self.request._body = await self.request.reader.read()
+            self.request._body = await self.request.reader.read_to_end()
         return BytesBody(self.request._body)
 
 
 class StrModelBinding(ModelBinding):
 
     async def bind(self) -> Any:
         return self.__build_str(self.arg_name, **self._kws)
```

### Comparing `naja_atra-1.1.0/naja_atra/request_handlers/websocket_controller_handler.py` & `naja_atra-1.1.1/naja_atra/request_handlers/websocket_controller_handler.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/server.py` & `naja_atra-1.1.1/naja_atra/server.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/utils/__init__.py` & `naja_atra-1.1.1/naja_atra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/utils/http_utils.py` & `naja_atra-1.1.1/naja_atra/utils/http_utils.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra/utils/logger.py` & `naja_atra-1.1.1/naja_atra/utils/logger.py`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/naja_atra.egg-info/PKG-INFO` & `naja_atra-1.1.1/naja_atra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naja-atra
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a simple http server, use MVC like design.
 Author-email: keijack <keijack.wu@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Keijack Wu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naja_atra-1.1.0/pyproject.toml` & `naja_atra-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naja_atra-1.1.0/tests/test_all_ctrls.py` & `naja_atra-1.1.1/tests/test_all_ctrls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 
 from gzip import GzipFile
 import os
 import json
+import socket
 import websocket
 import unittest
 import urllib.request
 import urllib.error
 import http.client
 from typing import Dict
 from threading import Thread
@@ -243,13 +244,44 @@
         age = 18
         res: Dict = self.visit(
             f"model_binding/person?name={name}&sex={sex}&age={age}", return_type="JSON")
         assert res["name"] == name
         assert res["sex"] == sex
         assert res["age"] == age
 
+    def test_send_chunked(self):
+        sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        try:
+            sock.connect(("127.0.0.1", self.PORT))
+            request = (
+                "POST {} HTTP/1.1\r\n"
+                "Host: {}\r\n"
+                "Transfer-Encoding: chunked\r\n"
+                "Content-Type: text/plain\r\n"
+                "\r\n"
+                "8\r\n"
+                "Mozilla \r\n"
+                "11\r\n"
+                "Developer Network\r\n"
+                "0\r\n"
+                "\r\n"
+            ).format(f"/chunked", f"127.0.0.1:{self.PORT}")
+
+            sock.sendall(request.encode('utf-8'))
+            response = b''
+            while True:
+                data = sock.recv(4096)
+                if not data:
+                    break
+                response += data
+            response = response.split(b'\r\n')[-1].strip()
+            res = json.loads(response)
+            assert res["data"] == "Mozilla Developer Network"
+        finally:
+            sock.close()
+
 
 class CoroutineServerTest(ThreadingServerTest):
 
     PORT = 9091
 
     COROUTINE = True
```

