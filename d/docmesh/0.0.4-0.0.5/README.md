# Comparing `tmp/docmesh-0.0.4.tar.gz` & `tmp/docmesh-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh-0.0.4.tar` & `docmesh-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-10 11:02:39.301355 docmesh-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-05-10 11:57:43.381182 docmesh-0.0.4/docmesh/__init__.py
--rw-r--r--   0        0        0      882 2024-05-10 11:02:39.301355 docmesh-0.0.4/docmesh/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-10 11:07:24.642695 docmesh-0.0.4/docmesh/db/auth.py
--rw-r--r--   0        0        0     7540 2024-05-10 11:54:09.340126 docmesh-0.0.4/docmesh/db/neo.py
--rw-r--r--   0        0        0      276 2024-05-10 11:02:39.301355 docmesh-0.0.4/docmesh/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-10 11:02:39.301355 docmesh-0.0.4/docmesh/utils/graph_utils.py
--rw-r--r--   0        0        0     3148 2024-05-10 11:02:39.301355 docmesh-0.0.4/docmesh/utils/semantic_scholar.py
--rw-r--r--   0        0        0      745 2024-05-10 11:56:50.344920 docmesh-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 docmesh-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-10 11:02:39.301355 docmesh-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-13 03:47:28.446209 docmesh-0.0.5/docmesh/__init__.py
+-rw-r--r--   0        0        0     1092 2024-05-12 15:13:18.166469 docmesh-0.0.5/docmesh/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-10 11:07:24.642695 docmesh-0.0.5/docmesh/db/auth.py
+-rw-r--r--   0        0        0    10070 2024-05-13 02:09:44.402228 docmesh-0.0.5/docmesh/db/neo.py
+-rw-r--r--   0        0        0      379 2024-05-11 04:30:05.745437 docmesh-0.0.5/docmesh/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-10 11:02:39.301355 docmesh-0.0.5/docmesh/utils/graph_utils.py
+-rw-r--r--   0        0        0     3496 2024-05-11 04:34:00.106569 docmesh-0.0.5/docmesh/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      745 2024-05-12 04:34:50.295290 docmesh-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 docmesh-0.0.5/PKG-INFO
```

### Comparing `docmesh-0.0.4/docmesh/db/__init__.py` & `docmesh-0.0.5/docmesh/db/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,17 +4,20 @@
     get_entity,
     add_entity,
     follow_entity,
     list_follows,
     list_popular_entities,
     get_paper_from_id,
     get_paper_from_title,
-    add_paper,
+    add_paper_from_title,
+    add_paper_from_arxiv,
     read_paper,
     list_latest_papers,
+    list_unread_similar_papers,
+    list_unread_semantic_papers,
     list_unread_follows_papers,
     list_unread_influential_papers,
     get_latest_citegraph,
 )
 from .auth import (
     add_auth_for_entity,
     get_auth_from_entity,
@@ -27,17 +30,20 @@
     "get_entity",
     "add_entity",
     "follow_entity",
     "list_follows",
     "list_popular_entities",
     "get_paper_from_id",
     "get_paper_from_title",
-    "add_paper",
+    "add_paper_from_title",
+    "add_paper_from_arxiv",
     "read_paper",
     "list_latest_papers",
+    "list_unread_similar_papers",
+    "list_unread_semantic_papers",
     "list_unread_follows_papers",
     "list_unread_influential_papers",
     "get_latest_citegraph",
     "add_auth_for_entity",
     "get_auth_from_entity",
     "get_entity_from_auth",
 ]
```

### Comparing `docmesh-0.0.4/docmesh/db/auth.py` & `docmesh-0.0.5/docmesh/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.4/docmesh/db/neo.py` & `docmesh-0.0.5/docmesh/db/neo.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,25 @@
 
 from neomodel import db
 from neomodel import (
     StructuredNode,
     StructuredRel,
     StringProperty,
     IntegerProperty,
+    FloatProperty,
     DateTimeProperty,
+    ArrayProperty,
     RelationshipTo,
     RelationshipFrom,
 )
 from neomodel.integration.pandas import to_dataframe
 
 from ..utils.semantic_scholar import (
-    get_paper_id,
+    get_paper_id_from_title,
+    get_paper_id_from_arxiv,
     get_references,
     get_paper_details,
     PaperIdNotFound,
 )
 
 
 class FollowRel(StructuredRel):
@@ -50,14 +53,16 @@
     title = StringProperty()
     abstract = StringProperty()
     summary = StringProperty()
     publication_date = DateTimeProperty()
     reference_count = IntegerProperty()
     citation_count = IntegerProperty()
     pdf = StringProperty()
+    # openai text-embedding-3-large cast to 1024
+    embedding_te3l = ArrayProperty(FloatProperty())
 
     readers = RelationshipFrom("Entity", "read", model=ReadRel)
     references = RelationshipTo("Paper", "cite")
     citations = RelationshipFrom("Paper", "cite")
 
     @property
     def serialize(self) -> dict[str, Any]:
@@ -81,16 +86,16 @@
 
 def get_entity(entity_name: str) -> Entity:
     entity = Entity.nodes.get(name=entity_name)
     return entity
 
 
 @db.transaction
-def add_entity(name: str) -> Entity:
-    entity: Entity = Entity.create_or_update({"name": name})
+def add_entity(entity_name: str) -> Entity:
+    entity: Entity = Entity.create_or_update({"name": entity_name})
     return entity
 
 
 @db.transaction
 def follow_entity(follower_name: str, follow_name: str) -> None:
     follower_entity = get_entity(follower_name)
     followed_entity = get_entity(follow_name)
@@ -121,15 +126,17 @@
         } AS num_reads
         ORDER BY num_followers DESC, num_reads DESC
         LIMIT $n
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"n": n},
+            params={
+                "n": n,
+            },
         )
     )
 
     return df
 
 
 def get_paper_from_id(paper_id: str) -> Paper:
@@ -139,42 +146,57 @@
 
 def get_paper_from_title(title: str) -> Paper:
     paper = Paper.nodes.get(title=title)
     return paper
 
 
 @db.transaction
-def _add_paper(paper: DataFrame, references: DataFrame) -> Paper:
+def _add_paper_references(paper: DataFrame, references: DataFrame) -> Paper:
     paper: Paper = Paper.create_or_update(*paper.to_dict(orient="records"))[0]
 
     if references.shape[0] != 0:
         references: list[Paper] = Paper.create_or_update(*references.to_dict(orient="records"))
 
         for reference in references:
             # XXX: neomodel says that they can ensure relationship uniqueness
             # however, it doesn't
             if not paper.references.is_connected(reference):
                 paper.references.connect(reference)
 
     return paper
 
 
-def add_paper(title: str) -> Paper:
-    paper_id = get_paper_id(title)
+def _add_paper(paper_id: str) -> Paper:
     if paper_id is None:
         raise PaperIdNotFound(f"Cannot find semantic scholar paper id for {title}.")
     paper = get_paper_details([paper_id])
 
     references_ids = get_references(paper_id)
     if len(references_ids) == 0:
         references = pd.DataFrame()
     else:
         references = get_paper_details(references_ids)
 
-    paper = _add_paper(paper, references)
+    paper = _add_paper_references(paper, references)
+    return paper
+
+
+def add_paper_from_title(title: str) -> Paper:
+    if (paper_id := get_paper_id_from_title(title)) is None:
+        raise PaperIdNotFound(f"Cannot find semantic scholar paper id from title {title}.")
+
+    paper = _add_paper(paper_id)
+    return paper
+
+
+def add_paper_from_arxiv(arxiv_id: str) -> Paper:
+    if (paper_id := get_paper_id_from_arxiv(arxiv_id)) is None:
+        raise PaperIdNotFound(f"Cannot find semantic scholar paper id from arxiv {arxiv_id}.")
+
+    paper = _add_paper(paper_id)
     return paper
 
 
 @db.transaction
 def read_paper(entity_name: str, paper_id: str) -> None:
     entity = get_entity(entity_name)
     paper = get_paper_from_id(paper_id=paper_id)
@@ -185,88 +207,154 @@
 
 
 @db.transaction
 def list_latest_papers(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e:Entity) -[r:read]-> (p:Paper)
-        WHERE e.name = $name
+        WHERE e.name = $entity_name
         RETURN p.paper_id AS paper_id, p.title AS title
         ORDER BY r.read_time DESC
         LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"name": entity_name, "n": n},
+            params={
+                "entity_name": entity_name,
+                "n": n,
+            },
+        )
+    )
+
+    return df
+
+
+@db.transaction
+def list_unread_similar_papers(entity_name: str, paper_id: str, n: int) -> DataFrame:
+    # XXX: use cypher query language, since OGM is not well supported
+    query = """
+        MATCH (p0:Paper)
+        WHERE p0.paper_id = $paper_id
+        CALL db.index.vector.queryNodes('vector_embedding_te3l', $n, p0.embedding_te3l)
+        YIELD node AS p, score
+        WHERE NOT EXISTS {
+            (p) <-[:read]- (e:Entity)
+            WHERE e.name = $entity_name 
+        }
+        RETURN p.title AS title, p.pdf AS pdf, score
+    """
+    df = to_dataframe(
+        db.cypher_query(
+            query,
+            params={
+                "entity_name": entity_name,
+                "paper_id": paper_id,
+                "n": n,
+            },
+        )
+    )
+
+    return df
+
+
+@db.transaction
+def list_unread_semantic_papers(entity_name: str, semantic_embedding: list[float], n: int) -> DataFrame:
+    # XXX: use cypher query language, since OGM is not well supported
+    query = """
+        CALL db.index.vector.queryNodes('vector_embedding_te3l', $n, $semantic_embedding)
+        YIELD node AS p, score
+        WHERE NOT EXISTS {
+            (p) <-[:read]- (e:Entity)
+            WHERE e.name = $entity_name 
+        }
+        RETURN p.title AS title, p.pdf AS pdf, score
+    """
+    df = to_dataframe(
+        db.cypher_query(
+            query,
+            params={
+                "entity_name": entity_name,
+                "semantic_embedding": semantic_embedding,
+                "n": n,
+            },
         )
     )
 
     return df
 
 
 @db.transaction
 def list_unread_follows_papers(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e1:Entity) -[:follow]-> (:Entity) -[r:read]-> (p:Paper)
         WHERE e1.name = $name
         AND NOT EXISTS {
             (p) <-[:read]- (e2:Entity)
-            WHERE e2.name = $name
+            WHERE e2.name = $entity_name
         }
         RETURN p.title AS title, p.pdf AS pdf
         ORDER BY r.read_time, p.citation_count DESC
         LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"name": entity_name, "n": n},
