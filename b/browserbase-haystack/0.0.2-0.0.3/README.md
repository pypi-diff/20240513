# Comparing `tmp/browserbase_haystack-0.0.2.tar.gz` & `tmp/browserbase_haystack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase_haystack-0.0.2.tar", last modified: Fri Apr 19 11:20:26 2024, max compression
+gzip compressed data, was "browserbase_haystack-0.0.3.tar", last modified: Mon May 13 10:30:07 2024, max compression
```

## Comparing `browserbase_haystack-0.0.2.tar` & `browserbase_haystack-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.443551 browserbase_haystack-0.0.2/
--rw-r--r--   0 mish       (501) staff       (20)     1063 2024-04-18 21:20:37.000000 browserbase_haystack-0.0.2/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     2191 2024-04-19 11:20:26.443290 browserbase_haystack-0.0.2/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)     1578 2024-04-19 11:13:39.000000 browserbase_haystack-0.0.2/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.442211 browserbase_haystack-0.0.2/browserbase_haystack/
--rw-r--r--   0 mish       (501) staff       (20)      825 2024-04-19 11:20:09.000000 browserbase_haystack-0.0.2/browserbase_haystack/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-19 11:20:26.443057 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     2191 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      284 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       24 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       21 2024-04-19 11:20:26.000000 browserbase_haystack-0.0.2/browserbase_haystack.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      672 2024-04-19 11:18:27.000000 browserbase_haystack-0.0.2/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-19 11:20:26.443595 browserbase_haystack-0.0.2/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.752153 browserbase_haystack-0.0.3/
+-rw-r--r--   0 mish       (501) staff       (20)     1063 2024-04-18 21:20:37.000000 browserbase_haystack-0.0.3/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-13 10:30:07.751965 browserbase_haystack-0.0.3/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)     2343 2024-05-13 10:23:31.000000 browserbase_haystack-0.0.3/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.750963 browserbase_haystack-0.0.3/browserbase_haystack/
+-rw-r--r--   0 mish       (501) staff       (20)     1004 2024-05-13 10:25:51.000000 browserbase_haystack-0.0.3/browserbase_haystack/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.751768 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      284 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       24 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       21 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      672 2024-05-13 10:29:43.000000 browserbase_haystack-0.0.3/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-13 10:30:07.752204 browserbase_haystack-0.0.3/setup.cfg
```

### Comparing `browserbase_haystack-0.0.2/LICENSE` & `browserbase_haystack-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase_haystack-0.0.2/PKG-INFO` & `browserbase_haystack-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,20 @@
-Metadata-Version: 2.1
-Name: browserbase-haystack
-Version: 0.0.2
-Summary: Browserbase Haystack Fetcher
-Author-email: Browserbase <info@browserbase.com>
-Project-URL: Homepage, https://browserbase.com
-Project-URL: Issues, https://github.com/browserbase/haystack/issues
-Project-URL: Source, https://github.com/browserbase/haystack
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: haystack-ai
-Requires-Dist: browserbase
-
 # Browserbase Haystack Fetcher
 
