# Comparing `tmp/grand-graph-0.5.0.tar.gz` & `tmp/grand-graph-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grand-graph-0.5.0.tar", last modified: Wed Apr 17 13:57:38 2024, max compression
+gzip compressed data, was "grand-graph-0.5.1.tar", last modified: Mon May 13 12:15:19 2024, max compression
```

## Comparing `grand-graph-0.5.0.tar` & `grand-graph-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.291848 grand-graph-0.5.0/
--rw-r--r--   0 mateljk1   (501) staff       (20)    10140 2024-04-17 13:53:45.000000 grand-graph-0.5.0/LICENSE
--rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-04-17 13:57:38.291674 grand-graph-0.5.0/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)     5268 2024-04-17 13:53:45.000000 grand-graph-0.5.0/README.md
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.225326 grand-graph-0.5.0/grand/
--rw-r--r--   0 mateljk1   (501) staff       (20)     2378 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/__init__.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.227855 grand-graph-0.5.0/grand/backends/
--rw-r--r--   0 mateljk1   (501) staff       (20)      572 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    15497 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_dataframe.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    16291 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_dynamodb.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     8762 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_gremlin.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     7200 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_igraph.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     8963 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_networkit.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     5335 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_networkx.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    20274 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/_sqlbackend.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    10763 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/backend.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1915 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/metadatastore.py
--rw-r--r--   0 mateljk1   (501) staff       (20)    12799 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_backends.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     2467 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_cached_backend.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     1411 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/backends/test_metadatastore.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.228231 grand-graph-0.5.0/grand/dialects/
--rw-r--r--   0 mateljk1   (501) staff       (20)     8702 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/dialects/__init__.py
--rw-r--r--   0 mateljk1   (501) staff       (20)     5411 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/dialects/test_dialect.py
--rw-r--r--   0 mateljk1   (501) staff       (20)      405 2024-04-17 13:53:45.000000 grand-graph-0.5.0/grand/test_graph.py
-drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-04-17 13:57:38.229103 grand-graph-0.5.0/grand_graph.egg-info/
--rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/PKG-INFO
--rw-r--r--   0 mateljk1   (501) staff       (20)      685 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/SOURCES.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/dependency_links.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)      132 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/requires.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)        6 2024-04-17 13:57:38.000000 grand-graph-0.5.0/grand_graph.egg-info/top_level.txt
--rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-04-17 13:57:38.291907 grand-graph-0.5.0/setup.cfg
--rw-r--r--   0 mateljk1   (501) staff       (20)      892 2024-04-17 13:57:23.000000 grand-graph-0.5.0/setup.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-13 12:15:19.908448 grand-graph-0.5.1/
+-rw-r--r--   0 mateljk1   (501) staff       (20)    10140 2024-04-17 13:53:45.000000 grand-graph-0.5.1/LICENSE
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-05-13 12:15:19.908197 grand-graph-0.5.1/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5268 2024-04-17 13:53:45.000000 grand-graph-0.5.1/README.md
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-13 12:15:19.901892 grand-graph-0.5.1/grand/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2378 2024-05-13 12:14:44.000000 grand-graph-0.5.1/grand/__init__.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-13 12:15:19.905713 grand-graph-0.5.1/grand/backends/
+-rw-r--r--   0 mateljk1   (501) staff       (20)      572 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/backends/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    15916 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_dataframe.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    16724 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_dynamodb.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     9030 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_gremlin.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     7454 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_igraph.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     9209 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_networkit.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5549 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/_networkx.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    20944 2024-05-13 12:13:17.000000 grand-graph-0.5.1/grand/backends/_sqlbackend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    11462 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/backends/backend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1915 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/backends/metadatastore.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)    14591 2024-05-13 12:13:17.000000 grand-graph-0.5.1/grand/backends/test_backends.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     2467 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/backends/test_cached_backend.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     1411 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/backends/test_metadatastore.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-13 12:15:19.906376 grand-graph-0.5.1/grand/dialects/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     9181 2024-05-04 13:36:34.000000 grand-graph-0.5.1/grand/dialects/__init__.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5411 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/dialects/test_dialect.py
+-rw-r--r--   0 mateljk1   (501) staff       (20)      405 2024-04-17 13:53:45.000000 grand-graph-0.5.1/grand/test_graph.py
+drwxr-xr-x   0 mateljk1   (501) staff       (20)        0 2024-05-13 12:15:19.907706 grand-graph-0.5.1/grand_graph.egg-info/
+-rw-r--r--   0 mateljk1   (501) staff       (20)     5790 2024-05-13 12:15:19.000000 grand-graph-0.5.1/grand_graph.egg-info/PKG-INFO
+-rw-r--r--   0 mateljk1   (501) staff       (20)      685 2024-05-13 12:15:19.000000 grand-graph-0.5.1/grand_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        1 2024-05-13 12:15:19.000000 grand-graph-0.5.1/grand_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)      132 2024-05-13 12:15:19.000000 grand-graph-0.5.1/grand_graph.egg-info/requires.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)        6 2024-05-13 12:15:19.000000 grand-graph-0.5.1/grand_graph.egg-info/top_level.txt
+-rw-r--r--   0 mateljk1   (501) staff       (20)       38 2024-05-13 12:15:19.908533 grand-graph-0.5.1/setup.cfg
+-rw-r--r--   0 mateljk1   (501) staff       (20)      892 2024-05-13 12:14:47.000000 grand-graph-0.5.1/setup.py
```

### Comparing `grand-graph-0.5.0/LICENSE` & `grand-graph-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/PKG-INFO` & `grand-graph-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-graph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Graph database wrapper for non-graph datastores
 Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: grand-graph Version: 0.5.0 Summary: Graph database
