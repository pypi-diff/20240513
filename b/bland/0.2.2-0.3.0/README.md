# Comparing `tmp/bland-0.2.2.tar.gz` & `tmp/bland-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bland-0.2.2.tar", max compression
+gzip compressed data, was "bland-0.3.0.tar", max compression
```

## Comparing `bland-0.2.2.tar` & `bland-0.3.0.tar`

### file list

```diff
@@ -1,139 +1,146 @@
--rw-r--r--   0        0        0     4713 2024-03-08 21:05:36.455396 bland-0.2.2/README.md
--rw-r--r--   0        0        0      421 2024-03-08 21:05:36.455396 bland-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5082 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/__init__.py
--rw-r--r--   0        0        0      909 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/__init__.py
--rw-r--r--   0        0        0    31903 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/client.py
--rw-r--r--   0        0        0     1355 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/__init__.py
--rw-r--r--   0        0        0     3098 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/analysis_object.py
--rw-r--r--   0        0        0     1886 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/analyze_batch_request.py
--rw-r--r--   0        0        0     1125 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/batch_analysis_object.py
--rw-r--r--   0        0        0     1402 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/batch_call_data.py
--rw-r--r--   0        0        0     1364 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/batch_details_response.py
--rw-r--r--   0        0        0     1649 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/batch_object.py
--rw-r--r--   0        0        0     1618 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/batch_params.py
--rw-r--r--   0        0        0     1754 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/call_data.py
--rw-r--r--   0        0        0     1432 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/call_length.py
--rw-r--r--   0        0        0     1380 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/call_length_summary.py
--rw-r--r--   0        0        0      994 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/call_params.py
--rw-r--r--   0        0        0     1090 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/list_batches_response.py
--rw-r--r--   0        0        0     1236 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/queue_status.py
--rw-r--r--   0        0        0     1356 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/retrieve_batch_analysis_response.py
--rw-r--r--   0        0        0     3238 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/send_batch_request.py
--rw-r--r--   0        0        0     1108 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/send_batch_response.py
--rw-r--r--   0        0        0      128 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/status_enum.py
--rw-r--r--   0        0        0     1349 2024-03-08 21:05:36.455396 bland-0.2.2/src/blandai/batches/types/stop_active_batch_response.py
--rw-r--r--   0        0        0      601 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/__init__.py
--rw-r--r--   0        0        0    27070 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/client.py
--rw-r--r--   0        0        0      869 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/__init__.py
--rw-r--r--   0        0        0     1459 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/analyze_call.py
--rw-r--r--   0        0        0     1694 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/analyze_call_response.py
--rw-r--r--   0        0        0      158 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/answered_by_enum.py
--rw-r--r--   0        0        0     1564 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/audio_recording_response.py
--rw-r--r--   0        0        0     4840 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/call_details_response.py
--rw-r--r--   0        0        0       83 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/call_id_param.py
--rw-r--r--   0        0        0       76 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/goal.py
--rw-r--r--   0        0        0     1052 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/list_calls_response.py
--rw-r--r--   0        0        0     1218 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/listed_call_data.py
--rw-r--r--   0        0        0     1257 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/stop_call_response.py
--rw-r--r--   0        0        0     1048 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/transcript.py
--rw-r--r--   0        0        0      152 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/calls/types/user_enum.py
--rw-r--r--   0        0        0    13122 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/client.py
--rw-r--r--   0        0        0      467 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/__init__.py
--rw-r--r--   0        0        0      267 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/errors/__init__.py
--rw-r--r--   0        0        0      274 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/errors/bad_request_error.py
--rw-r--r--   0        0        0      270 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/errors/server_error.py
--rw-r--r--   0        0        0      276 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0      470 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/__init__.py
--rw-r--r--   0        0        0      157 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/call_id.py
--rw-r--r--   0        0        0     1565 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/custom_tool.py
--rw-r--r--   0        0        0      886 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/error_body.py
--rw-r--r--   0        0        0      916 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/error_detail.py
--rw-r--r--   0        0        0      106 2024-03-08 21:05:36.459396 bland-0.2.2/src/blandai/commons/types/phone_number.py
--rw-r--r--   0        0        0      124 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/commons/types/status.py
--rw-r--r--   0        0        0      166 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/commons/types/tools.py
--rw-r--r--   0        0        0       79 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/commons/types/voice_id.py
--rw-r--r--   0        0        0       79 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/commons/types/webhook.py
--rw-r--r--   0        0        0      790 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/api_error.py
--rw-r--r--   0        0        0     1187 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/file.py
--rw-r--r--   0        0        0     4882 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/core/request_options.py
--rw-r--r--   0        0        0      193 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/environment.py
--rw-r--r--   0        0        0      571 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/__init__.py
--rw-r--r--   0        0        0    20051 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/client.py
--rw-r--r--   0        0        0      817 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/__init__.py
--rw-r--r--   0        0        0      127 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/country_code.py
--rw-r--r--   0        0        0     1463 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number.py
--rw-r--r--   0        0        0     1653 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_details_response.py
--rw-r--r--   0        0        0     1812 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_request.py
--rw-r--r--   0        0        0      949 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_response.py
--rw-r--r--   0        0        0     1071 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/list_inbound_response.py
--rw-r--r--   0        0        0      132 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/model.py
--rw-r--r--   0        0        0     6631 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/update_inbound.py
--rw-r--r--   0        0        0     1541 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/update_inbound_response.py
--rw-r--r--   0        0        0     2269 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/inbound_numbers/types/voice_settings.py
--rw-r--r--   0        0        0      267 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/__init__.py
--rw-r--r--   0        0        0    10344 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/client.py
--rw-r--r--   0        0        0      381 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/types/__init__.py
--rw-r--r--   0        0        0     1040 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/types/list_outbound_response.py
--rw-r--r--   0        0        0     1002 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/types/outbound_number.py
--rw-r--r--   0        0        0     1160 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/types/outbound_purchase.py
--rw-r--r--   0        0        0      952 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/outbound_numbers/types/outbound_purchase_response.py
--rw-r--r--   0        0        0        0 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/py.typed
--rw-r--r--   0        0        0      923 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/__init__.py
--rw-r--r--   0        0        0    31698 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/client.py
--rw-r--r--   0        0        0     1376 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/__init__.py
--rw-r--r--   0        0        0      144 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/a_2_p_status_enum.py
--rw-r--r--   0        0        0      972 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/check_status_request.py
--rw-r--r--   0        0        0     1254 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/check_status_response.py
--rw-r--r--   0        0        0     1435 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/get_messages_request.py
--rw-r--r--   0        0        0      987 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/get_messages_response.py
--rw-r--r--   0        0        0      227 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/legal_structure_enum.py
--rw-r--r--   0        0        0     2637 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/register_request.py
--rw-r--r--   0        0        0      916 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/register_response.py
--rw-r--r--   0        0        0      162 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/toggle_reply_enum.py
--rw-r--r--   0        0        0     1234 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/toggle_reply_request.py
--rw-r--r--   0        0        0     1027 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/toggle_reply_response.py
--rw-r--r--   0        0        0     1131 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/trusted_user.py
--rw-r--r--   0        0        0     1172 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/update_prompt_request.py
--rw-r--r--   0        0        0      880 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/update_prompt_response.py
--rw-r--r--   0        0        0     1224 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/update_webhook_request.py
--rw-r--r--   0        0        0      881 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/update_webhook_response.py
--rw-r--r--   0        0        0      729 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/sms/types/vertical_enum.py
--rw-r--r--   0        0        0      851 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/__init__.py
--rw-r--r--   0        0        0     2707 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/dynamic_data.py
--rw-r--r--   0        0        0      125 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/interruption_threshold.py
--rw-r--r--   0        0        0      123 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/method_enum.py
--rw-r--r--   0        0        0      144 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/model_enum.py
--rw-r--r--   0        0        0     1606 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/pronunciation_object.py
--rw-r--r--   0        0        0      188 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/prounciation_guide.py
--rw-r--r--   0        0        0     1379 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/response_data.py
--rw-r--r--   0        0        0    10171 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/send_call.py
--rw-r--r--   0        0        0     1782 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/send_call_response.py
--rw-r--r--   0        0        0      117 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/temperature.py
--rw-r--r--   0        0        0      117 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/transfer_list.py
--rw-r--r--   0        0        0      140 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/types/voicemail_action.py
--rw-r--r--   0        0        0      963 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/__init__.py
--rw-r--r--   0        0        0    41204 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/client.py
--rw-r--r--   0        0        0     1437 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/__init__.py
--rw-r--r--   0        0        0     1963 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/create_voice_preset_request.py
--rw-r--r--   0        0        0     1144 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/create_voice_preset_response.py
--rw-r--r--   0        0        0     1098 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/delete_voice_preset_response.py
--rw-r--r--   0        0        0     1263 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/generate_voice_sample_request.py
--rw-r--r--   0        0        0     1034 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/generate_voice_sample_response.py
--rw-r--r--   0        0        0     1206 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/list_voice_options_response.py
--rw-r--r--   0        0        0      157 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/optimize_for.py
--rw-r--r--   0        0        0     1082 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/preset.py
--rw-r--r--   0        0        0     1180 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/publish_voice_preset_response.py
--rw-r--r--   0        0        0     1044 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/retrieve_voice_preset_response.py
--rw-r--r--   0        0        0     1985 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/retrieved_voice.py
--rw-r--r--   0        0        0     2088 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/update_voice_preset_request.py
--rw-r--r--   0        0        0     1339 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/update_voice_preset_response.py
--rw-r--r--   0        0        0      926 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/voice.py
--rw-r--r--   0        0        0     1719 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/voice_settings_data.py
--rw-r--r--   0        0        0     1227 2024-03-08 21:05:36.463396 bland-0.2.2/src/blandai/voices/types/voice_updates.py
--rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 bland-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4713 2024-05-13 06:45:42.267316 bland-0.3.0/README.md
+-rw-r--r--   0        0        0      587 2024-05-13 06:45:42.267316 bland-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5293 2024-05-13 06:45:42.267316 bland-0.3.0/src/bland/__init__.py
+-rw-r--r--   0        0        0      909 2024-05-13 06:45:42.267316 bland-0.3.0/src/bland/batches/__init__.py
+-rw-r--r--   0        0        0    65809 2024-05-13 06:45:42.267316 bland-0.3.0/src/bland/batches/client.py
+-rw-r--r--   0        0        0     1355 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/__init__.py
+-rw-r--r--   0        0        0     3128 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/analysis_object.py
+-rw-r--r--   0        0        0     1897 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/analyze_batch_request.py
+-rw-r--r--   0        0        0     1112 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/batch_analysis_object.py
+-rw-r--r--   0        0        0     1395 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/batch_call_data.py
+-rw-r--r--   0        0        0     1354 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/batch_details_response.py
+-rw-r--r--   0        0        0     1648 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/batch_object.py
+-rw-r--r--   0        0        0     1617 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/batch_params.py
+-rw-r--r--   0        0        0     1788 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/call_data.py
+-rw-r--r--   0        0        0     1515 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/call_length.py
+-rw-r--r--   0        0        0     1423 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/call_length_summary.py
+-rw-r--r--   0        0        0      975 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/call_params.py
+-rw-r--r--   0        0        0     1077 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/list_batches_response.py
+-rw-r--r--   0        0        0     1226 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/queue_status.py
+-rw-r--r--   0        0        0     1346 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/retrieve_batch_analysis_response.py
+-rw-r--r--   0        0        0     3287 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/send_batch_request.py
+-rw-r--r--   0        0        0     1095 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/send_batch_response.py
+-rw-r--r--   0        0        0      154 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/status_enum.py
+-rw-r--r--   0        0        0     1342 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/batches/types/stop_active_batch_response.py
+-rw-r--r--   0        0        0      601 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/__init__.py
+-rw-r--r--   0        0        0    32314 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/client.py
+-rw-r--r--   0        0        0      869 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/__init__.py
+-rw-r--r--   0        0        0     1446 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/analyze_call.py
+-rw-r--r--   0        0        0     1687 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/analyze_call_response.py
+-rw-r--r--   0        0        0      184 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/answered_by_enum.py
+-rw-r--r--   0        0        0     1551 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/audio_recording_response.py
+-rw-r--r--   0        0        0     4901 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/call_details_response.py
+-rw-r--r--   0        0        0       83 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/call_id_param.py
+-rw-r--r--   0        0        0       76 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/goal.py
+-rw-r--r--   0        0        0     1036 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/list_calls_response.py
+-rw-r--r--   0        0        0     1237 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/listed_call_data.py
+-rw-r--r--   0        0        0     1244 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/stop_call_response.py
+-rw-r--r--   0        0        0     1032 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/transcript.py
+-rw-r--r--   0        0        0      178 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/calls/types/user_enum.py
+-rw-r--r--   0        0        0    36774 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/client.py
+-rw-r--r--   0        0        0      467 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/errors/__init__.py
+-rw-r--r--   0        0        0      274 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/errors/bad_request_error.py
+-rw-r--r--   0        0        0      270 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/errors/server_error.py
+-rw-r--r--   0        0        0      276 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      470 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/call_id.py
+-rw-r--r--   0        0        0     1561 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/custom_tool.py
+-rw-r--r--   0        0        0      867 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/error_body.py
+-rw-r--r--   0        0        0      897 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/error_detail.py
+-rw-r--r--   0        0        0      106 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/phone_number.py
+-rw-r--r--   0        0        0      150 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/status.py
+-rw-r--r--   0        0        0      166 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/tools.py
+-rw-r--r--   0        0        0       79 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/voice_id.py
+-rw-r--r--   0        0        0       79 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/commons/types/webhook.py
+-rw-r--r--   0        0        0      853 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/core/api_error.py
+-rw-r--r--   0        0        0     1484 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-13 06:45:42.271316 bland-0.3.0/src/bland/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/core/request_options.py
+-rw-r--r--   0        0        0      193 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/environment.py
+-rw-r--r--   0        0        0      571 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/__init__.py
+-rw-r--r--   0        0        0    40055 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/client.py
+-rw-r--r--   0        0        0      817 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/country_code.py
+-rw-r--r--   0        0        0     1444 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/inbound_number.py
+-rw-r--r--   0        0        0     1649 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_details_response.py
+-rw-r--r--   0        0        0     1802 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_request.py
+-rw-r--r--   0        0        0      930 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_response.py
+-rw-r--r--   0        0        0     1055 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/list_inbound_response.py
+-rw-r--r--   0        0        0      158 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/model.py
+-rw-r--r--   0        0        0     6666 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/update_inbound.py
+-rw-r--r--   0        0        0     1534 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/update_inbound_response.py
+-rw-r--r--   0        0        0     2259 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/inbound_numbers/types/voice_settings.py
+-rw-r--r--   0        0        0      267 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/__init__.py
+-rw-r--r--   0        0        0    12413 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/client.py
+-rw-r--r--   0        0        0      381 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/types/__init__.py
+-rw-r--r--   0        0        0     1024 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/types/list_outbound_response.py
+-rw-r--r--   0        0        0      983 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/types/outbound_number.py
+-rw-r--r--   0        0        0     1144 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/types/outbound_purchase.py
+-rw-r--r--   0        0        0      933 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/outbound_numbers/types/outbound_purchase_response.py
+-rw-r--r--   0        0        0        0 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/py.typed
+-rw-r--r--   0        0        0      923 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/__init__.py
+-rw-r--r--   0        0        0    46726 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/client.py
+-rw-r--r--   0        0        0     1376 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/__init__.py
+-rw-r--r--   0        0        0      170 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/a_2_p_status_enum.py
+-rw-r--r--   0        0        0      956 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/check_status_request.py
+-rw-r--r--   0        0        0     1273 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/check_status_response.py
+-rw-r--r--   0        0        0     1457 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/get_messages_request.py
+-rw-r--r--   0        0        0      971 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/get_messages_response.py
+-rw-r--r--   0        0        0      272 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/legal_structure_enum.py
+-rw-r--r--   0        0        0     2692 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/register_request.py
+-rw-r--r--   0        0        0      897 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/register_response.py
+-rw-r--r--   0        0        0      188 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/toggle_reply_enum.py
+-rw-r--r--   0        0        0     1221 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/toggle_reply_request.py
+-rw-r--r--   0        0        0     1011 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/toggle_reply_response.py
+-rw-r--r--   0        0        0     1112 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/trusted_user.py
+-rw-r--r--   0        0        0     1159 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/update_prompt_request.py
+-rw-r--r--   0        0        0      861 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/update_prompt_response.py
+-rw-r--r--   0        0        0     1211 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/update_webhook_request.py
+-rw-r--r--   0        0        0      862 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/update_webhook_response.py
+-rw-r--r--   0        0        0      902 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/sms/types/vertical_enum.py
+-rw-r--r--   0        0        0      851 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/__init__.py
+-rw-r--r--   0        0        0     2729 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/dynamic_data.py
+-rw-r--r--   0        0        0      125 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/interruption_threshold.py
+-rw-r--r--   0        0        0      149 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/method_enum.py
+-rw-r--r--   0        0        0      170 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/model_enum.py
+-rw-r--r--   0        0        0     1598 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/pronunciation_object.py
+-rw-r--r--   0        0        0      188 2024-05-13 06:45:42.275316 bland-0.3.0/src/bland/types/prounciation_guide.py
+-rw-r--r--   0        0        0     1392 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/response_data.py
+-rw-r--r--   0        0        0    10282 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/send_call.py
+-rw-r--r--   0        0        0     1798 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/send_call_response.py
+-rw-r--r--   0        0        0      117 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/temperature.py
+-rw-r--r--   0        0        0      117 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/transfer_list.py
+-rw-r--r--   0        0        0      166 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/types/voicemail_action.py
+-rw-r--r--   0        0        0       73 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/version.py
+-rw-r--r--   0        0        0      963 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/__init__.py
+-rw-r--r--   0        0        0    56110 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/client.py
+-rw-r--r--   0        0        0     1437 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/__init__.py
+-rw-r--r--   0        0        0     1965 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/create_voice_preset_request.py
+-rw-r--r--   0        0        0     1131 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/create_voice_preset_response.py
+-rw-r--r--   0        0        0     1085 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/delete_voice_preset_response.py
+-rw-r--r--   0        0        0     1250 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/generate_voice_sample_request.py
+-rw-r--r--   0        0        0     1018 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/generate_voice_sample_response.py
+-rw-r--r--   0        0        0     1193 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/list_voice_options_response.py
+-rw-r--r--   0        0        0      183 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/optimize_for.py
+-rw-r--r--   0        0        0     1063 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/preset.py
+-rw-r--r--   0        0        0     1167 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/publish_voice_preset_response.py
+-rw-r--r--   0        0        0     1028 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/retrieve_voice_preset_response.py
+-rw-r--r--   0        0        0     1996 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/retrieved_voice.py
+-rw-r--r--   0        0        0     2090 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/update_voice_preset_request.py
+-rw-r--r--   0        0        0     1329 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/update_voice_preset_response.py
+-rw-r--r--   0        0        0      907 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/voice.py
+-rw-r--r--   0        0        0     1718 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/voice_settings_data.py
+-rw-r--r--   0        0        0     1214 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/voices/types/voice_updates.py
+-rw-r--r--   0        0        0      193 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/web_agents/__init__.py
+-rw-r--r--   0        0        0    18124 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/web_agents/client.py
+-rw-r--r--   0        0        0      250 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/web_agents/types/__init__.py
+-rw-r--r--   0        0        0     4675 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/web_agents/types/create_web_agent_request.py
+-rw-r--r--   0        0        0     1060 2024-05-13 06:45:42.279316 bland-0.3.0/src/bland/web_agents/types/create_web_agent_response.py
+-rw-r--r--   0        0        0     5032 1970-01-01 00:00:00.000000 bland-0.3.0/PKG-INFO
```

### Comparing `bland-0.2.2/README.md` & `bland-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/__init__.py` & `bland-0.3.0/src/bland/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     ResponseData,
     SendCall,
     SendCallResponse,
     Temperature,
     TransferList,
     VoicemailAction,
 )
