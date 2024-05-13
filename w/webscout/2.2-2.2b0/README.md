# Comparing `tmp/webscout-2.2.tar.gz` & `tmp/webscout-2.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.2.tar", last modified: Sun May 12 05:42:48 2024, max compression
+gzip compressed data, was "webscout-2.2b0.tar", last modified: Mon May 13 07:37:06 2024, max compression
```

## Comparing `webscout-2.2.tar` & `webscout-2.2b0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.749788 webscout-2.2/
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.359171 webscout-2.2/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.376729 webscout-2.2/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.404951 webscout-2.2/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.417384 webscout-2.2/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.2/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.2/LICENSE.md
--rw-rw-rw-   0        0        0    46475 2024-05-12 05:42:48.744790 webscout-2.2/PKG-INFO
--rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-12 05:42:48.750789 webscout-2.2/setup.cfg
--rw-rw-rw-   0        0        0     2781 2024-05-12 05:24:59.000000 webscout-2.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.564553 webscout-2.2/webscout/
--rw-rw-rw-   0        0        0    17297 2024-05-10 14:45:32.000000 webscout-2.2/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.2/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.2/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.2/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.2/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.731790 webscout-2.2/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.2/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.2/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.2/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.2/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.2/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.2/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.2/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.2/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.2/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.2/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.2/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.2/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.2/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.2/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.2/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.2/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.2/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.2/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.2/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     2338 2024-05-12 05:18:43.000000 webscout-2.2/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.2/webscout/__main__.py
--rw-rw-rw-   0        0        0      711 2024-05-10 14:40:09.000000 webscout-2.2/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.2/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.2/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24489 2024-05-10 14:33:00.000000 webscout-2.2/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.2/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.2/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.2/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.2/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.2/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.2/webscout/voice.py
--rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.2/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.2/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.2/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-12 05:42:48.738788 webscout-2.2/webscout.egg-info/
--rw-rw-rw-   0        0        0    46475 2024-05-12 05:42:47.000000 webscout-2.2/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1592 2024-05-12 05:42:48.000000 webscout-2.2/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 05:42:47.000000 webscout-2.2/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2024-05-12 05:42:47.000000 webscout-2.2/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-05-12 05:42:47.000000 webscout-2.2/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 05:42:47.000000 webscout-2.2/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.385669 webscout-2.2b0/
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.119052 webscout-2.2b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.136053 webscout-2.2b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.296483 webscout-2.2b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.479268 webscout-2.2b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.2b0/LICENSE.md
+-rw-rw-rw-   0        0        0    46603 2024-05-13 07:37:06.381673 webscout-2.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.2b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:37:06.385669 webscout-2.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     2696 2024-05-13 07:35:11.000000 webscout-2.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.695582 webscout-2.2b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.2b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.2b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.290314 webscout-2.2b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.2b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.2b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.2b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.2b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.2b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.2b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.2b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.2b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.2b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.2b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.2b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.2b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.2b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.2b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.2b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.2b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.2b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.2b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.2b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     2595 2024-05-13 07:31:21.000000 webscout-2.2b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.2b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.2b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.2b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.2b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.2b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.2b0/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.2b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.2b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.376671 webscout-2.2b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    46603 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      366 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.2/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.2b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.2b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/networks/filepath_converter.py` & `webscout-2.2b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/networks/google_searcher.py` & `webscout-2.2b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/networks/network_configs.py` & `webscout-2.2b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.2b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/utilsdw/enver.py` & `webscout-2.2b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/DeepWEBS/utilsdw/logger.py` & `webscout-2.2b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/LICENSE.md` & `webscout-2.2b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.2/PKG-INFO` & `webscout-2.2b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.2
-Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Version: 2.2b0
+Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -32,15 +32,14 @@
 Requires-Dist: selenium
 Requires-Dist: tqdm
 Requires-Dist: webdriver-manager
 Requires-Dist: halo>=0.0.31
 Requires-Dist: g4f>=0.2.2.3
 Requires-Dist: rich
 Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
@@ -51,14 +50,18 @@
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
 Requires-Dist: playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
