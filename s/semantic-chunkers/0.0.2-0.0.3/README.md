# Comparing `tmp/semantic_chunkers-0.0.2.tar.gz` & `tmp/semantic_chunkers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_chunkers-0.0.2.tar", max compression
+gzip compressed data, was "semantic_chunkers-0.0.3.tar", max compression
```

## Comparing `semantic_chunkers-0.0.2.tar` & `semantic_chunkers-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-05-11 12:53:58.410362 semantic_chunkers-0.0.2/LICENSE
--rw-r--r--   0        0        0     1391 2024-05-11 12:53:58.410362 semantic_chunkers-0.0.2/README.md
--rw-r--r--   0        0        0     1006 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/__init__.py
--rw-r--r--   0        0        0      375 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/__init__.py
--rw-r--r--   0        0        0     1242 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/base.py
--rw-r--r--   0        0        0     2238 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/consecutive.py
--rw-r--r--   0        0        0     3211 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/cumulative.py
--rw-r--r--   0        0        0    18448 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/chunkers/statistical.py
--rw-r--r--   0        0        0      352 2024-05-11 12:53:58.466362 semantic_chunkers-0.0.2/semantic_chunkers/schema.py
--rw-r--r--   0        0        0        0 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/splitters/__init__.py
--rw-r--r--   0        0        0     2003 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/splitters/sentence.py
--rw-r--r--   0        0        0        0 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/logger.py
--rw-r--r--   0        0        0      192 2024-05-11 12:53:58.470362 semantic_chunkers-0.0.2/semantic_chunkers/utils/text.py
--rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-13 08:11:18.775424 semantic_chunkers-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1391 2024-05-13 08:11:18.775424 semantic_chunkers-0.0.3/README.md
+-rw-r--r--   0        0        0     1006 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/__init__.py
+-rw-r--r--   0        0        0     1521 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/base.py
+-rw-r--r--   0        0        0     2734 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/consecutive.py
+-rw-r--r--   0        0        0     3582 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/cumulative.py
+-rw-r--r--   0        0        0    18475 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/chunkers/statistical.py
+-rw-r--r--   0        0        0      353 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/schema.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/splitters/__init__.py
+-rw-r--r--   0        0        0     2003 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/splitters/sentence.py
+-rw-r--r--   0        0        0        0 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/logger.py
+-rw-r--r--   0        0        0      192 2024-05-13 08:11:18.835424 semantic_chunkers-0.0.3/semantic_chunkers/utils/text.py
+-rw-r--r--   0        0        0     2251 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.3/PKG-INFO
```

### Comparing `semantic_chunkers-0.0.2/LICENSE` & `semantic_chunkers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.2/README.md` & `semantic_chunkers-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.2/pyproject.toml` & `semantic_chunkers-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-chunkers"
-version = "0.0.2"
+version = "0.0.3"
 description = "Super advanced chunking methods for AI"
 authors = ["Aurelio AI <hello@aurelio.ai>"]
 readme = "README.md"
 packages = [{include = "semantic_chunkers"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/consecutive.py` & `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/consecutive.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, List
+from tqdm.auto import tqdm
 
 import numpy as np
 
 from semantic_router.encoders.base import BaseEncoder
-from semantic_chunkers.schema import ChunkSet
+from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
 
 
 class ConsecutiveChunker(BaseChunker):
     """
     Called "consecutive sim chunker" because we check the similarities of consecutive document embeddings (compare ith to i+1th document embedding).
     """
@@ -18,43 +19,57 @@
         name: str = "consecutive_chunker",
         score_threshold: float = 0.45,
     ):
         super().__init__(name=name, encoder=encoder)
         encoder.score_threshold = score_threshold
         self.score_threshold = score_threshold
 
-    def __call__(self, docs: List[Any]) -> List[ChunkSet]:
-        """Split documents into smaller chunks based on semantic similarity.
+    def _chunk(self, splits: List[Any], batch_size: int = 64) -> List[Chunk]:
+        """Merge splits into chunks using semantic similarity.
 
-        :param docs: list of text documents to be split, if only wanted to
-            split a single document, pass it as a list with a single element.
+        :param splits: splits to be merged into chunks.
 
-        :return: list of ChunkSet objects containing the chunks.
+        :return: list of chunks.
         """
-        # Check if there's only a single document
-        if len(docs) == 1:
-            raise ValueError(
-                "There is only one document provided; at least two are required to determine topics based on similarity."
-            )
-
-        doc_embeds = self.encoder(docs)
-        norm_embeds = doc_embeds / np.linalg.norm(doc_embeds, axis=1, keepdims=True)
+        split_embeds = []
+        num_splits = len(splits)
+        for i in tqdm(range(0, num_splits, batch_size)):
+            split_embeds.extend(self.encoder(splits[i : i + batch_size]))
+        norm_embeds = split_embeds / np.linalg.norm(split_embeds, axis=1, keepdims=True)
         sim_matrix = np.matmul(norm_embeds, norm_embeds.T)
-        total_docs = len(docs)
-        splits = []
+        chunks = []
         curr_split_start_idx = 0
-        curr_split_num = 1
 
-        for idx in range(1, total_docs):
+        for idx in tqdm(range(1, norm_embeds.shape[0])):
             curr_sim_score = sim_matrix[idx - 1][idx]
             if idx < len(sim_matrix) and curr_sim_score < self.score_threshold:
-                splits.append(
-                    ChunkSet(
-                        docs=list(docs[curr_split_start_idx:idx]),
+                chunks.append(
+                    Chunk(
+                        splits=splits[curr_split_start_idx:idx],
                         is_triggered=True,
                         triggered_score=curr_sim_score,
                     )
                 )
                 curr_split_start_idx = idx
-                curr_split_num += 1
-        splits.append(ChunkSet(docs=list(docs[curr_split_start_idx:])))
-        return splits
+        # append final chunk
+        chunks.append(Chunk(splits=splits[curr_split_start_idx:]))
+        self.chunks = chunks
+        return chunks
+
+    def __call__(self, docs: List[Any]) -> List[List[Chunk]]:
+        """Split documents into smaller chunks based on semantic similarity.
+
+        :param docs: list of text documents to be split, if only wanted to
+            split a single document, pass it as a list with a single element.
+
+        :return: list of list objects containing the chunks.
+        """
+        all_chunks = []
+        for doc in docs:
+            # split the document into sentences (if needed)
+            if isinstance(doc, str):
+                splits = self._split(doc)
+            else:
+                splits = doc
+            doc_chunks = self._chunk(splits)
+            all_chunks.append(doc_chunks)
+        return all_chunks
```

### Comparing `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/cumulative.py` & `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/cumulative.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import List
+from typing import Any, List
+from tqdm.auto import tqdm
 
 import numpy as np
 
 from semantic_router.encoders import BaseEncoder
-from semantic_chunkers.schema import ChunkSet
+from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
 
 
 class CumulativeChunker(BaseChunker):
     """
     Called "cumulative sim" because we check the similarities of the
     embeddings of cumulative concatenated documents with the next document.
@@ -19,62 +20,74 @@
         name: str = "cumulative_chunker",
         score_threshold: float = 0.45,
     ):
         super().__init__(name=name, encoder=encoder)
         encoder.score_threshold = score_threshold
         self.score_threshold = score_threshold
 