+Metadata-Version: 2.1 Name: grand-graph Version: 0.5.1 Summary: Graph database
 wrapper for non-graph datastores Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky Author-email: opensource@matelsky.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: sql Provides-Extra: dynamodb Provides-
 Extra: igraph Provides-Extra: networkit License-File: LICENSE
                                [docs/grand.png]
```

### Comparing `grand-graph-0.5.0/README.md` & `grand-graph-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand/__init__.py` & `grand-graph-0.5.1/grand/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 from .backends import Backend, NetworkXBackend
 from .dialects import NetworkXDialect, IGraphDialect, NetworkitDialect
 
 
 _DEFAULT_BACKEND = NetworkXBackend
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 
 class Graph:
     """
     A grand.Graph enables you to manipulate a graph using multiple dialects.
 
     """
```

### Comparing `grand-graph-0.5.0/grand/backends/__init__.py` & `grand-graph-0.5.1/grand/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand/backends/_dataframe.py` & `grand-graph-0.5.1/grand/backends/_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,19 +116,21 @@
         Returns:
             Generator: A generator of all nodes (arbitrary sort)
 
         """
         if self._node_df is not None:
             return [
                 (
-                    node_id,
-                    row.to_dict(),
+                    (
+                        node_id,
+                        row.to_dict(),
+                    )
+                    if include_metadata
+                    else node_id
                 )
-                if include_metadata
-                else node_id
                 for node_id, row in self._node_df.iterrows()
             ]
 
         else:
             return [
                 (node_id, {}) if include_metadata else node_id
                 for node_id in self._edge_df[self._edge_df_source_column]
@@ -283,22 +285,20 @@
             v (Hashable): The target node ID
 
         Returns:
             dict: Metadata associated with this edge
 
         """
         if self._directed:
-            return (
-                self._edge_df[
-                    (self._edge_df[self._edge_df_source_column] == u)
-                    & (self._edge_df[self._edge_df_target_column] == v)
-                ]
-                .iloc[0]
-                .to_dict()
-            )
+            result = self._edge_df[
+                (self._edge_df[self._edge_df_source_column] == u)
+                & (self._edge_df[self._edge_df_target_column] == v)
+            ]
+            if len(result):
+                return self._edge_as_dict(result.iloc[0])
 
         else:
             left = self._edge_df[
                 (self._edge_df[self._edge_df_source_column] == u)
                 & (self._edge_df[self._edge_df_target_column] == v)
             ]
             if len(left):
@@ -351,17 +351,19 @@
                         (self._edge_df[self._edge_df_source_column] == u)
                     ].iterrows()
                 ]
             )
         else:
             return iter(
                 [
-                    row[self._edge_df_source_column]
-                    if row[self._edge_df_source_column] != u
-                    else row[self._edge_df_target_column]
+                    (
+                        row[self._edge_df_source_column]
+                        if row[self._edge_df_source_column] != u
+                        else row[self._edge_df_target_column]
+                    )
                     for _, row in self._edge_df[
                         (self._edge_df[self._edge_df_source_column] == u)
                         | (self._edge_df[self._edge_df_target_column] == u)
                     ].iterrows()
                 ]
             )
 
@@ -426,17 +428,19 @@
                         (self._edge_df[self._edge_df_target_column] == u)
                     ].iterrows()
                 ]
             )
         else:
             return iter(
                 [
-                    row[self._edge_df_source_column]
-                    if row[self._edge_df_target_column] != u
-                    else row[self._edge_df_target_column]
+                    (
+                        row[self._edge_df_source_column]
+                        if row[self._edge_df_target_column] != u
+                        else row[self._edge_df_target_column]
+                    )
                     for _, row in self._edge_df[
                         (self._edge_df[self._edge_df_target_column] == u)
                         | (self._edge_df[self._edge_df_source_column] == u)
                     ].iterrows()
                 ]
             )
 
