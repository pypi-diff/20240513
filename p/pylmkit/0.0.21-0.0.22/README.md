# Comparing `tmp/pylmkit-0.0.21.tar.gz` & `tmp/pylmkit-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylmkit-0.0.21.tar", last modified: Sun Mar 31 09:19:21 2024, max compression
+gzip compressed data, was "pylmkit-0.0.22.tar", last modified: Mon May 13 14:59:11 2024, max compression
```

## Comparing `pylmkit-0.0.21.tar` & `pylmkit-0.0.22.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.328294 pylmkit-0.0.21/
--rw-rw-rw-   0        0        0    11558 2023-11-18 10:35:19.000000 pylmkit-0.0.21/LICENSE
--rw-rw-rw-   0        0        0    11946 2024-03-31 09:19:21.326299 pylmkit-0.0.21/PKG-INFO
--rw-rw-rw-   0        0        0    11428 2024-03-23 15:40:43.000000 pylmkit-0.0.21/README.md
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.118858 pylmkit-0.0.21/pylmkit/
--rw-rw-rw-   0        0        0      166 2024-03-17 14:32:36.000000 pylmkit-0.0.21/pylmkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.170715 pylmkit-0.0.21/pylmkit/app/
--rw-rw-rw-   0        0        0      114 2024-03-17 13:30:42.000000 pylmkit-0.0.21/pylmkit/app/__init__.py
--rw-rw-rw-   0        0        0        4 2024-02-16 12:05:53.000000 pylmkit-0.0.21/pylmkit/app/agents.py
--rw-rw-rw-   0        0        0     9231 2024-03-31 09:13:12.000000 pylmkit-0.0.21/pylmkit/app/chatdb.py
--rw-rw-rw-   0        0        0    11467 2023-12-02 04:24:22.000000 pylmkit-0.0.21/pylmkit/app/rag.py
--rw-rw-rw-   0        0        0     4175 2023-12-01 08:45:59.000000 pylmkit-0.0.21/pylmkit/app/roleplay.py
--rw-rw-rw-   0        0        0     5025 2024-03-17 12:42:07.000000 pylmkit-0.0.21/pylmkit/app/summary.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.201632 pylmkit-0.0.21/pylmkit/core/
--rw-rw-rw-   0        0        0      104 2023-12-08 09:53:54.000000 pylmkit-0.0.21/pylmkit/core/__init__.py
--rw-rw-rw-   0        0        0    17166 2024-03-31 08:58:43.000000 pylmkit-0.0.21/pylmkit/core/base.py
--rw-rw-rw-   0        0        0     3890 2024-03-31 07:46:35.000000 pylmkit-0.0.21/pylmkit/core/html.py
--rw-rw-rw-   0        0        0     1930 2024-03-31 05:05:43.000000 pylmkit-0.0.21/pylmkit/core/parse.py
--rw-rw-rw-   0        0        0     1378 2024-03-31 09:07:45.000000 pylmkit-0.0.21/pylmkit/core/prompt.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.227563 pylmkit-0.0.21/pylmkit/llms/
--rw-rw-rw-   0        0        0     3359 2023-12-05 13:34:08.000000 pylmkit-0.0.21/pylmkit/llms/__init__.py
--rw-rw-rw-   0        0        0     2947 2023-12-05 15:55:51.000000 pylmkit-0.0.21/pylmkit/llms/_huggingface_llm.py
--rw-rw-rw-   0        0        0     5443 2023-12-05 15:22:21.000000 pylmkit-0.0.21/pylmkit/llms/_spark.py
--rw-rw-rw-   0        0        0     1616 2024-03-23 15:16:31.000000 pylmkit-0.0.21/pylmkit/llms/_zhipu.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.243520 pylmkit-0.0.21/pylmkit/memory/
--rw-rw-rw-   0        0        0      145 2023-11-17 14:17:43.000000 pylmkit-0.0.21/pylmkit/memory/__init__.py
--rw-rw-rw-   0        0        0        4 2023-11-17 07:52:29.000000 pylmkit-0.0.21/pylmkit/memory/memory_type.py
--rw-rw-rw-   0        0        0     2604 2023-11-26 08:21:33.000000 pylmkit-0.0.21/pylmkit/memory/memory_usage.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.263469 pylmkit-0.0.21/pylmkit/perception/
--rw-rw-rw-   0        0        0        0 2023-11-18 01:25:31.000000 pylmkit-0.0.21/pylmkit/perception/__init__.py
--rw-rw-rw-   0        0        0     6659 2024-03-17 12:47:04.000000 pylmkit-0.0.21/pylmkit/perception/directory.py
--rw-rw-rw-   0        0        0     7304 2024-03-17 11:52:32.000000 pylmkit-0.0.21/pylmkit/perception/text.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.277430 pylmkit-0.0.21/pylmkit/tools/
--rw-rw-rw-   0        0        0       25 2024-03-21 16:42:38.000000 pylmkit-0.0.21/pylmkit/tools/__init__.py
--rw-rw-rw-   0        0        0     3312 2024-03-27 15:58:01.000000 pylmkit-0.0.21/pylmkit/tools/executor.py
--rw-rw-rw-   0        0        0     1361 2024-03-29 11:14:08.000000 pylmkit-0.0.21/pylmkit/tools/kit.py
--rw-rw-rw-   0        0        0     1791 2023-11-26 08:24:14.000000 pylmkit-0.0.21/pylmkit/tools/search.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.294384 pylmkit-0.0.21/pylmkit/utils/
--rw-rw-rw-   0        0        0        0 2023-11-26 11:01:32.000000 pylmkit-0.0.21/pylmkit/utils/__init__.py
--rw-rw-rw-   0        0        0     4497 2023-12-09 13:41:51.000000 pylmkit-0.0.21/pylmkit/utils/data_utils.py
--rw-rw-rw-   0        0        0    29548 2024-03-31 07:05:11.000000 pylmkit-0.0.21/pylmkit/utils/db_base.py
--rw-rw-rw-   0        0        0      428 2023-12-01 17:24:46.000000 pylmkit-0.0.21/pylmkit/utils/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.304356 pylmkit-0.0.21/pylmkit/web/
--rw-rw-rw-   0        0        0       47 2024-03-17 14:32:27.000000 pylmkit-0.0.21/pylmkit/web/__init__.py
--rw-rw-rw-   0        0        0     1402 2024-03-31 08:51:10.000000 pylmkit-0.0.21/pylmkit/web/webui.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.139798 pylmkit-0.0.21/pylmkit.egg-info/
--rw-rw-rw-   0        0        0    11946 2024-03-31 09:19:19.000000 pylmkit-0.0.21/pylmkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1033 2024-03-31 09:19:20.000000 pylmkit-0.0.21/pylmkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 09:19:19.000000 pylmkit-0.0.21/pylmkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      150 2024-03-31 09:19:19.000000 pylmkit-0.0.21/pylmkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-31 09:19:19.000000 pylmkit-0.0.21/pylmkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-31 09:19:21.329295 pylmkit-0.0.21/setup.cfg
--rw-rw-rw-   0        0        0     1624 2024-03-31 09:18:20.000000 pylmkit-0.0.21/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 09:19:21.322309 pylmkit-0.0.21/test/
--rw-rw-rw-   0        0        0      656 2024-02-20 14:55:02.000000 pylmkit-0.0.21/test/test_newllm.py
--rw-rw-rw-   0        0        0     2028 2024-02-16 12:46:34.000000 pylmkit-0.0.21/test/test_rag.py
--rw-rw-rw-   0        0        0     1325 2024-02-16 12:16:54.000000 pylmkit-0.0.21/test/test_roleplay.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.144645 pylmkit-0.0.22/
+-rw-rw-rw-   0        0        0    11558 2023-11-18 10:35:19.000000 pylmkit-0.0.22/LICENSE
+-rw-rw-rw-   0        0        0    12119 2024-05-13 14:59:11.142650 pylmkit-0.0.22/PKG-INFO
+-rw-rw-rw-   0        0        0    11601 2024-03-31 09:23:19.000000 pylmkit-0.0.22/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:10.991057 pylmkit-0.0.22/pylmkit/
+-rw-rw-rw-   0        0        0      166 2024-05-02 08:29:50.000000 pylmkit-0.0.22/pylmkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.047907 pylmkit-0.0.22/pylmkit/app/
+-rw-rw-rw-   0        0        0      114 2024-03-17 13:30:42.000000 pylmkit-0.0.22/pylmkit/app/__init__.py
+-rw-rw-rw-   0        0        0    19159 2024-05-13 14:52:56.000000 pylmkit-0.0.22/pylmkit/app/chatdb.py
+-rw-rw-rw-   0        0        0    17019 2024-05-03 03:49:31.000000 pylmkit-0.0.22/pylmkit/app/rag.py
+-rw-rw-rw-   0        0        0     6475 2024-05-03 03:49:45.000000 pylmkit-0.0.22/pylmkit/app/roleplay.py
+-rw-rw-rw-   0        0        0     5004 2024-04-30 12:59:54.000000 pylmkit-0.0.22/pylmkit/app/summary.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.066855 pylmkit-0.0.22/pylmkit/core/
+-rw-rw-rw-   0        0        0      110 2024-05-02 08:29:43.000000 pylmkit-0.0.22/pylmkit/core/__init__.py
+-rw-rw-rw-   0        0        0    19736 2024-05-02 11:27:13.000000 pylmkit-0.0.22/pylmkit/core/base.py
+-rw-rw-rw-   0        0        0      774 2024-04-10 15:42:20.000000 pylmkit-0.0.22/pylmkit/core/flow.py
+-rw-rw-rw-   0        0        0     3890 2024-04-03 16:43:05.000000 pylmkit-0.0.22/pylmkit/core/html.py
+-rw-rw-rw-   0        0        0     5554 2024-05-13 14:51:28.000000 pylmkit-0.0.22/pylmkit/core/prompt.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.085802 pylmkit-0.0.22/pylmkit/llms/
+-rw-rw-rw-   0        0        0     3359 2023-12-05 13:34:08.000000 pylmkit-0.0.22/pylmkit/llms/__init__.py
+-rw-rw-rw-   0        0        0     2947 2023-12-05 15:55:51.000000 pylmkit-0.0.22/pylmkit/llms/_huggingface_llm.py
+-rw-rw-rw-   0        0        0     5443 2023-12-05 15:22:21.000000 pylmkit-0.0.22/pylmkit/llms/_spark.py
+-rw-rw-rw-   0        0        0     1616 2024-03-23 15:16:31.000000 pylmkit-0.0.22/pylmkit/llms/_zhipu.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.090788 pylmkit-0.0.22/pylmkit/memory/
+-rw-rw-rw-   0        0        0      125 2024-05-02 08:34:32.000000 pylmkit-0.0.22/pylmkit/memory/__init__.py
+-rw-rw-rw-   0        0        0     2703 2024-05-02 08:34:23.000000 pylmkit-0.0.22/pylmkit/memory/common.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.102757 pylmkit-0.0.22/pylmkit/perception/
+-rw-rw-rw-   0        0        0        0 2023-11-18 01:25:31.000000 pylmkit-0.0.22/pylmkit/perception/__init__.py
+-rw-rw-rw-   0        0        0     6659 2024-03-17 12:47:04.000000 pylmkit-0.0.22/pylmkit/perception/directory.py
+-rw-rw-rw-   0        0        0     7304 2024-03-17 11:52:32.000000 pylmkit-0.0.22/pylmkit/perception/text.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.121706 pylmkit-0.0.22/pylmkit/tools/
+-rw-rw-rw-   0        0        0     1127 2024-05-02 09:01:01.000000 pylmkit-0.0.22/pylmkit/tools/__init__.py
+-rw-rw-rw-   0        0        0     2538 2024-05-03 10:07:23.000000 pylmkit-0.0.22/pylmkit/tools/action.py
+-rw-rw-rw-   0        0        0     2654 2024-05-03 04:31:05.000000 pylmkit-0.0.22/pylmkit/tools/common.py
+-rw-rw-rw-   0        0        0     4766 2024-05-13 14:57:19.000000 pylmkit-0.0.22/pylmkit/tools/executor.py
+-rw-rw-rw-   0        0        0     3965 2024-05-03 11:15:58.000000 pylmkit-0.0.22/pylmkit/tools/kit.py
+-rw-rw-rw-   0        0        0     2828 2024-05-02 12:11:46.000000 pylmkit-0.0.22/pylmkit/tools/parse.py
+-rw-rw-rw-   0        0        0     1791 2023-11-26 08:24:14.000000 pylmkit-0.0.22/pylmkit/tools/search.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.127690 pylmkit-0.0.22/pylmkit/utils/
+-rw-rw-rw-   0        0        0        0 2023-11-26 11:01:32.000000 pylmkit-0.0.22/pylmkit/utils/__init__.py
+-rw-rw-rw-   0        0        0     5969 2024-05-02 10:47:19.000000 pylmkit-0.0.22/pylmkit/utils/data_utils.py
+-rw-rw-rw-   0        0        0    29905 2024-05-01 03:47:27.000000 pylmkit-0.0.22/pylmkit/utils/sql_base.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.133676 pylmkit-0.0.22/pylmkit/web/
+-rw-rw-rw-   0        0        0       47 2024-05-02 08:42:06.000000 pylmkit-0.0.22/pylmkit/web/__init__.py
+-rw-rw-rw-   0        0        0    10010 2024-05-03 11:36:28.000000 pylmkit-0.0.22/pylmkit/web/webui.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.019979 pylmkit-0.0.22/pylmkit.egg-info/
+-rw-rw-rw-   0        0        0    12119 2024-05-13 14:59:10.000000 pylmkit-0.0.22/pylmkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1021 2024-05-13 14:59:10.000000 pylmkit-0.0.22/pylmkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:59:10.000000 pylmkit-0.0.22/pylmkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2024-05-13 14:59:10.000000 pylmkit-0.0.22/pylmkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 14:59:10.000000 pylmkit-0.0.22/pylmkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:59:11.144645 pylmkit-0.0.22/setup.cfg
+-rw-rw-rw-   0        0        0     1624 2024-05-13 14:59:04.000000 pylmkit-0.0.22/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:59:11.140655 pylmkit-0.0.22/test/
+-rw-rw-rw-   0        0        0      656 2024-02-20 14:55:02.000000 pylmkit-0.0.22/test/test_newllm.py
+-rw-rw-rw-   0        0        0     2028 2024-02-16 12:46:34.000000 pylmkit-0.0.22/test/test_rag.py
+-rw-rw-rw-   0        0        0     1325 2024-02-16 12:16:54.000000 pylmkit-0.0.22/test/test_roleplay.py
```

### Comparing `pylmkit-0.0.21/LICENSE` & `pylmkit-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/PKG-INFO` & `pylmkit-0.0.22/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylmkit
-Version: 0.0.21
+Version: 0.0.22
 Summary: pylmkit: Help users quickly build practical large model applications!
 Home-page: https://github.com/52phm/pylmkit
 Author: 52phm
 Author-email: 2374521450@qq.com
 License: Apache License-2.0
 Project-URL: Homepage, http://app.pylmkit.cn
 Project-URL: Documentation, http://en.pylmkit.cn
