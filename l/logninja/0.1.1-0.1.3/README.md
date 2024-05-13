# Comparing `tmp/logninja-0.1.1.tar.gz` & `tmp/logninja-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logninja-0.1.1.tar", last modified: Sat May 11 22:43:34 2024, max compression
+gzip compressed data, was "logninja-0.1.3.tar", last modified: Mon May 13 16:02:16 2024, max compression
```

## Comparing `logninja-0.1.1.tar` & `logninja-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 22:43:34.747139 logninja-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-05-11 18:30:54.000000 logninja-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1180 2024-05-11 22:43:34.742978 logninja-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2024-05-11 22:42:33.000000 logninja-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 22:43:34.668043 logninja-0.1.1/logninja/
--rw-rw-rw-   0        0        0      677 2024-05-11 21:15:31.000000 logninja-0.1.1/logninja/__init__.py
--rw-rw-rw-   0        0        0      139 2024-05-11 20:21:58.000000 logninja-0.1.1/logninja/console_formatter.py
--rw-rw-rw-   0        0        0     1323 2024-05-11 22:41:07.000000 logninja-0.1.1/logninja/decorators.py
--rw-rw-rw-   0        0        0     2122 2024-05-11 20:53:45.000000 logninja-0.1.1/logninja/json_formatter.py
--rw-rw-rw-   0        0        0      757 2024-05-11 20:56:04.000000 logninja-0.1.1/logninja/uvicorn_logger_name_filter.py
-drwxrwxrwx   0        0        0        0 2024-05-11 22:43:34.739580 logninja-0.1.1/logninja.egg-info/
--rw-rw-rw-   0        0        0     1180 2024-05-11 22:43:34.000000 logninja-0.1.1/logninja.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-11 22:43:34.000000 logninja-0.1.1/logninja.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 22:43:34.000000 logninja-0.1.1/logninja.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-11 22:43:34.000000 logninja-0.1.1/logninja.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-11 22:43:34.747139 logninja-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-05-11 22:41:57.000000 logninja-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.085021 logninja-0.1.3/
+-rw-rw-rw-   0        0        0     1092 2024-05-11 18:30:54.000000 logninja-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      958 2024-05-13 16:02:16.082499 logninja-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       69 2024-05-11 22:42:33.000000 logninja-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 16:02:15.785781 logninja-0.1.3/logninja/
+-rw-rw-rw-   0        0        0      716 2024-05-13 01:19:58.000000 logninja-0.1.3/logninja/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.022503 logninja-0.1.3/logninja/asgi/
+-rw-rw-rw-   0        0        0        0 2024-05-11 22:58:24.000000 logninja-0.1.3/logninja/asgi/__init__.py
+-rw-rw-rw-   0        0        0     3924 2024-05-13 01:26:33.000000 logninja-0.1.3/logninja/asgi/middleware.py
+-rw-rw-rw-   0        0        0      139 2024-05-11 20:21:58.000000 logninja-0.1.3/logninja/console_formatter.py
+-rw-rw-rw-   0        0        0      470 2024-05-11 23:30:27.000000 logninja-0.1.3/logninja/contextvars_filter.py
+-rw-rw-rw-   0        0        0     1481 2024-05-13 01:25:36.000000 logninja-0.1.3/logninja/decorators.py
+-rw-rw-rw-   0        0        0     1891 2024-05-13 01:20:22.000000 logninja-0.1.3/logninja/json_formatter.py
+drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.078505 logninja-0.1.3/logninja.egg-info/
+-rw-rw-rw-   0        0        0      958 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 16:02:14.000000 logninja-0.1.3/logninja.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      885 2024-05-13 15:54:33.000000 logninja-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 16:02:16.085021 logninja-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 16:02:16.066906 logninja-0.1.3/tests/
+-rw-rw-rw-   0        0        0     1263 2024-05-12 21:17:02.000000 logninja-0.1.3/tests/test_json_formatter.py
```

### Comparing `logninja-0.1.1/LICENSE` & `logninja-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `logninja-0.1.1/PKG-INFO` & `logninja-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.1
+Version: 0.1.3
 Summary: A log configuration library for Python projects.
-Home-page: https://github.com/ppcantidio/logmancer.py
-Author: Pedro Cantidio
-Author-email: ppcantidio@gmail.com
+Author-email: Pedro Cantidio <ppcantidio@gmail.com>
+Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: starlette
+Requires-Dist: starlette<0.38.0,>=0.37.2; extra == "starlette"
 
-LogNinja is a library that provides a set of tools to configure logging in Python projects. It is designed to be used with the standard logging module and provides a set of classes and functions to help you configure your loggers, formatters, and filters. LogMancer is designed to be easy to use and flexible, allowing you to configure your loggers in a way that best suits your project.
+# LogNinja
+Simple logging setup to be used at python applications.
```