@@ -456,14 +460,27 @@
         # Return number of unique sources intersected with number of unique targets
         return len(
             set(self._edge_df[self._edge_df_source_column]).intersection(
                 set(self._edge_df[self._edge_df_target_column])
             )
         )
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return len(self._edge_df)
+
     def ingest_from_edgelist_dataframe(
         self, edgelist: pd.DataFrame, source_column: str, target_column: str
     ) -> dict:
         """
         Ingest an edgelist from a Pandas DataFrame.
 
         """
```

### Comparing `grand-graph-0.5.0/grand/backends/_dynamodb.py` & `grand-graph-0.5.1/grand/backends/_dynamodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,19 +187,21 @@
 
         Returns:
             Generator: A generator of all nodes (arbitrary sort)
 
         """
         return [
             (
-                node[self._primary_key],
-                {k: v for k, v in node.items() if k not in [self._primary_key]},
+                (
+                    node[self._primary_key],
+                    {k: v for k, v in node.items() if k not in [self._primary_key]},
+                )
+                if include_metadata
+                else node[self._primary_key]
             )
-            if include_metadata
-            else node[self._primary_key]
             for node in self._scan_table(self._node_table)
         ]
 
     def has_node(self, u: Hashable) -> bool:
         """
         Return true if the node exists in the graph.
 
@@ -260,17 +262,19 @@
             include_metadata (bool: False): Whether to include edge metadata
 
         Returns:
             Generator: A generator of all edges (arbitrary sort)
 
         """
         return [
-            (edge[self._edge_source_key], edge[self._edge_target_key], edge)
-            if include_metadata
-            else (edge[self._edge_source_key], edge[self._edge_target_key])
+            (
+                (edge[self._edge_source_key], edge[self._edge_target_key], edge)
+                if include_metadata
+                else (edge[self._edge_source_key], edge[self._edge_target_key])
+            )
             for edge in self._scan_table(self._edge_table)
         ]
 
     def get_node_by_id(self, node_name: Hashable):
         """
         Return the data associated with a node.
 
@@ -431,14 +435,29 @@
             int: The count of nodes
 
         """
         return self._client.describe_table(TableName=self._node_table_name)["Table"][
             "ItemCount"
         ]
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return self._client.describe_table(TableName=self._edge_table_name)["Table"][
+            "ItemCount"
+        ]
+
     # Ingesting
 
     def ingest_from_edgelist_dataframe(
         self, edgelist: pd.DataFrame, source_column: str, target_column: str
     ) -> dict:
         """
         Ingest an edgelist from a Pandas DataFrame.
```

### Comparing `grand-graph-0.5.0/grand/backends/_gremlin.py` & `grand-graph-0.5.1/grand/backends/_gremlin.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,9 +310,22 @@
 
         Returns:
             int: The count of nodes
 
         """
         return self._g.V().count().toList()[0]
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return self._g.E().count().toList()[0]
+
     def teardown(self) -> None:
         self._g.V().drop().toList()
```

### Comparing `grand-graph-0.5.0/grand/backends/_igraph.py` & `grand-graph-0.5.1/grand/backends/_igraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -254,7 +254,20 @@
             None
 
         Returns:
             int: The count of nodes
 
         """
         return self._ig.vcount()
+
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return self._ig.ecount()
```

### Comparing `grand-graph-0.5.0/grand/backends/_networkit.py` & `grand-graph-0.5.1/grand/backends/_networkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -277,19 +277,32 @@
                         val[v] = self._meta.get_edge(v, u)
             return val
 
         return iter(
             [self._names.get_name(i) for i in self._nk_graph.iterInNeighbors(my_id)]
         )
 
-    def get_node_count(self) -> Iterable:
+    def get_node_count(self) -> int:
         """
         Get an integer count of the number of nodes in this graph.
 
         Arguments:
             None
 
         Returns:
             int: The count of nodes
 
         """
