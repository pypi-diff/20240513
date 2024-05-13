# Comparing `tmp/ragstack_ai_llamaindex-1.0.1.tar.gz` & `tmp/ragstack_ai_llamaindex-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_llamaindex-1.0.1.tar", max compression
+gzip compressed data, was "ragstack_ai_llamaindex-1.0.2.tar", max compression
```

## Comparing `ragstack_ai_llamaindex-1.0.1.tar` & `ragstack_ai_llamaindex-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      374 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/README.md
--rw-r--r--   0        0        0     1802 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      271 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/__init__.py
--rw-r--r--   0        0        0      345 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/__init__.py
--rw-r--r--   0        0        0     1809 2024-04-30 16:33:53.855756 ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/retriever.py
--rw-r--r--   0        0        0     2136 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-05-13 16:31:21.120384 ragstack_ai_llamaindex-1.0.2/README.md
+-rw-r--r--   0        0        0     1819 2024-05-13 16:31:21.120384 ragstack_ai_llamaindex-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-13 16:31:21.120384 ragstack_ai_llamaindex-1.0.2/ragstack_llamaindex/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-13 16:31:21.120384 ragstack_ai_llamaindex-1.0.2/ragstack_llamaindex/colbert/__init__.py
+-rw-r--r--   0        0        0     1801 2024-05-13 16:31:21.120384 ragstack_ai_llamaindex-1.0.2/ragstack_llamaindex/colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     2174 1970-01-01 00:00:00.000000 ragstack_ai_llamaindex-1.0.2/PKG-INFO
```

### Comparing `ragstack_ai_llamaindex-1.0.1/pyproject.toml` & `ragstack_ai_llamaindex-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "ragstack-ai-llamaindex"
-version = "1.0.1"
+version = "1.0.2"
 description = "DataStax RAGStack Llama Index"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_llamaindex" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 astrapy = "^1"
 cassio = "~0.1.4"
 unstructured = "0.12.5"
-ragstack-ai-colbert = "1.0.1"
+ragstack-ai-colbert = "1.0.2"
 
 # llama-index
 llama-index = "0.10.31"
 llama-index-vector-stores-astra-db = "0.1.7"
 llama-index-vector-stores-cassandra = "0.1.3"
 llama-index-embeddings-langchain = "0.1.2"
 llama-parse = "0.4.1"
@@ -30,14 +30,15 @@
 llama-index-llms-bedrock = { version = "0.1.7", optional = true }
 llama-index-embeddings-bedrock = { version = "0.1.4", optional = true }
 ## google
 llama-index-llms-gemini = { version = "0.1.7", optional = true }
 llama-index-multi-modal-llms-gemini = { version = "0.1.5", optional = true }
 llama-index-llms-vertex = { version = "0.1.5", optional = true }
 llama-index-embeddings-gemini = { version = "0.1.6", optional = true }
+cffi = "^1.16.0"
 
 [tool.poetry.extras]
 colbert = ["ragstack-ai-colbert"]
 google = ["llama-index-llms-gemini", "llama-index-multi-modal-llms-gemini", "llama-index-llms-vertex", "llama-index-embeddings-gemini"]
 azure = ["llama-index-llms-azure-openai", "llama-index-embeddings-azure-openai"]
 bedrock = ["llama-index-llms-bedrock", "llama-index-embeddings-bedrock"]
```

### Comparing `ragstack_ai_llamaindex-1.0.1/ragstack_llamaindex/colbert/retriever.py` & `ragstack_ai_llamaindex-1.0.2/ragstack_llamaindex/colbert/colbert_retriever.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,55 @@
+from typing import Any, List, Optional, Tuple
 
-from llama_index.core.schema import NodeWithScore, QueryBundle, TextNode
 from llama_index.core.callbacks.base import CallbackManager
-from llama_index.core.retrievers import BaseRetriever as LlamaIndexBaseRetriever
 from llama_index.core.constants import DEFAULT_SIMILARITY_TOP_K
