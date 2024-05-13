# Comparing `tmp/openelm_pytorch-0.1.0.tar.gz` & `tmp/openelm_pytorch-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openelm_pytorch-0.1.0.tar", last modified: Mon May 13 14:31:48 2024, max compression
+gzip compressed data, was "openelm_pytorch-0.1.0rc1.tar", last modified: Fri May 10 22:20:40 2024, max compression
```

## Comparing `openelm_pytorch-0.1.0.tar` & `openelm_pytorch-0.1.0rc1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.349974 openelm_pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.337974 openelm_pytorch-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.341974 openelm_pytorch-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 14:31:48.349974 openelm_pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.341974 openelm_pytorch-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/examples/generate_text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.341974 openelm_pytorch-0.1.0/examples/train_lora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/examples/train_lora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13447 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/examples/train_lora/gutenberg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/examples/train_lora/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.341974 openelm_pytorch-0.1.0/openelm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/openelm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/openelm_pytorch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/openelm_pytorch/openelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/openelm_pytorch/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/openelm_pytorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.345974 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 14:31:48.000000 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-13 14:31:48.000000 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:31:48.000000 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-13 14:31:48.000000 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 14:31:48.000000 openelm_pytorch-0.1.0/openelm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:31:48.349974 openelm_pytorch-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:48.345974 openelm_pytorch-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    25644 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/openelm_mlx.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    13940 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/test_openelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 14:31:41.000000 openelm_pytorch-0.1.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.273783 openelm_pytorch-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.265783 openelm_pytorch-0.1.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.265783 openelm_pytorch-0.1.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-10 22:20:40.273783 openelm_pytorch-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.265783 openelm_pytorch-0.1.0rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/examples/generate_text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.265783 openelm_pytorch-0.1.0rc1/examples/train_lora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/examples/train_lora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14156 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/examples/train_lora/gutenberg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14120 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/examples/train_lora/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.269783 openelm_pytorch-0.1.0rc1/openelm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch/openelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.273783 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-10 22:20:40.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-10 22:20:40.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 22:20:40.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-10 22:20:40.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-10 22:20:40.000000 openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 22:20:40.273783 openelm_pytorch-0.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:40.269783 openelm_pytorch-0.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25644 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/openelm_mlx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/test_openelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-10 22:20:33.000000 openelm_pytorch-0.1.0rc1/tests/utils.py
```

### Comparing `openelm_pytorch-0.1.0/.github/workflows/publish.yaml` & `openelm_pytorch-0.1.0rc1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/.github/workflows/test.yaml` & `openelm_pytorch-0.1.0rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/.gitignore` & `openelm_pytorch-0.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/LICENSE` & `openelm_pytorch-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/PKG-INFO` & `openelm_pytorch-0.1.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: openelm-pytorch
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: openelm-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: einops<1,>=0.7.0
 Requires-Dist: safetensors<1,>=0.4.0
 Requires-Dist: torch<3.0,>=2.0
 Provides-Extra: mlx
 Requires-Dist: mlx<1,>=0.10.0; extra == "mlx"
 Provides-Extra: train
-Requires-Dist: lora-pytorch~=0.2.0; extra == "train"
+Requires-Dist: lora-pytorch~=0.1.0; extra == "train"
 Requires-Dist: lightning~=2.2.0; extra == "train"
 Requires-Dist: tensorboard~=2.14.0; extra == "train"
+Requires-Dist: torchdata~=0.7.0; extra == "train"
 Requires-Dist: tqdm; extra == "train"
 Provides-Extra: test
 Requires-Dist: black==24.4.2; extra == "test"
 Requires-Dist: mlx==0.10.0; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: numpy==1.26.4; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
```

### Comparing `openelm_pytorch-0.1.0/README.md` & `openelm_pytorch-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/examples/train_lora/gutenberg.py` & `openelm_pytorch-0.1.0rc1/examples/train_lora/gutenberg.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 from pathlib import Path
-from typing import Generator, Generic, List, Literal, TypeVar
+from typing import Generator, List, Literal, Optional
 
 import requests
 from torch.hub import get_dir
