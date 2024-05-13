# Comparing `tmp/webscout-2.2b0.tar.gz` & `tmp/webscout-2.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-2.2b0.tar", last modified: Mon May 13 07:37:06 2024, max compression
+gzip compressed data, was "webscout-2.3b0.tar", last modified: Mon May 13 08:26:00 2024, max compression
```

## Comparing `webscout-2.2b0.tar` & `webscout-2.3b0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.385669 webscout-2.2b0/
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.119052 webscout-2.2b0/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.136053 webscout-2.2b0/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.296483 webscout-2.2b0/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.479268 webscout-2.2b0/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.2b0/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.2b0/LICENSE.md
--rw-rw-rw-   0        0        0    46603 2024-05-13 07:37:06.381673 webscout-2.2b0/PKG-INFO
--rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.2b0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 07:37:06.385669 webscout-2.2b0/setup.cfg
--rw-rw-rw-   0        0        0     2696 2024-05-13 07:35:11.000000 webscout-2.2b0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:05.695582 webscout-2.2b0/webscout/
--rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.2b0/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.2b0/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.290314 webscout-2.2b0/webscout/Provider/
--rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.2b0/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.2b0/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.2b0/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.2b0/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.2b0/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.2b0/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.2b0/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.2b0/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.2b0/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.2b0/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.2b0/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.2b0/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.2b0/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.2b0/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.2b0/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.2b0/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.2b0/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.2b0/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.2b0/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     2595 2024-05-13 07:31:21.000000 webscout-2.2b0/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.2b0/webscout/async_providers.py
--rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.2b0/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.2b0/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.2b0/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.2b0/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.2b0/webscout/voice.py
--rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.2b0/webscout/webai.py
--rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.2b0/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.2b0/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:06.376671 webscout-2.2b0/webscout.egg-info/
--rw-rw-rw-   0        0        0    46603 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1592 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      366 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-13 07:37:04.000000 webscout-2.2b0/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.429375 webscout-2.3b0/
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.019969 webscout-2.3b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.055985 webscout-2.3b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.089983 webscout-2.3b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.103987 webscout-2.3b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-2.3b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-2.3b0/LICENSE.md
+-rw-rw-rw-   0        0        0    46603 2024-05-13 08:26:00.421374 webscout-2.3b0/PKG-INFO
+-rw-rw-rw-   0        0        0    44185 2024-05-12 05:27:05.000000 webscout-2.3b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:26:00.429375 webscout-2.3b0/setup.cfg
+-rw-rw-rw-   0        0        0     2696 2024-05-13 08:03:16.000000 webscout-2.3b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.231150 webscout-2.3b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-2.3b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33266 2024-05-12 05:18:53.000000 webscout-2.3b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     1910 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.387383 webscout-2.3b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-2.3b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-2.3b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-2.3b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-2.3b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-2.3b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-2.3b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-2.3b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-2.3b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-2.3b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-2.3b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-2.3b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-2.3b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-2.3b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-2.3b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-2.3b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-2.3b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-2.3b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-11 08:21:09.000000 webscout-2.3b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1318 2024-05-12 05:15:53.000000 webscout-2.3b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     2256 2024-05-13 08:07:51.000000 webscout-2.3b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-2.3b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    17059 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-2.3b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-2.3b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-2.3b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-11 09:00:53.000000 webscout-2.3b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-2.3b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    84668 2024-05-12 05:18:15.000000 webscout-2.3b0/webscout/webai.py
+-rw-rw-rw-   0        0        0     3159 2024-05-10 15:13:22.000000 webscout-2.3b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    42902 2024-05-10 04:39:59.000000 webscout-2.3b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:26:00.395371 webscout-2.3b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    46603 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1592 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      366 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-13 08:25:59.000000 webscout-2.3b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-2.2b0/DeepWEBS/documents/query_results_extractor.py` & `webscout-2.3b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-2.3b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/networks/filepath_converter.py` & `webscout-2.3b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/networks/google_searcher.py` & `webscout-2.3b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/networks/network_configs.py` & `webscout-2.3b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/networks/webpage_fetcher.py` & `webscout-2.3b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/utilsdw/enver.py` & `webscout-2.3b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/DeepWEBS/utilsdw/logger.py` & `webscout-2.3b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/LICENSE.md` & `webscout-2.3b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/PKG-INFO` & `webscout-2.3b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.2b0
+Version: 2.3b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.2b0 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
 anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
 transcribe yt videos, temporary email and phone number generation, has TTS
 support, and webai (terminal gpt and open interpreter). Author: OEvortex
 Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
 License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
