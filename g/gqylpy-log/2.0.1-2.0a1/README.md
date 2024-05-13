# Comparing `tmp/gqylpy_log-2.0.1.tar.gz` & `tmp/gqylpy_log-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_log-2.0.1.tar", last modified: Mon May 13 00:59:53 2024, max compression
+gzip compressed data, was "gqylpy_log-2.0a1.tar", last modified: Mon Apr 15 00:53:09 2024, max compression
```

## Comparing `gqylpy_log-2.0.1.tar` & `gqylpy_log-2.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:59:53.468912 gqylpy_log-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-13 00:59:49.000000 gqylpy_log-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-13 00:59:53.468912 gqylpy_log-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-13 00:59:49.000000 gqylpy_log-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:59:53.464912 gqylpy_log-2.0.1/gqylpy_log/
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-05-13 00:59:49.000000 gqylpy_log-2.0.1/gqylpy_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-05-13 00:59:49.000000 gqylpy_log-2.0.1/gqylpy_log/g log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 00:59:53.468912 gqylpy_log-2.0.1/gqylpy_log.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-13 00:59:53.000000 gqylpy_log-2.0.1/gqylpy_log.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-13 00:59:53.000000 gqylpy_log-2.0.1/gqylpy_log.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 00:59:53.000000 gqylpy_log-2.0.1/gqylpy_log.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 00:59:53.000000 gqylpy_log-2.0.1/gqylpy_log.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 00:59:53.468912 gqylpy_log-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-13 00:59:49.000000 gqylpy_log-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/gqylpy_log/
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/gqylpy_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/gqylpy_log/g log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/gqylpy_log.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:53:09.000000 gqylpy_log-2.0a1/gqylpy_log.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:53:09.681287 gqylpy_log-2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-15 00:52:54.000000 gqylpy_log-2.0a1/setup.py
```

### Comparing `gqylpy_log-2.0.1/LICENSE` & `gqylpy_log-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqylpy_log-2.0.1/PKG-INFO` & `gqylpy_log-2.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gqylpy_log
-Version: 2.0.1
-Summary: Secondary encapsulation `logging`, more convenient and fast to create the logger. Use this module can quickly create instances of `logging.Logger` and complete a series of log configuration, make your code cleaner.
+Version: 2.0a1
+Summary: Secondary encapsulation `logging`, more convenient and fast to create
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `gqylpy_log-2.0.1/README.md` & `gqylpy_log-2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `gqylpy_log-2.0.1/gqylpy_log/__init__.py` & `gqylpy_log-2.0a1/gqylpy_log/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Secondary encapsulation `logging`, more convenient and fast to create the
 logger. Use this module can quickly create instances of `logging.Logger` and
 complete a series of log configuration, make your code cleaner.
 
     >>> import gqylpy_log as glog
     >>> glog.info(...)
 
