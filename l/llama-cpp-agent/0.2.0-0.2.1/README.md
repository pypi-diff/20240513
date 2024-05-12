# Comparing `tmp/llama_cpp_agent-0.2.0.tar.gz` & `tmp/llama_cpp_agent-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_cpp_agent-0.2.0.tar", last modified: Sun May 12 16:24:11 2024, max compression
+gzip compressed data, was "llama_cpp_agent-0.2.1.tar", last modified: Sun May 12 21:11:30 2024, max compression
```

## Comparing `llama_cpp_agent-0.2.0.tar` & `llama_cpp_agent-0.2.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.305178 llama_cpp_agent-0.2.0/
--rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.0/LICENSE
--rw-rw-rw-   0        0        0    10017 2024-05-12 16:24:11.304177 llama_cpp_agent-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8792 2024-05-12 16:23:39.000000 llama_cpp_agent-0.2.0/ReadMe.md
--rw-rw-rw-   0        0        0     1054 2024-05-12 16:23:39.000000 llama_cpp_agent-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-12 16:24:11.305178 llama_cpp_agent-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.251598 llama_cpp_agent-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.271722 llama_cpp_agent-0.2.0/src/llama_cpp_agent/
--rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.281765 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/
--rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/__init__.py
--rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py
--rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory.py
--rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py
--rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/memory_tools.py
--rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py
--rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
--rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chain.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.286499 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/
--rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/__init__.py
--rw-rw-rw-   0        0        0     6999 2024-05-12 00:16:58.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/basic_chat_history.py
--rw-rw-rw-   0        0        0     1834 2024-05-12 00:07:51.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/chat_history_base.py
--rw-rw-rw-   0        0        0     3144 2024-05-12 11:29:01.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/messages.py
--rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling.py
--rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.288169 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/
--rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
--rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
--rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/hermes_2_pro_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.290177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/
--rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/__init__.py
--rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/schema_generator.py
--rw-rw-rw-   0        0        0    21379 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.292177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/
--rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/__init__.py
--rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/documentation_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.294177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/
--rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/__init__.py
--rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/settings.py
--rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_prompt_template.py
--rw-rw-rw-   0        0        0    22304 2024-05-12 04:37:01.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/messages_formatter.py
--rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/mixtral_8x22b_agent.py
--rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/output_parser.py
--rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompt_templates.py
--rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompts.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.300177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/
--rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/__init__.py
--rw-rw-rw-   0        0        0     8076 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_python.py
--rw-rw-rw-   0        0        0    13772 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_server.py
--rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/provider_base.py
--rw-rw-rw-   0        0        0     9067 2024-05-12 03:32:34.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/tgi_server.py
--rw-rw-rw-   0        0        0     6607 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/vllm_server.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.302177 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/
--rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/__init__.py
--rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py
--rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/structured_output_agent.py
--rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent/text_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 16:24:11.302177 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/
--rw-rw-rw-   0        0        0    10017 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2187 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      206 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-12 16:24:11.000000 llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.828156 llama_cpp_agent-0.2.1/
+-rw-rw-rw-   0        0        0     1115 2023-12-31 18:08:30.000000 llama_cpp_agent-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0    10023 2024-05-12 21:11:30.828156 llama_cpp_agent-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8798 2024-05-12 19:32:32.000000 llama_cpp_agent-0.2.1/ReadMe.md
+-rw-rw-rw-   0        0        0     1054 2024-05-12 21:10:06.000000 llama_cpp_agent-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-12 21:11:30.829156 llama_cpp_agent-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.773691 llama_cpp_agent-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.788200 llama_cpp_agent-0.2.1/src/llama_cpp_agent/
+-rw-rw-rw-   0        0        0      342 2024-05-12 15:02:27.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.796981 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/
+-rw-rw-rw-   0        0        0        0 2023-12-31 14:27:21.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/__init__.py
+-rw-rw-rw-   0        0        0     3408 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/core_memory_manager.py
+-rw-rw-rw-   0        0        0     1654 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/event_memory.py
+-rw-rw-rw-   0        0        0     3882 2024-05-11 19:58:35.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/event_memory_manager.py
+-rw-rw-rw-   0        0        0     9949 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/memory_tools.py
+-rw-rw-rw-   0        0        0     5031 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/retrieval_memory.py
+-rw-rw-rw-   0        0        0     1640 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py
+-rw-rw-rw-   0        0        0    12570 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chain.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.799318 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/
+-rw-rw-rw-   0        0        0      307 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/__init__.py
+-rw-rw-rw-   0        0        0     6999 2024-05-12 00:16:58.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/basic_chat_history.py
+-rw-rw-rw-   0        0        0     1834 2024-05-12 00:07:51.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/chat_history_base.py
+-rw-rw-rw-   0        0        0     3113 2024-05-12 20:46:35.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/messages.py
+-rw-rw-rw-   0        0        0    10771 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/function_calling.py
+-rw-rw-rw-   0        0        0    12448 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/function_calling_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.800329 llama_cpp_agent-0.2.1/src/llama_cpp_agent/gbnf_grammar_generator/
+-rw-rw-rw-   0        0        0        0 2023-12-27 02:55:26.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/gbnf_grammar_generator/__init__.py
+-rw-rw-rw-   0        0        0    52886 2024-05-11 21:21:16.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py
+-rw-rw-rw-   0        0        0    13675 2024-05-12 13:59:03.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/hermes_2_pro_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.801328 llama_cpp_agent-0.2.1/src/llama_cpp_agent/json_schema_generator/
+-rw-rw-rw-   0        0        0       53 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/json_schema_generator/__init__.py
+-rw-rw-rw-   0        0        0    11683 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/json_schema_generator/schema_generator.py
+-rw-rw-rw-   0        0        0    21379 2024-05-12 20:44:35.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.802328 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_documentation/
+-rw-rw-rw-   0        0        0      116 2024-05-09 08:09:41.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_documentation/__init__.py
+-rw-rw-rw-   0        0        0    18850 2024-05-12 00:42:14.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_documentation/documentation_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.803833 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_output_settings/
+-rw-rw-rw-   0        0        0       76 2024-05-09 12:50:53.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_output_settings/__init__.py
+-rw-rw-rw-   0        0        0    32939 2024-05-12 05:26:57.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_output_settings/settings.py
+-rw-rw-rw-   0        0        0     7027 2024-03-29 17:24:31.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_prompt_template.py
+-rw-rw-rw-   0        0        0    22343 2024-05-12 20:42:40.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/messages_formatter.py
+-rw-rw-rw-   0        0        0     3990 2024-05-12 13:53:06.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/mixtral_8x22b_agent.py
+-rw-rw-rw-   0        0        0     3613 2024-04-18 21:27:19.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/output_parser.py
+-rw-rw-rw-   0        0        0     5296 2024-05-12 04:02:32.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/prompt_templates.py
+-rw-rw-rw-   0        0        0      816 2024-05-12 03:46:37.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/prompts.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.824880 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/
+-rw-rw-rw-   0        0        0      277 2024-05-11 22:28:46.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/__init__.py
+-rw-rw-rw-   0        0        0     8076 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/llama_cpp_python.py
+-rw-rw-rw-   0        0        0    13772 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/llama_cpp_server.py
+-rw-rw-rw-   0        0        0     5392 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/provider_base.py
+-rw-rw-rw-   0        0        0     9067 2024-05-12 03:32:34.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/tgi_server.py
+-rw-rw-rw-   0        0        0     6607 2024-05-12 01:18:50.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/vllm_server.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.826146 llama_cpp_agent-0.2.1/src/llama_cpp_agent/rag/
+-rw-rw-rw-   0        0        0        0 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/rag/__init__.py
+-rw-rw-rw-   0        0        0     2359 2024-05-05 05:07:17.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/rag/rag_colbert_reranker.py
+-rw-rw-rw-   0        0        0     7073 2024-05-12 13:57:15.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/structured_output_agent.py
+-rw-rw-rw-   0        0        0     3945 2024-05-11 21:29:08.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent/text_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 21:11:30.827158 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/
+-rw-rw-rw-   0        0        0    10023 2024-05-12 21:11:30.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2187 2024-05-12 21:11:30.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 21:11:30.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      206 2024-05-12 21:11:30.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-12 21:11:30.000000 llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/top_level.txt
```

### Comparing `llama_cpp_agent-0.2.0/LICENSE` & `llama_cpp_agent-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/PKG-INFO` & `llama_cpp_agent-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.0
+Version: 0.2.1
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,33 @@
 Provides-Extra: mixtral-agent
 Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
 <img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
 ## Table of Contents
 - [Introduction](#introduction)
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
 - [Discord Community](#discord-community)
@@ -51,31 +70,15 @@
 - [Additional Information](#additional-information)
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
```

### Comparing `llama_cpp_agent-0.2.0/ReadMe.md` & `llama_cpp_agent-0.2.1/ReadMe.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # llama-cpp-agent
 
 <img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
 ## Table of Contents
 - [Introduction](#introduction)
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
 - [Discord Community](#discord-community)
@@ -21,31 +40,15 @@
 - [Additional Information](#additional-information)
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
```

### Comparing `llama_cpp_agent-0.2.0/pyproject.toml` & `llama_cpp_agent-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [  "setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "llama-cpp-agent"
-version = "0.2.0"
+version = "0.2.1"
 description = "A framework for building LLM based AI agents with llama.cpp."
 
 readme = "ReadMe.md"
 dependencies = [
     "llama-cpp-python>=0.2.60",
     "pydantic>=2.5.3",
     "requests>=2.31.0",
```

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/core_memory_manager.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/core_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/event_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/event_memory_manager.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/event_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/memory_tools.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/memory_tools.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/retrieval_memory.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/agent_memory/retrieval_memory_manager.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/chain.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/chain.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/basic_chat_history.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/basic_chat_history.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/chat_history_base.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/chat_history_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/chat_history/messages.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/chat_history/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,14 @@
                     count = 1
                     for tool_call in message.tool_calls:
                         content += f"{count}. Function: {tool_call.function.name}\nArguments: {tool_call.function.arguments}\n"
                         count += 1
                 else:
                     content = f"Function Call:\nFunction: {message.tool_calls[0].function.name}\nArguments: {message.tool_calls[0].function.arguments}\n"
         elif isinstance(message, ToolMessage):
-            content = f"Function Call Result:\nResult: {message.content}\n"
+            content = f"{message.content}\n"
         else:
             content = f"{message.content}"
         # Construct the dictionary for the current message
         msg_dict = {"role": message.role.value, "content": content}
         result.append(msg_dict)
     return result
```

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/function_calling.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/function_calling_agent.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/function_calling_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/gbnf_grammar_generator/gbnf_grammar_from_pydantic_models.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/hermes_2_pro_agent.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/hermes_2_pro_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/json_schema_generator/schema_generator.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/json_schema_generator/schema_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_agent.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_documentation/documentation_generation.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_documentation/documentation_generation.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_output_settings/settings.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_output_settings/settings.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/llm_prompt_template.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/llm_prompt_template.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/messages_formatter.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/messages_formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,20 +123,20 @@
 USER_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
 ASSISTANT_PROMPT_START_OPEN_CHAT = """GPT4 Correct Assistant: """
 ASSISTANT_PROMPT_END_OPEN_CHAT = """<|end_of_turn|>"""
 FUNCTION_PROMPT_START_OPEN_CHAT = """"""
 FUNCTION_PROMPT_END_OPEN_CHAT = """"""
 DEFAULT_OPEN_CHAT_STOP_SEQUENCES = ["<|end_of_turn|>"]
 
-SYS_PROMPT_START_PHI_3 = """"""
-SYS_PROMPT_END_PHI_3 = """\n\n"""
-USER_PROMPT_START_PHI_3 = """<|user|>"""
-USER_PROMPT_END_PHI_3 = """<|end|>\n"""
-ASSISTANT_PROMPT_START_PHI_3 = """<|assistant|>"""
-ASSISTANT_PROMPT_END_PHI_3 = """<|end|>\n"""
+SYS_PROMPT_START_PHI_3 = """<|system|>\n"""
+SYS_PROMPT_END_PHI_3 = """<|endoftext|>\n"""
+USER_PROMPT_START_PHI_3 = """<|user|>\n"""
+USER_PROMPT_END_PHI_3 = """<|endoftext|>\n"""
+ASSISTANT_PROMPT_START_PHI_3 = """<|assistant|>\n"""
+ASSISTANT_PROMPT_END_PHI_3 = """<|endoftext|>\n"""
 FUNCTION_PROMPT_START_PHI_3 = """"""
 FUNCTION_PROMPT_END_PHI_3 = """"""
 DEFAULT_PHI_3_STOP_SEQUENCES = ["<|end|>", "<|end_of_turn|>"]
 
 
 class MessagesFormatterType(Enum):
     """
@@ -542,19 +542,19 @@
     "",
     SYS_PROMPT_START_PHI_3,
     SYS_PROMPT_END_PHI_3,
     USER_PROMPT_START_PHI_3,
     USER_PROMPT_END_PHI_3,
     ASSISTANT_PROMPT_START_PHI_3,
     ASSISTANT_PROMPT_END_PHI_3,
-    True,
+    False,
     DEFAULT_PHI_3_STOP_SEQUENCES,
     True,
     FUNCTION_PROMPT_START_PHI_3,
-    FUNCTION_PROMPT_END_PHI_3,
+    FUNCTION_PROMPT_END_PHI_3
 )
 
 predefined_formatter = {
     MessagesFormatterType.MIXTRAL: mixtral_formatter,
     MessagesFormatterType.CHATML: chatml_formatter,
     MessagesFormatterType.VICUNA: vicuna_formatter,
     MessagesFormatterType.LLAMA_2: llama_2_formatter,
```

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/mixtral_8x22b_agent.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/mixtral_8x22b_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/output_parser.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompt_templates.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/prompts.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_python.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/llama_cpp_python.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/llama_cpp_server.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/llama_cpp_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/provider_base.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/provider_base.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/tgi_server.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/tgi_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/providers/vllm_server.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/providers/vllm_server.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/rag/rag_colbert_reranker.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/rag/rag_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/structured_output_agent.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/structured_output_agent.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent/text_utils.py` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent/text_utils.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/PKG-INFO` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-cpp-agent
-Version: 0.2.0
+Version: 0.2.1
 Summary: A framework for building LLM based AI agents with llama.cpp.
 Author-email: Maximilian Winter <maximilian.winter.91@gmail.com>
 Project-URL: Homepage, https://github.com/Maximilian-Winter/llama-cpp-agent
 Project-URL: Bug Tracker, https://github.com/Maximilian-Winter/llama-cpp-agent/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,14 +28,33 @@
 Provides-Extra: mixtral-agent
 Requires-Dist: mistral-common; extra == "mixtral-agent"
 
 # llama-cpp-agent
 
 <img src="https://github.com/Maximilian-Winter/llama-cpp-agent/blob/db41b3184ebc902f50edbd3d27f7a3a1128b7d7d/logo/logo_orange.png" alt="llama-cpp-agent logo" width="400"/>
 
+## Introduction
+The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
+
+The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
+
+The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
+
+## Key Features
+- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
+- **Structured Output**: Generate structured output (objects) from LLMs.
+- **Single and Parallel Function Calling**: Execute functions using LLMs.
+- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
+- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
+- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
+- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
+- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
+- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
+
+
 ## Table of Contents
 - [Introduction](#introduction)
 - [Key Features](#key-features)
 - [Installation](#installation)
 - [Documentation](#documentation)
 - [Getting Started](#getting-started)
 - [Discord Community](#discord-community)
@@ -51,31 +70,15 @@
 - [Additional Information](#additional-information)
     - [Predefined Messages Formatter](#predefined-messages-formatter)
     - [Creating Custom Messages Formatter](#creating-custom-messages-formatter)
 - [Contributing](#contributing)
 - [License](#license)
 - [FAQ](#faq)
 
-## Introduction
-The llama-cpp-agent framework is a tool designed to simplify interactions with Large Language Models (LLMs). It provides an interface for chatting with LLMs, executing function calls, generating structured output, performing retrieval augmented generation, and processing text using agentic chains with tools. 
-
-The framework uses guided sampling to constrain the model output to the user defined structures. This way also models not fine-tuned to do function calling and JSON output will be able to do it.
 
-The framework is compatible with the llama.cpp server, llama-cpp-python and its server, and with TGI and vllm servers.
-
-## Key Features
-- **Simple Chat Interface**: Engage in seamless conversations with LLMs.
-- **Structured Output**: Generate structured output (objects) from LLMs.
-- **Single and Parallel Function Calling**: Execute functions using LLMs.
-- **RAG - Retrieval Augmented Generation**: Perform retrieval augmented generation with colbert reranking.
-- **Agent Chains**: Process text using agent chains with tools, supporting Conversational, Sequential, and Mapping Chains.
-- **Guided Sampling**: Allows most 7B LLMs to do function calling and structured output. Thanks to grammars and JSON schema generation for guided sampling.
-- **Multiple Providers**: Works with llama-cpp-python, llama.cpp server, TGI server and vllm server as provider!
-- **Compatibility**: Works with python functions, pydantic tools, llama-index tools, and OpenAI tool schemas.
-- **Flexibility**: Suitable for various applications, from casual chatting to specific function executions.
 
 ## Installation
 Install the llama-cpp-agent framework using pip:
 ```shell
 pip install llama-cpp-agent
 ```
 ## Documentation
```

### Comparing `llama_cpp_agent-0.2.0/src/llama_cpp_agent.egg-info/SOURCES.txt` & `llama_cpp_agent-0.2.1/src/llama_cpp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

