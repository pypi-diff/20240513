# Comparing `tmp/nchuchain-1.0.7.tar.gz` & `tmp/nchuchain-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nchuchain-1.0.7.tar", last modified: Mon May 13 13:53:28 2024, max compression
+gzip compressed data, was "nchuchain-1.0.8.tar", last modified: Mon May 13 14:25:11 2024, max compression
```

## Comparing `nchuchain-1.0.7.tar` & `nchuchain-1.0.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.443004 nchuchain-1.0.7/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.7/LICENSE
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      885 2024-05-13 13:53:28.439004 nchuchain-1.0.7/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       12 2024-05-13 11:51:17.000000 nchuchain-1.0.7/README.md
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 12:53:46.000000 nchuchain-1.0.7/nchuchain/__init__.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/chains/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      392 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/chains/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     5424 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/chains/retrieval_qa.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/data_modules/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      411 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/data_modules/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3481 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/data_modules/context_prefix_tree.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/llms/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      405 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/llms/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3410 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/llms/chat_completions_llm.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/loaders/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      391 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/loaders/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3159 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/loaders/text_loader.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/models/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      442 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/models/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      120 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/models/base.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)    11473 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/models/generative_model.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/retrievers/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      516 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/retrievers/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1724 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/retrievers/base.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     8571 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/retrievers/pyserini_bm25.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     6860 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/retrievers/rank_bm25.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/splitters/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      397 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/splitters/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3319 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/splitters/text_splitter.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain/utils/
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      610 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/utils/__init__.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3704 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/utils/config.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      785 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/utils/data.py
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     7239 2024-05-13 11:47:31.000000 nchuchain-1.0.7/nchuchain/utils/template.py
-drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 13:53:28.439004 nchuchain-1.0.7/nchuchain.egg-info/
--rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      885 2024-05-13 13:53:28.000000 nchuchain-1.0.7/nchuchain.egg-info/PKG-INFO
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      884 2024-05-13 13:53:28.000000 nchuchain-1.0.7/nchuchain.egg-info/SOURCES.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 13:53:28.000000 nchuchain-1.0.7/nchuchain.egg-info/dependency_links.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      155 2024-05-13 13:53:28.000000 nchuchain-1.0.7/nchuchain.egg-info/requires.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       10 2024-05-13 13:53:28.000000 nchuchain-1.0.7/nchuchain.egg-info/top_level.txt
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-13 13:53:28.443004 nchuchain-1.0.7/setup.cfg
--rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1361 2024-05-13 13:52:56.000000 nchuchain-1.0.7/setup.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1068 2024-05-07 09:39:28.000000 nchuchain-1.0.8/LICENSE
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      986 2024-05-13 14:25:11.332966 nchuchain-1.0.8/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      112 2024-05-13 14:00:42.000000 nchuchain-1.0.8/README.md
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 12:53:46.000000 nchuchain-1.0.8/nchuchain/__init__.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/chains/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      392 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/chains/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     5424 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/chains/retrieval_qa.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/data_modules/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      411 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/data_modules/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3481 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/data_modules/context_prefix_tree.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/llms/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      405 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/llms/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3410 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/llms/chat_completions_llm.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/loaders/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      391 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/loaders/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3159 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/loaders/text_loader.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/models/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      442 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/models/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      120 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/models/base.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)    11473 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/models/generative_model.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/retrievers/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      516 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/retrievers/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1724 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/retrievers/base.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     8571 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/retrievers/pyserini_bm25.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     6860 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/retrievers/rank_bm25.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/splitters/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      397 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/splitters/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3319 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/splitters/text_splitter.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain/utils/
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      610 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/utils/__init__.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     3704 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/utils/config.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      830 2024-05-13 14:23:24.000000 nchuchain-1.0.8/nchuchain/utils/data.py
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     7239 2024-05-13 11:47:31.000000 nchuchain-1.0.8/nchuchain/utils/template.py
+drwxrwxr-x   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        0 2024-05-13 14:25:11.332966 nchuchain-1.0.8/nchuchain.egg-info/
+-rw-r--r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      986 2024-05-13 14:25:11.000000 nchuchain-1.0.8/nchuchain.egg-info/PKG-INFO
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      884 2024-05-13 14:25:11.000000 nchuchain-1.0.8/nchuchain.egg-info/SOURCES.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)        1 2024-05-13 14:25:11.000000 nchuchain-1.0.8/nchuchain.egg-info/dependency_links.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)      155 2024-05-13 14:25:11.000000 nchuchain-1.0.8/nchuchain.egg-info/requires.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       10 2024-05-13 14:25:11.000000 nchuchain-1.0.8/nchuchain.egg-info/top_level.txt
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)       38 2024-05-13 14:25:11.332966 nchuchain-1.0.8/setup.cfg
+-rw-rw-r--   0 111_ms_wenchuan  (1000) 111_ms_wenchuan  (1000)     1361 2024-05-13 14:24:53.000000 nchuchain-1.0.8/setup.py
```

### Comparing `nchuchain-1.0.7/LICENSE` & `nchuchain-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/chains/retrieval_qa.py` & `nchuchain-1.0.8/nchuchain/chains/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/data_modules/context_prefix_tree.py` & `nchuchain-1.0.8/nchuchain/data_modules/context_prefix_tree.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/llms/chat_completions_llm.py` & `nchuchain-1.0.8/nchuchain/llms/chat_completions_llm.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/loaders/text_loader.py` & `nchuchain-1.0.8/nchuchain/loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/models/generative_model.py` & `nchuchain-1.0.8/nchuchain/models/generative_model.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/retrievers/__init__.py` & `nchuchain-1.0.8/nchuchain/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/retrievers/base.py` & `nchuchain-1.0.8/nchuchain/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/retrievers/pyserini_bm25.py` & `nchuchain-1.0.8/nchuchain/retrievers/pyserini_bm25.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/retrievers/rank_bm25.py` & `nchuchain-1.0.8/nchuchain/retrievers/rank_bm25.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/splitters/text_splitter.py` & `nchuchain-1.0.8/nchuchain/splitters/text_splitter.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/utils/__init__.py` & `nchuchain-1.0.8/nchuchain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/utils/config.py` & `nchuchain-1.0.8/nchuchain/utils/config.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain/utils/data.py` & `nchuchain-1.0.8/nchuchain/utils/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict
 
 
 class Document(object):