@@ -48,15 +48,18 @@
 <img src="./docs/images/RAG.png" width="500" height="260" alt="PyLMKit RAG" style="display: block; margin-left: auto; margin-right: auto;">
 
 
 ## 长文本摘要
 在一些长篇幅、长文本场景下，由于模型本身或硬件资源受限而无法一次性处理长文本，因此需要通过`分而治之`的思想进行长文本摘要提取。
 
 ## 数据库
-功能更新中....
+与你的结构化数据聊天：支持主流数据库、表格型excel等数据！
+
+- ChatDB：支持数据库问答
+- ChatTable：支持`txt,excel,csv`等`pandas dataframe`表格的问答
 
 ## 智能体
 功能更新中....
 
 # 3.网页端Web
 支持streamlit页面自定义参数交互、对话功能，主要作用用于功能测试和demo演示。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylmkit Version: 0.0.21 Summary: pylmkit: Help
+Metadata-Version: 2.1 Name: pylmkit Version: 0.0.22 Summary: pylmkit: Help
 users quickly build practical large model applications! Home-page: https://
 github.com/52phm/pylmkit Author: 52phm Author-email: 2374521450@qq.com License:
 Apache License-2.0 Project-URL: Homepage, http://app.pylmkit.cn Project-URL:
 Documentation, http://en.pylmkit.cn Project-URL: åºç¨ä¸»é¡µ, http://
 app.pylmkit.cn Project-URL: ä¸­æææ¡£, http://zh.pylmkit.cn Description-
 Content-Type: text/markdown License-File: LICENSE # PyLMKit **pylmkit**
 æ¯ä¸ä¸ªæ¨å¨æå»ºæéæå·æå®ç¨ä»·å¼çå¤§æ¨¡åï¼LMï¼åºç¨ç¨åºçé¡¹ç®ï¼æ¨å¨å¸®å©ç¨æ·å¿«éãçµæ´»ãæéå¯¹æ§å°æå»ºç¬¦åå¶ä¸å¡éæ±ã
