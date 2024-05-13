# Comparing `tmp/nadl-1.0.2.tar.gz` & `tmp/nadl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.0.2.tar", last modified: Wed May  8 04:41:17 2024, max compression
+gzip compressed data, was "nadl-1.1.0.tar", last modified: Mon May 13 05:07:28 2024, max compression
```

## Comparing `nadl-1.0.2.tar` & `nadl-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     2243 2024-05-08 04:41:17.804169 nadl-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.0.2/readme.org
--rw-r--r--   0        0        0     1665 2024-05-08 04:40:44.028812 nadl-1.0.2/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.0.2/src/nadl/blocks.py
--rw-r--r--   0        0        0     3034 2024-05-08 04:39:50.114195 nadl-1.0.2/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.0.2/src/nadl/images.py
--rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.0.2/src/nadl/keys.py
--rw-r--r--   0        0        0     3696 2024-04-22 06:27:20.032703 nadl-1.0.2/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.0.2/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.0.2/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.0.2/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.0.2/src/nadl/py.typed
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.0.2/src/nadl/transformers.py
--rw-r--r--   0        0        0     1964 2024-04-22 04:28:48.528308 nadl-1.0.2/src/nadl/utils.py
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 nadl-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2243 2024-05-13 05:07:28.664880 nadl-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.1.0/readme.org
+-rw-r--r--   0        0        0     1665 2024-05-13 05:06:19.700554 nadl-1.1.0/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.1.0/src/nadl/blocks.py
+-rw-r--r--   0        0        0     3550 2024-05-13 05:02:54.634502 nadl-1.1.0/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.1.0/src/nadl/images.py
+-rw-r--r--   0        0        0     3170 2024-04-22 06:27:49.753850 nadl-1.1.0/src/nadl/keys.py
+-rw-r--r--   0        0        0     3696 2024-04-22 06:27:20.032703 nadl-1.1.0/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.1.0/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.1.0/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.1.0/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.1.0/src/nadl/py.typed
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.1.0/src/nadl/transformers.py
+-rw-r--r--   0        0        0     1964 2024-04-22 04:28:48.528308 nadl-1.1.0/src/nadl/utils.py
+-rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 nadl-1.1.0/PKG-INFO
```

### Comparing `nadl-1.0.2/pyproject.toml` & `nadl-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 description = "Nasy's Deep Learning Toolkit"
 authors = [
     { name = "Nasy", email = "nasyxx+python@gmail.com" },
     { name = "Nasy", email = "nasyxx+dl@gmail.com" },
     { name = "Nasy", email = "nasyxx+git@gmail.com" },
 ]
 dependencies = [
-    "jax>=0.4.26",
+    "jax>=0.4.28",
     "numpy>=1.26.4",
     "rich>=13.7.1",
     "jaxtyping>=0.2.28",
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
 ]
