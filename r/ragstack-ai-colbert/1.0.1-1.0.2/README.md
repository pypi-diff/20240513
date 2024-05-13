# Comparing `tmp/ragstack_ai_colbert-1.0.1.tar.gz` & `tmp/ragstack_ai_colbert-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_colbert-1.0.1.tar", max compression
+gzip compressed data, was "ragstack_ai_colbert-1.0.2.tar", max compression
```

## Comparing `ragstack_ai_colbert-1.0.1.tar` & `ragstack_ai_colbert-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      374 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/README.md
--rw-r--r--   0        0        0      600 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1512 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_embedding_model.py
--rw-r--r--   0        0        0     1853 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_retriever.py
--rw-r--r--   0        0        0     2989 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/base_vector_store.py
--rw-r--r--   0        0        0     7928 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/cassandra_vector_store.py
--rw-r--r--   0        0        0    12718 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_embedding_model.py
--rw-r--r--   0        0        0    13608 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_retriever.py
--rw-r--r--   0        0        0      695 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/constant.py
--rw-r--r--   0        0        0      154 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/__init__.py
--rw-r--r--   0        0        0     5617 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/chunk_encoder.py
--rw-r--r--   0        0        0     7136 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/distributed.py
--rw-r--r--   0        0        0     6962 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/distributed/runner.py
--rw-r--r--   0        0        0     2702 2024-04-30 14:58:37.552511 ragstack_ai_colbert-1.0.1/ragstack_colbert/objects.py
--rw-r--r--   0        0        0     1210 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      374 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/README.md
+-rw-r--r--   0        0        0      596 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1542 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/__init__.py
+-rw-r--r--   0        0        0     2470 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_database.py
+-rw-r--r--   0        0        0     1848 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_embedding_model.py
+-rw-r--r--   0        0        0     5645 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_retriever.py
+-rw-r--r--   0        0        0     3275 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/base_vector_store.py
+-rw-r--r--   0        0        0     8525 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/cassandra_database.py
+-rw-r--r--   0        0        0     5403 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_embedding_model.py
+-rw-r--r--   0        0        0    15736 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     4385 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0      664 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/constant.py
+-rw-r--r--   0        0        0     2178 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/objects.py
+-rw-r--r--   0        0        0     4580 2024-05-13 16:14:59.192325 ragstack_ai_colbert-1.0.2/ragstack_colbert/text_encoder.py
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 ragstack_ai_colbert-1.0.2/PKG-INFO
```

### Comparing `ragstack_ai_colbert-1.0.1/pyproject.toml` & `ragstack_ai_colbert-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "ragstack-ai-colbert"
-version = "1.0.1"
+version = "1.0.2"
 description = "DataStax RAGStack Colbert implementation"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_colbert" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 colbert-ai = "0.2.19"
 pyarrow = "14.0.1"
 torch = "2.2.1"
 cassio = "~0.1.7"
-nest-asyncio = "^1.6.0"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-tests-utils = { path = "../tests-utils", develop = true }
```

### Comparing `ragstack_ai_colbert-1.0.1/ragstack_colbert/__init__.py` & `ragstack_ai_colbert-1.0.2/ragstack_colbert/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
 This package provides a suite of tools for encoding and retrieving text using the ColBERT model, integrated with a
 Cassandra database for scalable storage and retrieval operations. It includes classes for token embeddings,
 managing the vector store, and performing efficient similarity searches. Utilities for working with embeddings
 and constants related to the ColBERT model configuration are also provided.
 
 Exports:
-- CassandraVectorStore: Implementation of a ColBERT vector store using Cassandra for storage.
+- CassandraDatabase: Implementation of a BaseDatabase using Cassandra for storage.
 - ColbertEmbeddingModel: Class for generating and managing token embeddings using the ColBERT model.
+- ColbertVectorStore: Implementation of a BaseVectorStore.
 - ColbertRetriever: Retriever class for executing ColBERT searches within a vector store.
 - DEFAULT_COLBERT_MODEL: The default identifier for the ColBERT model.
 - DEFAULT_COLBERT_DIM: The default dimensionality for ColBERT model embeddings.
-- EmbeddedChunk: Data class for representing a chunk of embedded text.
-- RetrievedChunk: Data class for representing a chunk of retrieved text.
+- Chunk: Data class for representing a chunk of embedded text.
 """
 
-from .cassandra_vector_store import CassandraVectorStore
-from .colbert_retriever import ColbertRetriever
+from .cassandra_database import CassandraDatabase
 from .colbert_embedding_model import ColbertEmbeddingModel
+from .colbert_retriever import ColbertRetriever
+from .colbert_vector_store import ColbertVectorStore
 from .constant import DEFAULT_COLBERT_DIM, DEFAULT_COLBERT_MODEL
-from .objects import ChunkData, EmbeddedChunk, RetrievedChunk
+from .objects import Chunk, Embedding, Metadata, Vector
 
 __all__ = [
-    "CassandraVectorStore",
-    "ChunkData",
+    "CassandraDatabase",
     "ColbertEmbeddingModel",
     "ColbertRetriever",
+    "ColbertVectorStore",
     "DEFAULT_COLBERT_DIM",
     "DEFAULT_COLBERT_MODEL",
-    "EmbeddedChunk",
-    "RetrievedChunk",
+    "Chunk",
+    "Embedding",
+    "Metadata",
+    "Vector",
 ]
```

### Comparing `ragstack_ai_colbert-1.0.1/ragstack_colbert/base_vector_store.py` & `ragstack_ai_colbert-1.0.2/ragstack_colbert/base_database.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,81 +2,78 @@
 This module defines abstract base classes for implementing storage mechanisms for text chunk
 embeddings, specifically designed to work with ColBERT or similar embedding models.
 """
 
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple
 