-        return len([i for i in self.all_nodes_as_iterable()])
+        return self._nk_graph.numberOfNodes()
+
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return self._nk_graph.numberOfEdges()
```

### Comparing `grand-graph-0.5.0/grand/backends/_networkx.py` & `grand-graph-0.5.1/grand/backends/_networkx.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,14 +164,27 @@
 
         Returns:
             int: The count of nodes
 
         """
         return len(self._nx_graph)
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return len(self._nx_graph.edges)
+
     def ingest_from_edgelist_dataframe(
         self, edgelist: pd.DataFrame, source_column: str, target_column: str
     ) -> dict:
         """
         Ingest an edgelist from a Pandas DataFrame.
 
         """
@@ -196,10 +209,7 @@
 
         return {
             "node_count": len(nodes),
             "node_duration": 0,
             "edge_count": len(edgelist),
             "edge_duration": time.time() - tic,
         }
-
-    def teardown(self) -> None:
-        return
```

### Comparing `grand-graph-0.5.0/grand/backends/_sqlbackend.py` & `grand-graph-0.5.1/grand/backends/_sqlbackend.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,33 +70,33 @@
                 primary_key=True,
             ),
             sqlalchemy.Column("_metadata", sqlalchemy.JSON),
         )
         self._node_table.create(self._engine, checkfirst=True)
 
         source_column = sqlalchemy.Column(
-                self._edge_source_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
+            self._edge_source_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
         )
 
         target_column = sqlalchemy.Column(
-                self._edge_target_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
+            self._edge_target_key, sqlalchemy.String(_DEFAULT_SQL_STR_LEN)
         )
 
         # Create edges table
         self._edge_table = sqlalchemy.Table(
             self._edge_table_name,
             self._metadata,
             sqlalchemy.Column(
                 self._primary_key,
                 sqlalchemy.String(_DEFAULT_SQL_STR_LEN),
                 primary_key=True,
             ),
             sqlalchemy.Column("_metadata", sqlalchemy.JSON),
             source_column,
-            target_column
+            target_column,
         )
         self._edge_table.create(self._engine, checkfirst=True)
 
         # Create source and target index
         sindex = Index("edge_source", source_column)
         sindex.create(self._engine, checkfirst=True)
 
@@ -152,18 +152,21 @@
             self._connection.execute(
                 self._node_table.insert(),
                 parameters={self._primary_key: node_name, "_metadata": metadata},
             )
         return node_name
 
     def add_nodes_from(self, nodes_for_adding, **attr):
-        nodes = [{
-            self._primary_key: node,
-            "_metadata": {**attr, **metadata},
-        } for node, metadata in nodes_for_adding]
+        nodes = [
+            {
+                self._primary_key: node,
+                "_metadata": {**attr, **metadata},
+            }
+            for node, metadata in nodes_for_adding
+        ]
 
         self._connection.execute(self._node_table.insert(), nodes)
 
     def _upsert_node(self, node_name: Hashable, metadata: dict) -> Hashable:
         """
         Add a new node to the graph, or update an existing one.
 
@@ -200,15 +203,17 @@
         Returns:
             Generator: A generator of all nodes (arbitrary sort)
 
         """
         if include_metadata:
             sql = self._node_table.select()
         else:
-            sql = self._node_table.select().with_only_columns(self._node_table.c[self._primary_key])
+            sql = self._node_table.select().with_only_columns(
+                self._node_table.c[self._primary_key]
+            )
 
         results = []
         for x in self._connection.execute(sql):
             results.append(x if include_metadata else x[0])
 
         return results
 
@@ -273,20 +278,23 @@
                 ),
                 parameters={"_metadata": existing_metadata},
             )
 
         return pk
 
     def add_edges_from(self, ebunch_to_add, **attr):
-        edges = [{
-            self._primary_key: f"__{u}__{v}",
-            self._edge_source_key: u,
-            self._edge_target_key: v,
-            "_metadata": {**attr, **metadata},
-        } for u, v, metadata in ebunch_to_add]
+        edges = [
+            {
+                self._primary_key: f"__{u}__{v}",
+                self._edge_source_key: u,
+                self._edge_target_key: v,
+                "_metadata": {**attr, **metadata},
+            }
+            for u, v, metadata in ebunch_to_add
+        ]
 
         self._connection.execute(self._edge_table.insert(), edges)
 
     def all_edges_as_iterable(self, include_metadata: bool = False) -> Generator:
         """
         Get a list of all edges in this graph, arbitrary sort.
 
@@ -295,15 +303,15 @@
 
         Returns:
             Generator: A generator of all edges (arbitrary sort)
         """
 
         columns = [
             self._node_table.c[self._edge_source_key],
-            self._node_table.c[self._edge_target_key]
+            self._node_table.c[self._edge_target_key],
         ]
 
         if include_metadata:
             columns.append(self._node_table.c["_metadata"])
 
         sql = self._node_table.select().with_only_columns(columns)
         return self._connection.execute(sql).fetchall()
@@ -341,36 +349,34 @@
 
         Returns:
             dict: Metadata associated with this edge
 
         """
         if self._directed:
             pk = f"__{u}__{v}"