@@ -15,16 +15,18 @@
 çº§åè¯åå¥å­ãä¿æç¸åçææï¼ä½ä½¿å®ä»¬æ´æèºãæè¦ä½ åªåå¤æ´æ­£ãæ¹è¿ï¼ä¸è¦åä»»ä½è§£éã
 æçç¬¬ä¸å¥è¯æ¯{query} ``` [PyLMKit RAG]## RAG RAGï¼Retrieval-Augmented
 Generationï¼æ£ç´¢å¢å¼ºçæï¼æ¯ä¸ç§å©ç¨ç¥è¯åºæ£ç´¢çæ¹æ³ï¼æä¾ä¸ç¨æ·æ¥è¯¢ç¸å³çåå®¹ï¼ä»èå¢å¼ºæ¨¡åç­æ¡çåç¡®æ§åç¹å¼æ§ãRAGåæ¬æ¬å°ç¥è¯åºãåºäºç½ç»çç¥è¯åºãè®°å¿ç¥è¯åºåæ°æ®åºç¥è¯åºã
 **PyLMKitè®¾è®¡äºåç§RAGåè½** - åºäºæ¬å°ææ¡£çç¥è¯åºDocRAG -
 åºäºç½é¡µçç¥è¯åºWebRAG - åºäºæ°æ®åºçç¥è¯åºDBRAG -
 åºäºè®°å¿çç¥è¯åºMemoryRAG [PyLMKit RAG]## é¿ææ¬æè¦
 å¨ä¸äºé¿ç¯å¹ãé¿ææ¬åºæ¯ä¸ï¼ç±äºæ¨¡åæ¬èº«æç¡¬ä»¶èµæºåéèæ æ³ä¸æ¬¡æ§å¤çé¿ææ¬ï¼å æ­¤éè¦éè¿`åèæ²»ä¹`çææ³è¿è¡é¿ææ¬æè¦æåã
-## æ°æ®åº åè½æ´æ°ä¸­.... ## æºè½ä½ åè½æ´æ°ä¸­.... #
-3.ç½é¡µç«¯Web
+## æ°æ®åº
+ä¸ä½ çç»æåæ°æ®èå¤©ï¼æ¯æä¸»æµæ°æ®åºãè¡¨æ ¼åexcelç­æ°æ®ï¼
+- ChatDBï¼æ¯ææ°æ®åºé®ç­ - ChatTableï¼æ¯æ`txt,excel,csv`ç­`pandas
+dataframe`è¡¨æ ¼çé®ç­ ## æºè½ä½ åè½æ´æ°ä¸­.... # 3.ç½é¡µç«¯Web
 æ¯æstreamlité¡µé¢èªå®ä¹åæ°äº¤äºãå¯¹è¯åè½ï¼ä¸»è¦ä½ç¨ç¨äºåè½æµè¯ådemoæ¼ç¤ºã
 # 4.API æ´æ°ä¸­ï¼åé¢éç»­æä¾åè½åºç¨çåç«¯APIæ¥å£ã #
 5.å¿«éå¼å§ `PyLMKit`ç®åéæäº`LLM`æ¨¡ååä¸ºï¼ -
 `API`ä»è´¹è°ç¨å - æ¬å°å¼æºæ¨¡åä¸è½½é¨ç½²
 `LLM`æ¨¡åæä¸¤ç§è°ç¨æ¹å¼ï¼ - æ®éæ¨¡å¼ï¼invoke(query) -
 æµå¼æ¨¡å¼ï¼stream(query) ## APIä»£çæ¨¡å ### API KEYéç½®
 **ç¬¬ä¸ç§æ¹æ³**ï¼ä¸ä¸ªæ¹ä¾¿çæ¹æ³æ¯åå»ºä¸ä¸ªåç§°ä¸º`.env`æä»¶ï¼å¹¶å¨å¶ä¸­éç½®ææçAPIå¯é¥ä¿¡æ¯ï¼ä»èæ¹ä¾¿å°ä½¿ç¨ä¸åçæ¨¡åã`.env`æä»¶çæ ¼å¼å¦ä¸ï¼
```

### Comparing `pylmkit-0.0.21/README.md` & `pylmkit-0.0.22/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,18 @@
 <img src="./docs/images/RAG.png" width="500" height="260" alt="PyLMKit RAG" style="display: block; margin-left: auto; margin-right: auto;">
 
 
 ## 长文本摘要
 在一些长篇幅、长文本场景下，由于模型本身或硬件资源受限而无法一次性处理长文本，因此需要通过`分而治之`的思想进行长文本摘要提取。
 
 ## 数据库
-功能更新中....
+与你的结构化数据聊天：支持主流数据库、表格型excel等数据！
+
+- ChatDB：支持数据库问答
+- ChatTable：支持`txt,excel,csv`等`pandas dataframe`表格的问答
 
 ## 智能体
 功能更新中....
 
 # 3.网页端Web
 支持streamlit页面自定义参数交互、对话功能，主要作用用于功能测试和demo演示。
```

#### html2text {}

```diff
@@ -9,16 +9,18 @@
 çº§åè¯åå¥å­ãä¿æç¸åçææï¼ä½ä½¿å®ä»¬æ´æèºãæè¦ä½ åªåå¤æ´æ­£ãæ¹è¿ï¼ä¸è¦åä»»ä½è§£éã
 æçç¬¬ä¸å¥è¯æ¯{query} ``` [PyLMKit RAG]## RAG RAGï¼Retrieval-Augmented
 Generationï¼æ£ç´¢å¢å¼ºçæï¼æ¯ä¸ç§å©ç¨ç¥è¯åºæ£ç´¢çæ¹æ³ï¼æä¾ä¸ç¨æ·æ¥è¯¢ç¸å³çåå®¹ï¼ä»èå¢å¼ºæ¨¡åç­æ¡çåç¡®æ§åç¹å¼æ§ãRAGåæ¬æ¬å°ç¥è¯åºãåºäºç½ç»çç¥è¯åºãè®°å¿ç¥è¯åºåæ°æ®åºç¥è¯åºã
 **PyLMKitè®¾è®¡äºåç§RAGåè½** - åºäºæ¬å°ææ¡£çç¥è¯åºDocRAG -
 åºäºç½é¡µçç¥è¯åºWebRAG - åºäºæ°æ®åºçç¥è¯åºDBRAG -
 åºäºè®°å¿çç¥è¯åºMemoryRAG [PyLMKit RAG]## é¿ææ¬æè¦
 å¨ä¸äºé¿ç¯å¹ãé¿ææ¬åºæ¯ä¸ï¼ç±äºæ¨¡åæ¬èº«æç¡¬ä»¶èµæºåéèæ æ³ä¸æ¬¡æ§å¤çé¿ææ¬ï¼å æ­¤éè¦éè¿`åèæ²»ä¹`çææ³è¿è¡é¿ææ¬æè¦æåã
-## æ°æ®åº åè½æ´æ°ä¸­.... ## æºè½ä½ åè½æ´æ°ä¸­.... #
-3.ç½é¡µç«¯Web
+## æ°æ®åº
+ä¸ä½ çç»æåæ°æ®èå¤©ï¼æ¯æä¸»æµæ°æ®åºãè¡¨æ ¼åexcelç­æ°æ®ï¼
+- ChatDBï¼æ¯ææ°æ®åºé®ç­ - ChatTableï¼æ¯æ`txt,excel,csv`ç­`pandas
+dataframe`è¡¨æ ¼çé®ç­ ## æºè½ä½ åè½æ´æ°ä¸­.... # 3.ç½é¡µç«¯Web
 æ¯æstreamlité¡µé¢èªå®ä¹åæ°äº¤äºãå¯¹è¯åè½ï¼ä¸»è¦ä½ç¨ç¨äºåè½æµè¯ådemoæ¼ç¤ºã
 # 4.API æ´æ°ä¸­ï¼åé¢éç»­æä¾åè½åºç¨çåç«¯APIæ¥å£ã #
 5.å¿«éå¼å§ `PyLMKit`ç®åéæäº`LLM`æ¨¡ååä¸ºï¼ -
 `API`ä»è´¹è°ç¨å - æ¬å°å¼æºæ¨¡åä¸è½½é¨ç½²
 `LLM`æ¨¡åæä¸¤ç§è°ç¨æ¹å¼ï¼ - æ®éæ¨¡å¼ï¼invoke(query) -
 æµå¼æ¨¡å¼ï¼stream(query) ## APIä»£çæ¨¡å ### API KEYéç½®
 **ç¬¬ä¸ç§æ¹æ³**ï¼ä¸ä¸ªæ¹ä¾¿çæ¹æ³æ¯åå»ºä¸ä¸ªåç§°ä¸º`.env`æä»¶ï¼å¹¶å¨å¶ä¸­éç½®ææçAPIå¯é¥ä¿¡æ¯ï¼ä»èæ¹ä¾¿å°ä½¿ç¨ä¸åçæ¨¡åã`.env`æä»¶çæ ¼å¼å¦ä¸ï¼
```

