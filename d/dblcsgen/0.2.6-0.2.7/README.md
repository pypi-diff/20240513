# Comparing `tmp/dblcsgen-0.2.6.tar.gz` & `tmp/dblcsgen-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dblcsgen-0.2.6.tar", last modified: Wed May  8 09:02:52 2024, max compression
+gzip compressed data, was "dblcsgen-0.2.7.tar", last modified: Mon May 13 11:55:28 2024, max compression
```

## Comparing `dblcsgen-0.2.6.tar` & `dblcsgen-0.2.7.tar`

### file list

```diff
@@ -1,80 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.451008 dblcsgen-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-08 09:02:50.000000 dblcsgen-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    28343 2024-05-08 09:02:52.451008 dblcsgen-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-05-08 09:02:50.000000 dblcsgen-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.443008 dblcsgen-0.2.6/dblcsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28343 2024-05-08 09:02:52.000000 dblcsgen-0.2.6/dblcsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-08 09:02:52.000000 dblcsgen-0.2.6/dblcsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 09:02:52.000000 dblcsgen-0.2.6/dblcsgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-08 09:02:52.000000 dblcsgen-0.2.6/dblcsgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 09:02:52.000000 dblcsgen-0.2.6/dblcsgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 09:02:52.451008 dblcsgen-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.435008 dblcsgen-0.2.6/sglang/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.435008 dblcsgen-0.2.6/sglang/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/backend/base_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/backend/runtime_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/global_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.435008 dblcsgen-0.2.6/sglang/lang/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10476 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/chat_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    27168 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     8260 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/lang/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/launch_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.439008 dblcsgen-0.2.6/sglang/srt/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/backend_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.439008 dblcsgen-0.2.6/sglang/srt/constrained/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/constrained/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/constrained/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/constrained/fsm_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/constrained/jump_forward.py
--rw-r--r--   0 runner    (1001) docker     (127)    15496 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/hf_transformers_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.439008 dblcsgen-0.2.6/sglang/srt/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/layers/context_flashattention_nopad.py
--rw-r--r--   0 runner    (1001) docker     (127)    12622 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/layers/extend_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/layers/logits_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/layers/radix_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/layers/token_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.439008 dblcsgen-0.2.6/sglang/srt/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/detokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/io_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/openai_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.443008 dblcsgen-0.2.6/sglang/srt/managers/router/
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/infer_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28072 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/model_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    16926 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/model_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6524 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/radix_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/router/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/managers/tokenizer_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/memory_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/mm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/model_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.443008 dblcsgen-0.2.6/sglang/srt/models/
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/dbrx.py
--rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/dbrx_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/gemma.py
--rw-r--r--   0 runner    (1001) docker     (127)    11611 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/llama2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14922 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/llava.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/mistral.py
--rw-r--r--   0 runner    (1001) docker     (127)    13915 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/mixtral.py
--rw-r--r--   0 runner    (1001) docker     (127)     9225 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/qwen.py
--rw-r--r--   0 runner    (1001) docker     (127)    11307 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/qwen2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/stablelm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/models/yivl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/sampling_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    27702 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     9143 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/server_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     7582 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/srt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 09:02:52.443008 dblcsgen-0.2.6/sglang/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/test/test_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/test/test_openai_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/test/test_programs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-08 09:02:47.000000 dblcsgen-0.2.6/sglang/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 11:55:26.000000 dblcsgen-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14367 2024-05-13 11:55:26.000000 dblcsgen-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/dblcsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28445 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-13 11:55:28.000000 dblcsgen-0.2.7/dblcsgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/base_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/backend/runtime_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/global_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.310349 dblcsgen-0.2.7/sglang/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/chat_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8284 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/lang/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/launch_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/constrained/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/fsm_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/constrained/jump_forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/flush_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/hf_transformers_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/context_flashattention_nopad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/extend_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/logits_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/radix_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/layers/token_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.314349 dblcsgen-0.2.7/sglang/srt/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/detokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/io_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.318349 dblcsgen-0.2.7/sglang/srt/managers/router/
+-rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/infer_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29391 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/model_rpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16526 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/model_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7924 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/radix_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/router/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/managers/tokenizer_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/memory_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8889 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/mm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/model_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.318349 dblcsgen-0.2.7/sglang/srt/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/commandr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14158 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/dbrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11071 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/dbrx_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/gemma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/llama2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14941 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/llava.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/mistral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/mixtral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/qwen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/qwen2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10828 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/stablelm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/models/yivl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13214 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/openai_api_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/sampling_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9550 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/server_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15930 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/srt/weight_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:55:28.322348 dblcsgen-0.2.7/sglang/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_openai_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_programs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-05-13 11:55:22.000000 dblcsgen-0.2.7/sglang/utils.py
```

### Comparing `dblcsgen-0.2.6/LICENSE` & `dblcsgen-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/PKG-INFO` & `dblcsgen-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.6
+Version: 0.2.7
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,19 +218,19 @@
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
-Requires-Dist: vllm>=0.4.0; extra == "srt"
+Requires-Dist: vllm>=0.4.2; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
-Requires-Dist: pydantic==2.7.1; extra == "srt"
+Requires-Dist: packaging; extra == "srt"
 Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 
 <div align="center">
 <img src="assets/logo.png" alt="logo" width="400"></img>
 </div>
@@ -526,15 +526,14 @@
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
 ### OpenAI Compatible API
-
 In addition, the server supports an experimental OpenAI-compatible API.
 
 ```python
 import openai
 client = openai.Client(
     base_url="http://127.0.0.1:30000/v1", api_key="EMPTY")
 
@@ -556,23 +555,25 @@
     ],
     temperature=0,
     max_tokens=64,
 )
 print(response)
 ```
 