```

### Comparing `webscout-2.2b0/README.md` & `webscout-2.3b0/README.md`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/setup.py` & `webscout-2.3b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="2.2-beta",
+    version="2.3-beta",
     description="Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-2.2b0/webscout/AIauto.py` & `webscout-2.3b0/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/AIbase.py` & `webscout-2.3b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/AIutel.py` & `webscout-2.3b0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/DWEBS.py` & `webscout-2.3b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/LLM.py` & `webscout-2.3b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Berlin4h.py` & `webscout-2.3b0/webscout/Provider/Berlin4h.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Blackboxai.py` & `webscout-2.3b0/webscout/Provider/Blackboxai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/ChatGPTUK.py` & `webscout-2.3b0/webscout/Provider/ChatGPTUK.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Cohere.py` & `webscout-2.3b0/webscout/Provider/Cohere.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Gemini.py` & `webscout-2.3b0/webscout/Provider/Gemini.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Groq.py` & `webscout-2.3b0/webscout/Provider/Groq.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Koboldai.py` & `webscout-2.3b0/webscout/Provider/Koboldai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Leo.py` & `webscout-2.3b0/webscout/Provider/Leo.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Llama2.py` & `webscout-2.3b0/webscout/Provider/Llama2.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/OpenGPT.py` & `webscout-2.3b0/webscout/Provider/OpenGPT.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Openai.py` & `webscout-2.3b0/webscout/Provider/Openai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Perplexity.py` & `webscout-2.3b0/webscout/Provider/Perplexity.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Phind.py` & `webscout-2.3b0/webscout/Provider/Phind.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Reka.py` & `webscout-2.3b0/webscout/Provider/Reka.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/ThinkAnyAI.py` & `webscout-2.3b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Xjai.py` & `webscout-2.3b0/webscout/Provider/Xjai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Yepchat.py` & `webscout-2.3b0/webscout/Provider/Yepchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/Youchat.py` & `webscout-2.3b0/webscout/Provider/Youchat.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/Provider/__init__.py` & `webscout-2.3b0/webscout/Provider/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/__init__.py` & `webscout-2.3b0/webscout/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,127 +1,120 @@
-"""Webscout.
-
-Search for anything using the Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
-"""
-# webscout/__init__.py
-
 from .webscout_search import WEBS
 from .webscout_search_async import AsyncWEBS
 from .version import __version__
 from .DWEBS import DeepWEBS
 from .transcriber import transcriber
-from .voice import play_audio, talk
+from .voice import play_audio
 from .tempid import Client as TempMailClient, TemporaryPhoneNumber
-from .models import MapsResult
 from .LLM import LLM
-from .Local import *
+# Import Localai models and utilities directly
+from .Localai import *
 import g4f
 # Import provider classes for direct access
 from .Provider import (
-    ThinkAnyAI,
-    Xjai,
-    LLAMA2,
-    AsyncLLAMA2,
-    Cohere,
-    REKA,
-    GROQ,
-    AsyncGROQ,
-    OPENAI,
-    AsyncOPENAI,
-    LEO,
-    AsyncLEO,
-    KOBOLDAI,
-    AsyncKOBOLDAI,
-    OPENGPT,
-    AsyncOPENGPT,
-    PERPLEXITY,
-    BLACKBOXAI,
-    AsyncBLACKBOXAI,
-    PhindSearch,
-    AsyncPhindSearch,
-    YEPCHAT,
-    AsyncYEPCHAT,
-    YouChat,
-    GEMINI,
-    Berlin4h,
-    ChatGPTUK,
+   ThinkAnyAI,
+   Xjai,
+   LLAMA2, 
+   AsyncLLAMA2,
+   Cohere,
+   REKA,
+   GROQ,
+   AsyncGROQ,
+   OPENAI,
+   AsyncOPENAI,
+   LEO,
+   AsyncLEO,
+   KOBOLDAI,
+   AsyncKOBOLDAI,
+   OPENGPT,
+   AsyncOPENGPT,
+   PERPLEXITY,
+   BLACKBOXAI,
+   AsyncBLACKBOXAI,
+   PhindSearch,
+   AsyncPhindSearch,
+   YEPCHAT,
+   AsyncYEPCHAT,
+   YouChat,
+   GEMINI,
+   Berlin4h,
+   ChatGPTUK,
 )
 
 __repo__ = "https://github.com/OE-LUCIFER/Webscout"
 
 webai = [
-    "leo",
-    "openai",
-    "opengpt",
-    "koboldai",
-    "gemini",
-    "phind",
-    "blackboxai",
-    "g4fauto",
-    "perplexity",
-    "groq",
-    "reka",
-    "cohere",
-    "yepchat",
-    "you",
-    "xjai",
-    "thinkany",
-    "berlin4h",
-    "chatgptuk",
-    "auto",
+   "leo",
+   "openai",
+   "opengpt",
+   "koboldai",
+   "gemini",
+   "phind",
+   "blackboxai",
+   "g4fauto",
+   "perplexity",
+   "groq",
+   "reka",
+   "cohere",
+   "yepchat",
+   "you",
+   "xjai",
+   "thinkany",
+   "berlin4h",
+   "chatgptuk",
+   "auto",
 ]
 
 gpt4free_providers = [
-    provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
+   provider.__name__ for provider in g4f.Provider.__providers__  # if provider.working
 ]
 
 available_providers = webai + gpt4free_providers
 
-# Add all the provider classes you want to directly import to __all__
+# Add all the provider classes, Localai models, Thread, and Model to __all__
 __all__ = [
-    "WEBS",
-    "AsyncWEBS",
-    "__version__",
-    "DeepWEBS",
-    "transcriber",
-    "play_audio",
-    "talk",
-    "TempMailClient", 
-    "TemporaryPhoneNumber",
-    "MapsResult",
-    "LLM",
-    "Model",
-    "Thread",
-
-    # AI Providers
-    "ThinkAnyAI",
-    "Xjai",
-    "LLAMA2",
-    "AsyncLLAMA2",
-    "Cohere",
-    "REKA",
-    "GROQ",
-    "AsyncGROQ",
-    "OPENAI",
-    "AsyncOPENAI",
-    "LEO",
-    "AsyncLEO",
-    "KOBOLDAI",
-    "AsyncKOBOLDAI",
-    "OPENGPT",
-    "AsyncOPENGPT",
-    "PERPLEXITY",
-    "BLACKBOXAI",
-    "AsyncBLACKBOXAI",
-    "PhindSearch",
-    "AsyncPhindSearch",
-    "YEPCHAT",
-    "AsyncYEPCHAT",
-    "YouChat",
-    "GEMINI",
-    "Berlin4h",
-    "ChatGPTUK",
+   "WEBS",
+   "AsyncWEBS",
+   "__version__",
+   "DeepWEBS",
+   "transcriber",
+   "play_audio",
+   "TempMailClient", 
+   "TemporaryPhoneNumber",
+   "LLM",
+   # Localai models and utilities 
+   "Model",
+   "Thread",
+   "formats", 
+
+   # AI Providers
+   "ThinkAnyAI",
+   "Xjai",
+   "LLAMA2",
+   "AsyncLLAMA2",
+   "Cohere",
+   "REKA",
+   "GROQ",
+   "AsyncGROQ",
+   "OPENAI",
+   "AsyncOPENAI",
+   "LEO",
+   "AsyncLEO",
+   "KOBOLDAI",
+   "AsyncKOBOLDAI",
+   "OPENGPT",
+   "AsyncOPENGPT",
+   "PERPLEXITY",
+   "BLACKBOXAI",
+   "AsyncBLACKBOXAI",
+   "PhindSearch",
+   "AsyncPhindSearch",
+   "YEPCHAT",
+   "AsyncYEPCHAT",
+   "YouChat",
+   "GEMINI",
+   "Berlin4h",
+   "ChatGPTUK",
 ]
 
-# Set up basic logger
 import logging
-logging.getLogger("webscout").addHandler(logging.NullHandler()) 
+logging.getLogger("webscout").addHandler(logging.NullHandler())
```

