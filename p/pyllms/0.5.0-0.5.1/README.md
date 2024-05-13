# Comparing `tmp/pyllms-0.5.0.tar.gz` & `tmp/pyllms-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllms-0.5.0.tar", last modified: Mon Mar 25 16:00:20 2024, max compression
+gzip compressed data, was "pyllms-0.5.1.tar", last modified: Mon May 13 18:28:46 2024, max compression
```

## Comparing `pyllms-0.5.0.tar` & `pyllms-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-03-25 16:00:20.184847 pyllms-0.5.0/
--rw-r--r--   0 prelovac   (502) staff       (20)     1068 2024-03-24 05:01:59.000000 pyllms-0.5.0/LICENSE
--rw-r--r--   0 prelovac   (502) staff       (20)    13697 2024-03-25 16:00:20.184397 pyllms-0.5.0/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)    11789 2024-03-24 05:01:59.000000 pyllms-0.5.0/README.md
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-03-25 16:00:20.176775 pyllms-0.5.0/llms/
--rw-r--r--   0 prelovac   (502) staff       (20)      295 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)    22355 2024-03-24 05:09:05.000000 pyllms-0.5.0/llms/llms.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-03-25 16:00:20.181247 pyllms-0.5.0/llms/providers/
--rw-r--r--   0 prelovac   (502) staff       (20)      437 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1910 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/ai21.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3008 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/aleph.py
--rw-r--r--   0 prelovac   (502) staff       (20)    13786 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1914 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/base_provider.py
--rw-r--r--   0 prelovac   (502) staff       (20)     1779 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/bedrock_anthropic.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3655 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/cohere.py
--rw-r--r--   0 prelovac   (502) staff       (20)     4319 2024-03-25 15:38:17.000000 pyllms-0.5.0/llms/providers/google.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3729 2024-03-25 15:44:45.000000 pyllms-0.5.0/llms/providers/google_genai.py
--rw-r--r--   0 prelovac   (502) staff       (20)     3472 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/huggingface.py
--rw-r--r--   0 prelovac   (502) staff       (20)     8875 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/mistral.py
--rw-r--r--   0 prelovac   (502) staff       (20)     6864 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/ollama.py
--rw-r--r--   0 prelovac   (502) staff       (20)    12192 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/providers/openai.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-03-25 16:00:20.181808 pyllms-0.5.0/llms/results/
--rw-r--r--   0 prelovac   (502) staff       (20)        0 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/results/__init__.py
--rw-r--r--   0 prelovac   (502) staff       (20)     9387 2024-03-24 05:01:59.000000 pyllms-0.5.0/llms/results/result.py
-drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-03-25 16:00:20.183696 pyllms-0.5.0/pyllms.egg-info/
--rw-r--r--   0 prelovac   (502) staff       (20)    13697 2024-03-25 16:00:20.000000 pyllms-0.5.0/pyllms.egg-info/PKG-INFO
--rw-r--r--   0 prelovac   (502) staff       (20)      610 2024-03-25 16:00:20.000000 pyllms-0.5.0/pyllms.egg-info/SOURCES.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        1 2024-03-25 16:00:20.000000 pyllms-0.5.0/pyllms.egg-info/dependency_links.txt
--rw-r--r--   0 prelovac   (502) staff       (20)      232 2024-03-25 16:00:20.000000 pyllms-0.5.0/pyllms.egg-info/requires.txt
--rw-r--r--   0 prelovac   (502) staff       (20)        5 2024-03-25 16:00:20.000000 pyllms-0.5.0/pyllms.egg-info/top_level.txt
--rw-r--r--   0 prelovac   (502) staff       (20)       38 2024-03-25 16:00:20.184935 pyllms-0.5.0/setup.cfg
--rw-r--r--   0 prelovac   (502) staff       (20)     2211 2024-03-25 15:59:46.000000 pyllms-0.5.0/setup.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-13 18:28:46.327683 pyllms-0.5.1/
+-rw-r--r--   0 prelovac   (502) staff       (20)     1068 2024-03-24 05:01:59.000000 pyllms-0.5.1/LICENSE
+-rw-r--r--   0 prelovac   (502) staff       (20)    13956 2024-05-13 18:28:46.327076 pyllms-0.5.1/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)    12081 2024-05-13 18:24:37.000000 pyllms-0.5.1/README.md
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-13 18:28:46.319052 pyllms-0.5.1/llms/
+-rw-r--r--   0 prelovac   (502) staff       (20)      295 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    22355 2024-04-23 00:34:45.000000 pyllms-0.5.1/llms/llms.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-13 18:28:46.323381 pyllms-0.5.1/llms/providers/
+-rw-r--r--   0 prelovac   (502) staff       (20)      437 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1910 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/ai21.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3008 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/aleph.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    13796 2024-05-13 18:26:37.000000 pyllms-0.5.1/llms/providers/anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     1914 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/base_provider.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     2138 2024-05-13 18:26:37.000000 pyllms-0.5.1/llms/providers/bedrock_anthropic.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3655 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/cohere.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     4319 2024-03-25 15:38:17.000000 pyllms-0.5.1/llms/providers/google.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3729 2024-03-25 15:44:45.000000 pyllms-0.5.1/llms/providers/google_genai.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     3472 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/huggingface.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     8875 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/mistral.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     6864 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/providers/ollama.py
+-rw-r--r--   0 prelovac   (502) staff       (20)    12434 2024-05-13 18:27:08.000000 pyllms-0.5.1/llms/providers/openai.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-13 18:28:46.324098 pyllms-0.5.1/llms/results/
+-rw-r--r--   0 prelovac   (502) staff       (20)        0 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/results/__init__.py
+-rw-r--r--   0 prelovac   (502) staff       (20)     9387 2024-03-24 05:01:59.000000 pyllms-0.5.1/llms/results/result.py
+drwxr-xr-x   0 prelovac   (502) staff       (20)        0 2024-05-13 18:28:46.326266 pyllms-0.5.1/pyllms.egg-info/
+-rw-r--r--   0 prelovac   (502) staff       (20)    13956 2024-05-13 18:28:46.000000 pyllms-0.5.1/pyllms.egg-info/PKG-INFO
+-rw-r--r--   0 prelovac   (502) staff       (20)      610 2024-05-13 18:28:46.000000 pyllms-0.5.1/pyllms.egg-info/SOURCES.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        1 2024-05-13 18:28:46.000000 pyllms-0.5.1/pyllms.egg-info/dependency_links.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)      214 2024-05-13 18:28:46.000000 pyllms-0.5.1/pyllms.egg-info/requires.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)        5 2024-05-13 18:28:46.000000 pyllms-0.5.1/pyllms.egg-info/top_level.txt
+-rw-r--r--   0 prelovac   (502) staff       (20)       38 2024-05-13 18:28:46.327783 pyllms-0.5.1/setup.cfg
+-rw-r--r--   0 prelovac   (502) staff       (20)     2182 2024-05-13 18:26:56.000000 pyllms-0.5.1/setup.py
```

### Comparing `pyllms-0.5.0/LICENSE` & `pyllms-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/PKG-INFO` & `pyllms-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.5.0
+Version: 0.5.1
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, Mistral, Ollama, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub,vertex ai,palm,palm2
@@ -22,22 +22,21 @@
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1
 Requires-Dist: tiktoken
 Requires-Dist: anthropic>=0.18