-            return (
-                self._connection.execute(
-                    self._edge_table.select().where(
-                        self._edge_table.c[self._primary_key] == pk
-                    )
+            result = self._connection.execute(
+                self._edge_table.select().where(
+                    self._edge_table.c[self._primary_key] == pk
                 )
-                .fetchone()
-                ._metadata
-            )
+            ).fetchone()
+            if result:
+                return result._metadata
+            raise KeyError(f"Edge {u}-{v} not found.")
         else:
-            return (
-                self._connection.execute(
-                    self._edge_table.select().where(
-                        or_(
-                            (self._edge_table.c[self._primary_key] == f"__{u}__{v}"),
-                            (self._edge_table.c[self._primary_key] == f"__{v}__{u}"),
-                        )
+            result = self._connection.execute(
+                self._edge_table.select().where(
+                    or_(
+                        (self._edge_table.c[self._primary_key] == f"__{u}__{v}"),
+                        (self._edge_table.c[self._primary_key] == f"__{v}__{u}"),
                     )
                 )
-                .fetchone()
-                ._metadata
-            )
+            ).fetchone()
+            if result:
+                return result._metadata
+            raise KeyError(f"Edge {u}-{v} not found.")
 
     def get_node_neighbors(
         self, u: Hashable, include_metadata: bool = False
     ) -> Generator:
         """
         Get a generator of all downstream nodes from this node.
 
@@ -380,26 +386,28 @@
         Returns:
             Generator
 
         """
 
         if self._directed:
             res = self._connection.execute(
-                self._edge_table.select().where(
-                    self._edge_table.c[self._edge_source_key] == str(u)
-                ).order_by(self._edge_table.c[self._primary_key])
+                self._edge_table.select()
+                .where(self._edge_table.c[self._edge_source_key] == str(u))
+                .order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
         else:
             res = self._connection.execute(
-                self._edge_table.select().where(
+                self._edge_table.select()
+                .where(
                     or_(
                         (self._edge_table.c[self._edge_source_key] == str(u)),
                         (self._edge_table.c[self._edge_target_key] == str(u)),
                     )
-                ).order_by(self._edge_table.c[self._primary_key])
+                )
+                .order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
 
         res = [x._asdict() for x in res]
 
         if include_metadata:
             return {
                 (
@@ -432,26 +440,28 @@
 
         Returns:
             Generator
 
         """
         if self._directed:
             res = self._connection.execute(
-                self._edge_table.select().where(
-                    self._edge_table.c[self._edge_target_key] == str(u)
-                ).order_by(self._edge_table.c[self._primary_key])
+                self._edge_table.select()
+                .where(self._edge_table.c[self._edge_target_key] == str(u))
+                .order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
         else:
             res = self._connection.execute(
-                self._edge_table.select().where(
+                self._edge_table.select()
+                .where(
                     or_(
                         (self._edge_table.c[self._edge_target_key] == str(u)),
                         (self._edge_table.c[self._edge_source_key] == str(u)),
                     )
-                ).order_by(self._edge_table.c[self._primary_key])
+                )
+                .order_by(self._edge_table.c[self._primary_key])
             ).fetchall()
 
         res = [x._asdict() for x in res]
 
         if include_metadata:
             return {
                 (
@@ -469,29 +479,44 @@
                     if r[self._edge_source_key] != str(u)
                     else r[self._edge_target_key]
                 )
                 for r in res
             ]
         )
 
-    def get_node_count(self) -> Iterable:
+    def get_node_count(self) -> int:
         """
         Get an integer count of the number of nodes in this graph.
 
         Arguments:
             None
 
         Returns:
             int: The count of nodes
 
         """
         return self._connection.execute(
             select(func.count()).select_from(self._node_table)
         ).scalar()
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return self._connection.execute(
+            select(func.count()).select_from(self._edge_table)
+        ).scalar()
+
     def out_degrees(self, nbunch=None):
         """
         Return the in-degree of each node in the graph.
 
         Arguments:
             nbunch (Iterable): The nodes to get the in-degree of
 
@@ -499,15 +524,17 @@
             dict: A dictionary of node: in-degree pairs
 
         """
 
         if nbunch is None:
             where_clause = None
         elif isinstance(nbunch, (list, tuple)):
-            where_clause = self._edge_table.c[self._edge_source_key].in_([str(x) for x in nbunch])
+            where_clause = self._edge_table.c[self._edge_source_key].in_(
+                [str(x) for x in nbunch]
+            )
         else:
             # single node:
             where_clause = self._edge_table.c[self._edge_source_key] == str(nbunch)
 
         if self._directed:
             query = (
                 select(self._edge_table.c[self._edge_source_key], func.count())
@@ -520,18 +547,15 @@
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_source_key])
             )
 
         if where_clause is not None:
             query = query.where(where_clause)
 
-        results = {
-            r[0]: r[1]
-            for r in self._connection.execute(query)
-        }
+        results = {r[0]: r[1] for r in self._connection.execute(query)}
 
         if nbunch and not isinstance(nbunch, (list, tuple)):
             return results.get(nbunch, 0)
         return results
 
     def in_degrees(self, nbunch=None):
         """
@@ -544,15 +568,17 @@
             dict: A dictionary of node: in-degree pairs
 
         """
 
         if nbunch is None:
             where_clause = None
         elif isinstance(nbunch, (list, tuple)):
-            where_clause = self._edge_table.c[self._edge_target_key].in_([str(x) for x in nbunch])
+            where_clause = self._edge_table.c[self._edge_target_key].in_(
+                [str(x) for x in nbunch]
+            )
         else:
             # single node:
             where_clause = self._edge_table.c[self._edge_target_key] == str(nbunch)
 
         if self._directed:
             query = (
                 select(self._edge_table.c[self._edge_target_key], func.count())
@@ -565,18 +591,15 @@
                 .select_from(self._edge_table)
                 .group_by(self._edge_table.c[self._edge_target_key])
             )
 
         if where_clause is not None:
             query = query.where(where_clause)
 
-        results = {
-            r[0]: r[1]
-            for r in self._connection.execute(query)
-        }
+        results = {r[0]: r[1] for r in self._connection.execute(query)}
 
         if nbunch and not isinstance(nbunch, (list, tuple)):
             return results.get(nbunch, 0)
         return results
 
     def ingest_from_edgelist_dataframe(
         self, edgelist: pd.DataFrame, source_column: str, target_column: str
@@ -644,7 +667,13 @@
 
         return {
             "node_count": len(nodes),
             "node_duration": time.time() - node_tic,
             "edge_count": len(edgelist),
             "edge_duration": edge_toc,
         }
+
+    def commit(self):
+        self._connection.commit()
+
+    def close(self):
+        self._connection.close()
```

### Comparing `grand-graph-0.5.0/grand/backends/backend.py` & `grand-graph-0.5.1/grand/backends/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,14 +114,30 @@
             bool: True if the node exists
         """
         try:
             return self.get_node_by_id(u) is not None
         except KeyError:
             return False
 
+    def has_edge(self, u: Hashable, v: Hashable) -> bool:
+        """
+        Return true if the edge exists in the graph.
+
+        Arguments:
+            u (Hashable): The source node ID
+            v (Hashable): The target node ID
+
+        Returns:
+            bool: True if the edge exists
+        """
+        try:
+            return self.get_edge_by_id(u, v) is not None
+        except KeyError:
+            return False
+
     def add_edge(self, u: Hashable, v: Hashable, metadata: dict):
         """
         Add a new edge to the graph between two nodes.
 
         If the graph is directed, this edge will start (source) at the `u` node
         and end (target) at the `v` node.
 
@@ -218,14 +234,27 @@
 
         Returns:
             int: The count of nodes
 
         """
         return len([i for i in self.all_nodes_as_iterable()])
 
+    def get_edge_count(self) -> int:
+        """
+        Get an integer count of the number of edges in this graph.
+
+        Arguments:
+            None
+
+        Returns:
+            int: The count of edges
+
+        """
+        return len([i for i in self.all_edges_as_iterable()])
+
     def degree(self, u: Hashable) -> int:
         """
         Get the degree of a node.
 
         Arguments:
             u (Hashable): The node ID
 
@@ -278,26 +307,23 @@
         if isinstance(nbunch, (list, tuple)):
             return {node: self.out_degree(node) for node in nbunch}
         else:
             return self.out_degree(nbunch)
 
 
 class CachedBackend(Backend):
-
     """
     A proxy Backend that serves as a cache for any other grand.Backend.
 
     """
 
-    def __init__(self, backend: Backend):
-        ...
+    def __init__(self, backend: Backend): ...
 
 
 class InMemoryCachedBackend(CachedBackend):
-
     """
     A proxy Backend that serves as a cache for any other grand.Backend.
 
     Wraps each call to the Backend with an LRU cache.
 
     """
```

### Comparing `grand-graph-0.5.0/grand/backends/metadatastore.py` & `grand-graph-0.5.1/grand/backends/metadatastore.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand/backends/test_backends.py` & `grand-graph-0.5.1/grand/backends/test_backends.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,94 +39,125 @@
 backend_test_params = [
     pytest.param(
         (NetworkXBackend, {}),
         marks=pytest.mark.skipif(
             os.environ.get("TEST_NETWORKXBACKEND", default="1") != "1",
             reason="NetworkX Backend skipped because $TEST_NETWORKXBACKEND != 1.",
         ),
+        id="NetworkXBackend",
     ),
 ]
 backend_test_params = [
     pytest.param(
         (DataFrameBackend, {}),
         marks=pytest.mark.skipif(
             os.environ.get("TEST_DATAFRAMEBACKEND", default="1") != "1",
             reason="DataFrameBackend skipped because $TEST_DATAFRAMEBACKEND != 1.",
         ),
+        id="DataFrameBackend",
     ),
 ]
 
 if _CAN_IMPORT_DYNAMODB:
     backend_test_params.append(
         pytest.param(
             (DynamoDBBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_DYNAMODB", default="1") != "1",
                 reason="DynamoDB Backend skipped because $TEST_DYNAMODB != 0 or boto3 is not installed",
             ),
+            id="DynamoDBBackend",
         ),
     )
 
 if _CAN_IMPORT_SQL:
     backend_test_params.append(
         pytest.param(
             (SQLBackend, {"db_url": "sqlite:///:memory:"}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_SQLBACKEND", default="1") != "1",
                 reason="SQL Backend skipped because $TEST_SQLBACKEND != 1 or sqlalchemy is not installed.",
             ),
+            id="SQLBackend",
         ),
     )
 if _CAN_IMPORT_IGRAPH:
     backend_test_params.append(
         pytest.param(
             (IGraphBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_IGRAPHBACKEND", default="1") != "1",
                 reason="IGraph Backend skipped because $TEST_IGRAPHBACKEND != 1 or igraph is not installed.",
             ),
+            id="IGraphBackend",
         ),
     )
 if _CAN_IMPORT_NETWORKIT:
     backend_test_params.append(
         pytest.param(
             (NetworkitBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_NETWORKIT", default="1") != "1",
                 reason="Networkit Backend skipped because $TEST_NETWORKIT != 1 or networkit is not installed.",
             ),
+            id="NetworkitBackend",
         ),
     )
 
 if os.environ.get("TEST_NETWORKITBACKEND") == "1":
     from ._networkit import NetworkitBackend
 
     backend_test_params.append(
         pytest.param(
             (NetworkitBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_NETWORKITBACKEND") != "1",
                 reason="Networkit Backend skipped because $TEST_NETWORKITBACKEND != 1.",
             ),
+            id="NetworkitBackend",
         ),
     )
 
 if os.environ.get("TEST_IGRAPHBACKEND") == "1":
     from ._igraph import IGraphBackend
 
     backend_test_params.append(
         pytest.param(
             (IGraphBackend, {}),
             marks=pytest.mark.skipif(
                 os.environ.get("TEST_IGRAPHBACKEND") != "1",
                 reason="Networkit Backend skipped because $TEST_IGRAPHBACKEND != 1.",
             ),
+            id="IGraphBackend",
         ),
     )
 
+# @pytest.mark.parametrize("backend", backend_test_params)
+class TestBackendPersistence:
+    def test_sqlite_persistence(self):
+        if not _CAN_IMPORT_SQL:
+            return
+
+        dbpath = "grand_peristence_test_temp.db"
+        url = "sqlite:///"+dbpath
+
+        #arrange
+        backend = SQLBackend(db_url=url, directed=True)
+        node0 = backend.add_node("A",{"foo":"bar"})
+        backend.commit()
+        backend.close()
+        #act
+        backend = SQLBackend(db_url=url, directed=True)
+        nodes = list(backend.all_nodes_as_iterable())
+        #assert
+        assert node0 in nodes
+        #cleanup
+        os.remove(dbpath)
+
+
 
 @pytest.mark.parametrize("backend", backend_test_params)
 class TestBackend:
     def test_can_create(self, backend):
         backend, kwargs = backend
         backend(**kwargs)
 
@@ -365,7 +396,36 @@
         assert G.nx.degree("baz") == 0
         assert G.nx.out_degree("foo") == 2
         assert G.nx.out_degree("bar") == 0
         assert G.nx.out_degree("baz") == 0
         assert G.nx.in_degree("foo") == 0
         assert G.nx.in_degree("bar") == 1
         assert G.nx.in_degree("baz") == 1
+
+    def test_node_count(self, backend):
+        backend, kwargs = backend
+        G = Graph(backend=backend(**kwargs))
+        G.nx.add_node("foo", bar=True)
+        G.nx.add_node("bar", foo=True)
+        assert len(G.nx) == 2
+
+
+@pytest.mark.benchmark
+@pytest.mark.parametrize("backend", backend_test_params)
+def test_node_addition_performance(backend):
+    backend, kwargs = backend
+    G = Graph(backend=backend(directed=True, **kwargs))
+    for i in range(1000):
+        G.nx.add_node(i)
+    assert len(G.nx) == 1000
+
+
+@pytest.mark.benchmark
+@pytest.mark.parametrize("backend", backend_test_params)
+def test_get_density_performance(backend):
+    backend, kwargs = backend
+    G = Graph(backend=backend(directed=True, **kwargs))
+    for i in range(1000):
+        G.nx.add_node(i)
+    for i in range(1000 - 1):
+        G.nx.add_edge(i, i + 1)
+    assert nx.density(G.nx) <= 0.005
```

### Comparing `grand-graph-0.5.0/grand/backends/test_cached_backend.py` & `grand-graph-0.5.1/grand/backends/test_cached_backend.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand/backends/test_metadatastore.py` & `grand-graph-0.5.1/grand/backends/test_metadatastore.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand/dialects/__init__.py` & `grand-graph-0.5.1/grand/dialects/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -176,14 +176,27 @@
 
     def out_degree(self, nbunch=None):
         return self.parent.backend.out_degrees(nbunch)
 
     def is_directed(self):
         return self.parent.backend.is_directed()
 
+    def __len__(self):
+        return self.parent.backend.get_node_count()
+
+    def number_of_nodes(self):
+        return self.parent.backend.get_node_count()
+
+    def number_of_edges(self, u=None, v=None):
+        if u is None and v is None:
+            return self.parent.backend.get_edge_count()
+        # Get the number of edges between u and v. because we don't support
+        # multigraphs, this is 1 if there is an edge, 0 otherwise.
+        return 1 if self.parent.backend.has_edge(u, v) else 0
+
 
 class IGraphDialect(nx.Graph):
     """
     An IGraphDialect provides a python-igraph-like interface
 
     """
 
@@ -214,15 +227,15 @@
     @property
     def es(self):
         return [
             i for i in self.parent.backend.all_edges_as_iterable(include_metadata=True)
         ]
 
     def add_edges(self, edgelist: List[Tuple[Hashable, Hashable]]):
-        for (u, v) in edgelist:
+        for u, v in edgelist:
             self.parent.backend.add_edge(u, v, {})
 
     def get_edgelist(self):
         return self.parent.backend.all_edges_as_iterable(include_metadata=False)
 
 
 class NetworkitDialect:
@@ -275,27 +288,27 @@
         return self.parent.backend.in_degree(v)
 
     def degreeOut(self, v):
         return self.parent.backend.out_degree(v)
 
     def density(self):
         # TODO: implement backend#degree?
-        E = len(self.parent.backend.all_edges_as_iterable())
+        E = self.parent.backend.get_edge_count()
         V = self.parent.backend.get_node_count()
 
         if self.parent.backend.is_directed():
             return E / (V * (V - 1))
         else:
             return 2 * E / (V * (V - 1))
 
     def numberOfNodes(self) -> int:
         return self.parent.backend.get_node_count()
 
     def numberOfEdges(self) -> int:
-        return len(self.parent.backend.all_edges_as_iterable())
+        return self.parent.backend.get_edge_count()
 
     def removeEdge(self, u, v) -> None:
         raise NotImplementedError
         return self.parent.backend.remove_edge(u, v)
 
     def removeNode(self, u: Hashable) -> None:
         if hasattr(self.parent.backend, "remove_node"):
```

### Comparing `grand-graph-0.5.0/grand/dialects/test_dialect.py` & `grand-graph-0.5.1/grand/dialects/test_dialect.py`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/grand_graph.egg-info/PKG-INFO` & `grand-graph-0.5.1/grand_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grand-graph
-Version: 0.5.0
+Version: 0.5.1
 Summary: Graph database wrapper for non-graph datastores
 Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky
 Author-email: opensource@matelsky.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: grand-graph Version: 0.5.0 Summary: Graph database
+Metadata-Version: 2.1 Name: grand-graph Version: 0.5.1 Summary: Graph database
 wrapper for non-graph datastores Home-page: https://github.com/aplbrain/grand
 Author: Jordan Matelsky Author-email: opensource@matelsky.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Description-Content-
 Type: text/markdown Provides-Extra: sql Provides-Extra: dynamodb Provides-
 Extra: igraph Provides-Extra: networkit License-File: LICENSE
                                [docs/grand.png]
```

### Comparing `grand-graph-0.5.0/grand_graph.egg-info/SOURCES.txt` & `grand-graph-0.5.1/grand_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grand-graph-0.5.0/setup.py` & `grand-graph-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="grand-graph",
-    version="0.5.0",
+    version="0.5.1",
     author="Jordan Matelsky",
     author_email="opensource@matelsky.com",
     description="Graph database wrapper for non-graph datastores",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aplbrain/grand",
     packages=setuptools.find_packages(),
```