### Comparing `webscout-2.2b0/webscout/async_providers.py` & `webscout-2.3b0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/cli.py` & `webscout-2.3b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/g4f.py` & `webscout-2.3b0/webscout/g4f.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/models.py` & `webscout-2.3b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/tempid.py` & `webscout-2.3b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/transcriber.py` & `webscout-2.3b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/utils.py` & `webscout-2.3b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/voice.py` & `webscout-2.3b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/webai.py` & `webscout-2.3b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/webscout_search.py` & `webscout-2.3b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout/webscout_search_async.py` & `webscout-2.3b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-2.2b0/webscout.egg-info/PKG-INFO` & `webscout-2.3b0/webscout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 2.2b0
+Version: 2.3b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com. Also contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, and webai (terminal gpt and open interpreter).
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webscout Version: 2.2b0 Summary: Search for
+Metadata-Version: 2.1 Name: webscout Version: 2.3b0 Summary: Search for
 anything using Google, DuckDuckGo, phind.com. Also contains AI models, can
 transcribe yt videos, temporary email and phone number generation, has TTS
 support, and webai (terminal gpt and open interpreter). Author: OEvortex
 Author-email: helpingai5@gmail.com License: HelpingAI Simplified Universal
 License Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
 Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
```

### Comparing `webscout-2.2b0/webscout.egg-info/SOURCES.txt` & `webscout-2.3b0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

