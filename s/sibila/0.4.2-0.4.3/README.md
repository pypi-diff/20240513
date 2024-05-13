# Comparing `tmp/sibila-0.4.2.tar.gz` & `tmp/sibila-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sibila-0.4.2.tar", last modified: Sat May  4 18:37:55 2024, max compression
+gzip compressed data, was "sibila-0.4.3.tar", last modified: Mon May 13 15:02:48 2024, max compression
```

## Comparing `sibila-0.4.2.tar` & `sibila-0.4.3.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.2/LICENSE
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-05-04 18:37:55.353221 sibila-0.4.2/PKG-INFO
--rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3487 2024-04-29 17:34:57.000000 sibila-0.4.2/README.md
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1629 2024-05-04 10:29:39.000000 sibila-0.4.2/pyproject.toml
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-05-04 18:37:55.353221 sibila-0.4.2/setup.cfg
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.349221 sibila-0.4.2/sibila/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1312 2024-05-04 10:16:01.000000 sibila-0.4.2/sibila/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14965 2024-05-01 14:34:46.000000 sibila-0.4.2/sibila/anthropic.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.2/sibila/cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.2/sibila/context.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    10272 2024-04-27 10:05:28.000000 sibila-0.4.2/sibila/gen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.2/sibila/json_grammar.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    24981 2024-04-27 09:42:38.000000 sibila-0.4.2/sibila/json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    23826 2024-05-01 14:34:53.000000 sibila-0.4.2/sibila/llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    16238 2024-05-01 14:34:55.000000 sibila-0.4.2/sibila/mistral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    74668 2024-05-04 17:30:39.000000 sibila-0.4.2/sibila/model.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    48077 2024-05-01 10:56:43.000000 sibila-0.4.2/sibila/models.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.2/sibila/multigen.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2489 2024-04-29 14:30:36.000000 sibila-0.4.2/sibila/null.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    21545 2024-05-01 14:35:09.000000 sibila-0.4.2/sibila/openai.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.349221 sibila-0.4.2/sibila/res/
--rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.2/sibila/res/__init__.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14777 2024-04-27 19:34:06.000000 sibila-0.4.2/sibila/res/base_formats.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1996 2024-05-04 17:37:24.000000 sibila-0.4.2/sibila/res/base_models.json
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    15043 2024-05-01 14:35:37.000000 sibila-0.4.2/sibila/schema_format_openai.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.2/sibila/text_splitter.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20235 2024-04-26 15:07:47.000000 sibila-0.4.2/sibila/thread.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.2/sibila/tools.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1245 2024-04-29 15:26:33.000000 sibila-0.4.2/sibila/utils.py
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/sibila.egg-info/
--rw-r--r--   0 jorge     (1000) jorge     (1000)     4746 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/PKG-INFO
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1167 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/SOURCES.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/dependency_links.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/entry_points.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)      144 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/requires.txt
--rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-05-04 18:37:55.000000 sibila-0.4.2/sibila.egg-info/top_level.txt
-drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-04 18:37:55.353221 sibila-0.4.2/tests/
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4037 2024-04-29 16:15:42.000000 sibila-0.4.2/tests/test_anthropic_claude-3-haiku.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    11685 2024-04-29 16:05:39.000000 sibila-0.4.2/tests/test_cli.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4515 2024-04-29 16:05:46.000000 sibila-0.4.2/tests/test_common_llamacpp.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     8266 2024-04-29 15:07:11.000000 sibila-0.4.2/tests/test_common_llamacpp_examples.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     3780 2024-04-27 19:04:48.000000 sibila-0.4.2/tests/test_common_remote.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     7624 2024-04-27 20:12:25.000000 sibila-0.4.2/tests/test_common_remote_examples.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    20543 2024-04-26 18:26:18.000000 sibila-0.4.2/tests/test_examples_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4369 2024-04-26 10:26:46.000000 sibila-0.4.2/tests/test_fireworks_mixtral.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.2/tests/test_formats.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)    14927 2024-02-29 16:31:57.000000 sibila-0.4.2/tests/test_json_schema.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     1664 2024-04-27 17:53:16.000000 sibila-0.4.2/tests/test_llamacpp_models_dir.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     7957 2024-04-26 10:32:15.000000 sibila-0.4.2/tests/test_llamacpp_tinyllama.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4090 2024-04-26 10:27:01.000000 sibila-0.4.2/tests/test_mixtral_mistral_small.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4613 2024-04-04 18:27:52.000000 sibila-0.4.2/tests/test_null_extract.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4099 2024-04-29 16:16:00.000000 sibila-0.4.2/tests/test_openai_gpt35.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4086 2024-04-29 16:15:54.000000 sibila-0.4.2/tests/test_openai_gpt4.py
--rw-rw-r--   0 jorge     (1000) jorge     (1000)     4338 2024-04-26 10:27:29.000000 sibila-0.4.2/tests/test_together_mixtral.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-13 15:02:48.248113 sibila-0.4.3/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1078 2024-01-30 10:27:20.000000 sibila-0.4.3/LICENSE
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4758 2024-05-13 15:02:48.248113 sibila-0.4.3/PKG-INFO
+-rwxrwxr-x   0 jorge     (1000) jorge     (1000)     3499 2024-05-13 14:50:16.000000 sibila-0.4.3/README.md
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1629 2024-05-04 10:29:39.000000 sibila-0.4.3/pyproject.toml
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       38 2024-05-13 15:02:48.248113 sibila-0.4.3/setup.cfg
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-13 15:02:48.244113 sibila-0.4.3/sibila/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)     1346 2024-05-13 10:04:39.000000 sibila-0.4.3/sibila/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14965 2024-05-01 14:34:46.000000 sibila-0.4.3/sibila/anthropic.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    29858 2024-03-09 11:56:55.000000 sibila-0.4.3/sibila/cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     5366 2024-03-13 19:10:42.000000 sibila-0.4.3/sibila/context.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    10272 2024-04-27 10:05:28.000000 sibila-0.4.3/sibila/gen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8577 2024-03-06 10:11:40.000000 sibila-0.4.3/sibila/json_grammar.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    26021 2024-05-13 14:53:41.000000 sibila-0.4.3/sibila/json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    23826 2024-05-01 14:34:53.000000 sibila-0.4.3/sibila/llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    16238 2024-05-01 14:34:55.000000 sibila-0.4.3/sibila/mistral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    74668 2024-05-13 09:02:04.000000 sibila-0.4.3/sibila/model.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    48300 2024-05-13 10:10:45.000000 sibila-0.4.3/sibila/models.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    17408 2024-02-29 10:46:02.000000 sibila-0.4.3/sibila/multigen.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2489 2024-04-29 14:30:36.000000 sibila-0.4.3/sibila/null.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    21545 2024-05-01 14:35:09.000000 sibila-0.4.3/sibila/openai.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-13 15:02:48.244113 sibila-0.4.3/sibila/res/
+-rwxr-xr-x   0 jorge     (1000) jorge     (1000)        0 2024-03-07 18:25:20.000000 sibila-0.4.3/sibila/res/__init__.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14777 2024-04-27 19:34:06.000000 sibila-0.4.3/sibila/res/base_formats.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2098 2024-05-13 09:31:25.000000 sibila-0.4.3/sibila/res/base_models.json
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    22635 2024-05-13 10:51:15.000000 sibila-0.4.3/sibila/schema_format_openai.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4628 2024-02-26 20:11:39.000000 sibila-0.4.3/sibila/text_splitter.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20299 2024-05-13 14:52:23.000000 sibila-0.4.3/sibila/thread.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    13103 2024-04-08 14:37:15.000000 sibila-0.4.3/sibila/tools.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1245 2024-04-29 15:26:33.000000 sibila-0.4.3/sibila/utils.py
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-13 15:02:48.248113 sibila-0.4.3/sibila.egg-info/
+-rw-r--r--   0 jorge     (1000) jorge     (1000)     4758 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/PKG-INFO
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1200 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/SOURCES.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        1 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/dependency_links.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)       43 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/entry_points.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)      144 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/requires.txt
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)        7 2024-05-13 15:02:48.000000 sibila-0.4.3/sibila.egg-info/top_level.txt
+drwxrwxr-x   0 jorge     (1000) jorge     (1000)        0 2024-05-13 15:02:48.248113 sibila-0.4.3/tests/
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4037 2024-04-29 16:15:42.000000 sibila-0.4.3/tests/test_anthropic_claude-3-haiku.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    11685 2024-04-29 16:05:39.000000 sibila-0.4.3/tests/test_cli.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4511 2024-05-13 11:42:06.000000 sibila-0.4.3/tests/test_common_llamacpp.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     8266 2024-04-29 15:07:11.000000 sibila-0.4.3/tests/test_common_llamacpp_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     3795 2024-05-13 10:11:37.000000 sibila-0.4.3/tests/test_common_remote.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7588 2024-05-13 10:13:02.000000 sibila-0.4.3/tests/test_common_remote_examples.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    20543 2024-04-26 18:26:18.000000 sibila-0.4.3/tests/test_examples_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4369 2024-04-26 10:26:46.000000 sibila-0.4.3/tests/test_fireworks_mixtral.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     2347 2024-03-16 12:05:44.000000 sibila-0.4.3/tests/test_formats.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    14896 2024-05-10 16:13:39.000000 sibila-0.4.3/tests/test_json_schema.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     1664 2024-04-27 17:53:16.000000 sibila-0.4.3/tests/test_llamacpp_models_dir.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     7957 2024-04-26 10:32:15.000000 sibila-0.4.3/tests/test_llamacpp_tinyllama.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4090 2024-04-26 10:27:01.000000 sibila-0.4.3/tests/test_mixtral_mistral_small.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4623 2024-05-10 16:05:54.000000 sibila-0.4.3/tests/test_null_extract.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4099 2024-04-29 16:16:00.000000 sibila-0.4.3/tests/test_openai_gpt35.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4086 2024-04-29 16:15:54.000000 sibila-0.4.3/tests/test_openai_gpt4.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)    13016 2024-05-11 09:44:02.000000 sibila-0.4.3/tests/test_pydantic_dataclass.py
+-rw-rw-r--   0 jorge     (1000) jorge     (1000)     4338 2024-04-26 10:27:29.000000 sibila-0.4.3/tests/test_together_mixtral.py
```

### Comparing `sibila-0.4.2/LICENSE` & `sibila-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/PKG-INFO` & `sibila-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.2
+Version: 0.4.3
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -30,26 +30,28 @@
 Requires-Dist: pydantic>=2.0
 Requires-Dist: typing_extensions
 Requires-Dist: tqdm
 Requires-Dist: pytest-asyncio>=0.17
 
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
+Extract structured data from remote or local LLM models. Because predictable output is important for serious use of LLMs.
 
 - Query structured data into Pydantic objects, dataclasses or simple types.
 - Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
 - Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
 - Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
 
