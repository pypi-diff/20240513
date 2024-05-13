# Comparing `tmp/elia_chat-1.2.0.tar.gz` & `tmp/elia_chat-1.3.0.tar.gz`

## Comparing `elia_chat-1.2.0.tar` & `elia_chat-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.python-version
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.2.0/requirements-dev.lock
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.2.0/requirements.lock
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/__main__.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/app.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/chats_manager.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/config.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/constants.py
--rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/elia.scss
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/launch_args.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/locations.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/models.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/runtime_config.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/time_display.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/converters.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/database.py
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/import_chatgpt.py
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/database/models.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/chat_details.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/chat_screen.py
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/help_screen.py
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/screens/home_screen.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/agent_is_typing.py
--rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/app_header.py
--rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_header.py
--rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_list.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chat_options.py
--rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/chatbox.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/prompt_input.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.2.0/elia_chat/widgets/token_analysis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.2.0/.gitignore
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 elia_chat-1.2.0/README.md
--rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 elia_chat-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.python-version
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 elia_chat-1.3.0/requirements-dev.lock
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 elia_chat-1.3.0/requirements.lock
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/__main__.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/app.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/chats_manager.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/config.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/constants.py
+-rw-r--r--   0        0        0     8984 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/elia.scss
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/launch_args.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/locations.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/models.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/runtime_config.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/time_display.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/converters.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/database.py
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/import_chatgpt.py
+-rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/database/models.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/chat_details.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/chat_screen.py
+-rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/help_screen.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/screens/home_screen.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/agent_is_typing.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/app_header.py
+-rw-r--r--   0        0        0    10891 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_header.py
+-rw-r--r--   0        0        0     4586 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_list.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chat_options.py
+-rw-r--r--   0        0        0    10502 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/chatbox.py
+-rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/prompt_input.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 elia_chat-1.3.0/elia_chat/widgets/token_analysis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 elia_chat-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 elia_chat-1.3.0/.gitignore
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 elia_chat-1.3.0/README.md
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 elia_chat-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 elia_chat-1.3.0/PKG-INFO
```

### Comparing `elia_chat-1.2.0/.pre-commit-config.yaml` & `elia_chat-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/requirements-dev.lock` & `elia_chat-1.3.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/requirements.lock` & `elia_chat-1.3.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/__main__.py` & `elia_chat-1.3.0/elia_chat/__main__.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/app.py` & `elia_chat-1.3.0/elia_chat/app.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/chats_manager.py` & `elia_chat-1.3.0/elia_chat/chats_manager.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/config.py` & `elia_chat-1.3.0/elia_chat/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,24 +50,31 @@
     return [
         EliaChatModel(
             id="elia-gpt-3.5-turbo",
             name="gpt-3.5-turbo",
             display_name="GPT-3.5 Turbo",
             provider="OpenAI",
             product="ChatGPT",
-            description="The fastest ChatGPT model, great for most everyday tasks",
+            description="Fast & inexpensive model for simple tasks.",
+        ),
+        EliaChatModel(
+            id="elia-gpt-4o",
+            name="openai/gpt-4o",
+            display_name="GPT-4o",
+            provider="OpenAI",
+            product="ChatGPT",
+            description="Fastest and most affordable flagship model.",
         ),
         EliaChatModel(
             id="elia-gpt-4-turbo",
             name="gpt-4-turbo",
             display_name="GPT-4 Turbo",
             provider="OpenAI",
             product="ChatGPT",
-            description="The most powerful ChatGPT model, capable of "
-            "complex tasks which require advanced reasoning",
+            description="Previous high-intelligence model.",
         ),
     ]
 
 
 def get_builtin_anthropic_models() -> list[EliaChatModel]:
     return [
         EliaChatModel(
```

### Comparing `elia_chat-1.2.0/elia_chat/elia.scss` & `elia_chat-1.3.0/elia_chat/elia.scss`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/locations.py` & `elia_chat-1.3.0/elia_chat/locations.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/models.py` & `elia_chat-1.3.0/elia_chat/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/time_display.py` & `elia_chat-1.3.0/elia_chat/time_display.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/database/converters.py` & `elia_chat-1.3.0/elia_chat/database/converters.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/database/database.py` & `elia_chat-1.3.0/elia_chat/database/database.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/database/import_chatgpt.py` & `elia_chat-1.3.0/elia_chat/database/import_chatgpt.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/database/models.py` & `elia_chat-1.3.0/elia_chat/database/models.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/screens/chat_details.py` & `elia_chat-1.3.0/elia_chat/screens/chat_details.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/screens/chat_screen.py` & `elia_chat-1.3.0/elia_chat/screens/chat_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/screens/help_screen.py` & `elia_chat-1.3.0/elia_chat/screens/help_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/screens/home_screen.py` & `elia_chat-1.3.0/elia_chat/screens/home_screen.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/app_header.py` & `elia_chat-1.3.0/elia_chat/widgets/app_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/chat.py` & `elia_chat-1.3.0/elia_chat/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/chat_header.py` & `elia_chat-1.3.0/elia_chat/widgets/chat_header.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/chat_list.py` & `elia_chat-1.3.0/elia_chat/widgets/chat_list.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/chat_options.py` & `elia_chat-1.3.0/elia_chat/widgets/chat_options.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/chatbox.py` & `elia_chat-1.3.0/elia_chat/widgets/chatbox.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/prompt_input.py` & `elia_chat-1.3.0/elia_chat/widgets/prompt_input.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/elia_chat/widgets/token_analysis.py` & `elia_chat-1.3.0/elia_chat/widgets/token_analysis.py`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/.gitignore` & `elia_chat-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `elia_chat-1.2.0/README.md` & `elia_chat-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,51 +1,55 @@
-## Elia
+<h1 align="center">
+    <img src="https://github.com/darrenburns/elia/assets/5740731/4037b91a-1ad8-4d5b-884d-b3f1b495acf4" width="126px">
+</h1>
+<p align="center">
+  <i align="center">A snappy, keyboard-centric terminal user interface for interacting with large language models.</i><br>
+  <i align="center">Chat with Claude 3, ChatGPT, and local models like Llama 3, Phi 3, Mistral and Gemma.</i>
+</p>
+
+![elia-screenshot-collage](https://github.com/darrenburns/elia/assets/5740731/75f8563f-ce1a-4c9c-98c0-1bd1f7010814)
+
+## Introduction
+
+`elia` is an application for interacting with LLMs which runs entirely in your terminal, and is designed to be keyboard-focused, efficient, and fun to use!
+It stores your conversations in a local SQLite database, and allows you to interact with a variety of models.
+Speak with proprietary models such as ChatGPT and Claude, or with local models running through `ollama` or LocalAI.
 
-A powerful terminal user interface for interacting with large language models.
-
-Chat with Claude 3, ChatGPT, and local models like Llama 3, Phi 3, Mistral and Gemma.
-
-<img width="1439" alt="elia-stacked-screenshot" src="https://github.com/darrenburns/elia/assets/5740731/8fb15936-abeb-4464-b34d-f6cb001913e4">
-
-Your conversations are stored locally in a SQLite database.
-
-Conversations with local models are done via `ollama` and never leave your machine.
-
-### Installation
+## Installation
 
 Install Elia with [pipx](https://github.com/pypa/pipx):
 
 ```bash
 pipx install elia-chat
 ```
 
 Depending on the model you wish to use, you may need to set one or more environment variables (e.g. `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`, etc).
 
-### Quickstart
+## Quickstart
 
 Launch Elia from the command line:
 
 ```bash
 elia
 ```
 
 Launch directly a new chat from the command line:
 
 ```bash
 elia "What is the Zen of Python?"
 ```
 
-### Running local models
+## Running local models
 
 1. Install [`ollama`](https://github.com/ollama/ollama).
 2. Pull the model you require, e.g. `ollama pull llama3`.
 3. Run the local ollama server: `ollama serve`.
 4. Add the model to the config file (see below).
 
-### Configuration
+## Configuration
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
@@ -84,26 +88,26 @@
 
 [[models]]
 id = "personal-gpt-3.5-turbo"
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Personal)"
 ```
 
-### Import from ChatGPT
+## Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
 ```
 
-### Wiping the database
+## Wiping the database
 
 ```bash
 elia reset
 ```
 
-### Uninstalling
+## Uninstalling
 
 ```bash
 pipx uninstall elia-chat
 ```
```

### Comparing `elia_chat-1.2.0/pyproject.toml` & `elia_chat-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "elia_chat"
-version = "1.2.0"
+version = "1.3.0"
 description = "A powerful terminal user interface for interacting with large language models."
 authors = [
     { name = "Darren Burns", email = "darrenb900@gmail.com" }
 ]
 dependencies = [
     "textual[syntax]==0.58.1",
     "sqlmodel>=0.0.9",
```

### Comparing `elia_chat-1.2.0/PKG-INFO` & `elia_chat-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: elia_chat
-Version: 1.2.0
+Version: 1.3.0
 Summary: A powerful terminal user interface for interacting with large language models.
 Author-email: Darren Burns <darrenb900@gmail.com>
 Requires-Python: >=3.11
 Requires-Dist: aiosqlite>=0.20.0
 Requires-Dist: click-default-group>=1.2.4
 Requires-Dist: click>=8.1.6
 Requires-Dist: greenlet>=3.0.3
@@ -12,58 +12,62 @@
 Requires-Dist: litellm>=1.35.38
 Requires-Dist: pydantic-settings>=2.2.1
 Requires-Dist: sqlmodel>=0.0.9
 Requires-Dist: textual[syntax]==0.58.1
 Requires-Dist: xdg-base-dirs>=6.0.1
 Description-Content-Type: text/markdown
 
-## Elia
+<h1 align="center">
+    <img src="https://github.com/darrenburns/elia/assets/5740731/4037b91a-1ad8-4d5b-884d-b3f1b495acf4" width="126px">
+</h1>
+<p align="center">
+  <i align="center">A snappy, keyboard-centric terminal user interface for interacting with large language models.</i><br>
+  <i align="center">Chat with Claude 3, ChatGPT, and local models like Llama 3, Phi 3, Mistral and Gemma.</i>
+</p>
+
+![elia-screenshot-collage](https://github.com/darrenburns/elia/assets/5740731/75f8563f-ce1a-4c9c-98c0-1bd1f7010814)
+
+## Introduction
+
+`elia` is an application for interacting with LLMs which runs entirely in your terminal, and is designed to be keyboard-focused, efficient, and fun to use!
+It stores your conversations in a local SQLite database, and allows you to interact with a variety of models.
+Speak with proprietary models such as ChatGPT and Claude, or with local models running through `ollama` or LocalAI.
 
-A powerful terminal user interface for interacting with large language models.
-
-Chat with Claude 3, ChatGPT, and local models like Llama 3, Phi 3, Mistral and Gemma.
-
-<img width="1439" alt="elia-stacked-screenshot" src="https://github.com/darrenburns/elia/assets/5740731/8fb15936-abeb-4464-b34d-f6cb001913e4">
-
-Your conversations are stored locally in a SQLite database.
-
-Conversations with local models are done via `ollama` and never leave your machine.
-
-### Installation
+## Installation
 
 Install Elia with [pipx](https://github.com/pypa/pipx):
 
 ```bash
 pipx install elia-chat
 ```
 
 Depending on the model you wish to use, you may need to set one or more environment variables (e.g. `OPENAI_API_KEY`, `ANTHROPIC_API_KEY`, etc).
 
-### Quickstart
+## Quickstart
 
 Launch Elia from the command line:
 
 ```bash
 elia
 ```
 
 Launch directly a new chat from the command line:
 
 ```bash
 elia "What is the Zen of Python?"
 ```
 
-### Running local models
+## Running local models
 
 1. Install [`ollama`](https://github.com/ollama/ollama).
 2. Pull the model you require, e.g. `ollama pull llama3`.
 3. Run the local ollama server: `ollama serve`.
 4. Add the model to the config file (see below).
 
-### Configuration
+## Configuration
 
 The location of the configuration file is noted at the bottom of
 the options window (`ctrl+o`).
 
 The example file below shows the available options, as well as examples of how to add new models.
 
 ```toml
@@ -102,26 +106,26 @@
 
 [[models]]
 id = "personal-gpt-3.5-turbo"
 name = "gpt-3.5-turbo"
 display_name = "GPT 3.5 Turbo (Personal)"
 ```
 
-### Import from ChatGPT
+## Import from ChatGPT
 
 Export your conversations to a JSON file using the ChatGPT UI, then import them using the `import` command.
 
 ```bash
 elia import 'path/to/conversations.json'
 ```
 
-### Wiping the database
+## Wiping the database
 
 ```bash
 elia reset
 ```
 
-### Uninstalling
+## Uninstalling
 
 ```bash
 pipx uninstall elia-chat
 ```
```