-Requires-Dist: anthropic_bedrock
 Requires-Dist: ai21
 Requires-Dist: cohere
 Requires-Dist: aleph-alpha-client
 Requires-Dist: huggingface_hub
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: prettytable
-Requires-Dist: protobuf~=3.20.3
+Requires-Dist: protobuf>=3.20.3
 Requires-Dist: grpcio~=1.54.2
 Requires-Dist: google-generativeai
 Requires-Dist: mistralai
 Requires-Dist: ollama
 Provides-Extra: local
 Requires-Dist: einops; extra == "local"
 Requires-Dist: accelerate; extra == "local"
@@ -254,14 +253,16 @@
 | GoogleProvider('chat-bison') | Total Tokens: 2759 | Total Cost: 0.00689 | Median Latency: 2.83 | Aggregated speed: 36.24 | Accuracy: 19.23% |
 | GoogleProvider('text-bison') | Total Tokens: 1155 | Total Cost: 0.00897 | Median Latency: 0.38 | Aggregated speed: 60.60 | Accuracy: 25.64% |
 | CohereProvider('command') | Total Tokens: 4033 | Total Cost: 0.08125 | Median Latency: 5.77 | Aggregated speed: 9.44 | Accuracy: 11.54% |
 | OpenAIProvider('gpt-3.5-turbo') | Total Tokens: 2570 | Total Cost: 0.00825 | Median Latency: 2.38 | Aggregated speed: 30.47 | Accuracy: 38.46% |
 | OpenAIProvider('gpt-4') | Total Tokens: 2860 | Total Cost: 0.21837 | Median Latency: 3.22 | Aggregated speed: 10.52 | Accuracy: 44.87% |
 | AnthropicProvider('claude-instant-v1') | Total Tokens: 3437 | Total Cost: 0.02153 | Median Latency: 1.84 | Aggregated speed: 61.64 | Accuracy: 42.31% |
 | AnthropicProvider('claude-2') | Total Tokens: 3545 | Total Cost: 0.13337 | Median Latency: 6.83 | Aggregated speed: 19.51 | Accuracy: 69.23% |
