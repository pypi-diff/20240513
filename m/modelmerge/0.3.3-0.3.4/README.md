# Comparing `tmp/modelmerge-0.3.3.tar.gz` & `tmp/modelmerge-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelmerge-0.3.3.tar", last modified: Mon May 13 07:25:37 2024, max compression
+gzip compressed data, was "modelmerge-0.3.4.tar", last modified: Mon May 13 08:38:25 2024, max compression
```

## Comparing `modelmerge-0.3.3.tar` & `modelmerge-0.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.383972 modelmerge-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 07:25:25.000000 modelmerge-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 07:25:37.383972 modelmerge-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 07:25:25.000000 modelmerge-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 07:25:37.383972 modelmerge-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 07:25:25.000000 modelmerge-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.379972 modelmerge-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.379972 modelmerge-0.3.3/src/ModelMerge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.379972 modelmerge-0.3.3/src/ModelMerge/models/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30040 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/chatgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/genimi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/models/groq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.379972 modelmerge-0.3.3/src/ModelMerge/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/plugins/today.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/plugins/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/plugins/websearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.383972 modelmerge-0.3.3/src/ModelMerge/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/tools/function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.383972 modelmerge-0.3.3/src/ModelMerge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/utils/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-13 07:25:25.000000 modelmerge-0.3.3/src/ModelMerge/utils/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.383972 modelmerge-0.3.3/src/modelmerge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 07:25:37.000000 modelmerge-0.3.3/src/modelmerge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-13 07:25:37.000000 modelmerge-0.3.3/src/modelmerge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 07:25:37.000000 modelmerge-0.3.3/src/modelmerge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 07:25:37.000000 modelmerge-0.3.3/src/modelmerge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 07:25:37.000000 modelmerge-0.3.3/src/modelmerge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 07:25:37.383972 modelmerge-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 07:25:25.000000 modelmerge-0.3.3/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 07:25:25.000000 modelmerge-0.3.3/test/test_ddg_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 07:25:25.000000 modelmerge-0.3.3/test/test_google_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.441986 modelmerge-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 08:38:14.000000 modelmerge-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 08:38:25.441986 modelmerge-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 08:38:14.000000 modelmerge-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:38:25.441986 modelmerge-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 08:38:14.000000 modelmerge-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.433986 modelmerge-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.433986 modelmerge-0.3.4/src/ModelMerge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30042 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/chatgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/genimi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/models/groq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/plugins/websearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/tools/function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/src/ModelMerge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-13 08:38:14.000000 modelmerge-0.3.4/src/ModelMerge/utils/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.441986 modelmerge-0.3.4/src/modelmerge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 08:38:25.000000 modelmerge-0.3.4/src/modelmerge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:38:25.437986 modelmerge-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test_ddg_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 08:38:14.000000 modelmerge-0.3.4/test/test_google_search.py
```

### Comparing `modelmerge-0.3.3/LICENSE` & `modelmerge-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/PKG-INFO` & `modelmerge-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.3
+Version: 0.3.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
```

### Comparing `modelmerge-0.3.3/README.md` & `modelmerge-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/models/chatgpt.py` & `modelmerge-0.3.4/src/ModelMerge/models/chatgpt.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,21 +360,20 @@
             raise Exception(f"{response.status_code} {response.reason} {response.text}")
         response_role: str = None
         full_response: str = ""
         function_full_response: str = ""
         function_call_name: str = ""
         need_function_call: bool = False
         for line in response.iter_lines():
-            if not line:
+            if not line or line.decode("utf-8").startswith(':'):
                 continue
-            # print("line", line.decode("utf-8"))
-            if line.decode("utf-8")[:6] == "data: ":
+            if line.decode("utf-8").startswith('data:'):
                 line = line.decode("utf-8")[6:]
             else:
-                print(line.decode("utf-8"))
+                print("line", line.decode("utf-8"))
                 full_response = json.loads(line.decode("utf-8"))["choices"][0]["message"]["content"]
                 yield full_response
                 break
             if line == "[DONE]":
                 break
             resp: dict = json.loads(line)
             # print("resp", resp)
```

### Comparing `modelmerge-0.3.3/src/ModelMerge/models/claude.py` & `modelmerge-0.3.4/src/ModelMerge/models/claude.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/models/config.py` & `modelmerge-0.3.4/src/ModelMerge/models/config.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/models/genimi.py` & `modelmerge-0.3.4/src/ModelMerge/models/genimi.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/models/groq.py` & `modelmerge-0.3.4/src/ModelMerge/models/groq.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/plugins/websearch.py` & `modelmerge-0.3.4/src/ModelMerge/plugins/websearch.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/tools/function_call.py` & `modelmerge-0.3.4/src/ModelMerge/tools/function_call.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/utils/prompt.py` & `modelmerge-0.3.4/src/ModelMerge/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/src/ModelMerge/utils/scripts.py` & `modelmerge-0.3.4/src/ModelMerge/utils/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import base64
 import tiktoken
 import requests
 import urllib.parse
 
 def get_encode_text(text, model_name):
     tiktoken.get_encoding("cl100k_base")
+    model_name = "gpt-3.5-turbo"
     encoding = tiktoken.encoding_for_model(model_name)
     encode_text = encoding.encode(text)
     return encoding, encode_text
 
 def get_text_token_len(text, model_name):
     encoding, encode_text = get_encode_text(text, model_name)
     return len(encode_text)
```

### Comparing `modelmerge-0.3.3/src/modelmerge.egg-info/PKG-INFO` & `modelmerge-0.3.4/src/modelmerge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelmerge
-Version: 0.3.3
+Version: 0.3.4
 Summary: modelmerge is a multi-large language model API aggregator.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: requests
 Requires-Dist: pdfminer.six
 Requires-Dist: beautifulsoup4
```

### Comparing `modelmerge-0.3.3/src/modelmerge.egg-info/SOURCES.txt` & `modelmerge-0.3.4/src/modelmerge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelmerge-0.3.3/test/test_google_search.py` & `modelmerge-0.3.4/test/test_google_search.py`

 * *Files identical despite different names*