### Comparing `pylmkit-0.0.21/pylmkit/app/summary.py` & `pylmkit-0.0.22/pylmkit/app/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import requests, os
 from tqdm import tqdm
 from concurrent.futures import ThreadPoolExecutor
 
 
 def split_text(text, chunk_size=3000):
     # 将文本分割成指定大小的段落
     return [text[i: i + chunk_size] for i in range(0, len(text), chunk_size)]
```

### Comparing `pylmkit-0.0.21/pylmkit/core/base.py` & `pylmkit-0.0.22/pylmkit/core/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from abc import ABC
+import re
 import time, logging
 import pandas as pd
 from pathlib import Path
-from tqdm import tqdm
 import streamlit as st
-from pylmkit.utils.data_utils import read_yaml, read_json, write_yaml, write_json
-from pylmkit.utils.data_utils import message_as_string, document_as_dict, dict_as_document
-from pylmkit.utils.data_utils import text_as_document
+from pylmkit.utils.data_utils import *
+from pylmkit.core.prompt import *
 from functools import partial
 from pylmkit.core.html import init_css, init_footer, init_logo
 from pylmkit.core.html import _zh, _en
-from pylmkit.core.parse import CodeBlockParse
-from pylmkit.utils.db_base import DBConnector
-from pylmkit.core.prompt import sql_prompt, sql_qa_prompt
+
+logging.basicConfig(
+    level=logging.INFO,
+    format='%(asctime)s - %(name)s.%(filename)s - %(levelname)s - %(lineno)d - %(message)s',
+    datefmt='%Y-%m-%d %H:%M:%S',
+)
 logger = logging.getLogger(__name__)
 
 
 class BaseMemory(object):
     human_prefix: str = "Human"
     ai_prefix: str = "AI"
     system_prefix: str = "System"
@@ -202,48 +203,116 @@
                 input1=_input1,
                 input2=_input2,
                 type=_type,
                 value=value
             )
 
 
-class BaseChatRunnable(object):
+class BaseSQLRunnable(object):
     def __init__(self, model, connector):
         self.model = model
         self.connector = connector
         self.sql_prompt = sql_prompt
         self.sql_qa_prompt = sql_qa_prompt
+        self.chart_prompt = chart_prompt
+        self.select_tool_prompt = select_tool_prompt
+        self.tool_list = [table_list, line_chart, pie_chart, bar_chart, funnel_chart, scatter_chart, text_answer]
+
+    def runnable(self, prompt_list, rollback_num: int = 5, connector: dict = {}):
+        from pylmkit.tools.kit import SQLToolKit
+        res = SQLToolKit.sql_executor(
+            model=self.model,
+            prompt_list=prompt_list,
+            rollback_num=rollback_num,
+            db=self.connector,
+            connector=connector
+        )
+        return res
+
+    def wrapper(self, fun):
+        return partial(fun)
 
-    def runnable(self, query, max_rollback_num: int = 5, code_type: str = 'sql'):
-        runnable_results = {"status": False, "query": None, "result": None, 'error': None}
+
+class BaseAgentParse(object):
+    def __init__(self):
+        pass
+
+    def base(self, command: str, formatter: str, parse_type: str):
+        """解析命令字符串中的特定格式代码块。
+
+        ## 参数
+        command : str
+            包含要解析的代码块的字符串。
+        formatter : str
+            指定要解析的代码块的格式化器，例如'tool'或'python'。
+        parse_type : str
+            指定解析类型，'xml'或'codeblock'。
+
+        ## 返回
+        OutputFormat
+            一个OutputFormat实例，其中包含解析结果的状态、输出和错误信息。
+
+        ## 示例
+        >>> command = "这里是文字<tool>第一个工具内容</tool>这里是文字<tool>第二个工具内容</tool>这里是文字"
+        >>> results = parse(command, 'tool', 'xml')
+        >>> print(results.output)
+        ['第一个工具内容', '第二个工具内容']
+        """
+        from pylmkit.tools.parse import OutputFormat
+        _results = OutputFormat()
+        _results.output = _results.output.copy()
+        if parse_type == 'xml':
+            pattern = f'<{formatter}>(.*?)</{formatter}>'
+        elif parse_type == 'codeblock':
+            pattern = f'```{formatter}\n(.*?)\n```'
+        else:
+            raise TypeError('Type must be specified!')
         try:
-            if max_rollback_num != 0:
-                model_respond = self.model.invoke(query)
-                model_respond = model_respond if isinstance(model_respond, str) else model_respond.content
-                code_query = CodeBlockParse().base(model_respond, code_type)
-                if code_query['status']:
-                    runnable_results['query'] = code_query['output']
-                    code_result = self.connector.run(code_query['output'])  # sql [(列名),(数值记录)]
-                    if code_result['status']:
-                        runnable_results['result'] = code_result['output']
-                        runnable_results['status'] = True
-                        return runnable_results
-                    else:
-                        logging.info('Run error，RollBack...')
-                        return self.runnable(query, max_rollback_num-1, code_type)
-                else:
-                    logging.info('Generate error，RollBack...')
-                    return self.runnable(query, max_rollback_num-1, code_type)
+            matches = re.findall(pattern, command, re.DOTALL)
+            if matches:
+                _results.output = matches
+                _results.status = True
             else:
-                return runnable_results
+                _results.output = []
+            return _results
         except Exception as e:
