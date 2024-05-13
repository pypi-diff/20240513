# Comparing `tmp/conva_ai-0.0.8.tar.gz` & `tmp/conva_ai-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conva_ai-0.0.8.tar", last modified: Fri Apr 19 19:00:08 2024, max compression
+gzip compressed data, was "conva_ai-0.1.0.tar", last modified: Mon May 13 15:08:36 2024, max compression
```

## Comparing `conva_ai-0.0.8.tar` & `conva_ai-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 19:00:08.632023 conva_ai-0.0.8/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3178 2024-04-19 19:00:08.631725 conva_ai-0.0.8/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     2533 2024-04-19 18:59:51.000000 conva_ai-0.0.8/README.md
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 19:00:08.629421 conva_ai-0.0.8/conva_ai/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-19 08:25:37.000000 conva_ai-0.0.8/conva_ai/__init__.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      648 2024-04-19 13:17:53.000000 conva_ai-0.0.8/conva_ai/base.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     1900 2024-04-19 12:11:13.000000 conva_ai-0.0.8/conva_ai/client.py
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      667 2024-04-19 08:25:37.000000 conva_ai-0.0.8/conva_ai/response.py
-drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-04-19 19:00:08.631193 conva_ai-0.0.8/conva_ai.egg-info/
--rw-r--r--   0 harikrishnanc   (501) staff       (20)     3178 2024-04-19 19:00:08.000000 conva_ai-0.0.8/conva_ai.egg-info/PKG-INFO
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-04-19 19:00:08.000000 conva_ai-0.0.8/conva_ai.egg-info/SOURCES.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-04-19 19:00:08.000000 conva_ai-0.0.8/conva_ai.egg-info/dependency_links.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      107 2024-04-19 19:00:08.000000 conva_ai-0.0.8/conva_ai.egg-info/requires.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-04-19 19:00:08.000000 conva_ai-0.0.8/conva_ai.egg-info/top_level.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      652 2024-04-19 18:59:51.000000 conva_ai-0.0.8/pyproject.toml
--rw-r--r--   0 harikrishnanc   (501) staff       (20)      467 2024-04-19 08:25:37.000000 conva_ai-0.0.8/requirements.txt
--rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-04-19 19:00:08.632228 conva_ai-0.0.8/setup.cfg
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.063070 conva_ai-0.1.0/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3650 2024-05-13 15:08:36.062804 conva_ai-0.1.0/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     2844 2024-05-13 15:07:54.000000 conva_ai-0.1.0/README.md
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.061287 conva_ai-0.1.0/conva_ai/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       41 2024-04-20 05:49:43.000000 conva_ai-0.1.0/conva_ai/__init__.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      677 2024-05-13 15:07:54.000000 conva_ai-0.1.0/conva_ai/base.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     4015 2024-05-13 15:07:54.000000 conva_ai-0.1.0/conva_ai/client.py
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      604 2024-04-25 13:45:56.000000 conva_ai-0.1.0/conva_ai/response.py
+drwxr-xr-x   0 harikrishnanc   (501) staff       (20)        0 2024-05-13 15:08:36.062471 conva_ai-0.1.0/conva_ai.egg-info/
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)     3650 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/PKG-INFO
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      278 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        1 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      193 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/requires.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)        9 2024-05-13 15:08:36.000000 conva_ai-0.1.0/conva_ai.egg-info/top_level.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      652 2024-05-13 15:07:54.000000 conva_ai-0.1.0/pyproject.toml
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)      571 2024-04-23 09:58:39.000000 conva_ai-0.1.0/requirements.txt
+-rw-r--r--   0 harikrishnanc   (501) staff       (20)       38 2024-05-13 15:08:36.063138 conva_ai-0.1.0/setup.cfg
```

### Comparing `conva_ai-0.0.8/PKG-INFO` & `conva_ai-0.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,79 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.8
+Version: 0.1.0
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types==0.6.0
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: idna==3.7
 Requires-Dist: pydantic==2.7.0
 Requires-Dist: pydantic-core==2.18.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: sseclient-py==1.8.0
 Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: urllib3==2.2.1
 
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```
 import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
 
 final_response = asyncio.run(generate(client, "how are you", True))
 print(final_response)
 ```
 
