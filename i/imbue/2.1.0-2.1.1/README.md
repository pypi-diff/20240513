# Comparing `tmp/imbue-2.1.0.tar.gz` & `tmp/imbue-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imbue-2.1.0.tar", max compression
+gzip compressed data, was "imbue-2.1.1.tar", max compression
```

## Comparing `imbue-2.1.0.tar` & `imbue-2.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1070 2024-05-03 13:31:23.480868 imbue-2.1.0/LICENSE
--rw-r--r--   0        0        0     5330 2024-05-03 13:31:23.480868 imbue-2.1.0/README.md
--rw-r--r--   0        0        0      583 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/__init__.py
--rw-r--r--   0        0        0      786 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/abc.py
--rw-r--r--   0        0        0     6735 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/container.py
--rw-r--r--   0        0        0        0 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/__init__.py
--rw-r--r--   0        0        0     3089 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/abc.py
--rw-r--r--   0        0        0     1782 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/application.py
--rw-r--r--   0        0        0     4279 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/base.py
--rw-r--r--   0        0        0      461 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/factory.py
--rw-r--r--   0        0        0      587 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/task.py
--rw-r--r--   0        0        0     1188 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/contexts/thread.py
--rw-r--r--   0        0        0     1237 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/dependency.py
--rw-r--r--   0        0        0      288 2024-05-03 13:31:23.480868 imbue-2.1.0/imbue/exceptions.py
--rw-r--r--   0        0        0      716 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/fastapi/README.md
--rw-r--r--   0        0        0      106 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/fastapi/__init__.py
--rw-r--r--   0        0        0      872 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/fastapi/app.py
--rw-r--r--   0        0        0      987 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/fastapi/request.py
--rw-r--r--   0        0        0     1209 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/package.py
--rw-r--r--   0        0        0        0 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/providers/__init__.py
--rw-r--r--   0        0        0      966 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/providers/abc.py
--rw-r--r--   0        0        0     1728 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/providers/common.py
--rw-r--r--   0        0        0     2036 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/providers/function.py
--rw-r--r--   0        0        0     3333 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/providers/instance.py
--rw-r--r--   0        0        0        0 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/py.typed
--rw-r--r--   0        0        0     4172 2024-05-03 13:31:23.484868 imbue-2.1.0/imbue/utils.py
--rw-r--r--   0        0        0      970 2024-05-03 13:31:23.484868 imbue-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 imbue-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-13 07:52:27.117802 imbue-2.1.1/LICENSE
+-rw-r--r--   0        0        0     5330 2024-05-13 07:52:27.117802 imbue-2.1.1/README.md
+-rw-r--r--   0        0        0      583 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/__init__.py
+-rw-r--r--   0        0        0      786 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/abc.py
+-rw-r--r--   0        0        0     6735 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/container.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/__init__.py
+-rw-r--r--   0        0        0     3089 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/abc.py
+-rw-r--r--   0        0        0     2055 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/application.py
+-rw-r--r--   0        0        0     4279 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/base.py
+-rw-r--r--   0        0        0      461 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/factory.py
+-rw-r--r--   0        0        0      587 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/task.py
+-rw-r--r--   0        0        0     1461 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/contexts/thread.py
+-rw-r--r--   0        0        0     1237 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/dependency.py
+-rw-r--r--   0        0        0      288 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/exceptions.py
+-rw-r--r--   0        0        0      716 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/fastapi/README.md
+-rw-r--r--   0        0        0      106 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/fastapi/__init__.py
+-rw-r--r--   0        0        0      872 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/fastapi/app.py
+-rw-r--r--   0        0        0      987 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/fastapi/request.py
+-rw-r--r--   0        0        0     1209 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/package.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/providers/__init__.py
+-rw-r--r--   0        0        0      966 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/providers/abc.py
+-rw-r--r--   0        0        0     1728 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/providers/common.py
+-rw-r--r--   0        0        0     2036 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/providers/function.py
+-rw-r--r--   0        0        0     3333 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/providers/instance.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/py.typed
+-rw-r--r--   0        0        0     4172 2024-05-13 07:52:27.117802 imbue-2.1.1/imbue/utils.py
+-rw-r--r--   0        0        0      970 2024-05-13 07:52:27.117802 imbue-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6102 1970-01-01 00:00:00.000000 imbue-2.1.1/PKG-INFO
```

### Comparing `imbue-2.1.0/LICENSE` & `imbue-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/README.md` & `imbue-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/__init__.py` & `imbue-2.1.1/imbue/__init__.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/abc.py` & `imbue-2.1.1/imbue/abc.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/container.py` & `imbue-2.1.1/imbue/container.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/contexts/abc.py` & `imbue-2.1.1/imbue/contexts/abc.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/contexts/application.py` & `imbue-2.1.1/imbue/contexts/application.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import threading
-from typing import Any, ContextManager, Dict
+from typing import Any, Callable, ContextManager, Dict, Type, overload
 
 from imbue.abc import InternalContainer