-from torch import Tensor
+from .objects import Chunk, Vector
 
-from .objects import BaseChunk, ChunkData, EmbeddedChunk
 
-
-class BaseVectorStore(ABC):
+class BaseDatabase(ABC):
     """
     Abstract base class (ABC) for a storage system designed to hold vector representations of text chunks,
     typically generated by a ColBERT model or similar embedding model.
 
     This class defines the interface for storing and managing the embedded text chunks, supporting
     operations like adding new chunks to the store and deleting existing documents by their identifiers.
     """
 
     @abstractmethod
-    def put_chunks(
-        self, chunks: List[EmbeddedChunk], delete_existing: Optional[bool] = False
-    ) -> None:
+    def add_chunks(self, chunks: List[Chunk]) -> List[Tuple[str, int]]:
         """
-        Stores a list of embedded text chunks in the vector store, with an option to delete existing
-        entries before insertion.
+        Stores a list of embedded text chunks in the vector store
 
         Parameters:
-            chunks (List[EmbeddedChunk]): A list of `EmbeddedChunk` instances to be stored.
-            delete_existing (Optional[bool]): If True, any existing chunks with the same doc_ids
-                                               as those in the `chunks` list will be deleted before
-                                               inserting the new ones. Defaults to False.
+            chunks (List[Chunk]): A list of `Chunk` instances to be stored.
+
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
         """
 
     @abstractmethod
-    def delete_chunks(self, doc_ids: List[str]) -> None:
+    def delete_chunks(self, doc_ids: List[str]) -> bool:
         """
         Deletes chunks from the vector store based on their document id.
 
         Parameters:
             doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
+
+        Returns:
+            True if the delete was successful.
         """
 
     @abstractmethod
-    async def search_relevant_chunks(self, vector: List[float], n: int) -> List[BaseChunk]:
+    async def search_relevant_chunks(self, vector: Vector, n: int) -> List[Chunk]:
         """
-        Searches for relevant chunks using ANN for an embedded token vector.
-
-        Parameters:
-            vector (List[float]): A vector embedding for a query token.
-            n (int): The number of items to return from the search
+        Retrieves 'n' ANN results for an embedded token vector.
 
         Returns:
-            A list of chunks with doc_id and chunk_id. Fewer than 'n' results may be returned.
+            A list of Chunks with only `doc_id` and `chunk_id` set.
+            Fewer than 'n' results may be returned.
         """
 
     @abstractmethod
-    async def get_chunk_embeddings(self, chunk: BaseChunk) -> Tuple[BaseChunk, List[Tensor]]:
+    async def get_chunk_embedding(self, doc_id: str, chunk_id: int) -> Chunk:
         """
-        Retrieve all the embedding data for a chunk.
-
-        Parameters:
-            chunk (BaseChunk): The chunk to return.
+        Retrieve the embedding data for a chunk.
 
         Returns:
-            A RetrievedChunk including doc_id, chunk_id, and the embeddings for the chunk.
+            A chunk with `doc_id`, `chunk_id`, and `embedding` set.
         """
 
     @abstractmethod
-    async def get_chunk_data(self, chunk: BaseChunk) -> Tuple[BaseChunk, ChunkData]:
+    async def get_chunk_data(
+        self, doc_id: str, chunk_id: int, include_embedding: Optional[bool]
+    ) -> Chunk:
         """
-        Fetches the text and metadata for a given doc_id and chunk_id.
-
-        Parameters:
-            chunk (BaseChunk): The chunk to return.
+        Retrieve the text and metadata for a chunk.
 
         Returns:
-            ChunkData including text and metadata for the chunk.
+            A chunk with `doc_id`, `chunk_id`, `text`, `metadata`, and optionally `embedding` set.
+        """
+
+    @abstractmethod
+    def close(self) -> None:
+        """
+        Cleans up any open resources.
         """
```

### Comparing `ragstack_ai_colbert-1.0.1/ragstack_colbert/cassandra_vector_store.py` & `ragstack_ai_colbert-1.0.2/ragstack_colbert/cassandra_database.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,188 +1,253 @@
 """
 This module provides an implementation of the BaseVectorStore abstract class, specifically designed
 for use with a Cassandra database backend. It allows for the efficient storage and management of text embeddings
 generated by a ColBERT model, facilitating scalable and high-relevancy retrieval operations.
 """
 
 import logging
-from typing import Any, Dict, List, Optional, Set, Tuple
+from typing import List, Optional, Set, Tuple
 
-import torch
+import cassio
 from cassandra.cluster import ResponseFuture, Session
 from cassio.table.query import Predicate, PredicateOperator
 from cassio.table.tables import ClusteredMetadataVectorCassandraTable
-from torch import Tensor
 
