# Comparing `tmp/cheeseapi_websocket-1.0.1.tar.gz` & `tmp/cheeseapi_websocket-1.0.2.tar.gz`

## Comparing `cheeseapi_websocket-1.0.1.tar` & `cheeseapi_websocket-1.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/CheeseAPI_Websocket/__init__.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/CheeseAPI_Websocket/handle.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/CheeseAPI_Websocket/websocket.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/LICENSE
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/__init__.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/handle.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/websocket.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/README.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 cheeseapi_websocket-1.0.2/PKG-INFO
```

### Comparing `cheeseapi_websocket-1.0.1/CheeseAPI_Websocket/handle.py` & `cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/handle.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.1/CheeseAPI_Websocket/websocket.py` & `cheeseapi_websocket-1.0.2/CheeseAPI_Websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.1/LICENSE` & `cheeseapi_websocket-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi_websocket-1.0.1/README.md` & `cheeseapi_websocket-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 ```python
 import threading, time
 
 from CheeseAPI import app, WebsocketClient, Response
 from CheeseAPI_Websocket import websocket
 
-app.modules = [ 'CheeseAPI_Websocket' ] # 加入模块
+app.modules.append('CheeseAPI_Websocket') # 加入模块
 
 websocket.init() # 初始化redis连接
 
 @app.route.websocket('/')
 class Test(WebsocketClient):
     ...
```

### Comparing `cheeseapi_websocket-1.0.1/pyproject.toml` & `cheeseapi_websocket-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI_Websocket"
-version = "1.0.1"
+version = "1.0.2"
 description = "一款基于CheeseAPI的升级款Websocket插件。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
-keywords = [ 'websocket' ]
+keywords = [ 'CheeseAPI', 'websocket' ]
 
 dependencies = [
-    "CheeseAPI==1.1.*",
+    "CheeseAPI==1.2.*",
     "redis"
 ]
 
 [project.urls]
 Source = "https://github.com/CheeseUnknown/CheeseAPI_Websocket"
 
 [tool.hatch.build.targets.sdist]
```

### Comparing `cheeseapi_websocket-1.0.1/PKG-INFO` & `cheeseapi_websocket-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.3
 Name: CheeseAPI_Websocket
-Version: 1.0.1
+Version: 1.0.2
 Summary: 一款基于CheeseAPI的升级款Websocket插件。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI_Websocket
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
-Keywords: websocket
-Requires-Dist: cheeseapi==1.1.*
+Keywords: CheeseAPI,websocket
+Requires-Dist: cheeseapi==1.2.*
 Requires-Dist: redis
 Description-Content-Type: text/markdown
 
 # **CheeseAPI_Websocket**
 
 ## **介绍**
 
@@ -30,15 +30,15 @@
 
 ```python
 import threading, time
 
 from CheeseAPI import app, WebsocketClient, Response
 from CheeseAPI_Websocket import websocket
 
-app.modules = [ 'CheeseAPI_Websocket' ] # 加入模块
+app.modules.append('CheeseAPI_Websocket') # 加入模块
 
 websocket.init() # 初始化redis连接
 
 @app.route.websocket('/')
 class Test(WebsocketClient):
     ...
```