-    def __call__(self, docs: List[str]) -> List[ChunkSet]:
-        """Split documents into smaller chunks based on semantic similarity.
+    def _chunk(self, splits: List[Any], batch_size: int = 64) -> List[Chunk]:
+        """Merge splits into chunks using semantic similarity.
 
-        :param docs: list of text documents to be chunk, if only wanted to
-            chunk a single document, pass it as a list with a single element.
+        :param splits: splits to be merged into chunks.
 
-        :return: list of ChunkSet objects containing the chunks.
+        :return: list of chunks.
         """
-        total_docs = len(docs)
-        # Check if there's only a single document
-        if total_docs == 1:
-            raise ValueError(
-                "There is only one document provided; at least two are required "
-                "to determine topics based on similarity."
-            )
         chunks = []
         curr_chunk_start_idx = 0
+        num_splits = len(splits)
 
-        for idx in range(0, total_docs):
-            if idx + 1 < total_docs:  # Ensure there is a next document to compare with.
+        for idx in tqdm(range(num_splits)):
+            if idx + 1 < num_splits:  # Ensure there is a next document to compare with.
                 if idx == 0:
                     # On the first iteration, compare the
                     # first document directly to the second.
-                    curr_chunk_docs = docs[idx]
+                    curr_chunk_docs = splits[idx]
                 else:
                     # For subsequent iterations, compare cumulative
                     # documents up to the current one with the next.
-                    curr_chunk_docs = "\n".join(docs[curr_chunk_start_idx : idx + 1])
-                next_doc = docs[idx + 1]
+                    curr_chunk_docs = "\n".join(splits[curr_chunk_start_idx : idx + 1])
+                next_doc = splits[idx + 1]
 
                 # Embedding and similarity calculation remains the same.
                 curr_chunk_docs_embed = self.encoder([curr_chunk_docs])[0]
                 next_doc_embed = self.encoder([next_doc])[0]
                 curr_sim_score = np.dot(curr_chunk_docs_embed, next_doc_embed) / (
                     np.linalg.norm(curr_chunk_docs_embed)
                     * np.linalg.norm(next_doc_embed)
                 )
                 # Decision to chunk based on similarity score.
                 if curr_sim_score < self.score_threshold:
                     chunks.append(
-                        ChunkSet(
-                            docs=list(docs[curr_chunk_start_idx : idx + 1]),
+                        Chunk(
+                            splits=list(splits[curr_chunk_start_idx : idx + 1]),
                             is_triggered=True,
                             triggered_score=curr_sim_score,
                         )
                     )
                     curr_chunk_start_idx = (
                         idx + 1
                     )  # Update the start index for the next segment.
 
         # Add the last segment after the loop.
-        if curr_chunk_start_idx < total_docs:
-            chunks.append(ChunkSet(docs=list(docs[curr_chunk_start_idx:])))
+        if curr_chunk_start_idx < num_splits:
+            chunks.append(Chunk(splits=list(splits[curr_chunk_start_idx:])))
 
         return chunks
+
+    def __call__(self, docs: List[str]) -> List[List[Chunk]]:
+        """Split documents into smaller chunks based on semantic similarity.
+
+        :param docs: list of text documents to be chunk, if only wanted to
+            chunk a single document, pass it as a list with a single element.
+
+        :return: list of list objects containing the chunks.
+        """
+        all_chunks = []
+        for doc in docs:
+            # split the document into sentences (if needed)
+            if isinstance(doc, str):
+                splits = self._split(doc)
+            else:
+                splits = doc
+            doc_chunks = self._chunk(splits)
+            all_chunks.append(doc_chunks)
+        return all_chunks
```

### Comparing `semantic_chunkers-0.0.2/semantic_chunkers/chunkers/statistical.py` & `semantic_chunkers-0.0.3/semantic_chunkers/chunkers/statistical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from dataclasses import dataclass
 from typing import List
 
 import numpy as np
 
 from semantic_router.encoders.base import BaseEncoder
-from semantic_chunkers.schema import ChunkSet
+from semantic_chunkers.schema import Chunk
 from semantic_chunkers.chunkers.base import BaseChunker
-from semantic_chunkers.splitters import sentence
 from semantic_chunkers.utils.text import tiktoken_length
 from semantic_chunkers.utils.logger import logger
 
 
 @dataclass
 class ChunkStatistics:
     total_documents: int
@@ -59,50 +58,53 @@
         self.plot_chunks = plot_chunks
         self.min_split_tokens = min_split_tokens
         self.max_split_tokens = max_split_tokens
         self.split_tokens_tolerance = split_tokens_tolerance
         self.enable_statistics = enable_statistics
         self.statistics: ChunkStatistics
 
-    def __call__(self, docs: List[str]) -> List[ChunkSet]:
+    def __call__(self, docs: List[str]) -> List[List[Chunk]]:
         """Chunk documents into smaller chunks based on semantic similarity.
 
         :param docs: list of text documents to be split, if only wanted to
             split a single document, pass it as a list with a single element.
 
         :return: list of DocumentChunk objects containing the split documents.
         """
         if not docs:
             raise ValueError("At least one document is required for splitting.")
 
-        if len(docs) == 1:
-            token_count = tiktoken_length(docs[0])
+        all_chunks = []
+
+        for doc in docs:
+            token_count = tiktoken_length(doc)
             if token_count > self.max_split_tokens:
                 logger.info(
                     f"Single document exceeds the maximum token limit "
                     f"of {self.max_split_tokens}. "
                     "Splitting to sentences before semantically merging."
                 )
-            docs = sentence.regex_splitter(docs[0])
-        encoded_docs = self._encode_documents(docs)
-        similarities = self._calculate_similarity_scores(encoded_docs)
-        if self.dynamic_threshold:
-            self._find_optimal_threshold(docs, similarities)
-        else:
-            self.calculated_threshold = self.encoder.score_threshold
-        split_indices = self._find_split_indices(similarities=similarities)
-        chunks = self._split_documents(docs, split_indices, similarities)
-
-        if self.plot_chunks:
-            self.plot_similarity_scores(similarities, split_indices, chunks)
-
-        if self.enable_statistics:
-            print(self.statistics)
+            splits = self._split(doc)
+            encoded_splits = self._encode_documents(splits)
+            similarities = self._calculate_similarity_scores(encoded_splits)
+            if self.dynamic_threshold:
+                self._find_optimal_threshold(splits, similarities)
+            else:
+                self.calculated_threshold = self.encoder.score_threshold
+            split_indices = self._find_split_indices(similarities=similarities)
+            doc_chunks = self._split_documents(splits, split_indices, similarities)
+
+            if self.plot_chunks:
+                self.plot_similarity_scores(similarities, split_indices, doc_chunks)
+
+            if self.enable_statistics:
+                print(self.statistics)
+            all_chunks.append(doc_chunks)
 
-        return chunks
+        return all_chunks
 
     def _encode_documents(self, docs: List[str]) -> np.ndarray:
         """
         Encodes a list of documents into embeddings. If the number of documents exceeds 2000,
         the documents are split into batches to avoid overloading the encoder. OpenAI has a
         limit of len(array) < 2048.
 