+Provides-Extra: local
+Requires-Dist: llama-cpp-python; extra == "local"
+Requires-Dist: colorama; extra == "local"
+Requires-Dist: numpy; extra == "local"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.2 Summary: Search for anything
-using the Google, DuckDuckGo, phind.com. Also containes AI models, can
-transcribe yt videos, temporary email and phone number generation, have TTS
-support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Metadata-Version: 2.1 Name: webscout Version: 2.2b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, and webai (terminal gpt and open interpreter). Author: OEvortex
+Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
+License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -17,21 +17,23 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Description-Content-
 Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Requires-Dist: clipman
-Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
-== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
+Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
+Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
+Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
+Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
+Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
+pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
+python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
+Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
```

### Comparing `webscout-2.2/README.md` & `webscout-2.2b0/README.md`

 * *Files identical despite different names*

### Comparing `webscout-2.2/setup.py` & `webscout-2.2b0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,49 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.2", 
-    description="Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)",
+    version="2.2-beta",
+    description="Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: Other/Proprietary License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Topic :: Internet :: WWW/HTTP :: Indexing/Search',
-        'Topic :: Software Development :: Libraries :: Python Modules',
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: Other/Proprietary License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
+        "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     install_requires=[
         "docstring_inheritance",
         "click",
         "curl_cffi",
         "lxml",
         "nest-asyncio",
         "selenium",
         "tqdm",
         "webdriver-manager",
         "halo>=0.0.31",
         "g4f>=0.2.2.3",
         "rich",
         "python-dotenv",
-        "Helpingai-T2",
         "beautifulsoup4",
         "markdownify",
         "pydantic",
         "requests",
         "sse_starlette",
         "termcolor",
         "tiktoken",
@@ -56,27 +55,29 @@
         "tls_client",
         "clipman",
         "playsound",
     ],
     entry_points={
         "console_scripts": [
             "WEBS = webscout.cli:cli",
-            "webscout-ai-phindsearch = webscout.AI:phindsearch",
-            "webscout-ai-yepchat = webscout.AI:yepchat",
-            "webscout-ai = webscout.AI:cli",
-            "webscout-llm = webscout.LLM:chat",
+            "webscout = webscout.webai:main",
         ],
     },
     extras_require={
         "dev": [
             "ruff>=0.1.6",
             "pytest>=7.4.2",
         ],
+        "local": [
+            'llama-cpp-python',
+            'colorama',
+            'numpy',
+        ],
     },
-    license='HelpingAI Simplified Universal License',
+    license="HelpingAI Simplified Universal License",
     project_urls={
-        'Documentation': 'https://github.com/OE-LUCIFER/Webscout/wiki',
-        'Source': 'https://github.com/OE-LUCIFER/Webscout',
-        'Tracker': 'https://github.com/OE-LUCIFER/Webscout/issues',
-        'YouTube': 'https://youtube.com/@OEvortex',
+        "Documentation": "https://github.com/OE-LUCIFER/Webscout/wiki",
+        "Source": "https://github.com/OE-LUCIFER/Webscout",
+        "Tracker": "https://github.com/OE-LUCIFER/Webscout/issues",
+        "YouTube": "https://youtube.com/@OEvortex",
     },
