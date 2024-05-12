# Comparing `tmp/foldedtensor-0.3.3.tar.gz` & `tmp/foldedtensor-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foldedtensor-0.3.3.tar", last modified: Wed Feb 14 22:15:11 2024, max compression
+gzip compressed data, was "foldedtensor-0.3.4.tar", last modified: Sun May 12 23:24:53 2024, max compression
```

## Comparing `foldedtensor-0.3.3.tar` & `foldedtensor-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:15:11.084773 foldedtensor-0.3.3/foldedtensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/foldedtensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/foldedtensor/functions.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/foldedtensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-02-14 22:15:11.000000 foldedtensor-0.3.3/foldedtensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-14 22:15:11.000000 foldedtensor-0.3.3/foldedtensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 22:15:11.000000 foldedtensor-0.3.3/foldedtensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-14 22:15:11.000000 foldedtensor-0.3.3/foldedtensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-14 22:15:11.000000 foldedtensor-0.3.3/foldedtensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/scripts/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 22:15:11.088774 foldedtensor-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/tests/test_folded_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-14 22:15:02.000000 foldedtensor-0.3.3/tests/test_multiprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:24:53.363340 foldedtensor-0.3.4/foldedtensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    13996 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/foldedtensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/foldedtensor/functions.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/foldedtensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-05-12 23:24:53.000000 foldedtensor-0.3.4/foldedtensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-12 23:24:53.000000 foldedtensor-0.3.4/foldedtensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 23:24:53.000000 foldedtensor-0.3.4/foldedtensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-12 23:24:53.000000 foldedtensor-0.3.4/foldedtensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-12 23:24:53.000000 foldedtensor-0.3.4/foldedtensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/scripts/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 23:24:53.367340 foldedtensor-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/tests/test_folded_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-12 23:24:48.000000 foldedtensor-0.3.4/tests/test_multiprocessing.py
```

### Comparing `foldedtensor-0.3.3/LICENSE` & `foldedtensor-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.3.3/PKG-INFO` & `foldedtensor-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedtensor
-Version: 0.3.3
+Version: 0.3.4
 Summary: PyTorch extension for handling deeply nested sequences of variable length
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2023 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -13,15 +13,15 @@
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/aphp/foldedtensor/
 Project-URL: repository, https://github.com/aphp/foldedtensor/
-Requires-Python: <4.0,>3.7.6
+Requires-Python: <4.0,>3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>1.0.0
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black==22.6.0; extra == "dev"
 Requires-Dist: pre-commit>=2.18; extra == "dev"
```

### Comparing `foldedtensor-0.3.3/README.md` & `foldedtensor-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.3.3/foldedtensor/__init__.py` & `foldedtensor-0.3.4/foldedtensor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,53 @@
 from multiprocessing.reduction import ForkingPickler
 from typing import List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import torch
 from torch.autograd import Function
 
+from . import _C
+
 np_to_torch_dtype = {
     torch.bool: bool,
     torch.uint8: np.uint8,
     torch.int8: np.int8,
     torch.int16: np.int16,
     torch.int32: np.int32,
     torch.int64: np.int64,
     torch.float16: np.float16,
     torch.float32: np.float32,
     torch.float64: np.float64,
     torch.complex64: np.complex64,
     torch.complex128: np.complex128,
 }
 