@@ -203,15 +205,15 @@
             f"({self.min_split_tokens}-{self.max_split_tokens})."
         )
 
         return self.calculated_threshold
 
     def _split_documents(
         self, docs: List[str], split_indices: List[int], similarities: List[float]
-    ) -> List[ChunkSet]:
+    ) -> List[Chunk]:
         """
         This method iterates through each document, appending it to the current split
         until it either reaches a split point (determined by split_indices) or exceeds
         the maximum token limit for a split (self.max_split_tokens).
         When a document causes the current token count to exceed this limit,
         or when a split point is reached and the minimum token requirement is met,
         the current split is finalized and added to the List of chunks.
@@ -241,16 +243,16 @@
                     current_split.append(doc)
                     current_tokens_count += doc_token_count
 
                     triggered_score = (
                         similarities[doc_idx] if doc_idx < len(similarities) else None
                     )
                     chunks.append(
-                        ChunkSet(
-                            docs=current_split.copy(),
+                        Chunk(
+                            splits=current_split.copy(),
                             is_triggered=True,
                             triggered_score=triggered_score,
                             token_count=current_tokens_count,
                         )
                     )
                     logger.debug(
                         f"Chunk finalized with {current_tokens_count} tokens due to "
@@ -260,16 +262,16 @@
                     chunks_by_threshold += 1
                     continue  # Move to the next document after splitting
 
             # Check if adding the current document exceeds the max token limit
             if current_tokens_count + doc_token_count > self.max_split_tokens:
                 if current_tokens_count >= self.min_split_tokens:
                     chunks.append(
-                        ChunkSet(
-                            docs=current_split.copy(),
+                        Chunk(
+                            splits=current_split.copy(),
                             is_triggered=False,
                             triggered_score=None,
                             token_count=current_tokens_count,
                         )
                     )
                     chunks_by_max_chunk_size += 1
                     logger.debug(
@@ -280,31 +282,31 @@
 
             current_split.append(doc)
             current_tokens_count += doc_token_count
 
         # Handle the last split
         if current_split:
             chunks.append(
-                ChunkSet(
-                    docs=current_split.copy(),
+                Chunk(
+                    splits=current_split.copy(),
                     is_triggered=False,
                     triggered_score=None,
                     token_count=current_tokens_count,
                 )
             )
             chunks_by_last_split += 1
             logger.debug(
                 f"Final split added with {current_tokens_count} "
                 "tokens due to remaining documents."
             )
 
         # Validation to ensure no tokens are lost during the split
         original_token_count = sum(token_counts)
         split_token_count = sum(
-            [tiktoken_length(doc) for split in chunks for doc in split.docs]
+            [tiktoken_length(doc) for split in chunks for doc in split.splits]
         )
         if original_token_count != split_token_count:
             logger.error(
                 f"Token count mismatch: {original_token_count} != {split_token_count}"
             )
             raise ValueError(
                 f"Token count mismatch: {original_token_count} != {split_token_count}"
@@ -337,15 +339,15 @@
 
         return chunks
 
     def plot_similarity_scores(
         self,
         similarities: List[float],
         split_indices: List[int],
-        chunks: list[ChunkSet],
+        chunks: list[Chunk],
     ):
         try:
             from matplotlib import pyplot as plt
         except ImportError:
             logger.warning(
                 "Plotting is disabled. Please `pip install "
                 "semantic-router[processing]`."
@@ -422,17 +424,15 @@
         """
         Computes similarity scores between the average of the last
         'window_size' sentences and the next one,
         plots a graph of these similarity scores, and prints the first
         sentence after a similarity score below
         a specified threshold.
         """
-        sentences = [
-            sentence for doc in docs for sentence in sentence.regex_splitter(doc)
-        ]
+        sentences = [sentence for doc in docs for sentence in self._split(doc)]
         encoded_sentences = self._encode_documents(sentences)
         similarity_scores = []
 
         for i in range(window_size, len(encoded_sentences)):
             window_avg_encoding = np.mean(
                 encoded_sentences[i - window_size : i], axis=0
             )
```

### Comparing `semantic_chunkers-0.0.2/semantic_chunkers/splitters/sentence.py` & `semantic_chunkers-0.0.3/semantic_chunkers/splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.2/semantic_chunkers/utils/logger.py` & `semantic_chunkers-0.0.3/semantic_chunkers/utils/logger.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.2/PKG-INFO` & `semantic_chunkers-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-chunkers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Super advanced chunking methods for AI
 Author: Aurelio AI
 Author-email: hello@aurelio.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