-No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+No matter how well you craft a prompt begging a model for the format you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
+
+
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
 
 class Info(BaseModel):
@@ -78,15 +80,15 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclasses. Also includes asynchronous access to remote models.
 
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
```

### Comparing `sibila-0.4.2/README.md` & `sibila-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
+Extract structured data from remote or local LLM models. Because predictable output is important for serious use of LLMs.
 
 - Query structured data into Pydantic objects, dataclasses or simple types.
 - Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
 - Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
 - Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
 
-No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+No matter how well you craft a prompt begging a model for the format you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
+
+
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
 
 class Info(BaseModel):
@@ -44,15 +46,15 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclasses. Also includes asynchronous access to remote models.
 
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
```

### Comparing `sibila-0.4.2/pyproject.toml` & `sibila-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/__init__.py` & `sibila-0.4.3/sibila/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Structured data from local or remote LLM models."""
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 __all__ = [
     "Models",
     "Model", "TextModel", "MessagesModel", "Tokenizer",
     "GenConf", "GenRes", "GenError", "GenOut",
     "AnthropicModel",
     "FireworksModel",
+    "GroqModel",
     "LlamaCppModel", "LlamaCppTokenizer",
     "MistralModel",
     "OpenAIModel", "OpenAITokenizer",
     "TogetherModel",
     "Thread", "MsgKind",
     "Context", "Trim",
     "JSchemaConf",
@@ -53,16 +54,17 @@
 
 from .openai import (
     OpenAIModel,
     OpenAITokenizer
 )
 
 from .schema_format_openai import (
-    TogetherModel,
-    FireworksModel
+    FireworksModel,
+    GroqModel,
+    TogetherModel
 )
 
 
 from .context import (
     Context,
     Trim
 )
```

### Comparing `sibila-0.4.2/sibila/anthropic.py` & `sibila-0.4.3/sibila/anthropic.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/cli.py` & `sibila-0.4.3/sibila/cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/context.py` & `sibila-0.4.3/sibila/context.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/gen.py` & `sibila-0.4.3/sibila/gen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/json_grammar.py` & `sibila-0.4.3/sibila/json_grammar.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/json_schema.py` & `sibila-0.4.3/sibila/json_schema.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """JSON Schema generator functions"""
 
 from typing import Any, Optional, Union, Literal, Annotated, get_origin, get_args
+from types import NoneType
 from enum import Enum
 
-from copy import copy
+from copy import copy, deepcopy
 
 import json
 
 import logging
 logger = logging.getLogger(__name__)
 
 from datetime import date, time, datetime
 
-from dataclasses import dataclass, is_dataclass, field, fields, MISSING
+from dataclasses import dataclass, is_dataclass, field, fields, asdict, MISSING
 
 from pydantic import BaseModel, TypeAdapter, ValidationError
 
 from .utils import (
     is_subclass_of,
     synth_desc
 )
@@ -124,14 +125,16 @@
                         DEB: bool = False) -> dict:
 
     """
     Massages JSON schema object to simplify as much as possible and remove all non-essential keys.
     Resolves $refs and eliminates definitions.
     """
    
+    sch = deepcopy(sch)
+
     # resolve $refs -> defs
     if schemaconf.resolve_refs:
         sch = json_schema_resolve_refs(sch)
         if DEB:
             from pprint import pprint
             print("resolved:")
             pprint(sch)
@@ -312,14 +315,16 @@
 
     - prim_type:
 
         - bool
         - int
         - float
         - str
+
+    - typing.Union
         
     - enums:
 
         - [1, 2, 3] or ["a","b"] - all items of the same prim_type
         - Literal['year', 'name'] - all items of the same prim_type
         - Enum, EnumInt, EnumStr, (Enum, int),... - all items of the same prim_type
 
@@ -344,33 +349,37 @@
 
     Args:
         type_: Type to be simplified, one of the above.
 
     Returns:
         Returns (type_, anno_desc, options) or (None,,) if not a supported type.
         options: optional keys
-        "str_format": str
-        "enum_list": []
+            "str_format": str
+            "enum_list": []
     """
 
     anno_desc = None
     options = {}
 
     if get_origin(type_) is Annotated:
         args = list(get_args(type_))
         type_ = args[0]
         if len(args) > 1:
             anno_desc = args[1]
 
 
     if (is_prim_type(type_) or
         is_dataclass(type_) or
-        is_subclass_of(type_, BaseModel)):
+        is_subclass_of(type_, BaseModel) or
+        get_origin(type_) is Union):
         ...
 