-from . import _C
+pass_through_functions = {
+    torch.Tensor._grad.__get__,
+    torch.Tensor.grad,
+    torch.Tensor._base.__get__,
+    torch.Tensor.__repr__,
+    torch.Tensor.__str__,
+    torch.Tensor.__format__,
+    torch.Tensor.shape.__get__,
+    torch.Tensor.size.__get__,
+    torch.Tensor.dtype.__get__,
+    torch.Tensor.device.__get__,
+}
+if hasattr(torch._C, "TensorBase"):
+    pass_through_functions.add(torch._C.TensorBase.size)
+else:
+    pass_through_functions.add(torch.Tensor.size)
+
+try:
+    DisableTorchFunctionSubclass = torch._C.DisableTorchFunctionSubclass
+except AttributeError:
+    DisableTorchFunctionSubclass = torch._C.DisableTorchFunction
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 
 
 # noinspection PyMethodOverriding
 class Refold(Function):
     @staticmethod
     def forward(
         ctx,
@@ -67,37 +89,29 @@
         # Perform inverse refolding, i.e., dims = old data_dims
         device = grad_output.device
         # full_names = grad_output.full_names
         np_new_indexer, shape_prefix = _C.make_refolding_indexer(
             ctx.lengths,
             ctx.old_data_dims,
         )
-        # new_data_flat.index_put_({new_indexer}, old_data_flat.index_select(0, old_indexer));
         shape_suffix = grad_output.shape[len(ctx.new_data_dims) :]
         grad_input = torch.zeros(
             (*shape_prefix, *shape_suffix), dtype=grad_output.dtype, device=device
         )
         grad_input.view(-1, *shape_suffix)[ctx.input_indexer] = grad_output.reshape(
             -1, *shape_suffix
         ).index_select(0, ctx.output_indexer)
         return grad_input, None
-        # return FoldedTensor(
-        #     data=refolded_data,
-        #     lengths=ctx.lengths,
-        #     data_dims=ctx.old_data_dims,
-        #     full_names=full_names,
-        #     indexer=indexer,
-        # )
 
 
 type_to_dtype_dict = {
-    int: torch.int64,
-    float: torch.float64,
+    int: torch.tensor([0]).dtype,
+    float: torch.tensor([0.0]).dtype,
     bool: torch.bool,
-    None: torch.float64,
+    None: torch.tensor([0.0]).dtype,
 }
 
 
 def get_metadata(nested_data):
     item = None
     deepness = 0
 
@@ -147,24 +161,26 @@
         if data_dims is not None:
             data_dims = tuple(
                 dim if isinstance(dim, int) else full_names.index(dim)
                 for dim in data_dims
             )
             if (data_dims[-1] + 1) != len(full_names):
                 raise ValueError(
-                    "The last dimension of `data_dims` must be the last variable dimension."
+                    "The last dimension of `data_dims` must be the last "
+                    "variable dimension."
                 )
         elif full_names is not None:
             data_dims = tuple(range(len(full_names)))
     if isinstance(data, torch.Tensor) and lengths is not None:
         data_dims = data_dims or tuple(range(len(lengths)))
         np_indexer, shape = _C.make_refolding_indexer(lengths, data_dims)
-        assert shape == list(
-            data.shape[: len(data_dims)]
-        ), f"Shape inferred from lengths is not compatible with data dims: {shape}, {data.shape}, {len(data_dims)}"
+        assert shape == list(data.shape[: len(data_dims)]), (
+            f"Shape inferred from lengths is not compatible with data dims: {shape}, "
+            f"{data.shape}, {len(data_dims)}"
+        )
         result = FoldedTensor(
             data=data,
             lengths=lengths,
             data_dims=data_dims,
             full_names=full_names,
             indexer=torch.from_numpy(np_indexer).to(data.device),
         )
@@ -204,14 +220,31 @@
             "- a `full_names` sequence of names for variable dimensions"
         )
     if device is not None:
         result = result.to(device)
     return result
 
 
