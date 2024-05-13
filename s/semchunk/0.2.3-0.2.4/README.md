# Comparing `tmp/semchunk-0.2.3.tar.gz` & `tmp/semchunk-0.2.4.tar.gz`

## Comparing `semchunk-0.2.3.tar` & `semchunk-0.2.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 semchunk-0.2.3/CHANGELOG.md
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 semchunk-0.2.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.2.3/.venv/Lib/site-packages/semchunk-0.1.0.dist-info/licenses/LICENCE
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 semchunk-0.2.3/src/semchunk/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.2.3/src/semchunk/py.typed
--rw-r--r--   0        0        0     5679 2020-02-02 00:00:00.000000 semchunk-0.2.3/src/semchunk/semchunk.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 semchunk-0.2.3/tests/bench.py
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 semchunk-0.2.3/tests/test_semchunk.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 semchunk-0.2.3/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.2.3/LICENCE
--rw-r--r--   0        0        0     5045 2020-02-02 00:00:00.000000 semchunk-0.2.3/README.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 semchunk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 semchunk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 semchunk-0.2.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 semchunk-0.2.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/py.typed
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 semchunk-0.2.4/src/semchunk/semchunk.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 semchunk-0.2.4/tests/bench.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 semchunk-0.2.4/tests/test_semchunk.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 semchunk-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 semchunk-0.2.4/LICENCE
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 semchunk-0.2.4/README.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 semchunk-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 semchunk-0.2.4/PKG-INFO
```

### Comparing `semchunk-0.2.3/CHANGELOG.md` & `semchunk-0.2.4/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 ## Changelog 🔄
 All notable changes to `semchunk` will be documented here. This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) and [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.2.4] - 2024-05-13