+    elif type_ is NoneType:
+        type_ = NoneType
+
     elif is_subclass_of(type_, datetime):
         type_ = str
         options["str_format"] = "date-time"
 
     elif is_subclass_of(type_, date):
         type_ = str
         options["str_format"] = "date"
@@ -489,52 +498,45 @@
 
 
 
 
 def build_type_json_schema(type_: Any, 
                            desc: Optional[str] = None,
                            options: dict = {},
-                           default: Optional[Any] = None) -> dict:
+                           default: Optional[Any] = MISSING) -> dict:
     """Render a JSON Schema specification for an accepted simple type.
 
     Args:
         type_: A type supported by get_type().
         desc: Optional description for field. Defaults to None, but if given, will override any Annotated type's description.
-        default: A default value for field. Defaults to {}.
-        format: A default value for strings. Defaults to None.
+        options: Type options for specifying enums, str_format. Defaults to {}.
+        default: A default value for field. Defaults to MISSING.
 
     Returns:
         A dict whose json.dumps() serialization is a valid JSON Schema specification for the given type_ arg.
     """
 
     out_type, anno_desc, options2 = get_type(type_)
     if out_type is None:
         raise TypeError(f"Unsupported type: '{type(type_)}'")
     
-    if desc is None:
-        desc = anno_desc
-
     if is_dataclass(out_type):
         out = build_dataclass_object_json_schema(out_type)
 
-        if desc is not None:
-            out["description"] = desc
-
     elif is_subclass_of(out_type, BaseModel):
         out = out_type.model_json_schema()
 