-from .base_vector_store import BaseVectorStore
-from .objects import BaseChunk, ChunkData, EmbeddedChunk
+from .base_database import BaseDatabase
+from .constant import DEFAULT_COLBERT_DIM
+from .objects import Chunk, Vector
 
 
-class CassandraVectorStore(BaseVectorStore):
+class CassandraDatabase(BaseDatabase):
     """
-    An implementation of the BaseVectorStore abstract base class using Cassandra as the backend
+    An implementation of the BaseDatabase abstract base class using Cassandra as the backend
     storage system. This class provides methods to store, retrieve, and manage text embeddings within
     a Cassandra database, specifically designed for handling vector embeddings generated by ColBERT.
 
-    Attributes:
-        session (Session): The Cassandra session instance used for database operations.
-        keyspace (str): The name of the Cassandra keyspace to use.
-        table_name (str): The name of the table within the keyspace for storing chunk embeddings.
-        full_table_name (str): The full name of the table (including keyspace) for queries.
-        insert_chunk_stmt (PreparedStatement): Prepared statement for inserting text chunks.
-        insert_colbert_stmt (PreparedStatement): Prepared statement for inserting embeddings.
-        query_colbert_ann_stmt (PreparedStatement): Prepared statement for ANN queries.
-        query_colbert_chunks_stmt (PreparedStatement): Prepared statement for retrieving chunks.
-        query_chunk_stmt (PreparedStatement): Prepared statement for retrieving chunk bodies.
-        delete_chunks_by_doc_id_stmt (PreparedStatement): Prepared statement for deleting chunks.
-
     The table schema and custom index for ANN queries are automatically created if they do not exist.
     """
 
     _table: ClusteredMetadataVectorCassandraTable
+    _instance = None
 
