# Comparing `tmp/flyflowclient-1.14.3.tar.gz` & `tmp/flyflowclient-1.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "flyflowclient-1.14.4.tar", last modified: Sun May 12 23:53:58 2024, max compression
```

## Comparing `flyflowclient-1.14.3.tar` & `flyflowclient-1.14.4.tar`

### file list

```diff
@@ -1,235 +1,15 @@
--rw-r--r--   0        0        0     9421 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/__main__.py
--rw-r--r--   0        0        0    63372 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_base_client.py
--rw-r--r--   0        0        0    20188 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_compat.py
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_constants.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_exceptions.py
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_files.py
--rw-r--r--   0        0        0    15448 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_legacy_response.py
--rw-r--r--   0        0        0    22078 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_models.py
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_module_client.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_qs.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_resource.py
--rw-r--r--   0        0        0    28605 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_response.py
--rw-r--r--   0        0        0    12106 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_streaming.py
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_types.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_version.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/py.typed
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/version.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_extras/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_extras/_common.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_extras/numpy_proxy.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_extras/pandas_proxy.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_logs.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_typing.py
--rw-r--r--   0        0        0    11105 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/_utils/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/__init__.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_cli.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_models.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_progress.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/_main.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/audio.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/completions.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/files.py
--rw-r--r--   0        0        0     5062 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/image.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/models.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/chat/__init__.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_api/chat/completions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_tools/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_tools/_main.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_tools/fine_tunes.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/cli/_tools/migrate.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/.keep
--rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/_old_api.py
--rw-r--r--   0        0        0    35191 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/_validators.py
--rw-r--r--   0        0        0    21063 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/azure.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/streaming/__init__.py
--rw-r--r--   0        0        0    40467 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/lib/streaming/_assistants.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/__init__.py
--rw-r--r--   0        0        0    57139 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/completions.py
--rw-r--r--   0        0        0    10710 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/embeddings.py
--rw-r--r--   0        0        0    26089 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/files.py
--rw-r--r--   0        0        0    24782 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/images.py
--rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/models.py
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/moderations.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/audio/__init__.py
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/audio/audio.py
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/audio/speech.py
--rw-r--r--   0        0        0    11088 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/audio/translations.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/__init__.py
--rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/beta.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0    30704 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/assistants/assistants.py
--rw-r--r--   0        0        0    19513 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/assistants/files.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/__init__.py
--rw-r--r--   0        0        0    48295 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/threads.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0    12300 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/messages/files.py
--rw-r--r--   0        0        0    22804 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/messages/messages.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0    73259 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/runs/runs.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/beta/threads/runs/steps.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/chat/__init__.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/chat/chat.py
--rw-r--r--   0        0        0    72812 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/chat/completions.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0    24550 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/resources/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/__init__.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/completion.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/completion_choice.py
--rw-r--r--   0        0        0     7329 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/completion_create_params.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/completion_usage.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/create_embedding_response.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/embedding.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/embedding_create_params.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/file_content.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/file_create_params.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/file_deleted.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/file_list_params.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/file_object.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/image.py
--rw-r--r--   0        0        0     1450 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/image_create_variation_params.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/image_edit_params.py
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/image_generate_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/images_response.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/model.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/model_deleted.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/moderation.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/moderation_create_params.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/moderation_create_response.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/__init__.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/speech_create_params.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/transcription.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/translation.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/audio/translation_create_params.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/__init__.py
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant.py
--rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_create_params.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_deleted.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_list_params.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_stream_event.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_tool.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_tool_param.py
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistant_update_params.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/code_interpreter_tool.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/code_interpreter_tool_param.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/function_tool.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/function_tool_param.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/retrieval_tool.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/retrieval_tool_param.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/thread.py
--rw-r--r--   0        0        0     4076 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/thread_create_and_run_params.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/thread_create_params.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/thread_deleted.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/thread_update_params.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistants/__init__.py
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistants/assistant_file.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistants/file_create_params.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistants/file_delete_response.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/assistants/file_list_params.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/chat/__init__.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/annotation.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/annotation_delta.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/file_citation_annotation.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/file_citation_delta_annotation.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/file_path_annotation.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/file_path_delta_annotation.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/image_file.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/image_file_content_block.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/image_file_delta.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/image_file_delta_block.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_content.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_content_delta.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_create_params.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_delta.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_delta_event.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_list_params.py
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/message_update_params.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/required_action_function_tool_call.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run.py
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run_create_params.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run_list_params.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run_status.py
--rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run_submit_tool_outputs_params.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/run_update_params.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/text.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/text_content_block.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/text_delta.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/text_delta_block.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/messages/file_list_params.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/messages/message_file.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/code_interpreter_logs.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/code_interpreter_output_image.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/code_interpreter_tool_call.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/code_interpreter_tool_call_delta.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/function_tool_call.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/function_tool_call_delta.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/message_creation_step_details.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/retrieval_tool_call.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/retrieval_tool_call_delta.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/run_step.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/run_step_delta.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/run_step_delta_event.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/run_step_delta_message_delta.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/step_list_params.py
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/tool_call.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/tool_call_delta.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/tool_call_delta_object.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/beta/threads/runs/tool_calls_step_details.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_assistant_message_param.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_content_part_image_param.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_content_part_param.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_content_part_text_param.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_function_call_option_param.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_function_message_param.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_message.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_message_param.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_message_tool_call.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_message_tool_call_param.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_named_tool_choice_param.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_role.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_system_message_param.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_token_logprob.py
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_tool_choice_option_param.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_tool_message_param.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_tool_param.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/chat_completion_user_message_param.py
--rw-r--r--   0        0        0    10675 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/chat/completion_create_params.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/job_list_events_params.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/fine_tuning/job_list_params.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared/error_object.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared/function_definition.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared/function_parameters.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared_params/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared_params/function_definition.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/src/flyflowclient/types/shared_params/function_parameters.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/LICENSE
--rw-r--r--   0        0        0    17869 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/README.md
--rw-r--r--   0        0        0     3951 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/pyproject.toml
--rw-r--r--   0        0        0    19454 2020-02-02 00:00:00.000000 flyflowclient-1.14.3/PKG-INFO
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.022524 flyflowclient-1.14.4/
+-rw-r--r--   0 carlcortright   (501) staff       (20)    11357 2024-05-12 23:23:34.000000 flyflowclient-1.14.4/LICENSE
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3825 2024-05-12 23:53:58.022318 flyflowclient-1.14.4/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3367 2024-05-12 23:53:44.000000 flyflowclient-1.14.4/README.md
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.021150 flyflowclient-1.14.4/flyflowclient/
+-rw-r--r--   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:29:28.000000 flyflowclient-1.14.4/flyflowclient/__init__.py
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3647 2024-05-12 23:45:58.000000 flyflowclient-1.14.4/flyflowclient/client.py
+drwxr-xr-x   0 carlcortright   (501) staff       (20)        0 2024-05-12 23:53:58.022035 flyflowclient-1.14.4/flyflowclient.egg-info/
+-rw-r--r--   0 carlcortright   (501) staff       (20)     3825 2024-05-12 23:53:57.000000 flyflowclient-1.14.4/flyflowclient.egg-info/PKG-INFO
+-rw-r--r--   0 carlcortright   (501) staff       (20)      260 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/SOURCES.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)        1 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/dependency_links.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       17 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/requires.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       14 2024-05-12 23:53:58.000000 flyflowclient-1.14.4/flyflowclient.egg-info/top_level.txt
+-rw-r--r--   0 carlcortright   (501) staff       (20)       38 2024-05-12 23:53:58.022572 flyflowclient-1.14.4/setup.cfg
+-rw-r--r--   0 carlcortright   (501) staff       (20)      634 2024-05-12 23:53:54.000000 flyflowclient-1.14.4/setup.py
```

### Comparing `flyflowclient-1.14.3/src/flyflowclient/types/chat/completion_create_params.py` & `flyflowclient-1.14.4/LICENSE`

 * *Files 27% similar despite different names*

```diff
@@ -1,280 +1,201 @@
-# File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
-
-from __future__ import annotations
-
-from typing import Dict, List, Union, Iterable, Optional
-from typing_extensions import Literal, Required, TypedDict
-
-from ...types import shared_params
-from .chat_completion_tool_param import ChatCompletionToolParam
-from .chat_completion_message_param import ChatCompletionMessageParam
-from .chat_completion_tool_choice_option_param import ChatCompletionToolChoiceOptionParam
-from .chat_completion_function_call_option_param import ChatCompletionFunctionCallOptionParam
-
-__all__ = [
-    "CompletionCreateParamsBase",
-    "FunctionCall",
-    "Function",
-    "ResponseFormat",
-    "CompletionCreateParamsNonStreaming",
-    "CompletionCreateParamsStreaming",
-]
-
-
-class CompletionCreateParamsBase(TypedDict, total=False):
-    messages: Required[Iterable[ChatCompletionMessageParam]]
-    """A list of messages comprising the conversation so far.
-
-    [Example Python code](https://cookbook.openai.com/examples/how_to_format_inputs_to_chatgpt_models).
-    """
-
-    model: Required[
-        Union[
-            str,
-            Literal[
-                "gpt-4-0125-preview",
-                "gpt-4-turbo-preview",
-                "gpt-4-1106-preview",
-                "gpt-4-vision-preview",
-                "gpt-4",
-                "gpt-4-0314",
-                "gpt-4-0613",
-                "gpt-4-32k",
-                "gpt-4-32k-0314",
-                "gpt-4-32k-0613",
-                "gpt-3.5-turbo",
-                "gpt-3.5-turbo-16k",
-                "gpt-3.5-turbo-0301",
-                "gpt-3.5-turbo-0613",
-                "gpt-3.5-turbo-1106",
-                "gpt-3.5-turbo-0125",
-                "gpt-3.5-turbo-16k-0613",
-            ],
-        ]
-    ]
-    """ID of the model to use.
-
-    See the
-    [model endpoint compatibility](https://platform.openai.com/docs/models/model-endpoint-compatibility)
-    table for details on which models work with the Chat API.
-    """
-
-    frequency_penalty: Optional[float]
-    """Number between -2.0 and 2.0.
-
-    Positive values penalize new tokens based on their existing frequency in the
-    text so far, decreasing the model's likelihood to repeat the same line verbatim.
-
-    [See more information about frequency and presence penalties.](https://platform.openai.com/docs/guides/text-generation/parameter-details)
-    """
-
-    function_call: FunctionCall
-    """Deprecated in favor of `tool_choice`.
-
-    Controls which (if any) function is called by the model. `none` means the model
-    will not call a function and instead generates a message. `auto` means the model
-    can pick between generating a message or calling a function. Specifying a
-    particular function via `{"name": "my_function"}` forces the model to call that
-    function.
-
-    `none` is the default when no functions are present. `auto` is the default if
-    functions are present.
-    """
-
-    functions: Iterable[Function]
-    """Deprecated in favor of `tools`.
-
-    A list of functions the model may generate JSON inputs for.
-    """
-
-    logit_bias: Optional[Dict[str, int]]
-    """Modify the likelihood of specified tokens appearing in the completion.
-
-    Accepts a JSON object that maps tokens (specified by their token ID in the
-    tokenizer) to an associated bias value from -100 to 100. Mathematically, the
-    bias is added to the logits generated by the model prior to sampling. The exact
-    effect will vary per model, but values between -1 and 1 should decrease or
-    increase likelihood of selection; values like -100 or 100 should result in a ban
-    or exclusive selection of the relevant token.
-    """
-
-    logprobs: Optional[bool]
-    """Whether to return log probabilities of the output tokens or not.
-
-    If true, returns the log probabilities of each output token returned in the
-    `content` of `message`. This option is currently not available on the
-    `gpt-4-vision-preview` model.
-    """
-
-    max_tokens: Optional[int]
-    """
-    The maximum number of [tokens](/tokenizer) that can be generated in the chat
-    completion.
-
-    The total length of input tokens and generated tokens is limited by the model's
-    context length.
-    [Example Python code](https://cookbook.openai.com/examples/how_to_count_tokens_with_tiktoken)
-    for counting tokens.
-    """
-
-    n: Optional[int]
-    """How many chat completion choices to generate for each input message.
-
-    Note that you will be charged based on the number of generated tokens across all
-    of the choices. Keep `n` as `1` to minimize costs.
-    """
-
-    presence_penalty: Optional[float]
-    """Number between -2.0 and 2.0.
-
-    Positive values penalize new tokens based on whether they appear in the text so
-    far, increasing the model's likelihood to talk about new topics.
-
-    [See more information about frequency and presence penalties.](https://platform.openai.com/docs/guides/text-generation/parameter-details)
-    """
-
-    response_format: ResponseFormat
-    """An object specifying the format that the model must output.
-
-    Compatible with
-    [GPT-4 Turbo](https://platform.openai.com/docs/models/gpt-4-and-gpt-4-turbo) and
-    all GPT-3.5 Turbo models newer than `gpt-3.5-turbo-1106`.
-
-    Setting to `{ "type": "json_object" }` enables JSON mode, which guarantees the
-    message the model generates is valid JSON.
-
-    **Important:** when using JSON mode, you **must** also instruct the model to
-    produce JSON yourself via a system or user message. Without this, the model may
-    generate an unending stream of whitespace until the generation reaches the token
-    limit, resulting in a long-running and seemingly "stuck" request. Also note that
-    the message content may be partially cut off if `finish_reason="length"`, which
-    indicates the generation exceeded `max_tokens` or the conversation exceeded the
-    max context length.
-    """
-
-    seed: Optional[int]
-    """
-    This feature is in Beta. If specified, our system will make a best effort to
-    sample deterministically, such that repeated requests with the same `seed` and
-    parameters should return the same result. Determinism is not guaranteed, and you
-    should refer to the `system_fingerprint` response parameter to monitor changes
-    in the backend.
-    """
-
-    stop: Union[Optional[str], List[str]]
-    """Up to 4 sequences where the API will stop generating further tokens."""
-
-    temperature: Optional[float]
-    """What sampling temperature to use, between 0 and 2.
-
-    Higher values like 0.8 will make the output more random, while lower values like
-    0.2 will make it more focused and deterministic.
-
-    We generally recommend altering this or `top_p` but not both.
-    """
-
-    tool_choice: ChatCompletionToolChoiceOptionParam
-    """
-    Controls which (if any) function is called by the model. `none` means the model
-    will not call a function and instead generates a message. `auto` means the model
-    can pick between generating a message or calling a function. Specifying a
-    particular function via
-    `{"type": "function", "function": {"name": "my_function"}}` forces the model to
-    call that function.
-
-    `none` is the default when no functions are present. `auto` is the default if
-    functions are present.
-    """
-
-    tools: Iterable[ChatCompletionToolParam]
-    """A list of tools the model may call.
-
-    Currently, only functions are supported as a tool. Use this to provide a list of
-    functions the model may generate JSON inputs for. A max of 128 functions are
-    supported.
-    """
-
-    top_logprobs: Optional[int]
-    """
-    An integer between 0 and 20 specifying the number of most likely tokens to
-    return at each token position, each with an associated log probability.
-    `logprobs` must be set to `true` if this parameter is used.
-    """
-
-    top_p: Optional[float]
-    """
-    An alternative to sampling with temperature, called nucleus sampling, where the
-    model considers the results of the tokens with top_p probability mass. So 0.1
-    means only the tokens comprising the top 10% probability mass are considered.
-
-    We generally recommend altering this or `temperature` but not both.
-    """
-
-    user: str
-    """
-    A unique identifier representing your end-user, which can help OpenAI to monitor
-    and detect abuse.
-    [Learn more](https://platform.openai.com/docs/guides/safety-best-practices/end-user-ids).
-    """
-
-
-FunctionCall = Union[Literal["none", "auto"], ChatCompletionFunctionCallOptionParam]
-
-
-class Function(TypedDict, total=False):
-    name: Required[str]
-    """The name of the function to be called.
-
-    Must be a-z, A-Z, 0-9, or contain underscores and dashes, with a maximum length
-    of 64.
-    """
-
-    description: str
-    """
-    A description of what the function does, used by the model to choose when and
-    how to call the function.
-    """
-
-    parameters: shared_params.FunctionParameters
-    """The parameters the functions accepts, described as a JSON Schema object.
-
-    See the
-    [guide](https://platform.openai.com/docs/guides/text-generation/function-calling)
-    for examples, and the
-    [JSON Schema reference](https://json-schema.org/understanding-json-schema/) for
-    documentation about the format.
-
-    Omitting `parameters` defines a function with an empty parameter list.
-    """
-
-
-class ResponseFormat(TypedDict, total=False):
-    type: Literal["text", "json_object"]
-    """Must be one of `text` or `json_object`."""
-
-
-class CompletionCreateParamsNonStreaming(CompletionCreateParamsBase):
-    stream: Optional[Literal[False]]
-    """If set, partial message deltas will be sent, like in ChatGPT.
-
-    Tokens will be sent as data-only
-    [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format)
-    as they become available, with the stream terminated by a `data: [DONE]`
-    message.
-    [Example Python code](https://cookbook.openai.com/examples/how_to_stream_completions).
-    """
-
-
-class CompletionCreateParamsStreaming(CompletionCreateParamsBase):
-    stream: Required[Literal[True]]
-    """If set, partial message deltas will be sent, like in ChatGPT.
-
-    Tokens will be sent as data-only
-    [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#Event_stream_format)
-    as they become available, with the stream terminated by a `data: [DONE]`
-    message.
-    [Example Python code](https://cookbook.openai.com/examples/how_to_stream_completions).
-    """
-
-
-CompletionCreateParams = Union[CompletionCreateParamsNonStreaming, CompletionCreateParamsStreaming]
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