-        if desc is not None:
-            out["description"] = desc
+    elif get_origin(out_type) is Union:
+        args = list(get_args(out_type))
+        out_json = [build_type_json_schema(t) for t in args]
+        out = {"anyOf": out_json} 
 
-    else: # prim_type or enum
+    else: # prim_type or enum or NoneType
         out = {}
 
-        if desc:
-            out["description"] = desc
-
         enum_list = options.get("enum_list")
         if enum_list is None:
             enum_list = options2.get("enum_list")
         if enum_list is not None:
             out["enum"] = enum_list
 
         str_format = options.get("str_format")
@@ -544,74 +546,88 @@
             if out_type is not str:
                 raise TypeError("Arg str_format is only valid for str type.")
 
             out["format"] = str_format
 
         out["type"] = get_json_type(out_type)
 
-        if default is not None:
-            if not isinstance(default, out_type):
-                raise TypeError(f"Arg default is not of type {out_type}.")
-
-            out["default"] = default
+    desc = desc or anno_desc
+    if desc is not None:
+        out["description"] = str(desc) # ensure string
+
+    if default is not MISSING:
+        # @TODO: better checking for Union origin types, deal with Literals, for example
+        if (get_origin(out_type) is not Union and
+            not isinstance(default, out_type) and
+            not isinstance(default, dict)):
+            raise TypeError(f"Arg default is not of type {out_type} nor dict.")
+        
+        out["default"] = default
 
     return out
 
 
 
 def build_array_json_schema(item_type: Any,
                             item_desc: Optional[str] = None,
                             item_options: dict = {},
-                            list_desc: Optional[str] = None) -> dict:
+                            list_desc: Optional[str] = None,
+                            default: Optional[Any] = MISSING) -> dict:
     """Render a JSON Schema specification for an list/array.
 
     Args:
         item_type: Type for array items.
         item_desc: Optional description for an array item. Defaults to None, but if given, will override any Annotated type's description.
         item_options: Optional array item options. Defaults to {}.
         list_desc: Optional description for the entire array. Defaults to None.
+        default: Optional default value. Defaults to MISSING.
 
     Returns:
         A dict whose json.dumps() serialization is a valid JSON Schema specification for the given array.
     """
 
     items_repr = build_type_json_schema(item_type, 
                                         item_desc,
                                         options=item_options)
 
     out: dict[str,Any] = {}
 
     if list_desc:
-        out["description"] = list_desc
+        out["description"] = str(list_desc) # ensure string
 
     out["items"] = items_repr
 
     out["type"] = "array"
 
+    if default is not MISSING:
+        out["default"] = default
+
     return out
 
 
 
 
 
 
 
 
 def build_type_or_array_json_schema(type_: Any,
-                                    default: Optional[Any] = None) -> tuple[dict,bool]:
+                                    default: Optional[Any] = MISSING) -> tuple[dict,bool]:
     """Build a JSON schema for given simple type or array. See build_*() functions for details."""
 
     # type list
-    item_type, item_desc, item_options, list_desc = get_type_list(type_)    
+    item_type, item_desc, item_options, list_desc = get_type_list(type_)
+
     if item_type is not None:            
         # build json schema for list of type_
         schema = build_array_json_schema(item_type, 
                                          item_desc, 
                                          item_options,
-                                         list_desc)
+                                         list_desc,
+                                         default)
         is_object = False
 
     else: # prim, enum, datetime, dataclass, BaseModel
         out_type, desc, options = get_type(type_)
         if out_type is None:
             raise TypeError(f"Unknown target type '{type_}'")
 
@@ -655,14 +671,25 @@
     out["required"] = required_keys        
 
     out["type"] = "object"
 
     return out
 
 
+def get_from_default_factory(obj: Any) -> Any:
+
+    if is_dataclass(obj) and not isinstance(obj, type): # dataclass obj
+        return asdict(obj)
+    elif isinstance(obj, BaseModel):
+        return dict(obj)
+    elif isinstance(obj, list) or is_prim_type(type(obj)):
+        return obj
+    
+    return None
+    
 
 
 
 def build_dataclass_object_json_schema(type_: Any) -> dict:
     """Build a JSON schema for a dataclass type."""
 
     desc = type_.__doc__
@@ -673,16 +700,19 @@
     required = []
 
     flds = fields(type_)
     for fl in flds:
         name = fl.name
         prop_type = fl.type # can be Annotated[] -> desc
         if fl.default is MISSING:
-            default = None
-            required.append(name)
+            if fl.default_factory is not MISSING:
+                default = get_from_default_factory(fl.default_factory())
+            else: # not default means required
+                default = MISSING
+                required.append(name)
         else:
             default = fl.default
 
         prop_schema, _ = build_type_or_array_json_schema(prop_type,
                                                          default=default)
 
         props[name] = prop_schema
@@ -750,18 +780,15 @@
             enum_list = list(get_args(type_))
             type_ = type(enum_list[0])
             break
 
         elif is_subclass_of(type_, Enum): # Enum types resolve to themselves
             break
 
-        elif (type_ is str or # prim_types
-              type_ is float or 
-              type_ is int or 
-              type_ is bool):
+        elif is_prim_type(type_):
             break
         
         else:
             raise TypeError(f"Unknown final type: '{type_}'")
 
     return type_, is_list
 
@@ -811,18 +838,15 @@
                 raise TypeError(f"Expecting str to initialize time but got: '{val}'")
             return time.fromisoformat(val)
 
         elif is_subclass_of(type_, Enum):
             return type_(val)
         
         # Literals also resolve to their prim_types        
-        elif (type_ is str or 
-              type_ is float or 
-              type_ is int or 
-              type_ is bool):
+        elif is_prim_type(type_):
             value = type_(val) 
             return value
         
         else:
             raise TypeError(f"Unexpected value of type '{type_}' for value '{val}'")
 
 
