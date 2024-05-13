# Comparing `tmp/taskingai-0.2.3.tar.gz` & `tmp/taskingai-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskingai-0.2.3.tar", last modified: Sat Apr 27 09:58:48 2024, max compression
+gzip compressed data, was "taskingai-0.2.4.tar", last modified: Mon May 13 12:19:35 2024, max compression
```

## Comparing `taskingai-0.2.3.tar` & `taskingai-0.2.4.tar`

### file list

```diff
@@ -1,213 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 09:55:50.000000 taskingai-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-27 09:58:48.903429 taskingai-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-27 09:55:50.000000 taskingai-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-27 09:55:50.000000 taskingai-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 09:58:48.903429 taskingai-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-27 09:55:50.000000 taskingai-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.871429 taskingai-0.2.3/taskingai/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.871429 taskingai-0.2.3/taskingai/assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/assistant/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/assistant/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/assistant/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.875429 taskingai-0.2.3/taskingai/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.879429 taskingai-0.2.3/taskingai/client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_bulk_create_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_create_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_delete_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_generate_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_get_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_assistants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_chats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_list_records.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_query_collection_chunks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_run_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/apis/api_update_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.879429 taskingai-0.2.3/taskingai/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.887429 taskingai-0.2.3/taskingai/client/models/entities/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action_authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action_body_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/action_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/assistant_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/assistant_memory_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_assistant_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_finish_reason.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_call.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_parameters_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_system_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_completion_user_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chat_memory_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/file_id_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/message_chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/message_content.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/message_generation_log.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/message_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/record_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/retrieval_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/retrieval_method.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/retrieval_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/retrieval_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/sort_order_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/status.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/text_embedding_input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/text_embedding_output.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/text_splitter_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/tool_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/tool_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/entities/upload_file_purpose.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.899429 taskingai-0.2.3/taskingai/client/models/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_bulk_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_bulk_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_run_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_run_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/action_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/assistant_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/base_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/base_empty_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_completion_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_completion_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chat_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_query_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/chunk_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/collection_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_generate_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_generate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/message_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_create_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_get_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/record_update_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/text_embedding_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/text_embedding_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/models/schemas/upload_file_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19459 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.899429 taskingai-0.2.3/taskingai/client/stream_apis/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/stream_apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/stream_apis/stream_api_chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/stream_apis/stream_api_message_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/taskingai/file/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/taskingai/inference/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/inference/chat_completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/inference/text_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/taskingai/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/retrieval/chunk.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/retrieval/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/retrieval/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/retrieval/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/taskingai/tool/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-04-27 09:55:50.000000 taskingai-0.2.3/taskingai/tool/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 09:58:48.903429 taskingai-0.2.3/taskingai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-04-27 09:58:48.000000 taskingai-0.2.3/taskingai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-04-27 09:58:48.000000 taskingai-0.2.3/taskingai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 09:58:48.000000 taskingai-0.2.3/taskingai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-27 09:58:48.000000 taskingai-0.2.3/taskingai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-27 09:58:48.000000 taskingai-0.2.3/taskingai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.615017 taskingai-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 12:16:26.000000 taskingai-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-13 12:19:35.611016 taskingai-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-13 12:16:26.000000 taskingai-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-13 12:16:26.000000 taskingai-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:19:35.615017 taskingai-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-13 12:16:26.000000 taskingai-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.579016 taskingai-0.2.4/taskingai/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.579016 taskingai-0.2.4/taskingai/assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/assistant/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/assistant/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8842 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/assistant/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.583016 taskingai-0.2.4/taskingai/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22868 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.587016 taskingai-0.2.4/taskingai/client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_bulk_create_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2388 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_create_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_delete_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_generate_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_get_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_assistants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_chats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_list_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_query_collection_chunks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_run_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/apis/api_update_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7762 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.587016 taskingai-0.2.4/taskingai/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.599017 taskingai-0.2.4/taskingai/client/models/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action_authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action_body_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/action_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/assistant_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/assistant_memory_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_assistant_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_finish_reason.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_parameters_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_parameters_property_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_system_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_completion_user_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chat_memory_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/file_id_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/message_chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/message_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/message_generation_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/message_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/record_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/retrieval_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/retrieval_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/retrieval_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/retrieval_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/sort_order_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/text_embedding_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/text_embedding_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/text_embedding_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/text_splitter_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/tool_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/tool_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/entities/upload_file_purpose.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/client/models/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_bulk_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_bulk_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_run_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/action_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/assistant_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/base_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/base_empty_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_completion_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_completion_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chat_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_query_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/chunk_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/collection_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_generate_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_generate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/message_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_create_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_get_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/record_update_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/text_embedding_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/text_embedding_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/models/schemas/upload_file_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19459 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/client/stream_apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/stream_apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/stream_apis/stream_api_chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/stream_apis/stream_api_message_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/inference/chat_completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/inference/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8210 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/retrieval/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/retrieval/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11072 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/retrieval/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/retrieval/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-05-13 12:16:26.000000 taskingai-0.2.4/taskingai/tool/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:19:35.611016 taskingai-0.2.4/taskingai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5638 2024-05-13 12:19:35.000000 taskingai-0.2.4/taskingai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9549 2024-05-13 12:19:35.000000 taskingai-0.2.4/taskingai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:19:35.000000 taskingai-0.2.4/taskingai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 12:19:35.000000 taskingai-0.2.4/taskingai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 12:19:35.000000 taskingai-0.2.4/taskingai.egg-info/top_level.txt
```

### Comparing `taskingai-0.2.3/PKG-INFO` & `taskingai-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskingai
-Version: 0.2.3
+Version: 0.2.4
 Summary: TaskingAI
 Home-page: https://www.tasking.ai
 Author-email: support@tasking.ai
 Keywords: TaskingAI,LLM,AI
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
```

### Comparing `taskingai-0.2.3/README.md` & `taskingai-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/pyproject.toml` & `taskingai-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/setup.py` & `taskingai-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/assistant/assistant.py` & `taskingai-0.2.4/taskingai/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/assistant/chat.py` & `taskingai-0.2.4/taskingai/assistant/chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/assistant/memory.py` & `taskingai-0.2.4/taskingai/assistant/memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/assistant/message.py` & `taskingai-0.2.4/taskingai/assistant/message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/api_client.py` & `taskingai-0.2.4/taskingai/client/api_client.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/__init__.py` & `taskingai-0.2.4/taskingai/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_bulk_create_actions.py` & `taskingai-0.2.4/taskingai/client/apis/api_bulk_create_actions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_chat_completion.py` & `taskingai-0.2.4/taskingai/client/apis/api_chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_assistant.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_chat.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_chunk.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_collection.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_message.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_create_record.py` & `taskingai-0.2.4/taskingai/client/apis/api_create_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_action.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_assistant.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_chat.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_chunk.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_collection.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_message.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_delete_record.py` & `taskingai-0.2.4/taskingai/client/apis/api_delete_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_generate_message.py` & `taskingai-0.2.4/taskingai/client/apis/api_generate_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_action.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_assistant.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_chat.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_chunk.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_collection.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_message.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_get_record.py` & `taskingai-0.2.4/taskingai/client/apis/api_get_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_actions.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_actions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_assistants.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_assistants.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_chats.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_chats.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_chunks.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_chunks.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_collections.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_collections.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_messages.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_messages.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_list_records.py` & `taskingai-0.2.4/taskingai/client/apis/api_list_records.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_query_collection_chunks.py` & `taskingai-0.2.4/taskingai/client/apis/api_query_collection_chunks.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_run_action.py` & `taskingai-0.2.4/taskingai/client/apis/api_run_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_text_embedding.py` & `taskingai-0.2.4/taskingai/client/apis/api_text_embedding.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_action.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_assistant.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_chat.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_chunk.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_collection.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_message.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/apis/api_update_record.py` & `taskingai-0.2.4/taskingai/client/apis/api_update_record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/configuration.py` & `taskingai-0.2.4/taskingai/client/configuration.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/error_handling.py` & `taskingai-0.2.4/taskingai/client/error_handling.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/exceptions.py` & `taskingai-0.2.4/taskingai/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/__init__.py` & `taskingai-0.2.4/taskingai/client/models/entities/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,17 +26,19 @@
 from .chat_completion_chunk import *
 from .chat_completion_finish_reason import *
 from .chat_completion_function import *
 from .chat_completion_function_call import *
 from .chat_completion_function_message import *
 from .chat_completion_function_parameters import *
 from .chat_completion_function_parameters_property import *
