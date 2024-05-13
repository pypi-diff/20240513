# Comparing `tmp/nooscope-rpc-1.0.8.tar.gz` & `tmp/nooscope-rpc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nooscope-rpc-1.0.8.tar", last modified: Thu Sep 30 02:47:24 2021, max compression
+gzip compressed data, was "nooscope-rpc-1.0.9.tar", last modified: Thu Sep 30 03:06:42 2021, max compression
```

## Comparing `nooscope-rpc-1.0.8.tar` & `nooscope-rpc-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35058 2021-09-30 01:07:43.000000 nooscope-rpc-1.0.8/LICENSE.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       40 2021-09-30 02:40:20.000000 nooscope-rpc-1.0.8/MANIFEST.in
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2305 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1831 2021-09-30 01:58:52.000000 nooscope-rpc-1.0.8/README.md
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      154 2021-09-30 01:13:54.000000 nooscope-rpc-1.0.8/pyproject.toml
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      618 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/setup.cfg
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       61 2021-09-30 02:34:00.000000 nooscope-rpc-1.0.8/setup.py
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 00:01:07.000000 nooscope-rpc-1.0.8/src/nooscope_rpc/__init__.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     5391 2021-09-30 02:46:28.000000 nooscope-rpc-1.0.8/src/nooscope_rpc/api.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      717 2021-09-30 00:28:06.000000 nooscope-rpc-1.0.8/src/nooscope_rpc/constants.py
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1245 2021-09-30 02:17:43.000000 nooscope-rpc-1.0.8/src/nooscope_rpc/selfsigned.cert
-drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2305 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/PKG-INFO
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)      381 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/requires.txt
--rw-r--r--   0 vagrant   (1000) vagrant   (1000)       13 2021-09-30 02:47:24.000000 nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/top_level.txt
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)    35058 2021-09-30 01:07:43.000000 nooscope-rpc-1.0.9/LICENSE.md
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       40 2021-09-30 02:40:20.000000 nooscope-rpc-1.0.9/MANIFEST.in
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2305 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1831 2021-09-30 01:58:52.000000 nooscope-rpc-1.0.9/README.md
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      154 2021-09-30 01:13:54.000000 nooscope-rpc-1.0.9/pyproject.toml
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      618 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/setup.cfg
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       61 2021-09-30 02:34:00.000000 nooscope-rpc-1.0.9/setup.py
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 00:01:07.000000 nooscope-rpc-1.0.9/src/nooscope_rpc/__init__.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     4788 2021-09-30 03:05:45.000000 nooscope-rpc-1.0.9/src/nooscope_rpc/api.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      717 2021-09-30 00:28:06.000000 nooscope-rpc-1.0.9/src/nooscope_rpc/constants.py
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     1245 2021-09-30 02:17:43.000000 nooscope-rpc-1.0.9/src/nooscope_rpc/selfsigned.cert
+drwxr-xr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)     2305 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)      381 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)        1 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       14 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/requires.txt
+-rw-r--r--   0 vagrant   (1000) vagrant   (1000)       13 2021-09-30 03:06:41.000000 nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/top_level.txt
```

### Comparing `nooscope-rpc-1.0.8/LICENSE.md` & `nooscope-rpc-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nooscope-rpc-1.0.8/PKG-INFO` & `nooscope-rpc-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nooscope-rpc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple TCP client impl to interact with IRC_BOT
 Home-page: https://github.com/deacon-ralph/irc_bot
 Author: HARDCHATTING_THUG
 Author-email: cumdata@protonmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/deacon-ralph/irc_bot/issues
 Platform: UNKNOWN
```

### Comparing `nooscope-rpc-1.0.8/README.md` & `nooscope-rpc-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nooscope-rpc-1.0.8/setup.cfg` & `nooscope-rpc-1.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nooscope-rpc
-version = 1.0.8
+version = 1.0.9
 author = HARDCHATTING_THUG
 author_email = cumdata@protonmail.com
 description = Simple TCP client impl to interact with IRC_BOT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/deacon-ralph/irc_bot
 project_urls =
```

### Comparing `nooscope-rpc-1.0.8/src/nooscope_rpc/api.py` & `nooscope-rpc-1.0.9/src/nooscope_rpc/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -177,32 +177,7 @@
                 _LOGGER.error('IncompleteReadError, client closed?')
                 data = None
                 break
 
         _LOGGER.info(f'LOOP WAS BROKEN: {data}')
         self.writer.close()
         await self.writer.wait_closed()
-
-import asyncio
-
-
-
-class Impl(IrcImpl):
-   async def on_message(self, target, by, message):
-      print(target, by, message)
-      # do some shit like
-      if message == 'hack_a_gibson' and by == 'ZeroCool':
-         await self.rpc.send_message('#test', 'hacking gibson from RPC')
-      elif message.startswith('dieplz'):
-         await self.rpc.disconnect()
-
-
-async def main():
-   # endless loop to always try and connect
-   while True:
-      tcp = TcpClient('127.0.0.1', 12345, Impl())
-      await tcp.connect()
-      await tcp.read()
-
-
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
```

### Comparing `nooscope-rpc-1.0.8/src/nooscope_rpc/constants.py` & `nooscope-rpc-1.0.9/src/nooscope_rpc/constants.py`

 * *Files identical despite different names*

### Comparing `nooscope-rpc-1.0.8/src/nooscope_rpc/selfsigned.cert` & `nooscope-rpc-1.0.9/src/nooscope_rpc/selfsigned.cert`

 * *Files identical despite different names*

### Comparing `nooscope-rpc-1.0.8/src/nooscope_rpc.egg-info/PKG-INFO` & `nooscope-rpc-1.0.9/src/nooscope_rpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nooscope-rpc
-Version: 1.0.8
+Version: 1.0.9
 Summary: Simple TCP client impl to interact with IRC_BOT
 Home-page: https://github.com/deacon-ralph/irc_bot
 Author: HARDCHATTING_THUG
 Author-email: cumdata@protonmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/deacon-ralph/irc_bot/issues
 Platform: UNKNOWN
```