@@ -848,20 +872,21 @@
 
 def get_json_type(t: Any) -> str:
     """Translate from native types to JSON's."""
     JSON_TYPE_FROM_PY_TYPE = {
         str: "string",
         float: "number",            
         int: "integer",            
-        bool: "boolean"
+        bool: "boolean",
+        NoneType: "null",
     }
     if t not in JSON_TYPE_FROM_PY_TYPE:
         raise TypeError(f"Unknown type '{t}'")
     
     return JSON_TYPE_FROM_PY_TYPE[t]
 
 
 
 # Useful:
 # string formats: https://json-schema.org/understanding-json-schema/reference/string#built-in-formats
-# Online JSON schema validator: https://www.jsonschemavalidator.net/
+# Online JSON schema validator: https://jsonschema.dev/
 # JSON pretty formatter: https://jsonformatter.org/json-pretty-print
```

### Comparing `sibila-0.4.2/sibila/llamacpp.py` & `sibila-0.4.3/sibila/llamacpp.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/mistral.py` & `sibila-0.4.3/sibila/mistral.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/model.py` & `sibila-0.4.3/sibila/model.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/models.py` & `sibila-0.4.3/sibila/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,18 @@
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
         "fireworks": {
             "mandatory": [],
             "flags": ["name_passthrough"]
         },
+        "groq": {
+            "mandatory": [],
+            "flags": ["name_passthrough"]
+        },
         "llamacpp": {
             "mandatory": ["name"],
             "flags": ["name_passthrough", "local"]
         },
         "mistral": {
             "mandatory": [],
             "flags": ["name_passthrough"]
@@ -192,14 +196,15 @@
     ALL_PROVIDER_NAMES = list(PROVIDER_CONF.keys()) + ["alias"] # providers + "alias"
 
     @classmethod
     def EMPTY_MODELS_DIR(_) -> dict:
         return {
             "anthropic": {},
             "fireworks": {},
+            "groq": {},
             "llamacpp": {},
             "mistral": {},
             "openai": {},
             "together": {},
             "alias": {},
         }
 
@@ -371,28 +376,33 @@
         if ctx_len is not None:
             args["ctx_len"] = ctx_len
 
         if resolved_create_args is not None:
             resolved_create_args.update(args)
 
 
-        logger.debug(f"Resolved '{res_name}' to '{provider}:{name}' with args: {args}")
+        logger.debug(f"Resolved '{res_name}' to provider '{provider}' with args: {args}")
 
 
         model: Model
         if provider == "anthropic":
 
             from .anthropic import AnthropicModel
             model = AnthropicModel(**args)
             
         elif provider == "fireworks":
 
             from .schema_format_openai import FireworksModel
             model = FireworksModel(**args)
             
+        elif provider == "groq":
+
+            from .schema_format_openai import GroqModel
+            model = GroqModel(**args)
+            
         elif provider == "llamacpp":
 
             # resolve filename -> path
             path = cls._locate_file(args["name"])
             if path is None:
                 path = args["name"] # LlamaCppModel should raise the exception, not us
             else:
@@ -416,21 +426,19 @@
             from .openai import OpenAIModel
             model = OpenAIModel(**args)
             
         elif provider == "together":
 
             from .schema_format_openai import TogetherModel
             model = TogetherModel(**args)
-            
-        """
-        elif provider == "hf":
-            from .hf import HFModel
-            
-            model = HFModel(**args)
-        """
+
+        else:
+            raise ValueError(f"Unknown provider '{provider}' for '{res_name}'")
+        
+    
            
         return model
 
 
 
 
     @classmethod
```

### Comparing `sibila-0.4.2/sibila/multigen.py` & `sibila-0.4.3/sibila/multigen.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/null.py` & `sibila-0.4.3/sibila/null.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/openai.py` & `sibila-0.4.3/sibila/openai.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/res/base_formats.json` & `sibila-0.4.3/sibila/res/base_formats.json`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/res/base_models.json` & `sibila-0.4.3/sibila/res/base_models.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428571428571%*

 * *Differences: {"'groq'": "OrderedDict([('_default', OrderedDict([('ctx_len', 8192), ('token_estimation_factor', "*

 * *           '0.4)]))])'}*

```diff
@@ -8,14 +8,20 @@
     },
     "fireworks": {
         "_default": {
             "ctx_len": 4096,
             "token_estimation_factor": 0.4
         }
     },