-from imbue.contexts.abc import ContextualizedContainer
+from imbue.contexts.abc import ContextualizedContainer, V
 from imbue.contexts.base import Context, make_context_decorator
 from imbue.contexts.task import TaskContainer
 from imbue.contexts.thread import ThreadContainer
 from imbue.dependency import Interface
 
 application_context = make_context_decorator(Context.APPLICATION)
 
@@ -26,14 +26,22 @@
     async def init(self) -> None:
         await super().init()
         # Init the main thread's container.
         container = ThreadContainer(self._container, self._contextualized)
         self._contextualized[container.CONTEXT] = container
         await self.enter_async_context(container)
 
+    @overload
+    async def get(self, interface: Type[V]) -> V:
+        """Specific type annotation for classes."""
+
+    @overload
+    async def get(self, interface: Callable) -> Callable:
+        """Specific type annotation for functions."""
+
     async def get(self, interface: Interface) -> Any:
         if provided := self._provided.get(interface):
             return provided
         with self._lock:
             if interface not in self._locks:
                 self._locks[interface] = threading.Lock()
         with self._locks[interface]:
```

### Comparing `imbue-2.1.0/imbue/contexts/base.py` & `imbue-2.1.1/imbue/contexts/base.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/contexts/task.py` & `imbue-2.1.1/imbue/contexts/task.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/dependency.py` & `imbue-2.1.1/imbue/dependency.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/fastapi/README.md` & `imbue-2.1.1/imbue/fastapi/README.md`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/fastapi/app.py` & `imbue-2.1.1/imbue/fastapi/app.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/fastapi/request.py` & `imbue-2.1.1/imbue/fastapi/request.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/package.py` & `imbue-2.1.1/imbue/package.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/providers/abc.py` & `imbue-2.1.1/imbue/providers/abc.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/providers/common.py` & `imbue-2.1.1/imbue/providers/common.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/providers/function.py` & `imbue-2.1.1/imbue/providers/function.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/providers/instance.py` & `imbue-2.1.1/imbue/providers/instance.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/imbue/utils.py` & `imbue-2.1.1/imbue/utils.py`

 * *Files identical despite different names*

### Comparing `imbue-2.1.0/pyproject.toml` & `imbue-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imbue"
-version = "2.1.0"
+version = "2.1.1"
 description = "Type based python dependency injection framework."
 authors = ["Gabriel Pajot <gab@lescactus.eu>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/imbue"
 include = ["imbue/py.typed"]
 
@@ -16,15 +16,15 @@
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "==8.2.0"
 pytest-asyncio = "==0.23.6"
 pytest-mock = "==3.14.0"
-ruff = "==0.4.2"
+ruff = "==0.4.4"
 mypy = "==1.10.0"
 pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `imbue-2.1.0/PKG-INFO` & `imbue-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imbue
-Version: 2.1.0
+Version: 2.1.1
 Summary: Type based python dependency injection framework.
 Home-page: https://github.com/gpajot/imbue
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@lescactus.eu
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

