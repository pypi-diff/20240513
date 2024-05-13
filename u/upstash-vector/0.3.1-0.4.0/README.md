# Comparing `tmp/upstash_vector-0.3.1.tar.gz` & `tmp/upstash_vector-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upstash_vector-0.3.1.tar", max compression
+gzip compressed data, was "upstash_vector-0.4.0.tar", max compression
```

## Comparing `upstash_vector-0.3.1.tar` & `upstash_vector-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1070 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/LICENSE
--rw-r--r--   0        0        0     5215 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/README.md
--rw-r--r--   0        0        0     1669 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/__init__.py
--rw-r--r--   0        0        0     3403 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/client.py
--rw-r--r--   0        0        0    16201 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/core/index_operations.py
--rw-r--r--   0        0        0       81 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/errors.py
--rw-r--r--   0        0        0     2187 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/http.py
--rw-r--r--   0        0        0        0 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/py.typed
--rw-r--r--   0        0        0     2074 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/types.py
--rw-r--r--   0        0        0     3145 2024-04-15 16:57:57.653452 upstash_vector-0.3.1/upstash_vector/utils.py
--rw-r--r--   0        0        0     6486 1970-01-01 00:00:00.000000 upstash_vector-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/LICENSE
+-rw-r--r--   0        0        0     9561 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/README.md
+-rw-r--r--   0        0        0     1669 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/__init__.py
+-rw-r--r--   0        0        0     3403 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/client.py
+-rw-r--r--   0        0        0    24263 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/core/index_operations.py
+-rw-r--r--   0        0        0       81 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/errors.py
+-rw-r--r--   0        0        0     2187 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/http.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/py.typed
+-rw-r--r--   0        0        0     2564 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/types.py
+-rw-r--r--   0        0        0     3145 2024-05-13 16:45:05.779091 upstash_vector-0.4.0/upstash_vector/utils.py
+-rw-r--r--   0        0        0    10832 1970-01-01 00:00:00.000000 upstash_vector-0.4.0/PKG-INFO
```

### Comparing `upstash_vector-0.3.1/LICENSE` & `upstash_vector-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.3.1/pyproject.toml` & `upstash_vector-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "upstash-vector"
-version = "0.3.1"
+version = "0.4.0"
 description = "Serverless Vector SDK from Upstash"
 license = "MIT"
 authors = ["Upstash <support@upstash.com>"]
 maintainers = ["Upstash <support@upstash.com>"]
 readme = "README.md"
 repository = "https://github.com/upstash/vector-py"
 keywords = ["Upstash Vector", "Serverless Vector"]
```

### Comparing `upstash_vector-0.3.1/upstash_vector/client.py` & `upstash_vector-0.4.0/upstash_vector/client.py`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.3.1/upstash_vector/http.py` & `upstash_vector-0.4.0/upstash_vector/http.py`

 * *Files identical despite different names*

### Comparing `upstash_vector-0.3.1/upstash_vector/types.py` & `upstash_vector-0.4.0/upstash_vector/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,23 +72,41 @@
         return cls(
             next_cursor=obj["nextCursor"],
             vectors=[FetchResult._from_json(v) for v in obj["vectors"]],
         )
 
 
 @dataclass
+class NamespaceInfo:
+    vector_count: int
+    pending_vector_count: int
+
+    @classmethod
+    def _from_json(cls, obj: dict) -> "NamespaceInfo":
+        return cls(
+            vector_count=obj["vectorCount"],
+            pending_vector_count=obj["pendingVectorCount"],
+        )
+
+
+@dataclass
 class InfoResult:
     vector_count: int
     pending_vector_count: int
     index_size: int
     dimension: int
     similarity_function: str
+    namespaces: Dict[str, NamespaceInfo]
 
     @classmethod
     def _from_json(cls, obj: dict) -> "InfoResult":
         return cls(
             vector_count=obj["vectorCount"],
             pending_vector_count=obj["pendingVectorCount"],
             index_size=obj["indexSize"],
             dimension=obj["dimension"],
             similarity_function=obj["similarityFunction"],
+            namespaces={
+                ns: NamespaceInfo._from_json(ns_info)
+                for ns, ns_info in obj["namespaces"].items()
+            },
         )
```

### Comparing `upstash_vector-0.3.1/upstash_vector/utils.py` & `upstash_vector-0.4.0/upstash_vector/utils.py`

 * *Files identical despite different names*