+    "groq": {
+        "_default": {
+            "ctx_len": 8192,
+            "token_estimation_factor": 0.4
+        }
+    },
     "llamacpp": {
         "_default": {
             "ctx_len": 2048
         }
     },
     "mistral": {
         "_default": {
```

### Comparing `sibila-0.4.2/sibila/schema_format_openai.py` & `sibila-0.4.3/sibila/schema_format_openai.py`

 * *Files 17% similar despite different names*

```diff
@@ -395,7 +395,199 @@
                          # other OpenAI API specific args
                          other_init_kwargs=other_init_kwargs)
 
 
 
 
 
+
+
+
+class GroqModel(SchemaFormatOpenAIModel):
+    """Access a Groq model with the OpenAI API.
+    Supports constrained JSON output, via the response_format JSON Schema mechanism.
+
+    Ref:
+        https://console.groq.com/docs/tool-use
+
+        https://github.com/groq/groq-api-cookbook/blob/main/parallel-tool-use/parallel-tool-use.ipynb
+    """
+
+    PROVIDER_NAME:str = "groq"
+    """Provider prefix that this class handles."""
+
+    DEFAULT_BASE_URL: str = "https://api.groq.com/openai/v1"
+    """Default API access URL"""
+
+    _token_estimation_factor: float
+    """Multiplication factor to estimate token usage: multiplies text length to obtain token length."""
+
+    DEFAULT_TOKEN_ESTIMATION_FACTOR: float = 0.4
+    """Default factor for token_estimation_factor."""
+
+
+    def __init__(self,
+                 name: str,
+                 *,
+                 
+                 # common base model args
+                 genconf: Optional[GenConf] = None,
+                 schemaconf: Optional[JSchemaConf] = None,
+                 ctx_len: Optional[int] = None,
+                 max_tokens_limit: Optional[int] = None,
+                 tokenizer: Optional[Tokenizer] = None,
+                
+                 # most important OpenAI API specific args
+                 api_key: Optional[str] = None,
+                 base_url: Optional[str] = None,
+                 token_estimation_factor: Optional[float] = None,
+                 
+                 # other OpenAI API specific args
+                 other_init_kwargs: dict = {},
+                 ):
+        """Create a Groq remote model.
+
+        Args:
+            name: Model name to resolve into an existing model.
+            genconf: Model generation configuration. Defaults to None.
+            schemaconf: Default configuration for JSON schema validation, used if generation call doesn't supply one. Defaults to None.
+            ctx_len: Maximum context length to be used (shared for input and output). None for model's default.
+            max_tokens_limit: Maximum output tokens limit. None for model's default.
+            tokenizer: An external initialized tokenizer to use instead of the created from the GGUF file. Defaults to None.
+            api_key: API key. Defaults to None, which will use env variable GROQ_API_KEY.
+            base_url: Base location for API access. Defaults to None, which will use env variable GROK_BASE_URL or a default.
+            token_estimation_factor: Used when no tokenizer is available. Multiplication factor to estimate token usage: multiplies total text length to obtain token length.
+            other_init_kwargs: Extra args for OpenAI.OpenAI() initialization. Defaults to {}.
+
+        Raises:
+            ImportError: If OpenAI API is not installed.
+            NameError: If model name was not found or there's an API or authentication problem.
+        """
+
+        if api_key is None:
+            api_key = os.environ.get("GROQ_API_KEY")
+        if base_url is None:
+            base_url = os.environ.get("GROQ_BASE_URL", self.DEFAULT_BASE_URL)
+
+        super().__init__(name,
+                         # common base model args
+                         genconf=genconf,
+                         schemaconf=schemaconf,
+                         ctx_len=ctx_len,
+                         max_tokens_limit=max_tokens_limit,
+                         tokenizer=tokenizer,
+                            
+                         # most important OpenAI API specific args
+                         api_key=api_key,
+                         base_url=base_url,
+                         token_estimation_factor=token_estimation_factor,
+                            
+                         # other OpenAI API specific args
+                         other_init_kwargs=other_init_kwargs)
+
+
+
+    def _gen_pre(self, 
+                 thread: Thread,
+                 genconf: Union[GenConf, None]
+                 ) -> tuple:
+
+        if genconf is None:
+            genconf = self.genconf
+
+        thread = self._prepare_gen_thread(thread, genconf)
+
+        token_len = self.token_len(thread, genconf)
+        resolved_max_tokens = self.resolve_genconf_max_tokens(token_len, genconf)
+
+
+        json_kwargs: dict = {}
+        if genconf.format == "json":
+            
+            if genconf.json_schema is not None:
+                json_kwargs["tool_choice"] = {
+                    "type": "function",
+                    "function": {"name": self.output_fn_name},
+                }
+
+                if isinstance(genconf.json_schema, str):
+                    params = json.loads(genconf.json_schema)
+                else:
+                    params = genconf.json_schema
+                
+                json_kwargs["tools"] = [
+                    {
+                        "type": "function",
+                        "function": {
+                            "name": self.output_fn_name,
+                            "parameters": params
+                        }
+                    }
+                ]
+
+            else: # free json output
+                json_kwargs["response_format"] = {"type": "json_object"}
+
+
+        # seed config is disabled, remote models and some hardware accelerated local models don't support it.
+        # seed = genconf.seed
+        # if seed == -1:
+        #    seed = int(time())
+        #    logger.debug(f"SchemaFormatOpenAIModel random seed={seed}")
+
+        
+        msgs = thread.as_chatml()
+
+        kwargs = {"model": self._model_name,
+                  "messages": msgs, # type: ignore[arg-type]
+                  "max_tokens": resolved_max_tokens,
+                  "stop": genconf.stop,
+                  "temperature": genconf.temperature,
+                  "top_p": genconf.top_p,
+                  # "seed": seed,
+                  "n": 1,
+                  **json_kwargs}
+
+        # inject model-specific args, if any
+        kwargs.update(genconf.resolve_special(self.PROVIDER_NAME))
+
+        logger.debug(f"{type(self).__name__} gen args: {kwargs}")
+
+        return (kwargs, genconf)
+
+
+    def _gen_post(self, 
+                  response: Any,
+                  pre_kwargs: dict,
+                  genconf: GenConf
+                  ) -> GenOut:
+            
+        logger.debug(f"SchemaFormatOpenAIModel response: {response}")
+
+        choice = response.choices[0]
+        finish = choice.finish_reason
+        # OpenAI-compatible provider endpoints can give non-standard finish_reason values. Map as needed:
+        if finish in ["eos", "tool_calls"]: finish = "stop"
+        message = choice.message
+
+        if "tool_choice" in pre_kwargs:
+            
+            # json schema generation via the tools API:
+            if message.tool_calls is not None:
+                if len(message.tool_calls) != 1:
+                    logger.warn(f"SchemaFormatOpenAIModel: expecting single message.tool_calls, but received {len(message.tool_calls)} - using first.")
+
+                fn = message.tool_calls[0].function
+                if fn.name != self.output_fn_name:
+                    logger.warn(f"SchemaFormatOpenAIModel: expecting '{self.output_fn_name}' function name, received ({fn.name})")
+
+                text = fn.arguments
+
+            else: # use content instead
+                logger.warn("SchemaFormatOpenAIModel: expecting message.tool_calls, but none received - using text content")
+                text = message.content # type: ignore[assignment]
+        
+        else:
+            # text or simple json format
+            text = message.content # type: ignore[assignment]
+
+        return self._prepare_gen_out(text, finish, genconf)
```

### Comparing `sibila-0.4.2/sibila/text_splitter.py` & `sibila-0.4.3/sibila/text_splitter.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/thread.py` & `sibila-0.4.3/sibila/thread.py`

 * *Files 1% similar despite different names*

```diff
@@ -655,7 +655,15 @@
         sep = self.join_sep.replace('\n', '\\n')
         out = f"inst=█{inst}█, sep='{sep}', len={len(self._msgs)}"
         for index,text in enumerate(self._msgs):
             text = text.replace("\n", "\\n")
             kind = Thread._kind_from_pos(index)
             out += f"\n{index}: {kind.name}=█{text}█"
         return out
+
+    def __repr__(self):
+        return self.__str__()
+    
+
+
+
+
```

### Comparing `sibila-0.4.2/sibila/tools.py` & `sibila-0.4.3/sibila/tools.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila/utils.py` & `sibila-0.4.3/sibila/utils.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/sibila.egg-info/PKG-INFO` & `sibila-0.4.3/sibila.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sibila
-Version: 0.4.2
+Version: 0.4.3
 Summary: Structured queries from local or online LLM models
 Author-email: Jorge Diogo <jndiogo@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jndiogo/sibila
 Project-URL: Documentation, https://jndiogo.github.io/sibila
 Project-URL: Issues, https://github.com/jndiogo/sibila/issues
 Keywords: llama.cpp,AI,Transformers,GPT,LLM
@@ -30,26 +30,28 @@
 Requires-Dist: pydantic>=2.0
 Requires-Dist: typing_extensions
 Requires-Dist: tqdm
 Requires-Dist: pytest-asyncio>=0.17
 
 # Sibila
 
-Extract structured data from remote or local LLM models. Predictable output is important for serious use of LLMs.
+Extract structured data from remote or local LLM models. Because predictable output is important for serious use of LLMs.
 
 - Query structured data into Pydantic objects, dataclasses or simple types.
 - Access remote models from OpenAI, Anthropic, Mistral AI and other providers.
 - Use local models like Llama-3, Phi-3, OpenChat or any other GGUF file model.
 - Besides structured extraction, Sibila is also a general purpose model access library, to generate plain text or free JSON results, with the same API for local and remote models.
 - Model management: download models, manage configuration, quickly switch between models.
 
-No matter how well you craft a prompt begging a model for the output you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
+No matter how well you craft a prompt begging a model for the format you need, it can always respond something else. Extracting structured data can be a big step into getting predictable behavior from your models.
 
 See [What can you do with Sibila?](https://jndiogo.github.io/sibila/what/)
 
+
+
 To extract structured data from a local model:
 
 ``` python
 from sibila import Models
 from pydantic import BaseModel
 
 class Info(BaseModel):
@@ -78,15 +80,15 @@
 
 ``` python
 model = Models.create("openai:gpt-4")
 
 model.extract(Info, "Who was the first man in the moon?")
 ```
 
-If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclass. Also includes asynchronous access to remote models.
+If Pydantic BaseModel objects are too much for your project, Sibila supports similar functionality with Python dataclasses. Also includes asynchronous access to remote models.
 
 
 
 
 ## Docs
 
 [The docs explain](https://jndiogo.github.io/sibila/) the main concepts, include examples and an API reference.
```

### Comparing `sibila-0.4.2/sibila.egg-info/SOURCES.txt` & `sibila-0.4.3/sibila.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,9 @@
 tests/test_json_schema.py
 tests/test_llamacpp_models_dir.py
 tests/test_llamacpp_tinyllama.py
 tests/test_mixtral_mistral_small.py
 tests/test_null_extract.py
 tests/test_openai_gpt35.py
 tests/test_openai_gpt4.py
+tests/test_pydantic_dataclass.py
 tests/test_together_mixtral.py
```

### Comparing `sibila-0.4.2/tests/test_anthropic_claude-3-haiku.py` & `sibila-0.4.3/tests/test_anthropic_claude-3-haiku.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_cli.py` & `sibila-0.4.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_common_llamacpp.py` & `sibila-0.4.3/tests/test_common_llamacpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     "Meta-Llama-3-8B-Instruct.Q4_K_M.gguf",
     "mistral-7b-instruct-v0.1.Q4_K_M.gguf",
     "openchat-3.5-0106.Q4_K_M.gguf",
     "openchat-3.5-1210.Q4_K_M.gguf",
     "phi-2.Q5_K_M.gguf",
     "Phi-3-mini-4k-instruct-q4.gguf",
     "stablelm-2-12b-chat-Q4_K_M.gguf",
-    "stablelm-2-zephyr-1_6b-Q4_K_M.gguf",
     "stablelm-zephyr-3b.Q4_K_M.gguf",
     "starling-lm-7b-alpha.Q5_K_M.gguf",
     "Starling-LM-7B-beta-Q4_K_M.gguf",
     "TinyDolphin-2.8-1.1b.Q4_K_M.gguf",
     "zephyr-7b-beta.Q4_K_M.gguf",
 ]
 
@@ -91,14 +90,15 @@
 """
 Models that don't pass these tests:
 "dolphin-2_6-phi-2.Q4_K_M.gguf",
 "kunoichi-dpo-v2-7b.Q4_K_M.gguf",
 "mistral-7b-instruct-v0.2.Q5_K_M.gguf",
 "qwen1_5-0_5b-chat-q4_k_m.gguf",
 "rocket-3b.Q4_K_M.gguf",
+"stablelm-2-zephyr-1_6b-Q4_K_M.gguf",
 "tinyllama-1.1b-chat-v1.0.Q4_K_M.gguf",
 "zephyr-7b-gemma-v0.1-Q4_K_M.gguf",
 """
```

### Comparing `sibila-0.4.2/tests/test_common_llamacpp_examples.py` & `sibila-0.4.3/tests/test_common_llamacpp_examples.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_common_remote.py` & `sibila-0.4.3/tests/test_common_remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,23 @@
 
 IN_CTX_LEN = 2048
 OUT_MAX_TOKENS = 1024
 
 models = [
     "anthropic:claude-3-haiku-20240307",
     "fireworks:accounts/fireworks/models/mixtral-8x7b-instruct",
+    "groq:llama3-70b-8192",
     "mistral:mistral-small-latest",
     "openai:gpt-3.5",
     "openai:gpt-4",
     "together:mistralai/Mixtral-8x7B-Instruct-v0.1",
 ]
 
 __models = [
-    "anthropic:claude-3-haiku-20240307",
+    "groq:llama3-70b-8192",
 ]
 
 
 
 
 def limit_rate(what: Union[str,Model]):
     if (isinstance(what, str) and "anthropic" in what or
```

### Comparing `sibila-0.4.2/tests/test_common_remote_examples.py` & `sibila-0.4.3/tests/test_common_remote_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "mistral:mistral-small-latest",
     "openai:gpt-3.5",
     "openai:gpt-4",
     "together:mistralai/Mixtral-8x7B-Instruct-v0.1",
 ]
 
 __models = [
-    "fireworks:accounts/fireworks/models/mixtral-8x7b-instruct"
+    "groq:llama3-70b-8192",
 ]
 
 """
 Providers/models that don't pass these tests:
 "fireworks:accounts/fireworks/models/mixtral-8x7b-instruct"
 """
```

### Comparing `sibila-0.4.2/tests/test_examples_tinyllama.py` & `sibila-0.4.3/tests/test_examples_tinyllama.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_fireworks_mixtral.py` & `sibila-0.4.3/tests/test_fireworks_mixtral.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_formats.py` & `sibila-0.4.3/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_json_schema.py` & `sibila-0.4.3/tests/test_json_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 
 from typing import Any, Optional, Union, Literal, Annotated, get_origin, get_args
 import enum
 
 from datetime import date, time, datetime
 
-from dataclasses import dataclass, is_dataclass, fields, MISSING
+from dataclasses import dataclass
 
 from pydantic import BaseModel, Field
 
 from sibila.json_schema import (
     JSchemaConf,
     get_type,
     get_type_list,
```

### Comparing `sibila-0.4.2/tests/test_llamacpp_models_dir.py` & `sibila-0.4.3/tests/test_llamacpp_models_dir.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_llamacpp_tinyllama.py` & `sibila-0.4.3/tests/test_llamacpp_tinyllama.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_mixtral_mistral_small.py` & `sibila-0.4.3/tests/test_mixtral_mistral_small.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_null_extract.py` & `sibila-0.4.3/tests/test_null_extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -129,46 +129,46 @@
 
 
 
 
 
 def test_pydantic():
 
-    class UserDetail(BaseModel):
+    class UserDetail1(BaseModel):
         """ Details about a user """
         name: str
         age: int
 
-    extract(list[UserDetail],
+    extract(list[UserDetail1],
             "Paul and his buddy Mathilda, they love to ride. He's 68 years old, she's 81.",
             '{"output": [{"name": "Paul", "age": 68}, {"name": "Mathilda", "age": 81}]}',
-            [UserDetail(name='Paul', age=68), UserDetail(name='Mathilda', age=81)])
+            [UserDetail1(name='Paul', age=68), UserDetail1(name='Mathilda', age=81)])
 
-    class UserDetail(BaseModel):
+    class UserDetail2(BaseModel):
         """ Details about a user """
         name: str = Field(..., description="The name for the user")
         age: int = Field(..., description="The user's age")
 
-    target = UserDetail
+    target = UserDetail2
     text = "Jane's 99 years old."
     response = '{"name": "Jane", "age": 99}'
-    expected = UserDetail(name='Jane', age=99)
+    expected = UserDetail2(name='Jane', age=99)
     extract(target,
             text,
             response,
             expected)
 
     model.set_response(response)
     assert model.pydantic(target, text) == expected
 
 
-    extract(list[UserDetail],
+    extract(list[UserDetail2],
             "Jane's 99 years old, Paul is 75.",
             '{"output": [{"name": "Jane", "age": 99}, {"name": "Paul", "age": 75}]}',
-            [UserDetail(name='Jane', age=99), UserDetail(name='Paul', age=75)])
+            [UserDetail2(name='Jane', age=99), UserDetail2(name='Paul', age=75)])
 
 
 
 
 def test_classify():
 
     classify(["yes", "no"],
```

### Comparing `sibila-0.4.2/tests/test_openai_gpt35.py` & `sibila-0.4.3/tests/test_openai_gpt35.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_openai_gpt4.py` & `sibila-0.4.3/tests/test_openai_gpt4.py`

 * *Files identical despite different names*

### Comparing `sibila-0.4.2/tests/test_together_mixtral.py` & `sibila-0.4.3/tests/test_together_mixtral.py`

 * *Files identical despite different names*

