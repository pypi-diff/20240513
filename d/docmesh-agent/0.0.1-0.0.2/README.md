# Comparing `tmp/docmesh_agent-0.0.1.tar.gz` & `tmp/docmesh_agent-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.1.tar` & `docmesh_agent-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.1/README.md
--rw-r--r--   0        0        0       22 2024-05-10 11:04:48.925963 docmesh_agent-0.0.1/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     3928 2024-05-10 11:14:01.104559 docmesh_agent-0.0.1/docmesh_agent/main.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.1/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.1/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      857 2024-05-10 11:02:39.301355 docmesh_agent-0.0.1/docmesh_agent/prompt.py
--rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.1/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.1/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0      677 2024-05-10 11:16:55.645388 docmesh_agent-0.0.1/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      455 2024-05-10 11:16:58.785403 docmesh_agent-0.0.1/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      569 2024-05-10 11:02:39.301355 docmesh_agent-0.0.1/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.1/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0     2299 2024-05-10 11:18:58.249989 docmesh_agent-0.0.1/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3926 2024-05-10 11:19:24.922119 docmesh_agent-0.0.1/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     4266 2024-05-10 11:19:22.830109 docmesh_agent-0.0.1/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     2392 2024-05-10 11:19:18.438088 docmesh_agent-0.0.1/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      718 2024-05-10 11:56:36.828854 docmesh_agent-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 docmesh_agent-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-13 03:47:40.246354 docmesh_agent-0.0.2/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     4050 2024-05-13 02:12:42.888413 docmesh_agent-0.0.2/docmesh_agent/main.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.2/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      857 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/prompt.py
+-rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.2/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0      787 2024-05-11 04:38:52.647986 docmesh_agent-0.0.2/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.2/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      741 2024-05-13 03:31:34.698480 docmesh_agent-0.0.2/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.2/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0     2299 2024-05-10 11:18:58.249989 docmesh_agent-0.0.2/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3926 2024-05-10 11:19:24.922119 docmesh_agent-0.0.2/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     5226 2024-05-11 05:02:21.234649 docmesh_agent-0.0.2/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4598 2024-05-13 03:40:24.188988 docmesh_agent-0.0.2/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      718 2024-05-13 03:47:45.210415 docmesh_agent-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      637 1970-01-01 00:00:00.000000 docmesh_agent-0.0.2/PKG-INFO
```

### Comparing `docmesh_agent-0.0.1/docmesh_agent/main.py` & `docmesh_agent-0.0.2/docmesh_agent/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,15 +63,19 @@
     return {"data": data}
 
 
 def _execute_agent(entity_name: str, query: str, session_id: str) -> str:
     # setup react prompt
     prompt = MEMORY_REACT_PROMPT
     # setup llm
-    llm = ChatOpenAI(model=os.getenv("OPENAI_MODEL"))
+    llm = ChatOpenAI(
+        base_url=os.getenv("OPENAI_CHAT_API_BASE"),
+        api_key=os.getenv("OPENAI_CHAT_API_KEY"),
+        model=os.getenv("OPENAI_CHAT_MODEL"),
+    )
     # set up all tools
     tools = [
         *EntityToolkit(entity_name=entity_name).get_tools(),
         *PaperToolkit(entity_name=entity_name).get_tools(),
         *RecommendToolkit(entity_name=entity_name).get_tools(),
     ]
     # setup ReAct agent
```

### Comparing `docmesh_agent-0.0.1/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.2/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/prompt.py` & `docmesh_agent-0.0.2/docmesh_agent/prompt.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.2/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.2/docmesh_agent/toolkit/paper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from langchain_core.tools import BaseToolkit
 
 from docmesh_agent.tools.base import BaseAgentTool
 from docmesh_agent.tools.paper import (
-    AddPaperTool,
+    AddPaperFromTitleTool,
+    AddPaperFromArxivTool,
     GetPaperIdTool,
     MarkPaperReadTool,
     PaperSummaryTool,
     ListLatestPaperTool,
 )
 
 
 class PaperToolkit(BaseToolkit):
     entity_name: str
 
     def get_tools(self) -> list[BaseAgentTool]:
         return [
-            AddPaperTool(entity_name=self.entity_name),
+            AddPaperFromTitleTool(entity_name=self.entity_name),
+            AddPaperFromArxivTool(entity_name=self.entity_name),
             GetPaperIdTool(entity_name=self.entity_name),
             MarkPaperReadTool(entity_name=self.entity_name),
             PaperSummaryTool(entity_name=self.entity_name),
             ListLatestPaperTool(entity_name=self.entity_name),
         ]