-    def __init__(
-        self, session: Session, keyspace: str, table_name: str, timeout: int = 180
+    def __new__(cls):
+        if cls._instance is None:
+            raise ValueError(
+                "This class cannot be instantiated directly. Please use the `from_astra()` or `from_session()` class methods."
+            )
+        return cls._instance
+
+    @classmethod
+    def from_astra(
+        cls,
+        database_id: str,
+        astra_token: str,
+        keyspace: Optional[str] = "default_keyspace",
+        table_name: Optional[str] = "colbert",
+        timeout: Optional[int] = 180,
+    ):
+        if cls._instance is None:
+            cassio.init(token=astra_token, database_id=database_id, keyspace=keyspace)
+            session = cassio.config.resolve_session()
+            session.default_timeout = timeout
+
+            return cls.from_session(
+                session=session, keyspace=keyspace, table_name=table_name
+            )
+        return cls._instance
+
+    @classmethod
+    def from_session(
+        cls,
+        session: Session,
+        keyspace: Optional[str] = "default_keyspace",
+        table_name: Optional[str] = "colbert",
+    ):
+        if cls._instance is None:
+            cls._instance = super().__new__(cls)
+            cls._instance._initialize(
+                session=session, keyspace=keyspace, table_name=table_name
+            )
+        return cls._instance
+
+    def _initialize(
+        self,
+        session: Session,
+        keyspace: str,
+        table_name: str,
     ):
         """
         Initializes a new instance of the CassandraVectorStore.
 
         Parameters:
             session (Session): The Cassandra session to use.
             keyspace (str): The keyspace in which the table exists or will be created.
             table_name (str): The name of the table to use or create for storing embeddings.
             timeout (int, optional): The default timeout in seconds for Cassandra operations. Defaults to 180.
         """
 
-        cluster_name = session.cluster.metadata.cluster_name.lower()
-        is_astra = "cndb" == cluster_name
-        logging.debug(f"colbert store is running on {'astra' if is_astra else 'apache cassandra'}")
+        try:
+            is_astra = session.cluster.cloud
+        except:
+            is_astra = False
 
-        session.default_timeout = timeout
+        logging.info(
+            f"Cassandra store is running on {'AstraDB' if is_astra else 'Apache Cassandra'}."
+        )
 
         self._table = ClusteredMetadataVectorCassandraTable(
             session=session,
             keyspace=keyspace,
             table=table_name,
             row_id_type=["INT", "INT"],
-            vector_dimension=128,
+            vector_dimension=DEFAULT_COLBERT_DIM,
             vector_source_model="bert" if is_astra else None,
             vector_similarity_function=None if is_astra else "DOT_PRODUCT",
         )
 
-    def put_chunks(
-        self, chunks: List[EmbeddedChunk], delete_existing: Optional[bool] = False
-    ) -> None:
-        """
-        Stores a list of EmbeddedChunk instances in the Cassandra database, managing both the text
-        body and the embeddings of each chunk. Optionally deletes existing chunks for each document
-        before insertion.
+    def add_chunks(self, chunks: List[Chunk]) -> List[Tuple[str, int]]:
+        """
+        Stores a list of embedded text chunks in the vector store
 
         Parameters:
-            chunks (List[EmbeddedChunk]): A list of EmbeddedChunk instances to store.
-            delete_existing (Optional[bool]): A flag indicating whether to delete existing chunks for the
-                                              documents related to the chunks being inserted.
-        """
+            chunks (List[Chunk]): A list of `Chunk` instances to be stored.
 
-        if delete_existing:
-            doc_ids = [c.doc_id for c in chunks]
-            self.delete_chunks(list(set(doc_ids)))
+        Returns:
+            a list of tuples: (doc_id, chunk_id)
+        """
 
         futures: List[Tuple[str, int, int, ResponseFuture]] = []
 
         for chunk in chunks:
             doc_id = chunk.doc_id
             chunk_id = chunk.chunk_id
-            text = chunk.data.text
-            metadata = {} if len(chunk.data.metadata) == 0 else chunk.data.metadata
+            text = chunk.text
+            metadata = chunk.metadata
 
-            future = self._table.put_async(partition_id=doc_id, row_id=(chunk_id, -1), body_blob=text, metadata=metadata)
+            future = self._table.put_async(
+                partition_id=doc_id,
+                row_id=(chunk_id, -1),
+                body_blob=text,
+                metadata=metadata,
+            )
 
             futures.append((doc_id, chunk_id, -1, future))
 
-            for index, vector in enumerate(chunk.embeddings.tolist()):
-                future = self._table.put_async(partition_id=doc_id, row_id=(chunk_id, index), vector=vector)
+            for index, vector in enumerate(chunk.embedding):
+                future = self._table.put_async(
+                    partition_id=doc_id, row_id=(chunk_id, index), vector=vector
+                )
                 futures.append((doc_id, chunk_id, index, future))
 
-            for (doc_id, chunk_id, embedding_id, future) in futures:
+            results: List[Tuple[str, int]] = []
+            for doc_id, chunk_id, embedding_id, future in futures:
                 try:
                     future.result()
+                    results.append((doc_id, chunk_id))
                 except Exception as e:
                     if embedding_id == -1:
-                        logging.error(f"issue inserting document data: {doc_id} chunk: {chunk_id}: {e}")
+                        logging.error(
+                            f"issue inserting document data: {doc_id} chunk: {chunk_id}: {e}"
+                        )
                     else:
-                        logging.error(f"issue inserting document embedding: {doc_id} chunk: {chunk_id} embedding: {embedding_id}: {e}")
+                        logging.error(
+                            f"issue inserting document embedding: {doc_id} chunk: {chunk_id} embedding: {embedding_id}: {e}"
+                        )
+
+        return results
 
     def delete_chunks(self, doc_ids: List[str]) -> None:
         """
-        Deletes all chunks associated with the specified document identifiers.
+        Deletes chunks from the vector store based on their document id.
 
         Parameters:
-            doc_ids (List[str]): A list of document identifiers whose chunks should be deleted.
+            doc_ids (List[str]): A list of document identifiers specifying the chunks to be deleted.
+
+        Returns:
+            True if the delete was successful.
         """
 
-        futures = [(doc_id, self._table.delete_partition_async(partition_id = doc_id)) for doc_id in doc_ids]
+        futures = [
+            (doc_id, self._table.delete_partition_async(partition_id=doc_id))
+            for doc_id in doc_ids
+        ]
 
-        for (doc_id, future) in futures:
+        success = True
+        for doc_id, future in futures:
             try:
                 future.result()
             except Exception as e:
+                success = False
                 logging.error(f"issue on delete of document: {doc_id}: {e}")
+        return success
 
-    async def search_relevant_chunks(self, vector: List[float], n: int) -> List[BaseChunk]:
+    async def search_relevant_chunks(self, vector: Vector, n: int) -> List[Chunk]:
         """
         Retrieves 'n' ANN results for an embedded token vector.
 
         Returns:
-            A set of tuples of (doc_id, chunk_id). Fewer than 'n' results may be returned.
+            A list of Chunks with only `doc_id` and `chunk_id` set.
+            Fewer than 'n' results may be returned.
         """
 
-        chunks: Set[BaseChunk] = set()
+        chunks: Set[Chunk] = set()
 
         # TODO: only return partition_id and row_id after cassio supports this
         rows = await self._table.aann_search(vector=vector, n=n)
         for row in rows:
-            chunks.add(BaseChunk(
-                doc_id=row["partition_id"],
-                chunk_id=row["row_id"][0],
-            ))
+            chunks.add(
+                Chunk(
+                    doc_id=row["partition_id"],
+                    chunk_id=row["row_id"][0],
+                )
+            )
         return list(chunks)
 
-    async def get_chunk_embeddings(self, chunk: BaseChunk) -> Tuple[BaseChunk, List[Tensor]]:
+    async def get_chunk_embedding(self, doc_id: str, chunk_id: int) -> Chunk:
         """
-        Retrieve all the embedding data for a chunk.
+        Retrieve the embedding data for a chunk.
 
         Returns:
-            A tuple where the first value is BaseChunk, and the second
-        value is the list of embeddings for the chunk.
+            A chunk with `doc_id`, `chunk_id`, and `embedding` set.
         """
 
-        row_id = (chunk.chunk_id, Predicate(PredicateOperator.GT, -1))
-        rows = await self._table.aget_partition(partition_id=chunk.doc_id, row_id=row_id)
+        row_id = (chunk_id, Predicate(PredicateOperator.GT, -1))
+        rows = await self._table.aget_partition(partition_id=doc_id, row_id=row_id)
 
-        embeddings = [torch.Tensor(row["vector"]) for row in rows]
+        embedding = [row["vector"] for row in rows]
 
-        return (chunk, embeddings)
+        return Chunk(doc_id=doc_id, chunk_id=chunk_id, embedding=embedding)
 
-    async def get_chunk_data(self, chunk: BaseChunk) -> Tuple[BaseChunk, ChunkData]:
+    async def get_chunk_data(
+        self, doc_id: str, chunk_id: int, include_embedding: Optional[bool]
+    ) -> Chunk:
         """
-        Fetches the text for a given chunk.
+        Retrieve the text and metadata for a chunk.
 
         Returns:
-            Tuple containing the chunk, and chunk_data
+            A chunk with `doc_id`, `chunk_id`, `text`, and `metadata` set.
         """
 
-        row_id = (chunk.chunk_id, Predicate(PredicateOperator.EQ, -1))
-        row = await self._table.aget(partition_id=chunk.doc_id, row_id=row_id)
+        row_id = (chunk_id, Predicate(PredicateOperator.EQ, -1))
+        row = await self._table.aget(partition_id=doc_id, row_id=row_id)
 
-        chunk_data = ChunkData(
+        if include_embedding is True:
+            embedded_chunk = await self.get_chunk_embedding(
+                doc_id=doc_id, chunk_id=chunk_id
+            )
+            embedding = embedded_chunk.embedding
+        else:
+            embedding = None
+
+        return Chunk(
+            doc_id=doc_id,
+            chunk_id=chunk_id,
             text=row["body_blob"],
-            metadata=row["metadata"]
+            metadata=row["metadata"],
+            embedding=embedding,
         )
-        return (chunk, chunk_data)
 
     def close(self) -> None:
         """
-        Closes the Cassandra session and any other resources. This method should be overridden to
-        ensure proper cleanup if necessary.
+        Cleans up any open resources.
         """
         pass
```

### Comparing `ragstack_ai_colbert-1.0.1/ragstack_colbert/colbert_retriever.py` & `ragstack_ai_colbert-1.0.2/ragstack_colbert/colbert_retriever.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,24 +7,22 @@
 to CPU computation if needed. This flexibility ensures that the retrieval system can be deployed in a
 variety of hardware environments.
 """
 
 import asyncio
 import logging
 import math
-import nest_asyncio
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 import torch
-from torch import Tensor
 
+from .base_database import BaseDatabase
 from .base_embedding_model import BaseEmbeddingModel
 from .base_retriever import BaseRetriever
-from .base_vector_store import BaseVectorStore
-from .objects import BaseChunk, ChunkData, RetrievedChunk
+from .objects import Chunk, Embedding, Vector
 
 
 def all_gpus_support_fp16(is_cuda: Optional[bool] = False):
     """
     Check if all available GPU devices support FP16 (half-precision) operations.
 
     Returns:
@@ -45,59 +43,61 @@
             return False
 
     # If all GPUs passed the check
     return True
 
 
 def max_similarity_torch(
-    query_vector: Tensor,
-    embedding_list: List[Tensor],
+    query_vector: Vector,
+    chunk_embedding: Embedding,
     is_cuda: Optional[bool] = False,
     is_fp16: Optional[bool] = False,
-) -> Tensor:
+) -> float:
     """
-    Calculates the maximum similarity (dot product) between a query vector and a list of embedding vectors,
+    Calculates the maximum similarity (dot product) between a query vector and a chunk embedding,
     leveraging PyTorch for efficient computation.
 
     Parameters:
-        query_vector (Tensor): A 1D tensor representing the query vector.
-        embedding_list (List[Tensor]): A list of 1D tensors, each representing an embedding vector.
+        query_vector (Vector): A list of float representing the query text.
+        chunk_embedding (Embedding): A list of Vector, each representing an chunk embedding vector.
         is_cuda (Optional[bool]): A flag indicating whether to use CUDA (GPU) for computation. Defaults to False.
         is_fp16 (bool): A flag indicating whether to half-precision floating point operations on CUDA (GPU).
                         Has no effect on CPU computation. Defaults to False.
 
     Returns:
         Tensor: A tensor containing the highest similarity score (dot product value) found between the query vector
                 and any of the embedding vectors in the list.
 
     Note:
         This function is designed to run on GPU for enhanced performance but can also execute on CPU.
     """
 
-    # Convert embedding list to a tensor
-    embedding_tensor = torch.stack(embedding_list)
+    # Convert inputs to tensors
+    query_tensor = torch.Tensor(query_vector)
+    embedding_tensor = torch.stack([torch.Tensor(v) for v in chunk_embedding])
 
     if is_cuda:
         device = torch.device("cuda")
-        query_vector = query_vector.to(device)
+        query_tensor = query_tensor.to(device)
         embedding_tensor = embedding_tensor.to(device)
 
         # Use half-precision operations if supported
         if is_fp16:
-            query_vector = query_vector.half()
+            query_tensor = query_tensor.half()
             embedding_tensor = embedding_tensor.half()
 
     # Perform the dot product operation
-    sims = torch.matmul(embedding_tensor, query_vector)
+    sims = torch.matmul(embedding_tensor, query_tensor)
 
     # Find the maximum similarity
     max_sim = torch.max(sims)
 
     # returns a tensor; the item() is the score
-    return max_sim
+    return float(max_sim.item())
+
 
 def get_trace(e: Exception) -> str:
     trace = ""
     tb = e.__traceback__
     while tb is not None:
         trace += f"\tFile: {tb.tb_frame.f_code.co_filename} Line: {tb.tb_lineno}\n"
         tb = tb.tb_next
@@ -118,227 +118,294 @@
                         Has no effect on CPU computation.
 
     Note:
         The class is designed to work with a GPU for optimal performance but will automatically fall back to CPU
         computation if a GPU is not available.
     """
 
-    vector_store: BaseVectorStore
-    embedding_model: BaseEmbeddingModel
-    is_cuda: bool = False
-    is_fp16: bool = False
+    _database: BaseDatabase
+    _embedding_model: BaseEmbeddingModel
+    _is_cuda: bool
+    _is_fp16: bool
 
     class Config:
         arbitrary_types_allowed = True
 
     def __init__(
         self,
-        vector_store: BaseVectorStore,
+        database: BaseDatabase,
         embedding_model: BaseEmbeddingModel,
     ):
         """
         Initializes the retriever with a specific vector store and Colbert embeddings model.
 
         Parameters:
-            vector_store (BaseVectorStore): The vector store to be used for retrieving embeddings.
+            database (BaseDatabase): The data store to be used for retrieving embeddings.
             embedding_model (BaseEmbeddingModel): The ColBERT embeddings model to be used for encoding
                                                          queries.
         """
 
-        self.vector_store = vector_store
-        self.embedding_model = embedding_model
-        self.is_cuda = torch.cuda.is_available()
-        self.is_fp16 = all_gpus_support_fp16(self.is_cuda)
+        self._database = database
+        self._embedding_model = embedding_model
+        self._is_cuda = torch.cuda.is_available()
+        self._is_fp16 = all_gpus_support_fp16(self._is_cuda)
 
     def close(self) -> None:
         """
         Closes any open resources held by the retriever.
         """
         pass
 
     async def _query_relevant_chunks(
-        self, query_embeddings: List[Tensor], top_k: int
-    ) -> Set[BaseChunk]:
+        self, query_embedding: Embedding, top_k: int
+    ) -> Set[Chunk]:
         """
-        Retrieves the top_k ANN results for each embedded query token.
+        Retrieves the top_k ANN Chunks (`doc_id` and `chunk_id` only) for each embedded query token.
         """
-        chunks: Set[BaseChunk] = set()
+        chunks: Set[Chunk] = set()
         # Collect all tasks
-        tasks = [self.vector_store.search_relevant_chunks(vector=v, n=top_k) for v in query_embeddings]
+        tasks = [
+            self._database.search_relevant_chunks(vector=v, n=top_k)
+            for v in query_embedding
+        ]
         results = await asyncio.gather(*tasks, return_exceptions=True)
 
         # Process results and handle potential exceptions
         for result in results:
             if isinstance(result, Exception):
-                logging.error(f"Issue on vector_store.get_relevant_chunks(): {result} at {get_trace(result)}")
+                logging.error(
+                    f"Issue on database.get_relevant_chunks(): {result} at {get_trace(result)}"
+                )
             else:
                 chunks.update(result)
 
         return chunks
 
-    async def _retrieve_chunks(
-        self, chunks: Set[BaseChunk]
-    ) -> Dict[BaseChunk, List[Tensor]]:
+    async def _get_chunk_embeddings(self, chunks: Set[Chunk]) -> List[Chunk]:
         """
-        Retrieves embeddings for a list of chunks, returning a dictionary mapping chunk to a list of PyTorch tensors.
+        Retrieves Chunks with `doc_id`, `chunk_id`, and `embedding` set.
         """
-        chunk_embeddings: Dict[BaseChunk, List[Tensor]] = {}
-
         # Collect all tasks
-        tasks = [self.vector_store.get_chunk_embeddings(chunk) for chunk in chunks]
+        tasks = [
+            self._database.get_chunk_embedding(doc_id=c.doc_id, chunk_id=c.chunk_id)
+            for c in chunks
+        ]
         results = await asyncio.gather(*tasks, return_exceptions=True)
 
         # Process results and handle potential exceptions
         for result in results:
             if isinstance(result, Exception):
-                logging.error(f"Issue on vector_store.get_chunk_embeddings(): {result} at {get_trace(result)}")
-            else:
-                chunk, embeddings = result
-                chunk_embeddings[chunk] = embeddings
+                logging.error(
+                    f"Issue on database.get_chunk_embeddings(): {result} at {get_trace(result)}"
+                )
 
-        return chunk_embeddings
+        return results
 
     def _score_chunks(
-        self, query_embeddings: Tensor, chunk_data: Dict[BaseChunk, List[Tensor]]
-    ) -> Dict[BaseChunk, Tensor]:
+        self, query_embedding: Embedding, chunk_embeddings: List[Chunk]
+    ) -> Dict[Chunk, float]:
         """
         Process the retrieved chunk data to calculate scores.
         """
         chunk_scores = {}
-        for chunk, embeddings in chunk_data.items():
+        for chunk in chunk_embeddings:
             chunk_scores[chunk] = sum(
                 max_similarity_torch(
-                    query_vector=qv,
-                    embedding_list=embeddings,
-                    is_cuda=self.is_cuda,
-                    is_fp16=self.is_fp16,
+                    query_vector=query_vector,
+                    chunk_embedding=chunk.embedding,
+                    is_cuda=self._is_cuda,
+                    is_fp16=self._is_fp16,
                 )
-                for qv in query_embeddings
+                for query_vector in query_embedding
             )
         return chunk_scores
 
-    async def _fetch_chunk_data(
+    async def _get_chunk_data(
         self,
-        chunks_by_score: List[BaseChunk],
-        chunk_scores:  Dict[BaseChunk, Tensor],
-    ) -> List[RetrievedChunk]:
+        chunks: List[Chunk],
+        include_embedding: Optional[bool] = False,
+    ) -> List[Chunk]:
         """
-        Fetches text and metadata for each chunk and ranks them based on scores.
-
-        Parameters:
-            chunks_by_score (List[Tuple[str, int]]): List of tuples containing (doc_id, chunk_id) sorted by score.
-            chunk_scores (Dict[Tuple[str, int], Tensor]): Dictionary mapping (doc_id, chunk_id) to their respective scores.
+        Fetches text and metadata for each chunk.
 
         Returns:
-            List[RetrievedChunk]: A list of RetrievedChunk objects with populated fields.
+            List[Chunk]: A list of chunks with `doc_id`, `chunk_id`, `text`, `metadata`, and optionally `embedding` set.
         """
 
         # Collect all tasks
-        tasks = [self.vector_store.get_chunk_data(chunk=chunk) for chunk in chunks_by_score]
+        tasks = [
+            self._database.get_chunk_data(
+                doc_id=c.doc_id,
+                chunk_id=c.chunk_id,
+                include_embedding=include_embedding,
+            )
+            for c in chunks
+        ]
         results = await asyncio.gather(*tasks, return_exceptions=True)
 
-        # Process results and handle potential exceptions
-        chunk_data_map: Dict[BaseChunk, ChunkData] = {}
         for result in results:
             if isinstance(result, Exception):
-                logging.error(f"Issue on vector_store.get_chunk_text_and_metadata(): {result} at {get_trace(result)}")
-            else:
-                chunk, chunk_data = result
-                chunk_data_map[chunk] = chunk_data
-
-        answers: List[RetrievedChunk] = []
-
-        for idx, chunk in enumerate(chunks_by_score):
-            score = chunk_scores[chunk]
-            chunk_data = chunk_data_map[chunk]
-            answers.append(
-                    RetrievedChunk(
-                        doc_id=chunk.doc_id,
-                        chunk_id=chunk.chunk_id,
-                        score=score.item(),  # Ensure score is a scalar if it's a tensor
-                        rank=idx + 1,
-                        data=chunk_data,
-                    )
+                logging.error(
+                    f"Issue on database.get_chunk_data(): {result} at {get_trace(result)}"
                 )
 
-        return answers
+        return results
 
-    async def aretrieve(
+    async def atext_search(
         self,
-        query: str,
-        k: int = 10,
-        query_maxlen: int = 64,
+        query_text: str,
+        k: Optional[int] = 5,
+        query_maxlen: Optional[int] = None,
+        include_embedding: Optional[bool] = False,
         **kwargs: Any,
-    ) -> List[RetrievedChunk]:
+    ) -> List[Tuple[Chunk, float]]:
         """
         Retrieves a list of text chunks most relevant to the given query, using semantic similarity as the criteria.
 
         Parameters:
-            query (str): The text query for which relevant chunks are to be retrieved.
-            k (int, optional): The number of top relevant chunks to retrieve. Defaults to 10.
-            query_maxlen (int, optional): The maximum number of tokens in the query. If -1, this will be calculated dynamically.
-            query_timeout (int, optional): The timeout in seconds for query execution. Defaults to 180.
-            **kwargs (Any): Additional keyword arguments that can be used for extending functionality.
+            query_text (str): The query text to search for relevant text chunks.
+            k (Optional[int]): The number of top results to retrieve. Default 5.
+            query_maxlen (Optional[int]): The maximum length of the query to consider. If None, the
+                                          maxlen will be dynamically generated.
+            include_embedding (Optional[bool]): Optional (default False) flag to include the
+                                                embedding vectors in the returned chunks
+            **kwargs (Any): Additional parameters that implementations might require for customized
+                            retrieval operations.
 
         Returns:
-            List[RetrievedChunk]: A list of RetrievedChunk objects, each representing a text chunk that is relevant
-                                  to the query, along with its similarity score and rank.
+            List[Tuple[Chunk, float]]: A list of retrieved Chunk, float Tuples, each representing a text chunk that is relevant
+                                  to the query, along with its similarity score.
+        """
+
+        query_embedding = self._embedding_model.embed_query(
+            query=query_text, query_maxlen=query_maxlen
+        )
+
+        return await self.aembedding_search(
+            query_embedding=query_embedding,
+            k=k,
+            include_embedding=include_embedding,
+            **kwargs,
+        )
 
-        Note:
-            The actual retrieval process involves encoding the query, performing an ANN search to find relevant
-            embeddings, scoring these embeddings for similarity, and retrieving the corresponding text chunks.
+    async def aembedding_search(
+        self,
+        query_embedding: Embedding,
+        k: Optional[int] = 5,
+        include_embedding: Optional[bool] = False,
+        **kwargs: Any,
+    ) -> List[Tuple[Chunk, float]]:
         """
+        Retrieves a list of text chunks most relevant to the given query, using semantic similarity as the criteria.
+
+        Parameters:
+            query_embedding (Embedding): The query embedding to search for relevant text chunks.
+            k (Optional[int]): The number of top results to retrieve. Default 5.
+            include_embedding (Optional[bool]): Optional (default False) flag to include the
+                                                embedding vectors in the returned chunks
+            **kwargs (Any): Additional parameters that implementations might require for customized
+                            retrieval operations.
 
-        query_embeddings = self.embedding_model.embed_query(
-            query, query_maxlen=query_maxlen
+        Returns:
+            List[Tuple[Chunk, float]]: A list of retrieved Chunk, float Tuples, each representing a text chunk that is relevant
+                                  to the query, along with its similarity score.
+        """
+
+        top_k = max(math.floor(len(query_embedding) / 2), 16)
+        logging.debug(
+            f"based on query length of {len(query_embedding)} tokens, retrieving {top_k} results per token-embedding"
         )
 
-        top_k = max(math.floor(len(query_embeddings) / 2), 16)
-        logging.debug(f"based on query length of {len(query_embeddings)} tokens, retrieving {top_k} results per token-embedding")
+        # search for relevant chunks (only with `doc_id` and `chunk_id` set)
+        relevant_chunks: List[Chunk] = await self._query_relevant_chunks(
+            query_embedding=query_embedding, top_k=top_k
+        )
 
-        chunks = await self._query_relevant_chunks(
-            query_embeddings=query_embeddings, top_k=top_k
+        # get the embedding for each chunk (with `doc_id`, `chunk_id`, and `embedding` set)
+        chunk_embeddings: List[Chunk] = await self._get_chunk_embeddings(
+            chunks=relevant_chunks
         )
 
-        # score each chunk
-        chunk_data = await self._retrieve_chunks(chunks=chunks)
-        chunk_scores = self._score_chunks(
-            query_embeddings=query_embeddings, chunk_data=chunk_data
+        # score the chunks using max_similarity
+        chunk_scores: Dict[Chunk, float] = self._score_chunks(
+            query_embedding=query_embedding,
+            chunk_embeddings=chunk_embeddings,
         )
 
-        # load the source chunk for the top k documents
-        chunks_by_score = sorted(chunk_scores, key=chunk_scores.get, reverse=True)[:k]
+        # only keep the top k sorted results
+        top_k_chunks: List[Chunk] = sorted(
+            chunk_scores, key=chunk_scores.get, reverse=True
+        )[:k]
 
-        answers = await self._fetch_chunk_data(
-            chunks_by_score=chunks_by_score, chunk_scores=chunk_scores
+        chunks: List[Chunk] = await self._get_chunk_data(
+            chunks=top_k_chunks, include_embedding=include_embedding
         )
-        return answers
 
-    def retrieve(
+        return [(chunk, chunk_scores[chunk]) for chunk in chunks]
+
+    def text_search(
         self,
-        query: str,
-        k: int = 10,
-        query_maxlen: int = 64,
+        query_text: str,
+        k: Optional[int] = 5,
+        query_maxlen: Optional[int] = None,
+        include_embedding: Optional[bool] = False,
         **kwargs: Any,
-    ) -> List[RetrievedChunk]:
+    ) -> List[Tuple[Chunk, float]]:
         """
-        Retrieves a list of text chunks most relevant to the given query, using semantic similarity as the criteria.
+        Retrieves a list of text chunks relevant to a given query from the vector store, ranked by
+        relevance or other metrics.
 
         Parameters:
-            query (str): The text query for which relevant chunks are to be retrieved.
-            k (int, optional): The number of top relevant chunks to retrieve. Defaults to 10.
-            query_maxlen (int, optional): //TODO figure out a better description for this parameter, and/or a better name.
-            **kwargs (Any): Additional keyword arguments that can be used for extending functionality.
+            query_text (str): The query text to search for relevant text chunks.
+            k (Optional[int]): The number of top results to retrieve. Default 5.
+            query_maxlen (Optional[int]): The maximum length of the query to consider. If None, the
+                                          maxlen will be dynamically generated.
+            include_embedding (Optional[bool]): Optional (default False) flag to include the
+                                                embedding vectors in the returned chunks
+            **kwargs (Any): Additional parameters that implementations might require for customized
+                            retrieval operations.
 
         Returns:
-            List[RetrievedChunk]: A list of RetrievedChunk objects, each representing a text chunk that is relevant
-                                  to the query, along with its similarity score and rank.
+            List[Tuple[Chunk, float]]: A list of retrieved Chunk, float Tuples, each representing a text chunk that is relevant
+                                  to the query, along with its similarity score.
+        """
 
-        Note:
-            The actual retrieval process involves encoding the query, performing an ANN search to find relevant
-            embeddings, scoring these embeddings for similarity, and retrieving the corresponding text chunks.
-        """
-        # nest_asyncio does not a new event loop to be created
-        # in the case there is already an event loop such as colab, it's required
-        nest_asyncio.apply()
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(self.aretrieve(query=query, k=k, query_maxlen=query_maxlen))
+        return asyncio.run(
+            self.atext_search(
+                query_text=query_text,
+                k=k,
+                query_maxlen=query_maxlen,
+                include_embedding=include_embedding,
+            )
+        )
+
+    def embedding_search(
+        self,
+        query_embedding: Embedding,
+        k: Optional[int] = 5,
+        include_embedding: Optional[bool] = False,
+        **kwargs: Any,
+    ) -> List[Tuple[Chunk, float]]:
+        """
+        Retrieves a list of text chunks relevant to a given query from the vector store, ranked by
+        relevance or other metrics.
+
+        Parameters:
+            query_embedding (Embedding): The query embedding to search for relevant text chunks.
+            k (Optional[int]): The number of top results to retrieve. Default 5.
+            include_embedding (Optional[bool]): Optional (default False) flag to include the
+                                                embedding vectors in the returned chunks
+            **kwargs (Any): Additional parameters that implementations might require for customized
+                            retrieval operations.
+
+        Returns:
+            List[Tuple[Chunk, float]]: A list of retrieved Chunk, float Tuples, each representing a text chunk that is relevant
+                                  to the query, along with its similarity score.
+        """
+
+        return asyncio.run(
+            self.aembedding_search(
+                query_embedding=query_embedding,
+                k=k,
+                include_embedding=include_embedding,
+            )
+        )
```

### Comparing `ragstack_ai_colbert-1.0.1/ragstack_colbert/constant.py` & `ragstack_ai_colbert-1.0.2/ragstack_colbert/constant.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,9 +10,7 @@
 """
 
 DEFAULT_COLBERT_MODEL = "colbert-ir/colbertv2.0"
 
 DEFAULT_COLBERT_DIM = 128
 
 MAX_MODEL_TOKENS = 512
-
-CHUNK_MAX_PER_DOC = 100000000
```

### Comparing `ragstack_ai_colbert-1.0.1/PKG-INFO` & `ragstack_ai_colbert-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-colbert
-Version: 1.0.1
+Version: 1.0.2
 Summary: DataStax RAGStack Colbert implementation
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cassio (>=0.1.7,<0.2.0)
 Requires-Dist: colbert-ai (==0.2.19)
-Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
 Requires-Dist: pyarrow (==14.0.1)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: torch (==2.2.1)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack ColBERT
```

