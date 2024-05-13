# Comparing `tmp/xingchen-1.1.2.tar.gz` & `tmp/xingchen-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xingchen-1.1.2.tar", last modified: Sat May 11 01:41:23 2024, max compression
+gzip compressed data, was "xingchen-1.1.3.tar", last modified: Mon May 13 03:18:47 2024, max compression
```

## Comparing `xingchen-1.1.2.tar` & `xingchen-1.1.3.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.155467 xingchen-1.1.2/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-11 01:41:23.155549 xingchen-1.1.2/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)    11848 2024-05-02 15:15:25.000000 xingchen-1.1.2/README.md
--rw-r--r--   0 frankin    (501) staff       (20)      771 2024-05-02 15:02:56.000000 xingchen-1.1.2/pyproject.toml
--rw-r--r--   0 frankin    (501) staff       (20)       69 2024-05-11 01:41:23.155831 xingchen-1.1.2/setup.cfg
--rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-05-11 01:40:10.000000 xingchen-1.1.2/setup.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.121679 xingchen-1.1.2/test/
--rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.2/test/test_base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     3120 2024-04-11 03:27:03.000000 xingchen-1.1.2/test/test_base_chat_request_aca_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.2/test/test_character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.2/test/test_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.2/test/test_character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.2/test/test_character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.2/test/test_character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.2/test/test_chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.2/test/test_chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.2/test/test_message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.2/test/test_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.2/test/test_result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.2/test/test_result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.2/test/test_result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.2/test/test_sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.2/test/test_user_profile.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.124129 xingchen-1.1.2/xingchen/
--rw-r--r--   0 frankin    (501) staff       (20)     6865 2024-05-11 01:40:18.000000 xingchen-1.1.2/xingchen/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     3764 2024-05-09 03:46:30.000000 xingchen-1.1.2/xingchen/aca_util.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.128739 xingchen-1.1.2/xingchen/api/
--rw-r--r--   0 frankin    (501) staff       (20)      410 2024-04-25 08:50:36.000000 xingchen-1.1.2/xingchen/api/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)    60683 2024-04-25 09:41:08.000000 xingchen-1.1.2/xingchen/api/character_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    12628 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     8021 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_extract_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    29175 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/chat_message_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     7592 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/api/common_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     5384 2024-04-11 06:12:19.000000 xingchen-1.1.2/xingchen/api/groupchat_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)     5637 2024-05-09 11:02:34.000000 xingchen-1.1.2/xingchen/api/openai_api_sub.py
--rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/api_client.py
--rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/api_response.py
--rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/configuration.py
--rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/exceptions.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.148125 xingchen-1.1.2/xingchen/models/
--rw-r--r--   0 frankin    (501) staff       (20)     3374 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.2/xingchen/models/advanced_settings.py
--rw-r--r--   0 frankin    (501) staff       (20)     2618 2024-04-11 03:27:03.000000 xingchen-1.1.2/xingchen/models/base_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     4766 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/character_advanced_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.2/xingchen/models/character_create_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2023 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2345 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/character_desc_generated_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.2/xingchen/models/character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2686 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/character_permission_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/character_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/character_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     5138 2024-04-25 09:41:54.000000 xingchen-1.1.2/xingchen/models/character_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     4759 2024-04-25 09:19:54.000000 xingchen-1.1.2/xingchen/models/character_version_create_or_update_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.2/xingchen/models/chat_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/chat_history_query_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_history_query_where.py
--rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     6915 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/chat_req_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/chat_room_user_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.2/xingchen/models/context.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.149917 xingchen-1.1.2/xingchen/models/custom/
--rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/custom/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/custom/base_response.py
--rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.2/xingchen/models/custom/character_model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     4814 2024-05-09 03:25:22.000000 xingchen-1.1.2/xingchen/models/custom/chat_response.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.151471 xingchen-1.1.2/xingchen/models/custom/groupchat/
--rw-r--r--   0 frankin    (501) staff       (20)       92 2024-04-09 12:57:52.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     2778 2024-04-11 07:45:59.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_ext_param.py
--rw-r--r--   0 frankin    (501) staff       (20)     1763 2024-04-09 13:04:39.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_reply_setting.py
--rw-r--r--   0 frankin    (501) staff       (20)     1303 2024-04-11 02:56:10.000000 xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_room_info.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.155200 xingchen-1.1.2/xingchen/models/custom/openai/
--rw-r--r--   0 frankin    (501) staff       (20)        0 2024-05-09 01:43:25.000000 xingchen-1.1.2/xingchen/models/custom/openai/__init__.py
--rw-r--r--   0 frankin    (501) staff       (20)     1431 2024-05-09 06:12:12.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_choice.py
--rw-r--r--   0 frankin    (501) staff       (20)     4347 2024-05-09 03:51:49.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_req.py
--rw-r--r--   0 frankin    (501) staff       (20)     2254 2024-05-09 06:28:07.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_resp.py
--rw-r--r--   0 frankin    (501) staff       (20)     1767 2024-05-09 02:04:02.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_function.py
--rw-r--r--   0 frankin    (501) staff       (20)     2005 2024-05-09 02:22:04.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1733 2024-05-09 02:39:47.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_req_tool.py
--rw-r--r--   0 frankin    (501) staff       (20)     1627 2024-05-09 02:38:45.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_function.py
--rw-r--r--   0 frankin    (501) staff       (20)     2016 2024-05-09 06:18:11.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_message.py
--rw-r--r--   0 frankin    (501) staff       (20)     1855 2024-05-09 06:19:13.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_tool.py
--rw-r--r--   0 frankin    (501) staff       (20)     1655 2024-05-09 02:30:52.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_tool_choice.py
--rw-r--r--   0 frankin    (501) staff       (20)     1568 2024-05-09 01:57:55.000000 xingchen-1.1.2/xingchen/models/custom/openai/openai_usage.py
--rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.2/xingchen/models/custom/platform_publish_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.2/xingchen/models/custom/reset_history_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     1778 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_data.py
--rw-r--r--   0 frankin    (501) staff       (20)     2162 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2399 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/extract_memory_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1718 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1712 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/file_conver_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/file_info_vo.py
--rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.2/xingchen/models/function_call.py
--rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/gateway_context.py
--rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/gateway_issued_params.py
--rw-r--r--   0 frankin    (501) staff       (20)     2494 2024-04-11 07:26:08.000000 xingchen-1.1.2/xingchen/models/input.py
--rw-r--r--   0 frankin    (501) staff       (20)     1506 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/keyword.py
--rw-r--r--   0 frankin    (501) staff       (20)     1698 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/kv_memory_config.py
--rw-r--r--   0 frankin    (501) staff       (20)     2237 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/long_term_memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     2089 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/memory.py
--rw-r--r--   0 frankin    (501) staff       (20)     1582 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/memory_summary.py
--rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.2/xingchen/models/message.py
--rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/message_rating_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/meta.py
--rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.2/xingchen/models/model_parameters.py
--rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1681 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/platform_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2009 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     1965 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/reject_answer_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2303 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/reject_condition.py
--rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/repository.py
--rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/repository_info.py
--rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_boolean.py
--rw-r--r--   0 frankin    (501) staff       (20)     2561 2024-04-25 05:48:37.000000 xingchen-1.1.2/xingchen/models/result_dto_character_desc_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_character_key.py
--rw-r--r--   0 frankin    (501) staff       (20)     2517 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_extract_kv_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2573 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_extract_summary_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2539 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_file_conver_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_list_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_page_result_character_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/result_dto_page_result_chat_message_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2617 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/result_dto_polling_image_detail_dto.py
--rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.2/xingchen/models/scenario.py
--rw-r--r--   0 frankin    (501) staff       (20)     1702 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/stop_chat_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.2/xingchen/models/sys_reminder_request.py
--rw-r--r--   0 frankin    (501) staff       (20)     2193 2024-04-24 06:58:03.000000 xingchen-1.1.2/xingchen/models/text_to_image_plugin.py
--rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/models/user_profile.py
--rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/py.typed
--rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.2/xingchen/rest.py
-drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-11 01:41:23.125342 xingchen-1.1.2/xingchen.egg-info/
--rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/PKG-INFO
--rw-r--r--   0 frankin    (501) staff       (20)     5654 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/SOURCES.txt
--rw-r--r--   0 frankin    (501) staff       (20)        1 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/dependency_links.txt
--rw-r--r--   0 frankin    (501) staff       (20)       85 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/requires.txt
--rw-r--r--   0 frankin    (501) staff       (20)        9 2024-05-11 01:41:23.000000 xingchen-1.1.2/xingchen.egg-info/top_level.txt
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.466316 xingchen-1.1.3/
+-rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-13 03:18:47.466474 xingchen-1.1.3/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)    11956 2024-05-13 03:18:05.000000 xingchen-1.1.3/README.md
+-rw-r--r--   0 frankin    (501) staff       (20)      771 2024-05-02 15:02:56.000000 xingchen-1.1.3/pyproject.toml
+-rw-r--r--   0 frankin    (501) staff       (20)       69 2024-05-13 03:18:47.466912 xingchen-1.1.3/setup.cfg
+-rw-r--r--   0 frankin    (501) staff       (20)     1152 2024-05-13 03:17:11.000000 xingchen-1.1.3/setup.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.402433 xingchen-1.1.3/test/
+-rw-r--r--   0 frankin    (501) staff       (20)     1655 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2985 2024-03-05 07:23:56.000000 xingchen-1.1.3/test/test_base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3120 2024-04-11 03:27:03.000000 xingchen-1.1.3/test/test_base_chat_request_aca_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2206 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3105 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3052 2024-03-05 07:24:20.000000 xingchen-1.1.3/test/test_character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3728 2024-03-05 07:23:29.000000 xingchen-1.1.3/test/test_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1448 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1734 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1742 2024-03-05 07:24:07.000000 xingchen-1.1.3/test/test_character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1533 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3182 2024-03-05 07:24:03.000000 xingchen-1.1.3/test/test_character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3150 2024-03-05 07:23:52.000000 xingchen-1.1.3/test/test_character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2815 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2088 2024-03-05 07:23:33.000000 xingchen-1.1.3/test/test_chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1851 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1786 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2018 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4043 2024-03-05 07:25:26.000000 xingchen-1.1.3/test/test_chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1549 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1711 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1459 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1508 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1744 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1798 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1577 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1604 2024-03-05 07:23:48.000000 xingchen-1.1.3/test/test_message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1359 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1608 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4471 2024-03-05 07:22:54.000000 xingchen-1.1.3/test/test_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2507 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1486 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1720 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1629 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4244 2024-03-05 07:23:36.000000 xingchen-1.1.3/test/test_result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1805 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4549 2024-03-05 07:22:38.000000 xingchen-1.1.3/test/test_result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5085 2024-03-05 07:24:24.000000 xingchen-1.1.3/test/test_result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2970 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1368 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1654 2024-03-05 07:24:31.000000 xingchen-1.1.3/test/test_sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1496 2023-11-07 06:12:48.000000 xingchen-1.1.3/test/test_user_profile.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.405376 xingchen-1.1.3/xingchen/
+-rw-r--r--   0 frankin    (501) staff       (20)     6883 2024-05-13 03:18:18.000000 xingchen-1.1.3/xingchen/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3752 2024-05-11 09:43:24.000000 xingchen-1.1.3/xingchen/aca_util.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.410741 xingchen-1.1.3/xingchen/api/
+-rw-r--r--   0 frankin    (501) staff       (20)      410 2024-04-25 08:50:36.000000 xingchen-1.1.3/xingchen/api/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)    60683 2024-04-25 09:41:08.000000 xingchen-1.1.3/xingchen/api/character_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    12628 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/api/chat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     8021 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/api/chat_extract_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    29175 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/api/chat_message_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7592 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/api/common_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5622 2024-05-11 09:35:52.000000 xingchen-1.1.3/xingchen/api/completion_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5384 2024-04-11 06:12:19.000000 xingchen-1.1.3/xingchen/api/groupchat_api_sub.py
+-rw-r--r--   0 frankin    (501) staff       (20)    30795 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/api_client.py
+-rw-r--r--   0 frankin    (501) staff       (20)      852 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/api_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)    15709 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/configuration.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5442 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/exceptions.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.453596 xingchen-1.1.3/xingchen/models/
+-rw-r--r--   0 frankin    (501) staff       (20)     3374 2024-04-25 05:48:37.000000 xingchen-1.1.3/xingchen/models/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2725 2024-03-05 06:43:53.000000 xingchen-1.1.3/xingchen/models/advanced_settings.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2618 2024-04-11 03:27:03.000000 xingchen-1.1.3/xingchen/models/base_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4766 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/character_advanced_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4800 2024-03-07 08:00:22.000000 xingchen-1.1.3/xingchen/models/character_create_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2023 2024-04-25 05:48:37.000000 xingchen-1.1.3/xingchen/models/character_desc_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2345 2024-04-25 05:48:37.000000 xingchen-1.1.3/xingchen/models/character_desc_generated_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7409 2024-03-07 08:02:21.000000 xingchen-1.1.3/xingchen/models/character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2686 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2467 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/character_permission_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3094 2024-03-05 07:28:35.000000 xingchen-1.1.3/xingchen/models/character_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2273 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/character_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     5138 2024-04-25 09:41:54.000000 xingchen-1.1.3/xingchen/models/character_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4759 2024-04-25 09:19:54.000000 xingchen-1.1.3/xingchen/models/character_version_create_or_update_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2906 2024-03-05 03:00:03.000000 xingchen-1.1.3/xingchen/models/chat_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3097 2024-03-05 07:28:35.000000 xingchen-1.1.3/xingchen/models/chat_history_query_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2917 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/chat_history_query_where.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3943 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     6915 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/chat_req_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2722 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/chat_room_user_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3673 2024-02-04 06:24:45.000000 xingchen-1.1.3/xingchen/models/context.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.455996 xingchen-1.1.3/xingchen/models/custom/
+-rw-r--r--   0 frankin    (501) staff       (20)       89 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/custom/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1992 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/custom/base_response.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1873 2024-03-05 07:02:49.000000 xingchen-1.1.3/xingchen/models/custom/character_model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4821 2024-05-11 08:27:16.000000 xingchen-1.1.3/xingchen/models/custom/chat_response.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.462467 xingchen-1.1.3/xingchen/models/custom/completion/
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2024-05-09 01:43:25.000000 xingchen-1.1.3/xingchen/models/custom/completion/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1415 2024-05-11 09:25:04.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_choice.py
+-rw-r--r--   0 frankin    (501) staff       (20)     4326 2024-05-11 09:21:43.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_req.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1758 2024-05-11 09:21:43.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_req_function.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1996 2024-05-11 09:21:43.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_req_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1687 2024-05-11 09:25:04.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_req_tool.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2719 2024-05-11 09:25:04.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_resp.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1618 2024-05-11 09:21:43.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_function.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2006 2024-05-11 09:25:04.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1814 2024-05-11 09:25:42.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_tool.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1603 2024-05-11 09:25:29.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_tool_choice.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1553 2024-05-11 09:21:43.000000 xingchen-1.1.3/xingchen/models/custom/completion/completion_usage.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.465761 xingchen-1.1.3/xingchen/models/custom/groupchat/
+-rw-r--r--   0 frankin    (501) staff       (20)       92 2024-04-09 12:57:52.000000 xingchen-1.1.3/xingchen/models/custom/groupchat/__init__.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2778 2024-04-11 07:45:59.000000 xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_ext_param.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1763 2024-04-09 13:04:39.000000 xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_reply_setting.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1303 2024-04-11 02:56:10.000000 xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_room_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2026 2024-03-06 07:00:38.000000 xingchen-1.1.3/xingchen/models/custom/platform_publish_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1818 2024-02-01 06:33:25.000000 xingchen-1.1.3/xingchen/models/custom/reset_history_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1778 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/extract_data.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2162 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/extract_kv_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2399 2024-04-25 05:48:37.000000 xingchen-1.1.3/xingchen/models/extract_memory_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/extract_summary_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1718 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/file_conver_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1712 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/file_conver_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2191 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/file_info_vo.py
+-rw-r--r--   0 frankin    (501) staff       (20)     7800 2024-02-02 08:00:56.000000 xingchen-1.1.3/xingchen/models/function_call.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2239 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/gateway_context.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2417 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/gateway_issued_params.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2494 2024-04-11 07:26:08.000000 xingchen-1.1.3/xingchen/models/input.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1506 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/keyword.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1698 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/kv_memory_config.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2237 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/long_term_memory.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2089 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/memory.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1582 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/memory_summary.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2692 2024-01-29 06:06:46.000000 xingchen-1.1.3/xingchen/models/message.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2251 2024-03-05 07:28:35.000000 xingchen-1.1.3/xingchen/models/message_rating_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2057 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/meta.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2899 2024-01-29 05:42:57.000000 xingchen-1.1.3/xingchen/models/model_parameters.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2904 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2929 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1681 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/platform_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2009 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/polling_image_detail_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1965 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/reject_answer_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2303 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/reject_condition.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2290 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/repository.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2719 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/repository_info.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2578 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_boolean.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2561 2024-04-25 05:48:37.000000 xingchen-1.1.3/xingchen/models/result_dto_character_desc_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2893 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_character_key.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2517 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/result_dto_extract_kv_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2573 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/result_dto_extract_summary_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2539 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/result_dto_file_conver_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3110 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_list_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3015 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_page_result_character_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     3040 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/result_dto_page_result_chat_message_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2617 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/result_dto_polling_image_detail_dto.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2062 2023-11-21 03:10:04.000000 xingchen-1.1.3/xingchen/models/scenario.py
+-rw-r--r--   0 frankin    (501) staff       (20)     1702 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/stop_chat_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2386 2024-03-05 07:28:35.000000 xingchen-1.1.3/xingchen/models/sys_reminder_request.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2193 2024-04-24 06:58:03.000000 xingchen-1.1.3/xingchen/models/text_to_image_plugin.py
+-rw-r--r--   0 frankin    (501) staff       (20)     2177 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/models/user_profile.py
+-rw-r--r--   0 frankin    (501) staff       (20)        0 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/py.typed
+-rw-r--r--   0 frankin    (501) staff       (20)    12934 2023-11-07 06:12:48.000000 xingchen-1.1.3/xingchen/rest.py
+drwxr-xr-x   0 frankin    (501) staff       (20)        0 2024-05-13 03:18:47.406680 xingchen-1.1.3/xingchen.egg-info/
+-rw-r--r--   0 frankin    (501) staff       (20)      333 2024-05-13 03:18:47.000000 xingchen-1.1.3/xingchen.egg-info/PKG-INFO
+-rw-r--r--   0 frankin    (501) staff       (20)     5728 2024-05-13 03:18:47.000000 xingchen-1.1.3/xingchen.egg-info/SOURCES.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        1 2024-05-13 03:18:47.000000 xingchen-1.1.3/xingchen.egg-info/dependency_links.txt
+-rw-r--r--   0 frankin    (501) staff       (20)       85 2024-05-13 03:18:47.000000 xingchen-1.1.3/xingchen.egg-info/requires.txt
+-rw-r--r--   0 frankin    (501) staff       (20)        9 2024-05-13 03:18:47.000000 xingchen-1.1.3/xingchen.egg-info/top_level.txt
```

### Comparing `xingchen-1.1.2/README.md` & `xingchen-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -248,14 +248,17 @@
 
 7. 验证
 ```commandline
 pip install {包名}=={版本名} -i https://www.pypi.org/simple/
 ```
 
 ## 版本变更
