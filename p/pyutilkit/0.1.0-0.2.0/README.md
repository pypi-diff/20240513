# Comparing `tmp/pyutilkit-0.1.0.tar.gz` & `tmp/pyutilkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyutilkit-0.1.0.tar", max compression
+gzip compressed data, was "pyutilkit-0.2.0.tar", max compression
```

## Comparing `pyutilkit-0.1.0.tar` & `pyutilkit-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1477 2024-05-12 17:26:27.967790 pyutilkit-0.1.0/docs/README.md
--rw-r--r--   0        0        0     2966 2024-05-12 17:26:28.644365 pyutilkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-12 17:26:27.967790 pyutilkit-0.1.0/src/pyutilkit/__init__.py
--rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.1.0/src/pyutilkit/classes.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.1.0/src/pyutilkit/data/__init__.py
--rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.1.0/src/pyutilkit/data/timezones.py
--rw-r--r--   0        0        0     1821 2024-05-12 17:26:28.644365 pyutilkit-0.1.0/src/pyutilkit/date_utils.py
--rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.1.0/src/pyutilkit/py.typed
--rw-r--r--   0        0        0     2190 2024-05-12 17:26:28.234420 pyutilkit-0.1.0/src/pyutilkit/term.py
--rw-r--r--   0        0        0     1073 2024-05-12 17:26:28.377734 pyutilkit-0.1.0/src/pyutilkit/timing.py
--rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pyutilkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7696 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1477 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/docs/README.md
+-rw-r--r--   0        0        0     2994 2024-05-13 16:52:54.889471 pyutilkit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-13 16:53:00.422686 pyutilkit-0.2.0/src/pyutilkit/__init__.py
+-rw-r--r--   0        0        0      462 2024-05-12 17:26:28.511050 pyutilkit-0.2.0/src/pyutilkit/classes.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/data/__init__.py
+-rw-r--r--   0        0        0     3866 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/data/timezones.py
+-rw-r--r--   0        0        0     1821 2024-05-12 17:26:28.644365 pyutilkit-0.2.0/src/pyutilkit/date_utils.py
+-rw-r--r--   0        0        0     1523 2024-05-13 16:50:53.492051 pyutilkit-0.2.0/src/pyutilkit/files.py
+-rw-r--r--   0        0        0        0 2024-05-12 17:26:27.967790 pyutilkit-0.2.0/src/pyutilkit/py.typed
+-rw-r--r--   0        0        0     2895 2024-05-13 16:50:11.949600 pyutilkit-0.2.0/src/pyutilkit/term.py
+-rw-r--r--   0        0        0     1073 2024-05-12 17:26:28.377734 pyutilkit-0.2.0/src/pyutilkit/timing.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 pyutilkit-0.2.0/PKG-INFO
```

### Comparing `pyutilkit-0.1.0/LICENSE.md` & `pyutilkit-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.1.0/docs/README.md` & `pyutilkit-0.2.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.1.0/pyproject.toml` & `pyutilkit-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "pyutilkit"
-version = "0.1.0"
+version = "0.2.0"
 description = "python's missing batteries"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "docs/README.md"
@@ -157,14 +157,15 @@
 pickleshare = { version = "^0.7", python = "^3.10" }
 pipdeptree = "^2.13"
 
 [tool.poetry.group.lint.dependencies]
 black = "^24.1"
 mypy = "^1.8"
 ruff = "^0.4"
