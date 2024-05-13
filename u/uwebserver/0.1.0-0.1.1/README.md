# Comparing `tmp/uwebserver-0.1.0.tar.gz` & `tmp/uwebserver-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwebserver-0.1.0.tar", last modified: Mon May 13 15:46:39 2024, max compression
+gzip compressed data, was "uwebserver-0.1.1.tar", last modified: Mon May 13 16:43:14 2024, max compression
```

## Comparing `uwebserver-0.1.0.tar` & `uwebserver-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:46:39.161087 uwebserver-0.1.0/
--rw-rw-rw-   0        0        0     1062 2024-05-12 16:25:08.000000 uwebserver-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2027 2024-05-13 15:46:39.159087 uwebserver-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       46 2024-05-12 20:10:55.000000 uwebserver-0.1.0/README.md
--rw-rw-rw-   0        0        0      969 2024-05-13 15:45:26.000000 uwebserver-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 15:46:39.161087 uwebserver-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 15:46:39.158090 uwebserver-0.1.0/uWebServer.egg-info/
--rw-rw-rw-   0        0        0     2027 2024-05-13 15:46:39.000000 uwebserver-0.1.0/uWebServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2024-05-13 15:46:39.000000 uwebserver-0.1.0/uWebServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:46:39.000000 uwebserver-0.1.0/uWebServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-13 15:46:39.000000 uwebserver-0.1.0/uWebServer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 15:46:39.000000 uwebserver-0.1.0/uWebServer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10268 2024-05-13 14:26:12.000000 uwebserver-0.1.0/uwebserver.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.697778 uwebserver-0.1.1/
+-rw-rw-rw-   0        0        0     1062 2024-05-12 16:25:08.000000 uwebserver-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2352 2024-05-13 16:43:14.696779 uwebserver-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-05-13 16:19:18.000000 uwebserver-0.1.1/README.md
+-rw-rw-rw-   0        0        0      967 2024-05-13 16:42:47.000000 uwebserver-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:43:14.697778 uwebserver-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.674798 uwebserver-0.1.1/uwebserver/
+-rw-rw-rw-   0        0        0      111 2024-05-13 16:31:00.000000 uwebserver-0.1.1/uwebserver/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 16:31:10.000000 uwebserver-0.1.1/uwebserver/py.typed
+-rw-rw-rw-   0        0        0    10280 2024-05-13 16:41:14.000000 uwebserver-0.1.1/uwebserver/webserver.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:43:14.694782 uwebserver-0.1.1/uwebserver.egg-info/
+-rw-rw-rw-   0        0        0     2352 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 16:43:14.000000 uwebserver-0.1.1/uwebserver.egg-info/top_level.txt
```

### Comparing `uwebserver-0.1.0/LICENSE` & `uwebserver-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uwebserver-0.1.0/pyproject.toml` & `uwebserver-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
-name = "uWebServer"
-version = "0.1.0"
+name = "uwebserver"
+version = "0.1.1"
 authors = [{ name = "0x4aK" }]
 description = "Simple web server for micropython"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: AsyncIO",
@@ -21,15 +21,15 @@
 dev = ["ruff >= 0.4.4", "pyright >= 1.1.362"]
 
 [build-system]
 requires = ["setuptools >= 69.5.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-py-modules = ["uwebserver"]
+packages = ["uwebserver"]
 
 [tool.pyright]
 reportMissingImports = false
 
 [tool.ruff]
 line-length = 100
 lint = { select = ["E", "F", "I", "UP", "SIM"] }
```

### Comparing `uwebserver-0.1.0/uwebserver.py` & `uwebserver-0.1.1/uwebserver/webserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,16 +177,16 @@
     def __init__(
         self,
         *,
         host: str = "0.0.0.0",
         port: int = 80,
         static_folder: str = "static",
     ) -> None:
-        self.h = host
-        self.p = port
+        self.host = host
+        self.port = port
         self.r: dict[tuple[str, str], Handler] = {}
         self.static = static_folder
         self._cah: "Handler" = self._dch  # Catch-all handler
         self._eh: "ErrorHanlder" = self._deh  # Error handler
         self.s: asyncio.Server | None = None
 
     def route(self, path: str, methods: "Methods" = ("GET",)):
@@ -333,9 +333,9 @@
         finally:
             w.close()
 
     def close(self):
         return self.s and self.s.close()
 
     async def run(self):
-        self.s = await asyncio.start_server(self._handle, self.h, self.p)
+        self.s = await asyncio.start_server(self._handle, self.host, self.port)
         await self.s.wait_closed()
```