-[Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
+[Browserbase](https://browserbase.com) is a developer platform to reliably run, manage, and monitor headless browsers.
+
+Power your AI data retrievals with:
+- [Serverless Infrastructure](https://docs.browserbase.com/under-the-hood) providing reliable browsers to extract data from complex UIs
+- [Stealth Mode](https://docs.browserbase.com/features/stealth-mode) with included fingerprinting tactics and automatic captcha solving
+- [Session Debugger](https://docs.browserbase.com/features/sessions) to inspect your Browser Session with networks timeline and logs
+- [Live Debug](https://docs.browserbase.com/guides/session-debug-connection/browser-remote-control) to quickly debug your automation
 
 ## Installation and setup
 
-- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
+- Get an API key and Project ID from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`, `BROWSERBASE_PROJECT_ID`).
 - Install the required dependencies:
 
 ```
 pip install browserbase-haystack
 ```
 
 ## Usage
@@ -40,27 +29,36 @@
 browserbase_fetcher = BrowserbaseFetcher()
 browserbase_fetcher.run(urls=["https://example.com"], text_content=False)
 ```
 
 ### In a pipeline
 
 ```py
-from browserbase_haystack import BrowserbaseFetcher
 from haystack import Pipeline
 from haystack.components.generators import OpenAIGenerator
 from haystack.components.builders import PromptBuilder
+from browserbase_haystack import BrowserbaseFetcher
 
 prompt_template = (
     "Tell me the titles of the given pages. Pages: {{ documents }}"
 )
 prompt_builder = PromptBuilder(template=prompt_template)
 llm = OpenAIGenerator()
 
+browserbase_fetcher = BrowserbaseFetcher()
+
 pipe = Pipeline()
-pipe.add_component("fetcher", self.browserbase_fetcher)
+pipe.add_component("fetcher", browserbase_fetcher)
 pipe.add_component("prompt_builder", prompt_builder)
 pipe.add_component("llm", llm)
 
 pipe.connect("fetcher.documents", "prompt_builder.documents")
 pipe.connect("prompt_builder.prompt", "llm.prompt")
 result = pipe.run(data={"fetcher": {"urls": ["https://example.com"]}})
 ```
+
+### Parameters
+
+- `urls` Required. A list of URLs to fetch
+- `session_id` Optional. The Session ID
+- `proxy` Optional. Enable Proxy
+- `text_content` Optional. Only return page text content
```

### Comparing `browserbase_haystack-0.0.2/browserbase_haystack/__init__.py` & `browserbase_haystack-0.0.3/browserbase_haystack/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,32 @@
-import os
 from haystack import component
 from haystack.dataclasses import Document
 from browserbase import Browserbase
 from typing import Optional, List, Sequence
 
 
 @component
 class BrowserbaseFetcher:
     def __init__(self, api_key: Optional[str] = None) -> None:
         self.browserbase = Browserbase(api_key=api_key)
 
     @component.output_types(documents=List[Document])
-    def run(self, urls: Sequence[str], text_content: bool = False):
-        pages = self.browserbase.load_urls(urls, text_content)
+    def run(
+        self,
+        urls: Sequence[str],
+        text_content: bool = False,
+        session_id: Optional[str] = None,
+        proxy: Optional[bool] = None,
+    ):
+        pages = self.browserbase.load_urls(
+            urls,
+            text_content,
+            session_id,
+            proxy,
+        )
 
         documents = []
         for i, page in enumerate(pages):
             documents.append(
                 Document(
                     content=page,
                     meta={
```

### Comparing `browserbase_haystack-0.0.2/browserbase_haystack.egg-info/PKG-INFO` & `browserbase_haystack-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase-haystack
-Version: 0.0.2
+Version: 0.0.3
 Summary: Browserbase Haystack Fetcher
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Issues, https://github.com/browserbase/haystack/issues
 Project-URL: Source, https://github.com/browserbase/haystack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,19 +13,25 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: haystack-ai
 Requires-Dist: browserbase
 
 # Browserbase Haystack Fetcher
 
-[Browserbase](https://browserbase.com) is a serverless platform for running headless browsers, it offers advanced debugging, session recordings, stealth mode, integrated proxies and captcha solving.
+[Browserbase](https://browserbase.com) is a developer platform to reliably run, manage, and monitor headless browsers.
+
+Power your AI data retrievals with:
+- [Serverless Infrastructure](https://docs.browserbase.com/under-the-hood) providing reliable browsers to extract data from complex UIs
+- [Stealth Mode](https://docs.browserbase.com/features/stealth-mode) with included fingerprinting tactics and automatic captcha solving
+- [Session Debugger](https://docs.browserbase.com/features/sessions) to inspect your Browser Session with networks timeline and logs
+- [Live Debug](https://docs.browserbase.com/guides/session-debug-connection/browser-remote-control) to quickly debug your automation
 
 ## Installation and setup
 
-- Get an API key from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`).
+- Get an API key and Project ID from [browserbase.com](https://browserbase.com) and set it in environment variables (`BROWSERBASE_API_KEY`, `BROWSERBASE_PROJECT_ID`).
 - Install the required dependencies:
 
 ```
 pip install browserbase-haystack
 ```
 
 ## Usage
@@ -40,27 +46,36 @@
 browserbase_fetcher = BrowserbaseFetcher()
 browserbase_fetcher.run(urls=["https://example.com"], text_content=False)
 ```
 
 ### In a pipeline
 
 ```py
-from browserbase_haystack import BrowserbaseFetcher
 from haystack import Pipeline
 from haystack.components.generators import OpenAIGenerator
 from haystack.components.builders import PromptBuilder
+from browserbase_haystack import BrowserbaseFetcher
 
 prompt_template = (
     "Tell me the titles of the given pages. Pages: {{ documents }}"
 )
 prompt_builder = PromptBuilder(template=prompt_template)
 llm = OpenAIGenerator()
 
+browserbase_fetcher = BrowserbaseFetcher()
+
 pipe = Pipeline()
-pipe.add_component("fetcher", self.browserbase_fetcher)
+pipe.add_component("fetcher", browserbase_fetcher)
 pipe.add_component("prompt_builder", prompt_builder)
 pipe.add_component("llm", llm)
 
 pipe.connect("fetcher.documents", "prompt_builder.documents")
 pipe.connect("prompt_builder.prompt", "llm.prompt")
 result = pipe.run(data={"fetcher": {"urls": ["https://example.com"]}})
 ```
+
+### Parameters
+
+- `urls` Required. A list of URLs to fetch
+- `session_id` Optional. The Session ID
+- `proxy` Optional. Enable Proxy
+- `text_content` Optional. Only return page text content
```

### Comparing `browserbase_haystack-0.0.2/pyproject.toml` & `browserbase_haystack-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase-haystack"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Haystack Fetcher"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