+from .chat_completion_function_parameters_property_items import *
 from .chat_completion_message import *
 from .chat_completion_role import *
 from .chat_completion_system_message import *
+from .chat_completion_usage import *
 from .chat_completion_user_message import *
 from .chat_memory import *
 from .chat_memory_message import *
 from .chunk import *
 from .collection import *
 from .file_id_data import *
 from .message import *
@@ -50,12 +52,13 @@
 from .retrieval_method import *
 from .retrieval_ref import *
 from .retrieval_type import *
 from .sort_order_enum import *
 from .status import *
 from .text_embedding_input_type import *
 from .text_embedding_output import *
+from .text_embedding_usage import *
 from .text_splitter import *
 from .text_splitter_type import *
 from .tool_ref import *
 from .tool_type import *
 from .upload_file_purpose import *
```

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/action.py` & `taskingai-0.2.4/taskingai/client/models/entities/action.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,17 @@
 
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
-from typing import Optional, Any, Dict
+from typing import Any, Dict
 from .action_method import ActionMethod
-from .action_param import ActionParam
-from .action_param import ActionParam
 from .action_body_type import ActionBodyType
-from .action_param import ActionParam
-from .chat_completion_function import ChatCompletionFunction
 from .action_authentication import ActionAuthentication
 
 __all__ = ["Action"]
 
 
 class Action(BaseModel):
     action_id: str = Field(..., min_length=20, max_length=30)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/action_authentication.py` & `taskingai-0.2.4/taskingai/client/models/entities/action_authentication.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/assistant.py` & `taskingai-0.2.4/taskingai/client/models/entities/assistant.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/assistant_memory.py` & `taskingai-0.2.4/taskingai/client/models/entities/assistant_memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
 from .chat_completion_finish_reason import ChatCompletionFinishReason
 from .chat_completion_assistant_message import ChatCompletionAssistantMessage
+from .chat_completion_usage import ChatCompletionUsage
 
 __all__ = ["ChatCompletion"]
 
 
 class ChatCompletion(BaseModel):
     finish_reason: ChatCompletionFinishReason = Field(...)
     message: ChatCompletionAssistantMessage = Field(...)
     created_timestamp: int = Field(...)
+    usage: ChatCompletionUsage = Field(...)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_assistant_message.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_assistant_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_chunk.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_message.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_parameters.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_parameters.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_function_parameters_property.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_function_parameters_property.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
 from typing import Optional, List
-
+from .chat_completion_function_parameters_property_items import ChatCompletionFunctionParametersPropertyItems
 
 __all__ = ["ChatCompletionFunctionParametersProperty"]
 
 
 class ChatCompletionFunctionParametersProperty(BaseModel):
-    type: str = Field(..., pattern="^(string|number|integer|boolean)$")
-    description: str = Field("", max_length=256)
+    type: str = Field(..., pattern="^(string|number|integer|boolean|array)$")
+    description: str = Field("", max_length=512)
     enum: Optional[List[str]] = Field(None)
+    items: Optional[ChatCompletionFunctionParametersPropertyItems] = Field(None)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_system_message.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_system_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_completion_user_message.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_completion_user_message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chat_memory.py` & `taskingai-0.2.4/taskingai/client/models/entities/chat_memory.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/chunk.py` & `taskingai-0.2.4/taskingai/client/models/entities/chunk.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/collection.py` & `taskingai-0.2.4/taskingai/client/models/entities/collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/message.py` & `taskingai-0.2.4/taskingai/client/models/entities/message.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/message_generation_log.py` & `taskingai-0.2.4/taskingai/client/models/entities/message_generation_log.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/record.py` & `taskingai-0.2.4/taskingai/client/models/entities/record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/retrieval_config.py` & `taskingai-0.2.4/taskingai/client/models/entities/retrieval_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,8 +17,10 @@
 
 __all__ = ["RetrievalConfig"]
 
 
 class RetrievalConfig(BaseModel):
     top_k: int = Field(3, ge=1, le=20)
     max_tokens: Optional[int] = Field(None, ge=1, le=8192)
+    score_threshold: Optional[float] = Field(None, ge=0.0, le=1.0)
     method: RetrievalMethod = Field(...)
+    function_description: Optional[str] = Field(None, min_length=0, max_length=1024)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/entities/text_splitter.py` & `taskingai-0.2.4/taskingai/client/models/entities/text_splitter.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 Author: James Yao
 Organization: TaskingAI
 License: Apache 2.0
 """
 
 from pydantic import BaseModel, Field
-from typing import Optional
+from typing import Optional, List
 from .text_splitter_type import TextSplitterType
 
 __all__ = ["TextSplitter"]
 
 
 class TextSplitter(BaseModel):
-    type: TextSplitterType = Field(...)
+    type: TextSplitterType = Field("token")
     chunk_size: Optional[int] = Field(None, ge=50, le=1000)
     chunk_overlap: Optional[int] = Field(None, ge=0, le=200)
+    separators: Optional[List[str]] = Field(None, min_length=1, max_length=16)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/__init__.py` & `taskingai-0.2.4/taskingai/client/models/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/action_bulk_create_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/action_bulk_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/action_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/action_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/action_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/action_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/action_update_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/action_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/assistant_create_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/assistant_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/assistant_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/assistant_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/assistant_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/assistant_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/assistant_update_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/assistant_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/chat_completion_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/chat_completion_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 from ..entities.chat_completion_assistant_message import ChatCompletionAssistantMessage
 from ..entities.chat_completion_function import ChatCompletionFunction
 
 __all__ = ["ChatCompletionRequest"]
 
 
 class ChatCompletionRequest(BaseModel):
-    model_id: str = Field(..., min_length=8, max_length=8)
+    model_id: str = Field(..., min_length=1, max_length=255)
     configs: Optional[Dict] = Field(None)
     stream: bool = Field(False)
     messages: List[
         Union[
             ChatCompletionFunctionMessage,
             ChatCompletionAssistantMessage,
             ChatCompletionUserMessage,
             ChatCompletionSystemMessage,
         ]
     ] = Field(...)
     function_call: Optional[str] = Field(None)
     functions: Optional[List[ChatCompletionFunction]] = Field(None)
+    save_logs: bool = Field(False)
```

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/chat_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/chat_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/chat_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/chat_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/chunk_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/chunk_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/chunk_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/chunk_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/collection_create_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/collection_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/collection_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/collection_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/collection_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/collection_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/collection_update_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/collection_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/message_create_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/message_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/message_generate_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/message_generate_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/message_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/message_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/message_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/message_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/record_create_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/record_create_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/record_list_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/record_list_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/record_list_response.py` & `taskingai-0.2.4/taskingai/client/models/schemas/record_list_response.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/record_update_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/record_update_request.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/models/schemas/text_embedding_request.py` & `taskingai-0.2.4/taskingai/client/models/schemas/text_embedding_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,10 +15,10 @@
 from typing import Optional, List, Union
 from ..entities.text_embedding_input_type import TextEmbeddingInputType
 
 __all__ = ["TextEmbeddingRequest"]
 
 
 class TextEmbeddingRequest(BaseModel):
