# Comparing `tmp/wherobots_python_dbapi-0.4.0.tar.gz` & `tmp/wherobots_python_dbapi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wherobots_python_dbapi-0.4.0.tar", max compression
+gzip compressed data, was "wherobots_python_dbapi-0.5.0.tar", max compression
```

## Comparing `wherobots_python_dbapi-0.4.0.tar` & `wherobots_python_dbapi-0.5.0.tar`

### file list

```diff
@@ -1,29 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-16 08:39:06.034287 wherobots_python_dbapi-0.4.0/LICENSE
--rw-r--r--   0        0        0     1348 2024-04-18 02:22:07.996092 wherobots_python_dbapi-0.4.0/README.md
--rw-r--r--   0        0        0      944 2024-04-18 02:22:07.996394 wherobots_python_dbapi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 08:39:06.035856 wherobots_python_dbapi-0.4.0/wherobots/__init__.py
--rw-r--r--   0        0        0      184 2024-04-16 08:39:06.036056 wherobots_python_dbapi-0.4.0/wherobots/db/__init__.py
--rw-r--r--   0        0        0      541 2024-04-17 12:40:13.095446 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      429 2024-04-17 01:59:58.204058 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    12468 2024-04-17 12:40:13.096330 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/connection.cpython-311.pyc
--rw-r--r--   0        0        0     7305 2024-04-17 01:59:58.204779 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/connection.cpython-39.pyc
--rw-r--r--   0        0        0     3027 2024-04-17 14:50:29.120119 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0        0        0     1968 2024-04-17 12:32:56.491121 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0        0        0     5223 2024-04-17 15:06:38.290095 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/cursor.cpython-311.pyc
--rw-r--r--   0        0        0     3340 2024-04-17 12:32:56.494241 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/cursor.cpython-39.pyc
--rw-r--r--   0        0        0     7200 2024-04-17 12:40:13.581645 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/driver.cpython-311.pyc
--rw-r--r--   0        0        0     4156 2024-04-17 02:03:05.852570 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/driver.cpython-39.pyc
--rw-r--r--   0        0        0     1534 2024-04-17 12:40:13.580458 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/errors.cpython-311.pyc
--rw-r--r--   0        0        0     1128 2024-04-17 02:01:32.187990 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/errors.cpython-39.pyc
--rw-r--r--   0        0        0      513 2024-04-17 12:40:13.578580 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/region.cpython-311.pyc
--rw-r--r--   0        0        0      405 2024-04-17 02:01:32.186523 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/region.cpython-39.pyc
--rw-r--r--   0        0        0      966 2024-04-17 12:40:13.579009 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/runtime.cpython-311.pyc
--rw-r--r--   0        0        0      815 2024-04-17 02:01:32.186879 wherobots_python_dbapi-0.4.0/wherobots/db/__pycache__/runtime.cpython-39.pyc
--rw-r--r--   0        0        0     7655 2024-04-17 01:55:28.212065 wherobots_python_dbapi-0.4.0/wherobots/db/connection.py
--rw-r--r--   0        0        0     1598 2024-04-18 02:22:07.996760 wherobots_python_dbapi-0.4.0/wherobots/db/constants.py
--rw-r--r--   0        0        0     2774 2024-04-18 02:22:07.997072 wherobots_python_dbapi-0.4.0/wherobots/db/cursor.py
--rw-r--r--   0        0        0     4643 2024-04-16 08:39:06.036769 wherobots_python_dbapi-0.4.0/wherobots/db/driver.py
--rw-r--r--   0        0        0      310 2024-04-16 08:39:06.036896 wherobots_python_dbapi-0.4.0/wherobots/db/errors.py
--rw-r--r--   0        0        0       80 2024-04-16 08:39:06.037003 wherobots_python_dbapi-0.4.0/wherobots/db/region.py
--rw-r--r--   0        0        0      491 2024-04-16 08:39:06.037125 wherobots_python_dbapi-0.4.0/wherobots/db/runtime.py
--rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2651 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/README.md
+-rw-r--r--   0        0        0      944 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/__init__.py
+-rw-r--r--   0        0        0     8317 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/connection.py
+-rw-r--r--   0        0        0     1767 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/constants.py
+-rw-r--r--   0        0        0     2774 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/cursor.py
+-rw-r--r--   0        0        0     5718 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/driver.py
+-rw-r--r--   0        0        0      310 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/errors.py
+-rw-r--r--   0        0        0       80 2024-05-13 03:05:01.523868 wherobots_python_dbapi-0.5.0/wherobots/db/region.py
+-rw-r--r--   0        0        0      491 2024-05-13 03:05:01.527868 wherobots_python_dbapi-0.5.0/wherobots/db/runtime.py
+-rw-r--r--   0        0        0     3495 1970-01-01 00:00:00.000000 wherobots_python_dbapi-0.5.0/PKG-INFO
```

### Comparing `wherobots_python_dbapi-0.4.0/LICENSE` & `wherobots_python_dbapi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.4.0/pyproject.toml` & `wherobots_python_dbapi-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wherobots-python-dbapi"
-version = "0.4.0"
+version = "0.5.0"
 description = "Python DB-API driver for Wherobots DB"
 authors = ["Maxime Petazzoni <max@wherobots.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "wherobots" }]
 
 [project.urls]
```

### Comparing `wherobots_python_dbapi-0.4.0/wherobots/db/connection.py` & `wherobots_python_dbapi-0.5.0/wherobots/db/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import json
 import logging
+import textwrap
 import threading
 import uuid
 from dataclasses import dataclass
-from typing import Callable, Any
+from typing import Any, Callable, Union
 
 import cbor2
 import pyarrow
 import websockets.exceptions
 import websockets.protocol
 import websockets.sync.client
 
 from wherobots.db.constants import (
     DEFAULT_READ_TIMEOUT_SECONDS,
     RequestKind,
     EventKind,
     ExecutionState,
     ResultsFormat,
     DataCompression,
+    GeometryRepresentation,
 )
 from wherobots.db.cursor import Cursor
 from wherobots.db.errors import NotSupportedError, OperationalError
 
-_DEFAULT_RESULTS_FORMAT = ResultsFormat.ARROW
-_DEFAULT_DATA_COMPRESSION = DataCompression.BROTLI
-
 
 @dataclass
 class Query:
     sql: str
     execution_id: str
     state: ExecutionState
     handler: Callable[[Any], None]
@@ -49,17 +48,24 @@
     corresponding query state. Queries are tracked by their unique execution ID.
     """
 
     def __init__(
         self,
         ws: websockets.sync.client.ClientConnection,
         read_timeout: float = DEFAULT_READ_TIMEOUT_SECONDS,
+        results_format: Union[ResultsFormat, None] = None,
+        data_compression: Union[DataCompression, None] = None,
+        geometry_representation: Union[GeometryRepresentation, None] = None,
     ):
         self.__ws = ws
         self.__read_timeout = read_timeout
+        self.__results_format = results_format
+        self.__data_compression = data_compression
+        self.__geometry_representation = geometry_representation
+
         self.__queries: dict[str, Query] = {}
         self.__thread = threading.Thread(
             target=self.__main_loop, daemon=True, name="wherobots-connection"
         )
         self.__thread.start()
 
     def __enter__(self):
@@ -151,27 +157,27 @@
             elif result_format == ResultsFormat.ARROW:
                 buffer = pyarrow.py_buffer(result_bytes)
                 stream = pyarrow.input_stream(buffer, result_compression)
                 with pyarrow.ipc.open_stream(stream) as reader:
                     query.handler(reader.read_pandas())
             else:
                 query.handler(
-                    OperationalError(
-                        f"Unsupported results format {result_format}"
-                    )
+                    OperationalError(f"Unsupported results format {result_format}")
                 )
         elif kind == EventKind.ERROR:
             query.state = ExecutionState.FAILED
             error = message.get("message")
             query.handler(OperationalError(error))
         else:
             logging.warning("Received unknown %s event!", kind)
 
     def __send(self, message: dict[str, Any]) -> None:
-        self.__ws.send(json.dumps(message))
+        request = json.dumps(message)
+        logging.debug("Request: %s", request)
+        self.__ws.send(request)
 
     def __recv(self) -> dict[str, Any]:
         frame = self.__ws.recv(timeout=self.__read_timeout)
         if isinstance(frame, str):
             message = json.loads(frame)
         elif isinstance(frame, bytes):
             message = cbor2.loads(frame)
@@ -190,28 +196,37 @@
 
         self.__queries[execution_id] = Query(
             sql=sql,
             execution_id=execution_id,
             state=ExecutionState.EXECUTION_REQUESTED,
             handler=handler,
         )
+
+        logging.info(
+            "Executing SQL query %s: %s", execution_id, textwrap.shorten(sql, width=60)
+        )
         self.__send(request)
         return execution_id
 
     def __request_results(self, execution_id: str) -> None:
         query = self.__queries.get(execution_id)
         if not query:
             return
 
         request = {
             "kind": RequestKind.RETRIEVE_RESULTS.value,
             "execution_id": execution_id,
-            "format": _DEFAULT_RESULTS_FORMAT.value,
-            "compression": _DEFAULT_DATA_COMPRESSION.value,
         }
+        if self.__results_format:
+            request["format"] = self.__results_format.value
+        if self.__data_compression:
+            request["compression"] = self.__data_compression.value
+        if self.__geometry_representation:
+            request["geometry"] = self.__geometry_representation.value
+
         query.state = ExecutionState.RESULTS_REQUESTED
         logging.info("Requesting results from %s ...", execution_id)
         self.__send(request)
 
     def __cancel_query(self, execution_id: str) -> None:
         query = self.__queries.pop(execution_id)
         if query:
```

### Comparing `wherobots_python_dbapi-0.4.0/wherobots/db/constants.py` & `wherobots_python_dbapi-0.5.0/wherobots/db/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from enum import auto
 from strenum import LowercaseStrEnum
 
 from .region import Region
 from .runtime import Runtime
 
 
-DEFAULT_ENDPOINT: str = "api.wherobots.services"  # "api.cloud.wherobots.com"
-STAGING_ENDPOINT: str = "api.staging.wherobots.services"  # "api.staging.wherobots.com"
+DEFAULT_ENDPOINT: str = "api.cloud.wherobots.com"  # "api.cloud.wherobots.com"
+STAGING_ENDPOINT: str = "api.staging.wherobots.com"  # "api.staging.wherobots.com"
 DEFAULT_RUNTIME: Runtime = Runtime.SEDONA
 DEFAULT_REGION: Region = Region.AWS_US_WEST_2
 DEFAULT_READ_TIMEOUT_SECONDS: float = 0.25
 DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS: float = 300
 MAX_MESSAGE_SIZE: int = 100 * 2**20  # 100MiB
+PROTOCOL_VERSION: str = "1.0.0"
 
 
 class ExecutionState(LowercaseStrEnum):
     IDLE = auto()
     "Not executing any operation."
 
     EXECUTION_REQUESTED = auto()
@@ -54,7 +55,15 @@
 class ResultsFormat(LowercaseStrEnum):
     JSON = auto()
     ARROW = auto()
 
 
 class DataCompression(LowercaseStrEnum):
     BROTLI = auto()
+
+
+class GeometryRepresentation(LowercaseStrEnum):
+    WKT = auto()
+    WKB = auto()
+    EWKT = auto()
+    EWKB = auto()
+    GEOJSON = auto()
```

### Comparing `wherobots_python_dbapi-0.4.0/wherobots/db/cursor.py` & `wherobots_python_dbapi-0.5.0/wherobots/db/cursor.py`

 * *Files identical despite different names*

### Comparing `wherobots_python_dbapi-0.4.0/wherobots/db/driver.py` & `wherobots_python_dbapi-0.5.0/wherobots/db/driver.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 """Wherobots DB driver.
 
 A PEP-0249 compatible driver for interfacing with Wherobots DB.
 """
 
 import logging
+import os
 import urllib.parse
 import queue
 import requests
 import tenacity
 import threading
+from typing import Union
 import websockets.sync.client
 
 from .constants import (
     DEFAULT_ENDPOINT,
     DEFAULT_REGION,
     DEFAULT_RUNTIME,
     DEFAULT_READ_TIMEOUT_SECONDS,
     DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS,
     MAX_MESSAGE_SIZE,
+    PROTOCOL_VERSION,
+    ResultsFormat,
+    DataCompression,
+    GeometryRepresentation,
 )
 from .errors import (
     InterfaceError,
     OperationalError,
 )
 from .region import Region
 from .runtime import Runtime
@@ -36,14 +42,17 @@
     host: str = DEFAULT_ENDPOINT,
     token: str = None,
     api_key: str = None,
     runtime: Runtime = None,
     region: Region = None,
     wait_timeout: float = DEFAULT_SESSION_WAIT_TIMEOUT_SECONDS,
     read_timeout: float = DEFAULT_READ_TIMEOUT_SECONDS,
+    results_format: Union[ResultsFormat, None] = None,
+    data_compression: Union[DataCompression, None] = None,
+    geometry_representation: Union[GeometryRepresentation, None] = None,
 ) -> Connection:
     if not token and not api_key:
         raise ValueError("At least one of `token` or `api_key` is required")
     if token and api_key:
         raise ValueError("`token` and `api_key` can't be both provided")
 
     headers = {}
@@ -109,38 +118,50 @@
     except Exception as e:
         raise InterfaceError("Could not acquire SQL session!", e)
 
     return connect_direct(
         uri=http_to_ws(session_uri),
         headers=headers,
         read_timeout=read_timeout,
+        results_format=results_format,
+        data_compression=data_compression,
+        geometry_representation=geometry_representation,
     )
 
 
 def http_to_ws(uri: str) -> str:
     """Converts an HTTP URI to a WebSocket URI."""
     parsed = urllib.parse.urlparse(uri)
     for from_scheme, to_scheme in [("http", "ws"), ("https", "wss")]:
         if parsed.scheme == from_scheme:
             parsed = parsed._replace(scheme=to_scheme)
     return str(urllib.parse.urlunparse(parsed))
 
 
+def append_protocol(uri: str, protocol: str) -> str:
+    """Appends the protocol version to the URI."""
+    return urllib.parse.urljoin(os.path.join(uri, ""), protocol)
+
+
 def connect_direct(
     uri: str,
     headers: dict[str, str] = None,
     read_timeout: float = DEFAULT_READ_TIMEOUT_SECONDS,
+    results_format: Union[ResultsFormat, None] = None,
+    data_compression: Union[DataCompression, None] = None,
+    geometry_representation: Union[GeometryRepresentation, None] = None,
 ) -> Connection:
     q = queue.SimpleQueue()
+    uri_with_protocol = append_protocol(uri, PROTOCOL_VERSION)
 
     def create_ws_connection():
         try:
-            logging.info("Connecting to SQL session at %s ...", uri)
+            logging.info("Connecting to SQL session at %s ...", uri_with_protocol)
             ws = websockets.sync.client.connect(
-                uri=uri,
+                uri=uri_with_protocol,
                 additional_headers=headers,
                 max_size=MAX_MESSAGE_SIZE,
             )
             q.put(ws)
         except Exception as e:
             q.put(e)
 
@@ -152,8 +173,14 @@
     dt.start()
     dt.join()
 
     result = q.get()
     if isinstance(result, Exception):
         raise InterfaceError("Failed to connect to SQL session!") from result
 
-    return Connection(result, read_timeout)
+    return Connection(
+        result,
+        read_timeout=read_timeout,
+        results_format=results_format,
+        data_compression=data_compression,
+        geometry_representation=geometry_representation,
+    )
```

