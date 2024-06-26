# Comparing `tmp/partial_json_parser-0.2.1.1.post1.tar.gz` & `tmp/partial_json_parser-0.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partial_json_parser-0.2.1.1.post1.tar", last modified: Mon May 13 18:02:44 2024, max compression
+gzip compressed data, was "partial_json_parser-0.2.1.post1.tar", last modified: Sat May 11 06:41:11 2024, max compression
```

## Comparing `partial_json_parser-0.2.1.1.post1.tar` & `partial_json_parser-0.2.1.post1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5774 2024-05-11 06:34:06.584003 partial_json_parser-0.2.1.1.post1/README.md
--rw-r--r--   0        0        0     1728 2024-05-13 18:02:44.113656 partial_json_parser-0.2.1.1.post1/pyproject.toml
--rw-r--r--   0        0        0      193 2024-05-13 14:56:25.317622 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/__init__.py
--rw-r--r--   0        0        0      860 2024-05-12 09:44:36.703555 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/api.py
--rw-r--r--   0        0        0     6990 2024-05-13 17:56:26.761359 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/complete.py
--rw-r--r--   0        0        0      150 2024-05-11 08:54:50.071644 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/exceptions.py
--rw-r--r--   0        0        0     9295 2024-05-13 14:57:12.051386 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/myelin.py
--rw-r--r--   0        0        0      992 2024-05-11 08:54:50.071644 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/options.py
--rw-r--r--   0        0        0      895 2024-05-13 12:00:07.250184 partial_json_parser-0.2.1.1.post1/src/partial_json_parser/playground.py
--rw-r--r--   0        0        0     6229 1970-01-01 00:00:00.000000 partial_json_parser-0.2.1.1.post1/PKG-INFO
+-rw-r--r--   0        0        0     5774 2024-05-11 06:34:06.584003 partial_json_parser-0.2.1.post1/README.md
+-rw-r--r--   0        0        0     1436 2024-05-11 06:41:11.487550 partial_json_parser-0.2.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     7753 2024-05-11 06:35:52.232447 partial_json_parser-0.2.1.post1/src/partial_json_parser/__init__.py
+-rw-r--r--   0        0        0      992 2024-04-03 08:20:30.049307 partial_json_parser-0.2.1.post1/src/partial_json_parser/options.py
+-rw-r--r--   0        0        0      885 2024-05-11 06:10:13.960124 partial_json_parser-0.2.1.post1/src/partial_json_parser/playground.py
+-rw-r--r--   0        0        0    19024 2024-05-10 15:51:01.796128 partial_json_parser-0.2.1.post1/tests/__pycache__/test_examples.cpython-312-pytest-7.4.4.pyo
+-rw-r--r--   0        0        0     4870 2024-05-10 15:51:01.804081 partial_json_parser-0.2.1.post1/tests/__pycache__/test_hypotheses.cpython-312-pytest-7.4.4.pyo
+-rw-r--r--   0        0        0     2662 2024-05-11 06:10:13.960124 partial_json_parser-0.2.1.post1/tests/test_examples.py
+-rw-r--r--   0        0        0     1332 2024-05-11 06:35:52.232447 partial_json_parser-0.2.1.post1/tests/test_hypotheses.py
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 partial_json_parser-0.2.1.post1/PKG-INFO
```

### Comparing `partial_json_parser-0.2.1.1.post1/README.md` & `partial_json_parser-0.2.1.post1/README.md`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.1.1.post1/pyproject.toml` & `partial_json_parser-0.2.1.post1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "partial-json-parser"
-version = "0.2.1.1.post1"
+version = "0.2.1.post1"
 description = "Parse partial JSON generated by LLM"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
+dependencies = []
 requires-python = ">=3.6"
 readme = "README.md"
 keywords = [
     "JSON",
     "parser",
     "LLM",
     "nlp",
@@ -35,61 +36,44 @@
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[tool.pdm.build]
-excludes = [
-    "tests",
-]
-
 [tool.pdm.dev-dependencies]
 dev = [
     "isort>=5.12.0",
     "black>=23.10.0",
     "hypothesis>=6.88.1",
     "tqdm>=4.66.1",
     "pytest>=7.4.2",
 ]
 
 [tool.pdm.scripts]
 test-examples = "pytest tests/test_examples.py"
-post_build = "python src/overrides.py 3.8"
-
-[tool.pdm.scripts.test-performance]
-call = "tests.test_performance:main"
 
 [tool.pdm.scripts.test-hypotheses]
 call = "tests.test_hypotheses:main"
 
 [tool.pdm.scripts.test]
 composite = [
     "test-examples",
     "test-hypotheses",
-    "test-performance",
 ]
 
 [tool.pdm.scripts.format]
 composite = [
     "isort ./{args}",
     "black ./{args}",
 ]
 
 [tool.pdm.scripts.playground]
 call = "partial_json_parser.playground:main"
 
 [tool.pdm.scripts.pre_build]
 composite = [
     "format",
-    "python src/overrides.py 3.6",
 ]
 
 [tool.black]
 line-length = 160
-
-[tool.isort]
-profile = "black"
-
-[tool.pyright]
-reportPossiblyUnboundVariable = false
```

