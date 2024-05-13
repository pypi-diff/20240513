# Comparing `tmp/modelmerge-0.3.1.tar.gz` & `tmp/modelmerge-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.1.tar", last modified: Fri May 10 10:16:47 2024, max compression
+gzip compressed data, was "modelmerge-0.3.2.tar", last modified: Mon May 13 06:12:09 2024, max compression
```

## Comparing `modelmerge-0.3.1.tar` & `modelmerge-0.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.988390 modelmerge-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-10 10:16:40.000000 modelmerge-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-10 10:16:47.988390 modelmerge-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-10 10:16:40.000000 modelmerge-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 10:16:47.988390 modelmerge-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-10 10:16:40.000000 modelmerge-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30077 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.984390 modelmerge-0.3.1/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-10 10:16:40.000000 modelmerge-0.3.1/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.988390 modelmerge-0.3.1/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-10 10:16:47.000000 modelmerge-0.3.1/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-10 10:16:47.000000 modelmerge-0.3.1/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 10:16:47.000000 modelmerge-0.3.1/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-10 10:16:47.000000 modelmerge-0.3.1/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-10 10:16:47.000000 modelmerge-0.3.1/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 10:16:47.988390 modelmerge-0.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-10 10:16:40.000000 modelmerge-0.3.1/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-10 10:16:40.000000 modelmerge-0.3.1/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-10 10:16:40.000000 modelmerge-0.3.1/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.625208 modelmerge-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 06:11:57.000000 modelmerge-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 06:12:09.625208 modelmerge-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 06:11:57.000000 modelmerge-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:12:09.625208 modelmerge-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 06:11:57.000000 modelmerge-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.621208 modelmerge-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.621208 modelmerge-0.3.2/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.621208 modelmerge-0.3.2/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30040 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.621208 modelmerge-0.3.2/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.621208 modelmerge-0.3.2/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.625208 modelmerge-0.3.2/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-13 06:11:57.000000 modelmerge-0.3.2/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.625208 modelmerge-0.3.2/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 06:12:09.000000 modelmerge-0.3.2/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-13 06:12:09.000000 modelmerge-0.3.2/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:12:09.000000 modelmerge-0.3.2/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 06:12:09.000000 modelmerge-0.3.2/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 06:12:09.000000 modelmerge-0.3.2/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:12:09.625208 modelmerge-0.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 06:11:57.000000 modelmerge-0.3.2/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 06:11:57.000000 modelmerge-0.3.2/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 06:11:57.000000 modelmerge-0.3.2/test/test_google_search.py
```

### Comparing `modelmerge-0.3.1/LICENSE` & `modelmerge-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/PKG-INFO` & `modelmerge-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.1
+Version: 0.3.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
```

### Comparing `modelmerge-0.3.1/README.md` & `modelmerge-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.2/src/ModelMerge/models/chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,15 @@
             else 16385
             if "gpt-3.5-turbo-16k" in engine
             # else 99000
             # if "claude-2.1" in engine
             else 4000
         )
         self.truncate_limit: int = truncate_limit or (
-            32000
-            # 126500 Control the number of search characters to prevent excessive spending
+            127500
             if "gpt-4-1106-preview" in engine or "gpt-4-0125-preview" in engine or "gpt-4-turbo" in engine
             else 30500
             if "gpt-4-32k" in engine
             else 6500
             if "gpt-4" in engine
             else 14500
             if "gpt-3.5-turbo-16k" in engine or "gpt-3.5-turbo-1106" in engine
@@ -415,14 +414,15 @@
                 print("\033[32m function_call", function_call_name, "max token:", function_call_max_tokens, "\033[0m")
                 if function_call_name == "get_search_results":
                     prompt = json.loads(function_full_response)["prompt"]
                     yield "🌐 正在搜索您的问题，提取关键词..."
                     llm = BaseLLM(api_key=self.api_key, api_url=self.api_url.source_api_url , engine=self.engine, system_prompt=self.system_prompt)
                     keywords = llm.ask(search_key_word_prompt.format(source=prompt)).split("\n")
                     function_response = yield from eval(function_call_name)(prompt, keywords)
+                    function_call_max_tokens = 32000
                     function_response, text_len = cut_message(function_response, function_call_max_tokens, self.engine)
                     function_response = (
                         f"You need to response the following question: {prompt}. Search results is provided inside <Search_results></Search_results> XML tags. Your task is to think about the question step by step and then answer the above question in {LANGUAGE} based on the Search results provided. Please response in {LANGUAGE} and adopt a style that is logical, in-depth, and detailed. Note: In order to make the answer appear highly professional, you should be an expert in textual analysis, aiming to make the answer precise and comprehensive. Directly response markdown format, without using markdown code blocks"
                         "Here is the Search results, inside <Search_results></Search_results> XML tags:"
                         "<Search_results>"
                         "{}"
                         "</Search_results>"
```

### Comparing `modelmerge-0.3.1/src/ModelMerge/models/claude.py` & `modelmerge-0.3.2/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/models/config.py` & `modelmerge-0.3.2/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.2/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/models/groq.py` & `modelmerge-0.3.2/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.2/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.2/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.2/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.2/src/ModelMerge/utils/scripts.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.2/src/modelmerge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.1
+Version: 0.3.2
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
```

### Comparing `modelmerge-0.3.1/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.3.2/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.1/test/test_google_search.py` & `modelmerge-0.3.2/test/test_google_search.py`

 * *Files identical despite different names*