+You can try out the co-pilot on [Google Colab](https://colab.research.google.com/drive/1WtbARTRQ9wCvztrAQuEhQUvwImhtPZXd#scrollTo=ZSVBQsOelgfv)
+
+If you want to get the response as dictionary, then replace
+```
+out = res.model_dump_json(indent=4)
+```
+
+with
+```
+out = res.model_dump()
+```
+
 ### 2. How to clear history
 
 Conva AI client, by default keeps track of your conversation history and uses it as the context for responding intelligently
 
 You can clear conversation history by executing the below code:
 
 ```
 from conva_ai.client import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 client.clear_history()
 ```
 
 In case you are buliding an application where you don't want to track conversation history, you can disable history tracking
 
@@ -75,16 +92,16 @@
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
 import asyncio
 from conva_ai.client import AsyncConvaAI
 
 client = AsyncConvaAI(
-        copilot_id="<YOUR_COPILOT_ID>", 
-        copilot_version="<YOUR_COPILOT_VERSION>", 
+        assistant_id="<YOUR_ASSISTANT_ID>", 
+        assistant_version="<YOUR_ASSISTANT_VERSION>", 
         api_key="<YOUR_API_KEY>"
     )
 
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out=""
     async for res in response:
```

### Comparing `conva_ai-0.0.8/README.md` & `conva_ai-0.1.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,40 +5,52 @@
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```
 import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
 
 final_response = asyncio.run(generate(client, "how are you", True))
 print(final_response)
 ```
 
+You can try out the co-pilot on [Google Colab](https://colab.research.google.com/drive/1WtbARTRQ9wCvztrAQuEhQUvwImhtPZXd#scrollTo=ZSVBQsOelgfv)
+
+If you want to get the response as dictionary, then replace
+```
+out = res.model_dump_json(indent=4)
+```
+
+with
+```
+out = res.model_dump()
+```
+
 ### 2. How to clear history
 
 Conva AI client, by default keeps track of your conversation history and uses it as the context for responding intelligently
 
 You can clear conversation history by executing the below code:
 
 ```
 from conva_ai.client import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 client.clear_history()
 ```
 
 In case you are buliding an application where you don't want to track conversation history, you can disable history tracking
 
@@ -57,16 +69,16 @@
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
 import asyncio
 from conva_ai.client import AsyncConvaAI
 
 client = AsyncConvaAI(
-        copilot_id="<YOUR_COPILOT_ID>", 
-        copilot_version="<YOUR_COPILOT_VERSION>", 
+        assistant_id="<YOUR_ASSISTANT_ID>", 
+        assistant_version="<YOUR_ASSISTANT_VERSION>", 
         api_key="<YOUR_API_KEY>"
     )
 
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out=""
     async for res in response:
```

### Comparing `conva_ai-0.0.8/conva_ai/base.py` & `conva_ai-0.1.0/conva_ai/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import uuid
 import requests
 
 
 class BaseClient:
 
-    def __init__(self, copilot_id: str, copilot_version: str, api_key: str, host: str = "https://infer.conva.ai"):
-        self.copilot_id: str = copilot_id
+    def __init__(self, assistant_id: str, assistant_version: str, api_key: str, host: str = "https://infer.conva.ai"):
+        self.assistant_id: str = assistant_id
         self.api_key: str = api_key
-        self.copilot_version: str = copilot_version
+        self.assistant_version: str = assistant_version
         self.host: str = host
         self.keep_conversation_history: bool = True
         self.domain: str = ""
         self.history: str = ""
 
     def clear_history(self):
         """
         Clears the history tracked by the client
         """
         self.history: str = ""
 
     def use_history(self, use_history):
-        self.history = use_history
-
+        self.keep_conversation_history = use_history
```

### Comparing `conva_ai-0.0.8/conva_ai/response.py` & `conva_ai-0.1.0/conva_ai/response.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,16 +9,14 @@
     response_language: str
     is_final: bool
     domain_name: str | None = None
     app_name: str | None = None
     category: str | None = None
     llm_key: str | None = None
     message_type: str | None = None
-    app_action: str | None = None
     parameters: Dict[str, Any] = {}
-    hints: List[str] = []
-    suggestions: List[Dict[str, Any]] = []
     related_queries: List[str] = []
     conversation_history: str = ""
     is_error: bool = False
     is_unsupported: bool = False
     tool_name: str = ""
+    is_parameter_complete: bool = False
```

### Comparing `conva_ai-0.0.8/conva_ai.egg-info/PKG-INFO` & `conva_ai-0.1.0/conva_ai.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,79 @@
 Metadata-Version: 2.1
 Name: conva_ai
-Version: 0.0.8
+Version: 0.1.0
 Summary: Python SDK for using Conva AI co-pilots
 Author-email: Slang Labs <support@slanglabs.in>
 Project-URL: Homepage, http://www.slanglabs.in
 Project-URL: Documentation, https://docs.slanglabs.in/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types==0.6.0
+Requires-Dist: certifi==2024.2.2
+Requires-Dist: charset-normalizer==3.3.2
+Requires-Dist: idna==3.7
 Requires-Dist: pydantic==2.7.0
 Requires-Dist: pydantic-core==2.18.1
+Requires-Dist: requests==2.31.0
 Requires-Dist: sseclient-py==1.8.0
 Requires-Dist: typing-extensions==4.11.0
+Requires-Dist: urllib3==2.2.1
 
 # Python Library for Conva AI
 
 This is the python library for using Conva AI Co-pilots
 
 ## Examples
 
 ### 1. A simple example for generating response using Conva Co-pilot
 ```
 import asyncio
 from conva_ai import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out = ""
     async for res in response:
         out = res.model_dump_json(indent=4)
     return out
 
 final_response = asyncio.run(generate(client, "how are you", True))
 print(final_response)
 ```
 
+You can try out the co-pilot on [Google Colab](https://colab.research.google.com/drive/1WtbARTRQ9wCvztrAQuEhQUvwImhtPZXd#scrollTo=ZSVBQsOelgfv)
+
+If you want to get the response as dictionary, then replace
+```
+out = res.model_dump_json(indent=4)
+```
+
+with
+```
+out = res.model_dump()
+```
+
 ### 2. How to clear history
 
 Conva AI client, by default keeps track of your conversation history and uses it as the context for responding intelligently
 
 You can clear conversation history by executing the below code:
 
 ```
 from conva_ai.client import AsyncConvaAI
 client = AsyncConvaAI(
-    copilot_id="<YOUR_COPILOT_ID>", 
-    copilot_version="<YOUR_COPILOT_VERSION>", 
+    assistant_id="<YOUR_ASSISTANT_ID>", 
+    assistant_version="<YOUR_ASSISTANT_VERSION>", 
     api_key="<YOUR_API_KEY>"
 )
 client.clear_history()
 ```
 
 In case you are buliding an application where you don't want to track conversation history, you can disable history tracking
 
@@ -75,16 +92,16 @@
 Conva AI uses generative AI to give you the response to your query. In order for you to understand the reasoning behind the response. We also provide you with AI's reasoning
 
 ```
 import asyncio
 from conva_ai.client import AsyncConvaAI
 
 client = AsyncConvaAI(
-        copilot_id="<YOUR_COPILOT_ID>", 
-        copilot_version="<YOUR_COPILOT_VERSION>", 
+        assistant_id="<YOUR_ASSISTANT_ID>", 
+        assistant_version="<YOUR_ASSISTANT_VERSION>", 
         api_key="<YOUR_API_KEY>"
     )
 
 async def generate(client: AsyncConvaAI, query: str, stream: bool):
     response = client.invoke_capability(query, stream=stream)
     out=""
     async for res in response:
```

### Comparing `conva_ai-0.0.8/pyproject.toml` & `conva_ai-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "conva_ai"
-version = "0.0.8"
+version = "0.1.0"
 authors = [
   { name="Slang Labs", email="support@slanglabs.in" },
 ]
 dynamic = ["dependencies"]
 description = "Python SDK for using Conva AI co-pilots"
 readme = "README.md"
 requires-python = ">=3.10"
```