-from . import batches, calls, commons, inbound_numbers, outbound_numbers, sms, voices
+from . import batches, calls, commons, inbound_numbers, outbound_numbers, sms, voices, web_agents
 from .batches import (
     AnalysisObject,
     AnalyzeBatchRequest,
     BatchAnalysisObject,
     BatchCallData,
     BatchDetailsResponse,
     BatchObject,
@@ -92,14 +92,15 @@
     TrustedUser,
     UpdatePromptRequest,
     UpdatePromptResponse,
     UpdateWebhookRequest,
     UpdateWebhookResponse,
     VerticalEnum,
 )
+from .version import __version__
 from .voices import (
     CreateVoicePresetRequest,
     CreateVoicePresetResponse,
     DeleteVoicePresetResponse,
     GenerateVoiceSampleRequest,
     GenerateVoiceSampleResponse,
     ListVoiceOptionsResponse,
@@ -110,14 +111,15 @@
     RetrievedVoice,
     UpdateVoicePresetRequest,
     UpdateVoicePresetResponse,
     Voice,
     VoiceSettingsData,
     VoiceUpdates,
 )
+from .web_agents import CreateWebAgentRequest, CreateWebAgentResponse
 
 __all__ = [
     "A2PStatusEnum",
     "AnalysisObject",
     "AnalyzeBatchRequest",
     "AnalyzeCall",
     "AnalyzeCallResponse",
@@ -138,14 +140,16 @@
     "CallLengthSummary",
     "CallParams",
     "CheckStatusRequest",
     "CheckStatusResponse",
     "CountryCode",
     "CreateVoicePresetRequest",
     "CreateVoicePresetResponse",
+    "CreateWebAgentRequest",
+    "CreateWebAgentResponse",
     "CustomTool",
     "DeleteVoicePresetResponse",
     "DynamicData",
     "ErrorBody",
     "ErrorDetail",
     "GenerateVoiceSampleRequest",
     "GenerateVoiceSampleResponse",
@@ -214,15 +218,17 @@
     "Voice",
     "VoiceId",
     "VoiceSettings",
     "VoiceSettingsData",
     "VoiceUpdates",
     "VoicemailAction",
     "Webhook",
+    "__version__",
     "batches",
     "calls",
     "commons",
     "inbound_numbers",
     "outbound_numbers",
     "sms",
     "voices",
+    "web_agents",
 ]