+| OpenAIProvider('gpt-4-turbo') | Total Tokens: 5538 | Total Cost: 0.18256 | Median Latency: 10.68 | Aggregated speed: 14.45 | Accuracy: 74.07% |
+|    OpenAIProvider('gpt-4o')   | Total Tokens: 6483 | Total Cost: 0.10539 |  Median Latency: 1.91 | Aggregated speed: 94.01 | Accuracy: 85.19% |
 +-------------------------------+--------------------+---------------------+----------------------+-------------------------+------------------+
 
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
```

### Comparing `pyllms-0.5.0/README.md` & `pyllms-0.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -210,14 +210,16 @@
 | GoogleProvider('chat-bison') | Total Tokens: 2759 | Total Cost: 0.00689 | Median Latency: 2.83 | Aggregated speed: 36.24 | Accuracy: 19.23% |
 | GoogleProvider('text-bison') | Total Tokens: 1155 | Total Cost: 0.00897 | Median Latency: 0.38 | Aggregated speed: 60.60 | Accuracy: 25.64% |
 | CohereProvider('command') | Total Tokens: 4033 | Total Cost: 0.08125 | Median Latency: 5.77 | Aggregated speed: 9.44 | Accuracy: 11.54% |
 | OpenAIProvider('gpt-3.5-turbo') | Total Tokens: 2570 | Total Cost: 0.00825 | Median Latency: 2.38 | Aggregated speed: 30.47 | Accuracy: 38.46% |
 | OpenAIProvider('gpt-4') | Total Tokens: 2860 | Total Cost: 0.21837 | Median Latency: 3.22 | Aggregated speed: 10.52 | Accuracy: 44.87% |
 | AnthropicProvider('claude-instant-v1') | Total Tokens: 3437 | Total Cost: 0.02153 | Median Latency: 1.84 | Aggregated speed: 61.64 | Accuracy: 42.31% |
 | AnthropicProvider('claude-2') | Total Tokens: 3545 | Total Cost: 0.13337 | Median Latency: 6.83 | Aggregated speed: 19.51 | Accuracy: 69.23% |