```

### Comparing `docmesh_agent-0.0.1/docmesh_agent/tools/__init__.py` & `docmesh_agent-0.0.2/docmesh_agent/tools/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 from .entity import (
     FollowEntityTool,
     ListFollowsTool,
     ListPopularEntitiesTool,
 )
 from .paper import (
-    AddPaperTool,
+    AddPaperFromTitleTool,
+    AddPaperFromArxivTool,
     GetPaperIdTool,
     MarkPaperReadTool,
     PaperSummaryTool,
     ListLatestPaperTool,
 )
 from .recommend import (
     UnreadFollowsTool,
     UnreadInfluentialTool,
+    UnreadSimilarTool,
+    UnreadSemanticTool,
 )
 
 __all__ = [
     "FollowEntityTool",
     "ListFollowsTool",
     "ListPopularEntitiesTool",
-    "AddPaperTool",
+    "AddPaperFromTitleTool",
+    "AddPaperFromArxivTool",
     "GetPaperIdTool",
     "MarkPaperReadTool",
     "PaperSummaryTool",
     "ListLatestPaperTool",
     "UnreadFollowsTool",
     "UnreadInfluentialTool",
+    "UnreadSimilarTool",
+    "UnreadSemanticTool",
 ]
```

### Comparing `docmesh_agent-0.0.1/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.2/docmesh_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.2/docmesh_agent/tools/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.2/docmesh_agent/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.1/docmesh_agent/tools/paper.py` & `docmesh_agent-0.0.2/docmesh_agent/tools/paper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,74 @@
 from typing import Type, Optional
 from langchain.pydantic_v1 import BaseModel, Field
 
 from langchain.callbacks.manager import CallbackManagerForToolRun
 
 from docmesh.db.neo import (
-    add_paper,
+    add_paper_from_title,
+    add_paper_from_arxiv,
     read_paper,
     get_paper_from_id,
     get_paper_from_title,
     list_latest_papers,
 )
 from docmesh.utils.semantic_scholar import PaperIdNotFound
 from docmesh_agent.tools.base import BaseAgentTool
 
 
-class AddPaperToolInput(BaseModel):
+class AddPaperFromTitleToolInput(BaseModel):
     title: str = Field(description="paper title")
 
 
-class AddPaperTool(BaseAgentTool):
-    name: str = "add_paper"
-    description: str = "useful when you need to add a paper to database"
-    args_schema: Optional[Type[BaseModel]] = AddPaperToolInput
+class AddPaperFromTitleTool(BaseAgentTool):
+    name: str = "add_paper_from_title"
+    description: str = "useful when you need to add a paper use title"
+    args_schema: Optional[Type[BaseModel]] = AddPaperFromTitleToolInput
     handle_tool_error: bool = True
 
     def _run(
         self,
         title: str,
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> str:
         title = self._preporcess_input(title)
         try:
-            paper = add_paper(title)
+            paper = add_paper_from_title(title)
         except PaperIdNotFound:
-            self._raise_tool_error(f"Cannot find paper id for paper {title}, you may end execution.")
+            self._raise_tool_error(f"Cannot find paper id for title {title}, you may end execution.")
 
         msg = f"Successfully add paper {title} with id {paper.paper_id} into neo4j database."
         return f"\n{msg}\n"
 
 
+class AddPaperFromArxivToolInput(BaseModel):
+    arxiv_id: str = Field(description="arxiv id")
+
+
+class AddPaperFromArxivTool(BaseAgentTool):
+    name: str = "add_paper_from_arxiv_id"
+    description: str = "useful when you need to add a paper use arxiv id"
+    args_schema: Optional[Type[BaseModel]] = AddPaperFromArxivToolInput
+    handle_tool_error: bool = True
+
+    def _run(
+        self,
+        arxiv_id: str,
+        run_manager: Optional[CallbackManagerForToolRun] = None,
+    ) -> str:
+        arxiv_id = self._preporcess_input(arxiv_id)
+        try:
+            paper = add_paper_from_arxiv(arxiv_id)
+        except PaperIdNotFound:
+            self._raise_tool_error(f"Cannot find paper id for arxiv {arxiv_id}, you may end execution.")
+
+        msg = f"Successfully add arxiv {arxiv_id} with id {paper.paper_id} into neo4j database."
+        return f"\n{msg}\n"
+
+
 class GetPaperIdToolInput(BaseModel):
     title: str = Field(description="paper title")
 
 
 class GetPaperIdTool(BaseAgentTool):
     name: str = "get_paper_id"
     description: str = "useful when you need to find a paper id"
```

### Comparing `docmesh_agent-0.0.1/pyproject.toml` & `docmesh_agent-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh>=0.0.4",
+    "docmesh>=0.0.5",
     "langchain>=0.1.15",
     "langchain-openai>=0.1.3",
     "fastapi==0.111.0",
     "uvicorn==0.29.0",
     "gunicorn==19.3.0",
 ]
```

### Comparing `docmesh_agent-0.0.1/PKG-INFO` & `docmesh_agent-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.1
+Version: 0.0.2
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh>=0.0.4
+Requires-Dist: docmesh>=0.0.5
 Requires-Dist: langchain>=0.1.15
 Requires-Dist: langchain-openai>=0.1.3
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docmesh agent
```