+typing_extensions = "^4.11"
 
 [tool.poetry.group.test.dependencies]
 freezegun = "^1.5"
 pytest = "^8.0"
 pytest-cov = "^5.0"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `pyutilkit-0.1.0/src/pyutilkit/data/timezones.py` & `pyutilkit-0.2.0/src/pyutilkit/data/timezones.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.1.0/src/pyutilkit/date_utils.py` & `pyutilkit-0.2.0/src/pyutilkit/date_utils.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.1.0/src/pyutilkit/term.py` & `pyutilkit-0.2.0/src/pyutilkit/term.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import os
 from collections.abc import Iterable
 from enum import IntEnum, unique
 from math import ceil, floor
-from typing import Any
+from typing import TYPE_CHECKING, Any
+
+if TYPE_CHECKING:
+    from typing_extensions import Self  # py3.10: import from typing
 
 
 @unique
 class SGRCodes(IntEnum):
     RESET = 0
 
     BOLD = 1
@@ -56,41 +59,58 @@
 
     @property
     def sequence(self) -> str:
         return f"\033[{self.value}m"
 
 
 class SGRString(str):
-    _sgr: str
-    __slots__ = ("_sgr",)
-
-    def __new__(cls, value: Any, *, params: Iterable[SGRCodes] = ()) -> SGRString:
-        string = super().__new__(cls, value)
-        suffix = SGRCodes.RESET.sequence
-        prefix = "".join(param.sequence for param in params) or SGRCodes.RESET.sequence
-        object.__setattr__(string, "_sgr", f"{prefix}{value}{suffix}")
+    _sgr: tuple[SGRCodes, ...]
+    _string: str
+    __slots__ = ("_sgr", "_string")
+
+    def __new__(cls, obj: Any, *, params: Iterable[SGRCodes] = ()) -> Self:
+        string = super().__new__(cls, obj)
+        object.__setattr__(string, "_string", str(obj))
+        object.__setattr__(string, "_sgr", tuple(params))
         return string
 
     def __setattr__(self, name: str, value: Any) -> None:
         msg = "SGRString is immutable"
         raise AttributeError(msg)
 
     def __delattr__(self, name: str) -> None:
         msg = "SGRString is immutable"
         raise AttributeError(msg)
 
     def __str__(self) -> str:
-        return self._sgr
-
-
-def header(
-    text: str, *, padding: str = " ", left_spaces: int = 1, right_spaces: int = 1
-) -> None:
-    columns = os.get_terminal_size().columns
-    text = f"{' ' * left_spaces}{text.strip()}{' ' * right_spaces}"
-    title_length = len(text)
-    if title_length >= columns:
-        print(text.strip())
-        return
+        if not self._sgr:
+            return self._string
+        prefix = "".join(code.sequence for code in self._sgr)
+        return f"{prefix}{self._string}{SGRCodes.RESET.sequence}"
+
+    def __mul__(self, other: Any) -> Self:
+        if not isinstance(other, int):
+            return NotImplemented
+        return type(self)(self._string * other, params=self._sgr)
+
+    def __rmul__(self, other: Any) -> Self:
+        if not isinstance(other, int):
+            return NotImplemented
+        return type(self)(self._string * other, params=self._sgr)
+
+    def header(
+        self,
+        *,
+        padding: str = " ",
+        left_spaces: int = 1,
+        right_spaces: int = 1,
+        space: str = " ",
+    ) -> None:
+        columns = os.get_terminal_size().columns
+        text = f"{space * left_spaces}{self}{space * right_spaces}"
+        title_length = left_spaces + len(self) + right_spaces
+        if title_length >= columns:
+            print(text.strip())
+            return
 
-    half = (columns - len(text)) / 2
-    print(f"{padding * ceil(half)}{text}{padding * floor(half)}")
+        half = (columns - title_length) / 2
+        print(f"{padding * ceil(half)}{text}{padding * floor(half)}")
```

### Comparing `pyutilkit-0.1.0/src/pyutilkit/timing.py` & `pyutilkit-0.2.0/src/pyutilkit/timing.py`

 * *Files identical despite different names*

### Comparing `pyutilkit-0.1.0/PKG-INFO` & `pyutilkit-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyutilkit
-Version: 0.1.0
+Version: 0.2.0
 Summary: python's missing batteries
 Home-page: https://pyutilkit.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: utils
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.8,<4.0
```

