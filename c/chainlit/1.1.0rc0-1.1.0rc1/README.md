# Comparing `tmp/chainlit-1.1.0rc0.tar.gz` & `tmp/chainlit-1.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlit-1.1.0rc0.tar", max compression
+gzip compressed data, was "chainlit-1.1.0rc1.tar", max compression
```

## Comparing `chainlit-1.1.0rc0.tar` & `chainlit-1.1.0rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     3884 2024-05-06 12:52:40.694199 chainlit-1.1.0rc0/README.md
--rw-r--r--   0        0        0    10470 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/__init__.py
--rw-r--r--   0        0        0       87 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/__main__.py
--rw-r--r--   0        0        0     1410 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/action.py
--rw-r--r--   0        0        0     2681 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/auth.py
--rw-r--r--   0        0        0     1361 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/cache.py
--rw-r--r--   0        0        0      877 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/chat_settings.py
--rw-r--r--   0        0        0     4951 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/cli/__init__.py
--rw-r--r--   0        0        0      717 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/cli/utils.py
--rw-r--r--   0        0        0    16047 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/config.py
--rw-r--r--   0        0        0     2476 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/context.py
--rw-r--r--   0        0        0     8887 2024-05-06 12:54:57.055417 chainlit-1.1.0rc0/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-05-06 12:54:57.055417 chainlit-1.1.0rc0/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  6986912 2024-05-06 12:54:57.055417 chainlit-1.1.0rc0/chainlit/copilot/dist/index.js
--rw-r--r--   0        0        0    16486 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/data/__init__.py
--rw-r--r--   0        0        0      461 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/data/acl.py
--rw-r--r--   0        0        0    26109 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/data/sql_alchemy.py
--rw-r--r--   0        0        0     3007 2024-05-06 12:52:16.222092 chainlit-1.1.0rc0/chainlit/data/storage_clients.py
--rw-r--r--   0        0        0    10283 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/element.py
--rw-r--r--   0        0        0    12688 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/emitter.py
--rw-r--r--   0        0        0  3038679 2024-05-06 12:54:57.047417 chainlit-1.1.0rc0/chainlit/frontend/dist/assets/index-032fca02.js
--rw-r--r--   0        0        0     6605 2024-05-06 12:54:57.047417 chainlit-1.1.0rc0/chainlit/frontend/dist/assets/index-d088547c.css
--rw-r--r--   0        0        0     8887 2024-05-06 12:54:57.039417 chainlit-1.1.0rc0/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-05-06 12:54:57.039417 chainlit-1.1.0rc0/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  3763471 2024-05-06 12:54:57.043417 chainlit-1.1.0rc0/chainlit/frontend/dist/assets/react-plotly-8c993614.js
--rw-r--r--   0        0        0     6455 2024-05-06 12:54:57.039417 chainlit-1.1.0rc0/chainlit/frontend/dist/favicon.svg
--rw-r--r--   0        0        0     1005 2024-05-06 12:54:57.039417 chainlit-1.1.0rc0/chainlit/frontend/dist/index.html
--rw-r--r--   0        0        0      217 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/haystack/__init__.py
--rw-r--r--   0        0        0     5209 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/haystack/callbacks.py
--rw-r--r--   0        0        0      416 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/hello.py
--rw-r--r--   0        0        0     4949 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/input_widget.py
--rw-r--r--   0        0        0      217 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/langchain/__init__.py
--rw-r--r--   0        0        0    20484 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/langchain/callbacks.py
--rw-r--r--   0        0        0      817 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/langflow/__init__.py
--rw-r--r--   0        0        0      227 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/llama_index/__init__.py
--rw-r--r--   0        0        0     7277 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/llama_index/callbacks.py
--rw-r--r--   0        0        0      373 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/logger.py
--rw-r--r--   0        0        0     2025 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/markdown.py
--rw-r--r--   0        0        0    17961 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/message.py
--rw-r--r--   0        0        0    17459 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/oauth_providers.py
--rw-r--r--   0        0        0     1814 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/openai/__init__.py
--rw-r--r--   0        0        0       80 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/__init__.py
--rw-r--r--   0        0        0      948 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/config.py
--rw-r--r--   0        0        0     3858 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/provider.py
--rw-r--r--   0        0        0      207 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/__init__.py
--rw-r--r--   0        0        0     3495 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/anthropic.py
--rw-r--r--   0        0        0     2130 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/huggingface.py
--rw-r--r--   0        0        0     3103 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/langchain.py
--rw-r--r--   0        0        0    11956 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/openai.py
--rw-r--r--   0        0        0     5084 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/playground/providers/vertexai.py
--rw-r--r--   0        0        0        0 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/py.typed
--rw-r--r--   0        0        0      295 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/secret.py
--rw-r--r--   0        0        0    23851 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/server.py
--rw-r--r--   0        0        0     9241 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/session.py
--rw-r--r--   0        0        0    11654 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/socket.py
--rw-r--r--   0        0        0    13102 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/step.py
--rw-r--r--   0        0        0     1235 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/sync.py
--rw-r--r--   0        0        0     3060 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/telemetry.py
--rw-r--r--   0        0        0     7835 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/translations/en-US.json
--rw-r--r--   0        0        0     2034 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/translations.py
--rw-r--r--   0        0        0     5332 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/types.py
--rw-r--r--   0        0        0      619 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/user.py
--rw-r--r--   0        0        0     1498 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/user_session.py
--rw-r--r--   0        0        0     2604 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/utils.py
--rw-r--r--   0        0        0      196 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/chainlit/version.py
--rw-r--r--   0        0        0     2367 2024-05-06 12:52:16.226092 chainlit-1.1.0rc0/pyproject.toml
--rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 chainlit-1.1.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     3884 2024-05-06 13:25:53.693111 chainlit-1.1.0rc1/README.md
+-rw-r--r--   0        0        0    10470 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/__main__.py
+-rw-r--r--   0        0        0     1410 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/action.py
+-rw-r--r--   0        0        0     2681 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/auth.py
+-rw-r--r--   0        0        0     1361 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/cache.py
+-rw-r--r--   0        0        0      877 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/chat_settings.py
+-rw-r--r--   0        0        0     4951 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/cli/__init__.py
+-rw-r--r--   0        0        0      717 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/cli/utils.py
+-rw-r--r--   0        0        0    16047 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/config.py
+-rw-r--r--   0        0        0     2476 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/context.py
+-rw-r--r--   0        0        0     8887 2024-05-06 13:28:19.716263 chainlit-1.1.0rc1/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-05-06 13:28:19.716263 chainlit-1.1.0rc1/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  6986912 2024-05-06 13:28:19.716263 chainlit-1.1.0rc1/chainlit/copilot/dist/index.js
+-rw-r--r--   0        0        0    16486 2024-05-06 13:25:26.065258 chainlit-1.1.0rc1/chainlit/data/__init__.py
+-rw-r--r--   0        0        0      461 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/data/acl.py
+-rw-r--r--   0        0        0    26109 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/data/sql_alchemy.py
+-rw-r--r--   0        0        0     3007 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/data/storage_clients.py
+-rw-r--r--   0        0        0    10283 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/element.py
+-rw-r--r--   0        0        0    12688 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/emitter.py
+-rw-r--r--   0        0        0  3038679 2024-05-06 13:28:19.700263 chainlit-1.1.0rc1/chainlit/frontend/dist/assets/index-032fca02.js
+-rw-r--r--   0        0        0     6605 2024-05-06 13:28:19.696263 chainlit-1.1.0rc1/chainlit/frontend/dist/assets/index-d088547c.css
+-rw-r--r--   0        0        0     8887 2024-05-06 13:28:19.696263 chainlit-1.1.0rc1/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-05-06 13:28:19.700263 chainlit-1.1.0rc1/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  3763471 2024-05-06 13:28:19.704263 chainlit-1.1.0rc1/chainlit/frontend/dist/assets/react-plotly-8c993614.js
+-rw-r--r--   0        0        0     6455 2024-05-06 13:28:19.696263 chainlit-1.1.0rc1/chainlit/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0     1005 2024-05-06 13:28:19.696263 chainlit-1.1.0rc1/chainlit/frontend/dist/index.html
+-rw-r--r--   0        0        0      217 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/haystack/__init__.py
+-rw-r--r--   0        0        0     5209 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/haystack/callbacks.py
+-rw-r--r--   0        0        0      416 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/hello.py
+-rw-r--r--   0        0        0     4949 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/input_widget.py
+-rw-r--r--   0        0        0      217 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/langchain/__init__.py
+-rw-r--r--   0        0        0    20484 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/langchain/callbacks.py
+-rw-r--r--   0        0        0      817 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/langflow/__init__.py
+-rw-r--r--   0        0        0      227 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/llama_index/__init__.py
+-rw-r--r--   0        0        0     7277 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/llama_index/callbacks.py
+-rw-r--r--   0        0        0      373 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/logger.py
+-rw-r--r--   0        0        0     2025 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/markdown.py
+-rw-r--r--   0        0        0    17961 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/message.py
+-rw-r--r--   0        0        0    17459 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/oauth_providers.py
+-rw-r--r--   0        0        0     1814 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/openai/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/__init__.py
+-rw-r--r--   0        0        0      948 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/config.py
+-rw-r--r--   0        0        0     3858 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/provider.py
+-rw-r--r--   0        0        0      207 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/__init__.py
+-rw-r--r--   0        0        0     3495 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/anthropic.py
+-rw-r--r--   0        0        0     2130 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/huggingface.py
+-rw-r--r--   0        0        0     3103 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/langchain.py
+-rw-r--r--   0        0        0    11956 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/openai.py
+-rw-r--r--   0        0        0     5084 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/playground/providers/vertexai.py
+-rw-r--r--   0        0        0        0 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/py.typed
+-rw-r--r--   0        0        0      295 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/secret.py
+-rw-r--r--   0        0        0    23851 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/server.py
+-rw-r--r--   0        0        0     9241 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/session.py
+-rw-r--r--   0        0        0    11654 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/socket.py
+-rw-r--r--   0        0        0    13102 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/step.py
+-rw-r--r--   0        0        0     1235 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/sync.py
+-rw-r--r--   0        0        0     3060 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/telemetry.py
+-rw-r--r--   0        0        0     7835 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/translations/en-US.json
+-rw-r--r--   0        0        0     2034 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/translations.py
+-rw-r--r--   0        0        0     5332 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/types.py
+-rw-r--r--   0        0        0      619 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/user.py
+-rw-r--r--   0        0        0     1498 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/user_session.py
+-rw-r--r--   0        0        0     2604 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/utils.py
+-rw-r--r--   0        0        0      196 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/chainlit/version.py
+-rw-r--r--   0        0        0     2367 2024-05-06 13:25:26.069258 chainlit-1.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     5561 1970-01-01 00:00:00.000000 chainlit-1.1.0rc1/PKG-INFO
```

### Comparing `chainlit-1.1.0rc0/README.md` & `chainlit-1.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/__init__.py` & `chainlit-1.1.0rc1/chainlit/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/action.py` & `chainlit-1.1.0rc1/chainlit/action.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/auth.py` & `chainlit-1.1.0rc1/chainlit/auth.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/cache.py` & `chainlit-1.1.0rc1/chainlit/cache.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/chat_settings.py` & `chainlit-1.1.0rc1/chainlit/chat_settings.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/cli/__init__.py` & `chainlit-1.1.0rc1/chainlit/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/cli/utils.py` & `chainlit-1.1.0rc1/chainlit/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/config.py` & `chainlit-1.1.0rc1/chainlit/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/context.py` & `chainlit-1.1.0rc1/chainlit/context.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg` & `chainlit-1.1.0rc1/chainlit/copilot/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg` & `chainlit-1.1.0rc1/chainlit/copilot/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/copilot/dist/index.js` & `chainlit-1.1.0rc1/chainlit/copilot/dist/index.js`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/data/__init__.py` & `chainlit-1.1.0rc1/chainlit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/data/sql_alchemy.py` & `chainlit-1.1.0rc1/chainlit/data/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/data/storage_clients.py` & `chainlit-1.1.0rc1/chainlit/data/storage_clients.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/element.py` & `chainlit-1.1.0rc1/chainlit/element.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/emitter.py` & `chainlit-1.1.0rc1/chainlit/emitter.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/assets/index-032fca02.js` & `chainlit-1.1.0rc1/chainlit/frontend/dist/assets/index-032fca02.js`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/assets/index-d088547c.css` & `chainlit-1.1.0rc1/chainlit/frontend/dist/assets/index-d088547c.css`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg` & `chainlit-1.1.0rc1/chainlit/frontend/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg` & `chainlit-1.1.0rc1/chainlit/frontend/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/assets/react-plotly-8c993614.js` & `chainlit-1.1.0rc1/chainlit/frontend/dist/assets/react-plotly-8c993614.js`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/favicon.svg` & `chainlit-1.1.0rc1/chainlit/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/frontend/dist/index.html` & `chainlit-1.1.0rc1/chainlit/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/haystack/callbacks.py` & `chainlit-1.1.0rc1/chainlit/haystack/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/input_widget.py` & `chainlit-1.1.0rc1/chainlit/input_widget.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/langchain/callbacks.py` & `chainlit-1.1.0rc1/chainlit/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/langflow/__init__.py` & `chainlit-1.1.0rc1/chainlit/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/llama_index/callbacks.py` & `chainlit-1.1.0rc1/chainlit/llama_index/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/markdown.py` & `chainlit-1.1.0rc1/chainlit/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/message.py` & `chainlit-1.1.0rc1/chainlit/message.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/oauth_providers.py` & `chainlit-1.1.0rc1/chainlit/oauth_providers.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/openai/__init__.py` & `chainlit-1.1.0rc1/chainlit/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/config.py` & `chainlit-1.1.0rc1/chainlit/playground/config.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/provider.py` & `chainlit-1.1.0rc1/chainlit/playground/provider.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/providers/anthropic.py` & `chainlit-1.1.0rc1/chainlit/playground/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/providers/huggingface.py` & `chainlit-1.1.0rc1/chainlit/playground/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/providers/langchain.py` & `chainlit-1.1.0rc1/chainlit/playground/providers/langchain.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/providers/openai.py` & `chainlit-1.1.0rc1/chainlit/playground/providers/openai.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/playground/providers/vertexai.py` & `chainlit-1.1.0rc1/chainlit/playground/providers/vertexai.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/server.py` & `chainlit-1.1.0rc1/chainlit/server.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/session.py` & `chainlit-1.1.0rc1/chainlit/session.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/socket.py` & `chainlit-1.1.0rc1/chainlit/socket.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/step.py` & `chainlit-1.1.0rc1/chainlit/step.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/sync.py` & `chainlit-1.1.0rc1/chainlit/sync.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/telemetry.py` & `chainlit-1.1.0rc1/chainlit/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/translations/en-US.json` & `chainlit-1.1.0rc1/chainlit/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/translations.py` & `chainlit-1.1.0rc1/chainlit/translations.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/types.py` & `chainlit-1.1.0rc1/chainlit/types.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/user.py` & `chainlit-1.1.0rc1/chainlit/user.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/user_session.py` & `chainlit-1.1.0rc1/chainlit/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/chainlit/utils.py` & `chainlit-1.1.0rc1/chainlit/utils.py`

 * *Files identical despite different names*

### Comparing `chainlit-1.1.0rc0/pyproject.toml` & `chainlit-1.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlit"
-version = "1.1.0rc0"
+version = "1.1.0rc1"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'openai', 'copilot', 'langchain', 'conversational ai']
 description = "Build Conversational AI."
 authors = ["Chainlit"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
@@ -19,15 +19,15 @@
 [tool.poetry.scripts]
 # command_name = module_for_handler : function_for_handler
 chainlit = 'chainlit.cli:cli'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 httpx = ">=0.23.0"
-literalai = "0.0.509"
+literalai = "0.0.600"
 dataclasses_json = "^0.5.7"
 fastapi = "^0.110.1"
 starlette = "^0.37.2"
 uvicorn = "^0.25.0"
 fastapi-socketio = "^0.0.10"
 aiofiles = "^23.1.0"
 syncer = "^2.0.3"
```

### Comparing `chainlit-1.1.0rc0/PKG-INFO` & `chainlit-1.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlit
-Version: 1.1.0rc0
+Version: 1.1.0rc1
 Summary: Build Conversational AI.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,openai,copilot,langchain,conversational ai
 Author: Chainlit
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
@@ -18,15 +18,15 @@
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dataclasses_json (>=0.5.7,<0.6.0)
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: fastapi-socketio (>=0.0.10,<0.0.11)
 Requires-Dist: filetype (>=1.2.0,<2.0.0)
 Requires-Dist: httpx (>=0.23.0)
 Requires-Dist: lazify (>=0.4.0,<0.5.0)
-Requires-Dist: literalai (==0.0.509)
+Requires-Dist: literalai (==0.0.600)
 Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-graphql-client (>=0.4.3,<0.5.0)
 Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
```