-In above example, the server uses the chat template specified in the model tokenizer.
-You can override the chat template if needed when launching the server:
+
+By default, the server uses the chat template specified in the model tokenizer from Hugging Face. It should just work for most official models such as Llama-2/Llama-3.
+
+If needed, you can also override the chat template when launching the server:
 
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000 --chat-template llama-2
 ```
 
 If the chat template you are looking for is missing, you are welcome to contribute it.
-Meanwhile, you can also temporary register your chat template as follows:
+Meanwhile, you can also temporarily register your chat template as follows:
 
 ```json
 {
   "name": "my_model",
   "system": "<|im_start|>system",
   "user": "<|im_start|>user",
   "assistant": "<|im_start|>assistant",
@@ -607,18 +608,22 @@
   - `python -m sglang.launch_server --model-path google/gemma-7b-it --port 30000 --attention-reduce-in-fp32`
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-vicuna-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-34b --tokenizer-path liuhaotian/llava-v1.6-34b-tokenizer --port 3000`
 - Yi-VL
   - see [srt_example_yi_vl.py](examples/quick_start/srt_example_yi_vl.py).
-- AWQ/GPTQ quantization
+- StableLM
+- Command-R
+- DBRX
+- AWQ/GPTQ/Marlin quantization
 
-## Benchmark And Performance
+Instructions for supporting a new model are [here](https://github.com/sgl-project/sglang/blob/main/docs/model_support.md).
 
+## Benchmark And Performance
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
@@ -634,11 +639,8 @@
       year={2023},
       eprint={2312.07104},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
 ```
 
-[![Paper page](https://huggingface.co/datasets/huggingface/badges/resolve/main/paper-page-md.svg)](https://huggingface.co/papers/2312.07104)
-
-
 We learned from the design and reused some code of the following projects: [Guidance](https://github.com/guidance-ai/guidance), [vLLM](https://github.com/vllm-project/vllm), [LightLLM](https://github.com/ModelTC/lightllm), [FlashInfer](https://github.com/flashinfer-ai/flashinfer), [Outlines](https://github.com/outlines-dev/outlines), [LMQL](https://github.com/eth-sri/lmql).
```

### Comparing `dblcsgen-0.2.6/README.md` & `dblcsgen-0.2.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -293,15 +293,14 @@
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
 ### OpenAI Compatible API
-
 In addition, the server supports an experimental OpenAI-compatible API.
 
 ```python
 import openai
 client = openai.Client(
     base_url="http://127.0.0.1:30000/v1", api_key="EMPTY")
 
@@ -323,23 +322,25 @@
     ],
     temperature=0,
     max_tokens=64,
 )
 print(response)
 ```
 
-In above example, the server uses the chat template specified in the model tokenizer.
-You can override the chat template if needed when launching the server:
+
+By default, the server uses the chat template specified in the model tokenizer from Hugging Face. It should just work for most official models such as Llama-2/Llama-3.
+
+If needed, you can also override the chat template when launching the server:
 
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000 --chat-template llama-2
 ```
 
 If the chat template you are looking for is missing, you are welcome to contribute it.
-Meanwhile, you can also temporary register your chat template as follows:
+Meanwhile, you can also temporarily register your chat template as follows:
 
 ```json
 {
   "name": "my_model",
   "system": "<|im_start|>system",
   "user": "<|im_start|>user",
   "assistant": "<|im_start|>assistant",
@@ -374,18 +375,22 @@
   - `python -m sglang.launch_server --model-path google/gemma-7b-it --port 30000 --attention-reduce-in-fp32`
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-vicuna-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-34b --tokenizer-path liuhaotian/llava-v1.6-34b-tokenizer --port 3000`
 - Yi-VL
   - see [srt_example_yi_vl.py](examples/quick_start/srt_example_yi_vl.py).
-- AWQ/GPTQ quantization
+- StableLM
+- Command-R
+- DBRX
+- AWQ/GPTQ/Marlin quantization
 
-## Benchmark And Performance
+Instructions for supporting a new model are [here](https://github.com/sgl-project/sglang/blob/main/docs/model_support.md).
 
+## Benchmark And Performance
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
@@ -401,11 +406,8 @@
       year={2023},
       eprint={2312.07104},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
 ```
 
-[![Paper page](https://huggingface.co/datasets/huggingface/badges/resolve/main/paper-page-md.svg)](https://huggingface.co/papers/2312.07104)
-
-
 We learned from the design and reused some code of the following projects: [Guidance](https://github.com/guidance-ai/guidance), [vLLM](https://github.com/vllm-project/vllm), [LightLLM](https://github.com/ModelTC/lightllm), [FlashInfer](https://github.com/flashinfer-ai/flashinfer), [Outlines](https://github.com/outlines-dev/outlines), [LMQL](https://github.com/eth-sri/lmql).
```

### Comparing `dblcsgen-0.2.6/dblcsgen.egg-info/PKG-INFO` & `dblcsgen-0.2.7/dblcsgen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dblcsgen
-Version: 0.2.6
+Version: 0.2.7
 Summary: DBLC Fast Structured Generation
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -218,19 +218,19 @@
 Requires-Dist: fastapi; extra == "srt"
 Requires-Dist: psutil; extra == "srt"
 Requires-Dist: rpyc; extra == "srt"
 Requires-Dist: torch; extra == "srt"
 Requires-Dist: uvloop; extra == "srt"
 Requires-Dist: uvicorn; extra == "srt"
 Requires-Dist: zmq; extra == "srt"
-Requires-Dist: vllm>=0.4.0; extra == "srt"
+Requires-Dist: vllm>=0.4.2; extra == "srt"
 Requires-Dist: interegular; extra == "srt"
 Requires-Dist: pydantic; extra == "srt"
 Requires-Dist: pillow; extra == "srt"
-Requires-Dist: pydantic==2.7.1; extra == "srt"
+Requires-Dist: packaging; extra == "srt"
 Requires-Dist: outlines==0.0.34; extra == "srt"
 Provides-Extra: all
 Requires-Dist: sglang[srt]; extra == "all"
 
 <div align="center">
 <img src="assets/logo.png" alt="logo" width="400"></img>
 </div>
@@ -526,15 +526,14 @@
       "temperature": 0
     }
   }'
 ```
 Learn more about the argument format [here](docs/sampling_params.md).
 
 ### OpenAI Compatible API
-
 In addition, the server supports an experimental OpenAI-compatible API.
 
 ```python
 import openai
 client = openai.Client(
     base_url="http://127.0.0.1:30000/v1", api_key="EMPTY")
 
@@ -556,23 +555,25 @@
     ],
     temperature=0,
     max_tokens=64,
 )
 print(response)
 ```
 
-In above example, the server uses the chat template specified in the model tokenizer.
-You can override the chat template if needed when launching the server:
+
+By default, the server uses the chat template specified in the model tokenizer from Hugging Face. It should just work for most official models such as Llama-2/Llama-3.
+
+If needed, you can also override the chat template when launching the server:
 
 ```
 python -m sglang.launch_server --model-path meta-llama/Llama-2-7b-chat-hf --port 30000 --chat-template llama-2
 ```
 
 If the chat template you are looking for is missing, you are welcome to contribute it.
-Meanwhile, you can also temporary register your chat template as follows:
+Meanwhile, you can also temporarily register your chat template as follows:
 
 ```json
 {
   "name": "my_model",
   "system": "<|im_start|>system",
   "user": "<|im_start|>user",
   "assistant": "<|im_start|>assistant",
@@ -607,18 +608,22 @@
   - `python -m sglang.launch_server --model-path google/gemma-7b-it --port 30000 --attention-reduce-in-fp32`
 - LLaVA
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.5-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-vicuna-7b --tokenizer-path llava-hf/llava-1.5-7b-hf --chat-template vicuna_v1.1 --port 30000`
   - `python3 -m sglang.launch_server --model-path liuhaotian/llava-v1.6-34b --tokenizer-path liuhaotian/llava-v1.6-34b-tokenizer --port 3000`
 - Yi-VL
   - see [srt_example_yi_vl.py](examples/quick_start/srt_example_yi_vl.py).
-- AWQ/GPTQ quantization
+- StableLM
+- Command-R
+- DBRX
+- AWQ/GPTQ/Marlin quantization
 
-## Benchmark And Performance
+Instructions for supporting a new model are [here](https://github.com/sgl-project/sglang/blob/main/docs/model_support.md).
 
+## Benchmark And Performance
 - Llama-7B on NVIDIA A10G, FP16, Tensor Parallelism=1
 ![llama_7b](assets/llama_7b.jpg)
 
 - Mixtral-8x7B on NVIDIA A10G, FP16, Tensor Parallelism=8
 ![mixtral_8x7b](assets/mixtral_8x7b.jpg)
 
 Learn more [here](docs/benchmark_results.md).
@@ -634,11 +639,8 @@
       year={2023},
       eprint={2312.07104},
       archivePrefix={arXiv},
       primaryClass={cs.AI}
 }
 ```
 
-[![Paper page](https://huggingface.co/datasets/huggingface/badges/resolve/main/paper-page-md.svg)](https://huggingface.co/papers/2312.07104)
-
-
 We learned from the design and reused some code of the following projects: [Guidance](https://github.com/guidance-ai/guidance), [vLLM](https://github.com/vllm-project/vllm), [LightLLM](https://github.com/ModelTC/lightllm), [FlashInfer](https://github.com/flashinfer-ai/flashinfer), [Outlines](https://github.com/outlines-dev/outlines), [LMQL](https://github.com/eth-sri/lmql).
```

### Comparing `dblcsgen-0.2.6/dblcsgen.egg-info/SOURCES.txt` & `dblcsgen-0.2.7/dblcsgen.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,46 @@
 sglang/backend/runtime_endpoint.py
 sglang/lang/__init__.py
 sglang/lang/chat_template.py
 sglang/lang/compiler.py
 sglang/lang/interpreter.py
 sglang/lang/ir.py
 sglang/lang/tracer.py
-sglang/srt/backend_config.py
 sglang/srt/conversation.py
+sglang/srt/flush_cache.py
 sglang/srt/hf_transformers_utils.py
 sglang/srt/memory_pool.py
 sglang/srt/mm_utils.py
 sglang/srt/model_config.py
+sglang/srt/openai_api_adapter.py
+sglang/srt/openai_protocol.py
 sglang/srt/sampling_params.py
 sglang/srt/server.py
 sglang/srt/server_args.py
 sglang/srt/utils.py
+sglang/srt/weight_utils.py
 sglang/srt/constrained/__init__.py
 sglang/srt/constrained/base_cache.py
 sglang/srt/constrained/fsm_cache.py
 sglang/srt/constrained/jump_forward.py
 sglang/srt/layers/context_flashattention_nopad.py
 sglang/srt/layers/extend_attention.py
 sglang/srt/layers/logits_processor.py
 sglang/srt/layers/radix_attention.py
 sglang/srt/layers/token_attention.py
 sglang/srt/managers/detokenizer_manager.py
 sglang/srt/managers/io_struct.py
-sglang/srt/managers/openai_protocol.py
 sglang/srt/managers/tokenizer_manager.py
 sglang/srt/managers/router/infer_batch.py
 sglang/srt/managers/router/manager.py
 sglang/srt/managers/router/model_rpc.py
 sglang/srt/managers/router/model_runner.py
 sglang/srt/managers/router/radix_cache.py
 sglang/srt/managers/router/scheduler.py
+sglang/srt/models/commandr.py
 sglang/srt/models/dbrx.py
 sglang/srt/models/dbrx_config.py
 sglang/srt/models/gemma.py
 sglang/srt/models/llama2.py
 sglang/srt/models/llava.py
 sglang/srt/models/mistral.py
 sglang/srt/models/mixtral.py
```

### Comparing `dblcsgen-0.2.6/pyproject.toml` & `dblcsgen-0.2.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dblcsgen"
-version = "0.2.6"
+version = "0.2.7"
 description = "DBLC Fast Structured Generation"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
@@ -16,16 +16,15 @@
 dependencies = [
     "requests",
     "tqdm",
 ]
 
 [project.optional-dependencies]
 srt = ["aiohttp", "fastapi", "psutil", "rpyc", "torch", "uvloop", "uvicorn",
-    "zmq", "vllm>=0.4.0", "interegular", "pydantic", "pillow",
-    "pydantic==2.7.1",
+    "zmq", "vllm>=0.4.2", "interegular", "pydantic", "pillow", "packaging",
     "outlines==0.0.34" # There is a breaking change to regexes on 0.0.35, not handled by SGLang atm
 ]
 all = ["sglang[srt]"]
 
 [project.urls]
 "Homepage" = "https://github.com/sgl-project/sglang"
 "Bug Tracker" = "https://github.com/sgl-project/sglang/issues"
```

### Comparing `dblcsgen-0.2.6/sglang/api.py` & `dblcsgen-0.2.7/sglang/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Public API"""
+"""Some Public API Definitions"""
 
+import os
 import re
 from typing import Callable, List, Optional, Union
 
 from sglang.backend.base_backend import BaseBackend
-from sglang.backend.runtime_endpoint import RuntimeEndpoint
 from sglang.global_config import global_config
 from sglang.lang.ir import (
     SglExpr,
     SglExprList,
     SglFunction,
     SglGen,
     SglImage,
@@ -28,14 +28,15 @@
         return SglFunction(func, api_num_spec_tokens=api_num_spec_tokens)
 
     return decorator
 
 
 def Runtime(*args, **kwargs):
     # Avoid importing unnecessary dependency
+    os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
     from sglang.srt.server import Runtime
 
     return Runtime(*args, **kwargs)
 
 
 def set_default_backend(backend: BaseBackend):
     global_config.default_backend = backend
```

### Comparing `dblcsgen-0.2.6/sglang/backend/base_backend.py` & `dblcsgen-0.2.7/sglang/backend/base_backend.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/backend/runtime_endpoint.py` & `dblcsgen-0.2.7/sglang/backend/runtime_endpoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 from typing import Callable, List, Optional, Union
 
 import numpy as np
 import requests
+
 from sglang.backend.base_backend import BaseBackend
 from sglang.global_config import global_config
 from sglang.lang.chat_template import get_chat_template_by_model_path
 from sglang.lang.interpreter import StreamExecutor
 from sglang.lang.ir import SglArgument, SglSamplingParams
 from sglang.utils import encode_image_base64, find_printable_text, http_request
 
@@ -102,22 +103,24 @@
         sampling_params: SglSamplingParams,
     ):
         if sampling_params.dtype is None:
             data = {
                 "text": s.text_,
                 "sampling_params": {
                     "skip_special_tokens": global_config.skip_special_tokens_in_output,
+                    "spaces_between_special_tokens": global_config.spaces_between_special_tokens_in_out,
                     **sampling_params.to_srt_kwargs(),
                 },
             }
         elif sampling_params.dtype in [int, "int"]:
             data = {
                 "text": s.text_,
                 "sampling_params": {
                     "skip_special_tokens": global_config.skip_special_tokens_in_output,
+                    "spaces_between_special_tokens": global_config.spaces_between_special_tokens_in_out,
                     "dtype": "int",
                     **sampling_params.to_srt_kwargs(),
                 },
             }
         else:
             raise RuntimeError(f"Invalid dtype: {sampling_params.dtype}")
 
@@ -140,22 +143,24 @@
         sampling_params: SglSamplingParams,
     ):
         if sampling_params.dtype is None:
             data = {
                 "text": s.text_,
                 "sampling_params": {
                     "skip_special_tokens": global_config.skip_special_tokens_in_output,
+                    "spaces_between_special_tokens": global_config.spaces_between_special_tokens_in_out,
                     **sampling_params.to_srt_kwargs(),
                 },
             }
         elif sampling_params.dtype in [int, "int"]:
             data = {
                 "text": s.text_,
                 "sampling_params": {
                     "skip_special_tokens": global_config.skip_special_tokens_in_output,
+                    "spaces_between_special_tokens": global_config.spaces_between_special_tokens_in_out,
                     "dtype": "int",
                     **sampling_params.to_srt_kwargs(),
                 },
             }
         else:
             raise RuntimeError(f"Invalid dtype: {sampling_params.dtype}")
 
@@ -211,15 +216,14 @@
 
         # Compute logprob
         data = {
             "text": [s.text_ + c for c in choices],
             "sampling_params": {"max_new_tokens": 0},
             "return_logprob": True,
             "logprob_start_len": max(prompt_len - 2, 0),
-            "return_text_in_logprobs": True,
         }
         self._add_images(s, data)
         res = http_request(
             self.base_url + "/generate",
             json=data,
             auth_token=self.auth_token,
             api_key=self.api_key,
```

### Comparing `dblcsgen-0.2.6/sglang/global_config.py` & `dblcsgen-0.2.7/sglang/global_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,21 +8,25 @@
         # 2: output final text after every run
         self.verbosity = 0
 
         self.default_backend = None
 
         # Output configs
         self.skip_special_tokens_in_output = True
+        self.spaces_between_special_tokens_in_out = True
 
         # Optimization configs
         self.eager_fill_image = False
         self.enable_prefix_sharing = True
         self.enable_parallel_encoding = True
         self.enable_parallel_decoding = True
 
         # Choices: ["no_adjust", "adjust_cache"]
         # no_adjust: Do not adjust the position embedding of KV cache.
         # adjust_cache: Adjust the position embedding of KV cache.
         self.concate_and_append_mode = "no_adjust"
 
+        # Request dependency time due to network delay
+        self.request_dependency_time = 0.03
+
 
 global_config = GlobalConfig()
```

### Comparing `dblcsgen-0.2.6/sglang/lang/chat_template.py` & `dblcsgen-0.2.7/sglang/lang/chat_template.py`

 * *Files 6% similar despite different names*

```diff
@@ -223,14 +223,33 @@
             "user": ("\n<|im_start|>user\n", "<|im_end|>"),
             "assistant": ("\n<|im_start|>assistant\n", "<|im_end|>"),
         },
         stop_str=("<|im_end|>",),
     )
 )
 
+register_chat_template(
+    ChatTemplate(
+        name="c4ai-command-r",
+        default_system_prompt=None,
+        role_prefix_and_suffix={
+            "system": (
+                "<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>",
+                "<|END_OF_TURN_TOKEN|>",
+            ),
+            "user": ("<|START_OF_TURN_TOKEN|><|USER_TOKEN|>", "<|END_OF_TURN_TOKEN|>"),
+            "assistant": (
+                "<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>",
+                "<|END_OF_TURN_TOKEN|>",
+            ),
+        },
+        style=ChatTemplateStyle.PLAIN,
+    )
+)
+
 
 @register_chat_template_matching_function
 def match_dbrx(model_path: str):
     if "dbrx" in model_path.lower() and "instruct" in model_path.lower():
         return get_chat_template("dbrx-instruct")
 
 
@@ -283,14 +302,21 @@
 @register_chat_template_matching_function
 def match_gemma_it(model_path: str):
     model_path = model_path.lower()
     if "gemma" in model_path and "it" in model_path:
         return get_chat_template("gemma-it")
 
 
+@register_chat_template_matching_function
+def match_c4ai_command_r(model_path: str):
+    model_path = model_path.lower()
+    if "c4ai-command-r" in model_path:
+        return get_chat_template("c4ai-command-r")
+
+
 if __name__ == "__main__":
     messages = [
         {"role": "system", "content": None},  # None means default
         # {"role": "system", "content": "You are a helpful, respectful and honest assistant."},
         {"role": "user", "content": "Hello!"},
         {"role": "assistant", "content": "Hi!"},
         {"role": "user", "content": "What can you do?"},
```

### Comparing `dblcsgen-0.2.6/sglang/lang/compiler.py` & `dblcsgen-0.2.7/sglang/lang/compiler.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/lang/interpreter.py` & `dblcsgen-0.2.7/sglang/lang/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """The interpreter that executes SGL programs"""
 
 import asyncio
+import contextvars
 import multiprocessing
 import queue
 import threading
 import uuid
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import tqdm
+
 from sglang.global_config import global_config
 from sglang.lang.ir import (
     SglCommitLazy,
     SglConcateAndAppend,
     SglConstantText,
     SglExpr,
     SglExprList,
@@ -23,15 +25,15 @@
     SglRoleBegin,
     SglRoleEnd,
     SglSelect,
     SglVariable,
     SglVarScopeBegin,
     SglVarScopeEnd,
 )
-from sglang.utils import encode_image_base64
+from sglang.utils import encode_image_base64, get_exception_traceback
 
 
 def run_internal(state, program, func_args, func_kwargs, sync):
     try:
         state.ret_value = program.func(state, *func_args, **func_kwargs)
     except Exception as e:
         raise e
@@ -189,14 +191,15 @@
         self.stream = stream
         self.api_num_spec_tokens = api_num_spec_tokens
 
         self.variables = {}  # Dict[name: str -> value: str]
         self.variable_event = {}  # Dict[name: str -> event: threading.Event]
         self.meta_info = {}  # Dict[name: str -> info: str]
         self.is_finished = False
+        self.error = None
 
         # For completion
         self.text_ = ""  # The full text
 
         # For speculative execution
         self.speculated_text = ""
 
@@ -213,15 +216,21 @@
         # For fork/join
         self.fork_start_text_pos = None
 
         # Worker thread
         self.use_thread = use_thread
         if self.use_thread:
             self.queue = queue.Queue()
-            self.worker = threading.Thread(target=self._thread_worker_func)
+
+            def _run_worker_in_context():
+                self._thread_worker_func()
+
+            self.worker = threading.Thread(
+                target=contextvars.copy_context().run, args=(_run_worker_in_context,)
+            )
             self.worker.start()
 
         # For streaming
         if stream:
             self.stream_text_event = threading.Event()
             self.stream_var_event = {}
         else:
@@ -254,35 +263,34 @@
             if not got:
                 raise TimeoutError(f"Timeout while waiting for event '{name}'")
         ret = self.meta_info.get(name, None)
         return ret
 
     def fork(
         self,
-        number: int,
+        size: int = 1,
         position_ids_offset: Optional[List[int]] = None,
-        copy: bool = False,
     ):
-        if number > 1 or copy:
+        if size > 1:
             self.submit(SglCommitLazy())
-            self.sync()
 
-        number = int(number)
+        self.sync()
+        size = int(size)
 
         exes = [
             StreamExecutor(
                 self.backend,
                 self.arguments,
                 self.default_sampling_para,
                 self.chat_template,
                 self.stream,
             )
-            for _ in range(number)
+            for _ in range(size)
         ]
-        for i in range(number):
+        for i in range(size):
             exes[i].variables = dict(self.variables)
             exes[i].text_ = str(self.text_)
             exes[i].messages_ = list(self.messages_)
             exes[i].cur_role = self.cur_role
             exes[i].fork_start_text_pos = len(self.text_)
             exes[i].images_ = list(self.images_)
 
@@ -299,25 +307,47 @@
     def end(self):
         if self.use_thread:
             if self.worker.is_alive():
                 self.queue.put(None)
         self.backend.end_program(self)
 
     def _thread_worker_func(self):
+        error = None
+
         while True:
             expr = self.queue.get()
             if expr is None:
                 self.queue.task_done()
                 break
 
-            self._execute(expr)
+            try:
+                self._execute(expr)
+            except Exception as e:
+                print(f"Error in stream_executor: {get_exception_traceback()}")
+                error = e
+                break
             self.queue.task_done()
             if self.stream_text_event:
                 self.stream_text_event.set()
 
+        # Clean the queue and events
+        if error is not None:
+            try:
+                while True:
+                    self.queue.task_done()
+                    self.queue.get_nowait()
+            except queue.Empty:
+                pass
+            for name in self.variable_event:
+                self.variable_event[name].set()
+            if self.stream_var_event:
+                for name in self.stream_var_event:
+                    self.stream_var_event[name].set()
+            self.error = error
+
         if self.stream_text_event:
             self.stream_text_event.set()
 
         self.is_finished = True
 
     def _execute(self, other):
         if isinstance(other, str):
@@ -645,19 +675,18 @@
     def var_scope(self, name: str):
         self.stream_executor.submit(SglVarScopeBegin(name))
         yield
         self.stream_executor.submit(SglVarScopeEnd(name))
 
     def fork(
         self,
-        number: int = 1,
+        size: int = 1,
         position_ids_offset: Optional[List[int]] = None,
-        copy: bool = False,
     ):
-        stream_executors = self.stream_executor.fork(number, position_ids_offset, copy)
+        stream_executors = self.stream_executor.fork(size, position_ids_offset)
         states = [ProgramState(x) for x in stream_executors]
         state_group = ProgramStateGroup(states, self)
         return state_group
 
     @contextmanager
     def copy(self, position_ids_offset: Optional[List[int]] = None):
         state_group = self.fork(1, position_ids_offset, True)
@@ -669,15 +698,17 @@
     def text(self):
         return self.stream_executor.text()
 
     def messages(self):
         return self.stream_executor.messages()
 
     def sync(self):
-        return self.stream_executor.sync()
+        ret = self.stream_executor.sync()
+        self.error = self.stream_executor.error
+        return ret
 
     def text_iter(self, var_name: Optional[str] = None):
         if self.stream_executor.stream:
             prev = 0
             if var_name is None:
                 event = self.stream_executor.stream_text_event
                 while True:
@@ -759,14 +790,17 @@
 
     def __getitem__(self, name):
         return self.get_var(name)
 
     def __setitem__(self, name, value):
         self.set_var(name, value)
 
+    def __contains__(self, name):
+        return name in self.stream_executor.variables
+
     def __del__(self):
         self.stream_executor.end()
 
     def __repr__(self) -> str:
         return f"ProgramState({self.text()})"
```

### Comparing `dblcsgen-0.2.6/sglang/lang/ir.py` & `dblcsgen-0.2.7/sglang/lang/ir.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/lang/tracer.py` & `dblcsgen-0.2.7/sglang/lang/tracer.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,27 +105,29 @@
         if cur_scope is not None:
             cur_scope.add_child_state(self)
 
     ##################################
     ########### Public API ###########
     ##################################
 
-    def fork(self, number: int, position_ids_offset: Optional[List[int]] = None):
+    def fork(self, size: int = 1, position_ids_offset: Optional[List[int]] = None):
+        assert (size >= 1)
+
         if self.only_trace_prefix:
             raise StopTracing()
 
-        fork_node = SglFork(number)
+        fork_node = SglFork(size)
         fork_node.prev_node = self.last_node
 
         states = [
             TracerProgramState(self.backend, self.arguments, self.only_trace_prefix)
-            for _ in range(number)
+            for _ in range(size)
         ]
 
-        for i in range(number):
+        for i in range(size):
             node = SglGetForkItem(i)
             node.prev_node = fork_node
             states[i].last_node = node
             states[i].variables = dict(self.variables)
             states[i].messages_ = list(self.messages_)
             states[i].cur_role = self.cur_role
             states[i].chat_template = self.chat_template
```

### Comparing `dblcsgen-0.2.6/sglang/srt/constrained/__init__.py` & `dblcsgen-0.2.7/sglang/srt/constrained/__init__.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/constrained/base_cache.py` & `dblcsgen-0.2.7/sglang/srt/constrained/base_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/constrained/fsm_cache.py` & `dblcsgen-0.2.7/sglang/srt/constrained/fsm_cache.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/constrained/jump_forward.py` & `dblcsgen-0.2.7/sglang/srt/constrained/jump_forward.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import interegular
+
 from sglang.srt.constrained import FSMInfo, disk_cache, make_deterministic_fsm
 from sglang.srt.constrained.base_cache import BaseCache
 
 IP_REGEX = r"((25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(25[0-5]|2[0-4]\d|[01]?\d\d?)"
 
 
 class JumpForwardMap:
```

### Comparing `dblcsgen-0.2.6/sglang/srt/conversation.py` & `dblcsgen-0.2.7/sglang/srt/conversation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Adapted from
 # https://github.com/lm-sys/FastChat/blob/main/fastchat/conversation.py
 import dataclasses
 from enum import IntEnum, auto
 from typing import Dict, List, Optional, Tuple, Union
 
-from sglang.srt.managers.openai_protocol import ChatCompletionRequest
+from sglang.srt.openai_protocol import ChatCompletionRequest
 
 
 class SeparatorStyle(IntEnum):
     """Separator styles."""
 
     ADD_COLON_SINGLE = auto()
     ADD_COLON_TWO = auto()
@@ -396,15 +396,15 @@
     )
 )
 
 register_conv_template(
     Conversation(
         name="chatml",
         system_template="<|im_start|>system\n{system_message}",
-        system_message="You are an AI assistant.",
+        system_message="You are a helpful assistant.",
         roles=("<|im_start|>user", "<|im_start|>assistant"),
         sep_style=SeparatorStyle.CHATML,
         sep="<|im_end|>",
         stop_str=["<|endoftext|>", "<|im_end|>"],
     )
 )
```

### Comparing `dblcsgen-0.2.6/sglang/srt/hf_transformers_utils.py` & `dblcsgen-0.2.7/sglang/srt/hf_transformers_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import json
 import os
 import warnings
 from typing import List, Optional, Tuple, Union
 
 from huggingface_hub import snapshot_download
-from sglang.srt.utils import is_multimodal_model
 from transformers import (
     AutoConfig,
     AutoProcessor,
     AutoTokenizer,
     PreTrainedTokenizer,
     PreTrainedTokenizerFast,
 )
 
+from sglang.srt.utils import is_multimodal_model
+
 
 def download_from_hf(model_path: str):
     if os.path.exists(model_path):
         return model_path
 
     return snapshot_download(model_path, allow_patterns=["*.json", "*.bin", "*.model"])
```

### Comparing `dblcsgen-0.2.6/sglang/srt/layers/context_flashattention_nopad.py` & `dblcsgen-0.2.7/sglang/srt/layers/context_flashattention_nopad.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Adapted from
 # https://github.com/ModelTC/lightllm/blob/f2a54f0912293f683bf1d1695fd12c4098a5bf82/lightllm/models/llama/triton_kernel/context_flashattention_nopad.py#L1
 import torch
 import triton
 import triton.language as tl
+
 from sglang.srt.utils import wrap_kernel_launcher
 
 CUDA_CAPABILITY = torch.cuda.get_device_capability()
 
 
 @triton.jit
 def _fwd_kernel(
```

### Comparing `dblcsgen-0.2.6/sglang/srt/layers/extend_attention.py` & `dblcsgen-0.2.7/sglang/srt/layers/extend_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 import triton
 import triton.language as tl
+
 from sglang.srt.layers.context_flashattention_nopad import context_attention_fwd
 from sglang.srt.utils import wrap_kernel_launcher
 
 CUDA_CAPABILITY = torch.cuda.get_device_capability()
 
 
 @triton.jit
```

### Comparing `dblcsgen-0.2.6/sglang/srt/layers/logits_processor.py` & `dblcsgen-0.2.7/sglang/srt/layers/logits_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import torch
-from sglang.srt.managers.router.model_runner import ForwardMode, InputMetadata
 from torch import nn
-from vllm.model_executor.parallel_utils.communication_op import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
     tensor_model_parallel_all_gather,
 )
 
+from sglang.srt.managers.router.model_runner import ForwardMode, InputMetadata
+
 
 class LogitsProcessor(nn.Module):
     def __init__(self, config):
         super().__init__()
         self.config = config
         self.tp_size = get_tensor_model_parallel_world_size()
 
@@ -37,34 +38,37 @@
 
     def _get_top_logprobs(self, all_logprobs, input_metadata: InputMetadata):
         if input_metadata.forward_mode == ForwardMode.DECODE:
             decode_top_logprobs = []
             for i in range(all_logprobs.shape[0]):
                 k = input_metadata.top_logprobs_nums[i]
                 t = all_logprobs[i].topk(k)
-                v_cpu = t.values.cpu().tolist()
-                p_cpu = t.indices.cpu().tolist()
+                v_cpu = t.values.tolist()
+                p_cpu = t.indices.tolist()
                 decode_top_logprobs.append(list(zip(v_cpu, p_cpu)))
             return None, decode_top_logprobs
         else:
             prefill_top_logprobs, decode_top_logprobs = [], []
             pt = 0
             # NOTE: the GPU-CPU overhead can be reduced
-            extend_seq_lens_cpu = input_metadata.extend_seq_lens
-            for i in range(len(input_metadata.extend_seq_lens)):
+            extend_seq_lens_cpu = input_metadata.extend_seq_lens.cpu().numpy()
+            for i in range(len(extend_seq_lens_cpu)):
                 if extend_seq_lens_cpu[i] == 0:
+                    prefill_top_logprobs.append([])
+                    decode_top_logprobs.append([])
                     continue
                 k = input_metadata.top_logprobs_nums[i]
                 t = all_logprobs[pt : pt + extend_seq_lens_cpu[i]].topk(k)
-                vs_cpu = t.values.cpu().tolist()
-                ps_cpu = t.indices.cpu().tolist()
+                vs_cpu = t.values.tolist()
+                ps_cpu = t.indices.tolist()
                 prefill_top_logprobs.append(
                     [list(zip(vs_cpu[j], ps_cpu[j])) for j in range(len(vs_cpu) - 1)]
                 )
                 decode_top_logprobs.append(list(zip(vs_cpu[-1], ps_cpu[-1])))
+                pt += extend_seq_lens_cpu[i]
             return prefill_top_logprobs, decode_top_logprobs
 
     def forward(self, input_ids, hidden_states, weight, input_metadata: InputMetadata):
         # Get last index for next token prediction, except for DECODE mode.
         last_index = None
         if input_metadata.forward_mode != ForwardMode.DECODE:
             last_index = (
@@ -93,27 +97,33 @@
                 all_logits = last_logits
             else:
                 all_logits = torch.matmul(hidden_states, weight.T)
                 if self.tp_size > 1:
                     all_logits = tensor_model_parallel_all_gather(all_logits)
                 all_logits = all_logits[:, : self.config.vocab_size]
 
-            all_logprobs = torch.log(torch.softmax(all_logits.float(), dim=-1) + 1e-6)
-
-            prefill_top_logprobs, decode_top_logprobs = self._get_top_logprobs(
-                all_logprobs, input_metadata
-            )
+            all_logprobs = all_logits.float()
+            del all_logits
+            all_logprobs[:] = torch.nn.functional.log_softmax(all_logprobs, dim=-1)
+
+            return_top_logprob = any(x > 0 for x in input_metadata.top_logprobs_nums)
+            if return_top_logprob:
+                prefill_top_logprobs, decode_top_logprobs = self._get_top_logprobs(
+                    all_logprobs, input_metadata
+                )
+            else:
+                prefill_top_logprobs = decode_top_logprobs = None
 
             if input_metadata.forward_mode == ForwardMode.DECODE:
                 last_logprobs = all_logprobs
                 return last_logits, (
                     None,
                     None,
-                    decode_top_logprobs,
                     None,
+                    decode_top_logprobs,
                     last_logprobs,
                 )
             else:
                 # Compute the logprobs for the last token of each request.
                 last_logprobs = all_logprobs[last_index]
 
                 # Compute the logprobs and normalized logprobs for the prefill tokens.
@@ -124,17 +134,17 @@
                 ]
 
                 normalized_prompt_logprobs = self._get_normalized_prompt_logprobs(
                     prefill_token_logprobs, input_metadata
                 )
                 return last_logits, (
                     prefill_token_logprobs,
+                    normalized_prompt_logprobs,
                     prefill_top_logprobs,
                     decode_top_logprobs,
-                    normalized_prompt_logprobs,
                     last_logprobs,
                 )
 
 
 if __name__ == "__main__":
     all_logprobs = torch.tensor(
         #       s                     s                s
```

### Comparing `dblcsgen-0.2.6/sglang/srt/layers/radix_attention.py` & `dblcsgen-0.2.7/sglang/srt/layers/radix_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import torch
+from torch import nn
+
 from sglang.srt.layers.context_flashattention_nopad import context_attention_fwd
 from sglang.srt.layers.extend_attention import extend_attention_fwd
 from sglang.srt.layers.token_attention import token_attention_fwd
 from sglang.srt.managers.router.model_runner import ForwardMode, InputMetadata
-from torch import nn
 
 
 class RadixAttention(nn.Module):
     def __init__(self, num_heads, head_dim, scaling, num_kv_heads, layer_id):
         super().__init__()
         self.tp_q_head_num = num_heads
         self.tp_k_head_num = num_kv_heads
```

### Comparing `dblcsgen-0.2.6/sglang/srt/layers/token_attention.py` & `dblcsgen-0.2.7/sglang/srt/layers/token_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Adapted from
 # https://github.com/ModelTC/lightllm/blob/f2a54f0912293f683bf1d1695fd12c4098a5bf82/lightllm/models/llama/triton_kernel/token_attention_nopad_att1.py
 # https://github.com/ModelTC/lightllm/blob/f2a54f0912293f683bf1d1695fd12c4098a5bf82/lightllm/models/llama/triton_kernel/token_attention_softmax_and_reducev.py
 import torch
 import triton
 import triton.language as tl
+
 from sglang.srt.managers.router.model_runner import global_server_args_dict
 from sglang.srt.utils import wrap_kernel_launcher
 
 if global_server_args_dict.get("attention_reduce_in_fp32", False):
     REDUCE_TRITON_TYPE = tl.float32
     REDUCE_TORCH_TYPE = torch.float32
 else:
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/detokenizer_manager.py` & `dblcsgen-0.2.7/sglang/srt/managers/detokenizer_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import asyncio
 
 import uvloop
 import zmq
 import zmq.asyncio
+
 from sglang.srt.hf_transformers_utils import get_tokenizer
 from sglang.srt.managers.io_struct import BatchStrOut, BatchTokenIDOut
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import get_exception_traceback
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
@@ -33,18 +34,21 @@
     async def handle_loop(self):
         while True:
             recv_obj = await self.recv_from_router.recv_pyobj()
 
             if isinstance(recv_obj, BatchTokenIDOut):
                 output_tokens = recv_obj.output_tokens
 
-                # TODO(lmzheng): handle skip_special_tokens per request
+                # TODO(lmzheng): handle skip_special_tokens/spaces_between_special_tokens per request
                 output_strs = self.tokenizer.batch_decode(
                     output_tokens,
                     skip_special_tokens=recv_obj.skip_special_tokens[0],
+                    spaces_between_special_tokens=recv_obj.spaces_between_special_tokens[
+                        0
+                    ],
                 )
 
                 # Trim stop str
                 # TODO(lmzheng): handle the case where multiple stop strs are hit
                 for i in range(len(output_strs)):
                     if recv_obj.hit_stop_str[i] is not None:
                         pos = output_strs[i].find(recv_obj.hit_stop_str[i])
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/io_struct.py` & `dblcsgen-0.2.7/sglang/srt/managers/io_struct.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 from sglang.srt.sampling_params import SamplingParams
 
 
 @dataclass
 class GenerateReqInput:
     # The input prompt
-    text: Union[List[str], str]
+    text: Optional[Union[List[str], str]] = None
+    # The token ids for text; one can either specify text or input_ids
+    input_ids: Optional[Union[List[List[int]], List[int]]] = None
     # The image input
     image_data: Optional[Union[List[str], str]] = None
     # The sampling_params
     sampling_params: Union[List[Dict], Dict] = None
     # The request id
     rid: Optional[Union[List[str], str]] = None
     # Whether to return logprobs
@@ -24,29 +26,39 @@
     # Whether to detokenize tokens in logprobs
     return_text_in_logprobs: bool = False
     # Whether to stream output
     stream: bool = False
     # TODO: make all parameters a Union[List[T], T] to allow for batched requests
 
     def post_init(self):
-        is_single = isinstance(self.text, str)
+
+        if self.text is None:
+            assert self.input_ids is not None, "Either text or input_ids should be provided"
+        else:
+            assert self.input_ids is None, "Either text or input_ids should be provided"
+
+        if self.text is not None:
+            is_single = isinstance(self.text, str)
+        else:
+            is_single = isinstance(self.input_ids[0], int)
+        self.is_single = is_single
 
         if is_single:
             if self.sampling_params is None:
                 self.sampling_params = {}
             if self.rid is None:
                 self.rid = uuid.uuid4().hex
             if self.return_logprob is None:
                 self.return_logprob = False
             if self.logprob_start_len is None:
                 self.logprob_start_len = 0
             if self.top_logprobs_num is None:
                 self.top_logprobs_num = 0
         else:
-            num = len(self.text)
+            num = len(self.text) if self.text is not None else len(self.input_ids)
 
             if self.image_data is None:
                 self.image_data = [None] * num
             elif not isinstance(self.image_data, list):
                 self.image_data = [self.image_data] * num
 
             if self.sampling_params is None:
@@ -93,14 +105,15 @@
 @dataclass
 class BatchTokenIDOut:
     rids: List[str]
     output_tokens: List[List[int]]
     output_and_jump_forward_strs: List[str]
     hit_stop_str: List[Optional[str]]
     skip_special_tokens: List[bool]
+    spaces_between_special_tokens: List[bool]
     meta_info: List[Dict]
     finished: List[bool]
 
 
 @dataclass
 class BatchStrOut:
     rids: List[str]
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/openai_protocol.py` & `dblcsgen-0.2.7/sglang/srt/openai_protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""pydantic models for OpenAI API protocol"""
 import time
 from typing import Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field
 from typing_extensions import Literal
 
 
@@ -15,29 +16,32 @@
 class UsageInfo(BaseModel):
     prompt_tokens: int = 0
     total_tokens: int = 0
     completion_tokens: Optional[int] = 0
 
 
 class CompletionRequest(BaseModel):
+    # Ordered by official OpenAI API documentation
+    # https://platform.openai.com/docs/api-reference/completions/create
     model: str
-    prompt: Union[str, List[str]]
-    suffix: Optional[str] = None
-    max_tokens: Optional[int] = 16
-    temperature: Optional[float] = 0.7
-    top_p: Optional[float] = 1.0
-    n: Optional[int] = 1
-    stream: Optional[bool] = False
-    logprobs: Optional[int] = None
+    prompt: Union[List[int], List[List[int]], str, List[str]]
+    best_of: Optional[int] = None
     echo: Optional[bool] = False
-    stop: Optional[Union[str, List[str]]] = Field(default_factory=list)
-    presence_penalty: Optional[float] = 0.0
     frequency_penalty: Optional[float] = 0.0
-    best_of: Optional[int] = None
     logit_bias: Optional[Dict[str, float]] = None
+    logprobs: Optional[int] = None
+    max_tokens: Optional[int] = 16
+    n: int = 1
+    presence_penalty: Optional[float] = 0.0
+    seed: Optional[int] = None
+    stop: Optional[Union[str, List[str]]] = Field(default_factory=list)
+    stream: Optional[bool] = False
+    suffix: Optional[str] = None
+    temperature: Optional[float] = 1.0
+    top_p: Optional[float] = 1.0
     user: Optional[str] = None
 
     # Extra parameters for SRT backend only and will be ignored by OpenAI models.
     regex: Optional[str] = None
 
 
 class CompletionResponseChoice(BaseModel):
@@ -103,41 +107,52 @@
 
 
 ChatCompletionMessageParam = Union[
     ChatCompletionMessageGenericParam, ChatCompletionMessageUserParam
 ]
 
 
+class ResponseFormat(BaseModel):
+    # type must be "json_object" or "text"
+    type: Literal["text", "json_object"]
+
+
 class ChatCompletionRequest(BaseModel):
+    # Ordered by official OpenAI API documentation
+    # https://platform.openai.com/docs/api-reference/chat/create
+    messages: List[ChatCompletionMessageParam]
     model: str
-    messages: Union[str, List[ChatCompletionMessageParam]]
-    temperature: Optional[float] = 0.7
-    top_p: Optional[float] = 1.0
+    frequency_penalty: Optional[float] = 0.0
+    logit_bias: Optional[Dict[str, float]] = None
+    logprobs: Optional[bool] = False
+    top_logprobs: Optional[int] = None
+    max_tokens: Optional[int] = None
     n: Optional[int] = 1
-    max_tokens: Optional[int] = 16
+    presence_penalty: Optional[float] = 0.0
+    response_format: Optional[ResponseFormat] = None
+    seed: Optional[int] = None
     stop: Optional[Union[str, List[str]]] = Field(default_factory=list)
     stream: Optional[bool] = False
-    presence_penalty: Optional[float] = 0.0
-    frequency_penalty: Optional[float] = 0.0
-    logit_bias: Optional[Dict[str, float]] = None
+    temperature: Optional[float] = 0.7
+    top_p: Optional[float] = 1.0
     user: Optional[str] = None
-    best_of: Optional[int] = None
 
     # Extra parameters for SRT backend only and will be ignored by OpenAI models.
     regex: Optional[str] = None
 
 
 class ChatMessage(BaseModel):
     role: Optional[str] = None
     content: Optional[str] = None
 
 
 class ChatCompletionResponseChoice(BaseModel):
     index: int
     message: ChatMessage
+    logprobs: Optional[LogProbs] = None
     finish_reason: Optional[str] = None
 
 
 class ChatCompletionResponse(BaseModel):
     id: str
     object: str = "chat.completion"
     created: int = Field(default_factory=lambda: int(time.time()))
@@ -150,16 +165,17 @@
     role: Optional[str] = None
     content: Optional[str] = None
 
 
 class ChatCompletionResponseStreamChoice(BaseModel):
     index: int
     delta: DeltaMessage
+    logprobs: Optional[LogProbs] = None
     finish_reason: Optional[str] = None
 
 
 class ChatCompletionStreamResponse(BaseModel):
     id: str
     object: str = "chat.completion.chunk"
     created: int = Field(default_factory=lambda: int(time.time()))
     model: str
-    choices: List[ChatCompletionResponseStreamChoice]
+    choices: List[ChatCompletionResponseStreamChoice]
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/infer_batch.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/infer_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,71 +1,76 @@
 from dataclasses import dataclass
-from enum import Enum, auto
+from enum import IntEnum, auto
 from typing import List
 
 import numpy as np
 import torch
+
 from sglang.srt.managers.router.radix_cache import RadixCache
 from sglang.srt.memory_pool import ReqToTokenPool, TokenToKVPool
 
 
-class ForwardMode(Enum):
+class ForwardMode(IntEnum):
     PREFILL = auto()
     EXTEND = auto()
     DECODE = auto()
 
 
-class FinishReason(Enum):
-    LENGTH = auto()
+class FinishReason(IntEnum):
     EOS_TOKEN = auto()
+    LENGTH = auto()
     STOP_STR = auto()
 
 
 class Req:
     def __init__(self, rid, input_text, input_ids):
         self.rid = rid
         self.input_text = input_text
         self.input_ids = input_ids
         self.output_ids = []
 
         # Since jump forward may retokenize the prompt with partial outputs,
         # we maintain the original prompt length to report the correct usage.
         self.prompt_tokens = len(input_ids)
+
         # The number of decoded tokens for token usage report. Note that
         # this does not include the jump forward tokens.
         self.completion_tokens_wo_jump_forward = 0
 
         # For vision input
         self.pixel_values = None
         self.image_size = None
         self.image_offset = 0
         self.pad_value = None
 
+        # Sampling parameters
         self.sampling_params = None
-        self.return_logprob = False
-        self.logprob_start_len = 0
-        self.top_logprobs_num = 0
         self.stream = False
 
+        # Check finish
         self.tokenizer = None
         self.finished = False
         self.finish_reason = None
         self.hit_stop_str = None
 
         self.extend_input_len = 0
         self.prefix_indices = []
         self.last_node = None
 
+        # Logprobs
+        self.return_logprob = False
+        self.logprob_start_len = 0
+        self.top_logprobs_num = 0
+        self.normalized_prompt_logprob = None
         self.prefill_token_logprobs = None
         self.decode_token_logprobs = None
-        self.normalized_prompt_logprob = None
         self.prefill_top_logprobs = None
         self.decode_top_logprobs = None
 
-        # For constrained decoding
+        # Constrained decoding
         self.regex_fsm = None
         self.regex_fsm_state = 0
         self.jump_forward_map = None
         self.output_and_jump_forward_str = ""
 
     def max_new_tokens(self):
         return self.sampling_params.max_new_tokens
@@ -76,14 +81,17 @@
         # there should be a leading space.
         first_token = self.tokenizer.convert_ids_to_tokens(self.output_ids[0])
         first_token = (
             first_token.decode() if isinstance(first_token, bytes) else first_token
         )
         if first_token.startswith("▁"):
             old_output_str = " " + old_output_str
+        if self.input_text is None:
+            # TODO(lmzheng): This can be wrong. Check with Liangsheng.
+            self.input_text = self.tokenizer.decode(self.input_ids)
         new_input_string = (
             self.input_text
             + self.output_and_jump_forward_str
             + old_output_str
             + jump_forward_str
         )
         new_input_ids = self.tokenizer.encode(new_input_string)
@@ -160,16 +168,16 @@
     prefix_lens: torch.Tensor = None
     position_ids_offsets: torch.Tensor = None
     out_cache_loc: torch.Tensor = None
     out_cache_cont_start: torch.Tensor = None
     out_cache_cont_end: torch.Tensor = None
 
     # for processing logprobs
-    top_logprobs_nums: List[int] = None
     return_logprob: bool = False
+    top_logprobs_nums: List[int] = None
 
     # for multimodal
     pixel_values: List[torch.Tensor] = None
     image_sizes: List[List[int]] = None
     image_offsets: List[int] = None
 
     # other arguments for control
@@ -231,17 +239,16 @@
         position_ids_offsets = torch.zeros((bs,), dtype=torch.int32, device=device)
 
         # Alloc mem
         seq_lens, prefix_lens = np.array(seq_lens), np.array(prefix_lens)
         extend_num_tokens = seq_lens.sum() - prefix_lens.sum()
         out_cache_loc = self.token_to_kv_pool.alloc(extend_num_tokens)
         if out_cache_loc is None:
-            if not self.tree_cache.disable:
-                self.tree_cache.evict(extend_num_tokens, self.token_to_kv_pool.free)
-                out_cache_loc = self.token_to_kv_pool.alloc(extend_num_tokens)
+            self.tree_cache.evict(extend_num_tokens, self.token_to_kv_pool.dec_refs)
+            out_cache_loc = self.token_to_kv_pool.alloc(extend_num_tokens)
 
             if out_cache_loc is None:
                 print("Prefill out of memory. This should never happen.")
                 self.tree_cache.pretty_print()
                 exit()
 
         pt = 0
@@ -302,50 +309,50 @@
         self.logit_bias = logit_bias
 
     def check_decode_mem(self):
         bs = len(self.reqs)
         if self.token_to_kv_pool.available_size() >= bs:
             return True
 
-        if not self.tree_cache.disable:
-            self.tree_cache.evict(bs, self.token_to_kv_pool.free)
+        self.tree_cache.evict(bs, self.token_to_kv_pool.dec_refs)
+
         if self.token_to_kv_pool.available_size() >= bs:
             return True
 
         return False
 
     def retract_decode(self):
         sorted_indices = [i for i in range(len(self.reqs))]
         sorted_indices.sort(
             key=lambda i: (len(self.reqs[i].output_ids), -len(self.reqs[i].input_ids)),
             reverse=True,
         )
 
         retracted_reqs = []
-        seq_lens_np = self.seq_lens.cpu().numpy()
-        req_pool_indices_np = self.req_pool_indices.cpu().numpy()
+        seq_lens_cpu = self.seq_lens.cpu().numpy()
+        req_pool_indices_cpu = self.req_pool_indices.cpu().numpy()
         while self.token_to_kv_pool.available_size() < len(self.reqs):
             idx = sorted_indices.pop()
             req = self.reqs[idx]
             retracted_reqs.append(req)
 
-            self.tree_cache.dec_ref_counter(req.last_node)
+            # TODO: apply more fine-grained retraction
+            last_uncached_pos = len(req.prefix_indices)
+            token_indices = self.req_to_token_pool.req_to_token[
+                req_pool_indices_cpu[idx]
+            ][last_uncached_pos : seq_lens_cpu[idx]]
+            self.token_to_kv_pool.dec_refs(token_indices)
+
+            self.tree_cache.dec_lock_ref(req.last_node)
             req.prefix_indices = None
             req.last_node = None
             req.extend_input_len = 0
             req.output_ids = []
             req.regex_fsm_state = 0
 
-            # TODO: apply more fine-grained retraction
-
-            token_indices = self.req_to_token_pool.req_to_token[
-                req_pool_indices_np[idx]
-            ][: seq_lens_np[idx]]
-            self.token_to_kv_pool.free(token_indices)
-
         self.filter_batch(sorted_indices)
 
         return retracted_reqs
 
     def check_for_jump_forward(self):
         jump_forward_reqs = []
         filter_indices = [i for i in range(len(self.reqs))]
@@ -356,28 +363,26 @@
             if req.jump_forward_map is not None:
                 res = req.jump_forward_map.jump_forward(req.regex_fsm_state)
                 if res is not None:
                     jump_forward_str, next_state = res
                     if len(jump_forward_str) <= 1:
                         continue
 
-                    # insert the old request into tree_cache
-                    token_ids_in_memory = tuple(req.input_ids + req.output_ids)[:-1]
                     if req_pool_indices_cpu is None:
-                        req_pool_indices_cpu = self.req_pool_indices.cpu().tolist()
-                    req_pool_idx = req_pool_indices_cpu[i]
-                    indices = self.req_to_token_pool.req_to_token[
-                        req_pool_idx, : len(token_ids_in_memory)
-                    ]
-                    prefix_len = self.tree_cache.insert(
-                        token_ids_in_memory, indices.clone()
+                        req_pool_indices_cpu = self.req_pool_indices.tolist()
+
+                    # insert the old request into tree_cache
+                    self.tree_cache.cache_req(
+                        token_ids=tuple(req.input_ids + req.output_ids)[:-1],
+                        last_uncached_pos=len(req.prefix_indices),
+                        req_pool_idx=req_pool_indices_cpu[i],
                     )
-                    self.token_to_kv_pool.free(indices[:prefix_len])
-                    self.req_to_token_pool.free(req_pool_idx)
-                    self.tree_cache.dec_ref_counter(req.last_node)
+
+                    # unlock the last node
+                    self.tree_cache.dec_lock_ref(req.last_node)
 
                     # jump-forward
                     req.jump_forward_and_retokenize(jump_forward_str, next_state)
 
                     jump_forward_reqs.append(req)
                     filter_indices.remove(i)
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/manager.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import logging
 
 import uvloop
 import zmq
 import zmq.asyncio
-from sglang.srt.backend_config import GLOBAL_BACKEND_CONFIG
+
+from sglang import global_config
 from sglang.srt.managers.router.model_rpc import ModelRpcClient
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import get_exception_traceback
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 
@@ -25,15 +26,15 @@
         )
 
         # Init status
         self.model_client = model_client
         self.recv_reqs = []
 
         # Init some configs
-        self.extend_dependency_time = GLOBAL_BACKEND_CONFIG.extend_dependency_time
+        self.request_dependency_time = global_config.request_dependency_time
 
     async def loop_for_forward(self):
         while True:
             next_step_input = list(self.recv_reqs)
             self.recv_reqs = []
             out_pyobjs = await self.model_client.step(next_step_input)
 
@@ -41,17 +42,17 @@
                 self.send_to_detokenizer.send_pyobj(obj)
 
             # async sleep for receiving the subsequent request and avoiding cache miss
             slept = False
             if len(out_pyobjs) != 0:
                 has_finished = any([obj.finished for obj in out_pyobjs])
                 if has_finished:
-                    if self.extend_dependency_time > 0:
+                    if self.request_dependency_time > 0:
                         slept = True
-                        await asyncio.sleep(self.extend_dependency_time)
+                        await asyncio.sleep(self.request_dependency_time)
 
             if not slept:
                 await asyncio.sleep(0.0006)
 
     async def loop_for_recv_requests(self):
         while True:
             recv_req = await self.recv_from_tokenizer.recv_pyobj()
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/model_rpc.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/model_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import List
 
 import rpyc
 import torch
 from rpyc.utils.classic import obtain
 from rpyc.utils.server import ThreadedServer
+try:
+    from vllm.logger import _default_handler as vllm_default_logger
+except ImportError:
+    from vllm.logger import logger as vllm_default_logger
+
 from sglang.srt.constrained.fsm_cache import FSMCache
 from sglang.srt.constrained.jump_forward import JumpForwardCache
 from sglang.srt.hf_transformers_utils import get_processor, get_tokenizer
 from sglang.srt.managers.io_struct import (
     BatchTokenIDOut,
     FlushCacheReq,
     TokenizedGenerateReqInput,
@@ -26,17 +31,19 @@
 from sglang.srt.server_args import PortArgs, ServerArgs
 from sglang.srt.utils import (
     get_exception_traceback,
     get_int_token_logit_bias,
     is_multimodal_model,
     set_random_seed,
 )
-from vllm.logger import _default_handler as vllm_default_handler
+
 
 logger = logging.getLogger("model_rpc")
+vllm_default_logger.setLevel(logging.WARN)
+logging.getLogger("vllm.utils").setLevel(logging.WARN)
 
 
 class ModelRpcServer:
     def __init__(
         self,
         tp_rank: int,
         server_args: ServerArgs,
@@ -45,26 +52,23 @@
         server_args, port_args = [obtain(x) for x in [server_args, port_args]]
 
         # Copy arguments
         self.tp_rank = tp_rank
         self.tp_size = server_args.tp_size
         self.schedule_heuristic = server_args.schedule_heuristic
         self.disable_regex_jump_forward = server_args.disable_regex_jump_forward
-        vllm_default_handler.setLevel(
-            level=getattr(logging, server_args.log_level.upper())
-        )
 
         # Init model and tokenizer
         self.model_config = ModelConfig(
             server_args.model_path,
             server_args.trust_remote_code,
             context_length=server_args.context_length,
         )
 
-        # for model end global settings
+        # For model end global settings
         server_args_dict = {
             "enable_flashinfer": server_args.enable_flashinfer,
             "attention_reduce_in_fp32": server_args.attention_reduce_in_fp32,
         }
 
         self.model_runner = ModelRunner(
             model_config=self.model_config,
@@ -105,18 +109,23 @@
         set_random_seed(server_args.random_seed)
         logger.info(
             f"Rank {self.tp_rank}: "
             f"max_total_num_token={self.max_total_num_token}, "
             f"max_prefill_num_token={self.max_prefill_num_token}, "
             f"context_len={self.model_config.context_len}, "
         )
-        logger.info(server_args.get_optional_modes_logging())
+        if self.tp_rank == 0:
+            logger.info(f"server_args: {server_args.print_mode_args()}")
 
         # Init cache
-        self.tree_cache = RadixCache(server_args.disable_radix_cache)
+        self.tree_cache = RadixCache(
+            req_to_token_pool=self.model_runner.req_to_token_pool,
+            token_to_kv_pool=self.model_runner.token_to_kv_pool,
+            disable=server_args.disable_radix_cache,
+        )
         self.tree_cache_metrics = {"total": 0, "hit": 0}
         self.scheduler = Scheduler(
             self.schedule_heuristic,
             self.max_num_running_seq,
             self.max_prefill_num_token,
             self.max_total_num_token,
             self.tree_cache,
@@ -126,14 +135,16 @@
 
         # Init running status
         self.forward_queue: List[Req] = []
         self.running_batch: Batch = None
         self.out_pyobjs = []
         self.decode_forward_ct = 0
         self.stream_interval = server_args.stream_interval
+        self.num_generated_tokens = 0
+        self.last_stats_tic = time.time()
 
         # Init the FSM cache for constrained generation
         self.regex_fsm_cache = FSMCache(
             server_args.tokenizer_path,
             {
                 "tokenizer_mode": server_args.tokenizer_mode,
                 "trust_remote_code": server_args.trust_remote_code,
@@ -155,15 +166,15 @@
             self.regex_fsm_cache.reset()
             self.req_to_token_pool.clear()
             self.token_to_kv_pool.clear()
             torch.cuda.empty_cache()
             logger.info("Cache flushed successfully!")
         else:
             warnings.warn(
-                "Cache not flushed because there are pending requests. "
+                f"Cache not flushed because there are pending requests. "
                 f"#queue-req: {len(self.forward_queue)}, "
                 f"#running-req: {0 if self.running_batch is None else len(self.running_batch.reqs)}"
             )
 
     def exposed_step(self, recv_reqs):
         if self.tp_size != 1:
             recv_reqs = obtain(recv_reqs)
@@ -192,24 +203,27 @@
     def forward_step(self):
         new_batch = self.get_new_fill_batch()
 
         if new_batch is not None:
             # Run new fill batch
             self.forward_fill_batch(new_batch)
 
+            self.cache_filled_batch(new_batch)
+
             if not new_batch.is_empty():
                 if self.running_batch is None:
                     self.running_batch = new_batch
                 else:
                     self.running_batch.merge(new_batch)
         else:
             # Run decode batch
             if self.running_batch is not None:
                 # Run a few decode batches continuously for reducing overhead
                 for _ in range(10):
+                    self.num_generated_tokens += len(self.running_batch.reqs)
                     self.forward_decode_batch(self.running_batch)
 
                     if self.running_batch.is_empty():
                         self.running_batch = None
                         break
 
                     if self.out_pyobjs and self.running_batch.reqs[0].stream:
@@ -217,18 +231,22 @@
 
                     if self.running_batch is not None and self.tp_rank == 0:
                         if self.decode_forward_ct % 40 == 0:
                             num_used = self.max_total_num_token - (
                                 self.token_to_kv_pool.available_size()
                                 + self.tree_cache.evictable_size()
                             )
+                            throuhgput = self.num_generated_tokens / (time.time() - self.last_stats_tic)
+                            self.num_generated_tokens = 0
+                            self.last_stats_tic = time.time()
                             logger.info(
                                 f"#running-req: {len(self.running_batch.reqs)}, "
                                 f"#token: {num_used}, "
                                 f"token usage: {num_used / self.max_total_num_token:.2f}, "
+                                f"gen throughput (token/s): {throuhgput:.2f}, "
                                 f"#queue-req: {len(self.forward_queue)}"
                             )
             else:
                 # check the available size
                 available_size = (
                     self.token_to_kv_pool.available_size()
                     + self.tree_cache.evictable_size()
@@ -333,28 +351,27 @@
 
             if (
                 req.extend_input_len + req.max_new_tokens() + new_batch_total_tokens
                 < available_size
                 and req.extend_input_len + new_batch_input_tokens
                 < self.max_prefill_num_token
             ):
-                delta = self.tree_cache.inc_ref_counter(req.last_node)
+                delta = self.tree_cache.inc_lock_ref(req.last_node)
                 available_size += delta
 
                 if not (
                     req.extend_input_len + req.max_new_tokens() + new_batch_total_tokens
                     < available_size
                 ):
-                    # Undo the insertion
-                    delta = self.tree_cache.dec_ref_counter(req.last_node)
+                    # Undo locking
+                    delta = self.tree_cache.dec_lock_ref(req.last_node)
                     available_size += delta
                     break
                 else:
                     # Add this request to the running batch
-                    self.token_to_kv_pool.add_refs(req.prefix_indices)
                     can_run_list.append(req)
                     new_batch_total_tokens += (
                         req.extend_input_len + req.max_new_tokens()
                     )
                     new_batch_input_tokens += req.extend_input_len
             else:
                 break
@@ -377,20 +394,20 @@
                 f"new fill batch. #seq: {len(can_run_list)}. "
                 f"#cached_token: {hit_tokens}. "
                 f"#new_token: {new_batch_input_tokens}. "
                 f"#remaining_req: {len(self.forward_queue) - len(can_run_list)}. "
                 f"#running_req: {running_req}. "
                 f"tree_cache_hit_rate: {100.0 * tree_cache_hit_rate:.2f}%."
             )
-            logger.debug(
-                f"fsm_cache_hit_rate: {100.0 * self.regex_fsm_cache.get_cache_hit_rate():.2f}%. "
-                f"fsm_cache_avg_init_time: {self.regex_fsm_cache.get_avg_init_time():.2f}s. "
-                f"ff_cache_hit_rate: {100.0 * self.jump_forward_cache.get_cache_hit_rate():.2f}%. "
-                f"ff_cache_avg_init_time: {self.jump_forward_cache.get_avg_init_time():.2f}s. "
-            )
+            #logger.debug(
+            #    f"fsm_cache_hit_rate: {100.0 * self.regex_fsm_cache.get_cache_hit_rate():.2f}%. "
+            #    f"fsm_cache_avg_init_time: {self.regex_fsm_cache.get_avg_init_time():.2f}s. "
+            #    f"ff_cache_hit_rate: {100.0 * self.jump_forward_cache.get_cache_hit_rate():.2f}%. "
+            #    f"ff_cache_avg_init_time: {self.jump_forward_cache.get_avg_init_time():.2f}s. "
+            #)
 
         new_batch = Batch.init_new(
             can_run_list,
             self.req_to_token_pool,
             self.token_to_kv_pool,
             self.tree_cache,
         )
@@ -399,78 +416,88 @@
 
     def forward_fill_batch(self, batch: Batch):
         # Build batch tensors
         batch.prepare_for_extend(
             self.model_config.vocab_size, self.int_token_logit_bias
         )
 
-        prefill_token_logprobs = None
         if batch.extend_num_tokens != 0:
             # Forward
             logits, (
                 prefill_token_logprobs,
+                normalized_prompt_logprobs,
                 prefill_top_logprobs,
                 decode_top_logprobs,
-                normalized_prompt_logprobs,
                 last_logprobs,
             ) = self.model_runner.forward(batch, ForwardMode.EXTEND)
             if prefill_token_logprobs is not None:
-                prefill_token_logprobs = prefill_token_logprobs.cpu().tolist()
-                normalized_prompt_logprobs = normalized_prompt_logprobs.cpu().tolist()
+                prefill_token_logprobs = prefill_token_logprobs.tolist()
+                normalized_prompt_logprobs = normalized_prompt_logprobs.tolist()
 
             next_token_ids, _ = batch.sample(logits)
-            next_token_ids = next_token_ids.cpu().tolist()
+
+            # Only transfer the selected logprobs of the next token to CPU to reduce overhead.
+            if last_logprobs is not None:
+                last_token_logprobs = (
+                    last_logprobs[
+                        torch.arange(len(batch.reqs), device=next_token_ids.device),
+                        next_token_ids].tolist()
+                )
+
+            next_token_ids = next_token_ids.tolist()
         else:
             next_token_ids = [self.tokenizer.eos_token_id] * len(batch.reqs)
-            (
-                logits,
-                prefill_token_logprobs,
-                normalized_prompt_logprobs,
-                last_logprobs,
-            ) = (None,) * 4
-
-        # Only batch transfer the selected logprobs of the next token to CPU to reduce overhead.
-        reqs = batch.reqs
-        last_token_logprobs = None
-        if last_logprobs is not None:
-            last_token_logprobs = (
-                last_logprobs[torch.arange(len(reqs)), next_token_ids].cpu().tolist()
-            )
 
         # Check finish condition
         pt = 0
-        for i, req in enumerate(reqs):
+        for i, req in enumerate(batch.reqs):
             req.completion_tokens_wo_jump_forward += 1
             req.output_ids = [next_token_ids[i]]
             req.check_finished()
 
-            if prefill_token_logprobs is not None:
+            if req.return_logprob:
+                req.normalized_prompt_logprob = normalized_prompt_logprobs[i]
+
                 # If logprob_start_len > 0, then first logprob_start_len prompt tokens will be ignored.
                 req.prefill_token_logprobs = list(
                     zip(
                         prefill_token_logprobs[pt : pt + req.extend_input_len - 1],
                         req.input_ids[-req.extend_input_len + 1 :],
                     )
                 )
                 if req.logprob_start_len == 0:
                     req.prefill_token_logprobs = [
                         (None, req.input_ids[0])
                     ] + req.prefill_token_logprobs
                 req.decode_token_logprobs = [
                     (last_token_logprobs[i], next_token_ids[i])
                 ]
+
+            if req.top_logprobs_num > 0:
                 req.prefill_top_logprobs = prefill_top_logprobs[i]
                 if req.logprob_start_len == 0:
                     req.prefill_top_logprobs = [None] + req.prefill_top_logprobs
                 req.decode_top_logprobs = [decode_top_logprobs[i]]
-                req.normalized_prompt_logprob = normalized_prompt_logprobs[i]
-                pt += req.extend_input_len
+
+            pt += req.extend_input_len
 
         self.handle_finished_requests(batch)
 
+    def cache_filled_batch(self, batch: Batch):
+        req_pool_indices_cpu = batch.req_pool_indices.cpu().tolist()
+        for i, req in enumerate(batch.reqs):
+            new_prefix_indices, new_last_node = self.tree_cache.cache_req(
+                token_ids=tuple(req.input_ids + req.output_ids)[:-1],
+                last_uncached_pos=len(req.prefix_indices),
+                req_pool_idx=req_pool_indices_cpu[i],
+                del_in_memory_pool=False,
+                old_last_node=req.last_node,
+            )
+            req.prefix_indices, req.last_node = new_prefix_indices, new_last_node
+
     def forward_decode_batch(self, batch: Batch):
         # check if decode out of memory
         if not batch.check_decode_mem():
             old_ratio = self.new_token_ratio
             self.new_token_ratio = min(old_ratio + self.new_token_ratio_step[1], 1.0)
 
             retracted_reqs = batch.retract_decode()
@@ -508,46 +535,51 @@
                 return
 
         # Update batch tensors
         self.decode_forward_ct = (self.decode_forward_ct + 1) % (1 << 30)
         batch.prepare_for_decode()
 
         # Forward
-        logits, (_, _, decode_top_logprobs, _, last_logprobs) = (
-            self.model_runner.forward(batch, ForwardMode.DECODE)
-        )
+        logits, (
+            _,
+            _,
+            _,
+            decode_top_logprobs,
+            last_logprobs,
+        ) = self.model_runner.forward(batch, ForwardMode.DECODE)
         next_token_ids, _ = batch.sample(logits)
-        next_token_ids = next_token_ids.cpu().tolist()
+        next_token_ids = next_token_ids.tolist()
 
         # Only batch transfer the selected logprobs of the next token to CPU to reduce overhead.
-        reqs = batch.reqs
-        new_token_logprobs = None
         if last_logprobs is not None:
             new_token_logprobs = last_logprobs[
-                torch.arange(len(reqs)), next_token_ids
+                torch.arange(len(batch.reqs)), next_token_ids
             ].tolist()
 
         # Check finish condition
-        for i, (req, next_token_id) in enumerate(zip(reqs, next_token_ids)):
+        for i, (req, next_token_id) in enumerate(zip(batch.reqs, next_token_ids)):
             req.completion_tokens_wo_jump_forward += 1
             req.output_ids.append(next_token_id)
             req.check_finished()
 
-            if new_token_logprobs is not None:
+            if req.return_logprob:
                 req.decode_token_logprobs.append((new_token_logprobs[i], next_token_id))
+
+            if req.top_logprobs_num > 0:
                 req.decode_top_logprobs.append(decode_top_logprobs[i])
 
         self.handle_finished_requests(batch)
 
     def handle_finished_requests(self, batch: Batch):
         output_rids = []
         output_tokens = []
         output_and_jump_forward_strs = []
         output_hit_stop_str = []
         output_skip_special_tokens = []
+        output_spaces_between_special_tokens = []
         output_meta_info = []
         output_finished = []
         finished_indices = []
         unfinished_indices = []
         for i, req in enumerate(batch.reqs):
             if req.finished:
                 finished_indices.append(i)
@@ -566,21 +598,26 @@
                 output_rids.append(req.rid)
                 output_tokens.append(req.output_ids)
                 output_and_jump_forward_strs.append(req.output_and_jump_forward_str)
                 output_hit_stop_str.append(req.hit_stop_str)
                 output_skip_special_tokens.append(
                     req.sampling_params.skip_special_tokens
                 )
+                output_spaces_between_special_tokens.append(
+                    req.sampling_params.spaces_between_special_tokens
+                )
 
                 meta_info = {
                     "prompt_tokens": req.prompt_tokens,
                     "completion_tokens": len(req.input_ids)
                     + len(req.output_ids)
                     - req.prompt_tokens,
                     "completion_tokens_wo_jump_forward": req.completion_tokens_wo_jump_forward,
+                    "finish_reason": str(req.finish_reason),  # FIXME: convert to the correct string
+                    "hit_stop_str": req.hit_stop_str,
                 }
                 if req.return_logprob:
                     (
                         meta_info["prefill_token_logprobs"],
                         meta_info["decode_token_logprobs"],
                         meta_info["prefill_top_logprobs"],
                         meta_info["decode_top_logprobs"],
@@ -600,36 +637,33 @@
             self.out_pyobjs.append(
                 BatchTokenIDOut(
                     output_rids,
                     output_tokens,
                     output_and_jump_forward_strs,
                     output_hit_stop_str,
                     output_skip_special_tokens,
+                    output_spaces_between_special_tokens,
                     output_meta_info,
                     output_finished,
                 )
             )
 
         # Remove finished reqs
         if finished_indices:
             # Update radix cache
-            req_pool_indices_cpu = batch.req_pool_indices.cpu().tolist()
+            req_pool_indices_cpu = batch.req_pool_indices.tolist()
             for i in finished_indices:
                 req = batch.reqs[i]
-                req_pool_idx = req_pool_indices_cpu[i]
-                token_ids = tuple(req.input_ids + req.output_ids)
-                seq_len = len(token_ids) - 1
-                indices = self.req_to_token_pool.req_to_token[req_pool_idx, :seq_len]
-                prefix_len = self.tree_cache.insert(
-                    token_ids[:seq_len], indices.clone()
+                self.tree_cache.cache_req(
+                    token_ids=tuple(req.input_ids + req.output_ids)[:-1],
+                    last_uncached_pos=len(req.prefix_indices),
+                    req_pool_idx=req_pool_indices_cpu[i],
                 )
 
-                self.token_to_kv_pool.free(indices[:prefix_len])
-                self.req_to_token_pool.free(req_pool_idx)
-                self.tree_cache.dec_ref_counter(req.last_node)
+                self.tree_cache.dec_lock_ref(req.last_node)
 
             # Update batch tensors
             if unfinished_indices:
                 batch.filter_batch(unfinished_indices)
             else:
                 batch.reqs = []
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/model_runner.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/model_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import pkgutil
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import List
 
 import numpy as np
 import torch
-from sglang.srt.managers.router.infer_batch import Batch, ForwardMode
-from sglang.srt.memory_pool import ReqToTokenPool, TokenToKVPool
-from sglang.srt.utils import is_multimodal_model
-from sglang.utils import get_available_gpu_memory
 from vllm.model_executor.layers.quantization.awq import AWQConfig
 from vllm.model_executor.layers.quantization.gptq import GPTQConfig
 from vllm.model_executor.layers.quantization.marlin import MarlinConfig
-from vllm.model_executor.model_loader import _set_default_torch_dtype
-from vllm.model_executor.parallel_utils.parallel_state import initialize_model_parallel
+from vllm.model_executor.model_loader.utils import set_default_torch_dtype
+from vllm.distributed import initialize_model_parallel
+
+from sglang.srt.managers.router.infer_batch import Batch, ForwardMode
+from sglang.srt.memory_pool import ReqToTokenPool, TokenToKVPool
+from sglang.srt.utils import is_multimodal_model, get_available_gpu_memory
+
 
 QUANTIZATION_CONFIG_MAPPING = {
     "awq": AWQConfig,
     "gptq": GPTQConfig,
     "marlin": MarlinConfig,
 }
 
 logger = logging.getLogger("model_runner")
 
-
 # for server args in model endpoints
-global_server_args_dict: dict = None
+global_server_args_dict = {}
 
 
 @lru_cache()
 def import_model_classes():
     model_arch_name_to_cls = {}
     package_name = "sglang.srt.models"
     package = importlib.import_module(package_name)
@@ -82,16 +82,16 @@
     max_extend_len: int = 0
 
     out_cache_loc: torch.Tensor = None
     out_cache_cont_start: torch.Tensor = None
     out_cache_cont_end: torch.Tensor = None
 
     other_kv_index: torch.Tensor = None
-    top_logprobs_nums: List[int] = None
     return_logprob: bool = False
+    top_logprobs_nums: List[int] = None
 
     # for flashinfer
     qo_indptr: torch.Tensor = None
     kv_indptr: torch.Tensor = None
     kv_indices: torch.Tensor = None
     kv_last_page_len: torch.Tensor = None
     prefill_wrapper = None
@@ -103,26 +103,28 @@
             BatchPrefillWithPagedKVCacheWrapper,
         )
 
         self.kv_indptr = torch.zeros(
             (self.batch_size + 1,), dtype=torch.int32, device="cuda"
         )
         self.kv_indptr[1:] = torch.cumsum(self.seq_lens, dim=0)
+        self.kv_last_page_len = torch.ones(
+            (self.batch_size,), dtype=torch.int32, device="cuda"
+        )
+        req_pool_indices_cpu = self.req_pool_indices.cpu().numpy()
+        seq_lens_cpu = self.seq_lens.cpu().numpy()
         self.kv_indices = torch.cat(
             [
                 self.req_to_token_pool.req_to_token[
-                    self.req_pool_indices[i].item(), : self.seq_lens[i].item()
+                    req_pool_indices_cpu[i], : seq_lens_cpu[i]
                 ]
                 for i in range(self.batch_size)
             ],
             dim=0,
         ).contiguous()
-        self.kv_last_page_len = torch.ones(
-            (self.batch_size,), dtype=torch.int32, device="cuda"
-        )
 
         workspace_buffer = torch.empty(
             32 * 1024 * 1024, dtype=torch.int8, device="cuda"
         )
         if (
             self.forward_mode == ForwardMode.PREFILL
             or self.forward_mode == ForwardMode.EXTEND
@@ -137,24 +139,17 @@
             args = [
                 self.qo_indptr,
                 self.kv_indptr,
                 self.kv_indices,
                 self.kv_last_page_len,
                 self.model_runner.model_config.num_attention_heads // tp_size,
                 self.model_runner.model_config.num_key_value_heads // tp_size,
+                self.model_runner.model_config.head_dim
             ]
 
-            # flashinfer >= 0.0.3
-            # FIXME: Drop this when flashinfer updates to 0.0.4
-            if (
-                len(inspect.signature(self.prefill_wrapper.begin_forward).parameters)
-                == 7
-            ):
-                args.append(self.model_runner.model_config.head_dim)
-
             self.prefill_wrapper.begin_forward(*args)
         else:
             self.decode_wrapper = BatchDecodeWithPagedKVCacheWrapper(
                 workspace_buffer, "NHD"
             )
             self.decode_wrapper.begin_forward(
                 self.kv_indptr,
@@ -198,23 +193,23 @@
 
         if forward_mode == ForwardMode.DECODE:
             positions = ((seq_lens - 1) + position_ids_offsets).to(torch.int64)
             other_kv_index = model_runner.req_to_token_pool.req_to_token[
                 req_pool_indices[0], seq_lens[0] - 1
             ].item()
         else:
-            seq_lens_np = seq_lens.cpu().numpy()
-            prefix_lens_np = prefix_lens.cpu().numpy()
-            position_ids_offsets_np = position_ids_offsets.cpu().numpy()
+            seq_lens_cpu = seq_lens.cpu().numpy()
+            prefix_lens_cpu = prefix_lens.cpu().numpy()
+            position_ids_offsets_cpu = position_ids_offsets.cpu().numpy()
             positions = torch.tensor(
                 np.concatenate(
                     [
                         np.arange(
-                            prefix_lens_np[i] + position_ids_offsets_np[i],
-                            seq_lens_np[i] + position_ids_offsets_np[i],
+                            prefix_lens_cpu[i] + position_ids_offsets_cpu[i],
+                            seq_lens_cpu[i] + position_ids_offsets_cpu[i],
                         )
                         for i in range(batch_size)
                     ],
                     axis=0,
                 ),
                 device="cuda",
             )
@@ -232,17 +227,17 @@
             prefix_lens=prefix_lens,
             positions=positions,
             req_to_token_pool=model_runner.req_to_token_pool,
             token_to_kv_pool=model_runner.token_to_kv_pool,
             out_cache_loc=out_cache_loc,
             out_cache_cont_start=out_cache_cont_start,
             out_cache_cont_end=out_cache_cont_end,
-            top_logprobs_nums=top_logprobs_nums,
-            return_logprob=return_logprob,
             other_kv_index=other_kv_index,
+            return_logprob=return_logprob,
+            top_logprobs_nums=top_logprobs_nums,
         )
 
         if forward_mode == ForwardMode.EXTEND:
             ret.init_extend_args()
 
         if global_server_args_dict.get("enable_flashinfer", False):
             ret.init_flashinfer_args(tp_size)
@@ -278,17 +273,14 @@
         torch.distributed.init_process_group(
             backend="nccl",
             world_size=self.tp_size,
             rank=self.tp_rank,
             init_method=f"tcp://127.0.0.1:{self.nccl_port}",
         )
 
-        # A small all_reduce for warmup.
-        if self.tp_size > 1:
-            torch.distributed.all_reduce(torch.zeros(1).cuda())
         initialize_model_parallel(tensor_model_parallel_size=self.tp_size)
 
         total_gpu_memory = get_available_gpu_memory(
             self.tp_rank, distributed=self.tp_size > 1
         ) * (1 << 30)
         self.load_model()
         self.init_memory_pool(total_gpu_memory)
@@ -299,15 +291,15 @@
         """See also vllm/model_executor/model_loader.py::get_model"""
         # Select model class
         architectures = getattr(self.model_config.hf_config, "architectures", [])
         model_class = get_model_cls_by_arch_name(architectures)
         logger.info(f"Rank {self.tp_rank}: load weight begin.")
 
         # Load weights
-        linear_method = None
+        quant_config = None
 
         quant_cfg = getattr(self.model_config.hf_config, "quantization_config", None)
         if quant_cfg is not None:
             quant_method = quant_cfg.get("quant_method", "").lower()
             # compat: autogptq >=0.8.0 use checkpoint_format: str
             # compat: autogptq <=0.7.1 is_marlin_format: bool
             is_format_marlin = quant_cfg.get(
@@ -321,20 +313,19 @@
             quant_config_class = QUANTIZATION_CONFIG_MAPPING.get(quant_method)
 
             if quant_config_class is None:
                 raise ValueError(f"Unsupported quantization method: {quant_method}")
 
             quant_config = quant_config_class.from_config(quant_cfg)
             logger.info(f"quant_config: {quant_config}")
-            linear_method = quant_config.get_linear_method()
 
-        with _set_default_torch_dtype(torch.float16):
+        with set_default_torch_dtype(torch.float16):
             with torch.device("cuda"):
                 model = model_class(
-                    config=self.model_config.hf_config, linear_method=linear_method
+                    config=self.model_config.hf_config, quant_config=quant_config
                 )
             model.load_weights(
                 self.model_config.path,
                 cache_dir=None,
                 load_format=self.load_format,
                 revision=None,
             )
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/radix_cache.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/radix_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,192 +1,228 @@
 import heapq
 import time
 from collections import defaultdict
-from dataclasses import dataclass
-from typing import Tuple
 
 import torch
 
 
 class TreeNode:
     def __init__(self):
         self.children = defaultdict(TreeNode)
         self.parent = None
+        self.key = None
         self.value = None
-        self.ref_counter = 0
+        self.lock_ref = 0
         self.last_access_time = time.time()
 
-    def __lt__(self, other):
+    def __lt__(self, other: "TreeNode"):
         return self.last_access_time < other.last_access_time
 
 
-def match(key, seq):
+def _key_match(key0, key1):
     i = 0
-    for k, w in zip(key, seq):
-        if k != w:
+    for k0, k1 in zip(key0, key1):
+        if k0 != k1:
             break
         i += 1
     return i
 
 
 class RadixCache:
-    def __init__(self, disable=False):
-        self.reset()
+    def __init__(self, req_to_token_pool, token_to_kv_pool, disable: bool = False):
+        self.req_to_token_pool = req_to_token_pool
+        self.token_to_kv_pool = token_to_kv_pool
         self.disable = disable
+        self.reset()
 
     ##### Public API #####
 
     def reset(self):
         self.root_node = TreeNode()
+        self.root_node.key = []
         self.root_node.value = []
-        self.root_node.ref_counter = 1
+        self.root_node.lock_ref = 1
         self.evictable_size_ = 0
 
     def match_prefix(self, key):
         if self.disable:
             return [], self.root_node
 
         value = []
         last_node = [self.root_node]
         self._match_prefix_helper(self.root_node, key, value, last_node)
         if value:
             value = torch.concat(value)
+        else:
+            value = torch.tensor([], dtype=torch.int64)
         return value, last_node[0]
 
     def insert(self, key, value=None):
         if self.disable:
             return len(key)
 
         if value is None:
             value = [x for x in key]
         return self._insert_helper(self.root_node, key, value)
 
+    def cache_req(
+        self,
+        token_ids,
+        last_uncached_pos,
+        req_pool_idx,
+        del_in_memory_pool=True,
+        old_last_node=None,
+    ):
+        # Insert the request into radix cache
+        indices = self.req_to_token_pool.req_to_token[req_pool_idx, : len(token_ids)]
+        new_prefix_len = self.insert(token_ids, indices.clone())
+
+        # Radix Cache takes one ref in memory pool
+        self.token_to_kv_pool.dec_refs(indices[last_uncached_pos:new_prefix_len])
+
+        if del_in_memory_pool:
+            self.req_to_token_pool.free(req_pool_idx)
+        else:
+            cached_indices, new_last_node = self.match_prefix(token_ids)
+            assert len(cached_indices) == len(token_ids)
+
+            self.req_to_token_pool.req_to_token[
+                req_pool_idx, last_uncached_pos : len(cached_indices)
+            ] = cached_indices[last_uncached_pos:]
+            self.dec_lock_ref(old_last_node)
+            self.inc_lock_ref(new_last_node)
+            return cached_indices, new_last_node
+
     def pretty_print(self):
         self._print_helper(self.root_node, 0)
         print(f"#tokens: {self.total_size()}")
 
     def total_size(self):
         return self._total_size_helper(self.root_node)
 
     def evict(self, num_tokens, evict_callback):
         if self.disable:
-            raise RuntimeError()
+            return
 
         leaves = self._collect_leaves()
         heapq.heapify(leaves)
 
         num_evicted = 0
         while num_evicted < num_tokens and len(leaves):
             x = heapq.heappop(leaves)
 
             if x == self.root_node:
                 break
-            if x.ref_counter > 0:
+            if x.lock_ref > 0:
                 continue
 
             num_evicted += evict_callback(x.value)
             self._delete_leaf(x)
 
             if len(x.parent.children) == 0:
                 heapq.heappush(leaves, x.parent)
 
-    def inc_ref_counter(self, node):
+    def inc_lock_ref(self, node: TreeNode):
         delta = 0
         while node != self.root_node:
-            if node.ref_counter == 0:
+            if node.lock_ref == 0:
                 self.evictable_size_ -= len(node.value)
                 delta -= len(node.value)
-            node.ref_counter += 1
+            node.lock_ref += 1
             node = node.parent
         return delta
 
-    def dec_ref_counter(self, node):
+    def dec_lock_ref(self, node: TreeNode):
         delta = 0
         while node != self.root_node:
-            if node.ref_counter == 1:
+            if node.lock_ref == 1:
                 self.evictable_size_ += len(node.value)
                 delta += len(node.value)
-            node.ref_counter -= 1
+            node.lock_ref -= 1
             node = node.parent
         return delta
 
     def evictable_size(self):
         return self.evictable_size_
 
     ##### Internal Helper Functions #####
+
     def _match_prefix_helper(self, node, key, value, last_node):
         node.last_access_time = time.time()
+        if len(key) == 0:
+            return
 
-        for c_key, child in node.children.items():
-            prefix_len = match(c_key, key)
-            if prefix_len != 0:
-                if prefix_len < len(c_key):
-                    new_node = self._split_node(c_key, child, prefix_len)
-                    value.append(new_node.value)
-                    last_node[0] = new_node
-                else:
-                    value.append(child.value)
-                    last_node[0] = child
-                    self._match_prefix_helper(child, key[prefix_len:], value, last_node)
-                break
+        if key[0] in node.children.keys():
+            child = node.children[key[0]]
+            prefix_len = _key_match(child.key, key)
+            if prefix_len < len(child.key):
+                new_node = self._split_node(child.key, child, prefix_len)
+                value.append(new_node.value)
+                last_node[0] = new_node
+            else:
+                value.append(child.value)
+                last_node[0] = child
+                self._match_prefix_helper(child, key[prefix_len:], value, last_node)
 
-    def _split_node(self, key, child, split_len):
+    def _split_node(self, key, child: TreeNode, split_len):
         # new_node -> child
         new_node = TreeNode()
-        new_node.children = {key[split_len:]: child}
+        new_node.children = {key[split_len:][0]: child}
         new_node.parent = child.parent
-        new_node.ref_counter = child.ref_counter
+        new_node.lock_ref = child.lock_ref
+        new_node.key = child.key[:split_len]
         new_node.value = child.value[:split_len]
         child.parent = new_node
+        child.key = child.key[split_len:]
         child.value = child.value[split_len:]
-        new_node.parent.children[key[:split_len]] = new_node
-        del new_node.parent.children[key]
+        new_node.parent.children[key[:split_len][0]] = new_node
         return new_node
 
     def _insert_helper(self, node, key, value):
         node.last_access_time = time.time()
+        if len(key) == 0:
+            return 0
 
-        for c_key, child in node.children.items():
-            prefix_len = match(c_key, key)
+        if key[0] in node.children.keys():
+            child = node.children[key[0]]
+            prefix_len = _key_match(child.key, key)
 
-            if prefix_len == len(c_key):
+            if prefix_len == len(child.key):
                 if prefix_len == len(key):
                     return prefix_len
                 else:
                     key = key[prefix_len:]
                     value = value[prefix_len:]
                     return prefix_len + self._insert_helper(child, key, value)
 
-            if prefix_len:
-                new_node = self._split_node(c_key, child, prefix_len)
-                return prefix_len + self._insert_helper(
-                    new_node, key[prefix_len:], value[prefix_len:]
-                )
+            new_node = self._split_node(child.key, child, prefix_len)
+            return prefix_len + self._insert_helper(
+                new_node, key[prefix_len:], value[prefix_len:]
+            )
 
         if len(key):
             new_node = TreeNode()
             new_node.parent = node
+            new_node.key = key
             new_node.value = value
-            node.children[key] = new_node
+            node.children[key[0]] = new_node
             self.evictable_size_ += len(value)
         return 0
 
-    def _print_helper(self, node, indent):
+    def _print_helper(self, node: TreeNode, indent):
         for _, child in node.children.items():
-            print(
-                " " * indent, len(child.key), child.key[:10], f"r={child.ref_counter}"
-            )
+            print(" " * indent, len(child.key), child.key[:10], f"r={child.lock_ref}")
             self._print_helper(child, indent=indent + 2)
 
     def _delete_leaf(self, node):
         for k, v in node.parent.children.items():
             if v == node:
                 break
         del node.parent.children[k]
-        self.evictable_size_ -= len(k)
+        self.evictable_size_ -= len(node.key)
 
     def _total_size_helper(self, node):
         x = len(node.value)
         for child in node.children.values():
             x += self._total_size_helper(child)
         return x
 
@@ -201,15 +237,15 @@
                 dfs_(x)
 
         dfs_(self.root_node)
         return ret_list
 
 
 if __name__ == "__main__":
-    tree = RadixCache(disable=False)
+    tree = RadixCache(None, None, False)
 
     tree.insert("Hello")
     tree.insert("Hello")
     tree.insert("Hello_L.A.!")
     # tree.insert("Hello_world! Happy")
     # tree.insert("I love you!")
     tree.pretty_print()
```

### Comparing `dblcsgen-0.2.6/sglang/srt/managers/router/scheduler.py` & `dblcsgen-0.2.7/sglang/srt/managers/router/scheduler.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,48 +23,37 @@
             forward_queue.sort(key=lambda x: -len(x.prefix_indices))
             return forward_queue
         elif self.schedule_heuristic == "random":
             random.shuffle(forward_queue)
             return forward_queue
         elif self.schedule_heuristic == "fcfs":
             return forward_queue
-        elif self.schedule_heuristic == "weight":
+        elif self.schedule_heuristic == "dfs-weight":
             last_node_to_reqs = defaultdict(list)
             for req in forward_queue:
                 last_node_to_reqs[req.last_node].append(req)
-            for node in last_node_to_reqs:
-                last_node_to_reqs[node].sort(key=lambda x: -len(x.prefix_indices))
 
             node_to_weight = defaultdict(int)
-            self._calc_weight_recursive(
-                self.tree_cache.root_node, last_node_to_reqs, node_to_weight
-            )
+            for node in last_node_to_reqs:
+                node_to_weight[node] = len(last_node_to_reqs[node])
+            self.calc_weight(self.tree_cache.root_node, node_to_weight)
 
-            tmp_queue = []
-            self._get_weight_priority_recursive(
-                self.tree_cache.root_node, node_to_weight, last_node_to_reqs, tmp_queue
+            q = []
+            self.get_dfs_priority(
+                self.tree_cache.root_node, node_to_weight, last_node_to_reqs, q
             )
-            assert len(tmp_queue) == len(forward_queue)
-            return tmp_queue
+            assert len(q) == len(forward_queue)
+            return q
         else:
             raise ValueError(f"Unknown schedule_heuristic: {self.schedule_heuristic}")
 
-    def _calc_weight_recursive(self, cur_node, last_node_to_reqs, node_to_weight):
-        node_to_weight[cur_node] = 1
-        if cur_node in last_node_to_reqs:
-            node_to_weight[cur_node] += len(last_node_to_reqs[cur_node])
+    def calc_weight(self, cur_node, node_to_weight):
         for child in cur_node.children.values():
-            self._calc_weight_recursive(child, last_node_to_reqs, node_to_weight)
+            self.calc_weight(child, node_to_weight)
             node_to_weight[cur_node] += node_to_weight[child]
 
-    def _get_weight_priority_recursive(
-        self, cur_node, node_to_wight, last_node_to_reqs, tmp_queue
-    ):
-        visit_list = [child for child in cur_node.children.values()]
-        visit_list.sort(key=lambda x: -node_to_wight[x])
-        # for node in visit_list:
-        #     print(f"{node_to_wight[node]} {len(node.value) if node.value is not None else 0}")
-        for child in visit_list:
-            self._get_weight_priority_recursive(
-                child, node_to_wight, last_node_to_reqs, tmp_queue
-            )
-        tmp_queue.extend(last_node_to_reqs[cur_node])
+    def get_dfs_priority(self, cur_node, node_to_priority, last_node_to_reqs, q):
+        childs = [child for child in cur_node.children.values()]
+        childs.sort(key=lambda x: -node_to_priority[x])
+        for child in childs:
+            self.get_dfs_priority(child, node_to_priority, last_node_to_reqs, q)
+        q.extend(last_node_to_reqs[cur_node])
```

### Comparing `dblcsgen-0.2.6/sglang/srt/memory_pool.py` & `dblcsgen-0.2.7/sglang/srt/memory_pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,23 @@
     def free(self, free_index):
         if isinstance(free_index, (int,)):
             self.can_use_mem_size += 1
         else:
             self.can_use_mem_size += free_index.shape[0]
         self.mem_state[free_index] = 1
 
-        # if self.can_use_mem_size == len(self.mem_state):
-        #     print(f"ReqToTokenPool: freed all. size = {self.can_use_mem_size}.")
-
     def clear(self):
         self.mem_state.fill_(1)
         self.can_use_mem_size = len(self.mem_state)
 
 
 class TokenToKVPool:
     def __init__(self, size, dtype, head_num, head_dim, layer_num):
         self.mem_state = torch.zeros((size,), dtype=torch.int16, device="cuda")
-        self.alloc_ct = 0
+        self.total_ref_ct = 0
 
         # [size, key/value, head_num, head_dim] for each layer
         self.kv_data = [
             torch.empty((size, 2, head_num, head_dim), dtype=dtype, device="cuda")
             for _ in range(layer_num)
         ]
 
@@ -79,34 +76,28 @@
             return None
 
         start_loc = can_used_loc[0].item()
         select_index = torch.arange(start_loc, start_loc + need_size, device="cuda")
         self.add_refs(select_index)
         return select_index.to(torch.int32), start_loc, start_loc + need_size
 
-    def free(self, free_index):
-        return self.decrease_refs(free_index)
-
     def used_size(self):
         return len(torch.nonzero(self.mem_state).squeeze(1))
 
     def available_size(self):
         return torch.sum(self.mem_state == 0).item()
 
     def add_refs(self, token_index: torch.Tensor):
-        self.alloc_ct += len(token_index)
+        self.total_ref_ct += len(token_index)
         self.mem_state[token_index] += 1
 
-    def decrease_refs(self, token_index: torch.Tensor):
-        self.alloc_ct -= len(token_index)
+    def dec_refs(self, token_index: torch.Tensor):
+        self.total_ref_ct -= len(token_index)
         self.mem_state[token_index] -= 1
 
         num_freed = torch.sum(self.mem_state[token_index] == 0)
 
-        # if self.alloc_ct == 0:
-        #     print(f"TokenToKVPool: freed all. size = {len(self.mem_state)}.")
-
         return num_freed
 
     def clear(self):
         self.mem_state.fill_(0)
-        self.alloc_ct = 0
+        self.total_ref_ct = 0
```

### Comparing `dblcsgen-0.2.6/sglang/srt/mm_utils.py` & `dblcsgen-0.2.7/sglang/srt/mm_utils.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/model_config.py` & `dblcsgen-0.2.7/sglang/srt/model_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/models/dbrx.py` & `dblcsgen-0.2.7/sglang/srt/models/dbrx.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 # Adapted from:
 # https://github.com/vllm-project/vllm/blob/14ccd94c89d0ffd9da283545d93ab1dfea5da340/vllm/model_executor/models/dbrx.py
 # coding=utf-8
 from typing import Optional
 
 import torch
 import torch.nn as nn
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
-from sglang.srt.models.dbrx_config import DbrxConfig
 from vllm.model_executor.layers.fused_moe import fused_moe
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     QKVParallelLinear,
     ReplicatedLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     DEFAULT_VOCAB_PADDING_SIZE,
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.communication_op import (
+from vllm.distributed import (
     tensor_model_parallel_all_reduce,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_rank,
     get_tensor_model_parallel_world_size,
 )
 from vllm.model_executor.utils import set_weight_attrs
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+from sglang.srt.models.dbrx_config import DbrxConfig
+
 
 class DbrxRouter(nn.Module):
     """A Router implementation for DBRX that returns logits for each expert
     per token.
     """
 
     def __init__(
@@ -51,15 +53,15 @@
         self.num_total_experts = config.ffn_config.moe_num_experts
         self.d_model = config.d_model
         self.layer = ReplicatedLinear(
             self.d_model,
             self.num_total_experts,
             bias=False,
             params_dtype=params_dtype,
-            linear_method=None,
+            quant_config=None,
         )
 
     def forward(self, hidden_states: torch.Tensor) -> torch.Tensor:
         router_logits, _ = self.layer(hidden_states)
         return router_logits
 
 
@@ -70,15 +72,15 @@
     kernel is used for the forward pass, and finally we reduce the outputs
     across ranks.
     """
 
     def __init__(
         self,
         config: DbrxConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
         params_dtype: Optional[torch.dtype] = None,
     ):
         super().__init__()
         self.tp_size = get_tensor_model_parallel_world_size()
         self.num_total_experts = config.ffn_config.moe_num_experts
         self.top_k = config.ffn_config.moe_top_k
         self.d_model = config.d_model
@@ -167,20 +169,19 @@
         if self.tp_size > 1:
             final_hidden_states = tensor_model_parallel_all_reduce(final_hidden_states)
 
         return final_hidden_states.view(num_tokens, hidden_size)
 
 
 class DbrxAttention(nn.Module):
-
     def __init__(
         self,
         config: DbrxConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.d_model = config.d_model
         self.total_num_heads = config.n_heads
         self.head_dim = self.d_model // self.total_num_heads
         self.total_num_kv_heads = config.attn_config.kv_n_heads
         self.clip_qkv = config.attn_config.clip_qkv
@@ -190,21 +191,21 @@
         # pylint: disable=invalid-name
         self.Wqkv = QKVParallelLinear(
             self.d_model,
             self.head_dim,
             self.total_num_heads,
             self.total_num_kv_heads,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.out_proj = RowParallelLinear(
             self.d_model,
             self.d_model,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=self.max_position,
             base=int(self.rope_theta),
             is_neox_style=True,
@@ -247,24 +248,23 @@
         q, k = self.rotary_emb(position_ids, q, k)
         attn_output = self.attn(q, k, v, input_metadata)
         hidden_states, _ = self.out_proj(attn_output)
         return hidden_states
 
 
 class DbrxFusedNormAttention(nn.Module):
-
     def __init__(
         self,
         config: DbrxConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.d_model = config.d_model
-        self.attn = DbrxAttention(config, layer_id, linear_method)
+        self.attn = DbrxAttention(config, layer_id, quant_config=quant_config)
         self.norm_1 = nn.LayerNorm(self.d_model)
         self.norm_2 = nn.LayerNorm(self.d_model)
 
     def forward(
         self,
         position_ids: torch.Tensor,
         hidden_states: torch.Tensor,
@@ -280,24 +280,23 @@
         hidden_states = residual + x
         residual = hidden_states
         hidden_states = self.norm_2(hidden_states)
         return hidden_states, residual
 
 
 class DbrxBlock(nn.Module):
-
     def __init__(
         self,
         config: DbrxConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
-        self.norm_attn_norm = DbrxFusedNormAttention(config, layer_id, linear_method)
-        self.ffn = DbrxExperts(config, linear_method)
+        self.norm_attn_norm = DbrxFusedNormAttention(config, layer_id, quant_config=quant_config)
+        self.ffn = DbrxExperts(config, quant_config=quant_config)
 
     def forward(
         self,
         position_ids: torch.Tensor,
         hidden_states: torch.Tensor,
         input_metadata: InputMetadata,
     ) -> torch.Tensor:
@@ -308,27 +307,26 @@
         )
         hidden_states = self.ffn(hidden_states)
         hidden_states = hidden_states + residual
         return hidden_states
 
 
 class DbrxModel(nn.Module):
-
     def __init__(
         self,
         config: DbrxConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.wte = VocabParallelEmbedding(
             config.vocab_size,
             config.d_model,
         )
         self.blocks = nn.ModuleList(
-            [DbrxBlock(config, i, linear_method) for i in range(config.n_layers)]
+            [DbrxBlock(config, i, quant_config=quant_config) for i in range(config.n_layers)]
         )
         self.norm_f = nn.LayerNorm(config.d_model, eps=1e-5)
         for module in self.modules():
             if hasattr(module, "bias") and isinstance(module.bias, nn.Parameter):
                 # Remove the bias term in Linear and LayerNorm.
                 module.register_parameter("bias", None)
 
@@ -347,25 +345,24 @@
             block = self.blocks[i]
             hidden_states = block(position_ids, hidden_states, input_metadata)
         hidden_states = self.norm_f(hidden_states)
         return hidden_states
 
 
 class DbrxForCausalLM(nn.Module):
-
     def __init__(
         self,
         config: DbrxConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
+        self.quant_config = quant_config
         self.unpadded_vocab_size = config.vocab_size
-        self.transformer = DbrxModel(config, linear_method)
+        self.transformer = DbrxModel(config, quant_config=quant_config)
         self.lm_head = ParallelLMHead(
             config.vocab_size,
             config.d_model,
             org_num_embeddings=config.vocab_size,
             padding_size=DEFAULT_VOCAB_PADDING_SIZE,
         )
         self.logits_processor = LogitsProcessor(config)
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/dbrx_config.py` & `dblcsgen-0.2.7/sglang/srt/models/dbrx_config.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/srt/models/gemma.py` & `dblcsgen-0.2.7/sglang/srt/models/gemma.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 # Adapted from:
 # https://github.com/vllm-project/vllm/blob/d65fac2738f0287a41955b45df76a2d5a919bff6/vllm/model_executor/models/gemma.py
 """Inference-only Gemma model compatible with HuggingFace weights."""
 from typing import Optional, Tuple
 
 import torch
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from transformers import PretrainedConfig
 from vllm.config import LoRAConfig
 from vllm.model_executor.layers.activation import GeluAndMul
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     MergedColumnParallelLinear,
     QKVParallelLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import VocabParallelEmbedding
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 
 class GemmaMLP(nn.Module):
     def __init__(
         self,
         hidden_size: int,
         intermediate_size: int,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.gate_up_proj = MergedColumnParallelLinear(
             hidden_size,
             [intermediate_size] * 2,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.down_proj = RowParallelLinear(
-            intermediate_size, hidden_size, bias=False, linear_method=linear_method
+            intermediate_size, hidden_size, bias=False, quant_config=quant_config,
         )
         self.act_fn = GeluAndMul()
 
     def forward(self, x):
         gate_up, _ = self.gate_up_proj(x)
         x = self.act_fn(gate_up)
         x, _ = self.down_proj(x)
@@ -61,15 +63,15 @@
         hidden_size: int,
         num_heads: int,
         num_kv_heads: int,
         head_dim: int,
         layer_id: int = 0,
         max_position_embeddings: int = 8192,
         rope_theta: float = 10000,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = hidden_size
         tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
         assert self.total_num_heads % tp_size == 0
         self.num_heads = self.total_num_heads // tp_size
@@ -91,21 +93,21 @@
 
         self.qkv_proj = QKVParallelLinear(
             hidden_size,
             self.head_dim,
             self.total_num_heads,
             self.total_num_kv_heads,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
 
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=max_position_embeddings,
             base=self.rope_theta,
@@ -134,32 +136,32 @@
 
 
 class GemmaDecoderLayer(nn.Module):
     def __init__(
         self,
         config: PretrainedConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = config.hidden_size
         self.self_attn = GemmaAttention(
             hidden_size=self.hidden_size,
             num_heads=config.num_attention_heads,
             num_kv_heads=config.num_key_value_heads,
             head_dim=config.head_dim,
             layer_id=layer_id,
             max_position_embeddings=config.max_position_embeddings,
             rope_theta=config.rope_theta,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.mlp = GemmaMLP(
             hidden_size=self.hidden_size,
             intermediate_size=config.intermediate_size,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.input_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.post_attention_layernorm = RMSNorm(
             config.hidden_size, eps=config.rms_norm_eps
         )
 
     def forward(
@@ -187,26 +189,26 @@
         return hidden_states, residual
 
 
 class GemmaModel(nn.Module):
     def __init__(
         self,
         config: PretrainedConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
 
         self.embed_tokens = VocabParallelEmbedding(
             config.vocab_size,
             config.hidden_size,
         )
         self.layers = nn.ModuleList(
             [
-                GemmaDecoderLayer(config, i, linear_method)
+                GemmaDecoderLayer(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
@@ -259,22 +261,22 @@
     # Gemma does not apply LoRA to the embedding layer.
     embedding_modules = {}
     embedding_padding_modules = []
 
     def __init__(
         self,
         config: PretrainedConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
         lora_config: Optional[LoRAConfig] = None,
     ) -> None:
         del lora_config  # Unused.
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
-        self.model = GemmaModel(config, linear_method)
+        self.quant_config = quant_config
+        self.model = GemmaModel(config, quant_config=quant_config)
         self.logits_processor = LogitsProcessor(config)
 
     @torch.no_grad()
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/llama2.py` & `dblcsgen-0.2.7/sglang/srt/models/llama2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,59 @@
 # Adapted from
 # https://github.com/vllm-project/vllm/blob/671af2b1c0b3ed6d856d37c21a561cc429a10701/vllm/model_executor/models/llama.py#L1
 """Inference-only LLaMA model compatible with HuggingFace weights."""
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import torch
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from transformers import LlamaConfig
 from vllm.model_executor.layers.activation import SiluAndMul
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     MergedColumnParallelLinear,
     QKVParallelLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 
 class LlamaMLP(nn.Module):
     def __init__(
         self,
         hidden_size: int,
         intermediate_size: int,
         hidden_act: str,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.gate_up_proj = MergedColumnParallelLinear(
             hidden_size,
             [intermediate_size] * 2,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.down_proj = RowParallelLinear(
-            intermediate_size, hidden_size, bias=False, linear_method=linear_method
+            intermediate_size, hidden_size, bias=False, quant_config=quant_config,
         )
         if hidden_act != "silu":
             raise ValueError(
                 f"Unsupported activation: {hidden_act}. "
                 "Only silu is supported for now."
             )
         self.act_fn = SiluAndMul()
@@ -69,15 +71,15 @@
         hidden_size: int,
         num_heads: int,
         num_kv_heads: int,
         layer_id: int = 0,
         rope_theta: float = 10000,
         rope_scaling: Optional[Dict[str, Any]] = None,
         max_position_embeddings: int = 8192,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = hidden_size
         tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
         assert self.total_num_heads % tp_size == 0
         self.num_heads = self.total_num_heads // tp_size
@@ -100,21 +102,21 @@
 
         self.qkv_proj = QKVParallelLinear(
             hidden_size,
             self.head_dim,
             self.total_num_heads,
             self.total_num_kv_heads,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
 
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=max_position_embeddings,
             base=rope_theta,
@@ -143,36 +145,36 @@
 
 
 class LlamaDecoderLayer(nn.Module):
     def __init__(
         self,
         config: LlamaConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = config.hidden_size
         rope_theta = getattr(config, "rope_theta", 10000)
         rope_scaling = getattr(config, "rope_scaling", None)
         max_position_embeddings = getattr(config, "max_position_embeddings", 8192)
         self.self_attn = LlamaAttention(
             hidden_size=self.hidden_size,
             num_heads=config.num_attention_heads,
             num_kv_heads=config.num_key_value_heads,
             layer_id=layer_id,
             rope_theta=rope_theta,
             rope_scaling=rope_scaling,
             max_position_embeddings=max_position_embeddings,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.mlp = LlamaMLP(
             hidden_size=self.hidden_size,
             intermediate_size=config.intermediate_size,
             hidden_act=config.hidden_act,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.input_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.post_attention_layernorm = RMSNorm(
             config.hidden_size, eps=config.rms_norm_eps
         )
 
     def forward(
@@ -200,27 +202,27 @@
         return hidden_states, residual
 
 
 class LlamaModel(nn.Module):
     def __init__(
         self,
         config: LlamaConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
         self.embed_tokens = VocabParallelEmbedding(
             config.vocab_size,
             config.hidden_size,
         )
         self.layers = nn.ModuleList(
             [
-                LlamaDecoderLayer(config, i, linear_method)
+                LlamaDecoderLayer(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
@@ -246,20 +248,20 @@
         return hidden_states
 
 
 class LlamaForCausalLM(nn.Module):
     def __init__(
         self,
         config: LlamaConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
-        self.model = LlamaModel(config, linear_method)
+        self.quant_config = quant_config
+        self.model = LlamaModel(config, quant_config=quant_config)
         self.lm_head = ParallelLMHead(config.vocab_size, config.hidden_size)
         self.logits_processor = LogitsProcessor(config)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/llava.py` & `dblcsgen-0.2.7/sglang/srt/models/llava.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 """Inference-only LLaVa model compatible with HuggingFace weights."""
 
 from typing import List, Optional
 
 import numpy as np
 import torch
+from torch import nn
+from transformers import CLIPVisionModel, LlavaConfig
+from transformers.models.llava.modeling_llava import LlavaMultiModalProjector
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
+from sglang.srt.weight_utils import (
+    default_weight_loader,
+    hf_model_weights_iterator,
+)
+
 from sglang.srt.managers.router.infer_batch import ForwardMode
 from sglang.srt.managers.router.model_runner import InputMetadata
 from sglang.srt.mm_utils import (
     get_anyres_image_grid_shape,
     unpad_image,
     unpad_image_shape,
 )
 from sglang.srt.models.llama2 import LlamaForCausalLM
-from torch import nn
-from transformers import CLIPVisionModel, LlamaConfig, LlavaConfig
-from transformers.models.llava.modeling_llava import LlavaMultiModalProjector
-from vllm.model_executor.layers.linear import LinearMethodBase
-from vllm.model_executor.weight_utils import (
-    default_weight_loader,
-    hf_model_weights_iterator,
-)
 
 
 class LlavaLlamaForCausalLM(nn.Module):
     def __init__(
         self,
         config: LlavaConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
         self.vision_tower = None
         self.config.vision_config.hidden_size = config.mm_hidden_size
         self.config.text_config.hidden_size = config.hidden_size
         self.multi_modal_projector = LlavaMultiModalProjector(config)
-        self.language_model = LlamaForCausalLM(config, linear_method)
+        self.language_model = LlamaForCausalLM(config, quant_config=quant_config)
         if "unpad" in getattr(config, "mm_patch_merge_type", ""):
             self.language_model.model.image_newline = nn.Parameter(
                 torch.empty(config.text_config.hidden_size, dtype=torch.float16)
             )
 
     def pad_input_ids(self, input_ids, pad_value, pt_shape=None, image_size=None):
         new_image_feature_len = self.image_feature_len
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/mixtral.py` & `dblcsgen-0.2.7/sglang/srt/models/mixtral.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 # Adapted from
 # https://github.com/vllm-project/vllm/blob/d0215a58e78572d91dadafe9d832a2db89b09a13/vllm/model_executor/models/mixtral.py#L1
 """Inference-only Mixtral model."""
-from typing import List, Optional, Tuple
+from typing import Optional
 
 import numpy as np
 import torch
 import torch.nn.functional as F
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from transformers import MixtralConfig
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     QKVParallelLinear,
     ReplicatedLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.communication_op import (
+from vllm.distributed import (
     tensor_model_parallel_all_reduce,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_rank,
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 
 class MixtralMLP(nn.Module):
     def __init__(
         self,
         num_experts: int,
         hidden_size: int,
         intermediate_size: int,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.num_experts = num_experts
         self.ffn_dim = intermediate_size
         self.hidden_dim = hidden_size
 
         self.w1 = ReplicatedLinear(
-            self.hidden_dim, self.ffn_dim, bias=False, linear_method=linear_method
+            self.hidden_dim, self.ffn_dim, bias=False, quant_config=quant_config
         )
         self.w2 = ReplicatedLinear(
-            self.ffn_dim, self.hidden_dim, bias=False, linear_method=linear_method
+            self.ffn_dim, self.hidden_dim, bias=False, quant_config=quant_config
         )
         self.w3 = ReplicatedLinear(
-            self.hidden_dim, self.ffn_dim, bias=False, linear_method=linear_method
+            self.hidden_dim, self.ffn_dim, bias=False, quant_config=quant_config
         )
 
         # TODO: Use vllm's SiluAndMul
         self.act_fn = nn.SiLU()
 
     def forward(self, hidden_states: torch.Tensor) -> torch.Tensor:
         w1_out, _ = self.w1(hidden_states)
@@ -71,15 +73,15 @@
         return current_hidden_states
 
 
 class MixtralMoE(nn.Module):
     def __init__(
         self,
         config: MixtralConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.config = config
         self.rank = get_tensor_model_parallel_rank()
         self.tp_size = get_tensor_model_parallel_world_size()
         self.num_total_experts = config.num_local_experts
         self.top_k = config.num_experts_per_tok
@@ -98,15 +100,15 @@
         self.experts = nn.ModuleList(
             [
                 (
                     MixtralMLP(
                         self.num_total_experts,
                         config.hidden_size,
                         config.intermediate_size,
-                        linear_method=linear_method,
+                        quant_config=quant_config,
                     )
                     if idx in self.expert_indicies
                     else None
                 )
                 for idx in range(self.num_total_experts)
             ]
         )
@@ -143,15 +145,15 @@
         self,
         hidden_size: int,
         num_heads: int,
         num_kv_heads: int,
         layer_id: int = 0,
         max_position: int = 4096 * 32,
         rope_theta: float = 10000,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
         sliding_window: Optional[int] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = hidden_size
         tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
         assert self.total_num_heads % tp_size == 0
@@ -175,21 +177,21 @@
 
         self.qkv_proj = QKVParallelLinear(
             hidden_size,
             self.head_dim,
             self.total_num_heads,
             self.total_num_kv_heads,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=max_position,
             base=int(self.rope_theta),
             is_neox_style=True,
@@ -217,31 +219,31 @@
 
 
 class MixtralDecoderLayer(nn.Module):
     def __init__(
         self,
         config: MixtralConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = config.hidden_size
         # Requires transformers > 4.32.0
         rope_theta = getattr(config, "rope_theta", 10000)
         self.self_attn = MixtralAttention(
             hidden_size=self.hidden_size,
             num_heads=config.num_attention_heads,
             max_position=config.max_position_embeddings,
             num_kv_heads=config.num_key_value_heads,
             layer_id=layer_id,
             rope_theta=rope_theta,
             sliding_window=config.sliding_window,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
-        self.block_sparse_moe = MixtralMoE(config=config, linear_method=linear_method)
+        self.block_sparse_moe = MixtralMoE(config=config, quant_config=quant_config)
         self.input_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.post_attention_layernorm = RMSNorm(
             config.hidden_size, eps=config.rms_norm_eps
         )
 
     def forward(
         self,
@@ -268,28 +270,28 @@
         return hidden_states, residual
 
 
 class MixtralModel(nn.Module):
     def __init__(
         self,
         config: MixtralConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
 
         self.embed_tokens = VocabParallelEmbedding(
             config.vocab_size,
             config.hidden_size,
         )
         # config.num_hidden_layers=16
         self.layers = nn.ModuleList(
             [
-                MixtralDecoderLayer(config, i, linear_method=linear_method)
+                MixtralDecoderLayer(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
@@ -312,20 +314,20 @@
         return hidden_states
 
 
 class MixtralForCausalLM(nn.Module):
     def __init__(
         self,
         config: MixtralConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
-        self.model = MixtralModel(config, linear_method)
+        self.quant_config = quant_config
+        self.model = MixtralModel(config, quant_config=quant_config)
         self.lm_head = ParallelLMHead(config.vocab_size, config.hidden_size)
         self.logits_processor = LogitsProcessor(config)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/qwen.py` & `dblcsgen-0.2.7/sglang/srt/models/qwen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional
 
 import torch
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from transformers import PretrainedConfig
 from vllm.model_executor.layers.activation import SiluAndMul
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     MergedColumnParallelLinear,
     QKVParallelLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 
 class QWenMLP(nn.Module):
     def __init__(
         self,
         hidden_size: int,
         intermediate_size: int,
         hidden_act: str = "silu",
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.gate_up_proj = MergedColumnParallelLinear(
             hidden_size,
             2 * [intermediate_size],
             bias=False,
             gather_output=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.c_proj = RowParallelLinear(
             intermediate_size,
             hidden_size,
             bias=False,
             input_is_parallel=True,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         if hidden_act != "silu":
             raise ValueError(
                 f"Unsupported activation: {hidden_act}. "
                 "Only silu is supported for now."
             )
         self.act_fn = SiluAndMul()
@@ -70,15 +72,15 @@
         self,
         hidden_size: int,
         num_heads: int,
         max_position_embeddings: int,
         layer_id: int = 0,
         rope_theta: float = 10000,
         rope_scaling: Optional[Dict[str, Any]] = None,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ):
         super().__init__()
         self.hidden_size = hidden_size
         tensor_model_parallel_world_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
         assert self.total_num_heads % tensor_model_parallel_world_size == 0
         self.num_heads = self.total_num_heads // tensor_model_parallel_world_size
@@ -86,22 +88,22 @@
 
         # pylint: disable=invalid-name
         self.c_attn = QKVParallelLinear(
             hidden_size,
             self.head_dim,
             self.total_num_heads,
             bias=True,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.c_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
             input_is_parallel=True,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=max_position_embeddings,
             base=rope_theta,
             rope_scaling=rope_scaling,
@@ -126,36 +128,36 @@
         q, k = self.rotary_emb(positions, q, k)
         attn_output = self.attn(q, k, v, input_metadata)
         output, _ = self.c_proj(attn_output)
         return output
 
 
 class QWenBlock(nn.Module):
-    def __init__(self, config: PretrainedConfig, layer_id, linear_method=None):
+    def __init__(self, config: PretrainedConfig, layer_id, quant_config: Optional[QuantizationConfig] = None,):
         super().__init__()
         self.ln_1 = RMSNorm(config.hidden_size, eps=config.layer_norm_epsilon)
 
         rope_theta = getattr(config, "rope_theta", 10000)
         rope_scaling = getattr(config, "rope_scaling", None)
         self.attn = QWenAttention(
             config.hidden_size,
             config.num_attention_heads,
             config.max_position_embeddings,
             rope_theta=rope_theta,
             rope_scaling=rope_scaling,
             layer_id=layer_id,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
 
         self.ln_2 = RMSNorm(config.hidden_size, eps=config.layer_norm_epsilon)
 
         self.mlp = QWenMLP(
             config.hidden_size,
             config.intermediate_size // 2,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
 
     def forward(
         self,
         positions: torch.Tensor,
         hidden_states: torch.Tensor,
         input_metadata: InputMetadata,
@@ -175,27 +177,27 @@
         hidden_states = self.ln_2(hidden_states)
         hidden_states = self.mlp(hidden_states)
         hidden_states = residual + hidden_states
         return hidden_states
 
 
 class QWenModel(nn.Module):
-    def __init__(self, config: PretrainedConfig, linear_method=None):
+    def __init__(self, config: PretrainedConfig, quant_config: Optional[QuantizationConfig] = None,):
         super().__init__()
         self.config = config
         self.vocab_size = config.vocab_size
 
         vocab_size = ((config.vocab_size + 63) // 64) * 64
         self.wte = VocabParallelEmbedding(
             vocab_size,
             config.hidden_size,
         )
         self.h = nn.ModuleList(
             [
-                QWenBlock(config, i, linear_method=linear_method)
+                QWenBlock(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         self.ln_f = RMSNorm(config.hidden_size, eps=config.layer_norm_epsilon)
 
     def forward(
         self,
@@ -212,18 +214,18 @@
                 input_metadata,
             )
         hidden_states = self.ln_f(hidden_states)
         return hidden_states
 
 
 class QWenLMHeadModel(nn.Module):
-    def __init__(self, config: PretrainedConfig, linear_method=None):
+    def __init__(self, config: PretrainedConfig, quant_config: Optional[QuantizationConfig] = None,):
         super().__init__()
         self.config = config
-        self.transformer = QWenModel(config, linear_method=linear_method)
+        self.transformer = QWenModel(config, quant_config=quant_config)
         vocab_size = ((config.vocab_size + 63) // 64) * 64
         self.lm_head = ParallelLMHead(vocab_size, config.hidden_size)
         self.logits_processor = LogitsProcessor(config)
 
     def forward(
         self,
         input_ids: torch.Tensor,
@@ -270,8 +272,8 @@
                 if name.endswith(".bias") and name not in params_dict:
                     continue
                 param = params_dict[name]
                 weight_loader = getattr(param, "weight_loader", default_weight_loader)
                 weight_loader(param, loaded_weight)
 
 
-EntryClass = QWenLMHeadModel
+EntryClass = QWenLMHeadModel
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/qwen2.py` & `dblcsgen-0.2.7/sglang/srt/models/qwen2.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 # Adapted from llama2.py
 # Modify details for the adaptation of Qwen2 model.
 """Inference-only Qwen2 model compatible with HuggingFace weights."""
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 import torch
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from vllm.model_executor.layers.activation import SiluAndMul
 from vllm.model_executor.layers.layernorm import RMSNorm
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     MergedColumnParallelLinear,
     QKVParallelLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 Qwen2Config = None
 
 
 class Qwen2MLP(nn.Module):
     def __init__(
         self,
         hidden_size: int,
         intermediate_size: int,
         hidden_act: str,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.gate_up_proj = MergedColumnParallelLinear(
             hidden_size,
             [intermediate_size] * 2,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.down_proj = RowParallelLinear(
-            intermediate_size, hidden_size, bias=False, linear_method=linear_method
+            intermediate_size, hidden_size, bias=False, quant_config=quant_config,
         )
         if hidden_act != "silu":
             raise ValueError(
                 f"Unsupported activation: {hidden_act}. "
                 "Only silu is supported for now."
             )
         self.act_fn = SiluAndMul()
@@ -70,15 +72,15 @@
         hidden_size: int,
         num_heads: int,
         num_kv_heads: int,
         layer_id: int = 0,
         rope_theta: float = 1000000,
         rope_scaling: Optional[Dict[str, Any]] = None,
         max_position_embeddings: int = 32768,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = hidden_size
         tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = num_heads
         assert self.total_num_heads % tp_size == 0
         self.num_heads = self.total_num_heads // tp_size
@@ -101,21 +103,21 @@
 
         self.qkv_proj = QKVParallelLinear(
             hidden_size,
             self.head_dim,
             self.total_num_heads,
             self.total_num_kv_heads,
             bias=True,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             hidden_size,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
 
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.head_dim,
             max_position=max_position_embeddings,
             base=rope_theta,
@@ -144,36 +146,36 @@
 
 
 class Qwen2DecoderLayer(nn.Module):
     def __init__(
         self,
         config: Qwen2Config,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.hidden_size = config.hidden_size
         rope_theta = getattr(config, "rope_theta", 1000000)
         rope_scaling = getattr(config, "rope_scaling", None)
         max_position_embeddings = getattr(config, "max_position_embeddings", 32768)
         self.self_attn = Qwen2Attention(
             hidden_size=self.hidden_size,
             num_heads=config.num_attention_heads,
             num_kv_heads=config.num_key_value_heads,
             layer_id=layer_id,
             rope_theta=rope_theta,
             rope_scaling=rope_scaling,
             max_position_embeddings=max_position_embeddings,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.mlp = Qwen2MLP(
             hidden_size=self.hidden_size,
             intermediate_size=config.intermediate_size,
             hidden_act=config.hidden_act,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.input_layernorm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.post_attention_layernorm = RMSNorm(
             config.hidden_size, eps=config.rms_norm_eps
         )
 
     def forward(
@@ -201,27 +203,27 @@
         return hidden_states, residual
 
 
 class Qwen2Model(nn.Module):
     def __init__(
         self,
         config: Qwen2Config,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
         self.padding_idx = config.pad_token_id
         self.vocab_size = config.vocab_size
         self.embed_tokens = VocabParallelEmbedding(
             config.vocab_size,
             config.hidden_size,
         )
         self.layers = nn.ModuleList(
             [
-                Qwen2DecoderLayer(config, i, linear_method)
+                Qwen2DecoderLayer(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         self.norm = RMSNorm(config.hidden_size, eps=config.rms_norm_eps)
 
     def forward(
         self,
@@ -247,20 +249,20 @@
         return hidden_states
 
 
 class Qwen2ForCausalLM(nn.Module):
     def __init__(
         self,
         config: Qwen2Config,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
-        self.model = Qwen2Model(config, linear_method)
+        self.quant_config = quant_config
+        self.model = Qwen2Model(config, quant_config=quant_config)
         self.lm_head = ParallelLMHead(config.vocab_size, config.hidden_size)
         self.logits_processor = LogitsProcessor(config)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/stablelm.py` & `dblcsgen-0.2.7/sglang/srt/models/stablelm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 # This code is based on:
 # https://github.com/vllm-project/vllm/blob/main/vllm/model_executor/models/stablelm.py
 """Inference-only StableLM-2 (https://huggingface.co/stabilityai/stablelm-2-1_6b)
 model compatible with HuggingFace weights."""
 from typing import Optional, Tuple
 
 import torch
-from sglang.srt.layers.logits_processor import LogitsProcessor
-from sglang.srt.layers.radix_attention import RadixAttention
-from sglang.srt.managers.router.model_runner import InputMetadata
 from torch import nn
 from transformers import PretrainedConfig
 from vllm.model_executor.layers.activation import SiluAndMul
 from vllm.model_executor.layers.linear import (
-    LinearMethodBase,
     MergedColumnParallelLinear,
     QKVParallelLinear,
     RowParallelLinear,
 )
+from vllm.model_executor.layers.quantization.base_config import (
+    QuantizationConfig)
 from vllm.model_executor.layers.rotary_embedding import get_rope
 from vllm.model_executor.layers.vocab_parallel_embedding import (
     ParallelLMHead,
     VocabParallelEmbedding,
 )
-from vllm.model_executor.parallel_utils.parallel_state import (
+from vllm.distributed import (
     get_tensor_model_parallel_world_size,
 )
-from vllm.model_executor.weight_utils import (
+from sglang.srt.weight_utils import (
     default_weight_loader,
     hf_model_weights_iterator,
 )
 
+from sglang.srt.layers.logits_processor import LogitsProcessor
+from sglang.srt.layers.radix_attention import RadixAttention
+from sglang.srt.managers.router.model_runner import InputMetadata
+
 
 class StablelmMLP(nn.Module):
     def __init__(
-        self, config: PretrainedConfig, linear_method: Optional[LinearMethodBase] = None
+        self, config: PretrainedConfig, quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
         self.hidden_size = config.hidden_size
         self.intermediate_size = config.intermediate_size
         self.gate_up_proj = MergedColumnParallelLinear(
             config.hidden_size,
             [config.intermediate_size] * 2,
             bias=False,
-            linear_method=linear_method,
+            quant_config=quant_config,
         )
         self.down_proj = RowParallelLinear(
-            config.intermediate_size, config.hidden_size, bias=False
+            config.intermediate_size, config.hidden_size, bias=False, quant_config=quant_config,
         )
         self.act_fn = SiluAndMul()
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         gate_up, _ = self.gate_up_proj(x)
         x = self.act_fn(gate_up)
         x, _ = self.down_proj(x)
@@ -58,15 +60,15 @@
 
 
 class StablelmAttention(nn.Module):
     def __init__(
         self,
         config: PretrainedConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
         self.hidden_size = config.hidden_size
         tp_size = get_tensor_model_parallel_world_size()
         self.total_num_heads = config.num_attention_heads
         self.num_heads = self.total_num_heads // tp_size
@@ -100,21 +102,19 @@
 
         self.qkv_proj = QKVParallelLinear(
             self.hidden_size,
             self.head_dim,
             self.total_num_heads,
             self.total_num_key_value_heads,
             self.qkv_bias,
-            linear_method=linear_method,
         )
         self.o_proj = RowParallelLinear(
             self.total_num_heads * self.head_dim,
             self.hidden_size,
             bias=False,
-            linear_method=linear_method,
         )
         self.rotary_emb = get_rope(
             self.head_dim,
             rotary_dim=self.rotary_ndims,
             max_position=self.config.max_position_embeddings,
             base=self.config.rope_theta,
         )
@@ -141,19 +141,19 @@
 
 
 class StablelmDecoderLayer(nn.Module):
     def __init__(
         self,
         config: PretrainedConfig,
         layer_id: int = 0,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.self_attn = StablelmAttention(config, layer_id=layer_id)
-        self.mlp = StablelmMLP(config, linear_method)
+        self.mlp = StablelmMLP(config, quant_config=quant_config)
         norm_eps = getattr(config, "norm_eps", getattr(config, "layer_norm_eps", 1e-05))
         self.input_layernorm = nn.LayerNorm(config.hidden_size, eps=norm_eps)
         self.post_attention_layernorm = nn.LayerNorm(config.hidden_size, eps=norm_eps)
 
     def forward(
         self,
         positions: torch.Tensor,
@@ -177,24 +177,24 @@
         hidden_states = residual + hidden_states
 
         return hidden_states, residual
 
 
 class StableLMEpochModel(nn.Module):
     def __init__(
-        self, config: PretrainedConfig, linear_method: Optional[LinearMethodBase] = None
+        self, config: PretrainedConfig, quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.embed_tokens = VocabParallelEmbedding(
             config.vocab_size,
             config.hidden_size,
         )
         self.layers = nn.ModuleList(
             [
-                StablelmDecoderLayer(config, i, linear_method)
+                StablelmDecoderLayer(config, i, quant_config=quant_config)
                 for i in range(config.num_hidden_layers)
             ]
         )
         norm_eps = getattr(config, "norm_eps", getattr(config, "layer_norm_eps", 1e-05))
         self.norm = nn.LayerNorm(config.hidden_size, eps=norm_eps)
 
     def forward(
@@ -219,20 +219,20 @@
         return hidden_states
 
 
 class StableLmForCausalLM(nn.Module):
     def __init__(
         self,
         config: PretrainedConfig,
-        linear_method: Optional[LinearMethodBase] = None,
+        quant_config: Optional[QuantizationConfig] = None,
     ) -> None:
         super().__init__()
         self.config = config
-        self.linear_method = linear_method
-        self.model = StableLMEpochModel(config, linear_method)
+        self.quant_config = quant_config
+        self.model = StableLMEpochModel(config, quant_config=quant_config)
         self.lm_head = ParallelLMHead(config.vocab_size, config.hidden_size)
         self.logits_processor = LogitsProcessor(config)
 
     def forward(
         self,
         input_ids: torch.Tensor,
         positions: torch.Tensor,
```

### Comparing `dblcsgen-0.2.6/sglang/srt/models/yivl.py` & `dblcsgen-0.2.7/sglang/srt/models/yivl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Inference-only Yi-VL model."""
 
 import os
 from typing import List, Optional
 
 import torch
 import torch.nn as nn
+from transformers import CLIPVisionModel, LlavaConfig
+from sglang.srt.weight_utils import (
+    default_weight_loader,
+    hf_model_weights_iterator,
+)
+
 from sglang.srt.models.llava import (
     LlavaLlamaForCausalLM,
     clip_vision_embed_forward,
     monkey_path_clip_vision_embed_forward,
 )
-from transformers import CLIPVisionModel, LlavaConfig
-from vllm.model_executor.weight_utils import (
-    default_weight_loader,
-    hf_model_weights_iterator,
-)
 
 
 class YiVLForCausalLM(LlavaLlamaForCausalLM):
     def __init__(self, *args, **kwargs):
         self.config = kwargs["config"]
         super().__init__(self.config)
```

### Comparing `dblcsgen-0.2.6/sglang/srt/sampling_params.py` & `dblcsgen-0.2.7/sglang/srt/sampling_params.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,28 @@
         temperature: float = 1.0,
         top_p: float = 1.0,
         top_k: int = -1,
         frequency_penalty: float = 0.0,
         presence_penalty: float = 0.0,
         ignore_eos: bool = False,
         skip_special_tokens: bool = True,
+        spaces_between_special_tokens: bool = True,
         dtype: Optional[str] = None,
         regex: Optional[str] = None,
     ) -> None:
         self.temperature = temperature
         self.top_p = top_p
         self.top_k = top_k
         self.frequency_penalty = frequency_penalty
         self.presence_penalty = presence_penalty
         self.stop_strs = stop
         self.max_new_tokens = max_new_tokens
         self.ignore_eos = ignore_eos
         self.skip_special_tokens = skip_special_tokens
+        self.spaces_between_special_tokens = spaces_between_special_tokens
         self.dtype = dtype
         self.regex = regex
 
         # Process some special cases
         if self.temperature < _SAMPLING_EPS:
             self.temperature = 1.0
             self.top_k = 1
```

### Comparing `dblcsgen-0.2.6/sglang/srt/server_args.py` & `dblcsgen-0.2.7/sglang/srt/server_args.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,55 @@
+"""The arguments of the server."""
+
 import argparse
 import dataclasses
 from typing import List, Optional, Union
 
 
 @dataclasses.dataclass
 class ServerArgs:
+    # Model and tokenizer
     model_path: str
     tokenizer_path: Optional[str] = None
-    host: str = "127.0.0.1"
-    port: int = 30000
-    additional_ports: Optional[Union[List[int], int]] = None
     load_format: str = "auto"
     tokenizer_mode: str = "auto"
     chat_template: Optional[str] = None
     trust_remote_code: bool = True
+    context_length: Optional[int] = None
+
+    # Port
+    host: str = "127.0.0.1"
+    port: int = 30000
+    additional_ports: Optional[Union[List[int], int]] = None
+
+    # Memory and scheduling
     mem_fraction_static: Optional[float] = None
     max_prefill_num_token: Optional[int] = None
-    context_length: Optional[int] = None
-    tp_size: int = 1
     schedule_heuristic: str = "lpm"
     schedule_conservativeness: float = 1.0
-    attention_reduce_in_fp32: bool = False
-    random_seed: int = 42
+
+    # Other runtime options
+    tp_size: int = 1
     stream_interval: int = 8
+    random_seed: int = 42
+
+    # Logging
+    log_level: str = "info"
+    log_requests: bool = False
     disable_log_stats: bool = False
     log_stats_interval: int = 10
-    log_level: str = "info"
-    api_key: str = ""
     show_time_cost: bool = False
 
-    # optional modes
-    disable_radix_cache: bool = False
+    # Other
+    api_key: str = ""
+
+    # Optimization/debug options
     enable_flashinfer: bool = False
+    attention_reduce_in_fp32: bool = False
+    disable_radix_cache: bool = False
     disable_regex_jump_forward: bool = False
     disable_disk_cache: bool = False
 
     def __post_init__(self):
         if self.tokenizer_path is None:
             self.tokenizer_path = self.model_path
         if self.mem_fraction_static is None:
@@ -62,23 +76,24 @@
         )
         parser.add_argument(
             "--tokenizer-path",
             type=str,
             default=ServerArgs.tokenizer_path,
             help="The path of the tokenizer.",
         )
-        parser.add_argument("--host", type=str, default=ServerArgs.host)
-        parser.add_argument("--port", type=int, default=ServerArgs.port)
-        # we want to be able to pass a list of ports
+        parser.add_argument("--host", type=str, default=ServerArgs.host,
+                            help="The host of the server.")
+        parser.add_argument("--port", type=int, default=ServerArgs.port,
+                            help="The port of the server.")
         parser.add_argument(
             "--additional-ports",
             type=int,
             nargs="*",
             default=[],
-            help="Additional ports specified for launching server.",
+            help="Additional ports specified for the server.",
         )
         parser.add_argument(
             "--load-format",
             type=str,
             default=ServerArgs.load_format,
             choices=["auto", "pt", "safetensors", "npcache", "dummy"],
             help="The format of the model weights to load. "
@@ -109,105 +124,111 @@
         )
         parser.add_argument(
             "--trust-remote-code",
             action="store_true",
             help="Whether or not to allow for custom models defined on the Hub in their own modeling files.",
         )
         parser.add_argument(
+            "--context-length",
+            type=int,
+            default=ServerArgs.context_length,
+            help="The model's maximum context length. Defaults to None (will use the value from the model's config.json instead).",
+        )
+        parser.add_argument(
             "--mem-fraction-static",
             type=float,
             default=ServerArgs.mem_fraction_static,
             help="The fraction of the memory used for static allocation (model weights and KV cache memory pool). Use a smaller value if you see out-of-memory errors.",
         )
         parser.add_argument(
             "--max-prefill-num-token",
             type=int,
             default=ServerArgs.max_prefill_num_token,
             help="The maximum number of tokens in a prefill batch. The real bound will be the maximum of this value and the model's maximum context length.",
         )
         parser.add_argument(
-            "--context-length",
-            type=int,
-            default=ServerArgs.context_length,
-            help="The model's maximum context length. Use this to reduce the context length to save memory. Defaults to None (will use the value from the model's config.json instead).",
-        )
-        parser.add_argument(
-            "--tp-size",
-            type=int,
-            default=ServerArgs.tp_size,
-            help="Tensor parallelism degree.",
-        )
-        parser.add_argument(
             "--schedule-heuristic",
             type=str,
             default=ServerArgs.schedule_heuristic,
-            help="Schudule mode: [lpm, weight, random, fcfs]",
+            choices=["lpm", "random", "fcfs", "dfs-weight"],
+            help="Scheduling Heuristic.",
         )
         parser.add_argument(
             "--schedule-conservativeness",
             type=float,
             default=ServerArgs.schedule_conservativeness,
             help="How conservative the schedule policy is. A larger value means more conservative scheduling. Use a larger value if you see requests being retracted frequently.",
         )
         parser.add_argument(
-            "--random-seed",
+            "--tp-size",
             type=int,
-            default=ServerArgs.random_seed,
-            help="Random seed.",
-        )
-        parser.add_argument(
-            "--attention-reduce-in-fp32",
-            action="store_true",
-            help="Cast the intermidiate attention results to fp32 to avoid possible crashes related to fp16.",
+            default=ServerArgs.tp_size,
+            help="Tensor parallelism size.",
         )
         parser.add_argument(
             "--stream-interval",
             type=int,
             default=ServerArgs.stream_interval,
             help="The interval (or buffer size) for streaming in terms of the token length. A smaller value makes streaming smoother, while a larger value makes the throughput higher",
         )
         parser.add_argument(
+            "--random-seed",
+            type=int,
+            default=ServerArgs.random_seed,
+            help="Random seed.",
+        )
+        parser.add_argument(
             "--log-level",
             type=str,
             default=ServerArgs.log_level,
-            help="Log level",
+            help="Logging level",
+        )
+        parser.add_argument(
+            "--log-requests",
+            action="store_true",
+            help="Log all requests",
         )
         parser.add_argument(
             "--disable-log-stats",
             action="store_true",
             help="Disable logging throughput stats.",
         )
         parser.add_argument(
             "--log-stats-interval",
             type=int,
             default=ServerArgs.log_stats_interval,
             help="Log stats interval in second.",
         )
         parser.add_argument(
+            "--show-time-cost",
+            action="store_true",
+            help="Show time cost of custom marks",
+        )
+        parser.add_argument(
             "--api-key",
             type=str,
             default=ServerArgs.api_key,
-            help="Set API Key",
+            help="Set API key of the server",
         )
+
+        # Optimization/debug options
         parser.add_argument(
-            "--show-time-cost",
+            "--enable-flashinfer",
             action="store_true",
-            help="Show time cost of custom marks",
+            help="Enable flashinfer inference kernels",
         )
-
-        # optional modes
         parser.add_argument(
-            "--disable-radix-cache",
+            "--attention-reduce-in-fp32",
             action="store_true",
-            help="Disable RadixAttention",
+            help="Cast the intermidiate attention results to fp32 to avoid possible crashes related to fp16.",
         )
         parser.add_argument(
-            "--enable-flashinfer",
+            "--disable-radix-cache",
             action="store_true",
-            help="Enable flashinfer inference kernels",
+            help="Disable RadixAttention",
         )
         parser.add_argument(
             "--disable-regex-jump-forward",
             action="store_true",
             help="Disable regex jump-forward",
         )
         parser.add_argument(
@@ -220,24 +241,24 @@
     def from_cli_args(cls, args: argparse.Namespace):
         attrs = [attr.name for attr in dataclasses.fields(cls)]
         return cls(**{attr: getattr(args, attr) for attr in attrs})
 
     def url(self):
         return f"http://{self.host}:{self.port}"
 
-    def get_optional_modes_logging(self):
+    def print_mode_args(self):
         return (
-            f"disable_radix_cache={self.disable_radix_cache}, "
             f"enable_flashinfer={self.enable_flashinfer}, "
+            f"attention_reduce_in_fp32={self.attention_reduce_in_fp32}, "
+            f"disable_radix_cache={self.disable_radix_cache}, "
             f"disable_regex_jump_forward={self.disable_regex_jump_forward}, "
             f"disable_disk_cache={self.disable_disk_cache}, "
-            f"attention_reduce_in_fp32={self.attention_reduce_in_fp32}"
         )
 
 
 @dataclasses.dataclass
 class PortArgs:
     tokenizer_port: int
     router_port: int
     detokenizer_port: int
     nccl_port: int
-    model_rpc_ports: List[int]
+    model_rpc_ports: List[int]
```

### Comparing `dblcsgen-0.2.6/sglang/srt/utils.py` & `dblcsgen-0.2.7/sglang/srt/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+"""Common utilities."""
+
 import base64
 import os
 import random
 import socket
-import sys
 import time
-import traceback
+from importlib.metadata import PackageNotFoundError, version
 from io import BytesIO
 from typing import List, Optional
 
 import numpy as np
+import pydantic
 import requests
 import torch
+from fastapi.responses import JSONResponse
+from packaging import version as pkg_version
+from pydantic import BaseModel
+from starlette.middleware.base import BaseHTTPMiddleware
+
+from sglang.utils import get_exception_traceback
 
 show_time_cost = False
 time_infos = {}
 
 
 def enable_show_time_cost():
     global show_time_cost
@@ -78,14 +86,40 @@
             return result
 
         return inner_func
 
     return wrapper
 
 
+def get_available_gpu_memory(gpu_id, distributed=True):
+    """
+    Get available memory for cuda:gpu_id device.
+    When distributed is True, the available memory is the minimum available memory of all GPUs.
+    """
+    num_gpus = torch.cuda.device_count()
+    assert gpu_id < num_gpus
+
+    if torch.cuda.current_device() != gpu_id:
+        print(
+            f"WARNING: current device is not {gpu_id}, but {torch.cuda.current_device()}, ",
+            "which may cause useless memory allocation for torch CUDA context.",
+        )
+
+    free_gpu_memory, _ = torch.cuda.mem_get_info(gpu_id)
+
+    if distributed:
+        tensor = torch.tensor(free_gpu_memory, dtype=torch.float32).to(
+            torch.device("cuda", gpu_id)
+        )
+        torch.distributed.all_reduce(tensor, op=torch.distributed.ReduceOp.MIN)
+        free_gpu_memory = tensor.item()
+
+    return free_gpu_memory / (1 << 30)
+
+
 def set_random_seed(seed: int) -> None:
     random.seed(seed)
 
     torch.manual_seed(seed)
     if torch.cuda.is_available():
         torch.cuda.manual_seed_all(seed)
 
@@ -114,15 +148,15 @@
             s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             s.bind(("", port))
             return True
         except socket.error:
             return False
 
 
-def handle_port_init(
+def allocate_init_ports(
     port: Optional[int] = None,
     additional_ports: Optional[List[int]] = None,
     tp_size: int = 1,
 ):
     port = 30000 if port is None else port
     additional_ports = [] if additional_ports is None else additional_ports
     additional_ports = (
@@ -146,23 +180,15 @@
         )
         can_use_ports.extend(addtional_can_use_ports)
 
     additional_ports = can_use_ports[: 4 + tp_size]
     return port, additional_ports
 
 
-def get_exception_traceback():
-    etype, value, tb = sys.exc_info()
-    err_str = "".join(traceback.format_exception(etype, value, tb))
-    return err_str
-
-
 def get_int_token_logit_bias(tokenizer, vocab_size):
-    from transformers import LlamaTokenizer, LlamaTokenizerFast
-
     # a bug when model's vocab size > tokenizer.vocab_size
     vocab_size = tokenizer.vocab_size
     logit_bias = np.zeros(vocab_size, dtype=np.float32)
     for t_id in range(vocab_size):
         ss = tokenizer.decode([t_id]).strip()
         if not (ss.isdigit() or len(ss) == 0 or t_id == tokenizer.eos_token_id):
             logit_bias[t_id] = -1e5
@@ -263,7 +289,49 @@
     elif image_file.startswith("data:"):
         image_file = image_file.split(",")[1]
         image = Image.open(BytesIO(base64.b64decode(image_file)))
     else:
         image = Image.open(BytesIO(base64.b64decode(image_file)))
 
     return image
+
+
+def assert_pkg_version(pkg: str, min_version: str):
+    try:
+        installed_version = version(pkg)
+        if pkg_version.parse(installed_version) < pkg_version.parse(min_version):
+            raise Exception(
+                f"{pkg} is installed with version {installed_version} which "
+                f"is less than the minimum required version {min_version}"
+            )
+    except PackageNotFoundError:
+        raise Exception(f"{pkg} with minimum required version {min_version} is not installed")
+
+
+API_KEY_HEADER_NAME = "X-API-Key"
+
+
+class APIKeyValidatorMiddleware(BaseHTTPMiddleware):
+    def __init__(self, app, api_key: str):
+        super().__init__(app)
+        self.api_key = api_key
+
+    async def dispatch(self, request, call_next):
+        # extract API key from the request headers
+        api_key_header = request.headers.get(API_KEY_HEADER_NAME)
+        if not api_key_header or api_key_header != self.api_key:
+            return JSONResponse(
+                status_code=403,
+                content={"detail": "Invalid API Key"},
+            )
+        response = await call_next(request)
+        return response
+
+
+# FIXME: Remove this once we drop support for pydantic 1.x
+IS_PYDANTIC_1 = int(pydantic.VERSION.split(".")[0]) == 1
+
+
+def jsonify_pydantic_model(obj: BaseModel):
+    if IS_PYDANTIC_1:
+        return obj.json(ensure_ascii=False)
+    return obj.model_dump_json()
```

### Comparing `dblcsgen-0.2.6/sglang/test/test_conversation.py` & `dblcsgen-0.2.7/sglang/test/test_conversation.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/test/test_openai_protocol.py` & `dblcsgen-0.2.7/sglang/test/test_openai_protocol.py`

 * *Files identical despite different names*

### Comparing `dblcsgen-0.2.6/sglang/test/test_programs.py` & `dblcsgen-0.2.7/sglang/test/test_programs.py`

 * *Files 6% similar despite different names*

```diff
@@ -222,42 +222,42 @@
     )
     answer = ret["answer"].lower()
     assert "finland" in answer or "states" in answer
 
 
 def test_parallel_decoding():
     max_tokens = 64
-    number = 5
+    fork_size = 5
 
     @sgl.function
     def parallel_decoding(s, topic):
         s += "Act as a helpful assistant.\n"
         s += "USER: Give some tips for " + topic + ".\n"
         s += (
             "ASSISTANT: Okay. Here are "
-            + str(number)
+            + str(fork_size)
             + " concise tips, each under 8 words:\n"
         )
 
         # Generate skeleton
-        for i in range(1, 1 + number):
+        for i in range(1, 1 + fork_size):
             s += f"{i}." + sgl.gen(max_tokens=16, stop=[".", "\n"]) + ".\n"
 
         # Generate detailed tips
-        forks = s.fork(number)
-        for i in range(number):
+        forks = s.fork(fork_size)
+        for i in range(fork_size):
             forks[
                 i
             ] += f"Now, I expand tip {i+1} into a detailed paragraph:\nTip {i+1}:"
             forks[i] += sgl.gen("detailed_tip", max_tokens, stop=["\n\n"])
         forks.join()
 
         # Concatenate tips and summarize
         s += "Here are these tips with detailed explanation:\n"
-        for i in range(number):
+        for i in range(fork_size):
             s += f"Tip {i+1}:" + forks[i]["detailed_tip"] + "\n"
 
         s += "\nIn summary," + sgl.gen("summary", max_tokens=512)
 
     ret = parallel_decoding.run(topic="writing a good blog post", temperature=0.3)
 
 
@@ -292,15 +292,15 @@
     if check_answer:
         assert "Noah" in answer
 
 
 def test_image_qa():
     @sgl.function
     def image_qa(s, question):
-        s += sgl.user(sgl.image("test_image.png") + question)
+        s += sgl.user(sgl.image("example_image.png") + question)
         s += sgl.assistant(sgl.gen("answer"))
 
     state = image_qa.run(
         question="Please describe this image in simple words.",
         temperature=0,
         max_new_tokens=64,
     )
@@ -309,14 +309,15 @@
         or "car" in state.messages()[-1]["content"]
     )
 
 
 def test_stream():
     @sgl.function
     def qa(s, question):
+        s += sgl.system("You are a helpful assistant.")
         s += sgl.user(question)
         s += sgl.assistant(sgl.gen("answer"))
 
     ret = qa(
         question="Compose an engaging travel blog post about a recent trip to Hawaii, highlighting cultural experiences and must-see attractions.",
         stream=True,
     )
```

### Comparing `dblcsgen-0.2.6/sglang/utils.py` & `dblcsgen-0.2.7/sglang/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,25 @@
 """Common utilities."""
 
 import base64
 import json
+import sys
 import threading
+import traceback
 import urllib.request
 from io import BytesIO
 from json import dumps
 
 import requests
 
 
-def get_available_gpu_memory(gpu_id, distributed=True):
-    """
-    Get available memory for cuda:gpu_id device.
-    When distributed is True, the available memory is the minimum available memory of all GPUs.
-    """
-    import torch
-
-    num_gpus = torch.cuda.device_count()
-    assert gpu_id < num_gpus
-
-    if torch.cuda.current_device() != gpu_id:
-        print(
-            f"WARNING: current device is not {gpu_id}, but {torch.cuda.current_device()}, ",
-            "which may cause useless memory allocation for torch CUDA context.",
-        )
-
-    free_gpu_memory, _ = torch.cuda.mem_get_info(gpu_id)
-
-    if distributed:
-        tensor = torch.tensor(free_gpu_memory, dtype=torch.float32).to(
-            torch.device("cuda", gpu_id)
-        )
-        torch.distributed.all_reduce(tensor, op=torch.distributed.ReduceOp.MIN)
-        free_gpu_memory = tensor.item()
-
-    return free_gpu_memory / (1 << 30)
+def get_exception_traceback():
+    etype, value, tb = sys.exc_info()
+    err_str = "".join(traceback.format_exception(etype, value, tb))
+    return err_str
 
 
 def is_same_type(values):
     """Return whether the elements in values are of the same type."""
     if len(values) <= 1:
         return True
     else:
@@ -186,8 +166,8 @@
     t.join(timeout=timeout)
     if t.is_alive():
         raise TimeoutError()
 
     if not ret_value:
         raise RuntimeError()
 
-    return ret_value[0]
+    return ret_value[0]
```