-    @version: 2.0.1
+    @version: 2.0alpha1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-log
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `gqylpy_log-2.0.1/gqylpy_log/g log.py` & `gqylpy_log-2.0a1/gqylpy_log/g log.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,53 +89,45 @@
     logger = logging.Logger(name, level)
 
     if formatter.__class__ is dict:
         formatter = logging.Formatter(**formatter)
 
     for handler_or_params in handlers:
         if isinstance(handler_or_params, logging.Handler):
-            if handler_or_params.level == 0:
-                handler_or_params.setLevel(level)
-            if handler_or_params.formatter is None:
-                handler_or_params.setFormatter(formatter)
-            for x in filters:
-                handler_or_params.addFilter(x)
-            if options.get("onlyRecordCurrentLevel"):
-                handler_or_params.filters.append(
-                    only_record_current_level(handler_or_params.level)
-                )
             logger.addHandler(handler_or_params)
             continue
 
         if "formatter" in handler_or_params:
             the_formatter: Formatter = handler_or_params.pop("formatter")
             if the_formatter.__class__ is dict:
                 the_formatter = logging.Formatter(**the_formatter)
         else:
             the_formatter = formatter
 
-        the_level:   Level        = handler_or_params.pop("level", level)
-        the_filters: List[Filter] = handler_or_params.pop("filters", filters)
-        the_options: Options      = handler_or_params.pop("options", options)
+        the_level:   Level         = handler_or_params.pop("level", level)
+        the_filters: List[Filter]  = handler_or_params.pop("filters", filters)
+        the_options: Options       = handler_or_params.pop("options", options)
 
         handler_type: Type[logging.Handler] = \
             getattr(logging_handlers, handler_or_params.pop("name"))
 
         if issubclass(handler_type, logging.FileHandler):
             filename: str = handler_or_params["filename"]
             logdir:   str = os.path.dirname(os.path.abspath(filename))
             os.makedirs(logdir, exist_ok=True)
 
         handler: logging.Handler = handler_type(**handler_or_params)
         handler.setLevel(the_level)
         handler.setFormatter(the_formatter)
-        for x in the_filters:
-            handler.addFilter(x)
+        handler.filters.extend(
+            x for x in the_filters if x not in handler.filters
+        )
+
         if the_options.get("onlyRecordCurrentLevel"):
-            handler.filters.append(only_record_current_level(handler.level))
+            handler.addFilter(only_record_current_level(handler.level))
 
         logger.addHandler(handler)
 
     if gname:
         if not hasattr(gcode, "default") or gcode.default.name == "default":
             gcode.default = logger
         setattr(gpack, gname, logger)
@@ -166,29 +158,35 @@
         if gname is None:
             if not hasattr(gcode, "default"):
                 __init__("default", **gpack.default, gname="default")
             gobj: logging.Logger = default
         elif gname.__class__ is str:
             gobj: logging.Logger = getattr(gpack, gname, None)
             if gobj.__class__ is not logging.Logger:
-                raise NameError(
-                    f"gname '{gname}' not found in '{__package__}'."
-                )
+                raise NameError(f"gname '{gname}' not in '{__package__}'.")
         elif gname.__class__ is logging.Logger:
             gobj: logging.Logger = gname
         else:
             raise TypeError(
                 "parameter 'gname' type must be 'str' or 'logging.Logger', "
                 f"not '{gname.__class__.__name__}'."
             )
 
         if sys.version_info >= (3, 8):
-            if "stacklevel" not in kw:
-                kw["stacklevel"] = 2
-            elif kw["stacklevel"] < 2:
+            if "stacklevel" in kw:
+                if kw["stacklevel"].__class__ is not int:
+                    if not kw["stacklevel"].isdigit():
+                        raise TypeError(
+                            "parameter 'stacklevel' type must be 'int', "
+                            f"not '{kw['stacklevel'].__class__.__name__}'."
+                        )
+                    kw["stacklevel"] = int(kw["stacklevel"])
+                if kw["stacklevel"] < 2:
+                    kw["stacklevel"] = 2
+            else:
                 kw["stacklevel"] = 2
 
         msg: str = sep.join(str(m) for m in msg)
 
         if oneline:
             msg: str = linesep.join(
                 m.strip() for m in msg.split("\n") if m and not m.isspace()
```

### Comparing `gqylpy_log-2.0.1/gqylpy_log.egg-info/PKG-INFO` & `gqylpy_log-2.0a1/gqylpy_log.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gqylpy_log
-Version: 2.0.1
-Summary: Secondary encapsulation `logging`, more convenient and fast to create the logger. Use this module can quickly create instances of `logging.Logger` and complete a series of log configuration, make your code cleaner.
+Version: 2.0a1
+Summary: Secondary encapsulation `logging`, more convenient and fast to create
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-log
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `gqylpy_log-2.0.1/setup.py` & `gqylpy_log-2.0a1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     author_email=email,
     license="Apache 2.0",
     url="http://gqylpy.com",
     project_urls={"Source": source},
     description="""
         Secondary encapsulation `logging`, more convenient and fast to create
         the logger. Use this module can quickly create instances of
-        `logging.Logger` and complete a series of log configuration, make your
+        `logging.Logger` and complete a series of log configuration,make your
         code cleaner.
-    """.strip().replace('\n       ', ''),
+    """,
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     packages=[g.__name__],
     python_requires=">=3.8",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