+            params={
+                "entity_name": entity_name,
+                "n": n,
+            },
         )
     )
 
     return df
 
 
 @db.transaction
 def list_unread_influential_papers(entity_name: str, date_time: str) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (p:Paper)
         WHERE p.publication_date >= DATETIME($date_time).epochSeconds
         AND NOT EXISTS {
             (p) <-[:read]- (e:Entity)
-            WHERE e.name = $name
+            WHERE e.name = $entity_name
         }
         RETURN p.title AS title, p.pdf AS pdf
         ORDER BY p.citation_count DESC
         limit 10;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"date_time": date_time, "name": entity_name},
+            params={
+                "entity_name": entity_name,
+                "date_time": date_time,
+            },
         )
     )
 
     return df
 
 
 @db.transaction
 def get_latest_citegraph(entity_name: str, n: int) -> DataFrame:
     # XXX: use cypher query language, since OGM is not well supported
     query = """
         MATCH (e1:Entity) -[r:read]-> (p1:Paper) -[:cite]-> (p2:Paper) <-[:read]- (e2:Entity)
-        WHERE e1.name = $name AND e2.name = $name
+        WHERE e1.name = $name AND e2.name = $entity_name
         RETURN p1.paper_id AS p1_paper_id, p2.paper_id AS p2_paper_id
         ORDER BY r.read_time DESC
         LIMIT $n;
     """
     df = to_dataframe(
         db.cypher_query(
             query,
-            params={"name": entity_name, "n": n},
+            params={
+                "entity_name": entity_name,
+                "n": n,
+            },
         )
     )
 
     return df
```

### Comparing `docmesh-0.0.4/docmesh/utils/semantic_scholar.py` & `docmesh-0.0.5/docmesh/utils/semantic_scholar.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 
 from typing import Optional, Any
 from pandas.core.frame import DataFrame
 
 from retry import retry
 
 
-class PaperIdNotFound(Exception):
-    ...
+class PaperIdNotFound(Exception): ...
 
 
 def _sleep1() -> None:
     # semantic scholar api is restricted under 1 qps
     # so we sleep 1 second anyway to avoid rate limit
     time.sleep(1)
 
@@ -50,15 +49,15 @@
     )
     rsp.raise_for_status()
 
     return rsp.json()
 
 
 @retry(tries=3)
-def get_paper_id(title: str) -> Optional[str]:
+def get_paper_id_from_title(title: str) -> Optional[str]:
     _sleep1()
 
     headers = _get_headers()
     url = f"https://api.semanticscholar.org/graph/v1/paper/search?query=title:{title}&limit=1"
 
     rsp = requests.get(url, headers=headers)
     rsp.raise_for_status()
@@ -72,14 +71,28 @@
         return data[0]["paperId"]
     else:
         # retrieved title does not match with the query
         return None
 
 
 @retry(tries=3)
+def get_paper_id_from_arxiv(arxiv_id: str) -> Optional[str]:
+    _sleep1()
+
+    headers = _get_headers()
+    url = f"https://api.semanticscholar.org/graph/v1/paper/ARXIV:{arxiv_id}"
+
+    rsp = requests.get(url, headers=headers)
+    rsp.raise_for_status()
+
+    paper_id = rsp.json().get("paperId", None)
+    return paper_id
+
+
+@retry(tries=3)
 def get_references(paper_id: str) -> list[str]:
     fields = ["references"]
     details = _get_details([paper_id], fields)
 
     references = details[0]["references"]
     paper_ids = [ref["paperId"] for ref in references if ref["paperId"] is not None]
```

### Comparing `docmesh-0.0.4/pyproject.toml` & `docmesh-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh-0.0.4/PKG-INFO` & `docmesh-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh
-Version: 0.0.4
+Version: 0.0.5
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

