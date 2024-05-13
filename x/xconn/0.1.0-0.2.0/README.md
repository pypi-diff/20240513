# Comparing `tmp/xconn-0.1.0.tar.gz` & `tmp/xconn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xconn-0.1.0.tar", last modified: Sun May  5 20:07:33 2024, max compression
+gzip compressed data, was "xconn-0.2.0.tar", last modified: Mon May 13 13:12:19 2024, max compression
```

## Comparing `xconn-0.1.0.tar` & `xconn-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-05 20:07:33.471398 xconn-0.1.0/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1102 2024-05-05 19:24:41.000000 xconn-0.1.0/LICENSE
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2224 2024-05-05 20:07:33.471398 xconn-0.1.0/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       15 2024-05-05 19:24:41.000000 xconn-0.1.0/README.md
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      965 2024-05-05 19:24:41.000000 xconn-0.1.0/pyproject.toml
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       38 2024-05-05 20:07:33.471398 xconn-0.1.0/setup.cfg
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-05 20:07:33.471398 xconn-0.1.0/xconn/
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        0 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/__init__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2170 2024-05-05 19:31:02.000000 xconn-0.1.0/xconn/__main__.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1834 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/acceptor.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      686 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/app.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/client.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      968 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/helpers.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      978 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/joiner.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     2805 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/realm.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1307 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/router.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     1533 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/server.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     9772 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/session.py
--rw-rw-r--   0 om26er    (1000) om26er    (1000)     8545 2024-05-05 19:24:41.000000 xconn-0.1.0/xconn/types.py
-drwxrwxr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-05 20:07:33.471398 xconn-0.1.0/xconn.egg-info/
--rw-r--r--   0 om26er    (1000) om26er    (1000)     2224 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/PKG-INFO
--rw-rw-r--   0 om26er    (1000) om26er    (1000)      403 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/SOURCES.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/dependency_links.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       46 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/entry_points.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)       80 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/requires.txt
--rw-rw-r--   0 om26er    (1000) om26er    (1000)        6 2024-05-05 20:07:33.000000 xconn-0.1.0/xconn.egg-info/top_level.txt
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1107 2024-05-10 21:55:47.000000 xconn-0.2.0/LICENSE
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-13 13:12:19.511291 xconn-0.2.0/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      771 2024-05-08 19:52:19.000000 xconn-0.2.0/README.md
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2509 2024-05-13 13:11:29.000000 xconn-0.2.0/pyproject.toml
+-rw-r--r--   0 om26er    (1000) om26er    (1000)       38 2024-05-13 13:12:19.511291 xconn-0.2.0/setup.cfg
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/xconn/
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      181 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/__init__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     2173 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/__main__.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1834 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/acceptor.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1079 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/app.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      574 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/client.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      968 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/helpers.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      978 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/joiner.py
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     2374 2024-05-13 13:11:29.000000 xconn-0.2.0/xconn/realm.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1307 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/router.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     1686 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/server.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     9772 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/session.py
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)     8545 2024-05-08 19:52:19.000000 xconn-0.2.0/xconn/types.py
+drwxr-xr-x   0 om26er    (1000) om26er    (1000)        0 2024-05-13 13:12:19.511291 xconn-0.2.0/xconn.egg-info/
+-rw-r--r--   0 om26er    (1000) om26er    (1000)     3098 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/PKG-INFO
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      403 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/SOURCES.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        1 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/dependency_links.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)       46 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/entry_points.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)      110 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/requires.txt
+-rw-rw-r--   0 om26er    (1000) om26er    (1000)        6 2024-05-13 13:12:19.000000 xconn-0.2.0/xconn.egg-info/top_level.txt
```

### Comparing `xconn-0.1.0/LICENSE` & `xconn-0.2.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
-Copyright (c) 2024 XConnIO
 Copyright (c) 2024 Simple Things Inc.
+Copyright (c) 2024 XConnIO Ltd.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `xconn-0.1.0/xconn/__main__.py` & `xconn-0.2.0/xconn/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 import importlib
 import sys
 
 import uvloop
 from wampproto.serializers import CBORSerializer
 
-from xconn.app import WampApp
+from xconn.app import XConnApp
 from xconn.router import Router
 from xconn.server import Server
 from xconn.session import AsyncSession
 from xconn.types import ServerSideLocalBaseSession, ClientSideLocalBaseSession
 
 
 def main():
@@ -26,16 +26,16 @@
     split = parsed.APP.split(":")
     if len(split) != 2:
         raise RuntimeError("invalid app argument, must be of format: module:instance")
 
     # TODO: find a better, reliable way
     sys.path.append(parsed.directory)
     module = importlib.import_module(split[0])
-    app: WampApp = getattr(module, split[1])
-    if not isinstance(app, WampApp):
+    app: XConnApp = getattr(module, split[1])
+    if not isinstance(app, XConnApp):
         raise RuntimeError(f"app instance is of unknown type {type(app)}")
 
     # uvloop makes things fast.
     uvloop.install()
 
     router = Router()
     router.add_realm(parsed.realm)
```