+def _postprocess_func_result(result, input):
+    if (
+        input is not None
+        and input.shape[: len(input.data_dims)] != result.shape[: len(input.data_dims)]
+    ):
+        return result
+
+    return FoldedTensor(
+        data=result,
+        lengths=input.lengths,
+        data_dims=input.data_dims,
+        full_names=input.full_names,
+        indexer=input.indexer,
+        mask=input._mask,
+    )
+
+
 # noinspection PyUnresolvedReferences,PyInitNewSignature
 class FoldedTensor(torch.Tensor):
     """
     A FoldedTensor is an extension of Pytorch Tensors that provides operations for
     efficiently handling tensors containing deeply nested sequences variable sizes.
     It enables the flattening/unflattening (or unfolding/folding) of data dimensions
     based on a inner structure of sequence lengths. This library is particularly useful
@@ -292,54 +325,60 @@
                 mask=self._mask.to(result.device, copy=copy, non_blocking=non_blocking)
                 if self._mask is not None
                 else None,
             )
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
-        result = super().__torch_function__(func, types, args, kwargs)
+        if kwargs is None:
+            kwargs = {}
+        if func in pass_through_functions:
+            with DisableTorchFunctionSubclass():
+                return func(*args, **kwargs)
+        with DisableTorchFunctionSubclass():
+            result = func(*args, **kwargs)
 
         if func is torch.Tensor.share_memory_:
             self = args[0]
             self.indexer.share_memory_()
             if self._mask is not None:
                 self._mask.share_memory_()
-
-        if not isinstance(result, torch.Tensor):
-            return result
+            return self
 
         ft = None
-        for arg in (*args, *(kwargs or {}).values()):
+        for arg in (*args, *kwargs.values()):
             if isinstance(arg, FoldedTensor):
                 assert (
                     ft is None or ft.data_dims == arg.data_dims
-                ), "Cannot perform operation on FoldedTensors with different structure"
+                ), "Cannot perform operation on FoldedTensors with different structures"
                 ft = arg
-            if isinstance(arg, (list, tuple)):
+            elif isinstance(arg, (list, tuple)):
                 for item in arg:
                     if isinstance(item, FoldedTensor):
-                        assert (
-                            ft is None or ft.data_dims == item.data_dims
-                        ), "Cannot perform operation on FoldedTensors with different structure"
+                        assert ft is None or ft.data_dims == item.data_dims, (
+                            "Cannot perform operation on FoldedTensors with "
+                            "different structures"
+                        )
                         ft = item
 
+        if isinstance(result, torch.Tensor):
+            return _postprocess_func_result(result, ft)
+
         if (
-            ft is not None
-            and ft.shape[: len(ft.data_dims)] != result.shape[: len(ft.data_dims)]
+            isinstance(result, (tuple, list))
+            and len(result)
+            and isinstance(result[0], torch.Tensor)
         ):
-            return result.as_subclass(torch.Tensor)
+            return type(result)(
+                _postprocess_func_result(item, ft)
+                if isinstance(item, FoldedTensor)
+                else item
+                for item in result
+            )
 
-        result = FoldedTensor(
-            data=result,
-            lengths=ft.lengths,
-            data_dims=ft.data_dims,
-            full_names=ft.full_names,
-            indexer=ft.indexer,
-            mask=ft._mask,
-        )
         return result
 
     def clone(self):
         cloned = super().clone()
         cloned.indexer = self.indexer.clone()
         if self._mask is not None:
             cloned._mask = self._mask.clone()
```

### Comparing `foldedtensor-0.3.3/foldedtensor/functions.cpp` & `foldedtensor-0.3.4/foldedtensor/functions.cpp`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.3.3/foldedtensor.egg-info/PKG-INFO` & `foldedtensor-0.3.4/foldedtensor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foldedtensor
-Version: 0.3.3
+Version: 0.3.4
 Summary: PyTorch extension for handling deeply nested sequences of variable length
 Author-email: Perceval Wajsbürt <perceval.wajsburt-ext@aphp.fr>
 License: Copyright 2023 Assistance Publique - Hôpitaux de Paris
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
@@ -13,15 +13,15 @@
         
         3. Neither the name of the copyright holder nor the names of its contributors may be used to endorse or promote products derived from this software without specific prior written permission.
         
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/aphp/foldedtensor/
 Project-URL: repository, https://github.com/aphp/foldedtensor/
-Requires-Python: <4.0,>3.7.6
+Requires-Python: <4.0,>3.7.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>1.0.0
 Requires-Dist: numpy
 Provides-Extra: dev
 Requires-Dist: black==22.6.0; extra == "dev"
 Requires-Dist: pre-commit>=2.18; extra == "dev"
```

### Comparing `foldedtensor-0.3.3/pyproject.toml` & `foldedtensor-0.3.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     { name = "Perceval Wajsbürt", email = "perceval.wajsburt-ext@aphp.fr" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 urls.homepage = "https://github.com/aphp/foldedtensor/"
 urls.repository = "https://github.com/aphp/foldedtensor/"
 dynamic = ["version"]
-requires-python = ">3.7.6,<4.0"
+requires-python = ">3.7.1,<4.0"
 
 dependencies = [
     "torch>1.0.0",
     "numpy",
 ]
 
 [project.optional-dependencies]
@@ -78,15 +78,14 @@
 ]
 
 [tool.ruff]
 fix = true
 exclude = [
     ".git",
     "__pycache__",
-    "__init__.py",
     ".mypy_cache",
     ".pytest_cache",
     ".venv",
     "build",
 ]
 ignore = []
 line-length = 88
@@ -94,9 +93,10 @@
     "E",
     "F",
     "W",
     "I001"
 ]
 fixable = ["E", "F", "W", "I"]
 
-[isort]
-known-first-party = ["foldedtensor"]
+[tool.ruff.isort]
+    known-first-party = ["foldedtensor"]
+    known-third-party = ["build"]
```

### Comparing `foldedtensor-0.3.3/scripts/benchmark.py` & `foldedtensor-0.3.4/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `foldedtensor-0.3.3/tests/test_folded_tensor.py` & `foldedtensor-0.3.4/tests/test_folded_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,7 +400,20 @@
                 [0, 1, 2],
                 3,
             ],
             dtype=torch.float,
         )
 
     assert "'int' object is not iterable" in str(e.value)
+
+
+def test_max():
+    ft = as_folded_tensor(
+        [
+            [0, 1, 2],
+            [3, 4],
+        ],
+        dtype=torch.float,
+    )
+    values, indices = ft.max(-1)
+    assert (values == torch.tensor([2, 4])).all()
+    assert (indices == torch.tensor([2, 1])).all()
```

### Comparing `foldedtensor-0.3.3/tests/test_multiprocessing.py` & `foldedtensor-0.3.4/tests/test_multiprocessing.py`

 * *Files identical despite different names*