+### Changed
+- Improved chunking performance with larger chunk sizes by switching from linear to binary search for the identification of optimal chunk boundaries, courtesy of [@R0bk](https://github.com/R0bk) ([#3](https://github.com/umarbutler/semchunk/pull/3)) ([1e3ddb9](https://github.com/umarbutler/semchunk/pull/3/commits/1e3ddb91698f072da1d8a7d809a66467e1d31ff8)).
+
 ## [0.2.3] - 2024-03-11
 ### Fixed
 - Ensured that memoization does not overwrite `chunk()`'s function signature.
 
 ## [0.2.2] - 2024-02-05
 ### Fixed
 - Ensured that the `memoize` argument is passed back to `chunk()` in recursive calls.
@@ -36,14 +40,15 @@
 - Improved chunking performance.
 - improved test coverage.
 
 ## [0.1.0] - 2023-11-05
 ### Added
 - Added the `chunk()` function, which splits text into semantically meaningful chunks of a specified size as determined by a provided token counter.
 
+[0.2.4]: https://github.com/umarbutler/semchunk/compare/v0.2.3...v0.2.4
 [0.2.3]: https://github.com/umarbutler/semchunk/compare/v0.2.2...v0.2.3
 [0.2.2]: https://github.com/umarbutler/semchunk/compare/v0.2.1...v0.2.2
 [0.2.1]: https://github.com/umarbutler/semchunk/compare/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/umarbutler/semchunk/compare/v0.1.2...v0.2.0
 [0.1.2]: https://github.com/umarbutler/semchunk/compare/v0.1.1...v0.1.2
 [0.1.1]: https://github.com/umarbutler/semchunk/compare/v0.1.0...v0.1.1
 [0.1.0]: https://github.com/umarbutler/semchunk/releases/tag/v0.1.0
```

### Comparing `semchunk-0.2.3/.github/workflows/ci.yml` & `semchunk-0.2.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `semchunk-0.2.3/.venv/Lib/site-packages/semchunk-0.1.0.dist-info/licenses/LICENCE` & `semchunk-0.2.4/LICENCE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Umar Butler
+Copyright (c) 2024 Umar Butler
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `semchunk-0.2.3/src/semchunk/semchunk.py` & `semchunk-0.2.4/src/semchunk/semchunk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 import re
+
+from bisect import bisect_left
+from typing import Callable
 from functools import cache, wraps
+from itertools import accumulate
+
 
 _memoised_token_counters = {}
 """A map of token counters to their memoised versions."""
 
 _NON_WHITESPACE_SEMANTIC_SPLITTERS = (
     '.', '?', '!', '*', # Sentence terminators.
     ';', ',', '(', ')', '[', ']', "“", "”", '‘', '’', "'", '"', '`', # Clause separators.
@@ -41,18 +46,44 @@
         # If no semantically meaningful splitter is present in the text, return an empty string as the splitter and the text as a list of characters.
         else: # NOTE This code block will only be executed if the for loop completes without breaking.
             return '', splitter_is_whitespace, list(text)
     
     # Return the splitter and the split text.
     return splitter, splitter_is_whitespace, text.split(splitter)
 
-def chunk(text: str, chunk_size: int, token_counter: callable, memoize: bool=True, _recursion_depth: int = 0) -> list[str]:
+
+def merge_splits(splits: list[str], chunk_size: int, splitter: str, token_counter: Callable) -> tuple[int, str]:
+    """Merge splits until a chunk size is reached, returning the index of the last split included in the merged chunk along with the merged chunk itself."""
+    
+    average = 0.2
+    low = 0
+    high = len(splits) + 1
+    cumulative_lengths = list(accumulate([len(split) for split in splits], initial=0))
+    cumulative_lengths.append(cumulative_lengths[-1])
+
+    while low < high:
+        i = bisect_left(cumulative_lengths[low : high + 1], chunk_size * average)
+        midpoint = min(i + low, high - 1)
+
+        tokens = token_counter(splitter.join(splits[:midpoint]))
+
+        average = cumulative_lengths[midpoint] / tokens if cumulative_lengths[midpoint] else average
+
+        if tokens > chunk_size:
+            high = midpoint
+        else:
+            low = midpoint + 1
+
+    return low - 1, splitter.join(splits[:low - 1])
+
+
+def chunk(text: str, chunk_size: int, token_counter: Callable, memoize: bool = True, _recursion_depth: int = 0) -> list[str]:
     """Split text into semantically meaningful chunks of a specified size as determined by the provided token counter.
 
-   Args:
+    Args:
         text (str): The text to be chunked.
         chunk_size (int): The maximum number of tokens a chunk may contain.
         token_counter (callable): A callable that takes a string and returns the number of tokens in it.
         memoize (bool, optional): Whether to memoise the token counter. Defaults to True.
     
     Returns:
         list[str]: A list of chunks up to `chunk_size`-tokens-long, with any whitespace used to split the text removed."""
@@ -72,46 +103,35 @@
     for i, split in enumerate(splits):
         # Skip the split if it has already been added to a chunk.
         if i in skips:
             continue
         
         # If the split is over the chunk size, recursively chunk it.
         if token_counter(split) > chunk_size:
-            chunks.extend(chunk(split, chunk_size, token_counter=token_counter, memoize=memoize, _recursion_depth=_recursion_depth+1))
+            chunks.extend(chunk(split, chunk_size, token_counter = token_counter, memoize = memoize, _recursion_depth = _recursion_depth + 1))
 
-        # If the split is equal to or under the chunk size, merge it with all subsequent splits until the chunk size is reached.
+        # If the split is equal to or under the chunk size, add it and any subsequent splits to a new chunk until the chunk size is reached.
         else:
-            # Initalise the new chunk.
-            new_chunk = split
+            # Merge the split with subsequent splits until the chunk size is reached.
+            final_split_in_chunk_i, new_chunk = merge_splits(splits[i:], chunk_size, splitter, token_counter)
             
-            # Iterate through each subsequent split until the chunk size is reached.
-            for j, next_split in enumerate(splits[i+1:], start=i+1):
-                # Check whether the next split can be added to the chunk without exceeding the chunk size.
-                if token_counter(updated_chunk:=new_chunk+splitter+next_split) <= chunk_size:
-                    # Add the next split to the new chunk.
-                    new_chunk = updated_chunk
-                    
-                    # Add the index of the next split to the list of indices to skip.
-                    skips.add(j)
-                
-                # If the next split cannot be added to the chunk without exceeding the chunk size, break.
-                else:
-                    break
+            # Mark any splits included in the new chunk for exclusion from future chunks.
+            skips.update(range(i + 1, i + final_split_in_chunk_i))
             
             # Add the chunk.
             chunks.append(new_chunk)
 
         # If the splitter is not whitespace and the split is not the last split, add the splitter to the end of the last chunk if doing so would not cause it to exceed the chunk size otherwise add the splitter as a new chunk.
-        if not splitter_is_whitespace and not (i == len(splits) - 1 or all(j in skips for j in range(i+1, len(splits)))):
-            if token_counter(last_chunk_with_splitter:=chunks[-1]+splitter) <= chunk_size:
+        if not splitter_is_whitespace and not (i == len(splits) - 1 or all(j in skips for j in range(i + 1, len(splits)))):
+            if token_counter(last_chunk_with_splitter := chunks[-1] + splitter) <= chunk_size:
                 chunks[-1] = last_chunk_with_splitter
-            
             else:
                 chunks.append(splitter)
     
     # If this is not a recursive call, remove any empty chunks.
     if not _recursion_depth:
         chunks = list(filter(None, chunks))
     
     return chunks
 
+
 chunk = wraps(chunk)(cache(chunk))
```

### Comparing `semchunk-0.2.3/tests/bench.py` & `semchunk-0.2.4/tests/bench.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import semchunk
-import semantic_text_splitter
+from semantic_text_splitter import TextSplitter
 import test_semchunk
 import time
 
 chunk_size = 512
-semantic_text_splitter_chunker = semantic_text_splitter.TiktokenTextSplitter('gpt-4')
+semantic_text_splitter_chunker = TextSplitter.from_tiktoken_model('gpt-4', chunk_size)
 
 def bench_semchunk(text: str) -> None:
     semchunk.chunk(text, chunk_size=chunk_size, token_counter=test_semchunk._token_counter)
 
 def bench_semantic_text_splitter(text: str) -> None:
-    semantic_text_splitter_chunker.chunks(text, chunk_size)
+    semantic_text_splitter_chunker.chunks(text)
 
 libraries = {
     'semchunk': bench_semchunk,
     'semantic_text_splitter': bench_semantic_text_splitter,
 }
 
 def bench() -> dict[str, float]:
```

### Comparing `semchunk-0.2.3/tests/test_semchunk.py` & `semchunk-0.2.4/tests/test_semchunk.py`

 * *Files identical despite different names*

### Comparing `semchunk-0.2.3/README.md` & `semchunk-0.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # semchunk
 <a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <!-- <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a> -->
 
 `semchunk` is a fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 
-Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 70% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
+Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
 
 ## Installation 📦
 `semchunk` may be installed with `pip`:
 ```bash
 pip install semchunk
 ```
 
@@ -62,13 +62,13 @@
 1. Sentence interrupters (`:`, `—` and `…`);
 1. Word joiners (`/`, `\`, `–`, `&` and `-`); and
 1. All other characters.
 
 `semchunk` also relies on memoization to cache the results of token counters and the `chunk()` function, thereby improving performance.
 
 ## Benchmarks 📊
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it takes `semchunk` 24.41s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 1 minute and 48.01 seconds to chunk the same texts into 512-token-long chunks — a difference of 77.35%.
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds to chunk the same texts into 512-token-long chunks — a difference of 87.84%.
 
 The code used to benchmark `semchunk` and `semantic-text-splitter` is available [here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py).
 
 ## Licence 📄
 This library is licensed under the [MIT License](https://github.com/umarbutler/semchunk/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_c_o_v_/_c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and
 lightweight pure Python library for splitting text into semantically meaningful
 chunks. Owing to its complex yet highly efficient chunking algorithm,
 `semchunk` is both more semantically accurate than
 [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
 python.langchain.com/docs/modules/data_connection/document_transformers/
 text_splitters/recursive_text_splitter) (see [How It Works ð](https://
-github.com/umarbutler/semchunk#how-it-works-)) and is also over 70% faster than
+github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than
 [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/)
 (see the [Benchmarks ð](https://github.com/umarbutler/semchunk#benchmarks-
 )). ## Installation ð¦ `semchunk` may be installed with `pip`: ```bash pip
 install semchunk ``` ## Usage ð©âð» The code snippet below demonstrates
 how text can be chunked with `semchunk`: ```python >>> import semchunk >>>
 import tiktoken # `tiktoken` is not required but is used here to quickly count
 tokens. >>> text = 'The quick brown fox jumps over the lazy dog.' >>>
@@ -44,17 +44,17 @@
 by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
 `*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
 `â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
 1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
 `semchunk` also relies on memoization to cache the results of token counters
 and the `chunk()` function, thereby improving performance. ## Benchmarks ð
 On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it
-takes `semchunk` 24.41s seconds to split every sample in [NLTK's Gutenberg
+takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg
 Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
-token-long chunks (for context, the Corpus contains 18 texts and 3,001,260
-tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/
-project/semantic-text-splitter/) 1 minute and 48.01 seconds to chunk the same
-texts into 512-token-long chunks â a difference of 77.35%. The code used to
-benchmark `semchunk` and `semantic-text-splitter` is available [here](https://
-github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð This
-library is licensed under the [MIT License](https://github.com/umarbutler/
-semchunk/blob/main/LICENCE).
+token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
+texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
+(https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds
+to chunk the same texts into 512-token-long chunks â a difference of 87.84%.
+The code used to benchmark `semchunk` and `semantic-text-splitter` is available
+[here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py). ##
+Licence ð This library is licensed under the [MIT License](https://
+github.com/umarbutler/semchunk/blob/main/LICENCE).
```

### Comparing `semchunk-0.2.3/pyproject.toml` & `semchunk-0.2.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "semchunk"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   {name="Umar Butler", email="umar@umar.au"},
 ]
 description = "A fast and lightweight pure Python library for splitting text into semantically meaningful chunks."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
```

### Comparing `semchunk-0.2.3/PKG-INFO` & `semchunk-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: semchunk
-Version: 0.2.3
+Version: 0.2.4
 Summary: A fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 Project-URL: Homepage, https://github.com/umarbutler/semchunk
 Project-URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues
 Project-URL: Source, https://github.com/umarbutler/semchunk
 Author-email: Umar Butler <umar@umar.au>
 License: MIT
@@ -31,15 +31,15 @@
 Description-Content-Type: text/markdown
 
 # semchunk
 <a href="https://pypi.org/project/semchunk/" alt="PyPI Version"><img src="https://img.shields.io/pypi/v/semchunk"></a> <a href="https://github.com/umarbutler/semchunk/actions/workflows/ci.yml" alt="Build Status"><img src="https://img.shields.io/github/actions/workflow/status/umarbutler/semchunk/ci.yml?branch=main"></a> <a href="https://app.codecov.io/gh/umarbutler/semchunk" alt="Code Coverage"><img src="https://img.shields.io/codecov/c/github/umarbutler/semchunk"></a> <!-- <a href="https://pypistats.org/packages/semchunk" alt="Downloads"><img src="https://img.shields.io/pypi/dm/semchunk"></a> -->
 
 `semchunk` is a fast and lightweight pure Python library for splitting text into semantically meaningful chunks.
 
-Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 70% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
+Owing to its complex yet highly efficient chunking algorithm, `semchunk` is both more semantically accurate than [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://python.langchain.com/docs/modules/data_connection/document_transformers/text_splitters/recursive_text_splitter) (see [How It Works 🔍](https://github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) (see the [Benchmarks 📊](https://github.com/umarbutler/semchunk#benchmarks-)).
 
 ## Installation 📦
 `semchunk` may be installed with `pip`:
 ```bash
 pip install semchunk
 ```
 
@@ -94,13 +94,13 @@
 1. Sentence interrupters (`:`, `—` and `…`);
 1. Word joiners (`/`, `\`, `–`, `&` and `-`); and
 1. All other characters.
 
 `semchunk` also relies on memoization to cache the results of token counters and the `chunk()` function, thereby improving performance.
 
 ## Benchmarks 📊
-On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it takes `semchunk` 24.41s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 1 minute and 48.01 seconds to chunk the same texts into 512-token-long chunks — a difference of 77.35%.
+On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18 texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds to chunk the same texts into 512-token-long chunks — a difference of 87.84%.
 
 The code used to benchmark `semchunk` and `semantic-text-splitter` is available [here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py).
 
 ## Licence 📄
 This library is licensed under the [MIT License](https://github.com/umarbutler/semchunk/blob/main/LICENCE).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semchunk Version: 0.2.3 Summary: A fast and
+Metadata-Version: 2.3 Name: semchunk Version: 0.2.4 Summary: A fast and
 lightweight pure Python library for splitting text into semantically meaningful
 chunks. Project-URL: Homepage, https://github.com/umarbutler/semchunk Project-
 URL: Documentation, https://github.com/umarbutler/semchunk/blob/main/README.md
 Project-URL: Issues, https://github.com/umarbutler/semchunk/issues Project-URL:
 Source, https://github.com/umarbutler/semchunk Author-email: Umar Butler
 umar.au> License: MIT License-File: LICENCE Keywords:
 chunk,chunker,chunking,chunks,nlp,split,splits,splitter,splitting,text
@@ -24,15 +24,15 @@
 _c_/_g_i_t_h_u_b_/_u_m_a_r_b_u_t_l_e_r_/_s_e_m_c_h_u_n_k_]`semchunk` is a fast and lightweight pure Python
 library for splitting text into semantically meaningful chunks. Owing to its
 complex yet highly efficient chunking algorithm, `semchunk` is both more
 semantically accurate than
 [`langchain.text_splitter.RecursiveCharacterTextSplitter`](https://
 python.langchain.com/docs/modules/data_connection/document_transformers/
 text_splitters/recursive_text_splitter) (see [How It Works ð](https://
-github.com/umarbutler/semchunk#how-it-works-)) and is also over 70% faster than
+github.com/umarbutler/semchunk#how-it-works-)) and is also over 80% faster than
 [`semantic-text-splitter`](https://pypi.org/project/semantic-text-splitter/)
 (see the [Benchmarks ð](https://github.com/umarbutler/semchunk#benchmarks-
 )). ## Installation ð¦ `semchunk` may be installed with `pip`: ```bash pip
 install semchunk ``` ## Usage ð©âð» The code snippet below demonstrates
 how text can be chunked with `semchunk`: ```python >>> import semchunk >>>
 import tiktoken # `tiktoken` is not required but is used here to quickly count
 tokens. >>> text = 'The quick brown fox jumps over the lazy dog.' >>>
@@ -65,17 +65,17 @@
 by regex's `\s` character class); 1. Sentence terminators (`.`, `?`, `!` and
 `*`); 1. Clause separators (`;`, `,`, `(`, `)`, `[`, `]`, `â`, `â`, `â`,
 `â`, `'`, `"` and `` ` ``); 1. Sentence interrupters (`:`, `â` and `â¦`);
 1. Word joiners (`/`, `\`, `â`, `&` and `-`); and 1. All other characters.
 `semchunk` also relies on memoization to cache the results of token counters
 and the `chunk()` function, thereby improving performance. ## Benchmarks ð
 On a desktop with a Ryzen 3600, 64 GB of RAM, Windows 11 and Python 3.12.0, it
-takes `semchunk` 24.41s seconds to split every sample in [NLTK's Gutenberg
+takes `semchunk` 14.11s seconds to split every sample in [NLTK's Gutenberg
 Corpus](https://www.nltk.org/howto/corpus.html#plaintext-corpora) into 512-
-token-long chunks (for context, the Corpus contains 18 texts and 3,001,260
-tokens). By comparison, it takes [`semantic-text-splitter`](https://pypi.org/
-project/semantic-text-splitter/) 1 minute and 48.01 seconds to chunk the same
-texts into 512-token-long chunks â a difference of 77.35%. The code used to
-benchmark `semchunk` and `semantic-text-splitter` is available [here](https://
-github.com/umarbutler/semchunk/blob/main/tests/bench.py). ## Licence ð This
-library is licensed under the [MIT License](https://github.com/umarbutler/
-semchunk/blob/main/LICENCE).
+token-long chunks with GPT-4's tokenizer (for context, the Corpus contains 18
+texts and 3,001,260 tokens). By comparison, it takes [`semantic-text-splitter`]
+(https://pypi.org/project/semantic-text-splitter/) 2 minutes and 56.1 seconds
+to chunk the same texts into 512-token-long chunks â a difference of 87.84%.
+The code used to benchmark `semchunk` and `semantic-text-splitter` is available
+[here](https://github.com/umarbutler/semchunk/blob/main/tests/bench.py). ##
+Licence ð This library is licensed under the [MIT License](https://
+github.com/umarbutler/semchunk/blob/main/LICENCE).
```

