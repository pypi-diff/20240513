# Comparing `tmp/lfg_llama-1.3.3.tar.gz` & `tmp/lfg_llama-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfg_llama-1.3.3.tar", last modified: Sun May 12 07:32:58 2024, max compression
+gzip compressed data, was "lfg_llama-2.0.0.tar", last modified: Mon May 13 18:49:27 2024, max compression
```

## Comparing `lfg_llama-1.3.3.tar` & `lfg_llama-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.359264 lfg_llama-1.3.3/
--rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-12 07:32:58.358975 lfg_llama-1.3.3/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)     1671 2024-05-09 08:01:29.000000 lfg_llama-1.3.3/README.md
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.357833 lfg_llama-1.3.3/lfg/
--rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-1.3.3/lfg/__init__.py
--rwxr-xr-x   0 ob907      (502) staff       (20)     3575 2024-05-12 07:31:51.000000 lfg_llama-1.3.3/lfg/cli.py
-drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-12 07:32:58.358758 lfg_llama-1.3.3/lfg_llama.egg-info/
--rw-r--r--   0 ob907      (502) staff       (20)     1908 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/PKG-INFO
--rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/SOURCES.txt
--rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/dependency_links.txt
--rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/entry_points.txt
--rw-r--r--   0 ob907      (502) staff       (20)        5 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/requires.txt
--rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-12 07:32:58.000000 lfg_llama-1.3.3/lfg_llama.egg-info/top_level.txt
--rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-12 07:32:58.359336 lfg_llama-1.3.3/setup.cfg
--rw-r--r--   0 ob907      (502) staff       (20)      462 2024-05-12 07:32:51.000000 lfg_llama-1.3.3/setup.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:49:27.928620 lfg_llama-2.0.0/
+-rw-r--r--   0 ob907      (502) staff       (20)     2133 2024-05-13 18:49:27.928391 lfg_llama-2.0.0/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)     1893 2024-05-13 18:45:42.000000 lfg_llama-2.0.0/README.md
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:49:27.926634 lfg_llama-2.0.0/lfg/
+-rw-r--r--   0 ob907      (502) staff       (20)        0 2024-04-28 17:51:36.000000 lfg_llama-2.0.0/lfg/__init__.py
+-rwxr-xr-x   0 ob907      (502) staff       (20)     3031 2024-05-13 18:46:49.000000 lfg_llama-2.0.0/lfg/cli.py
+drwxr-xr-x   0 ob907      (502) staff       (20)        0 2024-05-13 18:49:27.928013 lfg_llama-2.0.0/lfg_llama.egg-info/
+-rw-r--r--   0 ob907      (502) staff       (20)     2133 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/PKG-INFO
+-rw-r--r--   0 ob907      (502) staff       (20)      245 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/SOURCES.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        1 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/dependency_links.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       37 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/entry_points.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        8 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/requires.txt
+-rw-r--r--   0 ob907      (502) staff       (20)        4 2024-05-13 18:49:27.000000 lfg_llama-2.0.0/lfg_llama.egg-info/top_level.txt
+-rw-r--r--   0 ob907      (502) staff       (20)       38 2024-05-13 18:49:27.928705 lfg_llama-2.0.0/setup.cfg
+-rw-r--r--   0 ob907      (502) staff       (20)      465 2024-05-13 18:48:02.000000 lfg_llama-2.0.0/setup.py
```

### Comparing `lfg_llama-1.3.3/PKG-INFO` & `lfg_llama-2.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.3
+Version: 2.0.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
-Requires-Dist: groq
+Requires-Dist: openapi
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
 ![Demo](example.gif)
 
-LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch.
+LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
-Testing the llama3 model. Initially it was made using ollama locally, but changed to use groq due to not needing to have the llama3 model downloaded.
+- Firstly, this was created to test Ollama -> Groq
+- I do not like the Github Copilot command-line
+- Quicker than using Gemini/ChatGPT/Google directly via the browser interface
+- Easier to find what needed without opening man pages
+- NEW: Changing to GPT-4o model which is free
+
+However, never trust the output entirely.
 
 ## Installation
 
 ```bash
 # install pipx
 brew install pipx
 
@@ -31,26 +37,26 @@
 # restart your terminal
 # install LFG
 pipx install lfg-llama
 ```
 
 ## Usage
 