-from torch.utils.data import IterableDataset
+from torchdata.datapipes.iter import IterableWrapper, IterDataPipe
 
 CACHE_DIR = Path(get_dir()) / "gutenberg"
 CACHE_DIR.mkdir(exist_ok=True)
 GUTENBERG_TOP_100_URLS = [
     # Romeo and Juliet by William Shakespeare
     "https://www.gutenberg.org/ebooks/1513.txt.utf-8",
     # Moby Dick; Or The Whale by Herman Melville
@@ -234,42 +234,20 @@
         out = indices[num_val : num_val + num_test]
     else:
         raise ValueError(f"Invalid split: {split}")
 
     return sorted(out)
 
 
-T = TypeVar("T")
-
-
-class ShuffleBuffer(Generic[T]):
-    def __init__(self, buffer_size: int):
-        self.buffer_size = buffer_size
-        self.buffer: list[T] = []
-
-    def add(self, item: T) -> None:
-        if len(self.buffer) > self.buffer_size:
-            self.buffer.pop(0)
-
-
-class GutenbergEBookDataset(IterableDataset):
-    def __init__(
-        self,
-        split: Literal["train", "val", "test"],
-        chunk_size: int = 4096,
-        drop_last: bool = False,
-    ):
-        self.split = split
-        self.chunk_size = chunk_size
-        self.drop_last = drop_last
+class GutenbergEBookLoader(IterDataPipe[str]):
+    def __init__(self, dp: IterDataPipe[str]):
+        self.dp = dp
 
     def __iter__(self) -> Generator[str, None, None]:
-        indices = get_split_indices(len(GUTENBERG_TOP_100_URLS), split=self.split)
-        for i in indices:
-            url = GUTENBERG_TOP_100_URLS[i]
+        for url in self.dp:
             cache_path = CACHE_DIR / Path(url).name
             if not cache_path.exists():
                 resp = requests.get(url)
                 try:
                     resp.raise_for_status()
                 except requests.exceptions.HTTPError:
                     continue
@@ -282,15 +260,59 @@
                 with open(cache_path, "w") as f:
                     f.write(text)
 
             else:
                 with open(cache_path, "r") as f:
                     text = f.read()
 
-            for i in range(0, len(text), self.chunk_size):
+            yield text
+
+
+class TextChunker(IterDataPipe[str]):
+    def __init__(
+        self,
+        dp: IterDataPipe[str],
+        chunk_size: int = 4096,
+        step_size: Optional[int] = None,
+        drop_last: bool = False,
+    ):
+        self.dp = dp
+        self.chunk_size = chunk_size
+        self.step_size = step_size or chunk_size
+        self.drop_last = drop_last
+
+    def __iter__(self) -> Generator[str, None, None]:
+        for text in self.dp:
+            for i in range(0, len(text), self.step_size):
                 chunk = text[i : i + self.chunk_size]
                 if self.drop_last and len(chunk) < self.chunk_size:
-                    break
+                    continue
+
                 chunk = chunk.split(" ", maxsplit=1)[-1]  # leading partial words
                 chunk = chunk.rsplit(" ", maxsplit=1)[0]  # trailing partial words
                 chunk = chunk.strip()  # leading/trailing whitespace
                 yield chunk
+
+
+def project_gutenberg_top_100_datapipe(
+    split: Literal["train", "val", "test"],
+    chunk_size: int = 4096,
+    step_size: Optional[int] = None,
+    shuffle: bool = False,
+    shuffle_buffer_size: int = 8192,
+    drop_last: bool = True,
+) -> IterDataPipe[str]:
+    indices = get_split_indices(len(GUTENBERG_TOP_100_URLS), split=split)
+    if shuffle:
+        random.shuffle(indices)
+
+    # Iterable datapipe of ebook URLs (ebooks are UTF-8 text files)
+    pipe: IterDataPipe = IterableWrapper([GUTENBERG_TOP_100_URLS[i] for i in indices])
+    pipe = GutenbergEBookLoader(pipe)
+    pipe = TextChunker(
+        pipe, chunk_size=chunk_size, step_size=step_size, drop_last=drop_last
+    )
+    pipe = pipe.sharding_filter()
+    if shuffle:
+        pipe = pipe.shuffle(buffer_size=shuffle_buffer_size)
+
+    return pipe
```

### Comparing `openelm_pytorch-0.1.0/examples/train_lora/train.py` & `openelm_pytorch-0.1.0rc1/examples/train_lora/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from dataclasses import dataclass
 from functools import partial
-from typing import Any, Callable, Literal, Sequence
+from typing import Any, Callable, Iterator, Literal, Sequence
 
 import torch
 from lightning import Fabric, seed_everything
 from lightning.fabric.loggers import TensorBoardLogger
 from lightning.fabric.strategies import DDPStrategy
 from lora_pytorch import LoRA
 from torch import Tensor
@@ -14,18 +14,23 @@
 from torch.utils.data import DataLoader
 from tqdm import tqdm
 
 from openelm_pytorch.openelm import OpenELM
 from openelm_pytorch.tokenizer import Tokenizer
 from openelm_pytorch.utils import get_torch_device
 
-from ..generate_text import PROMPT, generate
-from .gutenberg import GutenbergEBookDataset
+from .gutenberg import project_gutenberg_top_100_datapipe
 
 torch.set_float32_matmul_precision("medium")
+# From "The Treasure Island" by R.L.Stevenson, public domain.
+EVAL_PROMPT = (
+    "Squire Trelawney, Dr. Livesey, and the rest of these gentlemen having "
+    "asked me to write down the whole particulars about Treasure Island, "
+    "from the"
+)
 
 
 def collate_fn(
     batch: Sequence[str],
     tokenizer: Tokenizer,
     max_length: int = 1024,
     device: torch.device | str | None = None,
@@ -187,14 +192,15 @@
 
 
 def train(
     model: LoRA[OpenELM],
     train_dataloader: DataLoader,
     val_dataloader: DataLoader,
     accelerator: str = "auto",
+    strategy: str = "auto",
     precision: str | None = None,
     epochs: int = 10,
     lr: float = 1e-4,
     lr_warmup_steps: int = 250,
     accumulate_grad_batches: int = 1,
     log_frequency: int = 25,
 ):
@@ -240,67 +246,120 @@
             state=state,
             train_dataloader=train_dataloader,
             val_dataloader=val_dataloader,
             log_frequency=log_frequency,
         )
 
 
+def generate(
+    model: OpenELM | LoRA[OpenELM],
+    tokenizer: Tokenizer,
+    prompt: str,
+    max_new_tokens: int = 4096,
+    top_k: int = 10,
+    temperature: float = 1.0,
+    seed: int = 42,
+) -> Iterator[str]:
+    seed_everything(seed)
+    device = next(iter(model.parameters())).device
+    temperature = max(temperature, 1e-8)
+    is_training = model.training
+    model.eval()
+
+    print("Generating text...")
+    input_ids = tokenizer([prompt]).to(device)
+    tokens = input_ids[0].tolist()  # For decoding text later.
+
+    with torch.inference_mode():
+        outputs = model.forward(input_ids, use_kv_cache=True)
+        token = outputs["logits"][0, -1].argmax().item()
+        cache = outputs["past_key_values"]
+        tokens.append(token)
+
+        for i in range(max_new_tokens):
+            outputs = model.forward(
+                input_ids=torch.tensor([[token]], device=device),
+                past_key_values=cache,
+                use_kv_cache=True,
+            )
+            logits, cache = outputs["logits"], outputs["past_key_values"]
+            probs = torch.softmax(logits[0, -1] / temperature, dim=-1)
+            # Get top-k tokens, renormalize their probabilities, and weighted sample.
+            token_ids: Tensor  # for mypy
+            probs, token_ids = probs.topk(k=top_k, dim=-1)
+            probs /= probs.sum()
+            # Take weighted random sample from the top-k tokens.
+            sampled_idx: int = torch.multinomial(probs, num_samples=1).item()  # type: ignore
+            token: int = token_ids[sampled_idx].item()  # type: ignore
+
+            tokens.append(token)
+            if i % 5 == 0:
+                yield tokenizer.decode(tokens)
+
+    # Restore the model's original training state.
+    model.train(mode=is_training)
+
+
 def main(
     model_name: str,
     tokenizer_path: str,
     model_checkpoint: str | None = None,
     accelerator: str = "auto",
     precision: str | None = None,
     epochs: int = 3,
-    lr: float = 1e-5,
-    lr_warmup_steps: int = 100,
-    batch_size: int = 64,
+    lr: float = 1e-4,
+    lr_warmup_steps: int = 250,
+    batch_size: int = 16,
     accumulate_grad_batches: int = 1,
     log_frequency: int = 25,
     seed: int = 42,
     eval_only: bool = False,
-    eval_prompt: str = PROMPT,
+    eval_prompt: str = EVAL_PROMPT,
     eval_max_tokens: int = 1024,
 ):
     seed_everything(seed)
     # config = ModelConfig.from_name(model_name)
     # model = OpenELM.from_config(config)
     # model = OpenELM.from_pretrained(model_name)
     # model = LoRA.from_module(OpenELM.from_config(config), rank=5)
     model = OpenELM.from_pretrained(model_name)
     tokenizer = Tokenizer.from_file(tokenizer_path)
 
     if not eval_only:
         # NOTE: Only initialize the LoRA model if training has been requested.
-        lora_model = LoRA.from_module(model, rank=5)
+        lora_model = LoRA.from_module(model, rank=16)
         if model_checkpoint is not None:
             lora_model.load_state_dict(
                 ModelCheckpoint.load(model_checkpoint).state_dict
             )
 
         num_devices = torch.cuda.device_count()
         if num_devices > 0:
             # Lightning Fabric does not scale the batch size for distributed training.
             # In order to keep batch size the same, divide by the number of devices.
             if batch_size % num_devices != 0:
                 raise ValueError(f"{batch_size=} must be divisible by {num_devices=}.")
             batch_size = batch_size // num_devices
 
         train_dataloader = DataLoader(
-            GutenbergEBookDataset(
+            project_gutenberg_top_100_datapipe(
                 split="train",
                 chunk_size=4096,
+                step_size=1024,
+                shuffle=True,
                 drop_last=True,
             ),
             batch_size=batch_size,
             collate_fn=partial(collate_fn, tokenizer=tokenizer),
             drop_last=True,
         )
         val_dataloader = DataLoader(
-            GutenbergEBookDataset(split="val", chunk_size=4096),
+            project_gutenberg_top_100_datapipe(
+                split="val", chunk_size=4096, step_size=1024
+            ),
             batch_size=batch_size,
             collate_fn=partial(collate_fn, tokenizer=tokenizer),
         )
 
         train(
             model=model,
             train_dataloader=train_dataloader,
@@ -319,37 +378,36 @@
     model = model.to(get_torch_device())
     prev_output = ""
     for output in generate(
         model,
         tokenizer=tokenizer,
         prompt=eval_prompt,
         max_new_tokens=eval_max_tokens,
-        print_stats=True,
     ):
         # Return to the start of the line and print the output (no newline)
         print(output[len(prev_output) :], end="", flush=True)
         prev_output = output
     print()
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("--model-name", type=str, required=True)
-    parser.add_argument("--tokenizer-path", type=str, required=True)
+    parser.add_argument("--model-name", type=str)
+    parser.add_argument("--tokenizer-path", type=str)
     parser.add_argument("--model-checkpoint", type=str, default=None)
     parser.add_argument("--accelerator", type=str, default="auto")
     parser.add_argument("--precision", type=str, default=None)
     parser.add_argument("--epochs", type=int, default=10)
-    parser.add_argument("--lr", type=float, default=1e-5)
-    parser.add_argument("--lr-warmup-steps", type=int, default=100)
-    parser.add_argument("--batch-size", type=int, default=64)
+    parser.add_argument("--lr", type=float, default=1e-4)
+    parser.add_argument("--lr-warmup-steps", type=int, default=250)
+    parser.add_argument("--batch-size", type=int, default=16)
     parser.add_argument("--accumulate-grad-batches", type=int, default=1)
     parser.add_argument("--log-frequency", type=int, default=25)
     parser.add_argument("--seed", type=int, default=42)
     parser.add_argument("--eval-only", action="store_true")
-    parser.add_argument("--eval-prompt", type=str, default=PROMPT)
+    parser.add_argument("--eval-prompt", type=str, default=EVAL_PROMPT)
     parser.add_argument("--eval-max-tokens", type=int, default=1024)
     args = parser.parse_args()
 
     main(**vars(args))
```

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch/config.py` & `openelm_pytorch-0.1.0rc1/openelm_pytorch/config.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch/openelm.py` & `openelm_pytorch-0.1.0rc1/openelm_pytorch/openelm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import math
 from pathlib import Path
-from typing import Iterable, Optional, Tuple, Union, cast
+from typing import Optional, Tuple, Union, cast
 
 import torch
 import torch.nn.functional as F
+from einops import einsum, rearrange, repeat
 from safetensors.torch import load_file
 from torch import Tensor, nn
 
 from openelm_pytorch.config import (
     ModelConfig,
     PretrainedModelConfig,
     PretrainedModelName,
@@ -23,105 +24,70 @@
         dims: int,
         eps: float = 1e-6,
         device: torch.device | None = None,
         dtype: torch.dtype | None = None,
     ):
         super().__init__()
         self.weight = nn.Parameter(torch.ones(dims, device=device, dtype=dtype))
-        self.scale = dims**0.5
         self.eps = eps
 
     def forward(self, x: Tensor) -> Tensor:
-        # TODO: Optimize this!  RMSNorm ends up taking >25% of the total text
-        # generation time.  Possibly a Triton kernel?
-        weight = self.weight * self.scale
-        return weight * F.normalize(x, p=2.0, dim=-1, eps=self.eps)
+        scale: float = 1 / x.size(-1) ** 0.5
+        norm = (x).norm(p=2, dim=-1, keepdim=True) * scale
+        return self.weight * x / (norm + self.eps)
 
 
 class RoPE(nn.Module):
-    def __init__(
-        self,
-        dim: int,
-        base: float = 10_000.0,
-        scale: float = 1.0,
-        max_context_len: int = 4096,
-        device: torch.device | None = None,
-        dtype: torch.dtype | None = None,
-    ):
+    def __init__(self, dim: int, base: float = 10000, scale: float = 1.0):
         super().__init__()
         self.dim = dim
         self.base = base
         self.scale = scale
-        self.max_context_size = max_context_len
-
-        # Cache the sin/cos Tensors for better performance.
-        if device == torch.device("meta"):
-            device = torch.device("cpu")
-        self.register_buffer(
-            "_sin", torch.empty(0, device=device, dtype=dtype), persistent=False
-        )
-        self.register_buffer(
-            "_cos", torch.empty(0, device=device, dtype=dtype), persistent=False
-        )
-        self._sin: Tensor
-        self._cos: Tensor
 
-    def _create_sin_cos_theta(
+    def create_cos_sin_theta(
         self,
         n: int,
         d: int,
         offset: int = 0,
-        base: float = 10_000.0,
+        base: float = 10000,
         scale: float = 1.0,
         dtype: torch.dtype | None = None,
         device: torch.device | None = None,
     ) -> tuple[Tensor, Tensor]:
+        # TODO: Cache cos and sin values for performance.
         half_d = d // 2
         positions = torch.arange(offset, n, device=device, dtype=dtype) * scale
         freqs = torch.exp(
             -torch.arange(0.0, half_d, device=device, dtype=dtype)
             * (math.log(base) / half_d)
         )
         theta = positions[:, None] * freqs[None, :]
-        return torch.sin(theta), torch.cos(theta)
+        return torch.cos(theta), torch.sin(theta)
 
     def forward(self, x: Tensor, offset: int = 0) -> Tensor:
-        if self._sin.numel() == 0:
-            self._sin, self._cos = self._create_sin_cos_theta(
-                self.max_context_size,
-                self.dim,
-                offset=offset,
-                base=self.base,
-                scale=self.scale,
-                dtype=x.dtype,
-                device=x.device,
-            )
-
-        return _apply_rope(x, self._sin, self._cos, offset=offset)
-
+        shape = x.shape
+        x = rearrange(x, "b ... s d -> (b ...) s d")
+        n = x.shape[1] + offset
+        costheta, sintheta = self.create_cos_sin_theta(
+            n=n,
+            d=self.dim,
+            offset=offset,
+            base=self.base,
+            scale=self.scale,
+            device=x.device,
+            dtype=x.dtype,
+        )
 
-@torch.jit.script
-def _apply_rope(x: Tensor, sin_theta: Tensor, cos_theta: Tensor, offset: int) -> Tensor:
-    # TODO: Optimize this!  RoPE ends up taking 20-25% of the total text
-    # generation time.  Possibly use Triton to fuse the operations?
-
-    shape = x.shape
-    # einops notation: "b ... s d -> (b ...) s d"
-    x = x.view(-1, x.shape[-2], x.shape[-1])
-    n = x.shape[1]
-    sin = sin_theta[offset : n + offset]
-    cos = cos_theta[offset : n + offset]
-
-    x1 = x[..., : x.shape[-1] // 2]
-    x2 = x[..., x.shape[-1] // 2 :]
-    rx1 = x1 * cos - x2 * sin
-    rx2 = x1 * sin + x2 * cos
+        x1 = x[..., : self.dim // 2]
+        x2 = x[..., self.dim // 2 : self.dim]
+        rx1 = x1 * costheta - x2 * sintheta
+        rx2 = x1 * sintheta + x2 * costheta
 
-    x = torch.cat([rx1, rx2], dim=-1)
-    return x.view(shape)
+        rx = torch.cat([rx1, rx2], dim=-1)
+        return rx.view(shape)
 
 
 class MultiHeadAttention(nn.Module):
     def __init__(
         self,
         model_dim: int,
         num_query_heads: int,
@@ -138,17 +104,15 @@
             model_dim,
             (num_query_heads + num_kv_heads + num_kv_heads) * head_dim,
             bias=False,
             device=device,
             dtype=dtype,
         )
 
-        self.pos_embedding = RoPE(
-            head_dim, base=float(rope_freq_constant), device=device, dtype=dtype
-        )
+        self.pos_embedding = RoPE(head_dim, base=rope_freq_constant)
         self.q_norm = RMSNorm(head_dim, device=device, dtype=dtype)
         self.k_norm = RMSNorm(head_dim, device=device, dtype=dtype)
 
         self.out_proj = nn.Linear(
             num_query_heads * head_dim,
             model_dim,
             bias=False,
@@ -182,72 +146,72 @@
             device=device,
             dtype=dtype,
         )
 
     def forward(
         self,
         x: Tensor,
-        kv_cache: Optional[Tuple[Tensor, Tensor]] = None,
+        past_key_value: Optional[Tuple[Tensor, Tensor]] = None,
         use_kv_cache: bool = False,
-        attn_mask: Tensor | None = None,
         is_causal: bool = False,
     ) -> Tuple[Tensor, Optional[Tuple[Tensor, Tensor]]]:
         qkv = self.qkv_proj.forward(x)
-        # einops notation: "b s (h d) -> b h s d", d=self.head_dim
-        qkv = qkv.view(x.shape[0], x.shape[1], -1, self.head_dim).permute(0, 2, 1, 3)
-        queries, keys, values = qkv.split_with_sizes(
-            [self.num_q_heads, self.num_k_heads, self.num_v_heads], dim=1
-        )
+        qkv = rearrange(qkv, "b s (h d) -> b h s d", d=self.head_dim)
+        queries = qkv[:, : self.num_q_heads]
+        keys = qkv[:, self.num_q_heads : self.num_q_heads + self.num_k_heads]
+        values = qkv[:, self.num_q_heads + self.num_k_heads :]
 
         queries = self.q_norm.forward(queries)
         keys = self.k_norm.forward(keys)
 
         if use_kv_cache:
-            if kv_cache is not None:
-                past_keys, past_values = kv_cache
+            if past_key_value is not None:
+                past_keys = past_key_value[0]
+                past_values = past_key_value[1]
                 queries = self.pos_embedding.forward(queries, offset=past_keys.shape[2])
                 keys = self.pos_embedding.forward(keys, offset=past_keys.shape[2])
-                # TODO: Concatenating here is somewhat inefficient.  Switch to
-                # slicing the tensors for better performance???
                 keys = torch.cat([past_keys, keys], dim=2)
                 values = torch.cat([past_values, values], dim=2)
             else:
                 queries = self.pos_embedding.forward(queries)
                 keys = self.pos_embedding.forward(keys)
 
-            kv_cache = (keys, values)
+            past_key_value = (keys, values)
 
         if self.num_groups != 1:
             # NOTE: There is a big difference between 'torch.repeat' and 'mx.repeat'!
             # 'mx.repeat' repeats each element 'n' times, whereas 'torch.repeat' repeats
-            # the entire tensor dimension 'n' times.  Use 'repeat_interleave'
-            # to get the intended behavior.
-            # Einops notation: "b h s d -> b (g h) s d"
-            keys = keys.repeat_interleave(self.num_groups, dim=1)
-            values = values.repeat_interleave(self.num_groups, dim=1)
+            # the entire tensor dimension 'n' times.  To achieve the same behavior,
+            # we repeat along a new axis, and then rearrange the tensor.
+            keys = rearrange(
+                repeat(keys, "b h s d -> b h g s d", g=self.num_groups),
+                "b h g s d -> b (h g) s d",
+            )
+            values = rearrange(
+                repeat(values, "b h s d -> b h g s d", g=self.num_groups),
+                "b h g s d -> b (h g) s d",
+            )
 
         # NOTE: Because the GQA key/value tensors are repeated above, the QKV tensors
         # all have the same number of heads!  This is slightly less efficient than
         # the optimal implementation (without repeating keys/values), but it reduces
         # the attention computation below to vanilla scaled dot-product attention.
         attention_output = F.scaled_dot_product_attention(
             query=queries,
             key=keys,
             value=values,
-            attn_mask=attn_mask,
             is_causal=is_causal,
             scale=self.scale,
         )
         # Fold the attention heads back into the model dimension.
-        attention_output = attention_output.permute(0, 2, 1, 3).reshape(
-            x.shape[0], -1, self.head_dim * self.num_q_heads
-        )
+        attention_output = rearrange(attention_output, "b h s d -> b s h d")
+        attention_output = rearrange(attention_output, "b s h d -> b s (h d)")
 
         out = self.out_proj.forward(attention_output)
-        return out, kv_cache
+        return out, past_key_value
 
     def reset_parameters(self):
         """The initialization scheme is followed, following `OPT
         <https://arxiv.org/pdf/2205.01068.pdf>`_.
         """
         std = self.model_dim**-0.5
         nn.init.normal_(self.qkv_proj.weight, std=std)
@@ -290,15 +254,15 @@
             dim=config.model_dim, hidden_dim=hidden_dim, device=device, dtype=dtype
         )
 
     def forward(self, x: Tensor) -> Tensor:
         y = self.proj_1.forward(x)
         y1, y2 = y.chunk(2, dim=-1)
         y = self.act(y1) * y2
-        return self.proj_2.forward(y)
+        return self.proj_2(y)
 
     def reset_parameters(self):
         """The initialization scheme is followed, following `OPT
         <https://arxiv.org/pdf/2205.01068.pdf>`_.
         """
         std = self.dim**-0.5
         nn.init.normal_(self.proj_1.weight, std=std)
@@ -336,33 +300,31 @@
         )
         ffn_norm = RMSNorm(config.model_dim, device=device, dtype=dtype)
         return cls(attn=attn, attn_norm=attn_norm, ffn=ffn, ffn_norm=ffn_norm)
 
     def forward(
         self,
         x: Tensor,
-        kv_cache: tuple[Tensor, Tensor] | None = None,
+        past_key_value: tuple[Tensor, Tensor] | None = None,
         use_kv_cache: bool = False,
-        attn_mask: Tensor | None = None,
         is_causal: bool = False,
     ) -> Tuple[Tensor, Optional[Tuple[Tensor, Tensor]]]:
         # Pre-norm attention
         y_attn = self.attn_norm(x)
-        y_attn, kv_cache = self.attn.forward(
+        y_attn, past_key_value = self.attn.forward(
             y_attn,
-            kv_cache=kv_cache,
+            past_key_value=past_key_value,
             use_kv_cache=use_kv_cache,
-            attn_mask=attn_mask,
             is_causal=is_causal,
         )
         y_attn = x + y_attn
 
         # Pre-norm FFN
         y_ffn = y_attn + self.ffn(self.ffn_norm(y_attn))
-        return y_ffn, kv_cache
+        return y_ffn, past_key_value
 
     def reset_parameters(self):
         self.attn.reset_parameters()
         self.ffn.reset_parameters()
 
 
 class OpenELM(nn.Module):
@@ -447,45 +409,42 @@
             assign=True,  # Needed, because we used device='meta' above.
         )
         return model.eval()
 
     def forward(
         self,
         input_ids: Tensor,
-        kv_cache: list[tuple[Tensor, Tensor] | None] | None = None,
+        past_key_values: list[tuple[Tensor, Tensor] | None] | None = None,
         use_kv_cache: bool = False,
-        attn_mask: Tensor | None = None,
         is_causal: bool = True,
     ) -> Union[Tensor, dict[str, Tensor | list[tuple[Tensor, Tensor] | None]]]:
         num_layers = len(self.layers)
-        if kv_cache is None:
-            kv_cache = [None] * num_layers
-        kv_cache = cast(list[tuple[Tensor, Tensor] | None], kv_cache)
+        if past_key_values is None:
+            past_key_values = [None] * num_layers
+        past_key_values = cast(list[tuple[Tensor, Tensor] | None], past_key_values)
 
         x = self.token_embeddings.forward(input_ids)
-        is_causal = is_causal and (attn_mask is None) and (x.shape[1] > 1)
+        is_causal = is_causal and x.shape[1] > 1
 
-        layers: Iterable[TransformerDecoderLayer] = self.layers
-        for i, layer in enumerate(layers):
+        for i, layer in enumerate(self.layers):
             layer = cast(TransformerDecoderLayer, layer)
-            x, kv_cache[i] = layer.forward(
+            x, past_key_values[i] = layer.forward(
                 x,
-                kv_cache=kv_cache[i],
+                past_key_value=past_key_values[i],
                 use_kv_cache=use_kv_cache,
-                attn_mask=attn_mask,
                 # NOTE: If using KV cache, do not use causal attention.
                 is_causal=(is_causal and x.shape[1] > 1),
             )
 
         x = self.norm(x)
-        logits = torch.einsum("b s d, e d -> b s e", x, self.token_embeddings.weight)
+        logits = einsum(x, self.token_embeddings.weight, "b s d, e d -> b s e")
 
         if use_kv_cache:
-            assert kv_cache is not None
-            return {"logits": logits, "kv_cache": kv_cache}
+            assert past_key_values is not None
+            return {"logits": logits, "past_key_values": past_key_values}
         else:
             return logits
 
     def reset_parameters(self) -> None:
         std = self.token_embeddings.embedding_dim**-0.5
         nn.init.normal_(self.token_embeddings.weight, std=std)
```

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch/tokenizer.py` & `openelm_pytorch-0.1.0rc1/openelm_pytorch/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,30 +32,26 @@
         return cls(model=model)
 
     def __call__(
         self,
         text: str | Sequence[str],
         device: torch.device | None = None,
         max_length: int | None = None,
-        add_bos: bool = True,
-        add_eos: bool = False,
     ) -> Tensor:
         # NOTE: The default 'pad_id' is -1, but this causes problems with the
         # tokenizer.  Token ID 1 appears to be the same as 'pad_id'.
         PAD_ID = 1
 
         if isinstance(text, str):
             return torch.as_tensor(
-                self.model.Encode(text, add_bos=add_bos, add_eos=add_eos),
-                device=device,
-                dtype=torch.long,
+                self.model.Encode(text, add_bos=True), device=device, dtype=torch.long
             )
         else:  # isinstance(text, list)
             encoded: list[list[int]] = [
-                self.model.Encode(t, add_bos=add_bos, add_eos=add_eos) for t in text
+                self.model.Encode(t, add_bos=True) for t in text
             ]
             pad_length = max(len(e) for e in encoded)
             if max_length is not None:
                 pad_length = min(pad_length, max_length)
 
             out = torch.empty(
                 (len(encoded), pad_length), device=device, dtype=torch.long
```

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch/utils.py` & `openelm_pytorch-0.1.0rc1/openelm_pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch.egg-info/PKG-INFO` & `openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: openelm-pytorch
-Version: 0.1.0
+Version: 0.1.0rc1
 Summary: openelm-pytorch
 Author-email: Frank Odom <frank.odom.iii@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: einops<1,>=0.7.0
 Requires-Dist: safetensors<1,>=0.4.0
 Requires-Dist: torch<3.0,>=2.0
 Provides-Extra: mlx
 Requires-Dist: mlx<1,>=0.10.0; extra == "mlx"
 Provides-Extra: train
-Requires-Dist: lora-pytorch~=0.2.0; extra == "train"
+Requires-Dist: lora-pytorch~=0.1.0; extra == "train"
 Requires-Dist: lightning~=2.2.0; extra == "train"
 Requires-Dist: tensorboard~=2.14.0; extra == "train"
+Requires-Dist: torchdata~=0.7.0; extra == "train"
 Requires-Dist: tqdm; extra == "train"
 Provides-Extra: test
 Requires-Dist: black==24.4.2; extra == "test"
 Requires-Dist: mlx==0.10.0; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: numpy==1.26.4; extra == "test"
 Requires-Dist: pre-commit==3.7.0; extra == "test"
```

### Comparing `openelm_pytorch-0.1.0/openelm_pytorch.egg-info/SOURCES.txt` & `openelm_pytorch-0.1.0rc1/openelm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/pyproject.toml` & `openelm_pytorch-0.1.0rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 authors = [
     {name = "Frank Odom", email = "frank.odom.iii@gmail.com"},
 ]
 description = "openelm-pytorch"
 license = {text = "MIT"}
 dynamic = ["version", "readme"]  # NOTE: Must be in sync with [tool.setuptools.dynamic] below
 dependencies = [
+    "einops>=0.7.0,<1",
     "safetensors>=0.4.0,<1",
     "torch>=2.0,<3.0",
 ]
 requires-python = ">=3.9"
 classifiers = ["Programming Language :: Python :: 3"]
 
 [tool.setuptools.dynamic]
@@ -26,17 +27,18 @@
 
 # extra packages (e.g. pip install .[test])
 [project.optional-dependencies]
 mlx = [
     "mlx>=0.10.0,<1",
 ]
 train = [
-    "lora-pytorch~=0.2.0",
+    "lora-pytorch~=0.1.0",
     "lightning~=2.2.0",
     "tensorboard~=2.14.0",
+    "torchdata~=0.7.0",
     "tqdm",
 ]
 test = [
     "black==24.4.2",
     "mlx==0.10.0",
     "mypy==1.10.0",
     "numpy==1.26.4",
```

### Comparing `openelm_pytorch-0.1.0/tests/conftest.py` & `openelm_pytorch-0.1.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/tests/openelm_mlx.py` & `openelm_pytorch-0.1.0rc1/tests/openelm_mlx.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/tests/test_config.py` & `openelm_pytorch-0.1.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/tests/test_openelm.py` & `openelm_pytorch-0.1.0rc1/tests/test_openelm.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         kv_mlx: list[tuple[mx.array, mx.array]] | None = None
         kv: list[tuple[Tensor, Tensor]] | None = None
 
         for i in range(seq_len):
             y_mlx, kv_mlx = mha_mlx(
                 x_mlx[:, i : i + 1], use_kv_cache=True, past_key_value=kv_mlx
             )
-            y, kv = mha(x[:, i : i + 1], use_kv_cache=True, kv_cache=kv)
+            y, kv = mha(x[:, i : i + 1], use_kv_cache=True, past_key_value=kv)
 
             assert kv_mlx is not None
             assert kv is not None
             # NOTE: A few elements had differences of ~2e-5.  I think this is
             # acceptable, but I'd prefer to set the tolerance to 1e-5.  Investigate
             # whether we can lower the threshold somehow.
             torch.testing.assert_close(
@@ -235,15 +235,15 @@
         kv_mlx: list[tuple[mx.array, mx.array]] | None = None
         kv: list[tuple[Tensor, Tensor]] | None = None
 
         for i in range(seq_len):
             y_mlx, kv_mlx = tdl_mlx(
                 x_mlx[:, i : i + 1], use_kv_cache=True, past_key_value=kv_mlx
             )
-            y, kv = tdl(x[:, i : i + 1], use_kv_cache=True, kv_cache=kv)
+            y, kv = tdl(x[:, i : i + 1], use_kv_cache=True, past_key_value=kv)
 
             assert kv_mlx is not None
             assert kv is not None
             torch.testing.assert_close(
                 kv[0], mlx_to_torch(kv_mlx[0], device=device), rtol=1e-2, atol=1e-5
             )
             torch.testing.assert_close(
@@ -351,18 +351,21 @@
                 "use_kv_cache": True,
                 "is_causal": is_causal,
             }
         )
         y_mlx = outputs_mlx["logits"]
         cache_mlx = outputs_mlx["past_key_values"]
         outputs = openelm.forward(
-            x[:, i : i + 1], kv_cache=cache, use_kv_cache=True, is_causal=is_causal
+            x[:, i : i + 1],
+            use_kv_cache=True,
+            past_key_values=cache,
+            is_causal=is_causal,
         )
         y = outputs["logits"]
-        cache = outputs["kv_cache"]
+        cache = outputs["past_key_values"]
 
         assert cache_mlx is not None
         assert cache is not None
         for kv_mlx, kv in zip(cache_mlx, cache):
             torch.testing.assert_close(
                 kv[0], mlx_to_torch(kv_mlx[0], device=device), rtol=1e-3, atol=1e-4
             )
```

### Comparing `openelm_pytorch-0.1.0/tests/test_tokenizer.py` & `openelm_pytorch-0.1.0rc1/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `openelm_pytorch-0.1.0/tests/utils.py` & `openelm_pytorch-0.1.0rc1/tests/utils.py`

 * *Files identical despite different names*

