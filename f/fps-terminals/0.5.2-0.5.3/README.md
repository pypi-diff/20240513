# Comparing `tmp/fps_terminals-0.5.2.tar.gz` & `tmp/fps_terminals-0.5.3.tar.gz`

## Comparing `fps_terminals-0.5.2.tar` & `fps_terminals-0.5.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/fps_terminals/main.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/fps_terminals/routes.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/fps_terminals/win_server.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/pyproject.toml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/fps_terminals/main.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.5.3/PKG-INFO
```

### Comparing `fps_terminals-0.5.2/fps_terminals/main.py` & `fps_terminals-0.5.3/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/fps_terminals/routes.py` & `fps_terminals-0.5.3/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/fps_terminals/server.py` & `fps_terminals-0.5.3/fps_terminals/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         task = asyncio.create_task(self.send_data())
 
         def on_output():
             try:
                 self.data_or_disconnect = self.p_out.read(65536).decode()
                 self.event.set()
             except Exception:
+                os.close(self.fd)
                 self.loop.remove_reader(self.p_out)
                 self.data_or_disconnect = None
                 self.event.set()
 
         self.loop.add_reader(self.p_out, on_output)
         await websocket.send_json(["setup", {}])
         can_execute = permissions is None or "execute" in permissions.get("terminals", [])
@@ -70,7 +71,8 @@
                     await websocket.send_json(["stdout", self.data_or_disconnect])
 
     def quit(self, websocket):
         if websocket in self.websockets:
             self.websockets.remove(websocket)
         if not self.websockets:
             os.close(self.fd)
+            self.loop.remove_reader(self.p_out)
```

### Comparing `fps_terminals-0.5.2/fps_terminals/win_server.py` & `fps_terminals-0.5.3/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/.gitignore` & `fps_terminals-0.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/COPYING.md` & `fps_terminals-0.5.3/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/pyproject.toml` & `fps_terminals-0.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.2/PKG-INFO` & `fps_terminals-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_terminals
-Version: 0.5.2
+Version: 0.5.3
 Summary: An FPS plugin for the terminals API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