-)
+)
```

### Comparing `webscout-2.2/webscout/AIauto.py` & `webscout-2.2b0/webscout/AIauto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,82 @@
-from webscout.AI import Provider, AsyncProvider
-from webscout.AI import OPENGPT, AsyncOPENGPT
-from webscout.AI import KOBOLDAI, AsyncKOBOLDAI
-from webscout.AI import PhindSearch, AsyncPhindSearch
-from webscout.AI import LLAMA2, AsyncLLAMA2
-from webscout.AI import BLACKBOXAI, AsyncBLACKBOXAI
-from webscout.AI import PERPLEXITY
-from webscout.AI import ThinkAnyAI
-from webscout.AI import YouChat
-from webscout.AI import YEPCHAT
+from webscout.AIbase import Provider, AsyncProvider
+from webscout import OPENGPT, AsyncOPENGPT
+from webscout import KOBOLDAI, AsyncKOBOLDAI
+from webscout import PhindSearch, AsyncPhindSearch
+from webscout import LLAMA2, AsyncLLAMA2
+from webscout import BLACKBOXAI, AsyncBLACKBOXAI
+from webscout import PERPLEXITY
+from webscout import ThinkAnyAI
+from webscout import YouChat
+from webscout import YEPCHAT
+from webscout.AIbase import Provider, AsyncProvider
+from webscout import KOBOLDAI, AsyncKOBOLDAI
+from webscout import PhindSearch, AsyncPhindSearch
+from webscout import LLAMA2, AsyncLLAMA2
+from webscout import BLACKBOXAI, AsyncBLACKBOXAI
+from webscout import PERPLEXITY
+from webscout import ThinkAnyAI
+from webscout import YouChat
+from webscout import YEPCHAT, AsyncYEPCHAT
+from webscout import LEO, AsyncLEO
+from webscout import GROQ, AsyncGROQ
+from webscout import OPENAI, AsyncOPENAI
+from webscout import REKA
+from webscout import Xjai
+from webscout import Berlin4h
+from webscout import ChatGPTUK
 from webscout.g4f import GPT4FREE, AsyncGPT4FREE
 from webscout.g4f import TestProviders
 from webscout.exceptions import AllProvidersFailure
 from webscout.async_providers import mapper as async_provider_map
 from typing import AsyncGenerator
 
 from typing import Union
 from typing import Any
 import logging
 
 
 provider_map: dict[
-    str, Union[OPENGPT, KOBOLDAI, PhindSearch, LLAMA2, BLACKBOXAI, PERPLEXITY, GPT4FREE, ThinkAnyAI, YEPCHAT, YouChat]
+    str, Union[    ThinkAnyAI,
+    Xjai,
+    LLAMA2,
+    AsyncLLAMA2,
+    LEO,
+    AsyncLEO,
+    KOBOLDAI,
+    AsyncKOBOLDAI,
+    OPENGPT,
+    AsyncOPENGPT,
+    PERPLEXITY,
+    BLACKBOXAI,
+    AsyncBLACKBOXAI,
+    PhindSearch,
+    AsyncPhindSearch,
+    YEPCHAT,
+    AsyncYEPCHAT,
+    YouChat,
+    Berlin4h,
+    ChatGPTUK,]
 ] = {
     "PhindSearch": PhindSearch,
     "perplexity": PERPLEXITY,
     "opengpt": OPENGPT,
     "koboldai": KOBOLDAI,
     "llama2": LLAMA2,
     "blackboxai": BLACKBOXAI,
     "gpt4free": GPT4FREE,
     "thinkany": ThinkAnyAI,
     "yepchat": YEPCHAT,
     "you": YouChat,
+    "leo": LEO,
+    "xjai": Xjai,
+    "berlin4h": Berlin4h,
+    "chatgptuk": ChatGPTUK,
+    "gpt4free": GPT4FREE,
+    
 }
 
 
 class AUTO(Provider):
     def __init__(
         self,
         is_conversation: bool = True,
@@ -109,21 +150,21 @@
             "prompt": prompt,
             "stream": stream,
             "raw": raw,
             "optimizer": optimizer,
             "conversationally": conversationally,
         }
 
-        # tgpt-based providers
+        # webscout-based providers
         for provider_name, provider_obj in provider_map.items():
             # continue
             if provider_name in self.exclude:
                 continue
             try:
