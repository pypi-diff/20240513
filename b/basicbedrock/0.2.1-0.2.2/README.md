# Comparing `tmp/basicbedrock-0.2.1.tar.gz` & `tmp/basicbedrock-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basicbedrock-0.2.1.tar", last modified: Sat May 11 00:13:56 2024, max compression
+gzip compressed data, was "basicbedrock-0.2.2.tar", last modified: Mon May 13 21:26:57 2024, max compression
```

## Comparing `basicbedrock-0.2.1.tar` & `basicbedrock-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.243411 basicbedrock-0.2.1/
--rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.2.1/LICENSE
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-11 00:13:56.242588 basicbedrock-0.2.1/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.2.1/README.md
--rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-05-11 00:13:40.000000 basicbedrock-0.2.1/pyproject.toml
--rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-05-11 00:13:56.243515 basicbedrock-0.2.1/setup.cfg
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.236473 basicbedrock-0.2.1/src/
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.237928 basicbedrock-0.2.1/src/basicbedrock/
--rw-r--r--   0 dmattsn    (504) staff       (20)      330 2024-05-11 00:13:40.000000 basicbedrock-0.2.1/src/basicbedrock/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    19081 2024-05-11 00:13:29.000000 basicbedrock-0.2.1/src/basicbedrock/basicbedrock.py
--rw-r--r--   0 dmattsn    (504) staff       (20)    10079 2024-05-10 19:42:41.000000 basicbedrock-0.2.1/src/basicbedrock/guardrails.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     7632 2024-05-02 02:20:16.000000 basicbedrock-0.2.1/src/basicbedrock/guardrails_baseclasses.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.240561 basicbedrock-0.2.1/src/basicbedrock/models/
--rw-r--r--   0 dmattsn    (504) staff       (20)     6371 2024-04-30 18:13:06.000000 basicbedrock-0.2.1/src/basicbedrock/models/__init__.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2897 2024-04-30 18:26:06.000000 basicbedrock-0.2.1/src/basicbedrock/models/ai21.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5787 2024-04-30 18:26:06.000000 basicbedrock-0.2.1/src/basicbedrock/models/amazon.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5070 2024-04-30 18:28:26.000000 basicbedrock-0.2.1/src/basicbedrock/models/anthropic.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     5241 2024-04-11 00:27:04.000000 basicbedrock-0.2.1/src/basicbedrock/models/baseclasses.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3450 2024-04-30 18:26:06.000000 basicbedrock-0.2.1/src/basicbedrock/models/cohere.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     3694 2024-04-30 18:26:06.000000 basicbedrock-0.2.1/src/basicbedrock/models/meta.py
--rw-r--r--   0 dmattsn    (504) staff       (20)     2353 2024-04-30 18:44:40.000000 basicbedrock-0.2.1/src/basicbedrock/models/mistral.py
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.242087 basicbedrock-0.2.1/src/basicbedrock.egg-info/
--rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-11 00:13:56.000000 basicbedrock-0.2.1/src/basicbedrock.egg-info/PKG-INFO
--rw-r--r--   0 dmattsn    (504) staff       (20)      672 2024-05-11 00:13:56.000000 basicbedrock-0.2.1/src/basicbedrock.egg-info/SOURCES.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-05-11 00:13:56.000000 basicbedrock-0.2.1/src/basicbedrock.egg-info/dependency_links.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-05-11 00:13:56.000000 basicbedrock-0.2.1/src/basicbedrock.egg-info/requires.txt
--rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-05-11 00:13:56.000000 basicbedrock-0.2.1/src/basicbedrock.egg-info/top_level.txt
-drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-11 00:13:56.240727 basicbedrock-0.2.1/test/
--rw-r--r--   0 dmattsn    (504) staff       (20)     6682 2024-05-10 19:43:58.000000 basicbedrock-0.2.1/test/test_basicbedrock.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.392025 basicbedrock-0.2.2/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1048 2024-04-07 21:53:42.000000 basicbedrock-0.2.2/LICENSE
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-13 21:26:57.391649 basicbedrock-0.2.2/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)     1978 2024-04-11 00:27:04.000000 basicbedrock-0.2.2/README.md
+-rw-r--r--   0 dmattsn    (504) staff       (20)      811 2024-05-13 21:26:28.000000 basicbedrock-0.2.2/pyproject.toml
+-rw-r--r--   0 dmattsn    (504) staff       (20)       38 2024-05-13 21:26:57.392092 basicbedrock-0.2.2/setup.cfg
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.386222 basicbedrock-0.2.2/src/
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.387718 basicbedrock-0.2.2/src/basicbedrock/
+-rw-r--r--   0 dmattsn    (504) staff       (20)      330 2024-05-13 21:26:28.000000 basicbedrock-0.2.2/src/basicbedrock/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    19081 2024-05-11 00:13:29.000000 basicbedrock-0.2.2/src/basicbedrock/basicbedrock.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)    10079 2024-05-10 19:42:41.000000 basicbedrock-0.2.2/src/basicbedrock/guardrails.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     7632 2024-05-02 02:20:16.000000 basicbedrock-0.2.2/src/basicbedrock/guardrails_baseclasses.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.390613 basicbedrock-0.2.2/src/basicbedrock/models/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     6907 2024-05-13 20:47:03.000000 basicbedrock-0.2.2/src/basicbedrock/models/__init__.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2960 2024-05-13 15:27:33.000000 basicbedrock-0.2.2/src/basicbedrock/models/ai21.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5979 2024-05-13 15:27:33.000000 basicbedrock-0.2.2/src/basicbedrock/models/amazon.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5213 2024-05-13 15:28:43.000000 basicbedrock-0.2.2/src/basicbedrock/models/anthropic.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     5477 2024-05-13 15:27:33.000000 basicbedrock-0.2.2/src/basicbedrock/models/baseclasses.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     4798 2024-05-13 20:47:03.000000 basicbedrock-0.2.2/src/basicbedrock/models/cohere.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3862 2024-05-13 15:27:33.000000 basicbedrock-0.2.2/src/basicbedrock/models/meta.py
+-rw-r--r--   0 dmattsn    (504) staff       (20)     2414 2024-05-13 15:27:33.000000 basicbedrock-0.2.2/src/basicbedrock/models/mistral.py
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.391317 basicbedrock-0.2.2/src/basicbedrock.egg-info/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     3875 2024-05-13 21:26:57.000000 basicbedrock-0.2.2/src/basicbedrock.egg-info/PKG-INFO
+-rw-r--r--   0 dmattsn    (504) staff       (20)      672 2024-05-13 21:26:57.000000 basicbedrock-0.2.2/src/basicbedrock.egg-info/SOURCES.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)        1 2024-05-13 21:26:57.000000 basicbedrock-0.2.2/src/basicbedrock.egg-info/dependency_links.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       31 2024-05-13 21:26:57.000000 basicbedrock-0.2.2/src/basicbedrock.egg-info/requires.txt
+-rw-r--r--   0 dmattsn    (504) staff       (20)       13 2024-05-13 21:26:57.000000 basicbedrock-0.2.2/src/basicbedrock.egg-info/top_level.txt
+drwxr-xr-x   0 dmattsn    (504) staff       (20)        0 2024-05-13 21:26:57.390816 basicbedrock-0.2.2/test/
+-rw-r--r--   0 dmattsn    (504) staff       (20)     7365 2024-05-13 20:53:16.000000 basicbedrock-0.2.2/test/test_basicbedrock.py
```

### Comparing `basicbedrock-0.2.1/LICENSE` & `basicbedrock-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/PKG-INFO` & `basicbedrock-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.2.1
+Version: 0.2.2
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.2.1/README.md` & `basicbedrock-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/pyproject.toml` & `basicbedrock-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "basicbedrock"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 maintainers = [
     { name="cyberitech", email="mattsod@kaizencyber.io" },
 ]
 description = "An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas."
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/basicbedrock.py` & `basicbedrock-0.2.2/src/basicbedrock/basicbedrock.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/src/basicbedrock/guardrails.py` & `basicbedrock-0.2.2/src/basicbedrock/guardrails.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/src/basicbedrock/guardrails_baseclasses.py` & `basicbedrock-0.2.2/src/basicbedrock/guardrails_baseclasses.py`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/__init__.py` & `basicbedrock-0.2.2/src/basicbedrock/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseRequest,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseRequest,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0":AnthropicClaude3BaseRequest,
     "cohere.command-text-v14": CohereCommandTextBaseRequest,
     "cohere.command-light-text-v14": CohereCommandTextBaseRequest,
     "cohere.embed-english-v3": CohereEmbedBaseRequest,
     "cohere.embed-multilingual-v3": CohereEmbedBaseRequest,
+    "cohere.command-r-v1:0": CohereCommandRPLUSTextBaseRequest,
+    "cohere.command-r-plus-v1:0": CohereCommandRPLUSTextBaseRequest,
     "meta.llama2-13b-chat-v1": MetaLlamaV2BaseRequest,
     "meta.llama2-70b-chat-v1": MetaLlamaV2BaseRequest,
     "meta.llama3-8b-instruct-v1:0": MetaLlamaV3BaseRequest,
     "meta.llama3-70b-instruct-v1:0": MetaLlamaV3BaseRequest,
     "mistral.mistral-7b-instruct-v0:2": Mistral7BInstructRequest,
     "mistral.mixtral-8x7b-instruct-v0:1": Mistral8X7BInstructRequest,
     "mistral.mistral-large-2402-v1:0": MistralLargeRequest
@@ -50,14 +52,16 @@
     "anthropic.claude-3-sonnet-20240229-v1:0": AnthropicClaude3BaseResponse,
     "anthropic.claude-3-haiku-20240307-v1:0": AnthropicClaude3BaseResponse,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0": AnthropicClaude3BaseResponse,
     "cohere.command-text-v14": CohereCommandTextBaseResponse,
     "cohere.command-light-text-v14": CohereCommandTextBaseResponse,
     "cohere.embed-english-v3": CohereEmbedBaseResponse,
     "cohere.embed-multilingual-v3": CohereEmbedBaseResponse,
+    "cohere.command-r-v1:0": CohereCommandRPLUSTextBaseResponse,
+    "cohere.command-r-plus-v1:0": CohereCommandRPLUSTextBaseResponse,
     "meta.llama2-13b-chat-v1": MetaLlamaV2V3BaseResponse,
     "meta.llama2-70b-chat-v1": MetaLlamaV2V3BaseResponse,
     "meta.llama3-8b-instruct-v1:0": MetaLlamaV2V3BaseResponse,
     "meta.llama3-70b-instruct-v1:0":MetaLlamaV2V3BaseResponse,
     "mistral.mistral-7b-instruct-v0:2": MistralBaseResponse,
     "mistral.mixtral-8x7b-instruct-v0:1": MistralBaseResponse,
     "mistral.mistral-large-2402-v1:0": MistralBaseResponse
@@ -76,14 +80,16 @@
     "anthropic.claude-3-sonnet-20240229-v1:0": anthropic.ANTHROPIC_CLAUDE_V3_CONTEXT_WINDOW,
     "anthropic.claude-3-haiku-20240307-v1:0": anthropic.ANTHROPIC_CLAUDE_V3_CONTEXT_WINDOW,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0":AnthropicClaude3BaseRequest,
     "cohere.command-text-v14": cohere.COHERE_COMMAND_TEXT_CONTEXT_WINDOW,
     "cohere.command-light-text-v14": cohere.COHERE_COMMAND_TEXT_CONTEXT_WINDOW,
     "cohere.embed-english-v3": None,
     "cohere.embed-multilingual-v3": None,
+    "cohere.command-r-v1:0": COHERE_COMMAND_R_RPLUS_CONTEXT_WINDOW,
+    "cohere.command-r-plus-v1:0": COHERE_COMMAND_R_RPLUS_CONTEXT_WINDOW,
     "meta.llama2-13b-chat-v1": meta.META_LLAMA_V2_CONTEXT_WINDOW,
     "meta.llama2-70b-chat-v1": meta.META_LLAMA_V2_CONTEXT_WINDOW,
     "meta.llama3-8b-instruct-v1:0": meta.META_LLAMA_V3_CONTEXT_WINDOW,
     "meta.llama3-70b-instruct-v1:0": meta.META_LLAMA_V3_CONTEXT_WINDOW,
     "mistral.mistral-7b-instruct-v0:2": mistral.MISTRAL_CONTEXT_WINDOW,
     "mistral.mixtral-8x7b-instruct-v0:1": mistral.MISTRAL_CONTEXT_WINDOW,
     "mistral.mistral-large-2402-v1:0": mistral.MISTRAL_CONTEXT_WINDOW
@@ -99,14 +105,16 @@
     "anthropic.claude-v2": anthropic.ANTHROPIC_CLAUDE_MAX_OUTPUT,
     "anthropic.claude-v2:1": anthropic.ANTHROPIC_CLAUDE_MAX_OUTPUT,
     "anthropic.claude-3-sonnet-20240229-v1:0": anthropic.ANTHROPIC_CLAUDE_MAX_OUTPUT,
     "anthropic.claude-3-haiku-20240307-v1:0": anthropic.ANTHROPIC_CLAUDE_MAX_OUTPUT,
     #  unavailable "anthropic.claude-3-opus-20240229-v1:0":AnthropicClaude3BaseRequest,
     "cohere.command-text-v14": cohere.COHERE_COMMAND_TEXT_MAX_OUTPUT,
     "cohere.command-light-text-v14": cohere.COHERE_COMMAND_TEXT_MAX_OUTPUT,
+    "cohere.command-r-v1:0": COHERE_COMMAND_TEXT_MAX_OUTPUT,
+    "cohere.command-r-plus-v1:0": COHERE_COMMAND_TEXT_MAX_OUTPUT,
     "cohere.embed-english-v3": None,
     "cohere.embed-multilingual-v3": None,
     "meta.llama2-13b-chat-v1": meta.META_LLAMA_V2V3_MAX_OUTPUT,
     "meta.llama2-70b-chat-v1": meta.META_LLAMA_V2V3_MAX_OUTPUT,
     "meta.llama3-8b-instruct-v1:0": meta.META_LLAMA_V2V3_MAX_OUTPUT,
     "meta.llama3-70b-instruct-v1:0": meta.META_LLAMA_V2V3_MAX_OUTPUT,
     "mistral.mistral-7b-instruct-v0:2": mistral.MISTRAL_7B_INSTRUCT_MAX_OUTPUT,
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/ai21.py` & `basicbedrock-0.2.2/src/basicbedrock/models/ai21.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,32 @@
 from pydantic import BaseModel
 
 from .baseclasses import BaseAbstractRequest, BaseAbstractResponse
 
 AI21_JURASSIC2_CONTEXT_WINDOW = 8_000
 AI21_JURASSIC2_MAX_OUTPUT = 8_191
 
+
 class AI21Jurassic2BaseRequest(BaseAbstractRequest):
     """
     AI21 Jurassic 2 request format.
     This model supports max_token, temperature and top_p, stop_sequences, count_penalty, presence_penalty and frequncy_penalty
     it does not support top_k
     as of right now there is no BasicBedrock support for penalty parameters
     """
+
     prompt: str = "{PROMPT}"
     maxTokens: int = 250
     temperature: float = 0.5
     topP: float = 0.5
     stopSequences: List = []
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         """
         Update the prompt based on the input text.
         inserts text according to expected request conventions.
         :param text:
         :return:
         """
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/amazon.py` & `basicbedrock-0.2.2/src/basicbedrock/models/amazon.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,26 +99,32 @@
         input_text = input_text.format(PROMPT=text)
         input_text = input_text[:AMAZON_TITAN_G1_LITE_CONTEXT_WINDOW]
         self.set_prompt_raw(input_text)
 
     def set_prompt_raw(self, text):
         self.inputText = text
 
+    def get_prompt(self) -> str:
+        return self.inputText
+
 
 class AmazonTitanTextG1ExpressRequest(AmazonTitanTextV1Request):
 
     def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
         input_text = input_text[:AMAZON_TITAN_G1_EXPRESS_CONTEXT_WINDOW]
         self.set_prompt_raw(input_text)
 
     def set_prompt_raw(self, text):
         self.inputText = text
 
+    def get_prompt(self) -> str:
+        return self.inputText
+
 
 class AmazonTitanTextV1Response(BaseAbstractResponse):
     """
     Response structure for Amazon Titan Text V1 API both Express and Lite
     """
 
     def get_answer(self) -> List[float]:
@@ -128,14 +134,17 @@
 class AmazonTitanEmbedTextV1Request(BaseAbstractRequest):
     """
     Request structure for Amazon Titan Embedding V1 API
     This model accepts text and returns a list of floats, representing Amazon Titan embedding vectors.
     """
     inputText: str = "{PROMPT}"
 
+    def get_prompt(self) -> str:
+        return self.inputText
+
     def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
         self.set_prompt_raw(input_text)
 
     def set_prompt_raw(self, text):
         self.inputText = text
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/anthropic.py` & `basicbedrock-0.2.2/src/basicbedrock/models/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     max_tokens_to_sample: int = 250
     temperature: float = 0.5
     top_k: int = 125
     top_p: float = 0.5
     stop_sequences: list = ["\n\nHuman:"]
     anthropic_version: str = "bedrock-2023-05-31"
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         prompt = "\n\nHuman: {PROMPT}\n\nAssistant:"
         padding = len(prompt.replace("{PROMPT}",""))
         cut_text = text[:ANTHROPIC_CLAUDE_V1V2_CONTEXT_WINDOW-padding]
         prompt = prompt.format(PROMPT=cut_text)
         self.set_prompt_raw(prompt)
 
@@ -113,14 +116,17 @@
     top_p: float = 1.
     top_k: int = 25
     temperature: float = 0.5
     messages: List[AntropicClaude3Message] = [AntropicClaude3Message()]
     anthropic_version: str = "bedrock-2023-05-31"
     stop_sequences: List[str] = []
 
+    def get_prompt(self) -> str:
+        return self.messages[0].content[0].text
+
     def set_prompt(self, text):
         self.messages[0].update_prompt(text)
 
     def set_prompt_raw(self, text):
         self.messages[0].update_prompt_raw(text)
 
     def set_stop_words(self, stop_sequences: List[str]):
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/baseclasses.py` & `basicbedrock-0.2.2/src/basicbedrock/models/baseclasses.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,51 +21,58 @@
     temp: float = None
     max_tokens: int = None
     stop_words: typing.List[str] = []
 
 
 class BaseAbstractRequest(BaseModel, extra='forbid'):
     """
-    Abstract base class for all model requests. All model requests must inherit this class.
+    Abstract base class for all model requests. All model requests must inherit this class.\n
     update_prompt and update_promp_raw differ in the fact that some models expect a certain request format to work properly,
     eg, in certain cases boto3 may reject the request if the prompt does not begin with "Human:"\
     update_prompt will format all prompts as expected by the model, whereas update_prompt_raw will input text without formatting.
-    The other abstract methods all deal with setting hyperparam values P, K, temp, and max tokens.
-    Additionally, two non abstract methods allow the caller to return the request as a dict or json.
+    The other abstract methods all deal with setting hyperparam values P, K, temp, and max tokens.\n
+    Additionally, two non abstract methods allow the caller to return the request as a dict or json.\n
     """
 
     @abc.abstractmethod
     def set_prompt(self, text: str):
         """
-        Updates the prompt while maintaining its expected internal prompt structure
-        Example, if the prompt must begin with 'Human:' this will be maintained
+        Updates the prompt while maintaining its expected internal prompt structure\n
+        Example, if the prompt must begin with 'Human:' this will be maintained\n
         :param text: the prompt you want to use
         :return:
         """
         raise NotImplementedError("Abstract method update_prompt not implemented")
 
     @abc.abstractmethod
     def set_prompt_raw(self, text: str):
         """
-        Updates the prompt without regards to any expected prompt structure.
-        this is used for very precisely modifying prompts.
+        Updates the prompt without regards to any expected prompt structure.\n
+        this is used for very precisely modifying prompts.\n
         :param text: the exact prompt you want to use
         :return:
         """
         raise NotImplementedError("Abstract method update_prompt_raw not implemented")
 
     @abc.abstractmethod
     def set_stop_words(self, stop_words: typing.List[str]):
         """
-        Sets the stop words used in the model.
-        If the model does not support stop words, this is ignored
+        Sets the stop words used in the model.\n
+        If the model does not support stop words, this is ignored\n
         :param stop_words: the list of strings
         :return:
         """
 
+    @abc.abstractmethod
+    def get_prompt(self) -> str:
+        """
+        This retrieves only the current prompt from the model request structure.
+        :return: a str containing the extracted prompt
+        """
+
     def get_dict(self):
         j = json.loads(self.json())
         return j
 
     def get_json(self, indent: int = None):
         if not indent:
             return self.json()
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/cohere.py` & `basicbedrock-0.2.2/src/basicbedrock/models/cohere.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     prompt: str = "{PROMPT}"
     max_tokens: int = 250
     temperature: float = 0.5
     p: float = 0.5
     k: int = 125
     stop_sequences: List[str] = []
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
         input_text = input_text[:COHERE_COMMAND_TEXT_CONTEXT_WINDOW]
         self.set_prompt_raw(input_text)
 
     def set_prompt_raw(self, text):
@@ -74,14 +77,17 @@
     """
     All cohere command models use the same request format.
     Models support input text only.
     """
     texts: List[str] = ["{PROMPT}"]
     input_type: str = "search_document"
 
+    def get_prompt(self) -> str:
+        return self.texts[0]
+
     def set_prompt(self, text):
         input_text = "{PROMPT}"
         input_text = input_text.format(PROMPT=text)
         texts = [input_text]
         self.set_prompt_raw(texts)
 
     def set_prompt_raw(self, texts: list):
@@ -126,7 +132,53 @@
 class CohereEmbedBaseResponse(BaseAbstractResponse):
     """
     All Cohere Embed models use the same response format.
     """
 
     def get_answer(self) -> List[float]:
         return self.result_raw['embeddings'][0]
+
+
+class CohereCommandRPLUSTextBaseRequest(BaseAbstractRequest):
+
+    message: str = "{PROMPT}"
+    max_tokens: int = 250
+    temperature: float = 0.5
+    p: float = 0.5
+    k: int = 125
+    stop_sequences: List[str] = []
+
+    def set_prompt(self, text: str):
+        input_text = "{PROMPT}"
+        input_text = input_text.format(PROMPT=text)
+        input_text = input_text[:COHERE_COMMAND_R_RPLUS_CONTEXT_WINDOW]
+        self.set_prompt_raw(input_text)
+
+    def set_prompt_raw(self, text: str):
+        self.message = text
+
+    def set_stop_words(self, stop_words: typing.List[str]):
+        self.stop_sequences = stop_words
+
+    def get_prompt(self) -> str:
+        return self.message
+
+    def set_p(self, top_p: float):
+        self.p = top_p
+
+    def set_k(self, top_k: int):
+        self.k=top_k
+
+    def set_temp(self, temp: float):
+        self.temperature = temp
+
+    def set_max_tokens(self, max_tokens: int):
+        self.max_tokens = min(max_tokens, COHERE_COMMAND_TEXT_MAX_OUTPUT)
+
+
+class CohereCommandRPLUSTextBaseResponse(BaseAbstractResponse):
+    """
+    this is the base response format used by all text-family cohere models
+    """
+
+    def get_answer(self) -> str:
+        return self.result_raw['text']
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/meta.py` & `basicbedrock-0.2.2/src/basicbedrock/models/meta.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     It does not support top_k
     """
 
     max_gen_len: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
 
+    def get_prompt(self) -> str:
+        pass
 
     def set_stop_words(self, stop_words: typing.List[str]):
         """
         Meta Llama 2 models dont support stop words
         :param stop_words:
         :return:
         """
@@ -81,41 +83,47 @@
 
 class MetaLlamaV2BaseRequest(MetaLlamaBaseRequest):
     """
     Specifies the expected Llama 2 V1 family chat request format using the [INST] tags
     """
     prompt: str = "<s>[INST]{PROMPT}[/INST]"
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         prompt = "<s>[INST]{PROMPT}[/INST]"
         padding = len(prompt.replace("{PROMPT}",""))
         cut_text = text[:META_LLAMA_V2_CONTEXT_WINDOW-padding]
         prompt = prompt.format(PROMPT=cut_text)
         self.set_prompt_raw(prompt)
 
-
     def set_prompt_raw(self, text):
         """
         Update the prompt based on the input text without regards to expected input format
         what you insert, is inserted raw without formatting
         :param text:
         :return:
         """
         self.prompt = text
 
+
 class MetaLlamaV3BaseRequest(MetaLlamaBaseRequest):
     """
     Specifies the expected Llama 2 V1 family chat request format using the expected header format
     """
     prompt: str = (
         '<|begin_of_text|><|start_header_id|>user<|end_header_id|>\n'
         '\n'
         '{PROMPT}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n'
     )
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         prompt = str(
             "<|begin_of_text|><|start_header_id|>user<|end_header_id|>\n"
             "\n"
             "{PROMPT}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n"
         )
         padding = len(prompt.replace("{PROMPT}",""))
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock/models/mistral.py` & `basicbedrock-0.2.2/src/basicbedrock/models/mistral.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     prompt: str = "<s>[INST] {PROMPT} [/INST]"
     max_tokens: int = 250
     temperature: float = 0.5
     top_p: float = 0.5
     top_k: int = 125
     stop: typing.List[str] = []
 
+    def get_prompt(self) -> str:
+        return self.prompt
+
     def set_prompt(self, text):
         prompt = "<s>[INST] {PROMPT} [/INST]"
         padding = len(prompt.replace("{PROMPT}",""))
         cut_text = text[:MISTRAL_CONTEXT_WINDOW-padding]
         prompt = prompt.format(PROMPT=cut_text)
         self.set_prompt_raw(prompt)
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock.egg-info/PKG-INFO` & `basicbedrock-0.2.2/src/basicbedrock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: basicbedrock
-Version: 0.2.1
+Version: 0.2.2
 Summary: An abstraction layer for AWS Bedrock.  Removes the need to keep track of response/request schemas.
 Author-email: cyberitech <mattsod@kaizencyber.io>
 Maintainer-email: cyberitech <mattsod@kaizencyber.io>
 License: Copyright 2024 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `basicbedrock-0.2.1/src/basicbedrock.egg-info/SOURCES.txt` & `basicbedrock-0.2.2/src/basicbedrock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `basicbedrock-0.2.1/test/test_basicbedrock.py` & `basicbedrock-0.2.2/test/test_basicbedrock.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 from random import choice
 import json
 import boto3
 
 from basicbedrock import *
 
 
-def test_content_policy():
+def test_content_policy(bb: BasicBedrock, verbose=False):
     gr = Guardrails()
     gr.add_content_filter("SEXUAL","HIGH","HIGH")
     gr.install_guardrails()
     model = choice([model for model in bb.get_available_models() if "embed" not in model])
     r = bb.invoke(model,"write a lewd story",guardrail=gr)
-    print(r.get_answer())
+    if verbose: print(r.get_answer())
     gr.uninstall_guardrails()
 
 
-def test_filter_policy(bb: BasicBedrock):
+def test_filter_policy(bb: BasicBedrock, verbose=False):
     gr = Guardrails()
     gr.add_topic_filter(definition="Conversation related to politics", examples=[
         "Jane Doe is a great president!",
         "Randy Randolph is the better presidential candidate ",
         "the House of Lords and the House of Commons ",
         "This election season will be a great match up between political parties"
     ])
     gr.install_guardrails()
     model = choice([model for model in bb.get_available_models() if "embed" not in model])
     r = bb.invoke(model, "I am going to vote for in this year's elections", guardrail=gr)
-    print(r.get_answer())
+    if verbose: print(r.get_answer())
     gr.uninstall_guardrails()
 
 
-def test_no_guardrail(bb: BasicBedrock):
+def test_no_guardrail(bb: BasicBedrock, verbose=False):
     bb = BasicBedrock()
     model = choice([model for model in bb.get_available_models() if "embed" not in model])
     r = bb.invoke(model, "simple test", guardrail=None)
-    print(r.get_answer())
+    if verbose: print(r.get_answer())
 
 
-def test_invoke_with_string(bb, verbose=False):
+def test_invoke_with_string(bb:BasicBedrock, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with string")
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
-            print(r.get_answer_raw())
+            print(r.get_answer())
         print(f"done testing {model} in invoke with string")
 
 
-def test_invoke_with_invalid_json_blob(bb, verbose=False):
+def test_invoke_with_invalid_json_blob(bb:BasicBedrock, verbose=False):
     prompt = "{\"status\":\"invalid\"}"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with invalid json blob")
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
-            print(r.get_answer_raw())
+            print(r.get_answer())
         print(f"done testing {model} in invoke with invalid json blob")
 
 
-def test_invoke_with_valid_json_blob(bb, verbose=False):
+def test_invoke_with_valid_json_blob(bb:BasicBedrock, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid json blob")
         schema_inst = bb.get_model_request_object(model)
         schema_inst.set_prompt(prompt)
         blob = schema_inst.json()
         r = bb.invoke(model, blob, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid json blob")
 
 
-def test_invoke_with_valid_dict(bb, verbose=False):
+def test_invoke_with_valid_dict(bb:BasicBedrock, verbose=False):
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model in all_models:
         print(f"now testing {model} in invoke with valid dict")
         schema_inst = bb.get_model_request_object(model)
         schema_inst.set_prompt(prompt)
         j = schema_inst.json()
         d = json.loads(j)
         r = bb.invoke(model, d, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
         print(f"done testing {model} in invoke with valid dict")
 
 
-def test_invoke_with_invalid_dict(bb, verbose=False):
+def test_invoke_with_invalid_dict(bb:BasicBedrock, verbose=False):
     all_models = bb.get_available_models()
     d = {"status": "invalid"}
     for model in all_models:
         print(f"now testing {model} in invoke with invalid dict")
         try:
             r = bb.invoke(model, d, show_request=verbose)
         except ValueError:
             pass  # we expect this, it should fail in this case
         if verbose:
             print(f"could not call model {model} in invoke with dict {d} (Ok)")
         print(f"done testing {model} in invoke with dict")
 
 
-def test_get_boto3_body(bb,sess:boto3.session.Session, verbose=False):
+def test_get_boto3_body(bb:BasicBedrock,sess:boto3.session.Session, verbose=False):
     client = sess.client("bedrock-runtime")
     prompt = "tell me about foobar"
     all_models = bb.get_available_models()
     for model_id in all_models:
         print(f"now testing {model_id} invoke boto3 invoke_model() directly using get_boto3_body")
         body = bb.get_boto3_body(model_id, prompt)
         full_request = {
@@ -116,65 +116,78 @@
         if verbose:
             print(f"boto3 request: {full_request}")
         r = client.invoke_model(**full_request)
         assert (r['ResponseMetadata']['HTTPStatusCode'] == 200)
         print(f"done testing {model_id} invoke boto3 invoke_model() directly using get_boto3_body")
 
 
-def single_run(bb, verbose=False):
+def single_run(bb:BasicBedrock, verbose=False):
     prompt = "tell me about foobar"
-    bb.invoke("ai21.j2-mid-v1", prompt)
+    r=bb.invoke("cohere.command-r-v1:0", prompt)
+    if verbose: print(r.get_answer())
 
 
-def test_set_params(bb, verbose=True):
+def test_set_params(bb:BasicBedrock, verbose=True):
     params = bb.params
     params["max_tokens"] = 88
     params["top_p"] = 0.88
     params["top_k"] = 88
     params["temp"] = .88
     params["stop_words"] = ["User:", "foobar"]
     bb.set_params(params)
     prompt = "Hittem hard with dem params doe"
     for model in bb.get_available_models():
         r = bb.invoke(model, prompt, show_request=verbose)
         if verbose:
             print(r.get_answer_raw())
 
 
-def test_context_window_limits(bb, verbose=False):
+def test_context_window_limits(bb:BasicBedrock, verbose=False):
     for model_id,ctxt in model_request_context_windows.items():
         if not ctxt:  # embeds have no max
             continue
         print(f"now testing {model_id} test_context_window_limits")
         prompt = "My name is the real slim shady" * ctxt
         r = bb.invoke(model_id, prompt, show_request=verbose)
 
 
-def test_max_tokens(bb, verbose=False):
+def test_max_tokens(bb:BasicBedrock, verbose=False):
     for model_id,max_token in model_request_max_outputs.items():
         if not max_token:  # embeds have no max
             continue
         print(f"now testing {model_id} test_max_tokens")
         params = {
             "max_tokens": max_token,
         }
         print(params)
         prompt = "this is a test"
         bb.params = params
         r = bb.invoke(model_id, prompt, show_request=verbose)
 
 
+def test_get_prompts(bb:BasicBedrock, verbose=True):
+    prompt = "test of the prompt retreival"
+    for model in bb.get_available_models():
+        req_obj = bb.get_model_request_object(model)
+        req_obj.set_prompt(prompt)
+        output = req_obj.get_prompt()
+        if verbose:
+            print(model)
+            print(json.dumps(output))
+
+
 if __name__ == "__main__":
-    verbose = False
+    verbose = True
     session = boto3.session.Session(profile_name='default')
     bb = BasicBedrock(session=session)
     single_run(bb, verbose)
-    test_no_guardrail()
-    test_content_policy()
-    test_filter_policy()
+    test_get_prompts(bb,verbose)
+    test_no_guardrail(bb, verbose)
+    test_content_policy(bb, verbose)
+    test_filter_policy(bb, verbose)
     test_invoke_with_string(bb, verbose=verbose)
     test_get_boto3_body(bb, sess=session, verbose=verbose)
     test_set_params(bb, verbose=verbose)
     test_invoke_with_invalid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_json_blob(bb, verbose=verbose)
     test_invoke_with_valid_dict(bb, verbose=verbose)
     test_invoke_with_invalid_dict(bb, verbose=verbose)
```