### Comparing `logninja-0.1.1/logninja/decorators.py` & `logninja-0.1.3/logninja/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 import asyncio
 import functools
 import logging
 import time
 
-logger = logging.getLogger(__name__)
+from logninja import logger as logninja_logger
 
 
-def log_execution(func):
+def log_execution(logger: logging.Logger = logninja_logger):
     """
     Decorator to log the execution time of a function or coroutine.
 
     Args:
-        func (Callable): The function or coroutine to be decorated.
+        logger (logging.Logger): The logger to be used.
 
     Returns:
-        Callable: The decorated function or coroutine.
+        Callable: The decorator.
     """
 
-    def log_start(*args, **kwargs):
-        params = {"args": list(args), "kwargs": kwargs}
-        logger.info(
-            f"Starting execution of function {func.__qualname__}",
-            extra={"params": params},
-        )
-
-    def log_end(end: float, start: float):
-        logger.info(f"{func.__qualname__} executed in {end - start:.4f} seconds")
-
-    @functools.wraps(func)
-    def sync_wrapper(*args, **kwargs):
-        log_start(*args, **kwargs)
-
-        start = time.time()
-        result = func(*args, **kwargs)
-        end = time.time()
-
-        log_end(end, start)
-        return result
-
-    async def async_wrapper(*args, **kwargs):
-        log_start(*args, **kwargs)
-
-        start = time.time()
-        result = await func(*args, **kwargs)
-        end = time.time()
+    def decorator(func):
+        def log_start(*args, **kwargs):
+            params = {"args": list(args), "kwargs": kwargs}
+            logger.info(
+                f"Starting execution of function {func.__qualname__}",
+                extra={"params": params},
+            )
 
-        log_end(end, start)
-        return result
+        def log_end(end: float, start: float):
+            logger.info(f"{func.__qualname__} executed in {end - start:.4f} seconds")
 
-    return async_wrapper if asyncio.iscoroutinefunction(func) else sync_wrapper
+        @functools.wraps(func)
+        def sync_wrapper(*args, **kwargs):
+            log_start(*args, **kwargs)
+
+            start = time.time()
+            result = func(*args, **kwargs)
+            end = time.time()
+
+            log_end(end, start)
+            return result
+
+        async def async_wrapper(*args, **kwargs):
+            log_start(*args, **kwargs)
+
+            start = time.time()
+            result = await func(*args, **kwargs)
+            end = time.time()
+
+            log_end(end, start)
+            return result
+
+        return async_wrapper if asyncio.iscoroutinefunction(func) else sync_wrapper
+
+    return decorator
```

### Comparing `logninja-0.1.1/logninja/json_formatter.py` & `logninja-0.1.3/logninja/json_formatter.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime as dt
 import json
 import logging
-from contextvars import ContextVar
 
 LOG_RECORD_BUILTIN_ATTRS = {
     "args",
     "asctime",
     "created",
     "exc_info",
     "exc_text",
@@ -38,22 +37,18 @@
     "function": "funcName",
     "line": "lineno",
     "thread_name": "threadName",
 }
 
 
 class JSONFormatter(logging.Formatter):
-
     def format(self, record: logging.LogRecord) -> str:
         message = self._prepare_log_dict(record)
         return json.dumps(message, default=str)
 
-    def set_contextvar(self, contextvar: ContextVar):
-        self.contextvar = contextvar
-
     def _prepare_log_dict(self, record: logging.LogRecord):
         always_fields = {
             "message": record.getMessage(),
             "timestamp": dt.datetime.fromtimestamp(
                 record.created, tz=dt.timezone.utc
             ).isoformat(),
         }
@@ -73,11 +68,8 @@
         }
         message.update(always_fields)
 
         for key, val in record.__dict__.items():
             if key not in LOG_RECORD_BUILTIN_ATTRS:
                 message[key] = val
 
-        if self.contextvar:
-            message[self.contextvar.name] = self.contextvar.get()
-
         return message
```

### Comparing `logninja-0.1.1/logninja.egg-info/PKG-INFO` & `logninja-0.1.3/logninja.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.1
+Version: 0.1.3
 Summary: A log configuration library for Python projects.
-Home-page: https://github.com/ppcantidio/logmancer.py
-Author: Pedro Cantidio
-Author-email: ppcantidio@gmail.com
+Author-email: Pedro Cantidio <ppcantidio@gmail.com>
+Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: starlette
+Requires-Dist: starlette<0.38.0,>=0.37.2; extra == "starlette"
 
-LogNinja is a library that provides a set of tools to configure logging in Python projects. It is designed to be used with the standard logging module and provides a set of classes and functions to help you configure your loggers, formatters, and filters. LogMancer is designed to be easy to use and flexible, allowing you to configure your loggers in a way that best suits your project.
+# LogNinja
+Simple logging setup to be used at python applications.
```