-    model_id: str = Field(..., min_length=8, max_length=8)
+    model_id: str = Field(..., min_length=1, max_length=255)
     input: Union[str, List[str]] = Field(...)
     input_type: Optional[TextEmbeddingInputType] = Field(None)
```

### Comparing `taskingai-0.2.3/taskingai/client/rest.py` & `taskingai-0.2.4/taskingai/client/rest.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/stream.py` & `taskingai-0.2.4/taskingai/client/stream.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/stream_apis/stream_api_chat_completion.py` & `taskingai-0.2.4/taskingai/client/stream_apis/stream_api_chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/stream_apis/stream_api_message_generation.py` & `taskingai-0.2.4/taskingai/client/stream_apis/stream_api_message_generation.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/client/utils.py` & `taskingai-0.2.4/taskingai/client/utils.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/config.py` & `taskingai-0.2.4/taskingai/config.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/exceptions.py` & `taskingai-0.2.4/taskingai/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/file/file.py` & `taskingai-0.2.4/taskingai/file/file.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/inference/chat_completion.py` & `taskingai-0.2.4/taskingai/inference/chat_completion.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/inference/text_embedding.py` & `taskingai-0.2.4/taskingai/inference/text_embedding.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/retrieval/chunk.py` & `taskingai-0.2.4/taskingai/retrieval/chunk.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,56 +244,60 @@
 
 
 def query_chunks(
     collection_id: str,
     *,
     query_text: str,
     top_k: int = 3,
+    score_threshold: Optional[float] = None,
     max_tokens: Optional[int] = None,
 ) -> List[Chunk]:
     """
     Query chunks in a collection.
     :param collection_id: The ID of the collection.
     :param query_text: The query text.
     :param top_k: The number of most relevant chunks to return.
     :param max_tokens: The maximum number of tokens to return.
     """
 
     # only add non-None parameters
     body = ChunkQueryRequest(
         top_k=top_k,
         query_text=query_text,
+        score_threshold=score_threshold,
         max_tokens=max_tokens,
     )
     response: ChunkQueryResponse = api_query_collection_chunks(
         collection_id=collection_id,
         payload=body,
     )
     return response.data
 
 
 async def a_query_chunks(
     collection_id: str,
     *,
     query_text: str,
     top_k: int = 3,
+    score_threshold: Optional[float] = None,
     max_tokens: Optional[int] = None,
 ) -> List[Chunk]:
     """
     Query chunks in a collection.
     :param collection_id: The ID of the collection.
     :param query_text: The query text.
     :param top_k: The number of most relevant chunks to return.
     :param max_tokens: The maximum number of tokens to return.
     """
 
     # only add non-None parameters
     body = ChunkQueryRequest(
         top_k=top_k,
         query_text=query_text,
+        score_threshold=score_threshold,
         max_tokens=max_tokens,
     )
     response: ChunkQueryResponse = await async_api_query_collection_chunks(
         collection_id=collection_id,
         payload=body,
     )
     return response.data