### Comparing `xconn-0.1.0/xconn/acceptor.py` & `xconn-0.2.0/xconn/acceptor.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/app.py` & `xconn-0.2.0/xconn/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 
 
 class IApp:
     @property
     def procedures(self) -> dict[str, Callable]:
         raise NotImplementedError()
 
+    def include_app(self, app: "IApp") -> None:
+        raise NotImplementedError()
+
     def register(self, procedure: str):
         raise NotImplementedError()
 
 
-class WampApp(IApp):
+class XConnApp(IApp):
     def __init__(self):
         super().__init__()
         self._procedures = {}
 
     @property
     def procedures(self) -> dict[str, Callable]:
         return self._procedures
 
+    def include_app(self, app: "IApp", prefix: str = "") -> None:
+        if prefix is None or len(prefix) == 0:
+            self._procedures.update(app.procedures)
+        else:
+            for procedure, func in app.procedures.items():
+                self._procedures.update({prefix + procedure: func})
+
     def register(self, procedure: str):
         def _register(func):
             if procedure in self._procedures:
                 raise ValueError(f"procedure {procedure} already registered")
 
             self._procedures[procedure] = func
```

### Comparing `xconn-0.1.0/xconn/client.py` & `xconn-0.2.0/xconn/client.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/helpers.py` & `xconn-0.2.0/xconn/helpers.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/joiner.py` & `xconn-0.2.0/xconn/joiner.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/realm.py` & `xconn-0.2.0/xconn/realm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from asyncio import gather
 
-from wampproto.types import MessageWithRecipient
 from wampproto import dealer, broker, messages
 
 from xconn import types
 
 
 class Realm:
     def __init__(self):
@@ -32,40 +31,30 @@
         match msg.TYPE:
             case messages.Call.TYPE | messages.Yield.TYPE | messages.Register.TYPE | messages.UnRegister.TYPE:
                 recipient = self.dealer.receive_message(session_id, msg)
                 client = self.clients[recipient.recipient]
                 await client.send_message(recipient.message)
 
             case messages.Publish.TYPE:
-                recipients = self.broker.receive_message(session_id, msg)
-                if recipients is None:
-                    # no subscribers AND "acknowledge=False"
-                    return
-
-                # if the publish options had "acknowledge=True" the last one
-                # should be PUBLISHED.
-                published: MessageWithRecipient | None = None
-                if isinstance(recipients[-1].message, messages.Published):
-                    published = recipients.pop(-1)
-
-                tasks = []
-                for recipient in recipients:
-                    client = self.clients[recipient.recipient]
-                    tasks.append(client.send_message(recipient.message))
-
-                await gather(*tasks)
-
-                if published is not None:
-                    client = self.clients[published.recipient]
-                    await client.send_message(published.message)
+                publication = self.broker.receive_publish(session_id, msg)
 
-            case messages.Subscribe.TYPE | messages.UnSubscribe.TYPE:
-                recipients = self.broker.receive_message(session_id, msg)
-                recipient = recipients[0]
+                if len(publication.recipients) != 0:
+                    tasks = []
+                    for recipient in publication.recipients:
+                        client = self.clients[recipient]
+                        tasks.append(client.send_message(publication.event))
+
+                    await gather(*tasks)
+
+                if publication.ack is not None:
+                    client = self.clients[publication.ack.recipient]
+                    await client.send_message(publication.ack.message)
 
+            case messages.Subscribe.TYPE | messages.UnSubscribe.TYPE:
+                recipient = self.broker.receive_message(session_id, msg)
                 client = self.clients[recipient.recipient]
                 await client.send_message(recipient.message)
             case messages.Goodbye.TYPE:
                 self.dealer.remove_session(session_id)
                 self.broker.remove_session(session_id)
                 try:
                     client = self.clients.pop(session_id)
```

### Comparing `xconn-0.1.0/xconn/router.py` & `xconn-0.2.0/xconn/router.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/server.py` & `xconn-0.2.0/xconn/server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import aiohttp
 from aiohttp import web
+from wampproto.auth import IServerAuthenticator
 
 from xconn.router import Router
 from xconn.acceptor import AIOHttpAcceptor
 
 
 class Server:
-    def __init__(self, router: Router):
+    def __init__(self, router: Router, authenticator: IServerAuthenticator = None):
         self.router = router
+        self.authenticator = authenticator
 
     async def _websocket_handler(self, request):
         ws = web.WebSocketResponse(protocols=["wamp.2.json", "wamp.2.cbor", "wamp.2.msgpack"])
         # upgrade this connection to websocket.
         await ws.prepare(request)
 
-        acceptor = AIOHttpAcceptor()
+        acceptor = AIOHttpAcceptor(self.authenticator)
         base_session = await acceptor.accept(ws)
         self.router.attach_client(base_session)
 
         while not ws.closed:
             msg = await ws.receive()
 
             if msg.type == aiohttp.WSMsgType.TEXT or msg.type == aiohttp.WSMsgType.BINARY:
```

### Comparing `xconn-0.1.0/xconn/session.py` & `xconn-0.2.0/xconn/session.py`

 * *Files identical despite different names*

### Comparing `xconn-0.1.0/xconn/types.py` & `xconn-0.2.0/xconn/types.py`

 * *Files identical despite different names*