+| OpenAIProvider('gpt-4-turbo') | Total Tokens: 5538 | Total Cost: 0.18256 | Median Latency: 10.68 | Aggregated speed: 14.45 | Accuracy: 74.07% |
+|    OpenAIProvider('gpt-4o')   | Total Tokens: 6483 | Total Cost: 0.10539 |  Median Latency: 1.91 | Aggregated speed: 94.01 | Accuracy: 85.19% |
 +-------------------------------+--------------------+---------------------+----------------------+-------------------------+------------------+
 
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
```

### Comparing `pyllms-0.5.0/llms/llms.py` & `pyllms-0.5.1/llms/llms.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/ai21.py` & `pyllms-0.5.1/llms/providers/ai21.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/aleph.py` & `pyllms-0.5.1/llms/providers/aleph.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/anthropic.py` & `pyllms-0.5.1/llms/providers/anthropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 
         if system_message and self.model.startswith("claude-instant"):
             raise ValueError("System message is not supported for Claude instant")
         model_inputs = {
             "messages": messages,
             "system": system_message,
             "temperature": temperature,
-            "max_tokens": max_tokens,
+            "max_tokens_to_sample": max_tokens,
             "stop_sequences": stop_sequences,
         }
         return model_inputs
 
     def _prepare_model_inputs(
         self,
         prompt: str,
```

### Comparing `pyllms-0.5.0/llms/providers/base_provider.py` & `pyllms-0.5.1/llms/providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/bedrock_anthropic.py` & `pyllms-0.5.1/llms/providers/bedrock_anthropic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # llms/providers/bedrock_anthropic.py
 
 import os
 from typing import Union
 
-import anthropic_bedrock
+from anthropic import AnthropicBedrock, AsyncAnthropicBedrock
 
 from .anthropic import AnthropicProvider
 
 
 class BedrockAnthropicProvider(AnthropicProvider):
     MODEL_INFO = {
         "anthropic.claude-instant-v1": {"prompt": 1.63, "completion": 5.51, "token_limit": 9000},
         "anthropic.claude-v1": {
             "prompt": 11.02,
             "completion": 32.68,
             "token_limit": 100_000,
         },
         "anthropic.claude-v2": {"prompt": 11.02, "completion": 32.68, "token_limit": 100_000},
+        "anthropic.claude-3-haiku-20240307-v1:0": {"prompt": 0.25, "completion": 1.25, "token_limit": 200_000, "output_limit": 4_096},
+        "anthropic.claude-3-sonnet-20240229-v1:0": {"prompt": 3.00, "completion": 15, "token_limit": 200_000, "output_limit": 4_096},
     }
 
     def __init__(
         self,
         model: Union[str, None] = None,
         aws_access_key: Union[str, None] = None,
         aws_secret_key: Union[str, None] = None,
@@ -35,22 +37,26 @@
         if aws_access_key is None:
             aws_access_key = os.getenv("AWS_ACCESS_KEY_ID")
         if aws_secret_key is None:
             aws_access_key = os.getenv("AWS_SECRET_ACCESS_KEY")
 
         if client_kwargs is None:
             client_kwargs = {}
-        self.client = anthropic_bedrock.AnthropicBedrock(
+        self.client = AnthropicBedrock(
             aws_access_key=aws_access_key,
             aws_secret_key=aws_secret_key,
             aws_region=aws_region,
             **client_kwargs,
         )
 
         if async_client_kwargs is None:
             async_client_kwargs = {}
-        self.async_client = anthropic_bedrock.AsyncAnthropicBedrock(
+        self.async_client = AsyncAnthropicBedrock(
             aws_access_key=aws_access_key,
             aws_secret_key=aws_secret_key,
             aws_region=aws_region,
             **async_client_kwargs,
         )
+
+    @property
+    def support_message_api(self):
+        return "claude-3" in self.model
```

### Comparing `pyllms-0.5.0/llms/providers/cohere.py` & `pyllms-0.5.1/llms/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/google.py` & `pyllms-0.5.1/llms/providers/google.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/google_genai.py` & `pyllms-0.5.1/llms/providers/google_genai.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/huggingface.py` & `pyllms-0.5.1/llms/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/mistral.py` & `pyllms-0.5.1/llms/providers/mistral.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/ollama.py` & `pyllms-0.5.1/llms/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/llms/providers/openai.py` & `pyllms-0.5.1/llms/providers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     MODEL_INFO = {
         "gpt-3.5-turbo": {"prompt": 2.0, "completion": 2.0, "token_limit": 16_385, "is_chat": True, "output_limit": 4_096},
         "gpt-3.5-turbo-1106": {"prompt": 2.0, "completion": 2.0, "token_limit": 16_385, "is_chat": True, "output_limit": 4_096},
         "gpt-3.5-turbo-instruct": {"prompt": 2.0, "completion": 2.0, "token_limit": 4096, "is_chat": False},
         "gpt-4": {"prompt": 30.0, "completion": 60.0, "token_limit": 8192, "is_chat": True},
         "gpt-4-1106-preview": {"prompt": 10.0, "completion": 30.0, "token_limit": 128000, "is_chat": True, "output_limit": 4_096},
         "gpt-4-turbo-preview": {"prompt": 10.0, "completion": 30.0, "token_limit": 128000, "is_chat": True, "output_limit": 4_096},
+        "gpt-4-turbo": {"prompt": 10.0, "completion": 30.0, "token_limit": 128000, "is_chat": True, "output_limit": 4_096},
+        "gpt-4o": {"prompt": 5.0, "completion": 15.0, "token_limit": 128000, "is_chat": True, "output_limit": 4_096},
     }
 
     def __init__(
         self,
         api_key: Union[str, None] = None,
         model: Union[str, None] = None,
         client_kwargs: Union[dict, None] = None,
```

### Comparing `pyllms-0.5.0/llms/results/result.py` & `pyllms-0.5.1/llms/results/result.py`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/pyllms.egg-info/PKG-INFO` & `pyllms-0.5.1/pyllms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllms
-Version: 0.5.0
+Version: 0.5.1
 Summary: Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, Mistral, Ollama, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.
 Author: Vladimir Prelovac
 Author-email: vlad@kagi.com
 Project-URL: Documentation, https://github.com/kagisearch/pyllms
 Project-URL: Source Code, https://github.com/kagisearch/pyllms
 Project-URL: Issue Tracker, https://github.com/kagisearch/pyllms/issues
 Keywords: llm,llms,large language model,AI,NLP,natural language processing,gpt,chatgpt,openai,anthropic,ai21,cohere,aleph alpha,huggingface hub,vertex ai,palm,palm2
@@ -22,22 +22,21 @@
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai>=1
 Requires-Dist: tiktoken
 Requires-Dist: anthropic>=0.18
-Requires-Dist: anthropic_bedrock
 Requires-Dist: ai21
 Requires-Dist: cohere
 Requires-Dist: aleph-alpha-client
 Requires-Dist: huggingface_hub
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: prettytable
-Requires-Dist: protobuf~=3.20.3
+Requires-Dist: protobuf>=3.20.3
 Requires-Dist: grpcio~=1.54.2
 Requires-Dist: google-generativeai
 Requires-Dist: mistralai
 Requires-Dist: ollama
 Provides-Extra: local
 Requires-Dist: einops; extra == "local"
 Requires-Dist: accelerate; extra == "local"
@@ -254,14 +253,16 @@
 | GoogleProvider('chat-bison') | Total Tokens: 2759 | Total Cost: 0.00689 | Median Latency: 2.83 | Aggregated speed: 36.24 | Accuracy: 19.23% |
 | GoogleProvider('text-bison') | Total Tokens: 1155 | Total Cost: 0.00897 | Median Latency: 0.38 | Aggregated speed: 60.60 | Accuracy: 25.64% |
 | CohereProvider('command') | Total Tokens: 4033 | Total Cost: 0.08125 | Median Latency: 5.77 | Aggregated speed: 9.44 | Accuracy: 11.54% |
 | OpenAIProvider('gpt-3.5-turbo') | Total Tokens: 2570 | Total Cost: 0.00825 | Median Latency: 2.38 | Aggregated speed: 30.47 | Accuracy: 38.46% |
 | OpenAIProvider('gpt-4') | Total Tokens: 2860 | Total Cost: 0.21837 | Median Latency: 3.22 | Aggregated speed: 10.52 | Accuracy: 44.87% |
 | AnthropicProvider('claude-instant-v1') | Total Tokens: 3437 | Total Cost: 0.02153 | Median Latency: 1.84 | Aggregated speed: 61.64 | Accuracy: 42.31% |
 | AnthropicProvider('claude-2') | Total Tokens: 3545 | Total Cost: 0.13337 | Median Latency: 6.83 | Aggregated speed: 19.51 | Accuracy: 69.23% |
+| OpenAIProvider('gpt-4-turbo') | Total Tokens: 5538 | Total Cost: 0.18256 | Median Latency: 10.68 | Aggregated speed: 14.45 | Accuracy: 74.07% |
+|    OpenAIProvider('gpt-4o')   | Total Tokens: 6483 | Total Cost: 0.10539 |  Median Latency: 1.91 | Aggregated speed: 94.01 | Accuracy: 85.19% |
 +-------------------------------+--------------------+---------------------+----------------------+-------------------------+------------------+
 
 ```
 
 To evaluate models on your own prompts, simply pass a list of questions and optional answers as tuple. The evaluator will automatically evaluate the responses:
 
 ```
```

### Comparing `pyllms-0.5.0/pyllms.egg-info/SOURCES.txt` & `pyllms-0.5.1/pyllms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllms-0.5.0/setup.py` & `pyllms-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 _project_homepage = "https://github.com/kagisearch/pyllms"
 
 setup(
     name="pyllms",
-    version="0.5.0",
+    version="0.5.1",
     description="Minimal Python library to connect to LLMs (OpenAI, Anthropic, Google Palm2/Vertex, Mistral, Ollama, AI21, Cohere, Aleph-Alpha, HuggingfaceHub), with a built-in model performance benchmark.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Vladimir Prelovac",
     author_email="vlad@kagi.com",
     packages=find_packages(),
     install_requires=[
         "openai>=1",
         "tiktoken",
         "anthropic>=0.18",
-        "anthropic_bedrock",
         "ai21",
         "cohere",
         "aleph-alpha-client",
         "huggingface_hub",
         "google-cloud-aiplatform",
         "prettytable",
-        "protobuf~=3.20.3",
+        "protobuf>=3.20.3",
         "grpcio~=1.54.2",
         "google-generativeai",
         "mistralai",
         "ollama",
     ],
     extras_require={
         "local": ["einops", "accelerate"]
```

