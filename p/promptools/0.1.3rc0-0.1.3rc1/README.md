# Comparing `tmp/promptools-0.1.3rc0.tar.gz` & `tmp/promptools-0.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptools-0.1.3rc0.tar", last modified: Thu Jan  4 15:30:09 2024, max compression
+gzip compressed data, was "promptools-0.1.3rc1.tar", last modified: Fri Jan  5 02:51:31 2024, max compression
```

## Comparing `promptools-0.1.3rc0.tar` & `promptools-0.1.3rc1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3468 2023-10-30 14:05:52.045450 promptools-0.1.3rc0/README.md
--rw-r--r--   0        0        0     1140 2024-01-04 15:30:09.179281 promptools-0.1.3rc0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-30 13:59:37.021676 promptools-0.1.3rc0/src/promptools/__init__.py
--rw-r--r--   0        0        0       50 2023-10-29 21:28:54.685864 promptools-0.1.3rc0/src/promptools/extractors/__init__.py
--rw-r--r--   0        0        0     1025 2024-01-01 10:23:35.980286 promptools-0.1.3rc0/src/promptools/extractors/json.py
--rw-r--r--   0        0        0      379 2024-01-01 10:23:45.492456 promptools-0.1.3rc0/src/promptools/extractors/json.pyi
--rw-r--r--   0        0        0       35 2023-10-30 12:31:50.224918 promptools-0.1.3rc0/src/promptools/openai/__init__.py
--rw-r--r--   0        0        0      732 2024-01-04 13:25:21.490281 promptools-0.1.3rc0/src/promptools/openai/tokenize.py
--rw-r--r--   0        0        0      544 2024-01-01 10:36:21.175074 promptools-0.1.3rc0/src/promptools/openai/tokenize.pyi
--rw-r--r--   0        0        0     1497 2024-01-04 15:05:35.595662 promptools-0.1.3rc0/src/promptools/utils/sse.py
--rw-r--r--   0        0        0      661 2024-01-04 15:03:50.648515 promptools-0.1.3rc0/src/promptools/utils/sse.pyi
--rw-r--r--   0        0        0     4144 1970-01-01 00:00:00.000000 promptools-0.1.3rc0/PKG-INFO
+-rw-r--r--   0        0        0     3756 2024-01-05 02:40:38.833621 promptools-0.1.3rc1/README.md
+-rw-r--r--   0        0        0     1140 2024-01-05 02:51:31.108906 promptools-0.1.3rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-05 02:35:49.444124 promptools-0.1.3rc1/src/promptools/__init__.py
+-rw-r--r--   0        0        0       50 2023-10-29 21:28:54.685864 promptools-0.1.3rc1/src/promptools/extractors/__init__.py
+-rw-r--r--   0        0        0     1025 2024-01-01 10:23:35.980286 promptools-0.1.3rc1/src/promptools/extractors/json.py
+-rw-r--r--   0        0        0      379 2024-01-01 10:23:45.492456 promptools-0.1.3rc1/src/promptools/extractors/json.pyi
+-rw-r--r--   0        0        0       35 2023-10-30 12:31:50.224918 promptools-0.1.3rc1/src/promptools/openai/__init__.py
+-rw-r--r--   0        0        0      771 2024-01-05 02:22:25.024181 promptools-0.1.3rc1/src/promptools/openai/tokenize.py
+-rw-r--r--   0        0        0      632 2024-01-05 02:23:07.355341 promptools-0.1.3rc1/src/promptools/openai/tokenize.pyi
+-rw-r--r--   0        0        0     1541 2024-01-05 02:07:44.201604 promptools-0.1.3rc1/src/promptools/utils/sse.py
+-rw-r--r--   0        0        0     1121 2024-01-05 02:14:52.267241 promptools-0.1.3rc1/src/promptools/utils/sse.pyi
+-rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 promptools-0.1.3rc1/PKG-INFO
```

### Comparing `promptools-0.1.3rc0/README.md` & `promptools-0.1.3rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -93,18 +93,18 @@
 #### `count_token`
 
 count number of tokens in prompt
 
 ##### Usages
 
 ```py
-def count_token(prompt: str, enc: Encoding | None = None) -> int:
+def count_token(prompt: str | list[str], enc: Encoding | None = None) -> int:
 ```
 
-Provide your prompt, get its token count. The second parameter is the `tiktoken.Encoding` instance, will default to `get_encoding("cl100k_base")` if not provided.
+Provide your prompt / a list of prompts, get its token count. The second parameter is the `tiktoken.Encoding` instance, will default to `get_encoding("cl100k_base")` if not provided. The default `tiktoken.Encoding` instance is cached, and will not be re-created every time.
 
 ```py
 def count_token(prompt: dict | list[dict], enc: Encoding | None = None) -> int:
 ```
 
 Note that it can also be a single message / a list of messages. Every message should be a dict in the schema below:
 
@@ -128,14 +128,28 @@
 
 The output will be:
 
 ```py
 1
 ```
 
+##### List of plain texts
+
+```py
+from promptools.openai import count_token
+
+print(count_token(["hi", "hello"]))
+```
+
+The output will be:
+
+```py
+2
+```
+
 ###### Single message
 
 ```py
 from promptools.openai import count_token
 
 count_token({"role": "user", "content": "hi"})
 ```
```

### Comparing `promptools-0.1.3rc0/pyproject.toml` & `promptools-0.1.3rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promptools"
-version = "0.1.3rc0"
+version = "0.1.3rc1"
 description = "useful utilities for prompt engineering"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "partial-json-parser>=0.1.2.1",
     "attrs>=23",