-    def __init__(self, page_content: str, metadata: Dict[str, Any]):
+    def __init__(self, page_content: str, metadata: Optional[Dict[str, Any]] = None):
         self.page_content = page_content
-        self.metadata = metadata
+        self.metadata = metadata if metadata != None else {}
     
     def __repr__(self):
         return f"Document(page_content={repr(self.page_content)}, metadata={repr(self.metadata)})"
 
 
 class QAResult(object):
     def __init__(self, summary: str, answers: Dict[str, Document]):
```

### Comparing `nchuchain-1.0.7/nchuchain/utils/template.py` & `nchuchain-1.0.8/nchuchain/utils/template.py`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/nchuchain.egg-info/SOURCES.txt` & `nchuchain-1.0.8/nchuchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nchuchain-1.0.7/setup.py` & `nchuchain-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 PACKAGE_NAME = "nchuchain"
 AUTHOR = "WenChuan Hsu"
 AUTHOR_EMAIL = "wenchuan19991111@gmail.com"
 URL = "https://github.com/good22014040/nchuchain"
 DOWNLOAD_URL = "https://pypi.org/project/nchuchain/"
  
 LICENSE = "MIT"
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 DESCRIPTION = "A set of data tools in Python"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding="utf8")
 LONG_DESC_TYPE = "text/markdown"
  
 requirements = (HERE / "requirements.txt").read_text(encoding="utf8")
 INSTALL_REQUIRES = [s.strip() for s in requirements.split("\n")]
```

