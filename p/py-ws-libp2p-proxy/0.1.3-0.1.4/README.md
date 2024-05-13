# Comparing `tmp/py_ws_libp2p_proxy-0.1.3.tar.gz` & `tmp/py_ws_libp2p_proxy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_ws_libp2p_proxy-0.1.3.tar", max compression
+gzip compressed data, was "py_ws_libp2p_proxy-0.1.4.tar", max compression
```

## Comparing `py_ws_libp2p_proxy-0.1.3.tar` & `py_ws_libp2p_proxy-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11344 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/LICENSE
--rw-r--r--   0        0        0      257 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/README.md
--rw-r--r--   0        0        0      517 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3877 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/__init__.py
--rw-r--r--   0        0        0     2358 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/decorators.py
--rw-r--r--   0        0        0       53 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/logger.py
--rw-r--r--   0        0        0      794 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/message.py
--rw-r--r--   0        0        0      663 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/protocols_manager.py
--rw-r--r--   0        0        0     3452 2024-04-05 14:43:53.036234 py_ws_libp2p_proxy-0.1.3/pyproxy/utils/websocket.py
--rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11344 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/LICENSE
+-rw-r--r--   0        0        0      257 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/README.md
+-rw-r--r--   0        0        0      517 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3877 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/__init__.py
+-rw-r--r--   0        0        0     2358 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/decorators.py
+-rw-r--r--   0        0        0       53 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/logger.py
+-rw-r--r--   0        0        0     1002 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/message.py
+-rw-r--r--   0        0        0      663 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/protocols_manager.py
+-rw-r--r--   0        0        0     3474 2024-05-13 13:53:45.244402 py_ws_libp2p_proxy-0.1.4/pyproxy/utils/websocket.py
+-rw-r--r--   0        0        0      992 1970-01-01 00:00:00.000000 py_ws_libp2p_proxy-0.1.4/PKG-INFO
```

### Comparing `py_ws_libp2p_proxy-0.1.3/LICENSE` & `py_ws_libp2p_proxy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproject.toml` & `py_ws_libp2p_proxy-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-ws-libp2p-proxy"
-version = "0.1.3"
+version = "0.1.4"
 description = "API for libp2p-ws-proxy"
 authors = [
     "Mariia Livshits <m.bystramovich@gmail.com>",
 ]
 license = "Apache-2.0"
 
 repository = "https://github.com/tubleronchik/py-libp2p-proxy"
```

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproxy/__init__.py` & `py_ws_libp2p_proxy-0.1.4/pyproxy/__init__.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/decorators.py` & `py_ws_libp2p_proxy-0.1.4/pyproxy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/message.py` & `py_ws_libp2p_proxy-0.1.4/pyproxy/utils/message.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,7 +20,15 @@
         message = {"protocol": protocol, "serverPeerId": server_peer_id, "save_data": save_data, "data": {"data": data}}
     return json.dumps(message)
 
 
 def format_msg_for_subscribing(protocols: list) -> str:
     msg = {"protocols_to_listen": protocols}
     return json.dumps(msg)
+
+class InitialMessage:
+    def __init__(self, msg: str):
+        self._parse_msg(msg)
+
+    def _parse_msg(self, msg):
+        self.peer_id = msg["peerId"]
+        self.multi_addressess = msg["multiAddresses"]
```

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/protocols_manager.py` & `py_ws_libp2p_proxy-0.1.4/pyproxy/utils/protocols_manager.py`

 * *Files identical despite different names*

### Comparing `py_ws_libp2p_proxy-0.1.3/pyproxy/utils/websocket.py` & `py_ws_libp2p_proxy-0.1.4/pyproxy/utils/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import websockets
 import typing as tp
 import json
 from .logger import logger
-from .message import format_msg_from_libp2p, format_msg_for_subscribing
+from .message import format_msg_from_libp2p, format_msg_for_subscribing, InitialMessage
 from .decorators import set_websocket
 from .protocols_manager import ProtocolsManager, CallbackTypes
 
 
 class WebsocketClient:
     def __init__(
         self, protocols_manager: ProtocolsManager, proxy_server_url: str, peer_id_callback: tp.Optional[tp.Callable]
@@ -59,15 +59,15 @@
             logger.debug(f"Received message from server: {message}")
             await self._consumer(message)
 
     async def _consumer(self, message: str) -> None:
         message = json.loads(message)
         if "peerId" in message:
             if self.peer_id_callback is not None:
-                self.peer_id_callback(message["peerId"])
+                self.peer_id_callback(InitialMessage(message))
                 return
         if message.get("protocol") in self.protocols_manager.protocols:
             protocol = message.get("protocol")
             formated_msg = format_msg_from_libp2p(message)
             callback_obj = self.protocols_manager.protocols[protocol]
             callback_type = callback_obj.callback_type
             if callback_type == CallbackTypes.AsyncType:
```

### Comparing `py_ws_libp2p_proxy-0.1.3/PKG-INFO` & `py_ws_libp2p_proxy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ws-libp2p-proxy
-Version: 0.1.3
+Version: 0.1.4
 Summary: API for libp2p-ws-proxy
 Home-page: https://github.com/tubleronchik/py-libp2p-proxy
 License: Apache-2.0
 Author: Mariia Livshits
 Author-email: m.bystramovich@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