+### 1.1.3
+- 添加completion对话接口 `xingchen.api.completion_api_sub.AcACompletionApiSub.completions`
+
 ### 1.1.1
 - 添加群聊逻辑 `GroupChatApiSub.chat(非流式)`, `GroupChatApiSub.streamOut(流式)` 
 - 添加通义万相图片轮训接口 `ChatMessageApiSub.polling_image_detail`
 - 添加角色描述自动生成接口 `CharacterApiSub.auto_generate_desc`
 - 添加角色记忆抽取接口 `ChatExtractMessageApiSub.extract_memory_kv`
 
 ### 1.1.0
```

### Comparing `xingchen-1.1.2/pyproject.toml` & `xingchen-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/setup.py` & `xingchen-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "xingchen"
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum",
     "sseclient-py >= 1.8.0"
```

### Comparing `xingchen-1.1.2/test/test_advanced_settings.py` & `xingchen-1.1.3/test/test_advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_base_chat_request.py` & `xingchen-1.1.3/test/test_base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_base_chat_request_aca_chat_ext_param.py` & `xingchen-1.1.3/test/test_base_chat_request_aca_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_advanced_config.py` & `xingchen-1.1.3/test/test_character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_api_sub.py` & `xingchen-1.1.3/test/test_character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_create_dto.py` & `xingchen-1.1.3/test/test_character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_dto.py` & `xingchen-1.1.3/test/test_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_key.py` & `xingchen-1.1.3/test/test_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_permission_config.py` & `xingchen-1.1.3/test/test_character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_query_dto.py` & `xingchen-1.1.3/test/test_character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_query_where.py` & `xingchen-1.1.3/test/test_character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_update_dto.py` & `xingchen-1.1.3/test/test_character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_character_version_create_or_update_dto.py` & `xingchen-1.1.3/test/test_character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_api_sub.py` & `xingchen-1.1.3/test/test_chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_history_query_dto.py` & `xingchen-1.1.3/test/test_chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_history_query_where.py` & `xingchen-1.1.3/test/test_chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_message_api_sub.py` & `xingchen-1.1.3/test/test_chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_message_dto.py` & `xingchen-1.1.3/test/test_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_req_params.py` & `xingchen-1.1.3/test/test_chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_chat_room_user_dto.py` & `xingchen-1.1.3/test/test_chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_context.py` & `xingchen-1.1.3/test/test_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_file_info_vo.py` & `xingchen-1.1.3/test/test_file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_gateway_context.py` & `xingchen-1.1.3/test/test_gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_gateway_issued_params.py` & `xingchen-1.1.3/test/test_gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_input.py` & `xingchen-1.1.3/test/test_input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_message.py` & `xingchen-1.1.3/test/test_message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_message_rating_request.py` & `xingchen-1.1.3/test/test_message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_meta.py` & `xingchen-1.1.3/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_model_parameters.py` & `xingchen-1.1.3/test/test_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_page_result_character_dto.py` & `xingchen-1.1.3/test/test_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_page_result_chat_message_dto.py` & `xingchen-1.1.3/test/test_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_repository.py` & `xingchen-1.1.3/test/test_repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_repository_info.py` & `xingchen-1.1.3/test/test_repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_boolean.py` & `xingchen-1.1.3/test/test_result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_character_dto.py` & `xingchen-1.1.3/test/test_result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_character_key.py` & `xingchen-1.1.3/test/test_result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_list_character_dto.py` & `xingchen-1.1.3/test/test_result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_page_result_character_dto.py` & `xingchen-1.1.3/test/test_result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.3/test/test_result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_scenario.py` & `xingchen-1.1.3/test/test_scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_sys_reminder_request.py` & `xingchen-1.1.3/test/test_sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/test/test_user_profile.py` & `xingchen-1.1.3/test/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/__init__.py` & `xingchen-1.1.3/xingchen/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     The version of the OpenAPI document: v2
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
-__version__ = "1.1.2"
+__version__ = "1.1.3"
 
 # import apis into sdk package
 from xingchen.api.character_api_sub import CharacterApiSub
 from xingchen.api.chat_api_sub import ChatApiSub
 from xingchen.api.chat_message_api_sub import ChatMessageApiSub
 from xingchen.api.groupchat_api_sub import GroupChatApiSub
 from xingchen.api.chat_extract_message_api_sub import ChatExtractMessageApiSub
