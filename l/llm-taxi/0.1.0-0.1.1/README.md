# Comparing `tmp/llm_taxi-0.1.0.tar.gz` & `tmp/llm_taxi-0.1.1.tar.gz`

## Comparing `llm_taxi-0.1.0.tar` & `llm_taxi-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/.python-version
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/pyrightconfig.json
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/conversation.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/factory.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/anthropic.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/base.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/dashscope.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/deepinfra.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/deepseek.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/google.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/groq.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/mistral.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/openai.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/openrouter.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/perplexity.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/together.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/tests/test_llm.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/.python-version
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/pyrightconfig.json
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/requirements-dev.lock
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/conversation.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/factory.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/anthropic.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/base.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/dashscope.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/deepinfra.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/deepseek.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/google.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/groq.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/mistral.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/openai.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/openrouter.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/perplexity.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/together.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/tests/test_llm.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/PKG-INFO
```

### Comparing `llm_taxi-0.1.0/requirements-dev.lock` & `llm_taxi-0.1.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/requirements.lock` & `llm_taxi-0.1.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/factory.py` & `llm_taxi-0.1.1/src/llm_taxi/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,19 +47,20 @@
     **client_kwargs,
 ) -> LLM:
     provider, model = model.split(":", 1)
     if not (model_class := MODEL_CLASSES.get(provider)):
         msg = f"Unknown LLM provider: {provider}"
         raise ValueError(msg)
 
-    env_vars = model_class.env_vars
-    env_var_values: dict[str, str] = {
-        k: param if (param := locals().get(k)) is not None else _get_env(v)
-        for k, v in env_vars.items()
-    }
+    env_var_values: dict[str, str] = {}
+    for key, env_name in model_class.env_vars.items():
+        value = (
+            params if (params := locals().get(key)) is not None else _get_env(env_name)
+        )
+        env_var_values[key] = value
 
     return model_class(
         model=model,
         **env_var_values,
         call_kwargs=call_kwargs,
         **client_kwargs,
     )
```

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/__init__.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/anthropic.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/base.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/base.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/google.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/google.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/groq.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/groq.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/mistral.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/mistral.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/src/llm_taxi/llms/openai.py` & `llm_taxi-0.1.1/src/llm_taxi/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.0/tests/test_llm.py` & `llm_taxi-0.1.1/tests/test_llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import copy
 
 from llm_taxi.conversation import Message, Role
 from llm_taxi.factory import llm
 
 
 async def main():
     clients = [
@@ -14,15 +15,19 @@
         llm(model="mistral:mistral-small"),
         llm(model="perplexity:llama-3-8b-instruct"),
         llm(model="deepinfra:meta-llama/Meta-Llama-3-8B-Instruct"),
         llm(model="deepseek:deepseek-chat"),
         llm(model="openrouter:rwkv/rwkv-5-world-3b"),
         llm(model="dashscope:qwen-turbo"),
     ]
+
     for client in clients:
+        print(client.model)
+        copy.deepcopy(client)
+
         messages = [
             Message(role=Role.User, content="What is the capital of France?"),
         ]
         response = await client.response(messages)
         print(response)
 
         response = await client.streaming_response(messages)
```

### Comparing `llm_taxi-0.1.0/pyproject.toml` & `llm_taxi-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 [project]
 name = "llm-taxi"
-version = "0.1.0"
+version = "0.1.1"
 description = "Add your description here"
-authors = [
-    { name = "Yevgnen Koh", email = "wherejoystarts@gmail.com" }
-]
+authors = [{ name = "Yevgnen Koh", email = "wherejoystarts@gmail.com" }]
 dependencies = [
     "openai>=1.28.1",
     "pydantic>=2.7.1",
     "google-generativeai>=0.5.2",
     "together>=1.1.5",
     "groq>=0.5.0",
     "anthropic>=0.25.8",
```