```

### Comparing `taskingai-0.2.3/taskingai/retrieval/collection.py` & `taskingai-0.2.4/taskingai/retrieval/collection.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/retrieval/record.py` & `taskingai-0.2.4/taskingai/retrieval/record.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai/tool/action.py` & `taskingai-0.2.4/taskingai/tool/action.py`

 * *Files identical despite different names*

### Comparing `taskingai-0.2.3/taskingai.egg-info/PKG-INFO` & `taskingai-0.2.4/taskingai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskingai
-Version: 0.2.3
+Version: 0.2.4
 Summary: TaskingAI
 Home-page: https://www.tasking.ai
 Author-email: support@tasking.ai
 Keywords: TaskingAI,LLM,AI
 Description-Content-Type: text/markdown
 Requires-Dist: certifi>=14.05.14
 Requires-Dist: six>=1.10
```

### Comparing `taskingai-0.2.3/taskingai.egg-info/SOURCES.txt` & `taskingai-0.2.4/taskingai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -84,17 +84,19 @@
 taskingai/client/models/entities/chat_completion_chunk.py
 taskingai/client/models/entities/chat_completion_finish_reason.py
 taskingai/client/models/entities/chat_completion_function.py
 taskingai/client/models/entities/chat_completion_function_call.py
 taskingai/client/models/entities/chat_completion_function_message.py
 taskingai/client/models/entities/chat_completion_function_parameters.py
 taskingai/client/models/entities/chat_completion_function_parameters_property.py