-                self.provider_name = f"tgpt-{provider_name}"
+                self.provider_name = f"webscout-{provider_name}"
                 self.provider = provider_obj(
                     is_conversation=self.is_conversation,
                     max_tokens=self.max_tokens,
                     timeout=self.timeout,
                     intro=self.intro,
                     filepath=self.filepath,
                     update_file=self.update_file,
```

### Comparing `webscout-2.2/webscout/AIbase.py` & `webscout-2.2b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/AIutel.py` & `webscout-2.2b0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/DWEBS.py` & `webscout-2.2b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/LLM.py` & `webscout-2.2b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Berlin4h.py` & `webscout-2.2b0/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Blackboxai.py` & `webscout-2.2b0/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/ChatGPTUK.py` & `webscout-2.2b0/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Cohere.py` & `webscout-2.2b0/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Gemini.py` & `webscout-2.2b0/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Groq.py` & `webscout-2.2b0/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Koboldai.py` & `webscout-2.2b0/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Leo.py` & `webscout-2.2b0/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Llama2.py` & `webscout-2.2b0/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/OpenGPT.py` & `webscout-2.2b0/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Openai.py` & `webscout-2.2b0/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Perplexity.py` & `webscout-2.2b0/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Phind.py` & `webscout-2.2b0/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Reka.py` & `webscout-2.2b0/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/ThinkAnyAI.py` & `webscout-2.2b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Xjai.py` & `webscout-2.2b0/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Yepchat.py` & `webscout-2.2b0/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/Youchat.py` & `webscout-2.2b0/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/Provider/__init__.py` & `webscout-2.2b0/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/__init__.py` & `webscout-2.2b0/webscout/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Webscout.
 
-Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Search for anything using the Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 """
 # webscout/__init__.py
 
-from .webscout_search import WEBS 
-from .webscout_search_async import AsyncWEBS 
+from .webscout_search import WEBS
+from .webscout_search_async import AsyncWEBS
 from .version import __version__
-from .DWEBS import DeepWEBS 
+from .DWEBS import DeepWEBS
 from .transcriber import transcriber
-from .voice import play_audio
+from .voice import play_audio, talk
+from .tempid import Client as TempMailClient, TemporaryPhoneNumber
+from .models import MapsResult
+from .LLM import LLM
+from .Local import *
 import g4f
 # Import provider classes for direct access
 from .Provider import (
     ThinkAnyAI,
     Xjai,
     LLAMA2,
     AsyncLLAMA2,
@@ -70,21 +74,27 @@
     provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
 
 # Add all the provider classes you want to directly import to __all__
 __all__ = [
-    "WEBS", 
-    "AsyncWEBS", 
-    "__version__", 
-    "cli", 
-    "DeepWEBS", 
-    "transcriber", 
+    "WEBS",
+    "AsyncWEBS",
+    "__version__",
+    "DeepWEBS",
+    "transcriber",
     "play_audio",
+    "talk",
+    "TempMailClient", 
+    "TemporaryPhoneNumber",
+    "MapsResult",
+    "LLM",
+    "Model",
+    "Thread",
 
     # AI Providers
     "ThinkAnyAI",
     "Xjai",
     "LLAMA2",
     "AsyncLLAMA2",
     "Cohere",
```

### Comparing `webscout-2.2/webscout/async_providers.py` & `webscout-2.2b0/webscout/async_providers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from webscout.AI import AsyncPhindSearch
-from webscout.AI import AsyncYEPCHAT
-from webscout.AI import AsyncOPENGPT
-from webscout.AI import AsyncOPENAI
-from webscout.AI import AsyncLLAMA2
-from webscout.AI import AsyncLEO
-from webscout.AI import AsyncKOBOLDAI
-from webscout.AI import AsyncGROQ
-from webscout.AI import AsyncBLACKBOXAI
+from webscout import AsyncPhindSearch
+from webscout import AsyncYEPCHAT
+from webscout import AsyncOPENGPT
+from webscout import AsyncOPENAI
+from webscout import AsyncLLAMA2
+from webscout import AsyncLEO
+from webscout import AsyncKOBOLDAI
+from webscout import AsyncGROQ
+from webscout import AsyncBLACKBOXAI
 from webscout.g4f import AsyncGPT4FREE
 
 mapper: dict[str, object] = {
     "phind": AsyncPhindSearch,
     "opengpt": AsyncOPENGPT,
     "koboldai": AsyncKOBOLDAI,
     "blackboxai": AsyncBLACKBOXAI,
```

### Comparing `webscout-2.2/webscout/cli.py` & `webscout-2.2b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/g4f.py` & `webscout-2.2b0/webscout/g4f.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,16 +223,16 @@
     def __init__(
         self,
         provider: str = default_provider,
         is_conversation: bool = True,
         auth: str = None,
         max_tokens: int = 600,
         model: str = None,
-        chat_completion: bool = False,
-        ignore_working: bool = False,
+        chat_completion: bool = True,
+        ignore_working: bool = True,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
```

### Comparing `webscout-2.2/webscout/models.py` & `webscout-2.2b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/tempid.py` & `webscout-2.2b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/transcriber.py` & `webscout-2.2b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/utils.py` & `webscout-2.2b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/voice.py` & `webscout-2.2b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/webai.py` & `webscout-2.2b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/webscout_search.py` & `webscout-2.2b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout/webscout_search_async.py` & `webscout-2.2b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2/webscout.egg-info/PKG-INFO` & `webscout-2.2b0/webscout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.2
-Summary: Search for anything using the Google, DuckDuckGo, phind.com. Also containes AI models, can transcribe yt videos, temporary email and phone number generation, have TTS support and webai(terminal gpt and open interpeter)
+Version: 2.2b0
+Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
 Project-URL: YouTube, https://youtube.com/@OEvortex
@@ -32,15 +32,14 @@
 Requires-Dist: selenium
 Requires-Dist: tqdm
 Requires-Dist: webdriver-manager
 Requires-Dist: halo>=0.0.31
 Requires-Dist: g4f>=0.2.2.3
 Requires-Dist: rich
 Requires-Dist: python-dotenv
-Requires-Dist: Helpingai-T2
 Requires-Dist: beautifulsoup4
 Requires-Dist: markdownify
 Requires-Dist: pydantic
 Requires-Dist: requests
 Requires-Dist: sse_starlette
 Requires-Dist: termcolor
 Requires-Dist: tiktoken
@@ -51,14 +50,18 @@
 Requires-Dist: GoogleBard1>=2.1.4
 Requires-Dist: tls_client
 Requires-Dist: clipman
 Requires-Dist: playsound
 Provides-Extra: dev
 Requires-Dist: ruff>=0.1.6; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
+Provides-Extra: local
+Requires-Dist: llama-cpp-python; extra == "local"
+Requires-Dist: colorama; extra == "local"
+Requires-Dist: numpy; extra == "local"
 
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/devsdocode"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.2 Summary: Search for anything
-using the Google, DuckDuckGo, phind.com. Also containes AI models, can
-transcribe yt videos, temporary email and phone number generation, have TTS
-support and webai(terminal gpt and open interpeter) Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Metadata-Version: 2.1 Name: webscout Version: 2.2b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, and webai (terminal gpt and open interpreter). Author: OEvortex
+Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
+License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
 https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License ::
 Other/Proprietary License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -17,21 +17,23 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
 :: Software Development :: Libraries :: Python Modules Description-Content-
 Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
-Dist: Helpingai-T2 Requires-Dist: beautifulsoup4 Requires-Dist: markdownify
-Requires-Dist: pydantic Requires-Dist: requests Requires-Dist: sse_starlette
-Requires-Dist: termcolor Requires-Dist: tiktoken Requires-Dist: tldextract
-Requires-Dist: orjson Requires-Dist: PyYAML Requires-Dist: appdirs Requires-
-Dist: GoogleBard1>=2.1.4 Requires-Dist: tls_client Requires-Dist: clipman
-Requires-Dist: playsound Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra
-== "dev" Requires-Dist: pytest>=7.4.2; extra == "dev"
+Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
+Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
+Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
+Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: playsound
+Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra == "dev" Requires-Dist:
+pytest>=7.4.2; extra == "dev" Provides-Extra: local Requires-Dist: llama-cpp-
+python; extra == "local" Requires-Dist: colorama; extra == "local" Requires-
+Dist: numpy; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
  _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using the Google, DuckDuckGo,
 phind.com. Also containes AI models, can transcribe yt videos, temporary email
```

### Comparing `webscout-2.2/webscout.egg-info/SOURCES.txt` & `webscout-2.2b0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