-from typing import Any, List, Optional
-
-from ragstack_colbert.base_retriever import BaseRetriever
+from llama_index.core.retrievers import BaseRetriever
+from llama_index.core.schema import NodeWithScore, QueryBundle, TextNode
+from ragstack_colbert import Chunk
+from ragstack_colbert.base_retriever import BaseRetriever as ColbertBaseRetriever
 
 
-class ColbertLIRetriever(LlamaIndexBaseRetriever):
+class ColbertRetriever(BaseRetriever):
     """ColBERT vector store retriever.
 
     Args:
         retriever (BaseRetriever): vector store index.
         similarity_top_k (int): number of top k results to return.
     """
 
+    _retriever: ColbertBaseRetriever
+    _k: int
+    _query_maxlen: Optional[int]
+
     def __init__(
         self,
-        retriever: BaseRetriever,
+        retriever: ColbertBaseRetriever,
         similarity_top_k: int = DEFAULT_SIMILARITY_TOP_K,
         callback_manager: Optional[CallbackManager] = None,
         object_map: Optional[dict] = None,
         verbose: bool = False,
         query_maxlen: int = -1,
         **kwargs: Any,
     ) -> None:
         """Initialize params."""
         self._retriever = retriever
-        self._similarity_top_k = similarity_top_k
+        self._k = similarity_top_k
         self._query_maxlen = query_maxlen
         super().__init__(
             callback_manager=callback_manager,
             object_map=object_map,
             verbose=verbose,
         )
 
     def _retrieve(
         self,
         query_bundle: QueryBundle,
     ) -> List[NodeWithScore]:
-        nodes: List[NodeWithScore] = []
-
-        chunks = self._retriever.retrieve(query_bundle.query_str, k=self._similarity_top_k, query_maxlen=self._query_maxlen)
-        for chunk in chunks:
-            text = chunk.data.text
-            metadata=chunk.data.metadata
-            metadata["rank"] = chunk.rank
-
-            node = TextNode(text=text, metadata=metadata)
-            nodes.append(NodeWithScore(node=node, score=chunk.score))
-        return nodes
+        chunk_scores: List[Tuple[Chunk, float]] = self._retriever.text_search(
+            query_text=query_bundle.query_str,
+            k=self._k,
+            query_maxlen=self._query_maxlen,
+        )
+        return [
+            NodeWithScore(node=TextNode(text=c.text, metadata=c.metadata), score=s)
+            for (c, s) in chunk_scores
+        ]
```

### Comparing `ragstack_ai_llamaindex-1.0.1/PKG-INFO` & `ragstack_ai_llamaindex-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-llamaindex
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataStax RAGStack Llama Index
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -13,28 +13,29 @@
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: azure
 Provides-Extra: bedrock
 Provides-Extra: colbert
 Provides-Extra: google
 Requires-Dist: astrapy (>=1,<2)
 Requires-Dist: cassio (>=0.1.4,<0.2.0)
+Requires-Dist: cffi (>=1.16.0,<2.0.0)
 Requires-Dist: llama-index (==0.10.31)
 Requires-Dist: llama-index-embeddings-azure-openai (==0.1.7) ; extra == "azure"
 Requires-Dist: llama-index-embeddings-bedrock (==0.1.4) ; extra == "bedrock"
 Requires-Dist: llama-index-embeddings-gemini (==0.1.6) ; extra == "google"
 Requires-Dist: llama-index-embeddings-langchain (==0.1.2)
 Requires-Dist: llama-index-llms-azure-openai (==0.1.6) ; extra == "azure"
 Requires-Dist: llama-index-llms-bedrock (==0.1.7) ; extra == "bedrock"
 Requires-Dist: llama-index-llms-gemini (==0.1.7) ; extra == "google"
 Requires-Dist: llama-index-llms-vertex (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-multi-modal-llms-gemini (==0.1.5) ; extra == "google"
 Requires-Dist: llama-index-vector-stores-astra-db (==0.1.7)
 Requires-Dist: llama-index-vector-stores-cassandra (==0.1.3)
 Requires-Dist: llama-parse (==0.4.1)
-Requires-Dist: ragstack-ai-colbert (==1.0.1) ; extra == "colbert"
+Requires-Dist: ragstack-ai-colbert (==1.0.2) ; extra == "colbert"
 Requires-Dist: unstructured (==0.12.5)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack LLamaIndex
```