-This executable is using Groq, that means you need and [API token](https://console.groq.com/keys).
+This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
-Groq is free beta, for now.
+[GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-export GROQ_API_KEY=1337
+OPENAI_API_KEY={replace_me}
 ```
 
 ```
-$ lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query
+$ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
 lfg "kill port 3000"
```

### Comparing `lfg_llama-1.3.3/README.md` & `lfg_llama-2.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
 ![Demo](example.gif)
 
-LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch.
+LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
-Testing the llama3 model. Initially it was made using ollama locally, but changed to use groq due to not needing to have the llama3 model downloaded.
+- Firstly, this was created to test Ollama -> Groq
+- I do not like the Github Copilot command-line
+- Quicker than using Gemini/ChatGPT/Google directly via the browser interface
+- Easier to find what needed without opening man pages
+- NEW: Changing to GPT-4o model which is free
+
+However, never trust the output entirely.
 
 ## Installation
 
 ```bash
 # install pipx
 brew install pipx
 
@@ -22,26 +28,26 @@
 # restart your terminal
 # install LFG
 pipx install lfg-llama
 ```
 
 ## Usage
 
-This executable is using Groq, that means you need and [API token](https://console.groq.com/keys).
+This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
-Groq is free beta, for now.
+[GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-export GROQ_API_KEY=1337
+OPENAI_API_KEY={replace_me}
 ```
 
 ```
-$ lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query
+$ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
 lfg "kill port 3000"
```

### Comparing `lfg_llama-1.3.3/lfg/cli.py` & `lfg_llama-2.0.0/lfg/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,35 @@
 #!/usr/bin/python3
 
 import os
 import sys
 import argparse
-from enum import Enum
-from groq import Groq
-from groq.types.chat import ChatCompletion
+import openai
+from openai import OpenAI
+from openai.types.chat import ChatCompletion
 
 
-class Models(Enum):
-    """
-    Enumerates supported language models providing model ID references
-    for API calls.
-    """
-
-    LLAMA38B = "llama3-8b-8192"
-    LLAMA370B = "llama3-70b-8192"
-    MIXTRAL8X7B = "mixtral-8x7b-32768"
-    GEMMA7B = "gemma-7b-it"
-
-
-def get_groq_client() -> Groq:
-    """Retrieves the GROQ API key and creates a Groq client instance.
+def get_openai_client() -> OpenAI:
+    """Retrieves the OpenAI API key and creates a OpenAI client instance.
 
     Raises:
-        ValueError: If the GROQ_API_KEY environment variable is not set.
+        ValueError: If the OPENAI_API_KEY environment variable is not set.
     """
-    api_key = os.environ.get("GROQ_API_KEY")
+    api_key = os.environ.get("OPENAI_API_KEY")
     if not api_key:
-        raise ValueError("GROQ_API_KEY environment variable is not set")
+        raise ValueError("OPENAI_API_KEY environment variable is not set")
 
-    return Groq(api_key=api_key)
+    return OpenAI()
 
 
 def generate_system_prompt() -> str:
     """Returns the system prompt for the LLM interaction."""
 
     return """
-You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'. The layout of your response should be as follows: ```\n{command}\n``` \n\n Explanation:\n {explanation}.
+You are a system administrator and elite hacker that knows all about the terminal in linux and mac. I provide you with a question about a command, and you give me back a response which shows the command, then a short explanation. The command should be wrapped as a code block. If you get asked about the command lfg, reply "lfg query" with explanation 'This is me'. It is important you do not return commands you do not know. If that is the case, just respond 'I do not know'. The layout of your response should be as follows: ```\n{command}\n``` \n\n Explanation:\n {explanation}.
 """
 
 
 def handle_stream(stream: ChatCompletion) -> None:
     """Processes the output stream from the LLM, printing each response chunk.
 
     Args:
@@ -49,61 +37,56 @@
         LLM responses.
     """
     for chunk in stream:
         if chunk.choices[0].delta.content:
             print(chunk.choices[0].delta.content, end="", flush=True)
 
 
-def send_chat_query(query: str, model: str, client: Groq) -> ChatCompletion:
-    """Sends a query to the Groq API and handles the response.
+def send_chat_query(query: str, client: OpenAI) -> ChatCompletion:
+    """Sends a query to the OpenAI API and handles the response.
 
     Args:
         query (str): The user's query.
-        model (str): The LLM of choice
-        client (Groq): The Groq client instance.
+        client (OpenAI): The OpenAI client instance.
     """
     try:
         stream = client.chat.completions.create(
             messages=[
                 {"role": "system", "content": generate_system_prompt()},
                 {"role": "user", "content": query},
             ],
-            model=Models[model].value,
+            model="gpt-4o",
             stream=True,
         )
 
         return stream
-    except Groq.APIConnectionError as e:
+
+    except openai.APIConnectionError as e:
         print("The server could not be reached")
         print(e.__cause__)
-    except Groq.RateLimitError as e:
-        print("A 429 status code was received; Rate limited.")
+    except openai.RateLimitError as e:
+        print("A 429 status code was received; we should back off a bit.")
         print(e.response)
-    except Groq.APIStatusError as e:
+    except openai.APIStatusError as e:
         print("Another non-200-range status code was received")
         print(e.status_code)
         print(e.response)
 
 
 def main():
-    """Initializes the Groq client, and processes the query."""
+    """Initializes the OpenAI client, and processes the query."""
 
     parser = argparse.ArgumentParser()
     parser.add_argument("query", type=str, help="The query sent to the LLM")
-    parser.add_argument(
-        "-m",
-        choices=["llama38b", "llama370b", "mixtral8x7b", "gemma7b"],
-        default="llama370b",
-        help="Select the language model.",
-    )
+
     args = parser.parse_args()
 
     try:
-        client = get_groq_client()
-        stream = send_chat_query(args.query, args.m.upper(), client)
+        client = get_openai_client()
+        stream = send_chat_query(args.query, client)
 
         handle_stream(stream)
     except ValueError as e:
         print(f"Error: {e}")
 
 
 if __name__ == "__main__":
```

### Comparing `lfg_llama-1.3.3/lfg_llama.egg-info/PKG-INFO` & `lfg_llama-2.0.0/lfg_llama.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 Metadata-Version: 2.1
 Name: lfg-llama
-Version: 1.3.3
+Version: 2.0.0
 Summary: LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 Author: Bjarne Oeverli
 Author-email: bjarneocodes@gmail.com
 Description-Content-Type: text/markdown
-Requires-Dist: groq
+Requires-Dist: openapi
 
 # LFG
 
 > LFG, It Really Whips the Llama's Ass 🦙🦙🦙🦙
 
 ![Demo](example.gif)
 
-LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch.
+LFG is a command-line tool that intelligently helps you find the right terminal commands for your tasks. Such sales pitch. This interface is using GPT-4o as an engine.
 
 ## Why?
 
-Testing the llama3 model. Initially it was made using ollama locally, but changed to use groq due to not needing to have the llama3 model downloaded.
+- Firstly, this was created to test Ollama -> Groq
+- I do not like the Github Copilot command-line
+- Quicker than using Gemini/ChatGPT/Google directly via the browser interface
+- Easier to find what needed without opening man pages
+- NEW: Changing to GPT-4o model which is free
+
+However, never trust the output entirely.
 
 ## Installation
 
 ```bash
 # install pipx
 brew install pipx
 
@@ -31,26 +37,26 @@
 # restart your terminal
 # install LFG
 pipx install lfg-llama
 ```
 
 ## Usage
 
-This executable is using Groq, that means you need and [API token](https://console.groq.com/keys).
+This executable is using OpenAI, that means you need and [API token](https://platform.openai.com/api-keys).
 
-Groq is free beta, for now.
+[GPT-4o](https://platform.openai.com/docs/models/gpt-4o) is free to use.
 
 Add the token to your .bashrc/.zshrc and reload your terminal.
 
 ```
-export GROQ_API_KEY=1337
+OPENAI_API_KEY={replace_me}
 ```
 
 ```
-$ lfg [-h] [-m {llama38b,llama370b,mixtral8x7b,gemma7b}] query
+$ lfg query
 ```
 
 Now you can use the executable
 
 ```bash
 lfg "kill port 3000"
```

