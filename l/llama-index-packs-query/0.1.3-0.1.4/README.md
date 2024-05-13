# Comparing `tmp/llama_index_packs_query-0.1.3.tar.gz` & `tmp/llama_index_packs_query-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_packs_query-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_packs_query-0.1.4.tar", max compression
```

## Comparing `llama_index_packs_query-0.1.3.tar` & `llama_index_packs_query-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1958 2024-02-13 13:53:02.217666 llama_index_packs_query-0.1.3/README.md
--rw-r--r--   0        0        0      120 2024-02-13 13:53:02.218299 llama_index_packs_query-0.1.3/llama_index/packs/rag_fusion_query_pipeline/__init__.py
--rw-r--r--   0        0        0     4385 2024-02-13 13:53:02.218378 llama_index_packs_query-0.1.3/llama_index/packs/rag_fusion_query_pipeline/base.py
--rw-r--r--   0        0        0     1566 2024-02-22 01:30:36.424324 llama_index_packs_query-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2670 1970-01-01 00:00:00.000000 llama_index_packs_query-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1958 2024-05-13 15:37:48.583942 llama_index_packs_query-0.1.4/README.md
+-rw-r--r--   0        0        0      120 2024-05-13 15:37:48.583942 llama_index_packs_query-0.1.4/llama_index/packs/rag_fusion_query_pipeline/__init__.py
+-rw-r--r--   0        0        0     4269 2024-05-13 15:37:48.583942 llama_index_packs_query-0.1.4/llama_index/packs/rag_fusion_query_pipeline/base.py
+-rw-r--r--   0        0        0     1566 2024-05-13 15:37:48.583942 llama_index_packs_query-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 llama_index_packs_query-0.1.4/PKG-INFO
```

### Comparing `llama_index_packs_query-0.1.3/README.md` & `llama_index_packs_query-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_packs_query-0.1.3/llama_index/packs/rag_fusion_query_pipeline/base.py` & `llama_index_packs_query-0.1.4/llama_index/packs/rag_fusion_query_pipeline/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """RAG Fusion Pipeline."""
 
 from typing import Any, Dict, List, Optional
 
-from llama_index.core import Document, ServiceContext, VectorStoreIndex
+from llama_index.core import Document, VectorStoreIndex
 from llama_index.core.llama_pack.base import BaseLlamaPack
 from llama_index.core.llms.llm import LLM
 from llama_index.core.node_parser import SentenceSplitter
 from llama_index.core.query_pipeline.components.argpacks import ArgPackComponent
 from llama_index.core.query_pipeline.components.function import FnComponent
 from llama_index.core.query_pipeline.components.input import InputComponent
 from llama_index.core.query_pipeline.query import QueryPipeline
@@ -14,35 +14,34 @@
 from llama_index.core.schema import NodeWithScore
 from llama_index.llms.openai import OpenAI
 
 DEFAULT_CHUNK_SIZES = [128, 256, 512, 1024]
 
 
 def reciprocal_rank_fusion(
-    results: List[List[NodeWithScore]],
+    results: List[NodeWithScore],
 ) -> List[NodeWithScore]:
     """Apply reciprocal rank fusion.
 
     The original paper uses k=60 for best results:
     https://plg.uwaterloo.ca/~gvcormac/cormacksigir09-rrf.pdf
     """
     k = 60.0  # `k` is a parameter used to control the impact of outlier rankings.
     fused_scores = {}
     text_to_node = {}
 
     # compute reciprocal rank scores
-    for nodes_with_scores in results:
-        for rank, node_with_score in enumerate(
-            sorted(nodes_with_scores, key=lambda x: x.score or 0.0, reverse=True)
-        ):
-            text = node_with_score.node.get_content()
-            text_to_node[text] = node_with_score
-            if text not in fused_scores:
-                fused_scores[text] = 0.0
-            fused_scores[text] += 1.0 / (rank + k)
+    for rank, node_with_score in enumerate(
+        sorted(results, key=lambda x: x.score or 0.0, reverse=True)
+    ):
+        text = node_with_score.node.get_content()
+        text_to_node[text] = node_with_score
+        if text not in fused_scores:
+            fused_scores[text] = 0.0
+        fused_scores[text] += 1.0 / (rank + k)
 
     # sort results
     reranked_results = dict(
         sorted(fused_scores.items(), key=lambda x: x[1], reverse=True)
     )
 
     # adjust node scores
@@ -61,14 +60,15 @@
 
     """
 
     def __init__(
         self,
         documents: List[Document],
         llm: Optional[LLM] = None,
+        embed_model: Optional[Any] = "default",
         chunk_sizes: Optional[List[int]] = None,
     ) -> None:
         """Init params."""
         self.documents = documents
         self.chunk_sizes = chunk_sizes or DEFAULT_CHUNK_SIZES
 
         # construct index
@@ -76,29 +76,28 @@
 
         self.query_engines = []
         self.retrievers = {}
         for chunk_size in self.chunk_sizes:
             splitter = SentenceSplitter(chunk_size=chunk_size, chunk_overlap=0)
             nodes = splitter.get_nodes_from_documents(documents)
 
-            service_context = ServiceContext.from_defaults(llm=self.llm)
-            vector_index = VectorStoreIndex(nodes, service_context=service_context)
-            self.query_engines.append(vector_index.as_query_engine())
+            vector_index = VectorStoreIndex(nodes, embed_model=embed_model)
+            self.query_engines.append(vector_index.as_query_engine(llm=self.llm))
 
             self.retrievers[str(chunk_size)] = vector_index.as_retriever()
 
         # define rerank component
         rerank_component = FnComponent(fn=reciprocal_rank_fusion)
 
         # construct query pipeline
         p = QueryPipeline()
         module_dict = {
             **self.retrievers,
             "input": InputComponent(),
-            "summarizer": TreeSummarize(),
+            "summarizer": TreeSummarize(llm=llm),
             # NOTE: Join args
             "join": ArgPackComponent(),
             "reranker": rerank_component,
         }
         p.add_modules(module_dict)
         # add links from input to retriever (id'ed by chunk_size)
         for chunk_size in self.chunk_sizes:
```

### Comparing `llama_index_packs_query-0.1.3/pyproject.toml` & `llama_index_packs_query-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index packs query integration"
 exclude = ["**/BUILD"]
 keywords = ["fusion", "pipeline", "query", "rag"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-packs-query"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_packs_query-0.1.3/PKG-INFO` & `llama_index_packs_query-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-packs-query
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index packs query integration
 License: MIT
 Keywords: fusion,pipeline,query,rag
 Author: Your Name
 Author-email: you@example.com
 Maintainer: jerryjliu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # RAG Fusion Pipeline Llama Pack
 
 This LlamaPack creates the RAG Fusion Query Pipeline, which runs multiple retrievers in parallel (with varying chunk sizes), and aggregates the results in the end with reciprocal rank fusion.
```