@@ -57,11 +57,11 @@
 [tool.pdm.scripts.fmt]
 composite = [
     "isort .",
     "black .",
 ]
 
 [tool.black]
-line-length = 100
+line-length = 140
 
 [tool.isort]
 profile = "black"
```

### Comparing `promptools-0.1.3rc0/src/promptools/extractors/json.py` & `promptools-0.1.3rc1/src/promptools/extractors/json.py`

 * *Files identical despite different names*

### Comparing `promptools-0.1.3rc0/src/promptools/openai/tokenize.py` & `promptools-0.1.3rc1/src/promptools/openai/tokenize.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
     enc = enc or cached_get_encoding("cl100k_base")
 
     if isinstance(prompt, str):
         return len(enc.encode(prompt, disallowed_special=()))
 
     if isinstance(prompt, list):
-        return 3 + sum(count_token(i, enc) for i in prompt)
+        if len(prompt) == 0:
+            return 0
+        return sum(count_token(i, enc) for i in prompt) + (0 if isinstance(prompt[0], str) else 3)
 
     if isinstance(prompt, dict):
-        return (
-            3
-            + (len(enc.encode(f"name={prompt['name']}")) if "name" in prompt else 1)
-            + len(enc.encode(prompt["content"]))
-        )
+        return 3 + (len(enc.encode(f"name={prompt['name']}")) if "name" in prompt else 1) + len(enc.encode(prompt["content"]))
 
     raise TypeError(prompt)
```

### Comparing `promptools-0.1.3rc0/src/promptools/openai/tokenize.pyi` & `promptools-0.1.3rc1/src/promptools/openai/tokenize.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,8 +9,10 @@
 
 def cached_get_encoding(encoding_name: str) -> Encoding: ...
 @overload
 def count_token(prompt: str, enc: Encoding | None = None) -> int: ...
 @overload
 def count_token(prompt: Message, enc: Encoding | None = None) -> int: ...
 @overload
+def count_token(prompt: list[str], enc: Encoding | None = None) -> int: ...
+@overload
 def count_token(prompt: list[Message], enc: Encoding | None = None) -> int: ...
```

### Comparing `promptools-0.1.3rc0/src/promptools/utils/sse.pyi` & `promptools-0.1.3rc1/src/promptools/utils/sse.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import count
 from typing import Any, AsyncIterator, Callable, Iterator, ParamSpec, TypeVar, overload
 
-from attrs import asdict, define
+from attrs import define
 from promplate import Template
 
 _template: str
 
 global_count: count
 
 event_template: Template
@@ -15,11 +15,19 @@
     data: str
     event: Any = None
     id: Callable[[], Any] | Any = global_count.__next__
 
 AnyIterator = TypeVar("AnyIterator", Iterator[str], AsyncIterator[str])
 P = ParamSpec("P")
 
+type SyncAnyIterator = Iterator[str] | Iterator[tuple[str, Any]] | Iterator[tuple[str, Any, Callable[[], Any] | Any]]
+
+type AsyncAnyIterator = AsyncIterator[str] | AsyncIterator[tuple[str, Any]] | AsyncIterator[tuple[str, Any, Callable[[], Any] | Any]]
+
+@overload
+def as_event_stream(gen: SyncAnyIterator) -> Iterator[Event]: ...
+@overload
+def as_event_stream(gen: AsyncAnyIterator) -> AsyncIterator[Event]: ...
 @overload
-def as_event_stream(gen: AnyIterator) -> AnyIterator: ...
+def as_event_stream(gen: Callable[P, SyncAnyIterator]) -> Callable[P, Iterator[Event]]: ...
 @overload
-def as_event_stream(gen: Callable[P, AnyIterator]) -> Callable[P, AnyIterator]: ...
+def as_event_stream(gen: Callable[P, AsyncAnyIterator]) -> Callable[P, AsyncIterator[Event]]: ...
```

### Comparing `promptools-0.1.3rc0/PKG-INFO` & `promptools-0.1.3rc1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptools
-Version: 0.1.3rc0
+Version: 0.1.3rc1
 Summary: useful utilities for prompt engineering
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Framework :: Pydantic :: 2
 Classifier: Topic :: Utilities
 Classifier: Topic :: File Formats :: JSON
@@ -118,18 +118,18 @@
 #### `count_token`
 
 count number of tokens in prompt
 
 ##### Usages
 
 ```py
-def count_token(prompt: str, enc: Encoding | None = None) -> int:
+def count_token(prompt: str | list[str], enc: Encoding | None = None) -> int:
 ```
 
-Provide your prompt, get its token count. The second parameter is the `tiktoken.Encoding` instance, will default to `get_encoding("cl100k_base")` if not provided.
+Provide your prompt / a list of prompts, get its token count. The second parameter is the `tiktoken.Encoding` instance, will default to `get_encoding("cl100k_base")` if not provided. The default `tiktoken.Encoding` instance is cached, and will not be re-created every time.
 
 ```py
 def count_token(prompt: dict | list[dict], enc: Encoding | None = None) -> int:
 ```
 
 Note that it can also be a single message / a list of messages. Every message should be a dict in the schema below:
 
@@ -153,14 +153,28 @@
 
 The output will be:
 
 ```py
 1
 ```
 
+##### List of plain texts
+
+```py
+from promptools.openai import count_token
+
+print(count_token(["hi", "hello"]))
+```
+
+The output will be:
+
+```py
+2
+```
+
 ###### Single message
 
 ```py
 from promptools.openai import count_token
 
 count_token({"role": "user", "content": "hi"})
 ```
```