@@ -104,18 +104,17 @@
 from xingchen.models.polling_image_detail_dto import PollingImageDetailDTO
 from xingchen.models.result_dto_character_desc_dto import ResultDTOCharacterDescDTO
 from xingchen.models.result_dto_file_conver_dto import ResultDTOFileConvertDTO
 from xingchen.models.result_dto_polling_image_detail_dto import ResultDTOPollingImageDetailDTO
 from xingchen.models.result_dto_extract_kv_dto import ResultDTOExtractKVDTO
 from xingchen.models.result_dto_extract_summary_dto import ResultDTOExtractSummaryDTO
 
-# OpenAI models
-from xingchen.models.custom.openai.openai_req_function import OpenAiReqFunction
-from xingchen.models.custom.openai.openai_resp_function import OpenAiRespFunction
-from xingchen.models.custom.openai.openai_usage import OpenAiUsage
-from xingchen.models.custom.openai.openai_req_message import OpenAiReqMessage
-from xingchen.models.custom.openai.openai_resp_message import OpenAiRespMessage
-from xingchen.models.custom.openai.openai_req_tool import OpenAiReqTool
-from xingchen.models.custom.openai.openai_resp_tool import OpenAiRespTool
-from xingchen.models.custom.openai.openai_completion_req import OpenAiCompletionReq
-from xingchen.models.custom.openai.openai_completion_resp import OpenAiCompletionResp
-from xingchen.api.openai_api_sub import OpenAiApiSub
+from xingchen.models.custom.completion.completion_req_function import AcAReqFunction
+from xingchen.models.custom.completion.completion_resp_function import AcARespFunction
+from xingchen.models.custom.completion.completion_usage import AcAUsage
+from xingchen.models.custom.completion.completion_req_message import AcAReqMessage
+from xingchen.models.custom.completion.completion_resp_message import AcARespMessage
+from xingchen.models.custom.completion.completion_req_tool import AcAReqTool
+from xingchen.models.custom.completion.completion_resp_tool import AcARespTool
+from xingchen.models.custom.completion.completion_req import AcACompletionReq
+from xingchen.models.custom.completion.completion_resp import AcACompletionResp
+from xingchen.api.completion_api_sub import AcACompletionApiSub
```

### Comparing `xingchen-1.1.2/xingchen/aca_util.py` & `xingchen-1.1.3/xingchen/aca_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from xingchen.models import ChatReqParams, BaseChatRequest, Input
 from xingchen.models.custom import ChatResponse, ChatResult