+taskingai/client/models/entities/chat_completion_function_parameters_property_items.py
 taskingai/client/models/entities/chat_completion_message.py
 taskingai/client/models/entities/chat_completion_role.py
 taskingai/client/models/entities/chat_completion_system_message.py
+taskingai/client/models/entities/chat_completion_usage.py
 taskingai/client/models/entities/chat_completion_user_message.py
 taskingai/client/models/entities/chat_memory.py
 taskingai/client/models/entities/chat_memory_message.py
 taskingai/client/models/entities/chunk.py
 taskingai/client/models/entities/collection.py
 taskingai/client/models/entities/file_id_data.py
 taskingai/client/models/entities/message.py
@@ -108,14 +110,15 @@
 taskingai/client/models/entities/retrieval_method.py
 taskingai/client/models/entities/retrieval_ref.py
 taskingai/client/models/entities/retrieval_type.py
 taskingai/client/models/entities/sort_order_enum.py
 taskingai/client/models/entities/status.py
 taskingai/client/models/entities/text_embedding_input_type.py
 taskingai/client/models/entities/text_embedding_output.py
+taskingai/client/models/entities/text_embedding_usage.py
 taskingai/client/models/entities/text_splitter.py
 taskingai/client/models/entities/text_splitter_type.py
 taskingai/client/models/entities/tool_ref.py
 taskingai/client/models/entities/tool_type.py
 taskingai/client/models/entities/upload_file_purpose.py
 taskingai/client/models/schemas/__init__.py
 taskingai/client/models/schemas/action_bulk_create_request.py
```