### Comparing `partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/complete.py` & `partial_json_parser-0.2.1.post1/src/partial_json_parser/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,51 @@
-from typing import TYPE_CHECKING, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Tuple, Union
 
-from .exceptions import MalformedJSON, PartialJSON
 from .options import *
 
+Number = Union[int, float]
+JSON = Union[str, bool, Number, List["JSON"], Dict[str, "JSON"], None]
+
 if TYPE_CHECKING:
     from typing import Literal
 
 CompleteResult = Union[Tuple[int, Union[str, "Literal[True]"]], "Literal[False]"]  # (length, complete_string / already completed) / partial
 
 
-def fix(json_string: str, allow_partial: Union[Allow, int] = ALL):
-    """get the original slice and the trailing suffix separately"""
+class JSONDecodeError(ValueError):
+    pass
+
+
+class PartialJSON(JSONDecodeError):
+    pass
+
+
+class MalformedJSON(JSONDecodeError):
+    pass
+
+
+def parse_json(json_string: str, allow_partial: Union[Allow, int] = ALL, parser: Optional[Callable[[str], JSON]] = None) -> JSON:
+    if parser is None:
+        from json import loads as parser
+
+    return parser(ensure_json(json_string, allow_partial))
 
-    return _fix(json_string, Allow(allow_partial), True)
 
+def ensure_json(json_string: str, allow_partial: Union[Allow, int] = ALL):
+    """get the completed JSON string"""
+
+    head, tail = fix(json_string, allow_partial)
+    return head + tail
+
+
+def fix(json_string: str, allow_partial: Union[Allow, int] = ALL):
+    """get the original slice and the trailing suffix separately"""
 
-def _fix(json_string: str, allow: Allow, is_top_level=False):
     try:
-        result = complete_any(json_string.strip(), allow, is_top_level)
+        result = complete_any(json_string.strip(), Allow(allow_partial), is_top_level=True)
         if result is False:
             raise PartialJSON
 
         index, completion = result
         return json_string[:index], ("" if completion is True else completion)
 
     except (AssertionError, IndexError) as err:
@@ -230,7 +254,13 @@
         modified = True
         i -= 1
 
     if modified or i == length and not is_top_level:
         return (i, "") if NUM in allow else False
     else:
         return i, True
+
+
+loads = decode = parse_json
+
+
+__all__ = ["loads", "decode", "parse_json", "fix", "ensure_json", "JSONDecodeError", "PartialJSON", "MalformedJSON", "Allow", "JSON"]
```

### Comparing `partial_json_parser-0.2.1.1.post1/src/partial_json_parser/core/options.py` & `partial_json_parser-0.2.1.post1/src/partial_json_parser/options.py`

 * *Files identical despite different names*

### Comparing `partial_json_parser-0.2.1.1.post1/src/partial_json_parser/playground.py` & `partial_json_parser-0.2.1.post1/src/partial_json_parser/playground.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from rich.console import Console
 from rich.highlighter import JSONHighlighter
 from rich.style import Style
 from rich.text import Span
 
-from partial_json_parser import fix_fast
+from partial_json_parser import fix
 
 console = Console()
 highlight = JSONHighlighter()
 
 
 def main():
     while True:
         try:
             input_str = console.input("[d]>>> ")
 
-            head, tail = fix_fast(input_str)
+            head, tail = fix(input_str)
             json = head + tail
 
             rich_text = highlight(json)
             if tail:
                 rich_text.spans.append(Span(len(head), len(json), Style(dim=True)))
 
             console.print(" " * 3, rich_text)
```

### Comparing `partial_json_parser-0.2.1.1.post1/PKG-INFO` & `partial_json_parser-0.2.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: partial-json-parser
-Version: 0.2.1.1.post1
+Version: 0.2.1.post1
 Summary: Parse partial JSON generated by LLM
 Keywords: JSON,parser,LLM,nlp
 Home-page: https://promplate.dev/partial-json-parser
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