-from xingchen.models.custom.openai.openai_completion_resp import OpenAiCompletionResp
+from xingchen.models.custom.completion.completion_resp import AcACompletionResp
 
 from sseclient import SSEClient
 import json
 
 api_router_map = {
     '/v2/api/chat/send': 'aca-chat-send',
     '/v2/api/groupchat/send': 'aca-groupchat-send',
@@ -23,15 +23,15 @@
     '/v2/api/extract/kv': 'aca-extract-memory-kv',
     '/v2/api/extract/summary': 'aca-extract-memory-summary',
     '/v2/api/character/auto/desc': 'aca-char-auto-desc',
     '/v2/api/chat/polling/image': 'aca-polling-image',
     '/v2/api/chat/stop': 'aca-chat-stop',
     '/v2/api/common/file/asyn/upload': 'aca-doc-converter-submit',
     '/v2/api/common/file/asyn/download': 'aca-doc-converter-result',
-    '/v2/api/completions': 'aca-openai-completion',
+    '/v2/api/completions': 'aca-completion',
 }
 
 
 def get_service_router(path, async_req):
     if not path:
         return None
     if path.__eq__('/v2/api/chat/send') and async_req:
@@ -90,16 +90,16 @@
             success=True,
             http_status_code=200,
             code=200,
             data=ChatResult.from_dict(d)
         )
 
 
-def handle_openai_sse_response(client: SSEClient):
+def handle_completion_sse_response(client: SSEClient):
     events = client.events()
     for event in events:
         d = json.loads(event.data)
         error_code = d.get('errorCode', None)
         if error_code is not None:
             yield ChatResponse.from_dict(d)
             return
-        yield OpenAiCompletionResp.from_dict(d)
+        yield AcACompletionResp.from_dict(d)
```

### Comparing `xingchen-1.1.2/xingchen/api/character_api_sub.py` & `xingchen-1.1.3/xingchen/api/character_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/chat_api_sub.py` & `xingchen-1.1.3/xingchen/api/chat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/chat_extract_message_api_sub.py` & `xingchen-1.1.3/xingchen/api/chat_extract_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/chat_message_api_sub.py` & `xingchen-1.1.3/xingchen/api/chat_message_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/common_api_sub.py` & `xingchen-1.1.3/xingchen/api/common_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/groupchat_api_sub.py` & `xingchen-1.1.3/xingchen/api/groupchat_api_sub.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api/openai_api_sub.py` & `xingchen-1.1.3/xingchen/api/completion_api_sub.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 
 import requests
 from pydantic import Field
 from pydantic import validate_arguments
 from sseclient import SSEClient
 from typing_extensions import Annotated
 