-            # 这里可以添加更详细的错误处理逻辑
-            logger.info("Try error: " + str(e))
-            runnable_results['error'] = str(e)
-            return runnable_results
+            _results.error = str(e)
+            return _results
+
+
+class BasePromptFlow(object):
+    @classmethod
+    def formatted_str(cls, prompt_list: list, sep: str = '\n') -> str:
+        return f"{sep}".join(prompt_list).strip()
+
+    @classmethod
+    def set_language(cls, lang: str = 'zh') -> str:
+        if lang in ['zh', '中文', '中文简体', '中文繁体', 'china', 'China', 'Chinese', 'chinese', '中国']:
+            return "Please answer in simplified Chinese."
+        else:
+            return "Please answer in English."
+
+    @classmethod
+    def replace_placeholders(cls, template: str, replacements: dict):
+        replacements = {f'{{{key}}}': value for key, value in replacements.items()}
+
+        def replace_placeholder(match):
+            return replacements.get(match.group(0), match.group(0))
+
+        return re.sub(r'\{[a-zA-Z0-9_]+\}', replace_placeholder, template)
+
+    @classmethod
+    def formatted_list(cls, prompt_list: list, sep: str = '1__0__1', **kwargs) -> list:
+        if kwargs:
+            prompt = cls.formatted_str(prompt_list, sep=sep)
+            prompt = cls.replace_placeholders(prompt, kwargs)
+            prompt = prompt.split(sep)
+        else:
+            prompt = prompt_list
+        return prompt
 
 
 class BaseWebUI(object):
     def __init__(self,
                  title=None,
                  page_icon=None,
                  layout="centered",
@@ -266,16 +335,18 @@
         self.logo1 = logo1
         self.logo2 = logo2
         self.greetings = greetings
         self.placeholder = placeholder
         self.refer_name = refer_name
         if language in ['zh', '中国', 'china']:
             self.lang = _zh
+            self.spinner_text = 'PyLMKit：生成中，请稍候...'
         else:
             self.lang = _en
+            self.spinner_text = 'PyLMKit: Generating, please wait...'
         if self.title is None:
             self.title = self.lang.get('_title', '')
         if self.page_icon is None:
             self.page_icon = self.lang.get('_page_icon', None)
         if self.footer_describe is None:
             self.footer_describe = self.lang.get('_footer_describe', '')
         if self.sidebar_title is None:
@@ -302,29 +373,32 @@
             st.chat_message(msg["role"]).write(msg["content"])
             # refer setting
             refer = msg.get("refer", False)
             if refer:
                 with st.expander(label=self.refer_name, expanded=False):
                     st.markdown(refer, unsafe_allow_html=True)
 
-    def _input(self, content, role="user", avatar="😄"):
+    def _input(self, content, role="user", avatar="😄", message_type='messages'):
         st.chat_message(role, avatar=avatar).write(content, unsafe_allow_html=True)
         msg = {"role": role, "content": content}
-        st.session_state.messages.append(msg)
+        st.session_state[message_type].append(msg)
 
     def _output(self, content, refer=None, role="assistant"):
         # st.chat_message(role).write(content, unsafe_allow_html=True)
         with st.chat_message(role):
-            content_placeholder = st.empty()
-            full_content = ""
-            for chunk in str(content):
-                full_content += chunk + ""
-                time.sleep(0.01)
-                content_placeholder.markdown(full_content + "▌")
-            content_placeholder.markdown(full_content)
+            if isinstance(content, dict):
+                st.json(content)
+            else:
+                content_placeholder = st.empty()
+                full_content = ""
+                for chunk in str(content):
+                    full_content += chunk + ""
+                    time.sleep(0.01)
+                    content_placeholder.markdown(full_content + "▌")
+                content_placeholder.markdown(full_content)
 
         if refer:  # refer setting
             with st.expander(label=self.refer_name, expanded=False):
                 st.markdown(refer, unsafe_allow_html=True)
         msg = {"role": role, "content": content, "refer": refer}
         st.session_state.messages.append(msg)
 
@@ -341,37 +415,47 @@
                 st.session_state["output_kwargs"][arg['name']] = output_result[i]
                 if arg['type'] == 'chat':
                     response = output_result[i]
                 if arg['type'] == 'refer':
                     refer = output_result[i]
         return response, refer
 
-    def run(self, obj, input_param: list, output_param: list):
+    def base_run(self, obj, input_param: list, message_type="messages"):
         chat_variable = ""
         obj = self.wrapper(obj)
         for arg in input_param:
             if arg['type'] != 'chat':
                 self.input_kwargs[arg['name']] = generate_input_widget(mode='sidebar', **arg)
             else:
                 chat_variable = arg['name']
         if chat_variable:
             if prompt := st.chat_input(placeholder=self.placeholder):
                 self.input_kwargs[chat_variable] = prompt
-                self._input(content=prompt)
-                with st.spinner('PyLMKit: Generating, please wait...'):  # 正在生成，请稍候...
+                self._input(content=prompt, message_type=message_type)
+                with st.spinner(self.spinner_text):  # 正在生成，请稍候...
                     result = obj(**self.input_kwargs)
-                    response, refer = self.output_parse(output_param, result)
-                    self._output(content=response, refer=refer)
+                    return result, chat_variable
         else:
-            with st.spinner('PyLMKit: Generating, please wait...'):  # 正在生成，请稍候...
+            with st.spinner(self.spinner_text):  # 正在生成，请稍候...
                 result = obj(**self.input_kwargs)
+                return result, chat_variable
+
+    def run(self, obj, input_param: list, output_param: list):
+        result = self.base_run(obj, input_param)
+        if result:
+            result, chat_variable = result
+            if chat_variable:
                 response, refer = self.output_parse(output_param, result)
-                # self._output(content=response, refer=refer)
-                with st.expander(label="output", expanded=True):
-                    st.json(st.session_state["output_kwargs"], expanded=True)
+                self._output(content=response, refer=refer)
+            else:
+                with st.spinner(self.spinner_text):  # 正在生成，请稍候...
+                    response, refer = self.output_parse(output_param, result)
+                    # self._output(content=response, refer=refer)
+                    with st.expander(label="output", expanded=True):
+                        st.json(st.session_state["output_kwargs"], expanded=True)
 
     def wrapper(self, fun):
         return partial(fun)
 
     def param(self, label, type, value, mode='sidebar'):
         input_kwargs = {
             "label": label,
@@ -400,18 +484,7 @@
         #     st.sidebar.title(self.sidebar_title)
         # if self.sidebar_describe:
         #     st.sidebar.markdown(self.sidebar_describe, unsafe_allow_html=True)
         if self.logo2:
             st.markdown(init_logo.format(**self.logo2), unsafe_allow_html=True)
         if self.logo1:
             st.markdown(init_logo.format(**self.logo1), unsafe_allow_html=True)
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `pylmkit-0.0.21/pylmkit/core/html.py` & `pylmkit-0.0.22/pylmkit/core/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 pip install pylmkit -U
 ```
 ''',
     _logo1=input_prompt(
         logo_id="logo1",
         link="https://www.yuque.com/txhy/pylmkit",
         logo_rul="https://img1.baidu.com/it/u=2672705872,739783853&fm=253&fmt=auto&app=138&f=JPEG?w=500&h=500",
-        logo_title="pylmkit"
+        logo_title="PyLMKit"
     ),
     _logo2=input_prompt(
         logo_id="logo2",
         link="https://github.com/52phm/pylmkit",
         logo_rul="https://github.githubassets.com/favicons/favicon.svg",
         logo_title=""
     ),
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 _sidebar_title="PyLMKit", _refer_name="å¼ç¨ä¿¡æ¯",
 _greetings="æ¨å¥½ï¼æè½ä¸ºæ¨åäºä»ä¹?",
 _placeholder="è¯·è¾å¥æ¨çæ¶æ¯...", _footer_describe="Copyright Â© 2023
 PyLMKit | Make with Streamlit", _sidebar_describe=''' å¤§æ¨¡ååºç¨æ¡æ¶ï¼
 ```bash pip install pylmkit -U ``` ''', _logo1=input_prompt( logo_id="logo1",
 link="https://www.yuque.com/txhy/pylmkit", logo_rul="https://img1.baidu.com/it/
 u=2672705872,739783853&fm=253&fmt=auto&app=138&f=JPEG?w=500&h=500",
-logo_title="pylmkit" ), _logo2=input_prompt( logo_id="logo2", link="https://
+logo_title="PyLMKit" ), _logo2=input_prompt( logo_id="logo2", link="https://
 github.com/52phm/pylmkit", logo_rul="https://github.githubassets.com/favicons/
 favicon.svg", logo_title="" ), ) _en = input_prompt( _title="PyLMKit",
 _page_icon="ð", _sidebar_title="ð PyLMKit", _greetings="How can I help
 you?", _placeholder="Your message...", _refer_name="Citation Information",
 _footer_describe="Copyright Â© 2023 PyLMKit | Make with Streamlit",
 _sidebar_describe=''' **pylmkit**: Help users quickly build practical large
 model applications! [pylmkit](https://github.com/52phm/pylmkit) - LICENSE
```

### Comparing `pylmkit-0.0.21/pylmkit/llms/__init__.py` & `pylmkit-0.0.22/pylmkit/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/llms/_huggingface_llm.py` & `pylmkit-0.0.22/pylmkit/llms/_huggingface_llm.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/llms/_spark.py` & `pylmkit-0.0.22/pylmkit/llms/_spark.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/llms/_zhipu.py` & `pylmkit-0.0.22/pylmkit/llms/_zhipu.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/memory/memory_usage.py` & `pylmkit-0.0.22/pylmkit/memory/common.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from pylmkit.core import BaseMemory
+from pylmkit.core.base import BaseMemory
 
 
 class MemoryHistoryLength(BaseMemory):
-    """
-
-    例子
+    """根据历史聊天文本长度截取聊天记忆
+    ## 例子
     >>> from pylmkit.memory import MemoryHistoryLength
     >>> mhl = MemoryHistoryLength(memory_length=100)
     >>> mhl.add(role="user", content="中国首都在哪个城市？")
     >>> mhl.add(role="ai", content="北京")
     >>> mhl.add(role="user", content="广州属于哪个省？")
     >>> mhl.add(role="ai", content="广东")
     >>> print(mhl.get())
@@ -24,15 +23,15 @@
         return history_memory[-self.memory_length:]
 
     def origin_memory(self):
         return self.memory_messages
 
 
 class MemoryConversationsNumber(BaseMemory):
-    """
+    """根据历史聊天轮数来获取聊天记忆
     >>> from pylmkit.memory import MemoryConversationsNumber
     >>> mcn = MemoryConversationsNumber(number=1)
     >>> mcn.add(role="user", content="中国首都在哪个城市？")
     >>> mcn.add(role="ai", content="北京")
     >>> mcn.add(role="user", content="广州市属于中国哪个省？")
     >>> mcn.add(role="ai", content="广东省")
     >>> print(mcn.get())
```

### Comparing `pylmkit-0.0.21/pylmkit/perception/directory.py` & `pylmkit-0.0.22/pylmkit/perception/directory.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/perception/text.py` & `pylmkit-0.0.22/pylmkit/perception/text.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/tools/executor.py` & `pylmkit-0.0.22/pylmkit/tools/executor.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,115 @@
 import functools
 import logging
 import multiprocessing
 import sys
 from io import StringIO
 from typing import Dict, Optional
 from pydantic import Field, BaseModel
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, cast
+
+logging.basicConfig(level=logging.INFO,
+                    format='%(asctime)s - %(name)s.%(filename)s - %(levelname)s - %(lineno)d - %(message)s',
+                    datefmt='%Y-%m-%d %H:%M:%S',
+                    )
 logger = logging.getLogger(__name__)
 
 
-@functools.lru_cache(maxsize=None)
-def warn_once() -> None:
-    """Warn once about the dangers of PythonREPL."""
-    logger.warning("Python REPL can execute arbitrary code. Use with caution.")
+class PythonExecutor(object):
+    def __init__(self):
+        pass
+
+    @classmethod
+    def run(cls, command: str):
+        logger.warning("Python REPL can execute arbitrary code. Use with caution.")
+        results = {'output': None, "status": False, "error": ''}
+        if '```python' in command and '```' in command:
+            command = str(command).split(f'```{command}')[1].split('```')[0]
+        try:
+            exec(command, globals(), locals())
+            results['output'] = globals()['report_folder']
+            results['status'] = True
+        except Exception as e:
+            results['error'] = str(e)
+        return results
+
+    @classmethod
+    def run_mysql(cls, connect, code_text):
+        results = {'output': {"data": None, "columns": []}, "status": False, "error": None}
+        with connect.cursor() as cursor:
+            try:
+                # 执行SQL语句
+                cursor.execute(code_text)
+                results['output']['columns'] = [i[0] for i in cursor.description]
+                # 获取所有记录列表
+                results['output']['data'] = list(cursor.fetchall())
+                results['status'] = True
+            except Exception as e:
+                results['error'] = str(e)
+        return results
+
+
+class Executor(object):
+    def __init__(self):
+        pass
+
+    def runnable(self, executor, max_rollback_num: int = 5):
+        results = {"status": False, "error": None, 'output': []}
+        try:
+            if max_rollback_num:
+                respond = executor
+                if respond['status']:
+                    pass
+                else:
+                    results['error'] = respond.get('error', '')
+                    logging.info(f'Generate {str(executor)} error，RollBack...')
+                    return self.runnable()
+            else:
+                return results
+        except Exception as e:
+            # 这里可以添加更详细的错误处理逻辑
+            logger.error("BaseChartRunnable runnable Fail: " + str(e))
+            results['error'] = str(e)
+            return results
 
 
 class PythonREPL(BaseModel):
     """运行python代码"""
     globals: Optional[Dict] = Field(default_factory=dict, alias="_globals")
     locals: Optional[Dict] = Field(default_factory=dict, alias="_locals")
 
-    @classmethod
     def worker(
-            cls,
+            self,
             command: str,
             globals: Optional[Dict],
             locals: Optional[Dict],
             queue: multiprocessing.Queue,
-    ) -> None:
+    ):
+        results = {'output': "", "status": False, "error": None}
         old_stdout = sys.stdout
         sys.stdout = mystdout = StringIO()
         try:
             exec(command, globals, locals)
             sys.stdout = old_stdout
             queue.put(mystdout.getvalue())
+            results['status'] = True
+            results['output'] = globals.get('report_folder', "")
+            return results
         except Exception as e:
             sys.stdout = old_stdout
             queue.put(repr(e))
+            results['error'] = str(e)
+            return results
 
     def run(self, command: str, timeout: Optional[int] = None) -> str:
         """Run command with own globals/locals and returns anything printed.
         Timeout after the specified number of seconds."""
 
         # Warn against dangers of PythonREPL
-        warn_once()
+        logger.warning("Python REPL can execute arbitrary code. Use with caution.")
 
         queue: multiprocessing.Queue = multiprocessing.Queue()
 
         # Only use multiprocessing if we are enforcing a timeout
         if timeout is not None:
             # create a Process
             p = multiprocessing.Process(
@@ -56,45 +119,10 @@
             p.start()
             # wait for the process to finish or kill it after timeout seconds
             p.join(timeout)
             if p.is_alive():
                 p.terminate()
                 return "Execution timed out"
         else:
-            self.worker(command, self.globals, self.locals, queue)
+            return self.worker(command, self.globals, self.locals, queue)
         # get the result from the worker function
         return queue.get()
-
-
-class Executor(object):
-    def __init__(self):
-        pass
-
-    @classmethod
-    def run_python(cls, code_text: str, timeout: Optional[int] = None):
-        results = {'output': None, "status": False, "error": None}
-        try:
-            results['output'] = PythonREPL().run(command=code_text, timeout=timeout)
-            results['status'] = True
-        except Exception as e:
-            results['error'] = str(e)
-        return results
-
-    @classmethod
-    def run_mysql(cls, connect, code_text):
-        results = {'output': {"data": None, "columns": []}, "status": False, "error": None}
-        with connect.cursor() as cursor:
-            try:
-                # 执行SQL语句
-                cursor.execute(code_text)
-                results['output']['columns'] = [i[0] for i in cursor.description]
-                # 获取所有记录列表
-                results['output']['data'] = list(cursor.fetchall())
-                results['status'] = True
-            except Exception as e:
-                results['error'] = str(e)
-        return results
-
-
-
-
-
```

### Comparing `pylmkit-0.0.21/pylmkit/tools/kit.py` & `pylmkit-0.0.22/pylmkit/tools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import inspect
-from .executor import Executor
 
 
 def tool(func):
+    """工具定义"""
     name = func.__name__
     # 获取函数签名
     signature = inspect.signature(func)
     # 获取参数信息
     param_str = ", ".join([str(param) for param in signature.parameters.values()])
     # 提取返回类型
     return_str = signature.return_annotation
@@ -18,20 +18,13 @@
             if return_str is None:
                 return_str = "-> None"
             else:
                 return_str = "-> " + str(re.search(r"'([\w.]+)'", str(return_str)).group(1))
     else:
         return_str = ''
     describe = (f"({param_str.strip()}) {return_str.strip()} - " +
-                func.__doc__.replace('\n', ' ').replace('    ', ' ').replace('  ', ' ').strip())
+                func.__doc__.replace('\n', ' ').replace('    ', ' ').replace('  ', ' ').strip()
+                if func.__doc__ else f"() - None")
     func.name = name
     func.desc = f"{name}{describe}"
     func.all = f"{name}: {name}{describe}"
     return func
-
-
-@tool
-def write_python_run(code_block):
-    """请写一段Python程序代码内容如下:\n {question}\n 特别注意：必须返回完整的代码,并保持格式正确,且只能返回代码块"""
-
-    results = Executor().run_python(code_block)
-    return results
```

### Comparing `pylmkit-0.0.21/pylmkit/tools/search.py` & `pylmkit-0.0.22/pylmkit/tools/search.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/pylmkit/utils/db_base.py` & `pylmkit-0.0.22/pylmkit/utils/sql_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 """
 参考：https://github.com/eosphoros-ai/DB-GPT  MIT license
 复用DB-GPT数据库基础内容，做自定义调整
 Base class for RDBMS connectors.
 """
-
 from __future__ import annotations
 import re
 import os
 import logging
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Optional, Set, Tuple, cast
 from urllib.parse import quote
 from urllib.parse import quote_plus as urlquote
-
 import sqlalchemy
 import sqlparse
 from sqlalchemy import MetaData, Table, create_engine, inspect, select, text, String
 from sqlalchemy.engine import CursorResult
 from sqlalchemy.exc import ProgrammingError, SQLAlchemyError
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.schema import CreateTable
+from pylmkit.tools.parse import OutputFormat
 
+logging.basicConfig(level=logging.INFO,
+                    format='%(asctime)s - %(name)s.%(filename)s - %(levelname)s - %(lineno)d - %(message)s',
+                    datefmt='%Y-%m-%d %H:%M:%S',
+                    )
 logger = logging.getLogger(__name__)
 
-"""Database information class and database type enumeration."""
-
 
 class DbInfo:
     """Database information class."""
 
     def __init__(self, name, is_file_db: bool = False):
         """Create a new instance of DbInfo."""
         self.name = name
@@ -180,14 +181,23 @@
     def from_uri(
             cls, database_uri: str, engine_args: Optional[dict] = None, **kwargs: Any
     ) -> DBConnector:
         """Construct a SQLAlchemy engine from URI."""
         _engine_args = engine_args or {}
         return cls(create_engine(database_uri, **_engine_args), **kwargs)
 
+    def extract_db_type(self):
+        drivername = self._engine.url.drivername
+        if ":" in drivername:
+            return drivername.split(":")[0]
+        elif "+" in drivername:
+            return drivername.split("+")[0]
+        else:
+            return "sqlite"
+
     @property
     def dialect(self) -> str:
         """Return string representation of dialect to use."""
         return self._engine.dialect.name
 
     def _sync_tables_from_db(self) -> Iterable[str]:
         """Read table information from database."""
@@ -375,15 +385,15 @@
 
         Args:
             query (str): SQL query to run
             fetch (str): fetch type
         """
         result: List[Any] = []
 
-        logger.info(f"Query[{query}]")
+        logger.info(f"Run SQL:\n{query}")
         if not query:
             return result
         cursor = self.session.execute(text(query))
         if cursor.returns_rows:
             if fetch == "all":
                 result = cursor.fetchall()
             elif fetch == "one":
@@ -429,38 +439,37 @@
                 raise ValueError("Fetch parameter must be either 'one' or 'all'")
             field_names = list(cursor.keys())
 
             result = list(result)
             return field_names, result
         return [], None
 
-    def run(self, command: str, fetch: str = "all") -> Dict:
+    def run(self, command: str, fetch: str = "all"):
         """Execute a SQL command and return a string representing the results."""
-        results = {"status": False, "error": None, 'output': None}
-        logger.info("SQL: " + command)
+        results = OutputFormat()
         if not command or len(command) < 0:
             return results
         parsed, ttype, sql_type, table_name = self.__sql_parse(command)
         if ttype == sqlparse.tokens.DML:
             if sql_type == "SELECT":
                 try:
-                    results['output'] = self._query(command, fetch)
-                    results['status'] = True
+                    results.output = self._query(command, fetch)
+                    results.status = True
                 except Exception as e:
-                    results['error'] = str(e)
+                    results.error = str(e)
                 return results
             else:
                 try:
                     self._write(command)
                     select_sql = self.convert_sql_write_to_select(command)
                     logger.info(f"write result query:{select_sql}")
-                    results['output'] = self._query(select_sql)
-                    results['status'] = True
+                    results.output = self._query(select_sql)
+                    results.status = True
                 except Exception as e:
-                    results['error'] = str(e)
+                    results.error = str(e)
                 return results
         else:
             logger.info(
                 "DDL execution determines whether to enable through configuration "
             )
             cursor = self.session.execute(text(command))
             self.session.commit()
@@ -470,32 +479,32 @@
                     field_names = tuple(i[0:] for i in cursor.keys())
                     result = list(result)
                     result.insert(0, field_names)
                     logger.info("DDL Result:" + str(result))
                     if not result:
                         # return self._query(f"SHOW COLUMNS FROM {table_name}")
                         try:
-                            results['output'] = self.get_simple_fields(table_name)
-                            results['status'] = True
+                            results.output = self.get_simple_fields(table_name)
+                            results.status = True
                         except Exception as e:
-                            results['error'] = str(e)
+                            results.error = str(e)
                         return results
-                    results['output'] = result
-                    results['status'] = True
+                    results.output = result
+                    results.status = True
                     return results
                 except Exception as e:
-                    results['error'] = str(e)
+                    results.error = str(e)
                     return results
             else:
                 try:
-                    results['output'] = self.get_simple_fields(table_name)
-                    results['status'] = True
+                    results.output = self.get_simple_fields(table_name)
+                    results.status = True
                     return results
                 except Exception as e:
-                    results['error'] = str(e)
+                    results.error = str(e)
                     return results
 
     def run_to_df(self, command: str, fetch: str = "all"):
         """Execute sql command and return result as dataframe."""
         import pandas as pd
 
         # Pandas has too much dependence and the import time is too long
```

### Comparing `pylmkit-0.0.21/pylmkit.egg-info/PKG-INFO` & `pylmkit-0.0.22/pylmkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylmkit
-Version: 0.0.21
+Version: 0.0.22
 Summary: pylmkit: Help users quickly build practical large model applications!
 Home-page: https://github.com/52phm/pylmkit
 Author: 52phm
 Author-email: 2374521450@qq.com
 License: Apache License-2.0
 Project-URL: Homepage, http://app.pylmkit.cn
 Project-URL: Documentation, http://en.pylmkit.cn
@@ -48,15 +48,18 @@
 <img src="./docs/images/RAG.png" width="500" height="260" alt="PyLMKit RAG" style="display: block; margin-left: auto; margin-right: auto;">
 
 
 ## 长文本摘要
 在一些长篇幅、长文本场景下，由于模型本身或硬件资源受限而无法一次性处理长文本，因此需要通过`分而治之`的思想进行长文本摘要提取。
 
 ## 数据库
-功能更新中....
+与你的结构化数据聊天：支持主流数据库、表格型excel等数据！
+
+- ChatDB：支持数据库问答
+- ChatTable：支持`txt,excel,csv`等`pandas dataframe`表格的问答
 
 ## 智能体
 功能更新中....
 
 # 3.网页端Web
 支持streamlit页面自定义参数交互、对话功能，主要作用用于功能测试和demo演示。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pylmkit Version: 0.0.21 Summary: pylmkit: Help
+Metadata-Version: 2.1 Name: pylmkit Version: 0.0.22 Summary: pylmkit: Help
 users quickly build practical large model applications! Home-page: https://
 github.com/52phm/pylmkit Author: 52phm Author-email: 2374521450@qq.com License:
 Apache License-2.0 Project-URL: Homepage, http://app.pylmkit.cn Project-URL:
 Documentation, http://en.pylmkit.cn Project-URL: åºç¨ä¸»é¡µ, http://
 app.pylmkit.cn Project-URL: ä¸­æææ¡£, http://zh.pylmkit.cn Description-
 Content-Type: text/markdown License-File: LICENSE # PyLMKit **pylmkit**
 æ¯ä¸ä¸ªæ¨å¨æå»ºæéæå·æå®ç¨ä»·å¼çå¤§æ¨¡åï¼LMï¼åºç¨ç¨åºçé¡¹ç®ï¼æ¨å¨å¸®å©ç¨æ·å¿«éãçµæ´»ãæéå¯¹æ§å°æå»ºç¬¦åå¶ä¸å¡éæ±ã
@@ -15,16 +15,18 @@
 çº§åè¯åå¥å­ãä¿æç¸åçææï¼ä½ä½¿å®ä»¬æ´æèºãæè¦ä½ åªåå¤æ´æ­£ãæ¹è¿ï¼ä¸è¦åä»»ä½è§£éã
 æçç¬¬ä¸å¥è¯æ¯{query} ``` [PyLMKit RAG]## RAG RAGï¼Retrieval-Augmented
 Generationï¼æ£ç´¢å¢å¼ºçæï¼æ¯ä¸ç§å©ç¨ç¥è¯åºæ£ç´¢çæ¹æ³ï¼æä¾ä¸ç¨æ·æ¥è¯¢ç¸å³çåå®¹ï¼ä»èå¢å¼ºæ¨¡åç­æ¡çåç¡®æ§åç¹å¼æ§ãRAGåæ¬æ¬å°ç¥è¯åºãåºäºç½ç»çç¥è¯åºãè®°å¿ç¥è¯åºåæ°æ®åºç¥è¯åºã
 **PyLMKitè®¾è®¡äºåç§RAGåè½** - åºäºæ¬å°ææ¡£çç¥è¯åºDocRAG -
 åºäºç½é¡µçç¥è¯åºWebRAG - åºäºæ°æ®åºçç¥è¯åºDBRAG -
 åºäºè®°å¿çç¥è¯åºMemoryRAG [PyLMKit RAG]## é¿ææ¬æè¦
 å¨ä¸äºé¿ç¯å¹ãé¿ææ¬åºæ¯ä¸ï¼ç±äºæ¨¡åæ¬èº«æç¡¬ä»¶èµæºåéèæ æ³ä¸æ¬¡æ§å¤çé¿ææ¬ï¼å æ­¤éè¦éè¿`åèæ²»ä¹`çææ³è¿è¡é¿ææ¬æè¦æåã
-## æ°æ®åº åè½æ´æ°ä¸­.... ## æºè½ä½ åè½æ´æ°ä¸­.... #
-3.ç½é¡µç«¯Web
+## æ°æ®åº
+ä¸ä½ çç»æåæ°æ®èå¤©ï¼æ¯æä¸»æµæ°æ®åºãè¡¨æ ¼åexcelç­æ°æ®ï¼
+- ChatDBï¼æ¯ææ°æ®åºé®ç­ - ChatTableï¼æ¯æ`txt,excel,csv`ç­`pandas
+dataframe`è¡¨æ ¼çé®ç­ ## æºè½ä½ åè½æ´æ°ä¸­.... # 3.ç½é¡µç«¯Web
 æ¯æstreamlité¡µé¢èªå®ä¹åæ°äº¤äºãå¯¹è¯åè½ï¼ä¸»è¦ä½ç¨ç¨äºåè½æµè¯ådemoæ¼ç¤ºã
 # 4.API æ´æ°ä¸­ï¼åé¢éç»­æä¾åè½åºç¨çåç«¯APIæ¥å£ã #
 5.å¿«éå¼å§ `PyLMKit`ç®åéæäº`LLM`æ¨¡ååä¸ºï¼ -
 `API`ä»è´¹è°ç¨å - æ¬å°å¼æºæ¨¡åä¸è½½é¨ç½²
 `LLM`æ¨¡åæä¸¤ç§è°ç¨æ¹å¼ï¼ - æ®éæ¨¡å¼ï¼invoke(query) -
 æµå¼æ¨¡å¼ï¼stream(query) ## APIä»£çæ¨¡å ### API KEYéç½®
 **ç¬¬ä¸ç§æ¹æ³**ï¼ä¸ä¸ªæ¹ä¾¿çæ¹æ³æ¯åå»ºä¸ä¸ªåç§°ä¸º`.env`æä»¶ï¼å¹¶å¨å¶ä¸­éç½®ææçAPIå¯é¥ä¿¡æ¯ï¼ä»èæ¹ä¾¿å°ä½¿ç¨ä¸åçæ¨¡åã`.env`æä»¶çæ ¼å¼å¦ä¸ï¼
```

### Comparing `pylmkit-0.0.21/pylmkit.egg-info/SOURCES.txt` & `pylmkit-0.0.22/pylmkit.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 pylmkit/__init__.py
 pylmkit.egg-info/PKG-INFO
 pylmkit.egg-info/SOURCES.txt
 pylmkit.egg-info/dependency_links.txt
 pylmkit.egg-info/requires.txt
 pylmkit.egg-info/top_level.txt
 pylmkit/app/__init__.py
-pylmkit/app/agents.py
 pylmkit/app/chatdb.py
 pylmkit/app/rag.py
 pylmkit/app/roleplay.py
 pylmkit/app/summary.py
 pylmkit/core/__init__.py
 pylmkit/core/base.py
+pylmkit/core/flow.py
 pylmkit/core/html.py
-pylmkit/core/parse.py
 pylmkit/core/prompt.py
 pylmkit/llms/__init__.py
 pylmkit/llms/_huggingface_llm.py
 pylmkit/llms/_spark.py
 pylmkit/llms/_zhipu.py
 pylmkit/memory/__init__.py
-pylmkit/memory/memory_type.py
-pylmkit/memory/memory_usage.py
+pylmkit/memory/common.py
 pylmkit/perception/__init__.py
 pylmkit/perception/directory.py
 pylmkit/perception/text.py
 pylmkit/tools/__init__.py
+pylmkit/tools/action.py
+pylmkit/tools/common.py
 pylmkit/tools/executor.py
 pylmkit/tools/kit.py
+pylmkit/tools/parse.py
 pylmkit/tools/search.py
 pylmkit/utils/__init__.py
 pylmkit/utils/data_utils.py
-pylmkit/utils/db_base.py
-pylmkit/utils/logging.py
+pylmkit/utils/sql_base.py
 pylmkit/web/__init__.py
 pylmkit/web/webui.py
 test/test_newllm.py
 test/test_rag.py
 test/test_roleplay.py
```

### Comparing `pylmkit-0.0.21/setup.py` & `pylmkit-0.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pylmkit',  # 对外我们模块的名字
     author='52phm',  # 作者
     author_email='2374521450@qq.com',  # 作者邮箱
-    version='0.0.21',  # 版本号
+    version='0.0.22',  # 版本号
     description='pylmkit: Help users quickly build practical large model applications!',  # 项目摘要
     long_description=long_description,  # 项目介绍
     long_description_content_type="text/markdown",
     url="https://github.com/52phm/pylmkit",  # 程序主页地址
     packages=find_packages(),  # 要发布的模块
     license="Apache License-2.0",  # 协议（请注意按实际情况选择不同的协议），可选
     # 此处添加任意多个项目链接
```

### Comparing `pylmkit-0.0.21/test/test_newllm.py` & `pylmkit-0.0.22/test/test_newllm.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/test/test_rag.py` & `pylmkit-0.0.22/test/test_rag.py`

 * *Files identical despite different names*

### Comparing `pylmkit-0.0.21/test/test_roleplay.py` & `pylmkit-0.0.22/test/test_roleplay.py`

 * *Files identical despite different names*