```

### Comparing `bland-0.2.2/src/blandai/batches/__init__.py` & `bland-0.3.0/src/bland/batches/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/batches/client.py` & `bland-0.3.0/src/bland/calls/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,160 +1,156 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ..calls.types.analyze_call_response import AnalyzeCallResponse
 from ..commons.errors.server_error import ServerError
 from ..commons.errors.unauthorized_error import UnauthorizedError
 from ..commons.types.error_body import ErrorBody
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
-from .types.analyze_batch_request import AnalyzeBatchRequest
-from .types.batch_details_response import BatchDetailsResponse
-from .types.list_batches_response import ListBatchesResponse
-from .types.retrieve_batch_analysis_response import RetrieveBatchAnalysisResponse
-from .types.send_batch_request import SendBatchRequest
-from .types.send_batch_response import SendBatchResponse
-from .types.stop_active_batch_response import StopActiveBatchResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from .types.analyze_call_response import AnalyzeCallResponse
+from .types.audio_recording_response import AudioRecordingResponse
+from .types.call_details_response import CallDetailsResponse
+from .types.call_id_param import CallIdParam
+from .types.goal import Goal
+from .types.list_calls_response import ListCallsResponse
+from .types.stop_call_response import StopCallResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class BatchesClient:
+class CallsClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def send(
-        self, *, request: SendBatchRequest, request_options: typing.Optional[RequestOptions] = None
-    ) -> SendBatchResponse:
+    def analyze(
+        self,
+        call_id: CallIdParam,
+        *,
+        goal: Goal,
+        questions: typing.Sequence[typing.Sequence[str]],
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> AnalyzeCallResponse:
         """
-        Send large volumes of calls at once with a single API request.
+        Analyzes a call of calls based using questions and goals.
 
-        Parameters:
-            - request: SendBatchRequest.
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/batches"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SendBatchResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        goal : Goal
+            This is the overall purpose of the call. Provides context for the analysis to guide how the questions/transcripts are interpreted.
 
-    def analyze(
-        self, batch_id: str, *, request: AnalyzeBatchRequest, request_options: typing.Optional[RequestOptions] = None
-    ) -> AnalyzeCallResponse:
-        """
-        Analyzes a batch of calls based on using questions and goals.
+        questions : typing.Sequence[typing.Sequence[str]]
+            An array of questions to be analyzed for the call.
+
+            Each question should be an array with two elements - the question text and the expected answer type (e.g., “string”, “boolean”).
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls to be analyzed.
+            Fairly flexible in terms of the expected answer type, and unanswerable questions will default to `null`.
 
-            - request: AnalyzeBatchRequest.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Returns
+        -------
+        AnalyzeCallResponse
+
+        Examples
+        --------
+        from bland.client import BlandAI
+
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.calls.analyze(
+            call_id="string",
+            goal="string",
+            questions=[["string"]],
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {"goal": goal, "questions": questions}
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/analyze"
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/analyze"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AnalyzeCallResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AnalyzeCallResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def stop(
-        self, batch_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> StopActiveBatchResponse:
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> StopCallResponse:
         """
-        Stops all active calls in a batch.
+        End an active phone call by call_id.
+
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls to be cancelled.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Returns
+        -------
+        StopCallResponse
+
+        Examples
+        --------
+        from bland.client import BlandAI
+
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.calls.stop(
+            call_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/stop"
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/stop"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
@@ -164,104 +160,103 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StopActiveBatchResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(StopCallResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListBatchesResponse:
-        """
-        Retrieves batch-specific data for each batch you've created.
-
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/batches"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListBatchesResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    def details(
+    def list(
         self,
-        batch_id: str,
         *,
-        include_calls: typing.Optional[bool] = None,
-        include_transcripts: typing.Optional[bool] = None,
-        include_analysis: typing.Optional[bool] = None,
+        from_number: typing.Optional[str] = None,
+        to_number: typing.Optional[str] = None,
+        from_: typing.Optional[int] = None,
+        to: typing.Optional[int] = None,
+        limit: typing.Optional[int] = None,
+        ascending: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
-    ) -> BatchDetailsResponse:
+    ) -> ListCallsResponse:
         """
-        Retrieves calls and batch data for a specific batch_id.
+        Returns a set of metadata for each call dispatched by your account.
+
+        Parameters
+        ----------
+        from_number : typing.Optional[str]
+            Filter calls by the number they were dispatched from.
+
+            The number that initiated the call - the user's phone number for inbound calls, or the number your AI Agent called from for outbound calls.
+
+        to_number : typing.Optional[str]
+            Filter calls by the number they were dispatched to.
+
+            The number that answered the call - the user's phone number for outbound calls, or your AI Agent's number for inbound calls.
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls you want to retrieve.
+        from_ : typing.Optional[int]
+            The starting index (inclusive) for the range of calls to retrieve.
 
-            - include_calls: typing.Optional[bool]. Whether or not to include individual call data in the response.
+        to : typing.Optional[int]
+            The ending index for the range of calls to retrieve.
 
-                                                    If no value is provided, `include_calls` defaults to `true`.
-            - include_transcripts: typing.Optional[bool]. If calls are included, can be set to false to exclude transcripts from the response.
+        limit : typing.Optional[int]
+            The maximum number of calls to return in the response.
 
-                                                          If no value is provided, `include_transcripts` defaults to `true`.
-            - include_analysis: typing.Optional[bool]. If calls are included, can be set to false to exclude analysis from the response.
+        ascending : typing.Optional[bool]
+            Whether to sort the calls in ascending order of their creation time.
 
-                                                       If no value is provided, `include_analysis` defaults to `true`.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListCallsResponse
+
+        Examples
+        --------
+        from bland.client import BlandAI
+
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.calls.list(
+            from_number="string",
+            to_number="string",
+            from_=1,
+            to=1,
+            limit=1,
+            ascending=True,
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/calls"),
             params=jsonable_encoder(
                 remove_none_from_dict(
                     {
-                        "include_calls": include_calls,
-                        "include_transcripts": include_transcripts,
-                        "include_analysis": include_analysis,
+                        "from_number": from_number,
+                        "to_number": to_number,
+                        "from": from_,
+                        "to": to,
+                        "limit": limit,
+                        "ascending": ascending,
                         **(
                             request_options.get("additional_query_parameters", {})
                             if request_options is not None
                             else {}
                         ),
                     }
                 )
@@ -272,197 +267,277 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BatchDetailsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListCallsResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def retrieve(
-        self, batch_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> RetrieveBatchAnalysisResponse:
+    def details(
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> CallDetailsResponse:
         """
-        Retrieves the analyses for a specific batch of calls, including details of each call's analysis.
+        Retrieve detailed information, metadata and transcripts for a call.
+
+        Parameters
+        ----------
+        call_id : CallIdParam
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - batch_id: str. The unique identifier for the call batch. Returned in the response when creating a batch, or when listing all batches.
+        Returns
+        -------
+        CallDetailsResponse
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Examples
+        --------
+        from bland.client import BlandAI
+
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.calls.details(
+            call_id="string",
+        )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/analysis"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RetrieveBatchAnalysisResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(CallDetailsResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def recording(
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> AudioRecordingResponse:
+        """
+        Retrieve your call's audio recording.
 
-class AsyncBatchesClient:
-    def __init__(self, *, client_wrapper: AsyncClientWrapper):
-        self._client_wrapper = client_wrapper
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-    async def send(
-        self, *, request: SendBatchRequest, request_options: typing.Optional[RequestOptions] = None
-    ) -> SendBatchResponse:
-        """
-        Send large volumes of calls at once with a single API request.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudioRecordingResponse
 
-        Parameters:
-            - request: SendBatchRequest.
+        Examples
+        --------
+        from bland.client import BlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.calls.recording(
+            call_id="string",
+        )
         """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/batches"),
+        _response = self._client_wrapper.httpx_client.request(
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/recording"
+            ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(SendBatchResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AudioRecordingResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+
+class AsyncCallsClient:
+    def __init__(self, *, client_wrapper: AsyncClientWrapper):
+        self._client_wrapper = client_wrapper
+
     async def analyze(
-        self, batch_id: str, *, request: AnalyzeBatchRequest, request_options: typing.Optional[RequestOptions] = None
+        self,
+        call_id: CallIdParam,
+        *,
+        goal: Goal,
+        questions: typing.Sequence[typing.Sequence[str]],
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> AnalyzeCallResponse:
         """
-        Analyzes a batch of calls based on using questions and goals.
+        Analyzes a call of calls based using questions and goals.
+
+        Parameters
+        ----------
+        call_id : CallIdParam
+
+        goal : Goal
+            This is the overall purpose of the call. Provides context for the analysis to guide how the questions/transcripts are interpreted.
+
+        questions : typing.Sequence[typing.Sequence[str]]
+            An array of questions to be analyzed for the call.
+
+            Each question should be an array with two elements - the question text and the expected answer type (e.g., “string”, “boolean”).
+
+            Fairly flexible in terms of the expected answer type, and unanswerable questions will default to `null`.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls to be analyzed.
+        Returns
+        -------
+        AnalyzeCallResponse
 
-            - request: AnalyzeBatchRequest.
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.calls.analyze(
+            call_id="string",
+            goal="string",
+            questions=[["string"]],
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {"goal": goal, "questions": questions}
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/analyze"
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/analyze"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(AnalyzeCallResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AnalyzeCallResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def stop(
-        self, batch_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> StopActiveBatchResponse:
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> StopCallResponse:
         """
-        Stops all active calls in a batch.
+        End an active phone call by call_id.
+
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls to be cancelled.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        Returns
+        -------
+        StopCallResponse
+
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
+
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.calls.stop(
+            call_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/stop"
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/stop"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
@@ -472,175 +547,253 @@
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(StopActiveBatchResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(StopCallResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListBatchesResponse:
+    async def list(
+        self,
+        *,
+        from_number: typing.Optional[str] = None,
+        to_number: typing.Optional[str] = None,
+        from_: typing.Optional[int] = None,
+        to: typing.Optional[int] = None,
+        limit: typing.Optional[int] = None,
+        ascending: typing.Optional[bool] = None,
+        request_options: typing.Optional[RequestOptions] = None,
+    ) -> ListCallsResponse:
         """
-        Retrieves batch-specific data for each batch you've created.
+        Returns a set of metadata for each call dispatched by your account.
+
+        Parameters
+        ----------
+        from_number : typing.Optional[str]
+            Filter calls by the number they were dispatched from.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+            The number that initiated the call - the user's phone number for inbound calls, or the number your AI Agent called from for outbound calls.
+
+        to_number : typing.Optional[str]
+            Filter calls by the number they were dispatched to.
+
+            The number that answered the call - the user's phone number for outbound calls, or your AI Agent's number for inbound calls.
+
+        from_ : typing.Optional[int]
+            The starting index (inclusive) for the range of calls to retrieve.
+
+        to : typing.Optional[int]
+            The ending index for the range of calls to retrieve.
+
+        limit : typing.Optional[int]
+            The maximum number of calls to return in the response.
+
+        ascending : typing.Optional[bool]
+            Whether to sort the calls in ascending order of their creation time.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListCallsResponse
+
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
+
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.calls.list(
+            from_number="string",
+            to_number="string",
+            from_=1,
+            to=1,
+            limit=1,
+            ascending=True,
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/batches"),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/calls"),
             params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+                remove_none_from_dict(
+                    {
+                        "from_number": from_number,
+                        "to_number": to_number,
+                        "from": from_,
+                        "to": to,
+                        "limit": limit,
+                        "ascending": ascending,
+                        **(
+                            request_options.get("additional_query_parameters", {})
+                            if request_options is not None
+                            else {}
+                        ),
+                    }
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListBatchesResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListCallsResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def details(
-        self,
-        batch_id: str,
-        *,
-        include_calls: typing.Optional[bool] = None,
-        include_transcripts: typing.Optional[bool] = None,
-        include_analysis: typing.Optional[bool] = None,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> BatchDetailsResponse:
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> CallDetailsResponse:
         """
-        Retrieves calls and batch data for a specific batch_id.
+        Retrieve detailed information, metadata and transcripts for a call.
 
-        Parameters:
-            - batch_id: str. The unique identifier for the batch of calls you want to retrieve.
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-            - include_calls: typing.Optional[bool]. Whether or not to include individual call data in the response.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-                                                    If no value is provided, `include_calls` defaults to `true`.
-            - include_transcripts: typing.Optional[bool]. If calls are included, can be set to false to exclude transcripts from the response.
+        Returns
+        -------
+        CallDetailsResponse
 
-                                                          If no value is provided, `include_transcripts` defaults to `true`.
-            - include_analysis: typing.Optional[bool]. If calls are included, can be set to false to exclude analysis from the response.
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
 
-                                                       If no value is provided, `include_analysis` defaults to `true`.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.calls.details(
+            call_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}"),
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}"
+            ),
             params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "include_calls": include_calls,
-                        "include_transcripts": include_transcripts,
-                        "include_analysis": include_analysis,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
-                )
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(BatchDetailsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(CallDetailsResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def retrieve(
-        self, batch_id: str, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> RetrieveBatchAnalysisResponse:
+    async def recording(
+        self, call_id: CallIdParam, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> AudioRecordingResponse:
         """
-        Retrieves the analyses for a specific batch of calls, including details of each call's analysis.
+        Retrieve your call's audio recording.
 
-        Parameters:
-            - batch_id: str. The unique identifier for the call batch. Returned in the response when creating a batch, or when listing all batches.
+        Parameters
+        ----------
+        call_id : CallIdParam
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        AudioRecordingResponse
+
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
+
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.calls.recording(
+            call_id="string",
+        )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/batches/{jsonable_encoder(batch_id)}/analysis"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/calls/{jsonable_encoder(call_id)}/recording"
             ),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(RetrieveBatchAnalysisResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(AudioRecordingResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bland-0.2.2/src/blandai/batches/types/__init__.py` & `bland-0.3.0/src/bland/batches/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/batches/types/analysis_object.py` & `bland-0.3.0/src/bland/batches/types/analysis_object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .call_length import CallLength
 from .queue_status import QueueStatus
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AnalysisObject(pydantic.BaseModel):
+class AnalysisObject(pydantic_v1.BaseModel):
     """
-    from blandai import AnalysisObject, CallLength, CallLengthSummary, QueueStatus
+    Examples
+    --------
+    from bland import AnalysisObject, CallLength, CallLengthSummary, QueueStatus
 
     AnalysisObject(
         total_calls=3,
         completed_calls=2,
         in_progress_calls=1,
         queue_statuses=QueueStatus(
             complete=2,
@@ -37,64 +35,64 @@
                 _20_30=0,
                 _30_45=0,
                 _45_60=0,
                 _60_90=0,
                 _90_120=0,
                 _120=0,
             ),
-            all=[5, 5, 11],
+            all_=[5, 5, 11],
         ),
         call_ids=[
             "73c809a9-db35-4edb-8fa6-95a6a942daf8",
             "73c809a9-db35-4edb-8fa6-95a6a942daf9",
             "73c809a9-db35-4edb-8fa6-95a6a942daf0",
         ],
         error_messages=[
             "Cannot transfer to +12223334444 - Call is no longer active."
         ],
         endpoints={"API": "3"},
     )
     """
 
-    total_calls: int = pydantic.Field()
+    total_calls: int = pydantic_v1.Field()
     """
     The total number of calls in the batch, including completed and in-progress calls.
     """
 
-    completed_calls: int = pydantic.Field()
+    completed_calls: int = pydantic_v1.Field()
     """
     The total number of completed calls in the batch.
     """
 
-    in_progress_calls: int = pydantic.Field()
+    in_progress_calls: int = pydantic_v1.Field()
     """
     The total number of in-progress calls in the batch.
     """
 
-    queue_statuses: QueueStatus = pydantic.Field()
+    queue_statuses: QueueStatus = pydantic_v1.Field()
     """
     An object containing the number of calls in each queue status.
     """
 
-    call_lengths: CallLength = pydantic.Field()
+    call_lengths: CallLength = pydantic_v1.Field()
     """
     Contains `average`, `average_nonzero`, `summary` and `all` fields.
     """
 
-    call_ids: typing.List[str] = pydantic.Field()
+    call_ids: typing.List[str] = pydantic_v1.Field()
     """
     Contains each `call_id` in the batch.
     """
 
-    error_messages: typing.List[str] = pydantic.Field()
+    error_messages: typing.List[str] = pydantic_v1.Field()
     """
     Contains any error messages that calls in the batch may have.
     """
 
-    endpoints: typing.Dict[str, str] = pydantic.Field()
+    endpoints: typing.Dict[str, str] = pydantic_v1.Field()
     """
     Contains the number of calls that have been sent to each endpoint. Applicable only to API integrations.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -102,8 +100,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/analyze_batch_request.py` & `bland-0.3.0/src/bland/batches/types/analyze_batch_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AnalyzeBatchRequest(pydantic.BaseModel):
+class AnalyzeBatchRequest(pydantic_v1.BaseModel):
     """
-    from blandai import AnalyzeBatchRequest
+    Examples
+    --------
+    from bland import AnalyzeBatchRequest
 
     AnalyzeBatchRequest(
         goal="Renewal Confirmation",
         questions=[
             ["Who answered the call?", "human or voicemail"],
             ["Positive feedback about the product: ", "string"],
             ["Negative feedback about the product: ", "string"],
             ["Customer confirmed they were satisfied", "boolean"],
         ],
     )
     """
 
-    goal: str = pydantic.Field()
+    goal: str = pydantic_v1.Field()
     """
     This is the overall purpose of the batch of calls. Provides context for the analysis to guide how the questions/transcripts are interpreted.
     """
 
-    questions: typing.List[typing.List[str]] = pydantic.Field()
+    questions: typing.List[typing.List[str]] = pydantic_v1.Field()
     """
     An array of questions to be analyzed for each call in the batch.
     
     Each question should be an array with two elements: the question text and the expected answer type (e.g., “string”, “boolean”).
     
     Fairly flexible in terms of the expected answer type, and unanswerable questions will default to `null`.
     """
@@ -47,8 +45,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/batch_analysis_object.py` & `bland-0.3.0/src/bland/batches/types/batch_analysis_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BatchAnalysisObject(pydantic.BaseModel):
+class BatchAnalysisObject(pydantic_v1.BaseModel):
     call_id: str
     batch_id: str
     goal: str
-    answers: typing.List[str] = pydantic.Field()
+    answers: typing.List[str] = pydantic_v1.Field()
     """
     The results of the AI analysis.
     """
 
-    questions: typing.List[str] = pydantic.Field()
+    questions: typing.List[str] = pydantic_v1.Field()
     """
     The original questions asked by the AI.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -32,8 +28,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/batch_call_data.py` & `bland-0.3.0/src/bland/batches/types/batch_call_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BatchCallData(pydantic.BaseModel):
-    phone_number: PhoneNumber = pydantic.Field()
+class BatchCallData(pydantic_v1.BaseModel):
+    phone_number: PhoneNumber = pydantic_v1.Field()
     """
     The phone number to call.
     """
 
-    business: typing.Optional[str] = pydantic.Field(default=None)
+    business: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The name of the business or person being called.
     """
 
-    service: typing.Optional[str] = pydantic.Field(default=None)
+    service: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The service or product being discussed.
     """
 
-    date: typing.Optional[str] = pydantic.Field(default=None)
+    date: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The date of the event or deadline being discussed.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -40,8 +36,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/batch_details_response.py` & `bland-0.3.0/src/bland/batches/types/list_batches_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .analysis_object import AnalysisObject
-from .batch_params import BatchParams
-from .call_data import CallData
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ...core.pydantic_utilities import pydantic_v1
+from .batch_object import BatchObject
 
 
-class BatchDetailsResponse(pydantic.BaseModel):
-    batch_params: BatchParams = pydantic.Field()
+class ListBatchesResponse(pydantic_v1.BaseModel):
+    status: str = pydantic_v1.Field()
     """
-    An object containing parameters and settings for the batch.
+    Can be `success` or `error`.
     """
 
-    analysis: AnalysisObject = pydantic.Field()
+    batches: typing.List[BatchObject] = pydantic_v1.Field()
     """
-    An object containing analysis data for the batch.
-    """
-
-    call_data: typing.List[CallData] = pydantic.Field()
-    """
-    An array of objects, each representing individual call data.
+    An array of batch objects.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/batch_object.py` & `bland-0.3.0/src/bland/batches/types/batch_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .call_params import CallParams
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BatchObject(pydantic.BaseModel):
-    batch_id: str = pydantic.Field()
+class BatchObject(pydantic_v1.BaseModel):
+    batch_id: str = pydantic_v1.Field()
     """
     The unique identifier for the batch.
     """
 
     campaign_id: str
-    created_at: dt.datetime = pydantic.Field()
+    created_at: dt.datetime = pydantic_v1.Field()
     """
     The date and time the batch was created.
     """
 
-    label: str = pydantic.Field()
+    label: str = pydantic_v1.Field()
     """
     The label you assigned to the batch (if any).
     """
 
-    base_prompt: str = pydantic.Field()
+    base_prompt: str = pydantic_v1.Field()
     """
     The prompt or task used for all the phone calls in the batch.
     """
 
-    endpoint_code: str = pydantic.Field()
+    endpoint_code: str = pydantic_v1.Field()
     """
     Enterprise customers with custom endpoints will see the endpoint code here (if specified).
     
     The default value is `API`.
     """
 
-    call_params: CallParams = pydantic.Field()
+    call_params: CallParams = pydantic_v1.Field()
     """
     The base call parameters used to create the batch.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -53,8 +49,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/batch_params.py` & `bland-0.3.0/src/bland/batches/types/batch_params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .call_params import CallParams
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class BatchParams(pydantic.BaseModel):
-    id: str = pydantic.Field()
+class BatchParams(pydantic_v1.BaseModel):
+    id: str = pydantic_v1.Field()
     """
     The unique identifier of the batch - used as the `batch_id` parameter in other API calls.
     """
 
     campaign_id: typing.Optional[str] = None
-    created_at: dt.datetime = pydantic.Field()
+    created_at: dt.datetime = pydantic_v1.Field()
     """
     The creation timestamp of the batch.
     """
 
-    label: str = pydantic.Field()
+    label: str = pydantic_v1.Field()
     """
     The label or description of the batch.
     """
 
-    base_prompt: str = pydantic.Field()
+    base_prompt: str = pydantic_v1.Field()
     """
     The base prompt used for calls in this batch.
     """
 
-    endpoint_code: str = pydantic.Field()
+    endpoint_code: str = pydantic_v1.Field()
     """
     The endpoint code used for API integration.
     """
 
-    call_params: CallParams = pydantic.Field()
+    call_params: CallParams = pydantic_v1.Field()
     """
     An object containing parameters for the calls in the batch.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -51,8 +47,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/call_data.py` & `bland-0.3.0/src/bland/batches/types/batch_details_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...calls.types.answered_by_enum import AnsweredByEnum
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .analysis_object import AnalysisObject
+from .batch_params import BatchParams
+from .call_data import CallData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CallData(pydantic.BaseModel):
-    created_at: dt.datetime = pydantic.Field()
-    """
-    The timestamp when the individual call was created.
-    """
-
-    to: str = pydantic.Field()
-    """
-    The phone number the call was made to.
-    """
-
-    from_: str = pydantic.Field(alias="from")
-    """
-    The phone number the call was made from.
-    """
-
-    completed: bool = pydantic.Field()
-    """
-    Indicates if the call was completed.
-    """
-
-    call_id: str = pydantic.Field()
+class BatchDetailsResponse(pydantic_v1.BaseModel):
+    batch_params: BatchParams = pydantic_v1.Field()
     """
-    The unique identifier for each individual call.
+    An object containing parameters and settings for the batch.
     """
 
-    call_length: int = pydantic.Field()
+    analysis: AnalysisObject = pydantic_v1.Field()
     """
-    The duration of the call in minutes.
+    An object containing analysis data for the batch.
     """
 
-    answered_by: typing.Optional[AnsweredByEnum] = pydantic.Field(default=None)
+    call_data: typing.List[CallData] = pydantic_v1.Field()
     """
-    Contains a string value if the batch had `answered_by_enabled` set to `true`.
+    An array of objects, each representing individual call data.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/call_length.py` & `bland-0.3.0/src/bland/batches/types/call_length.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .call_length_summary import CallLengthSummary
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CallLength(pydantic.BaseModel):
-    average: int = pydantic.Field()
+class CallLength(pydantic_v1.BaseModel):
+    average: int = pydantic_v1.Field()
     """
     The average call length in minutes.
     """
 
-    average_nonzero: int = pydantic.Field()
+    average_nonzero: int = pydantic_v1.Field()
     """
     The average call length in minutes, excluding calls with a length of less than one second.
     """
 
-    summary: CallLengthSummary = pydantic.Field()
+    summary: CallLengthSummary = pydantic_v1.Field()
     """
     A summary of the call lengths, grouped into ranges.
     """
 
-    all: typing.List[int] = pydantic.Field()
+    all_: typing.List[int] = pydantic_v1.Field(alias="all")
     """
     Contains each call length, in case you want to use a different grouping than the default.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -40,8 +36,11 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/call_length_summary.py` & `bland-0.3.0/src/bland/batches/types/call_length_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class CallLengthSummary(pydantic.BaseModel):
-    _0_5: int = pydantic.Field(alias="0-5")
-    _5_10: int = pydantic.Field(alias="5-10")
-    _10_15: int = pydantic.Field(alias="10-15")
-    _15_20: int = pydantic.Field(alias="15-20")
-    _20_30: int = pydantic.Field(alias="20-30")
-    _30_45: int = pydantic.Field(alias="30-45")
-    _45_60: int = pydantic.Field(alias="45-60")
-    _60_90: int = pydantic.Field(alias="60-90")
-    _90_120: int = pydantic.Field(alias="90-120")
-    _120: int = pydantic.Field(alias="120+")
+
+class CallLengthSummary(pydantic_v1.BaseModel):
+    _0_5: int = pydantic_v1.Field(alias="0-5")
+    _5_10: int = pydantic_v1.Field(alias="5-10")
+    _10_15: int = pydantic_v1.Field(alias="10-15")
+    _15_20: int = pydantic_v1.Field(alias="15-20")
+    _20_30: int = pydantic_v1.Field(alias="20-30")
+    _30_45: int = pydantic_v1.Field(alias="30-45")
+    _45_60: int = pydantic_v1.Field(alias="45-60")
+    _60_90: int = pydantic_v1.Field(alias="60-90")
+    _90_120: int = pydantic_v1.Field(alias="90-120")
+    _120: int = pydantic_v1.Field(alias="120+")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/call_params.py` & `bland-0.3.0/src/bland/sms/types/trusted_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CallParams(pydantic.BaseModel):
-    reduce_latency: bool
-    voice_id: int
-    language: str
-    request_data: typing.Any
-    max_duration: int
-    wait_for_greeting: bool
+class TrustedUser(pydantic_v1.BaseModel):
+    position: typing.Optional[str] = None
+    first_name: typing.Optional[str] = None
+    last_name: typing.Optional[str] = None
+    phone_number: typing.Optional[PhoneNumber] = None
+    email: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/list_batches_response.py` & `bland-0.3.0/src/bland/sms/types/toggle_reply_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
-from .batch_object import BatchObject
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListBatchesResponse(pydantic.BaseModel):
-    status: str = pydantic.Field()
+class ToggleReplyRequest(pydantic_v1.BaseModel):
+    phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
     """
-    Can be `success` or `error`.
+    The phone number to update.
     """
 
-    batches: typing.List[BatchObject] = pydantic.Field()
+    on: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    An array of batch objects.
+    Turn human mode on or off.
+    
+    `true` means that the AI will not reply. `false` means the AI will reply.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/queue_status.py` & `bland-0.3.0/src/bland/batches/types/queue_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class QueueStatus(pydantic.BaseModel):
-    complete: typing.Optional[int] = pydantic.Field(default=None)
+class QueueStatus(pydantic_v1.BaseModel):
+    complete: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of completed calls in the batch.
     """
 
-    queued: typing.Optional[int] = pydantic.Field(default=None)
+    queued: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of calls that are queued.
     """
 
-    call_error: typing.Optional[int] = pydantic.Field(default=None)
+    call_error: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of calls that have an error.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -34,8 +30,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/retrieve_batch_analysis_response.py` & `bland-0.3.0/src/bland/voices/types/retrieve_voice_preset_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .batch_analysis_object import BatchAnalysisObject
-from .status_enum import StatusEnum
+from ...core.pydantic_utilities import pydantic_v1
+from .retrieved_voice import RetrievedVoice
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RetrieveBatchAnalysisResponse(pydantic.BaseModel):
-    status: StatusEnum = pydantic.Field()
-    """
-    Whether the request was successful or not.
-    """
-
-    message: str = pydantic.Field()
-    """
-    An error message or confirmation that the request was successful.
-    """
-
-    analysis: typing.List[BatchAnalysisObject] = pydantic.Field()
+class RetrieveVoicePresetResponse(pydantic_v1.BaseModel):
+    voice: RetrievedVoice = pydantic_v1.Field()
     """
-    An array of analysis objects, each corresponding to a call within the batch.
+    Contains detailed information about the specified voice preset.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/send_batch_request.py` & `bland-0.3.0/src/bland/batches/types/send_batch_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from ...types.send_call import SendCall
 from .batch_call_data import BatchCallData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 
 class SendBatchRequest(SendCall):
     """
-    from blandai import BatchCallData, SendBatchRequest
+    Examples
+    --------
+    from bland import BatchCallData, SendBatchRequest
 
     SendBatchRequest(
         phone_number="29382721828",
         task="Would love for you to check out our AI API!",
         base_prompt="You are calling a business to renew their subscription to a service before it expires on a date.",
         call_data=[
             BatchCallData(
@@ -37,39 +35,39 @@
         ],
         label="Subscription Renewal",
         campaign_id="1234",
         test_mode=True,
     )
     """
 
-    base_prompt: str = pydantic.Field()
+    base_prompt: str = pydantic_v1.Field()
     """
     This is the prompt or task used for all the phone calls in the request.
     
     Information can be inserted into it surrounding variable names with double curly braces.
     """
 
-    call_data: typing.List[BatchCallData] = pydantic.Field()
+    call_data: typing.List[BatchCallData] = pydantic_v1.Field()
     """
     Define a list of calls to make and their properties.
     
     Each call in call_data **MUST** have a `phone_number` property. Properties are case-sensitive.
     """
 
-    label: typing.Optional[str] = pydantic.Field(default=None)
+    label: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Adds a user-friendly label to your batch to keep track of it's original intention. This can help differentiate multiple call batches that are part of the same Campaign. Shown when a batch is retreived.
     """
 
-    campaign_id: typing.Optional[str] = pydantic.Field(default=None)
+    campaign_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Use `campaign_id` to organize related batches together. This can be set manually or auto-generated through Campaigns.
     """
 
-    test_mode: typing.Optional[bool] = pydantic.Field(default=None)
+    test_mode: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     When this is set to `true`, only the first call of `call_data` will be dispatched. A common use case is to set the first `phone_number` value to your own to confirm everything's set up properly.
     
     Includes additional information in the response when true so that it's easier to find any issues.
     
     If no value is provided, `test_mode` defaults to `false`.
     """
@@ -82,8 +80,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/send_batch_response.py` & `bland-0.3.0/src/bland/batches/types/send_batch_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SendBatchResponse(pydantic.BaseModel):
-    message: str = pydantic.Field()
+class SendBatchResponse(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
     """
     The type of response returned. This will always be “success” if the request was successful.
     """
 
-    batch_id: str = pydantic.Field()
+    batch_id: str = pydantic_v1.Field()
     """
     The unique identifier for the batch.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -29,8 +25,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/batches/types/stop_active_batch_response.py` & `bland-0.3.0/src/bland/batches/types/stop_active_batch_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StopActiveBatchResponse(pydantic.BaseModel):
-    status: str = pydantic.Field()
+class StopActiveBatchResponse(pydantic_v1.BaseModel):
+    status: str = pydantic_v1.Field()
     """
     The status of the request. If anything other than 'success', an error has occurred or all calls have already been completed.
     """
 
-    message: str = pydantic.Field()
+    message: str = pydantic_v1.Field()
     """
     A message describing the status of the request.
     """
 
-    num_calls: int = pydantic.Field()
+    num_calls: int = pydantic_v1.Field()
     """
     The number of calls that were cancelled.
     """
 
-    batch_id: str = pydantic.Field()
+    batch_id: str = pydantic_v1.Field()
     """
     The `batch_id` of the cancelled batch.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -39,8 +35,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/__init__.py` & `bland-0.3.0/src/bland/calls/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/calls/types/__init__.py` & `bland-0.3.0/src/bland/calls/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/calls/types/analyze_call.py` & `bland-0.3.0/src/bland/calls/types/analyze_call_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.status import Status
 from ...core.datetime_utils import serialize_datetime
-from .goal import Goal
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class AnalyzeCallResponse(pydantic_v1.BaseModel):
+    status: Status = pydantic_v1.Field()
+    """
+    Will be `success` if the request was successful.
+    """
+
+    message: str = pydantic_v1.Field()
+    """
+    Confirms the request was successful, or provides an error message if the request failed.
+    """
 
-class AnalyzeCall(pydantic.BaseModel):
-    goal: Goal = pydantic.Field()
+    answers: typing.List[typing.List[typing.Any]] = pydantic_v1.Field()
     """
-    This is the overall purpose of the call. Provides context for the analysis to guide how the questions/transcripts are interpreted.
+    Contains the analyzed answers for the call in an array.
     """
 
-    questions: typing.List[typing.List[str]] = pydantic.Field()
+    credits_used: int = pydantic_v1.Field()
     """
-    An array of questions to be analyzed for the call.
+    Token-based price for the analysis request.
     
-    Each question should be an array with two elements - the question text and the expected answer type (e.g., “string”, “boolean”).
+    As a rough estimate, the base cost is `0.003` credits with an additional `0.0015` credits per call in the call.
     
-    Fairly flexible in terms of the expected answer type, and unanswerable questions will default to `null`.
+    Longer call transcripts and higher numbers of questions can increase the cost, however the cost scales very effectively with calls vs. individual calls.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bland-0.2.2/src/blandai/calls/types/analyze_call_response.py` & `bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_details_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.status import Status
+from ...commons.types.phone_number import PhoneNumber
+from ...commons.types.voice_id import VoiceId
+from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class InboundNumberDetailsResponse(pydantic_v1.BaseModel):
+    created_at: str = pydantic_v1.Field()
+    """
+    The timestamp when the inbound number was configured.
+    """
 
-class AnalyzeCallResponse(pydantic.BaseModel):
-    status: Status = pydantic.Field()
+    phone_number: PhoneNumber = pydantic_v1.Field()
     """
-    Will be `success` if the request was successful.
+    The specific inbound phone number.
     """
 
-    message: str = pydantic.Field()
+    prompt: str = pydantic_v1.Field()
     """
-    Confirms the request was successful, or provides an error message if the request failed.
+    The prompt your agent is using.
     """
 
-    answers: typing.List[typing.List[typing.Any]] = pydantic.Field()
+    webhook: Webhook
+    voice_id: VoiceId
+    dynamic_data: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Contains the analyzed answers for the call in an array.
+    Any dynamic data associated with the inbound number, if applicable.
     """
 
-    credits_used: int = pydantic.Field()
+    max_duration: int = pydantic_v1.Field()
     """
-    Token-based price for the analysis request.
-    
-    As a rough estimate, the base cost is `0.003` credits with an additional `0.0015` credits per call in the call.
-    
-    Longer call transcripts and higher numbers of questions can increase the cost, however the cost scales very effectively with calls vs. individual calls.
+    The maximum duration of a call to the inbound number, in minutes.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/types/audio_recording_response.py` & `bland-0.3.0/src/bland/calls/types/audio_recording_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.status import Status
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class AudioRecordingResponse(pydantic.BaseModel):
+class AudioRecordingResponse(pydantic_v1.BaseModel):
     status: Status
-    message: typing.Optional[str] = pydantic.Field(default=None)
+    message: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     If the status is `success`, the `url` field will be present instead of this field.
     
     A 404 error will be returned if the call does not exist or the recording is not available. We can only retrieve recordings if the call was created with `record` set to `true`.
     
     A 400/500 error will be returned if there is an error retrieving the recording.
     """
 
-    url: typing.Optional[str] = pydantic.Field(default=None)
+    url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     If the status is `success`, the `url` will provide the exact location of the MP3 file storing the call's audio.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -35,8 +31,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/types/call_details_response.py` & `bland-0.3.0/src/bland/calls/types/call_details_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,62 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .answered_by_enum import AnsweredByEnum
 from .transcript import Transcript
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CallDetailsResponse(pydantic.BaseModel):
-    transcripts: typing.List[Transcript] = pydantic.Field()
+class CallDetailsResponse(pydantic_v1.BaseModel):
+    transcripts: typing.List[Transcript] = pydantic_v1.Field()
     """
     An array of phrases spoken during the call.
     """
 
-    variables: typing.Dict[str, str] = pydantic.Field()
+    variables: typing.Dict[str, str] = pydantic_v1.Field()
     """
     Variables created during the call - both system variables as well as generated with `dynamic_data`.
     
     For example, if you used a `dynamic_data` API request to generate a variable called `appointment_time`, you would see it here.
     """
 
-    concatenated_transcript: str = pydantic.Field()
+    concatenated_transcript: str = pydantic_v1.Field()
     """
     A single string containing all of the text from the call. Excludes system messages and auto-generated data.
     """
 
-    to: str = pydantic.Field()
+    to: str = pydantic_v1.Field()
     """
     The phone number that received the call.
     """
 
-    from_: str = pydantic.Field(alias="from")
+    from_: str = pydantic_v1.Field(alias="from")
     """
     The phone number that made the call.
     """
 
-    batch_id: str = pydantic.Field()
+    batch_id: str = pydantic_v1.Field()
     """
     If the call is part of a batch, it's batch_id will be here.
     """
 
-    request_data: typing.Dict[str, str] = pydantic.Field()
+    request_data: typing.Dict[str, str] = pydantic_v1.Field()
     """
     Details about parameters in the original api request.
     """
 
-    completed: bool = pydantic.Field()
+    completed: bool = pydantic_v1.Field()
     """
     Whether the call has been completed. If it differs from the value of `queue_status`, this will be the most up-to-date status.
     """
 
-    queue_status: str = pydantic.Field()
+    queue_status: str = pydantic_v1.Field()
     """
     The status of the call. During extremely high volume periods, calls may be queued for a short period of time before being dispatched.
     
     Progresses through the following stages -
     
     - `new` - An API request has been received.
     - `queued` - Call pararameters have been validated and authentication succeeded.
@@ -74,51 +70,51 @@
     - `queue_error` - Error occurred while the call was queued. Ex. Valid phone number but to an unserviced area.
     - `call_error` - Error occurred during live call. May be caused by transferring to an invalid phone number or an unforeseen error.
     - `complete_error` - Error occurred after the call was completed. Ex. A post-call webhook failed.
     
     If at any point an error occurs, it will be recorded in the `error_message` field.
     """
 
-    error_message: str = pydantic.Field()
+    error_message: str = pydantic_v1.Field()
     """
     If an error occurs, this will contain a description of the error. Otherwise, it will be null.
     """
 
-    answered_by: AnsweredByEnum = pydantic.Field()
+    answered_by: AnsweredByEnum = pydantic_v1.Field()
     """
     If `answered_by_enabled` was set to `true` in the original API request, this field contains one of the following values:
     
     - `human`: The call was answered by a human.
     - `voicemail`: The call was answered by an answering machine or voicemail.
     - `unknown`: There was not enough audio at the start of the call to make a determination.
     - `no-answer`: The call was not answered.
     - `null`: Not enabled, or still processing the result.
     """
 
-    endpoint_url: str = pydantic.Field()
+    endpoint_url: str = pydantic_v1.Field()
     """
     The URL that was called to dispatch the phone call.
     """
 
-    max_duration: float = pydantic.Field()
+    max_duration: float = pydantic_v1.Field()
     """
     The maximum length of time the call was allowed to last. If the call would exceed this length, it's ended early.
     """
 
-    corrected_duration: float = pydantic.Field()
+    corrected_duration: float = pydantic_v1.Field()
     """
     The total length of time the call was connected. This differs from `call_length` in that it includes ringing and connection time.
     """
 
-    call_length: float = pydantic.Field()
+    call_length: float = pydantic_v1.Field()
     """
     The length of the call in minutes.
     """
 
-    created_at: dt.datetime = pydantic.Field()
+    created_at: dt.datetime = pydantic_v1.Field()
     """
     The timestamp for when the call was dispatched.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -127,8 +123,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/types/list_calls_response.py` & `bland-0.3.0/src/bland/outbound_numbers/types/outbound_purchase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .listed_call_data import ListedCallData
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListCallsResponse(pydantic.BaseModel):
-    count: int = pydantic.Field()
+class OutboundPurchase(pydantic_v1.BaseModel):
+    area_code: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The total number of calls returned in the response.
+    Choose a three-digit area code for your phone number. If set as a parameter, a number will only be purchased by exact match if available.
+    
+    If no area code is set, the default `415` area code will be used.
     """
 
-    calls: typing.List[ListedCallData]
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/types/listed_call_data.py` & `bland-0.3.0/src/bland/outbound_numbers/types/outbound_number.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ListedCallData(pydantic.BaseModel):
-    call_id: str
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    call_length: float
-    to: str
-    from_: str = pydantic.Field(alias="from")
-    completed: bool
-    queue_status: str
-    error_message: typing.Optional[str] = None
-    answered_by: str
-    batch_id: typing.Optional[str] = None
+
+class OutboundNumber(pydantic_v1.BaseModel):
+    created_at: dt.datetime
+    phone_number: PhoneNumber
+    last_initiated: dt.datetime
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/calls/types/stop_call_response.py` & `bland-0.3.0/src/bland/web_agents/types/create_web_agent_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.status import Status
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class StopCallResponse(pydantic.BaseModel):
-    status: Status = pydantic.Field()
+class CreateWebAgentResponse(pydantic_v1.BaseModel):
+    status: str = pydantic_v1.Field()
     """
-    Can be `success` or `error`.
+    Can be success or error.
     """
 
-    message: str = pydantic.Field()
+    call_id: str = pydantic_v1.Field()
     """
-    If the status is `success`, the message will say “Call ended successfully.” Otherwise, if the status is `error`, the message will say “SID not found for the given c_id.” or “Internal server error.”
+    A unique identifier for the call (present only if status is success).
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bland-0.2.2/src/blandai/calls/types/transcript.py` & `bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
-from .user_enum import UserEnum
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Transcript(pydantic.BaseModel):
-    id: str
-    created_at: dt.datetime
-    text: str
-    user: UserEnum
-    c_id: str = pydantic.Field()
-    """
-    The unique identifier for the call.
-    """
+
+class InboundNumberResponse(pydantic_v1.BaseModel):
+    phone_number: PhoneNumber
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/commons/types/custom_tool.py` & `bland-0.3.0/src/bland/commons/types/custom_tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CustomTool(pydantic.BaseModel):
-    name: str = pydantic.Field()
+class CustomTool(pydantic_v1.BaseModel):
+    name: str = pydantic_v1.Field()
     """
     The name of the tool.
     """
 
-    description: str = pydantic.Field()
+    description: str = pydantic_v1.Field()
     """
     A short explanation of what the tool does.
     """
 
-    input_schema: typing.Any = pydantic.Field()
+    input_schema: typing.Any = pydantic_v1.Field()
     """
     A JSON schema describing the input data.
     """
 
-    speech: typing.Optional[str] = pydantic.Field(default=None)
+    speech: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A string that will be spoken to the agent while your tool waits for a response.
     """
 
-    response_data: typing.List[typing.Any] = pydantic.Field()
+    response_data: typing.List[typing.Any] = pydantic_v1.Field()
     """
     An array of objects that describe how to extract data from the response. Within the response data, you can create variables that the phone agent can reference in its prompt.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -44,8 +40,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/commons/types/error_body.py` & `bland-0.3.0/src/bland/outbound_numbers/types/outbound_purchase_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ErrorBody(pydantic.BaseModel):
-    status: str
-    message: str
+class OutboundPurchaseResponse(pydantic_v1.BaseModel):
+    phone_number: PhoneNumber
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/commons/types/error_detail.py` & `bland-0.3.0/src/bland/inbound_numbers/types/list_inbound_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .inbound_number import InboundNumber
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ErrorDetail(pydantic.BaseModel):
-    value: str
-    msg: str
-    param: str
-    location: str
+class ListInboundResponse(pydantic_v1.BaseModel):
+    response: typing.List[InboundNumber] = pydantic_v1.Field()
+    """
+    An array of objects, each representing an inbound phone number and its configuration.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/core/__init__.py` & `bland-0.3.0/src/bland/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
+from .pydantic_utilities import pydantic_v1
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
     "AsyncHttpClient",
     "BaseClientWrapper",
     "File",
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
     "convert_file_dict_to_httpx_tuples",
     "jsonable_encoder",
+    "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `bland-0.2.2/src/blandai/core/client_wrapper.py` & `bland-0.3.0/src/bland/core/client_wrapper.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,34 +4,42 @@
 
 import httpx
 
 from .http_client import AsyncHttpClient, HttpClient
 
 
 class BaseClientWrapper:
-    def __init__(self, *, api_key: str, base_url: str):
+    def __init__(self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None):
         self.api_key = api_key
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "bland",
-            "X-Fern-SDK-Version": "0.2.2",
+            "X-Fern-SDK-Version": "0.3.0",
         }
         headers["authorization"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.Client):
-        super().__init__(api_key=api_key, base_url=base_url)
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.Client
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
         self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.AsyncClient):
-        super().__init__(api_key=api_key, base_url=base_url)
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.AsyncClient
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
         self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `bland-0.2.2/src/blandai/core/datetime_utils.py` & `bland-0.3.0/src/bland/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/core/file.py` & `bland-0.3.0/src/bland/core/file.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/core/http_client.py` & `bland-0.3.0/src/bland/core/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import asyncio
 import email.utils
 import re
 import time
 import typing
+from contextlib import asynccontextmanager, contextmanager
 from functools import wraps
 from random import random
 
 import httpx
 
 INITIAL_RETRY_DELAY_SECONDS = 0.5
 MAX_RETRY_DELAY_SECONDS = 10
@@ -94,16 +95,18 @@
         if _should_retry(response=response):
             if max_retries > retries:
                 time.sleep(_retry_timeout(response=response, retries=retries))
                 return self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
     @wraps(httpx.Client.stream)
+    @contextmanager
     def stream(self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
 
 
 class AsyncHttpClient:
     def __init__(self, *, httpx_client: httpx.AsyncClient):
         self.httpx_client = httpx_client
 
     # Ensure that the signature of the `request` method is the same as the `httpx.Client.request` method
@@ -114,12 +117,14 @@
         response = await self.httpx_client.request(*args, **kwargs)
         if _should_retry(response=response):
             if max_retries > retries:
                 await asyncio.sleep(_retry_timeout(response=response, retries=retries))
                 return await self.request(max_retries=max_retries, retries=retries + 1, *args, **kwargs)
         return response
 
-    @wraps(httpx.AsyncClient.request)
+    @wraps(httpx.AsyncClient.stream)
+    @asynccontextmanager
     async def stream(
         self, *args: typing.Any, max_retries: int = 0, retries: int = 0, **kwargs: typing.Any
     ) -> typing.Any:
-        return self.httpx_client.stream(*args, **kwargs)
+        async with self.httpx_client.stream(*args, **kwargs) as stream:
+            yield stream
```

### Comparing `bland-0.2.2/src/blandai/core/jsonable_encoder.py` & `bland-0.3.0/src/bland/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `bland-0.2.2/src/blandai/core/request_options.py` & `bland-0.3.0/src/bland/core/request_options.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/__init__.py` & `bland-0.3.0/src/bland/inbound_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/client.py` & `bland-0.3.0/src/bland/outbound_numbers/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,417 +3,280 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..commons.errors.server_error import ServerError
 from ..commons.errors.unauthorized_error import UnauthorizedError
 from ..commons.types.error_body import ErrorBody
-from ..commons.types.phone_number import PhoneNumber
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.pydantic_utilities import pydantic_v1
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
-from .types.inbound_number_details_response import InboundNumberDetailsResponse
-from .types.inbound_number_request import InboundNumberRequest
-from .types.inbound_number_response import InboundNumberResponse
-from .types.list_inbound_response import ListInboundResponse
-from .types.update_inbound import UpdateInbound
-from .types.update_inbound_response import UpdateInboundResponse
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from .types.list_outbound_response import ListOutboundResponse
+from .types.outbound_purchase_response import OutboundPurchaseResponse
 
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
-class InboundNumbersClient:
+class OutboundNumbersClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def purchase(
-        self, *, request: InboundNumberRequest, request_options: typing.Optional[RequestOptions] = None
-    ) -> InboundNumberResponse:
+        self, *, area_code: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
+    ) -> OutboundPurchaseResponse:
         """
-        Purchase and configure a new inbound phone number. ($15/mo. subscription using your stored payment method).
+        Purchase and configure a new outbound phone number. ($15/mo. subscription using your stored payment method).
 
-        Parameters:
-            - request: InboundNumberRequest.
+        Parameters
+        ----------
+        area_code : typing.Optional[str]
+            Choose a three-digit area code for your phone number. If set as a parameter, a number will only be purchased by exact match if available.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/inbound/purchase"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InboundNumberResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            If no area code is set, the default `415` area code will be used.
 
-    def update(
-        self,
-        phone_number: PhoneNumber,
-        *,
-        request: UpdateInbound,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UpdateInboundResponse:
-        """
-        Update your inbound agent's settings, prompt and other details.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - phone_number: PhoneNumber.
+        Returns
+        -------
+        OutboundPurchaseResponse
 
-            - request: UpdateInbound.
+        Examples
+        --------
+        from bland.client import BlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.outbound_numbers.purchase(
+            area_code="string",
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if area_code is not OMIT:
+            _request["area_code"] = area_code
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/inbound/{jsonable_encoder(phone_number)}"
-            ),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/outbound/purchase"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UpdateInboundResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(OutboundPurchaseResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListInboundResponse:
+    def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListOutboundResponse:
         """
-        Retrieves a list of all inbound phone numbers configured for your account, along with their associated settings.
+        Retrieves a list of all outbound phone numbers configured for your account, along with their associated settings.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/inbound"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListInboundResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-    def details(
-        self, phone_number: PhoneNumber, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> InboundNumberDetailsResponse:
-        """
-        Retrieve settings for your inbound phone number.
+        Returns
+        -------
+        ListOutboundResponse
 
-        Parameters:
-            - phone_number: PhoneNumber.
+        Examples
+        --------
+        from bland.client import BlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = BlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        client.outbound_numbers.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/inbound/{jsonable_encoder(phone_number)}"
-            ),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/outbound"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InboundNumberDetailsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListOutboundResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
-class AsyncInboundNumbersClient:
+class AsyncOutboundNumbersClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def purchase(
-        self, *, request: InboundNumberRequest, request_options: typing.Optional[RequestOptions] = None
-    ) -> InboundNumberResponse:
+        self, *, area_code: typing.Optional[str] = OMIT, request_options: typing.Optional[RequestOptions] = None
+    ) -> OutboundPurchaseResponse:
         """
-        Purchase and configure a new inbound phone number. ($15/mo. subscription using your stored payment method).
+        Purchase and configure a new outbound phone number. ($15/mo. subscription using your stored payment method).
 
-        Parameters:
-            - request: InboundNumberRequest.
+        Parameters
+        ----------
+        area_code : typing.Optional[str]
+            Choose a three-digit area code for your phone number. If set as a parameter, a number will only be purchased by exact match if available.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/inbound/purchase"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            json=jsonable_encoder(request)
-            if request_options is None or request_options.get("additional_body_parameters") is None
-            else {
-                **jsonable_encoder(request),
-                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
-            },
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InboundNumberResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+            If no area code is set, the default `415` area code will be used.
 
-    async def update(
-        self,
-        phone_number: PhoneNumber,
-        *,
-        request: UpdateInbound,
-        request_options: typing.Optional[RequestOptions] = None,
-    ) -> UpdateInboundResponse:
-        """
-        Update your inbound agent's settings, prompt and other details.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-        Parameters:
-            - phone_number: PhoneNumber.
+        Returns
+        -------
+        OutboundPurchaseResponse
 
-            - request: UpdateInbound.
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.outbound_numbers.purchase(
+            area_code="string",
+        )
         """
+        _request: typing.Dict[str, typing.Any] = {}
+        if area_code is not OMIT:
+            _request["area_code"] = area_code
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/inbound/{jsonable_encoder(phone_number)}"
-            ),
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/outbound/purchase"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            json=jsonable_encoder(request)
+            json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
-                **jsonable_encoder(request),
+                **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(UpdateInboundResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(OutboundPurchaseResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListInboundResponse:
+    async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListOutboundResponse:
         """
-        Retrieves a list of all inbound phone numbers configured for your account, along with their associated settings.
+        Retrieves a list of all outbound phone numbers configured for your account, along with their associated settings.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        """
-        _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/inbound"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
-            ),
-            headers=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        **self._client_wrapper.get_headers(),
-                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
-                    }
-                )
-            ),
-            timeout=request_options.get("timeout_in_seconds")
-            if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
-            retries=0,
-            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
-        )
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ListInboundResponse, _response.json())  # type: ignore
-        if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        raise ApiError(status_code=_response.status_code, body=_response_json)
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-    async def details(
-        self, phone_number: PhoneNumber, *, request_options: typing.Optional[RequestOptions] = None
-    ) -> InboundNumberDetailsResponse:
-        """
-        Retrieve settings for your inbound phone number.
+        Returns
+        -------
+        ListOutboundResponse
 
-        Parameters:
-            - phone_number: PhoneNumber.
+        Examples
+        --------
+        from bland.client import AsyncBlandAI
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
+        client = AsyncBlandAI(
+            api_key="YOUR_API_KEY",
+        )
+        await client.outbound_numbers.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/inbound/{jsonable_encoder(phone_number)}"
-            ),
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "v1/outbound"),
             params=jsonable_encoder(
                 request_options.get("additional_query_parameters") if request_options is not None else None
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
                 )
             ),
             timeout=request_options.get("timeout_in_seconds")
             if request_options is not None and request_options.get("timeout_in_seconds") is not None
-            else 60,
+            else self._client_wrapper.get_timeout(),
             retries=0,
             max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(InboundNumberDetailsResponse, _response.json())  # type: ignore
+            return pydantic_v1.parse_obj_as(ListOutboundResponse, _response.json())  # type: ignore
         if _response.status_code == 500:
-            raise ServerError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise ServerError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
+            raise UnauthorizedError(pydantic_v1.parse_obj_as(ErrorBody, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/__init__.py` & `bland-0.3.0/src/bland/inbound_numbers/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number.py` & `bland-0.3.0/src/bland/inbound_numbers/types/inbound_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,22 +3,18 @@
 import datetime as dt
 import typing
 
 from ...commons.types.phone_number import PhoneNumber
 from ...commons.types.voice_id import VoiceId
 from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InboundNumber(pydantic.BaseModel):
+class InboundNumber(pydantic_v1.BaseModel):
     created_at: str
     phone_number: PhoneNumber
     prompt: str
     webhook: Webhook
     voice_id: VoiceId
     dynamic_data: typing.Optional[typing.List[typing.Any]] = None
     interruption_threshold: typing.Optional[int] = None
@@ -36,8 +32,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_details_response.py` & `bland-0.3.0/src/bland/voices/types/retrieved_voice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,73 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
-from ...commons.types.voice_id import VoiceId
-from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class RetrievedVoice(pydantic_v1.BaseModel):
+    voice_preset_id: str = pydantic_v1.Field()
+    """
+    The unique identifier for the voice preset.
+    """
+
+    voice_name: str = pydantic_v1.Field()
+    """
+    Public voice name.
+    """
+
+    description: str = pydantic_v1.Field()
+    """
+    The description of the voice preset.
+    """
+
+    reduce_latency: bool = pydantic_v1.Field()
+    """
+    Whether or not the voice preset is optimized for low latency.
+    """
+
+    interruption_threshold: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    The threshold for the voice preset to be interrupted by a new message.
+    """
 
-class InboundNumberDetailsResponse(pydantic.BaseModel):
-    created_at: str = pydantic.Field()
+    language: str = pydantic_v1.Field()
     """
-    The timestamp when the inbound number was configured.
+    The language code of the voice preset.
     """
 
-    phone_number: PhoneNumber = pydantic.Field()
+    voice_settings: typing.Any = pydantic_v1.Field()
     """
-    The specific inbound phone number.
+    The voice settings of the voice preset.
     """
 
-    prompt: str = pydantic.Field()
+    editable: bool = pydantic_v1.Field()
     """
-    The prompt your agent is using.
+    Whether or not your account can edit the preset.
     """
 
-    webhook: Webhook
-    voice_id: VoiceId
-    dynamic_data: typing.Optional[str] = pydantic.Field(default=None)
+    public: bool = pydantic_v1.Field()
     """
-    Any dynamic data associated with the inbound number, if applicable.
+    Whether or not the preset is publicly available.
     """
 
-    max_duration: int = pydantic.Field()
+    created_at: dt.datetime = pydantic_v1.Field()
     """
-    The maximum duration of a call to the inbound number, in minutes.
+    The date and time the preset was originally created.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_request.py` & `bland-0.3.0/src/bland/inbound_numbers/types/inbound_number_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,36 +2,32 @@
 
 import datetime as dt
 import typing
 
 from ...commons.types.phone_number import PhoneNumber
 from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .country_code import CountryCode
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InboundNumberRequest(pydantic.BaseModel):
-    area_code: typing.Optional[str] = pydantic.Field(default=None)
+class InboundNumberRequest(pydantic_v1.BaseModel):
+    area_code: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Choose a three-digit area code for your phone number. If set as a parameter, a number will only be purchased by exact match if available.
     
     If not provided, the default value `415` will be used.
     """
 
-    prompt: typing.Optional[str] = pydantic.Field(default=None)
+    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     This defines how the AI will start the conversation, information available to it, and its behaviors. Matches how the outbound `task` parameter functions.
     """
 
-    country_code: typing.Optional[CountryCode] = pydantic.Field(default=None)
+    country_code: typing.Optional[CountryCode] = pydantic_v1.Field(default=None)
     """
     Choose a country code for your phone number.
     
     If not provided, the default value `US` will be used.
     """
 
     webhook: typing.Optional[Webhook] = None
@@ -44,8 +40,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/inbound_number_response.py` & `bland-0.3.0/src/bland/voices/types/generate_voice_sample_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class InboundNumberResponse(pydantic.BaseModel):
-    phone_number: PhoneNumber
+class GenerateVoiceSampleResponse(pydantic_v1.BaseModel):
+    sample: typing.Any = pydantic_v1.Field()
+    """
+    The generated audio file of the spoken text using the specified or overridden voice preset settings.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/list_inbound_response.py` & `bland-0.3.0/src/bland/sms/types/update_prompt_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
-from .inbound_number import InboundNumber
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class UpdatePromptRequest(pydantic_v1.BaseModel):
+    phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
+    """
+    The phone number to update.
+    """
 
-class ListInboundResponse(pydantic.BaseModel):
-    response: typing.List[InboundNumber] = pydantic.Field()
+    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    An array of objects, each representing an inbound phone number and its configuration.
+    The prompt for the AI to use when replying.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/update_inbound.py` & `bland-0.3.0/src/bland/inbound_numbers/types/update_inbound.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,40 +4,38 @@
 import typing
 
 from ...commons.types.phone_number import PhoneNumber
 from ...commons.types.tools import Tools
 from ...commons.types.voice_id import VoiceId
 from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .model import Model
 from .voice_settings import VoiceSettings
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UpdateInbound(pydantic.BaseModel):
+class UpdateInbound(pydantic_v1.BaseModel):
     """
-    from blandai import UpdateInbound
+    Examples
+    --------
+    from bland import UpdateInbound
 
     UpdateInbound(
         prompt="29382721828",
         transfer_list={
             "default": "+1234567890",
             "sales": "+1234567890",
             "support": "+1234567890",
             "billing": "+1234567890",
         },
         model="enhanced",
     )
     """
 
-    prompt: str = pydantic.Field()
+    prompt: str = pydantic_v1.Field()
     """
     Provide instructions, relevant information, and examples of the ideal conversation flow.
     
     For inbound numbers, consider including additional context about the purpose of the call, and what types of callers to expect.
     
     **Best Practices:**
     
@@ -56,24 +54,24 @@
     - Simple, direct prompts are the most predictable and reliable.
     - Frame instructions positively:
       - `"Do this"` rather than `"Don't do this"`.
       - Ex. `“Keep the conversation casual”` rather than `“Don't be too formal”`.
       - This gives concrete examples of what to do, instead of leaving expected behavior open to interpretation.
     """
 
-    transfer_list: typing.Optional[typing.Dict[str, str]] = pydantic.Field(default=None)
+    transfer_list: typing.Optional[typing.Dict[str, str]] = pydantic_v1.Field(default=None)
     """
     Give your agent the ability to transfer calls to a set of phone numbers.
     
     Overrides `transfer_phone_number` if a `transfer_list.default` is specified.
     
     Will default to `transfer_list.default`, or the chosen phone number.
     """
 
-    model: typing.Optional[Model] = pydantic.Field(default=None)
+    model: typing.Optional[Model] = pydantic_v1.Field(default=None)
     """
     Select a model to use for your call.
     
     If no model is provided, the default value `enhanced` will be used.
     
     In nearly all cases, `enhanced` is the best choice for now.
     
@@ -94,74 +92,74 @@
     
     - `model: turbo`
       - The absolute fastest latency possible, can be verbose at times
       - Limited capabilities currently (excludes Transferring, IVR navigation, Custom Tools)
       - Extremely realistic conversation capabilities
     """
 
-    transfer_phone_number: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
+    transfer_phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
     """
     A phone number that the agent can transfer to under specific conditions - such as being asked to speak to a human or supervisor.
     
     Set to `null` to remove.
     
     Prompting Notes:
     
     - Specify conditions that the agent should transfer to a human under (examples are great!)
     - In the `task`, refer to the action solely as “transfer” or “transferring”.
     - Alternate phrasing such as “swap” or “switch” can mislead the agent, causing the action to be ignored.
     """
 
     voice_id: typing.Optional[VoiceId] = None
     webhook: typing.Optional[Webhook] = None
-    record: typing.Optional[bool] = pydantic.Field(default=None)
+    record: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     To record your phone call, set record to `true`. When your call completes, you can access through the `recording_url` field in the call details or your webhook.
     
     If no value is provided, the default value `false` will be used.
     """
 
-    first_sentence: typing.Optional[str] = pydantic.Field(default=None)
+    first_sentence: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A phrase that your call will start with instead of a generating one on the fly. This works both with and without `wait_for_greeting`. Can be more than one sentence, but must be less than 200 characters.
     
     To remove, set to `null` or an empty string.
     """
 
     tools: Tools
-    voice_settings: typing.Optional[VoiceSettings] = pydantic.Field(default=None)
+    voice_settings: typing.Optional[VoiceSettings] = pydantic_v1.Field(default=None)
     """
     Alter advanced voice settings for your agent.
     
     To remove, set to `null` or an empty string.
     """
 
-    dynamic_data: typing.Optional[str] = pydantic.Field(default=None)
+    dynamic_data: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Integrate data from external APIs into your agent's knowledge.
     
     Set to `null` or an empty string to clear dynamic data settings.
     
     Detailed usage in the Send Call endpoint.
     """
 
-    interruption_threshold: typing.Optional[int] = pydantic.Field(default=None)
+    interruption_threshold: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     How long our AI phone agent should wait in milliseconds before responding.
     
     When you increase the interruption latency, you force the AI phone agent to listen longer before responding. In practice, increasing the threshold results in less interruptions and more latency.
     
     Try setting the threshold to 500 milliseconds. You'll encounter higher latency, but you'll be interrupted less frequently.
     
     Set to `null` to reset to default.
     
     If no value is provided, the default value `50` will be used.
     """
 
-    max_duration: typing.Optional[int] = pydantic.Field(default=None)
+    max_duration: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The maximum duration in minutes that calls to your agent can last before being automatically terminated.
     
     Set to `null` to reset to default.
     
     If no value is provided, the default value `30` will be used.
     """
@@ -173,8 +171,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/update_inbound_response.py` & `bland-0.3.0/src/bland/inbound_numbers/types/update_inbound_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UpdateInboundResponse(pydantic.BaseModel):
-    status: str = pydantic.Field()
+class UpdateInboundResponse(pydantic_v1.BaseModel):
+    status: str = pydantic_v1.Field()
     """
     Whether the update was successful or not - will be `success` or `error`.
     """
 
-    message: str = pydantic.Field()
+    message: str = pydantic_v1.Field()
     """
     A message describing the status of the update.
     """
 
-    updates: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(default=None)
+    updates: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
     An object containing the updated settings for the inbound number.
     """
 
-    failed_updates: typing.Optional[typing.Dict[str, str]] = pydantic.Field(default=None)
+    failed_updates: typing.Optional[typing.Dict[str, str]] = pydantic_v1.Field(default=None)
     """
     If the update was unsuccessful, this will contain the settings that failed to update. Useful to determine how your request is being interpreted on our end.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -39,8 +35,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/inbound_numbers/types/voice_settings.py` & `bland-0.3.0/src/bland/inbound_numbers/types/voice_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceSettings(pydantic.BaseModel):
-    stability: typing.Optional[float] = pydantic.Field(default=None)
+class VoiceSettings(pydantic_v1.BaseModel):
+    stability: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Note: This is an experimental parameter and may behave unexpectedly.
     
     Adjust the predictability and consistency of the AI agent's voice. Lower values allow larger deviations from the baseline voice, whether default or cloned. Setting this too high however can cause a monotone voice.
     
     Accepts decimal values between `0` and `1` (inclusive).
     """
 
-    similarity: typing.Optional[float] = pydantic.Field(default=None)
+    similarity: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Note: This is an experimental parameter and may behave unexpectedly.
     
     Higher values will make speech differences between the selected voice and others more prominent. Extremely high values can cause voice distortion.
     
     Use lower values to lower the distinctiveness of the voice or eliminate unwanted audio static spikes.
     
     Accepts decimal values between `0` and `1` (inclusive).
     """
 
-    speed: typing.Optional[float] = pydantic.Field(default=None)
+    speed: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     Note: This is an experimental parameter and may behave unexpectedly.
     
     Note #2: Setting `reduce_latency` to false will cause this parameter to be ignored.
     
     How fast your agent talks! This parameter is simply a speech-speed multiplier, and works with fractional values such as `0.5` or large ones like `2`.
     
@@ -50,8 +46,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/outbound_numbers/types/list_outbound_response.py` & `bland-0.3.0/src/bland/calls/types/transcript.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .outbound_number import OutboundNumber
+from ...core.pydantic_utilities import pydantic_v1
+from .user_enum import UserEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ListOutboundResponse(pydantic.BaseModel):
-    outbound_numbers: typing.List[OutboundNumber] = pydantic.Field()
+class Transcript(pydantic_v1.BaseModel):
+    id: str
+    created_at: dt.datetime
+    text: str
+    user: UserEnum
+    c_id: str = pydantic_v1.Field()
     """
-    An array of outbound phone number objects.
+    The unique identifier for the call.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/outbound_numbers/types/outbound_number.py` & `bland-0.3.0/src/bland/sms/types/check_status_request.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class OutboundNumber(pydantic.BaseModel):
-    created_at: dt.datetime
-    phone_number: PhoneNumber
-    last_initiated: dt.datetime
+class CheckStatusRequest(pydantic_v1.BaseModel):
+    registration_id: str = pydantic_v1.Field()
+    """
+    The registration_id for the a2p registration.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/outbound_numbers/types/outbound_purchase.py` & `bland-0.3.0/src/bland/sms/types/get_messages_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class GetMessagesRequest(pydantic_v1.BaseModel):
+    phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
+    """
+    The phone number to get messages for.
+    """
+
+    to: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
+    """
+    The to number in the conversation. This is the number you _do not_ own.
+    """
 
-class OutboundPurchase(pydantic.BaseModel):
-    area_code: typing.Optional[str] = pydantic.Field(default=None)
-    """
-    Choose a three-digit area code for your phone number. If set as a parameter, a number will only be purchased by exact match if available.
-    
-    If no area code is set, the default `415` area code will be used.
+    from_: typing.Optional[PhoneNumber] = pydantic_v1.Field(alias="from", default=None)
+    """
+    The from number in the conversation. This is the number you _do_ own.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/outbound_numbers/types/outbound_purchase_response.py` & `bland-0.3.0/src/bland/voices/types/list_voice_options_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .preset import Preset
+from .voice import Voice
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class OutboundPurchaseResponse(pydantic.BaseModel):
-    phone_number: PhoneNumber
+class ListVoiceOptionsResponse(pydantic_v1.BaseModel):
+    voices: typing.List[Voice] = pydantic_v1.Field()
+    """
+    Contains a list of the voices available for your account, including custom and default presets.
+    """
+
+    presets: typing.List[Preset] = pydantic_v1.Field()
+    """
+    Contains a list of presets with their details.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/__init__.py` & `bland-0.3.0/src/bland/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/sms/types/__init__.py` & `bland-0.3.0/src/bland/sms/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/sms/types/check_status_request.py` & `bland-0.3.0/src/bland/voices/types/preset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CheckStatusRequest(pydantic.BaseModel):
-    registration_id: str = pydantic.Field()
-    """
-    The registration_id for the a2p registration.
-    """
+class Preset(pydantic_v1.BaseModel):
+    voice_name: str
+    description: str
+    reduce_latency: bool
+    interruption_threshold: typing.Optional[int] = None
+    language: str
+    voice_settings: typing.Any
+    editable: bool
+    public: bool
+    voice_preset_id: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/check_status_response.py` & `bland-0.3.0/src/bland/sms/types/check_status_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .a_2_p_status_enum import A2PStatusEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CheckStatusResponse(pydantic.BaseModel):
+class CheckStatusResponse(pydantic_v1.BaseModel):
     status: A2PStatusEnum
-    brand_type: str = pydantic.Field(alias="brandType")
+    brand_type: str = pydantic_v1.Field(alias="brandType")
     """
     The brand type of the A2P registration.
     """
 
-    failture_reason: typing.Optional[str] = pydantic.Field(alias="failtureReason", default=None)
+    failture_reason: typing.Optional[str] = pydantic_v1.Field(alias="failtureReason", default=None)
     """
     The reason the A2P registration failed.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -32,8 +28,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/get_messages_request.py` & `bland-0.3.0/src/bland/sms/types/update_webhook_request.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...commons.types.phone_number import PhoneNumber
+from ...commons.types.webhook import Webhook
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetMessagesRequest(pydantic.BaseModel):
-    phone_number: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
-    """
-    The phone number to get messages for.
-    """
-
-    to: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
+class UpdateWebhookRequest(pydantic_v1.BaseModel):
+    phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
     """
-    The to number in the conversation. This is the number you _do not_ own.
+    The phone number to update.
     """
 
-    from_: typing.Optional[PhoneNumber] = pydantic.Field(alias="from", default=None)
+    webhook: typing.Optional[Webhook] = pydantic_v1.Field(default=None)
     """
-    The from number in the conversation. This is the number you _do_ own.
+    The webhook to fire when an SMS is received.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/get_messages_response.py` & `bland-0.3.0/src/bland/sms/types/get_messages_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class GetMessagesResponse(pydantic.BaseModel):
-    messages: typing.List[typing.Any] = pydantic.Field()
+class GetMessagesResponse(pydantic_v1.BaseModel):
+    messages: typing.List[typing.Any] = pydantic_v1.Field()
     """
     A list of messages for the given conversation.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -24,8 +20,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/register_request.py` & `bland-0.3.0/src/bland/sms/types/register_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,88 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .legal_structure_enum import LegalStructureEnum
 from .trusted_user import TrustedUser
 from .vertical_enum import VerticalEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RegisterRequest(pydantic.BaseModel):
-    business_name: str = pydantic.Field(alias="businessName")
+class RegisterRequest(pydantic_v1.BaseModel):
+    business_name: str = pydantic_v1.Field(alias="businessName")
     """
     The legal name of your business.
     """
 
-    ein: str = pydantic.Field()
+    ein: str = pydantic_v1.Field()
     """
     Your Employer Identification Number.
     """
 
-    vertical: VerticalEnum = pydantic.Field()
+    vertical: VerticalEnum = pydantic_v1.Field()
     """
     The industry vertical of your business.
     """
 
-    address: str = pydantic.Field()
+    address: str = pydantic_v1.Field()
     """
     The business address.
     """
 
-    city: str = pydantic.Field()
+    city: str = pydantic_v1.Field()
     """
     The city of your business.
     """
 
-    state: str = pydantic.Field()
+    state: str = pydantic_v1.Field()
     """
     The state of your business. Must be a valid US state code.
     """
 
-    postal_code: str = pydantic.Field(alias="postalCode")
+    postal_code: str = pydantic_v1.Field(alias="postalCode")
     """
     The postal code of your business.
     """
 
-    country: str = pydantic.Field()
+    country: str = pydantic_v1.Field()
     """
     The country of your business.
     """
 
-    email: str = pydantic.Field()
+    email: str = pydantic_v1.Field()
     """
     The email address for your business.
     """
 
-    type: LegalStructureEnum = pydantic.Field()
+    type: LegalStructureEnum = pydantic_v1.Field()
     """
     Legal structure of the business.
     """
 
-    website: str = pydantic.Field()
+    website: str = pydantic_v1.Field()
     """
     Your business's website URL.
     """
 
-    opt_in_info: str = pydantic.Field()
+    opt_in_info: str = pydantic_v1.Field()
     """
     Information regarding opt-in procedures for your messaging service.
     
     EX: “Customers must explicitly consent on our website and during the phone call.”
     """
 
-    message_samples: typing.List[str] = pydantic.Field(alias="messageSamples")
+    message_samples: typing.List[str] = pydantic_v1.Field(alias="messageSamples")
     """
     An array of three strings, each a sample message you plan to use.
     """
 
-    trusted_user: TrustedUser = pydantic.Field()
+    trusted_user: TrustedUser = pydantic_v1.Field()
     """
     An object containing details about the trusted user registering the brand.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -95,8 +91,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/register_response.py` & `bland-0.3.0/src/bland/outbound_numbers/types/list_outbound_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .outbound_number import OutboundNumber
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RegisterResponse(pydantic.BaseModel):
-    message: str
-    data: typing.Dict[str, typing.Any]
+class ListOutboundResponse(pydantic_v1.BaseModel):
+    outbound_numbers: typing.List[OutboundNumber] = pydantic_v1.Field()
+    """
+    An array of outbound phone number objects.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/toggle_reply_request.py` & `bland-0.3.0/src/bland/voices/types/create_voice_preset_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .retrieved_voice import RetrievedVoice
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class ToggleReplyRequest(pydantic.BaseModel):
-    phone_number: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
+class CreateVoicePresetResponse(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
     """
-    The phone number to update.
+    Confirmation message indicating successful creation of the new voice preset.
     """
 
-    on: typing.Optional[bool] = pydantic.Field(default=None)
+    voice: RetrievedVoice = pydantic_v1.Field()
     """
-    Turn human mode on or off.
-    
-    `true` means that the AI will not reply. `false` means the AI will reply.
+    The newly created voice preset.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/toggle_reply_response.py` & `bland-0.3.0/src/bland/types/response_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,50 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from .toggle_reply_enum import ToggleReplyEnum
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class ResponseData(pydantic_v1.BaseModel):
+    """
+    Examples
+    --------
+    from bland import ResponseData
+
+    ResponseData(
+        name="Flight Status",
+        data="user.flights[0].status",
+        context="John's flight is currently Flight Status",
+    )
+    """
+
+    name: str = pydantic_v1.Field()
+    """
+    A label for the fetched data.
+    """
+
+    data: str = pydantic_v1.Field()
+    """
+    The JSON path in the API response to extract the data from.
+    """
 
-class ToggleReplyResponse(pydantic.BaseModel):
-    message: ToggleReplyEnum = pydantic.Field()
+    context: str = pydantic_v1.Field()
     """
-    A message indicating the success of the request.
+    How this data should be incorporated into the AI's knowledge.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/trusted_user.py` & `bland-0.3.0/src/bland/calls/types/listed_call_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TrustedUser(pydantic.BaseModel):
-    position: typing.Optional[str] = None
-    first_name: typing.Optional[str] = None
-    last_name: typing.Optional[str] = None
-    phone_number: typing.Optional[PhoneNumber] = None
-    email: typing.Optional[str] = None
+class ListedCallData(pydantic_v1.BaseModel):
+    call_id: str
+    created_at: dt.datetime = pydantic_v1.Field(alias="createdAt")
+    call_length: float
+    to: str
+    from_: str = pydantic_v1.Field(alias="from")
+    completed: bool
+    queue_status: str
+    error_message: typing.Optional[str] = None
+    answered_by: str
+    batch_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/update_prompt_request.py` & `bland-0.3.0/src/bland/voices/types/generate_voice_sample_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...commons.types.phone_number import PhoneNumber
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .voice_settings_data import VoiceSettingsData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UpdatePromptRequest(pydantic.BaseModel):
-    phone_number: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
+class GenerateVoiceSampleRequest(pydantic_v1.BaseModel):
+    text: str = pydantic_v1.Field()
     """
-    The phone number to update.
+    The text content to be spoken in the voice sample.
+    
+    Character limit: `200` characters.
     """
 
-    prompt: typing.Optional[str] = pydantic.Field(default=None)
+    voice_settings: typing.Optional[VoiceSettingsData] = pydantic_v1.Field(default=None)
     """
-    The prompt for the AI to use when replying.
+    Alternate `voice_settings` can be passed in to override the preset's default settings.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/update_prompt_response.py` & `bland-0.3.0/src/bland/batches/types/retrieve_batch_analysis_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class UpdatePromptResponse(pydantic.BaseModel):
-    status: str
+from ...core.pydantic_utilities import pydantic_v1
+from .batch_analysis_object import BatchAnalysisObject
+from .status_enum import StatusEnum
+
+
+class RetrieveBatchAnalysisResponse(pydantic_v1.BaseModel):
+    status: StatusEnum = pydantic_v1.Field()
+    """
+    Whether the request was successful or not.
+    """
+
+    message: str = pydantic_v1.Field()
+    """
+    An error message or confirmation that the request was successful.
+    """
+
+    analysis: typing.List[BatchAnalysisObject] = pydantic_v1.Field()
+    """
+    An array of analysis objects, each corresponding to a call within the batch.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/sms/types/update_webhook_response.py` & `bland-0.3.0/src/bland/voices/types/publish_voice_preset_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .retrieved_voice import RetrievedVoice
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UpdateWebhookResponse(pydantic.BaseModel):
-    status: str
+class PublishVoicePresetResponse(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
+    """
+    Confirmation message indicating the successful publication of the voice preset.
+    """
+
+    voice: RetrievedVoice = pydantic_v1.Field()
+    """
+    Contains detailed information about the published voice preset.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/types/__init__.py` & `bland-0.3.0/src/bland/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/types/dynamic_data.py` & `bland-0.3.0/src/bland/types/dynamic_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .method_enum import MethodEnum
 from .response_data import ResponseData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class DynamicData(pydantic.BaseModel):
+class DynamicData(pydantic_v1.BaseModel):
     """
-    from blandai import DynamicData, ResponseData
+    Examples
+    --------
+    from bland import DynamicData, ResponseData
 
     DynamicData(
         url="https://api.coindesk.com/v1/bpi/currentprice.json",
         response_data=[
             ResponseData(
                 name="BTC Price USD",
                 data="bpi.USD.rate",
@@ -30,40 +28,40 @@
                 data="bpi.EUR.rate",
                 context="In Euros: BTC Price USD EUR",
             ),
         ],
     )
     """
 
-    url: str = pydantic.Field()
+    url: str = pydantic_v1.Field()
     """
     The URL of the external API to fetch data from.
     """
 
-    response_data: typing.List[ResponseData] = pydantic.Field()
+    response_data: typing.List[ResponseData] = pydantic_v1.Field()
     """
     An array of objects describing how to parse and use the data fetched from the API.
     """
 
-    method: typing.Optional[MethodEnum] = pydantic.Field(default=None)
+    method: typing.Optional[MethodEnum] = pydantic_v1.Field(default=None)
     """
     Default value is `GET`.
     """
 
-    cache: typing.Optional[bool] = pydantic.Field(default=None)
+    cache: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Whether to fetch the data once at the beginning of the call, or to re-check continuously for data that might change mid-call. Default value is `true`.
     """
 
-    headers: typing.Optional[typing.Dict[str, str]] = pydantic.Field(default=None)
+    headers: typing.Optional[typing.Dict[str, str]] = pydantic_v1.Field(default=None)
     """
     An object of headers to send with the request.
     """
 
-    body: typing.Optional[str] = pydantic.Field(default=None)
+    body: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The body of the request.
     
     The following variables can be injected into the dynamic request body with double curly braces:
     
     - `from` (Ex. `+12223334444`)
     - `to`
@@ -81,8 +79,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/types/pronunciation_object.py` & `bland-0.3.0/src/bland/types/pronunciation_object.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PronunciationObject(pydantic.BaseModel):
-    word: typing.Optional[str] = pydantic.Field(default=None)
+class PronunciationObject(pydantic_v1.BaseModel):
+    word: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The word you want to guide the LLM on how to pronounce
     """
 
-    pronunciation: typing.Optional[str] = pydantic.Field(default=None)
+    pronunciation: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The word you want to guide the LLM on how to pronounce.
     """
 
-    case_insensitive: typing.Optional[bool] = pydantic.Field(default=None)
+    case_insensitive: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Whether or not to consider case. Particularly useful with names. EG - 'Max' the name versus 'max' the word. Defaults to false. `Not required`.
     """
 
-    spaced: typing.Optional[bool] = pydantic.Field(default=None)
+    spaced: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     whether or not to consider spaces. When `true`, the word 'high' would be flagged but NOT 'hightop'. Defaults to true. `Not required`.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -39,8 +35,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/types/response_data.py` & `bland-0.3.0/src/bland/voices/types/voice_settings_data.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .optimize_for import OptimizeFor
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class VoiceSettingsData(pydantic_v1.BaseModel):
+    speed: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Multiplies the speed of the voice (only `reduce_latency: true` voices).
+    """
 
-class ResponseData(pydantic.BaseModel):
+    interruption_threshold: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Delay before responding (in milliseconds).
     """
-    from blandai import ResponseData
 
-    ResponseData(
-        name="Flight Status",
-        data="user.flights[0].status",
-        context="John's flight is currently Flight Status",
-    )
+    stability: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Lower for more emotion, higher for more stability.
     """
 
-    name: str = pydantic.Field()
+    similarity: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    A label for the fetched data.
+    Match cloned voice more closely.
     """
 
-    data: str = pydantic.Field()
+    speech_flexibility: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    The JSON path in the API response to extract the data from.
+    Flexible pronunciation.
     """
 
-    context: str = pydantic.Field()
+    optimize_for: typing.Optional[OptimizeFor] = pydantic_v1.Field(default=None)
     """
-    How this data should be incorporated into the AI's knowledge.
+    The optimization setting for the voice.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/types/send_call.py` & `bland-0.3.0/src/bland/types/send_call.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,29 @@
 import typing
 
 from ..commons.types.phone_number import PhoneNumber
 from ..commons.types.tools import Tools
 from ..commons.types.voice_id import VoiceId
 from ..commons.types.webhook import Webhook
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 from .dynamic_data import DynamicData
 from .interruption_threshold import InterruptionThreshold
 from .model_enum import ModelEnum
 from .prounciation_guide import ProunciationGuide
 from .temperature import Temperature
 from .transfer_list import TransferList
 from .voicemail_action import VoicemailAction
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SendCall(pydantic.BaseModel):
+class SendCall(pydantic_v1.BaseModel):
     """
-    from blandai import PronunciationObject, SendCall
+    Examples
+    --------
+    from bland import PronunciationObject, SendCall
 
     SendCall(
         phone_number="29382721828",
         task="Would love for you to check out our AI API!",
         temperature=0.5,
         transfer_list={
             "default": "+1234567890",
@@ -46,187 +44,187 @@
                 word="AI",
                 pronunciation="A I",
             ),
         ],
     )
     """
 
-    phone_number: PhoneNumber = pydantic.Field()
+    phone_number: PhoneNumber = pydantic_v1.Field()
     """
     The phone number to call. Country code defaults to `+1` (US) if not specified.
     
     Formatting is flexible, however for the most predictable results use the **[E.164](https://www.twilio.com/docs/glossary/what-e164#examples-of-e164-numbers)** format.
     """
 
-    task: str = pydantic.Field()
+    task: str = pydantic_v1.Field()
     """
     Provide instructions, relevant information, and examples of the ideal conversation flow.
     """
 
-    transfer_list: typing.Optional[TransferList] = pydantic.Field(default=None)
+    transfer_list: typing.Optional[TransferList] = pydantic_v1.Field(default=None)
     """
     Give your agent the ability to transfer calls to a set of phone numbers.
     
     Overrides `transfer_phone_number` if a `transfer_list.default` is specified.
     
     Will default to `transfer_list.default`, or the chosen phone number.
     """
 
-    model: typing.Optional[ModelEnum] = pydantic.Field(default=None)
+    model: typing.Optional[ModelEnum] = pydantic_v1.Field(default=None)
     """
     Select a model to use for your call.
     
     In nearly all cases, `enhanced` is the best choice for now.
     """
 
-    pronunciation_guide: typing.Optional[ProunciationGuide] = pydantic.Field(default=None)
+    pronunciation_guide: typing.Optional[ProunciationGuide] = pydantic_v1.Field(default=None)
     """
     The pronunciation guide is an `array` of `objects` that guides the LLM on how to say specific words. This is great for situations with complicated terms or names.
     """
 
-    temperature: Temperature = pydantic.Field()
+    temperature: Temperature = pydantic_v1.Field()
     """
     A value between 0 and 1 that controls the randomness of the LLM. 0 will cause more deterministic outputs while 1 will cause more random.
     """
 
     tools: Tools
-    transfer_phone_number: typing.Optional[PhoneNumber] = pydantic.Field(default=None)
+    transfer_phone_number: typing.Optional[PhoneNumber] = pydantic_v1.Field(default=None)
     """
     A phone number that the agent can transfer to under specific conditions - such as being asked to speak to a human or supervisor.
     """
 
-    answered_by_enabled: typing.Optional[bool] = pydantic.Field(default=None)
+    answered_by_enabled: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Enables machine detection when the call starts to determine whether the call was answered by a person or a voicemail.
     
     Best Practices (when enabled) -
     
         - Since the determination is made at the beginning of the call, use `wait_for_greeting` to try and coax a human response.
     
         - If combined with first_sentence, try wording it so the person answering says something back - ex. `"Hello?"`
     
     Price - `$0.02` per call, however there is no charge for unanswered calls or calls that failed to send.
     """
 
-    from_: typing.Optional[str] = pydantic.Field(alias="from", default=None)
+    from_: typing.Optional[str] = pydantic_v1.Field(alias="from", default=None)
     """
     Specify a purchased Outbound Number to call from. Country code is required, spaces or parentheses must be excluded.
     
     By default, calls are initiated from a separate pool of numbers owned by Bland.
     """
 
-    reduce_latency: typing.Optional[bool] = pydantic.Field(default=None)
+    reduce_latency: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Reducing latency means that the agent will generate responses more quickly and have less of a delay. This must be set to `true` when using Voice Clones.
     """
 
-    voice_id: typing.Optional[VoiceId] = pydantic.Field(default=None)
+    voice_id: typing.Optional[VoiceId] = pydantic_v1.Field(default=None)
     """
     Determines the voice of the AI agent, in conjunction with `reduce_latency`.
     
     Use the `GET /v1/voices endpoint` to see a full list of your available voices.
     
     To create your own Voice Clone, visit our [Custom Voice Cloning page](https://app.bland.ai/home?page=voice-clone).
     """
 
-    voice_preset_id: typing.Optional[str] = pydantic.Field(default=None)
+    voice_preset_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Use a voice preset instead of specifying individual voice settings.
     
     To create a voice preset, see [Create a Voice Preset](https://docs.bland.ai/api-v1/post/voices).
     """
 
-    start_time: typing.Optional[str] = pydantic.Field(default=None)
+    start_time: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The time you want the call to start. If you don't specify a time (or the time is in the past), the call will send immediately.
     
     Set your time in the format `YYYY-MM-DD HH:MM:SS -HH:MM` (ex. `2021-01-01 12:00:00 -05:00`).
     
     The timezone is optional, and defaults to `UTC` if not specified.
     
     Note - Scheduled calls can be cancelled with the `POST /v1/calls/:call_id/stop` endpoint.
     """
 
-    webhook: typing.Optional[Webhook] = pydantic.Field(default=None)
+    webhook: typing.Optional[Webhook] = pydantic_v1.Field(default=None)
     """
     The webhook should be a http / https callback url. We will send the call_id and transcript to this URL after the call completes. This can be useful if you want to have real time notifications when calls finish.
     """
 
-    wait_for_greeting: typing.Optional[bool] = pydantic.Field(default=None)
+    wait_for_greeting: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Should the AI speak first or wait for someone else to talk?
     
     Creates more realistic conversations when answered with “Hello?”, “This is {name} speaking.” and so on.
     
         - When `false`, The AI starts speaking shortly after the call is answered.
     
         - When `true`, The AI will wait for the answerer to speak.
     """
 
-    first_sentence: typing.Optional[str] = pydantic.Field(default=None)
+    first_sentence: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A phrase that your call will start with instead of a generating one on the fly. This works both with and without `wait_for_greeting`. Can be more than one sentence, but must be less than 200 characters.
     """
 
-    record: typing.Optional[bool] = pydantic.Field(default=None)
+    record: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     To record your phone call, set `record` to true. When your call completes, you can access through the `recording_url` field in the call details or your webhook.
     """
 
-    voice_settings: typing.Optional[bool] = pydantic.Field(default=None)
+    voice_settings: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     Should the AI speak first or wait for someone else to talk? Creates more realistic conversations when answered with “Hello?”, “This is {name} speaking.” and so on. When `false` - The AI starts speaking shortly after the call is answered. When `true` - The AI will wait for the answerer to speak.
     """
 
-    language: typing.Optional[str] = pydantic.Field(default=None)
+    language: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     Select a supported language of your choice. Optimizes every part of our API for that language - transcription, speech, and other inner workings.
     
     Supported Languages and their codes -
     
     - English - `eng`
     - Spanish - `esp`
     - French - `fre`
     - Polish - `pol`
     """
 
-    max_duration: typing.Optional[int] = pydantic.Field(default=None)
+    max_duration: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Set the longest you want the call to possibly go in minutes. After the max_duration minutes have passed, the call will automatically end. Example Values - `20, 2`
     """
 
-    voicemail_action: typing.Optional[VoicemailAction] = pydantic.Field(default=None)
+    voicemail_action: typing.Optional[VoicemailAction] = pydantic_v1.Field(default=None)
     """
     Voicemail action tells the AI what to do when encountering a voicemail. This has 96% accuracy. There is no such thing as a perfect VM detection, but this gets close.
     
     The default value is hangup to save money and keep most users in compliance.
     
     Note - **Leaving voicemails is strongly discouraged.**
     """
 
-    amd: typing.Optional[bool] = pydantic.Field(default=None)
+    amd: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     AMD mode helps our AI navigate phone trees and IVR systems. If you know your call will hit an automated system you should switch it on.
     
     NOTE - AMD mode causes increased delay for the first response, even if answered by a human. Highly recommended to set to `false` in the majority of cases.
     """
 
-    request_data: typing.Optional[typing.Dict[str, typing.Any]] = pydantic.Field(default=None)
+    request_data: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
     When you want your AI to “know” a specific fact - like the caller's name or other relevant context.
     
     The AI agent will be aware of both the key names as well as their corresponding values.
     """
 
-    dynamic_data: typing.Optional[typing.List[DynamicData]] = pydantic.Field(default=None)
+    dynamic_data: typing.Optional[typing.List[DynamicData]] = pydantic_v1.Field(default=None)
     """
     Make dynamic requests to external APIs and use the data in your AI's responses.
     """
 
-    interruption_threshold: InterruptionThreshold = pydantic.Field()
+    interruption_threshold: InterruptionThreshold = pydantic_v1.Field()
     """
     When you increase the interruption latency, you force the AI phone agent to listen longer before responding. In practice, increasing the threshold results in less interruptions and more latency.
     
     Try setting the threshold to `500` milliseconds. You'll encounter higher latency, but you'll be interrupted much less frequently.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
@@ -237,8 +235,10 @@
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/types/send_call_response.py` & `bland-0.3.0/src/bland/types/send_call_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,50 +2,48 @@
 
 import datetime as dt
 import typing
 
 from ..commons.types.call_id import CallId
 from ..commons.types.status import Status
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class SendCallResponse(pydantic.BaseModel):
+class SendCallResponse(pydantic_v1.BaseModel):
     """
-    from blandai import SendCallResponse
+    Examples
+    --------
+    from bland import SendCallResponse
 
     SendCallResponse(
         status="success",
         message="Call successfully queued.",
         call_id="73c809a9-db35-4edb-8fa6-95a6a942daf8",
     )
     """
 
-    status: Status = pydantic.Field()
+    status: Status = pydantic_v1.Field()
     """
     Can be `success` or `error`.
     """
 
-    call_id: CallId = pydantic.Field()
+    call_id: CallId = pydantic_v1.Field()
     """
     A unique identifier for the call (present only if status is `success`).
     """
 
-    batch_id: typing.Optional[str] = pydantic.Field(default=None)
+    batch_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A unique identifier for the batcarrayh of calls (present only if status is `success`).
     
     If no batch is specified, this value will be `null`.
     """
 
-    message: typing.Optional[str] = pydantic.Field(default=None)
+    message: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A message describing the status of the call (present only if status is `success`).
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -53,8 +51,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/__init__.py` & `bland-0.3.0/src/bland/voices/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/voices/types/__init__.py` & `bland-0.3.0/src/bland/voices/types/__init__.py`

 * *Files identical despite different names*

### Comparing `bland-0.2.2/src/blandai/voices/types/create_voice_preset_request.py` & `bland-0.3.0/src/bland/voices/types/create_voice_preset_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,51 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .voice_settings_data import VoiceSettingsData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CreateVoicePresetRequest(pydantic.BaseModel):
-    voice_name: str = pydantic.Field()
+class CreateVoicePresetRequest(pydantic_v1.BaseModel):
+    voice_name: str = pydantic_v1.Field()
     """
     The name for the new voice preset.
     """
 
-    description: typing.Optional[str] = pydantic.Field(default=None)
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A description of the voice preset.
     """
 
-    voice_id: typing.Optional[int] = pydantic.Field(default=None)
+    voice_id: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The existing `voice_id` that will be mapped to the new voice preset.
     """
 
-    reduce_latency: typing.Optional[bool] = pydantic.Field(default=None)
+    reduce_latency: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     The current `reduce_latency` setting that will be mapped to the new voice preset.
     """
 
-    interruption_threshold: typing.Optional[int] = pydantic.Field(default=None)
+    interruption_threshold: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The threshold for voice interruption settings.
     
     If not provided, the default value is `50`.
     """
 
-    language: typing.Optional[str] = pydantic.Field(default=None)
+    language: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The language code for the voice preset.
     """
 
-    voice_settings: typing.Optional[VoiceSettingsData] = pydantic.Field(default=None)
+    voice_settings: typing.Optional[VoiceSettingsData] = pydantic_v1.Field(default=None)
     """
     A JSON object containing specific settings for the voice.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -57,8 +53,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/create_voice_preset_response.py` & `bland-0.3.0/src/bland/voices/types/voice_updates.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .retrieved_voice import RetrievedVoice
+from ...core.pydantic_utilities import pydantic_v1
+from .voice_settings_data import VoiceSettingsData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CreateVoicePresetResponse(pydantic.BaseModel):
-    message: str = pydantic.Field()
+class VoiceUpdates(pydantic_v1.BaseModel):
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Confirmation message indicating successful creation of the new voice preset.
+    The updated description of the voice preset.
     """
 
-    voice: RetrievedVoice = pydantic.Field()
+    voice_settings: typing.Optional[VoiceSettingsData] = pydantic_v1.Field(default=None)
     """
-    The newly created voice preset.
+    The updated voice settings, including optimization and interruption threshold.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/delete_voice_preset_response.py` & `bland-0.3.0/src/bland/voices/types/voice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class DeleteVoicePresetResponse(pydantic.BaseModel):
-    message: str = pydantic.Field()
-    """
-    Confirmation message indicating successful deletion of the voice preset.
-    """
-
-    voice: str = pydantic.Field()
-    """
-    The ID of the voice preset that was deleted.
-    """
+
+class Voice(pydantic_v1.BaseModel):
+    voice_id: int
+    name: str
+    is_custom: bool
+    reduce_latency: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/generate_voice_sample_response.py` & `bland-0.3.0/src/bland/voices/types/update_voice_preset_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
+from .retrieved_voice import RetrievedVoice
+from .voice_updates import VoiceUpdates
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class UpdateVoicePresetResponse(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
+    """
+    Confirmation message indicating successful update of the voice preset.
+    """
+
+    updates: VoiceUpdates = pydantic_v1.Field()
+    """
+    Contains the details of the updates applied to the voice preset.
+    """
 
-class GenerateVoiceSampleResponse(pydantic.BaseModel):
-    sample: typing.Any = pydantic.Field()
+    voice: RetrievedVoice = pydantic_v1.Field()
     """
-    The generated audio file of the spoken text using the specified or overridden voice preset settings.
+    Contains detailed information about the updated voice preset.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/list_voice_options_response.py` & `bland-0.3.0/src/bland/commons/types/error_body.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,26 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .preset import Preset
-from .voice import Voice
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class ListVoiceOptionsResponse(pydantic.BaseModel):
-    voices: typing.List[Voice] = pydantic.Field()
-    """
-    Contains a list of the voices available for your account, including custom and default presets.
-    """
-
-    presets: typing.List[Preset] = pydantic.Field()
-    """
-    Contains a list of presets with their details.
-    """
+
+class ErrorBody(pydantic_v1.BaseModel):
+    status: str
+    message: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/retrieve_voice_preset_response.py` & `bland-0.3.0/src/bland/sms/types/toggle_reply_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .retrieved_voice import RetrievedVoice
+from ...core.pydantic_utilities import pydantic_v1
+from .toggle_reply_enum import ToggleReplyEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class RetrieveVoicePresetResponse(pydantic.BaseModel):
-    voice: RetrievedVoice = pydantic.Field()
+class ToggleReplyResponse(pydantic_v1.BaseModel):
+    message: ToggleReplyEnum = pydantic_v1.Field()
     """
-    Contains detailed information about the specified voice preset.
+    A message indicating the success of the request.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/update_voice_preset_request.py` & `bland-0.3.0/src/bland/voices/types/update_voice_preset_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 from .voice_settings_data import VoiceSettingsData
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UpdateVoicePresetRequest(pydantic.BaseModel):
-    voice_name: typing.Optional[str] = pydantic.Field(default=None)
+class UpdateVoicePresetRequest(pydantic_v1.BaseModel):
+    voice_name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The name for the new voice preset.
     """
 
-    description: typing.Optional[str] = pydantic.Field(default=None)
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     A description of the voice preset.
     """
 
-    voice_id: typing.Optional[int] = pydantic.Field(default=None)
+    voice_id: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The existing `voice_id` that will be mapped to the new voice preset.
     """
 
-    reduce_latency: typing.Optional[bool] = pydantic.Field(default=None)
+    reduce_latency: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
     The current `reduce_latency` setting that will be mapped to the new voice preset.
     """
 
-    interruption_threshold: typing.Optional[int] = pydantic.Field(default=None)
+    interruption_threshold: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The threshold for voice interruption settings.
     
     If not provided, the default value is `50`.
     
     Reset to default by setting to `null`.
     """
 
-    language: typing.Optional[str] = pydantic.Field(default=None)
+    language: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The language code for the voice preset.
     
     Reset to default by setting to `null`.
     """
 
-    voice_settings: typing.Optional[VoiceSettingsData] = pydantic.Field(default=None)
+    voice_settings: typing.Optional[VoiceSettingsData] = pydantic_v1.Field(default=None)
     """
     A JSON object containing specific settings for the voice.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
@@ -61,8 +57,9 @@
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/update_voice_preset_response.py` & `bland-0.3.0/src/bland/batches/types/call_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,61 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
+from ...calls.types.answered_by_enum import AnsweredByEnum
 from ...core.datetime_utils import serialize_datetime
-from .retrieved_voice import RetrievedVoice
-from .voice_updates import VoiceUpdates
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
+class CallData(pydantic_v1.BaseModel):
+    created_at: dt.datetime = pydantic_v1.Field()
+    """
+    The timestamp when the individual call was created.
+    """
+
+    to: str = pydantic_v1.Field()
+    """
+    The phone number the call was made to.
+    """
+
+    from_: str = pydantic_v1.Field(alias="from")
+    """
+    The phone number the call was made from.
+    """
+
+    completed: bool = pydantic_v1.Field()
+    """
+    Indicates if the call was completed.
+    """
 
-class UpdateVoicePresetResponse(pydantic.BaseModel):
-    message: str = pydantic.Field()
+    call_id: str = pydantic_v1.Field()
     """
-    Confirmation message indicating successful update of the voice preset.
+    The unique identifier for each individual call.
     """
 
-    updates: VoiceUpdates = pydantic.Field()
+    call_length: int = pydantic_v1.Field()
     """
-    Contains the details of the updates applied to the voice preset.
+    The duration of the call in minutes.
     """
 
-    voice: RetrievedVoice = pydantic.Field()
+    answered_by: typing.Optional[AnsweredByEnum] = pydantic_v1.Field(default=None)
     """
-    Contains detailed information about the updated voice preset.
+    Contains a string value if the batch had `answered_by_enabled` set to `true`.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/voice.py` & `bland-0.3.0/src/bland/commons/types/error_detail.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class Voice(pydantic.BaseModel):
-    voice_id: int
-    name: str
-    is_custom: bool
-    reduce_latency: bool
+class ErrorDetail(pydantic_v1.BaseModel):
+    value: str
+    msg: str
+    param: str
+    location: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/src/blandai/voices/types/voice_updates.py` & `bland-0.3.0/src/bland/voices/types/delete_voice_preset_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from .voice_settings_data import VoiceSettingsData
+from ...core.pydantic_utilities import pydantic_v1
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class VoiceUpdates(pydantic.BaseModel):
-    description: typing.Optional[str] = pydantic.Field(default=None)
+class DeleteVoicePresetResponse(pydantic_v1.BaseModel):
+    message: str = pydantic_v1.Field()
     """
-    The updated description of the voice preset.
+    Confirmation message indicating successful deletion of the voice preset.
     """
 
-    voice_settings: typing.Optional[VoiceSettingsData] = pydantic.Field(default=None)
+    voice: str = pydantic_v1.Field()
     """
-    The updated voice settings, including optimization and interruption threshold.
+    The ID of the voice preset that was deleted.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `bland-0.2.2/PKG-INFO` & `bland-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bland
-Version: 0.2.2
+Version: 0.3.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