-from xingchen import OpenAiCompletionReq, OpenAiCompletionResp
-from xingchen.aca_util import handle_openai_sse_response
+from xingchen import AcACompletionReq, AcACompletionResp, aca_util
+from xingchen.aca_util import handle_completion_sse_response
 from xingchen.api_client import ApiClient
 from xingchen.exceptions import (
     ApiTypeError
 )
 from xingchen.models.custom import ChatResponse
 
 
-class OpenAiApiSub:
+class AcACompletionApiSub:
     def __init__(self, api_client=None) -> None:
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     def version(self):
         return self.api_client.api_version()
 
     @validate_arguments
-    def completions(self, chat_req_params: Annotated[OpenAiCompletionReq, Field(..., description="对话请求")],
-                    **kwargs) -> Union[OpenAiCompletionResp, Generator[OpenAiCompletionResp, None, None]]:
+    def completions(self, chat_req_params: Annotated[AcACompletionReq, Field(..., description="对话请求")],
+                    **kwargs) -> Union[AcACompletionResp, Generator[AcACompletionResp, None, None]]:
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             message = "Error! Please call the chat_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
             raise ValueError(message)
         return self.chat_with_http_info(chat_req_params, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def chat_with_http_info(self, chat_req_params: Annotated[OpenAiCompletionReq, Field(..., description="对话请求")],
-                            **kwargs) -> Union[OpenAiCompletionResp, Generator[OpenAiCompletionResp, None, None]]:  # noqa: E501
+    def chat_with_http_info(self, chat_req_params: Annotated[AcACompletionReq, Field(..., description="对话请求")],
+                            **kwargs) -> Union[AcACompletionResp, Generator[AcACompletionResp, None, None]]:  # noqa: E501
 
         _params = locals()
 
         _all_params = [
             'chat_req_params'
         ]
         _all_params.extend(
@@ -106,30 +106,31 @@
 
         is_stream = 'enable' == _header_params.get('X-DashScope-SSE') or 'enable' == _header_params.get('X-AcA-SSE') \
                     or chat_req_params.stream
         path = '/{0}/api/completions'.format(version)
         host = self.api_client.configuration.host
 
         _header_params['x-fag-appcode'] = 'aca'
-        _header_params['x-fag-servicename'] = 'aca-openai-completion'
         _header_params['Authorization'] = 'Bearer ' + self.api_client.configuration.access_token
 
         if is_stream:
-            _header_params['x-fag-servicename'] = 'aca-openai-completion'
+            service_name = aca_util.get_service_router(path, True)
             _header_params['Accept'] = 'text/event-stream;charset=UTF-8'
+            _header_params['x-fag-servicename'] = service_name
+
             body_params = self.api_client.sanitize_for_serialization(_body_params)
 
             request = requests.post(
                 host + path,
                 headers=_header_params,
                 json=body_params,
                 stream=True
             )
             client = SSEClient(request)
-            return (res for res in handle_openai_sse_response(client))
+            return (res for res in handle_completion_sse_response(client))
 
         response = self.api_client.call_api(
             '/{0}/api/completions'.format(version), 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
@@ -144,8 +145,8 @@
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
         d = response
         error_code = d.get('errorCode', None)
         if error_code is not None:
             return ChatResponse.from_dict(d)
-        return OpenAiCompletionResp.from_dict(d)
+        return AcACompletionResp.from_dict(d)
```

### Comparing `xingchen-1.1.2/xingchen/api_client.py` & `xingchen-1.1.3/xingchen/api_client.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/api_response.py` & `xingchen-1.1.3/xingchen/api_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/configuration.py` & `xingchen-1.1.3/xingchen/configuration.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/exceptions.py` & `xingchen-1.1.3/xingchen/exceptions.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/__init__.py` & `xingchen-1.1.3/xingchen/models/__init__.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/advanced_settings.py` & `xingchen-1.1.3/xingchen/models/advanced_settings.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/base_chat_request.py` & `xingchen-1.1.3/xingchen/models/base_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_advanced_config.py` & `xingchen-1.1.3/xingchen/models/character_advanced_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_create_dto.py` & `xingchen-1.1.3/xingchen/models/character_create_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_desc_dto.py` & `xingchen-1.1.3/xingchen/models/character_desc_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_desc_generated_request.py` & `xingchen-1.1.3/xingchen/models/character_desc_generated_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_dto.py` & `xingchen-1.1.3/xingchen/models/character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_key.py` & `xingchen-1.1.3/xingchen/models/character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_permission_config.py` & `xingchen-1.1.3/xingchen/models/character_permission_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_query_dto.py` & `xingchen-1.1.3/xingchen/models/character_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_query_where.py` & `xingchen-1.1.3/xingchen/models/character_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_update_dto.py` & `xingchen-1.1.3/xingchen/models/character_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/character_version_create_or_update_dto.py` & `xingchen-1.1.3/xingchen/models/character_version_create_or_update_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_context.py` & `xingchen-1.1.3/xingchen/models/chat_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_history_query_dto.py` & `xingchen-1.1.3/xingchen/models/chat_history_query_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_history_query_where.py` & `xingchen-1.1.3/xingchen/models/chat_history_query_where.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_message_dto.py` & `xingchen-1.1.3/xingchen/models/chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_req_params.py` & `xingchen-1.1.3/xingchen/models/chat_req_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/chat_room_user_dto.py` & `xingchen-1.1.3/xingchen/models/chat_room_user_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/context.py` & `xingchen-1.1.3/xingchen/models/context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/base_response.py` & `xingchen-1.1.3/xingchen/models/custom/base_response.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/character_model_parameters.py` & `xingchen-1.1.3/xingchen/models/custom/character_model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/chat_response.py` & `xingchen-1.1.3/xingchen/models/custom/chat_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             'choices': obj.get('choices'),
             'usage': obj.get('usage'),
             'context': obj.get('context')
         })
 
 
 class ChatResponse(BaseResponse):
-    data: Optional[Any] = Field(None, alias="chatResult")
+    data: Optional[ChatResult] = Field(None, alias="chatResult")
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         return pprint.pformat(self.dict(by_alias=False, exclude_none=True))
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_ext_param.py` & `xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_ext_param.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_reply_setting.py` & `xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_reply_setting.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/groupchat/group_chat_room_info.py` & `xingchen-1.1.3/xingchen/models/custom/groupchat/group_chat_room_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_choice.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_choice.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, Field, StrictStr, StrictInt
 
-from xingchen.models.custom.openai.openai_resp_message import OpenAiRespMessage
+from xingchen.models.custom.completion.completion_resp_message import AcARespMessage
 
 
-class OpenAiChoice(BaseModel):
+class AcAChoice(BaseModel):
     index: Optional[StrictInt] = Field(None, alias="index")
     finish_reason: Optional[StrictStr] = Field(None, alias="finish_reason")
-    message: Optional[OpenAiRespMessage] = Field(None, alias="message")
+    message: Optional[AcARespMessage] = Field(None, alias="message")
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         return pprint.pformat(self.dict(by_alias=True))
@@ -25,23 +25,23 @@
     def to_json(self) -> str:
         return json.dumps(self.to_dict())
 
     def to_dict(self):
         return self.dict(by_alias=True, exclude={}, exclude_none=True)
 
     @classmethod
-    def from_json(cls, json_str: str) -> OpenAiChoice:
+    def from_json(cls, json_str: str) -> AcAChoice:
         return cls.from_dict(json.loads(json_str))
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OpenAiChoice:
+    def from_dict(cls, obj: dict) -> AcAChoice:
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return OpenAiChoice.parse_obj(obj)
+            return AcAChoice.parse_obj(obj)
 
-        return OpenAiChoice.parse_obj({
+        return AcAChoice.parse_obj({
             'index': obj.get('index'),
             'finish_reason': obj.get('finish_reason'),
-            'message': OpenAiRespMessage.from_dict(obj.get('message')) if obj.get('message') is not None else None
+            'message': AcARespMessage.from_dict(obj.get('message')) if obj.get('message') is not None else None
         })
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_req.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_req.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import pprint
 from typing import Dict, Optional, Any
 
 from pydantic import BaseModel, Field, conlist, StrictStr, StrictFloat, StrictInt, StrictBool
 
-from xingchen import OpenAiReqMessage, OpenAiReqTool
+from xingchen import AcAReqMessage, AcAReqTool
 
 
-class OpenAiCompletionReq(BaseModel):
+class AcACompletionReq(BaseModel):
     """
     completions 接口请求参数
     """
-    messages: conlist(OpenAiReqMessage) = Field(..., description="""
+    messages: conlist(AcAReqMessage) = Field(..., description="""
     A list of messages comprising the conversation so far.
     Contain system message, user message, assistant message and tool message.
     """)
     model: StrictStr = Field(..., description="""
     xingchen model name, such as xingchen-plus
     """)
     max_tokens: Optional[StrictInt] = Field(None, alias="max_tokens", description="""
@@ -34,15 +34,15 @@
     We generally recommend altering this or top_p but not both.
     """)
     top_p: Optional[StrictFloat] = Field(None, description="""
     An alternative to sampling with temperature, called nucleus sampling, 
     where the model considers the results of the tokens with top_p probability mass. 
     So 0.1 means only the tokens comprising the top 10% probability mass are considered.
     """)
-    tools: Optional[conlist(OpenAiReqTool)] = Field(None, description="""
+    tools: Optional[conlist(AcAReqTool)] = Field(None, description="""
     A list of tools the model may call. Currently, only functions are supported as a tool. 
     Use this to provide a list of functions the model may generate JSON inputs for. A max of 128 functions are supported.
     """)
     tool_choice: Optional[Any] = Field(None, alias="tool_choice", description="""
     Controls which (if any) tool is called by the model. 
     none means the model will not call any tool and instead generates a message. 
     auto means the model can pick between generating a message or calling one or more tools. 
@@ -61,28 +61,28 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiCompletionReq':
+    def from_json(cls, json_str: str) -> 'AcACompletionReq':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiCompletionReq':
+    def from_dict(cls, obj: dict) -> 'AcACompletionReq':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_completion_resp.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_req_message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,25 @@
+from __future__ import annotations
+
 import json
 import pprint
+from typing import Optional
 
-from pydantic import BaseModel, Field, conlist
-
-from xingchen.models.custom.openai.openai_choice import OpenAiChoice
-from xingchen.models.custom.openai.openai_usage import OpenAiUsage
+from pydantic import BaseModel, Field, StrictStr
 
 
-class OpenAiCompletionResp(BaseModel):
+class AcAReqMessage(BaseModel):
     """
-    Completion response
+    Message
     """
-    id: str = Field(None, description="A unique identifier for the chat completion.")
-    created: int = Field(None, description="The Unix timestamp (in seconds) of when the chat completion was created.")
-    model: str = Field(None, description="The model used for the chat completion.")
-    choices: conlist(OpenAiChoice) = Field(None, description="A list of chat completion choices. Can be more than one if n is greater than 1.")
-    usage: OpenAiUsage = Field(None, description="Usage statistics for the completion request.")
+    name: Optional[StrictStr] = Field(None, description="角色名称")
+    role: StrictStr = Field(...,
+                            description="角色类型, user-用户发送的内容；system-系统指令；assistant-助手消息；tool-工具类消息")
+    content: Optional[StrictStr] = Field(None, description="消息内容")
+    tool_call_id: Optional[StrictStr] = Field(None, description="模型生成的工具调用id")
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -27,35 +27,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiCompletionResp':
+    def from_json(cls, json_str: str) -> AcAReqMessage:
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiCompletionResp':
+    def from_dict(cls, obj: dict) -> AcAReqMessage:
+        """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
-            "id": obj.get("id"),
-            "created": obj.get("created"),
-            "model": obj.get("model"),
-            "choices": [OpenAiChoice.from_dict(c) for c in obj.get("choices", []) if c is not None],
-            "usage": obj.get("usage"),
+            "name": obj.get("name"),
+            "role": obj.get("role"),
+            "content": obj.get("content"),
+            "tool_call_id": obj.get("tool_call_id")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_req_function.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_req_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import pprint
 from typing import Dict
 
 from pydantic import BaseModel, Field
 
 
-class OpenAiReqFunction(BaseModel):
+class AcAReqFunction(BaseModel):
     """
     completions 接口请求参数
     """
     name: str = Field(..., title="function名", description="function名")
     description: str = Field(..., title="function描述", description="function描述")
     parameters: Dict = Field(..., title="function参数定义", description="function参数定义，json schema格式")
 
@@ -23,28 +23,28 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiReqFunction':
+    def from_json(cls, json_str: str) -> 'AcAReqFunction':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiReqFunction':
+    def from_dict(cls, obj: dict) -> 'AcAReqFunction':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_req_message.py` & `xingchen-1.1.3/xingchen/models/custom/platform_publish_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,64 @@
+# coding: utf-8
+
+
 from __future__ import annotations
 
 import json
 import pprint
-from typing import Optional
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, Field, StrictStr, StrictBool
+from typing import Optional
 
 
-class OpenAiReqMessage(BaseModel):
+class PlatformPublishConfig(BaseModel):
     """
-    Message
+    平台发布配置
     """
-    name: Optional[StrictStr] = Field(None, description="角色名称")
-    role: StrictStr = Field(...,
-                            description="角色类型, user-用户发送的内容；system-系统指令；assistant-助手消息；tool-工具类消息")
-    content: Optional[StrictStr] = Field(None, description="消息内容")
-    tool_call_id: Optional[StrictStr] = Field(None, description="模型生成的工具调用id")
+    enabled: Optional[StrictBool] = Field(..., alias="enabled", description="是否开启")
+    private_share_type: StrictStr = Field(..., alias="privateShareType", description="""
+     私密分享类型
+     * selfShare - 仅自己可与角色聊天 （permConfig.allowChat=0）
+     * linkShare - 通过链接分享（允许获得链接的星尘用户可与ta聊天）  （permConfig.allowChat=0）
+     * allShare  - 所有星尘用户可见（需要平台审核）  （permConfig.allowChat=1）
+    """)
+    __properties = ["enabled", "privateShareType"]
 
     class Config:
-        """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
-        """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
-        """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OpenAiReqMessage:
-        """Create an instance of Message from a JSON string"""
+    def from_json(cls, json_str: str) -> PlatformPublishConfig:
+        """Create an instance of SysReminderRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OpenAiReqMessage:
-        """Create an instance of Message from a dict"""
+    def from_dict(cls, obj: dict) -> PlatformPublishConfig:
+        """Create an instance of SysReminderRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return cls.parse_obj(obj)
+            return PlatformPublishConfig.parse_obj(obj)
 
-        _obj = cls.parse_obj({
-            "name": obj.get("name"),
-            "role": obj.get("role"),
-            "content": obj.get("content"),
-            "tool_call_id": obj.get("tool_call_id")
+        _obj = PlatformPublishConfig.parse_obj({
+            "enabled": obj.get("enabled"),
+            "private_share_type": obj.get("privateShareType")
         })
         return _obj
+
+
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_req_tool.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_req_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, StrictStr, Field
 
-from xingchen import OpenAiReqFunction
+from xingchen import AcAReqFunction
 
 
-class OpenAiReqTool(BaseModel):
-    """
-    OpenAiTool
-    """
+class AcAReqTool(BaseModel):
     id: Optional[StrictStr] = Field(None, description="工具ID")
     type: Optional[StrictStr] = Field(None, description="工具类型, 目前只支持 function")
-    function: Optional[OpenAiReqFunction] = Field(..., description="工具函数")
+    function: Optional[AcAReqFunction] = Field(..., description="工具函数")
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -25,28 +22,28 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiReqTool':
+    def from_json(cls, json_str: str) -> 'AcAReqTool':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiReqTool':
+    def from_dict(cls, obj: dict) -> 'AcAReqTool':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_function.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_function.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import pprint
 
 from pydantic import BaseModel, Field
 
 
-class OpenAiRespFunction(BaseModel):
+class AcARespFunction(BaseModel):
     """
     completions 接口响应函数
     """
     name: str = Field(None, title="function名称", description="function名称")
     arguments: str = Field(None, title="模型输出function参数值", description="模型输出function参数值，json str格式")
 
     class Config:
@@ -21,28 +21,28 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiRespFunction':
+    def from_json(cls, json_str: str) -> 'AcARespFunction':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiRespFunction':
+    def from_dict(cls, obj: dict) -> 'AcARespFunction':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_message.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from __future__ import annotations
 
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, Field, StrictStr, conlist
-from xingchen.models.custom.openai.openai_resp_tool import OpenAiRespTool
+from xingchen.models.custom.completion.completion_resp_tool import AcARespTool
 
 
-class OpenAiRespMessage(BaseModel):
+class AcARespMessage(BaseModel):
     """
     Message
     """
     name: Optional[StrictStr] = Field(None, description="角色名称")
     role: StrictStr = Field(None, description="assistant-助手消息")
     content: Optional[StrictStr] = Field(None, description="消息内容")
-    tool_calls: Optional[conlist(OpenAiRespTool)] = Field(None, description="工具调用结果")
+    tool_calls: Optional[conlist(AcARespTool)] = Field(None, description="工具调用结果")
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -27,34 +27,34 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OpenAiRespMessage:
+    def from_json(cls, json_str: str) -> AcARespMessage:
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OpenAiRespMessage:
+    def from_dict(cls, obj: dict) -> AcARespMessage:
         """Create an instance of Message from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
             "name": obj.get("name"),
             "role": obj.get("role"),
             "content": obj.get("content"),
-            "tool_calls": [OpenAiRespTool.from_dict(v) for v in obj.get("tool_calls", [])]
+            "tool_calls": [AcARespTool.from_dict(v) for v in obj.get("tool_calls", [])]
         })
         return _obj
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_resp_tool.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_resp_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, StrictStr, Field
 
-from xingchen.models.custom.openai.openai_resp_function import OpenAiRespFunction
+from xingchen.models.custom.completion.completion_resp_function import AcARespFunction
 
 
-class OpenAiRespTool(BaseModel):
-    """
-    OpenAiTool
-    """
+class AcARespTool(BaseModel):
     id: Optional[StrictStr] = Field(None, description="工具ID")
     type: Optional[StrictStr] = Field(None, description="工具类型, 目前只支持 function")
-    function: Optional[OpenAiRespFunction] = Field(..., description="工具函数")
+    function: Optional[AcARespFunction] = Field(..., description="工具函数")
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -25,33 +22,33 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiRespTool':
+    def from_json(cls, json_str: str) -> 'AcARespTool':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiRespTool':
+    def from_dict(cls, obj: dict) -> 'AcARespTool':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
             "id": obj.get("id"),
             "type": obj.get("type"),
-            "function": OpenAiRespFunction.from_dict(obj.get("function")) if obj.get("function") is not None else None
+            "function": AcARespFunction.from_dict(obj.get("function")) if obj.get("function") is not None else None
         })
         return _obj
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_tool_choice.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_tool_choice.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, StrictStr, Field
 
-from xingchen import OpenAiReqFunction
+from xingchen import AcAReqFunction
 
 
-class OpenAiToolChoice(BaseModel):
-    """
-    OpenAiToolChoice
-    """
+class AcAToolChoice(BaseModel):
     type: Optional[StrictStr] = Field(None, description="工具类型, 目前只支持 function")
-    function: Optional[OpenAiReqFunction] = Field(..., description="工具函数描述")
+    function: Optional[AcAReqFunction] = Field(..., description="工具函数描述")
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -24,28 +21,28 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiToolChoice':
+    def from_json(cls, json_str: str) -> 'AcAToolChoice':
         """Create an instance of Message from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiToolChoice':
+    def from_dict(cls, obj: dict) -> 'AcAToolChoice':
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.parse_obj(obj)
 
         _obj = cls.parse_obj({
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/openai/openai_usage.py` & `xingchen-1.1.3/xingchen/models/custom/completion/completion_usage.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import pprint
 from typing import Optional
 
 from pydantic import BaseModel, Field, StrictInt
 
 
-class OpenAiUsage(BaseModel):
+class AcAUsage(BaseModel):
     """
     用量统计
     """
     prompt_tokens: Optional[StrictInt] = Field(None, description="Prompt token 数")
     completion_tokens: Optional[StrictInt] = Field(None, description="模型生成 token 数")
     total_tokens: Optional[StrictInt] = Field(None, description="token总数")
 
@@ -26,21 +26,21 @@
         return json.dumps(self.dict(by_alias=True))
 
     def to_dict(self) -> dict:
         """Returns the dictionary representation of the model using alias"""
         return self.dict(by_alias=True, exclude={}, exclude_none=True)
 
     @classmethod
-    def from_json(cls, json_str: str) -> 'OpenAiUsage':
+    def from_json(cls, json_str: str) -> 'AcAUsage':
         return cls.from_dict(json.loads(json_str))
 
     @classmethod
-    def from_dict(cls, obj: dict) -> 'OpenAiUsage':
+    def from_dict(cls, obj: dict) -> 'AcAUsage':
         if obj is None:
             return None
         if not isinstance(obj, dict):
-            return OpenAiUsage.parse_obj(obj)
-        return OpenAiUsage.parse_obj({
+            return AcAUsage.parse_obj(obj)
+        return AcAUsage.parse_obj({
             'prompt_tokens': obj.get('prompt_tokens'),
             'completion_tokens': obj.get('completion_tokens'),
             'total_tokens': obj.get('total_tokens')
         })
```

### Comparing `xingchen-1.1.2/xingchen/models/custom/reset_history_request.py` & `xingchen-1.1.3/xingchen/models/custom/reset_history_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/extract_data.py` & `xingchen-1.1.3/xingchen/models/extract_data.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/extract_kv_dto.py` & `xingchen-1.1.3/xingchen/models/extract_kv_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/extract_memory_request.py` & `xingchen-1.1.3/xingchen/models/extract_memory_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/extract_summary_dto.py` & `xingchen-1.1.3/xingchen/models/extract_summary_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/file_conver_dto.py` & `xingchen-1.1.3/xingchen/models/file_conver_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/file_conver_request.py` & `xingchen-1.1.3/xingchen/models/file_conver_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/file_info_vo.py` & `xingchen-1.1.3/xingchen/models/file_info_vo.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/function_call.py` & `xingchen-1.1.3/xingchen/models/function_call.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/gateway_context.py` & `xingchen-1.1.3/xingchen/models/gateway_context.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/gateway_issued_params.py` & `xingchen-1.1.3/xingchen/models/gateway_issued_params.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/input.py` & `xingchen-1.1.3/xingchen/models/input.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/keyword.py` & `xingchen-1.1.3/xingchen/models/keyword.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/kv_memory_config.py` & `xingchen-1.1.3/xingchen/models/kv_memory_config.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/long_term_memory.py` & `xingchen-1.1.3/xingchen/models/long_term_memory.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/memory.py` & `xingchen-1.1.3/xingchen/models/memory.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/memory_summary.py` & `xingchen-1.1.3/xingchen/models/memory_summary.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/message.py` & `xingchen-1.1.3/xingchen/models/message.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/message_rating_request.py` & `xingchen-1.1.3/xingchen/models/message_rating_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/meta.py` & `xingchen-1.1.3/xingchen/models/meta.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/model_parameters.py` & `xingchen-1.1.3/xingchen/models/model_parameters.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/page_result_character_dto.py` & `xingchen-1.1.3/xingchen/models/page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/page_result_chat_message_dto.py` & `xingchen-1.1.3/xingchen/models/page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/platform_plugin.py` & `xingchen-1.1.3/xingchen/models/platform_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/polling_image_detail_dto.py` & `xingchen-1.1.3/xingchen/models/polling_image_detail_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/reject_answer_plugin.py` & `xingchen-1.1.3/xingchen/models/reject_answer_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/reject_condition.py` & `xingchen-1.1.3/xingchen/models/reject_condition.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/repository.py` & `xingchen-1.1.3/xingchen/models/repository.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/repository_info.py` & `xingchen-1.1.3/xingchen/models/repository_info.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_boolean.py` & `xingchen-1.1.3/xingchen/models/result_dto_boolean.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_character_desc_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_character_desc_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_character_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_character_key.py` & `xingchen-1.1.3/xingchen/models/result_dto_character_key.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_extract_kv_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_extract_kv_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_extract_summary_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_extract_summary_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_file_conver_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_file_conver_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_list_character_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_list_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_page_result_character_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_page_result_character_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_page_result_chat_message_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_page_result_chat_message_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/result_dto_polling_image_detail_dto.py` & `xingchen-1.1.3/xingchen/models/result_dto_polling_image_detail_dto.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/scenario.py` & `xingchen-1.1.3/xingchen/models/scenario.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/stop_chat_request.py` & `xingchen-1.1.3/xingchen/models/stop_chat_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/sys_reminder_request.py` & `xingchen-1.1.3/xingchen/models/sys_reminder_request.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/text_to_image_plugin.py` & `xingchen-1.1.3/xingchen/models/text_to_image_plugin.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/models/user_profile.py` & `xingchen-1.1.3/xingchen/models/user_profile.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen/rest.py` & `xingchen-1.1.3/xingchen/rest.py`

 * *Files identical despite different names*

### Comparing `xingchen-1.1.2/xingchen.egg-info/SOURCES.txt` & `xingchen-1.1.3/xingchen.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 xingchen.egg-info/top_level.txt
 xingchen/api/__init__.py
 xingchen/api/character_api_sub.py
 xingchen/api/chat_api_sub.py
 xingchen/api/chat_extract_message_api_sub.py
 xingchen/api/chat_message_api_sub.py
 xingchen/api/common_api_sub.py
+xingchen/api/completion_api_sub.py
 xingchen/api/groupchat_api_sub.py
-xingchen/api/openai_api_sub.py
 xingchen/models/__init__.py
 xingchen/models/advanced_settings.py
 xingchen/models/base_chat_request.py
 xingchen/models/character_advanced_config.py
 xingchen/models/character_create_dto.py
 xingchen/models/character_desc_dto.py
 xingchen/models/character_desc_generated_request.py
@@ -132,23 +132,23 @@
 xingchen/models/user_profile.py
 xingchen/models/custom/__init__.py
 xingchen/models/custom/base_response.py
 xingchen/models/custom/character_model_parameters.py
 xingchen/models/custom/chat_response.py
 xingchen/models/custom/platform_publish_config.py
 xingchen/models/custom/reset_history_request.py
+xingchen/models/custom/completion/__init__.py
+xingchen/models/custom/completion/completion_choice.py
+xingchen/models/custom/completion/completion_req.py
+xingchen/models/custom/completion/completion_req_function.py
+xingchen/models/custom/completion/completion_req_message.py
+xingchen/models/custom/completion/completion_req_tool.py
+xingchen/models/custom/completion/completion_resp.py
+xingchen/models/custom/completion/completion_resp_function.py
+xingchen/models/custom/completion/completion_resp_message.py
+xingchen/models/custom/completion/completion_resp_tool.py
+xingchen/models/custom/completion/completion_tool_choice.py
+xingchen/models/custom/completion/completion_usage.py
 xingchen/models/custom/groupchat/__init__.py
 xingchen/models/custom/groupchat/group_chat_ext_param.py
 xingchen/models/custom/groupchat/group_chat_reply_setting.py
-xingchen/models/custom/groupchat/group_chat_room_info.py
-xingchen/models/custom/openai/__init__.py
-xingchen/models/custom/openai/openai_choice.py
-xingchen/models/custom/openai/openai_completion_req.py
-xingchen/models/custom/openai/openai_completion_resp.py
-xingchen/models/custom/openai/openai_req_function.py
-xingchen/models/custom/openai/openai_req_message.py
-xingchen/models/custom/openai/openai_req_tool.py
-xingchen/models/custom/openai/openai_resp_function.py
-xingchen/models/custom/openai/openai_resp_message.py
-xingchen/models/custom/openai/openai_resp_tool.py
-xingchen/models/custom/openai/openai_tool_choice.py
-xingchen/models/custom/openai/openai_usage.py
+xingchen/models/custom/groupchat/group_chat_room_info.py
```