-requires-python = ">=3.11"
-version = "1.0.2"
+requires-python = ">=3.12"
+version = "1.1.0"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
 
 [project.optional-dependencies]
 doc = [
-    "mkdocs-material>=9.5.18",
-    "mkdocs>=1.5.3",
-    "mike>=2.0.0",
-    "mkdocstrings[python]>=0.24.3",
+    "mkdocs-material>=9.5.22",
+    "mkdocs>=1.6.0",
+    "mike>=2.1.1",
+    "mkdocstrings[python]>=0.25.1",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
@@ -93,15 +93,15 @@
 implicit_reexport = true
 strict_equality = true
 strict = true
 warn_unused_configs = true
 mypy_path = "./typings"
 
 [tool.pyright]
-pythonVersion = "3.11"
+pythonVersion = "3.12"
 extraPaths = [
     "__pypackages__/3.12/lib",
     "src",
     "__pypackages__/3.11/lib",
 ]
 exclude = [
     "**/__pycache__",
```

### Comparing `nadl-1.0.2/readme.org` & `nadl-1.1.0/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/__init__.py` & `nadl-1.1.0/src/nadl/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 )
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.0.2"
+__version__ = "1.1.0"
 
 __all__ = [
   "PG",
   "SCALER",
   "DState",
   "IdxDataloader",
   "Keys",
```

### Comparing `nadl-1.0.2/src/nadl/blocks.py` & `nadl-1.1.0/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/data.py` & `nadl-1.1.0/src/nadl/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,90 +31,99 @@
 filename : data.py
 project  : nadl
 license  : GPL-3.0+
 
 Simple dataset and dataloader.
 """
 
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from .keys import Keys
 from typing import NamedTuple
 
 
-class DState(NamedTuple):
+class DState[T](NamedTuple):
   """Dataloader state."""
 
-  idx: jax.Array
+  xs: T
   pad: int | None = None
 
 
-class IdxDataloader(eqx.Module):
+class IdxDataloader[T](eqx.Module):
   """Simple index dataloader.
 
   Provide indexes only for datasets.
   """
 
   length: int
   key: Keys
   batch_size: int = 1
   shuffle: bool = False
   drop_last: bool = False
   auto_pad: bool = True
+  transform: Callable[[jax.Array], T] | None = None
 
   def __init__(
     self,
     length: int,
     batch_size: int = 1,
     shuffle: bool = False,
     drop_last: bool = False,
     auto_pad: bool = False,
     key: jax.Array | None = None,
+    transform: Callable[[jax.Array], T] | None = None,
   ) -> None:
     """Initiate the dataloader."""
     self.length = length
     self.batch_size = batch_size
     self.shuffle = shuffle
     self.drop_last = drop_last
     self.auto_pad = auto_pad
     self.key = Keys.from_int_or_key(key or 42)
+    self.transform = transform
 
-  def __call__(self, ki: int) -> Iterator[DState]:
+  def __call__(self, ki: int) -> Iterator[DState[T]]:
     """Get the indexes."""
     idxes = (
       jax.random.permutation(self.key(ki)[1], self.length)
       if self.shuffle
       else jnp.arange(self.length)
     )
-    if self.drop_last:
-      length = self.length - self.length % self.batch_size
-      idxes = idxes[:length]
-      pad = 0
-
-    pad = self.batch_size - len(idxes) % self.batch_size
-    if 0 < pad < self.batch_size:
-      idxes = jnp.r_[idxes, jnp.zeros(pad, idxes.dtype)]
-    if pad == self.batch_size:
-      pad = 0
-    idxes = idxes.reshape(-1, self.batch_size)
-
-    for i, idx in enumerate(idxes):
-      if pad and i >= idxes.shape[0] - 1:
-        if self.auto_pad:
-          yield DState(idx, pad)
-        else:
-          yield DState(idx[:-pad], 0)
-      else:
-        yield DState(idx, 0)
+    length = (
+      self.length if not self.drop_last else self.length - self.length % self.batch_size
+    )
+
+    pad = (
+      (self.batch_size - r) % self.batch_size if (r := length % self.batch_size) else 0
+    )
+    pad = pad if pad != self.batch_size else 0
+
+    if pad:
+      idxes = jnp.r_[idxes, jnp.full(pad, -1, idxes.dtype)]  # padding placeholder
+
+    idxes = idxes[:length + pad].reshape(-1, self.batch_size)
+
+    for i in idxes:
+      ii = i
+      if pad and not self.auto_pad and (ii == -1).any():
+        ii = ii[ii != -1]
+      xs = self.transform(ii) if self.transform else ii
+      yield DState(xs, pad if ((ii == -1).any() and self.auto_pad) else None)
 
 
 def __test() -> None:
   """Test."""
   dl = IdxDataloader(10, 3, shuffle=True, drop_last=False, auto_pad=True)
   for i, state in enumerate(dl(42)):
-    print(i, state.idx, state.pad)
+    print(i, state.xs, state.pad)
+  dl = IdxDataloader(10, 3, shuffle=True, drop_last=False, auto_pad=False)
+  for i, state in enumerate(dl(42)):
+    print(i, state.xs, state.pad)
+  dl = IdxDataloader(10, 3, shuffle=False, drop_last=True, auto_pad=False)
+  for i, state in enumerate(dl(42)):
+    print(i, state.xs, state.pad)
 
 
 if __name__ == "__main__":
   __test()
```

### Comparing `nadl-1.0.2/src/nadl/images.py` & `nadl-1.1.0/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/keys.py` & `nadl-1.1.0/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/loops.py` & `nadl-1.1.0/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/metrics.py` & `nadl-1.1.0/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/nets.py` & `nadl-1.1.0/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/preprocessing.py` & `nadl-1.1.0/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/transformers.py` & `nadl-1.1.0/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/src/nadl/utils.py` & `nadl-1.1.0/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.0.2/PKG-INFO` & `nadl-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.0.2
+Version: 1.1.0
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
-Requires-Python: >=3.11
-Requires-Dist: jax>=0.4.26
+Requires-Python: >=3.12
+Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: optax>=0.2.2
 Requires-Dist: equinox>=0.11.4
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: scikit-image>=0.23.2
-Requires-Dist: mkdocs-material>=9.5.18; extra == "doc"
-Requires-Dist: mkdocs>=1.5.3; extra == "doc"
-Requires-Dist: mike>=2.0.0; extra == "doc"
-Requires-Dist: mkdocstrings[python]>=0.24.3; extra == "doc"
+Requires-Dist: mkdocs-material>=9.5.22; extra == "doc"
+Requires-Dist: mkdocs>=1.6.0; extra == "doc"
+Requires-Dist: mike>=2.1.1; extra == "doc"
+Requires-Dist: mkdocstrings[python]>=0.25.1; extra == "doc"
 Provides-Extra: doc
 Description-Content-Type: text/plain
 
 #+options: ':nil *:t -:t ::t <:t H:3 \n:nil ^:{} arch:headline
 #+options: author:t broken-links:mark c:nil creator:nil
 #+options: d:(not "LOGBOOK") date:t e:t email:nil f:t inline:t num:t
 #+options: p:nil pri:nil prop:nil stat:t tags:t tasks:t tex:t
```

