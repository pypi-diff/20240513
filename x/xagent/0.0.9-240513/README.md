# Comparing `tmp/xagent-0.0.9.tar.gz` & `tmp/xagent-240513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagent-0.0.9.tar", last modified: Tue Apr 30 06:46:17 2024, max compression
+gzip compressed data, was "xagent-240513.tar", last modified: Mon May 13 05:40:24 2024, max compression
```

## Comparing `xagent-0.0.9.tar` & `xagent-240513.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.965921 xagent-0.0.9/
--rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.9/LICENSE
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-30 06:46:17.965714 xagent-0.0.9/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     7350 2024-04-29 10:55:35.000000 xagent-0.0.9/README.md
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-30 06:46:17.965980 xagent-0.0.9/setup.cfg
--rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.9/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.963467 xagent-0.0.9/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-0.0.9/tests/test_job.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4058 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3422 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2567 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_local_model.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8094 2024-04-29 10:55:36.000000 xagent-0.0.9/tests/test_xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.9/tests/test_zhipu_api_model.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.965452 xagent-0.0.9/xagent.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     1432 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      210 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-30 06:46:17.000000 xagent-0.0.9/xagent.egg-info/zip-safe
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.942276 xagent-0.0.9/xagents/
--rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/__init__.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.944952 xagent-0.0.9/xagents/agent/
--rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/agent/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3554 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/agent/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2206 2024-04-19 08:20:14.000000 xagent-0.0.9/xagents/agent/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.9/xagents/agent/memory.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8118 2024-04-30 06:16:53.000000 xagent-0.0.9/xagents/agent/xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2041 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/config.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.948925 xagent-0.0.9/xagents/kb/
--rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.9/xagents/kb/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)    12021 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8108 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)    13371 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3961 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/kb_file.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5516 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/kb/vector_store.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.956458 xagent-0.0.9/xagents/loader/
--rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.9/xagents/loader/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5376 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4226 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      945 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/csv_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1388 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/doc_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6064 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/docx_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1075 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/excel_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1594 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/json_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)      842 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/jsonl_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)      961 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/markdown_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3236 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/pdf_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1328 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/ppt_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2593 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/pptx_loader.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3374 2024-04-22 05:58:02.000000 xagent-0.0.9/xagents/loader/splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.9/xagents/loader/structed.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/loader/utils.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.958825 xagent-0.0.9/xagents/model/
--rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.9/xagents/model/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/model/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2426 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2243 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/local.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.9/xagents/model/openai.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4048 2024-04-29 10:55:36.000000 xagent-0.0.9/xagents/model/zhipu.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-30 06:46:17.960735 xagent-0.0.9/xagents/tool/
--rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.9/xagents/tool/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-0.0.9/xagents/tool/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-0.0.9/xagents/tool/common_tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-0.0.9/xagents/tool/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6639 2024-04-22 08:53:58.000000 xagent-0.0.9/xagents/tool/web_search.py
--rw-r--r--   0 chenhao    (501) staff       (20)      560 2024-04-19 07:38:46.000000 xagent-0.0.9/xagents/util.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.542261 xagent-240513/
+-rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-240513/LICENSE
+-rw-r--r--   0 chenhao    (501) staff       (20)      232 2024-05-13 05:40:24.542051 xagent-240513/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1392 2024-05-13 04:16:58.000000 xagent-240513/README.md
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-05-13 05:40:24.542336 xagent-240513/setup.cfg
+-rw-r--r--   0 chenhao    (501) staff       (20)     1174 2024-05-13 05:39:39.000000 xagent-240513/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.539955 xagent-240513/tests/
+-rw-r--r--   0 chenhao    (501) staff       (20)     2193 2024-04-19 07:38:46.000000 xagent-240513/tests/test_job.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4058 2024-04-29 10:55:36.000000 xagent-240513/tests/test_kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3358 2024-05-13 04:16:59.000000 xagent-240513/tests/test_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2567 2024-04-29 10:55:36.000000 xagent-240513/tests/test_local_model.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     9334 2024-05-13 04:16:59.000000 xagent-240513/tests/test_xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4803 2024-05-13 04:16:59.000000 xagent-240513/tests/test_zhipu_api_model.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.541633 xagent-240513/xagent.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      232 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1463 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      210 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-05-13 05:40:24.000000 xagent-240513/xagent.egg-info/zip-safe
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.523428 xagent-240513/xagents/
+-rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-240513/xagents/__init__.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.524942 xagent-240513/xagents/agent/
+-rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-240513/xagents/agent/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4232 2024-05-13 04:16:59.000000 xagent-240513/xagents/agent/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4115 2024-05-13 04:16:59.000000 xagent-240513/xagents/agent/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-240513/xagents/agent/memory.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8289 2024-05-13 04:16:59.000000 xagent-240513/xagents/agent/xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2129 2024-05-13 04:16:59.000000 xagent-240513/xagents/config.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.527492 xagent-240513/xagents/kb/
+-rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-240513/xagents/kb/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    11735 2024-05-13 04:16:59.000000 xagent-240513/xagents/kb/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     8225 2024-05-13 04:16:59.000000 xagent-240513/xagents/kb/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    13075 2024-05-13 04:16:59.000000 xagent-240513/xagents/kb/kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3967 2024-05-13 04:16:59.000000 xagent-240513/xagents/kb/kb_file.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5516 2024-04-29 10:55:36.000000 xagent-240513/xagents/kb/vector_store.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.534315 xagent-240513/xagents/loader/
+-rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-240513/xagents/loader/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     5446 2024-05-13 04:16:59.000000 xagent-240513/xagents/loader/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4256 2024-05-13 04:16:59.000000 xagent-240513/xagents/loader/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      945 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/csv_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1388 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/doc_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6064 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/docx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1075 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/excel_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1594 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/json_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      842 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/jsonl_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      961 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/markdown_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3177 2024-05-13 04:16:59.000000 xagent-240513/xagents/loader/pdf_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1328 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/ppt_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2593 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/pptx_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3896 2024-05-13 04:16:59.000000 xagent-240513/xagents/loader/splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-240513/xagents/loader/structed.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-29 10:55:36.000000 xagent-240513/xagents/loader/utils.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1198 2024-05-13 04:16:59.000000 xagent-240513/xagents/loader/xls_loader.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.536315 xagent-240513/xagents/model/
+-rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-240513/xagents/model/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-240513/xagents/model/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2594 2024-05-13 04:16:59.000000 xagent-240513/xagents/model/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2249 2024-05-10 07:04:29.000000 xagent-240513/xagents/model/local.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-240513/xagents/model/openai.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4048 2024-04-29 10:55:36.000000 xagent-240513/xagents/model/zhipu.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-05-13 05:40:24.538225 xagent-240513/xagents/tool/
+-rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-240513/xagents/tool/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1429 2024-04-19 08:20:14.000000 xagent-240513/xagents/tool/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1641 2024-04-22 03:01:50.000000 xagent-240513/xagents/tool/common_tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      463 2024-04-22 05:36:21.000000 xagent-240513/xagents/tool/core.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6639 2024-04-22 08:53:58.000000 xagent-240513/xagents/tool/web_search.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      669 2024-05-13 04:16:59.000000 xagent-240513/xagents/util.py
```

### Comparing `xagent-0.0.9/LICENSE` & `xagent-240513/LICENSE`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/setup.py` & `xagent-240513/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 import sys
 
 from setuptools import find_packages, setup
 
 from snippets.utils import get_latest_version, get_next_version, read2list
 
+
 def get_install_req():
     req = read2list("requirements.txt")
     return req
 
 
-
 if __name__ == "__main__":
     name = "xagent"
-    if len(sys.argv) >= 4 and sys.argv[-1].startswith("v"):
+    if len(sys.argv) >= 4:
         version = sys.argv.pop(-1)
     else:
         latest_version = get_latest_version(name)
         version = get_next_version(latest_version)
     print(f"version: {version}")
     install_req = get_install_req()
     print(f"install_req: {install_req}")
```

### Comparing `xagent-0.0.9/tests/test_job.py` & `xagent-240513/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/tests/test_kb.py` & `xagent-240513/tests/test_kb.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/tests/test_loader.py` & `xagent-240513/tests/test_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,89 +19,83 @@
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start test embd")
 
     @classmethod
-    def show_chunks(cls, chunks:Iterable[Chunk]):
+    def show_chunks(cls, chunks: Iterable[Chunk]):
         image_cnt = 0
         for chunk in chunks:
             logger.info(f"page={chunk.page_idx}, type={chunk.content_type}")
 
             if chunk.content_type == ContentType.IMAGE:
                 image_cnt += 1
                 logger.info(f"image:{chunk.image_name}")
                 logger.info(f"content:{chunk.content}")
                 logger.info(f"url:{chunk.url}")
             if chunk.content_type == ContentType.TEXT:
                 logger.info(f"text:{chunk.content}")
-    
+
             if chunk.content_type == ContentType.TABLE:
                 # logger.info(f"table:\n{chunk.data}")
                 logger.info(f"content:\n{chunk.content}")
             logger.info("*"*40+"\n")
         return image_cnt
 
     def test_load_pdf(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "image_table.pdf")
-        chunks = load_file(file_path, end_page=5, ocr=True)
+        chunks = load_file(file_path, end_page=5, ocr=False)
         # image_cnt = 0
         image_cnt = self.show_chunks(chunks)
 
         self.assertEqual(image_cnt, 4)
 
-
     def test_load_docx(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "Xagents中间件.docx")
-        chunks = load_file(file_path, ocr=True)
+        chunks = load_file(file_path, ocr=False)
         image_cnt = self.show_chunks(chunks)
 
         self.assertEqual(image_cnt, 1)
 
-
     # def test_load_doc(self):
     #     file_path = os.path.join(DATA_DIR, "kb_file", "初步设计文件.doc")
     #     chunks = load_file(file_path)
     #     image_cnt = self.show_chunks(chunks)
 
     #     self.assertEqual(image_cnt, 6)
-    
+
     def test_load_pptx(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "时序数据预测.pptx")
         chunks = load_file(file_path)
         image_cnt = self.show_chunks(chunks)
 
         self.assertEqual(image_cnt, 18)
-    
+
     def test_load_json(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "alpaca_data-0-3252-中文.json")
         chunks = list(load_file(file_path))
         self.show_chunks(chunks)
         self.assertEqual(len(chunks), 7)
-        
+
     def test_load_jsonl(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "LICENSE.jsonl")
         chunks = list(load_file(file_path))
         self.show_chunks(chunks)
         self.assertEqual(len(chunks), 17)
 
-
     def test_load_excel(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "大学综合排名2022.xlsx")
         chunks = list(load_file(file_path))
-        
+
         self.show_chunks(chunks)
 
         self.assertEqual(len(chunks), 3)
-        
+
     def test_load_txt(self):
         file_path = os.path.join(DATA_DIR, "kb_file", "requirements.txt")
         chunks = load_file(file_path)
         image_cnt = self.show_chunks(chunks)
         self.assertEqual(image_cnt, 0)
-        chunks = parse_file(file_path = file_path)
+        chunks = parse_file(file_path=file_path)
         logger.info(chunks)
         self.show_chunks(chunks)
-                
-
-
```

### Comparing `xagent-0.0.9/tests/test_local_model.py` & `xagent-240513/tests/test_local_model.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/tests/test_xagent.py` & `xagent-240513/tests/test_xagent.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,23 +10,55 @@
 from unittest import TestCase
 # sys.path.append("../")
 from xagents.agent.api import *
 from xagents.kb.api import *
 from loguru import logger
 from snippets import set_logger
 
+agent_name = "unittest_agent"
 
 # unit test
+
+
 class TestXagent(TestCase):
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start test embd")
 
+    def test_list_agents(self):
+        agents = list_agents()
+        logger.info(f"agents: {agents}")
+        agents_names = [agent.name for agent in agents]
+        self.assertIn(agent_name, agents_names)
+
+    def test_get_agent(self):
+        agent: XAgent = get_agent(name=agent_name)
+        logger.info(f"agent: {agent.get_info()}")
+
+    def test_create_delete_agent(self):
+        llm_config = dict(cls="GLM", version="glm-3-turbo")
+        tools_config = [dict(name="计算器"), dict(name="车次查询")]
+        agent_name = "temp_create_agent"
+        agent = create_agent(name=agent_name, llm_config=llm_config,
+                             kb_config=KBConfig(name="unittest_kb"),
+                             tools_config=tools_config, store_type=STORE_TYPE.DISK)
+        # logger.info(f"create Agent {agent.get_info()} success")
+        agent = get_agent(name=agent_name)
+        logger.info(f"create agent: {agent.get_info()} success")
+
+        delete_agent(name=agent_name)
+        logger.info(f"delete agent {agent_name} success")
+        agent = get_agent(name=agent_name)
+
+        self.assertRaises(Exception)
+
+        # create agent
+
     def test_agent_tool_use(self):
         agent_name = "unittest_agent"
         llm_config = dict(cls="GLM", version="glm-3-turbo")
         tools_config = [dict(name="计算器"), dict(name="车次查询")]
 
         # create agent
         agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, tools_config=tools_config)
@@ -57,18 +89,19 @@
 
         logger.info(f"create tools_config_v1 {tools_config} success")
         # create agent
         agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, tools_config=tools_config, kb_config=kb_config)
         logger.info(f"create Agent {agent.get_info()} success")
 
         # chat with agent
-        message = "帮我查询一下杭州的最新天气"#"你能帮我找一下今天关于杭州实时新闻吗？"
+        message = "帮我查询一下杭州的最新天气"  # "你能帮我找一下今天关于杭州实时新闻吗？"
         kb_search_config = KBSearchConfig(do_expand=True, expand_len=200)
         llm_gen_config = LLMGenConfig()
-        agent_resp = chat_agent(name=agent.name, message=message, use_kb = False, stream=False, kb_search_config= kb_search_config, llm_gen_config=llm_gen_config)
+        agent_resp = chat_agent(name=agent.name, message=message, use_kb=False, stream=False,
+                                kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
         logger.info(f"agent resp: {agent_resp.model_dump()}")
         self.assertIsNotNone(agent_resp.content)
         self.assertIsNotNone(agent_resp.usage)
 
     def test_agent_multi_turn(self):
         agent_name = "unittest_agent"
         llm_config = dict(cls="GLM", version="glm-3-turbo")
@@ -116,29 +149,29 @@
         except Exception as e:
             cur_dir = os.path.abspath(os.path.dirname(__file__))
             file_path = os.path.join(os.path.dirname(cur_dir), file_name)
             logger.debug(f"adding file:{file_path}")
             kb_file = create_kb_file(kb_name=kb_name, file=file_path)
 
     def test_agent_kb(self):
-        agent_name = "unittest_agent"
         llm_config = dict(cls="GLM", version="glm-3-turbo")
         kb_name = "unittest_kb"
         self._init_kb(kb_name)
         kb_config = KBConfig(name=kb_name)
 
         # create agent
         agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, kb_config=kb_config)
         logger.info(f"create Agent {agent.get_info()} success")
 
         # chat with agent
         message = "20240401发布了哪些功能？"
         llm_gen_config = LLMGenConfig()
         kb_search_config = KBSearchConfig(do_expand=True, expand_len=200)
-        agent_resp = chat_agent(name=agent.name, message=message, use_kb=True, stream=False, kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
+        agent_resp = chat_agent(name=agent.name, message=message, use_kb=True, stream=False,
+                                kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
         # agent_resp = agent.chat(name=agent.name, message=message, llm_gen_config=llm_gen_config)
 
         self.assertIsNotNone(agent_resp.content)
         content = "".join(agent_resp.content)
         logger.info(f"agent resp:{content}")
 
         self.assertIsNotNone(agent_resp.references)
@@ -148,15 +181,15 @@
 
         self.assertIsNotNone(agent_resp.usage)
 
         logger.info(f"agent resp: {agent_resp.model_dump(exclude={'content'})}")
 
     def test_inverted_index(self):
         # create kb
-        kb_name='test_inverted'
+        kb_name = 'test_inverted'
         try:
             kb = get_knowledge_base(kb_name)
         except Exception as e:
             kb = create_knowledge_base(kb_name)
         file_name = "README.md"
 
         # create kb_file
@@ -184,12 +217,12 @@
         agent: XAgent = create_agent(name=agent_name, llm_config=llm_config, kb_config=kb_config)
         logger.info(f"create Agent {agent.get_info()} success")
 
         # chat with agent
         message = "具体接口文档参考哪里？"
         llm_gen_config = LLMGenConfig()
         kb_search_config = KBSearchConfig(do_expand=True, expand_len=200)
-        agent_resp = chat_agent(name=agent.name, message=message, use_kb=True, stream=False, kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
+        agent_resp = chat_agent(name=agent.name, message=message, use_kb=True, stream=False,
+                                kb_search_config=kb_search_config, llm_gen_config=llm_gen_config)
         self.assertIsNotNone(agent_resp.content)
         content = "".join(agent_resp.content)
         logger.info(f"agent resp:{content}")
-
```

### Comparing `xagent-0.0.9/tests/test_zhipu_api_model.py` & `xagent-240513/tests/test_zhipu_api_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,112 +7,111 @@
 @Contact :   jerrychen1990@gmail.com
 '''
 import json
 import os
 from unittest import TestCase
 from xagents.model.zhipu import API_GLM
 from xagents.model.common import EMBD, LLMResp
-from xagents.model import get_embd_model,get_llm_model
+from xagents.model import get_embd_model, get_llm_model
 from xagents.tool import travel_searcher
 from xagents.tool.api import invoke_tool_call
 from loguru import logger
 from snippets import set_logger
 
 
 # unit test
 class TestEMBD(TestCase):
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start test embd")
-        cls.zhipu_api_embedding:EMBD= get_embd_model(dict(cls="ZhipuEmbedding", api_key=os.environ["ZHIPU_API_KEY"], batch_size=4))
+        cls.zhipu_api_embedding: EMBD = get_embd_model(dict(cls="ZhipuEmbedding", api_key=os.environ["ZHIPU_API_KEY"], batch_size=4))
 
     def test_zhipu_api(self):
         # set_logger("dev", "")
         texts = ["你好", "hello"]
         embds = self.zhipu_api_embedding.embed_documents(texts)
         logger.info(len(embds))
         self.assertEqual(len(embds), 2)
         import numpy as np
         logger.info(np.linalg.norm(embds[0]))
         self.assertAlmostEqual(np.linalg.norm(embds[0]), 1.0)
 
         print(embds[0][:4])
         embd = self.zhipu_api_embedding.embed_query(text=texts[0])
-        print(embd[:4])
-        self.assertListEqual(embds[0], embd)
-        
+        # print(embd[:4])
+        # self.assertListEqual(embds[0], embd)
+
+
 class TestGLM(TestCase):
 
     @classmethod
     def setUpClass(cls):
         set_logger("dev", __name__)
         logger.info("start llm")
-        cls.zhipu_api_llm_model:API_GLM = get_llm_model(dict(cls="GLM", api_key=os.environ["ZHIPU_API_KEY"], name="glm-3-turbo", version="glm-3-turbo" ))
+        cls.zhipu_api_llm_model: API_GLM = get_llm_model(
+            dict(cls="GLM", api_key=os.environ["ZHIPU_API_KEY"], name="glm-3-turbo", version="glm-3-turbo"))
 
     def test_zhipu_api(self):
         # set_logger("dev", "")
         prompt = "你好呀，你是谁"
         _system = "请用英语回答我的问题，你的名字叫XAgent"
-        
+
         # 测试zhipu api
-        resp:LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=False)        
+        resp: LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, temperature=0.7,
+                                                          top_p=0.95, max_tokens=100, log_level="INFO", stream=False)
 
         logger.info(json.dumps(resp.model_dump(), ensure_ascii=False, indent=4))
-        self.assertIsNotNone(resp.content)        
-        self.assertIsNotNone(resp.usage)        
-
+        self.assertIsNotNone(resp.content)
+        self.assertIsNotNone(resp.usage)
 
-        ## 流式
-        resp:LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=True)        
+        # 流式
+        resp: LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, temperature=0.7,
+                                                          top_p=0.95, max_tokens=100, log_level="INFO", stream=True)
         for chunk in resp.content:
             logger.info(chunk)
         logger.info(json.dumps(resp.model_dump(exclude={"content"}), ensure_ascii=False, indent=4))
         self.assertIsNotNone(resp.usage)
 
-  
-    def test_zhipu_api_tool_call(self):   
-
+    def test_zhipu_api_tool_call(self):
 
         prompt = "你能帮我查询2024年1月1日从北京南站到上海的火车票吗？"
         _system = None
         tools = [travel_searcher]
         # 测试zhipu api
-        resp:LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, tools=tools, temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=False)        
+        resp: LLMResp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, tools=tools,
+                                                          temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=False)
         logger.info(json.dumps(resp.model_dump(), ensure_ascii=False, indent=4))
-        self.assertIsNotNone(resp.tool_calls)        
-        self.assertIsNotNone(resp.usage)       
-        #调用工具
+        self.assertIsNotNone(resp.tool_calls)
+        self.assertIsNotNone(resp.usage)
+        # 调用工具
         logger.info("invoking tools")
-        for tool_call in resp.tool_calls:        
+        for tool_call in resp.tool_calls:
             tool_resp = invoke_tool_call(tool_call)
-                        
 
-            tool_call.resp=tool_resp
-            resp:LLMResp = self.zhipu_api_llm_model.observe(prompt=prompt, tool_call=tool_call, tools=tools, stream=False)
-            
-            logger.info(json.dumps(resp.model_dump(), ensure_ascii=False, indent=4))
-            self.assertIsNotNone(resp.content)        
-            self.assertIsNotNone(resp.usage)  
-        
-         
+            tool_call.resp = tool_resp
+            resp: LLMResp = self.zhipu_api_llm_model.observe(prompt=prompt, tool_call=tool_call, tools=tools, stream=False)
 
+            logger.info(json.dumps(resp.model_dump(), ensure_ascii=False, indent=4))
+            self.assertIsNotNone(resp.content)
+            self.assertIsNotNone(resp.usage)
 
         # ## 流式
-        resp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, tools=tools, temperature=0.7, top_p=0.95, max_tokens=100, log_level="INFO", stream=False)
+        resp = self.zhipu_api_llm_model.generate(prompt=prompt, system=_system, tools=tools, temperature=0.7,
+                                                 top_p=0.95, max_tokens=100, log_level="INFO", stream=False)
         logger.info(json.dumps(resp.model_dump(exclude={"content"}), ensure_ascii=False, indent=4))
 
-        self.assertIsNotNone(resp.tool_calls)        
+        self.assertIsNotNone(resp.tool_calls)
         self.assertIsNotNone(resp.usage)
-        
-        #调用工具
+
+        # 调用工具
         logger.info("invoking tools")
-        for tool_call in resp.tool_calls:        
+        for tool_call in resp.tool_calls:
             tool_resp = invoke_tool_call(tool_call)
-                    
-            tool_call.resp=tool_resp
-            resp:LLMResp = self.zhipu_api_llm_model.observe(prompt=prompt, tool_call=tool_call, tools=tools, stream=True)
+
+            tool_call.resp = tool_resp
+            resp: LLMResp = self.zhipu_api_llm_model.observe(prompt=prompt, tool_call=tool_call, tools=tools, stream=True)
             for chunk in resp.content:
                 logger.info(chunk)
             logger.info(json.dumps(resp.model_dump(exclude={"content"}), ensure_ascii=False, indent=4))
             self.assertIsNotNone(resp.usage)
```

### Comparing `xagent-0.0.9/xagent.egg-info/SOURCES.txt` & `xagent-240513/xagent.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ./xagents/loader/markdown_loader.py
 ./xagents/loader/pdf_loader.py
 ./xagents/loader/ppt_loader.py
 ./xagents/loader/pptx_loader.py
 ./xagents/loader/splitter.py
 ./xagents/loader/structed.py
 ./xagents/loader/utils.py
+./xagents/loader/xls_loader.py
 ./xagents/model/__init__.py
 ./xagents/model/api.py
 ./xagents/model/common.py
 ./xagents/model/local.py
 ./xagents/model/openai.py
 ./xagents/model/zhipu.py
 ./xagents/tool/__init__.py
```

### Comparing `xagent-0.0.9/xagents/__init__.py` & `xagent-240513/xagents/__init__.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/agent/api.py` & `xagent-240513/xagents/agent/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 '''
 @Time    :   2024/04/01 13:46:25
 @Author  :   ChenHao
 @Description  :   Agent问答的api
 @Contact :   jerrychen1990@gmail.com
 '''
 from enum import Enum
+import os
 from typing import List
+
 from xagents.tool.api import get_tools
 from xagents.model.common import LLMGenConfig
 from xagents.kb.api import KBSearchConfig
 from xagents.config import AGENT_DIR, XAGENT_CACHE_NUM
 from xagents.agent.common import AgentResp, KBConfig
 from xagents.agent.xagent import XAgent
 from cachetools import LRUCache, cached
@@ -30,68 +32,87 @@
                  kb_config: KBConfig = None, store_type=STORE_TYPE.CACHE) -> XAgent:
 
     logger.info(f"creating agent:{name}")
     # print(f"web_search_config2:{web_search_config}")
 
     @cached(agent_cache)
     def _get_or_create(name: str):
-        tools = get_tools( tools_config)  #  [{'name': '联网查询'}]
+        tools = get_tools(tools_config)  # [{'name': '联网查询'}]
         # print(f"web_search_config3:{web_search_config}")
         logger.info(f"getting tools_config:{tools_config}")
         logger.info(f"getting tools:{tools}")
         xagent = XAgent(name=name, llm_config=llm_config, memory_config=memory_config, kb_config=kb_config, tools=tools)
         return xagent
     agent = _get_or_create(name=name)
     if store_type == STORE_TYPE.DISK:
         agent.save(AGENT_DIR)
-        
+
     return agent
 
 
 @cached(agent_cache)
 def get_agent(name: str) -> XAgent:
-    agent = XAgent.load(AGENT_DIR, name)
-    return agent    
+    agent = XAgent.from_config(os.path.join(AGENT_DIR, name+".json"))
+    return agent
 
 
-def chat_agent(name: str, message: str, do_remember=True, details=False, stream=False,
-               use_kb=False, kb_search_config:KBSearchConfig=KBSearchConfig(),
-               fake_chat=False, llm_gen_config:LLMGenConfig = LLMGenConfig()) -> AgentResp:
+def chat_agent(name: str, message: str, history: List[dict] = None, do_remember=True, details=False, stream=False,
+               use_kb=False, kb_search_config: KBSearchConfig = KBSearchConfig(),
+               fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig()) -> AgentResp:
     """和Agent对话
 
     Args:
         name (str): Agent的名称
         message (str): 用户发送的消息
+        history (List[dict], optional): 历史对话记录. Defaults to None.
         do_remember (bool, optional): Agent是否要记住历史对话. Defaults to True.
         details (bool, optional): 是否返回详细调用信息. Defaults to False.
         use_kb (bool, optional): 是否使用知识库. Defaults to False.
         kb_search_config (KBSearchConfig, optional): 知识库查询参数，use_kb=True时生效. Defaults to KBSearchConfig().
         fake_chat (bool, optional): 是否fake大模型问答（fake_chat=True时，不会调用LLM）. Defaults to False.
         llm_gen_config (LLMGenConfig, optional): 大模型生成文本需要的参数. Defaults to LLMGenConfig.
 
     Returns:
         AgentResp: Agent回答的结构体
     """
     # logger.info(f"sending message:{message} to agent:{name}")
     agent = get_agent(name=name)
-    agent_resp = agent.chat(message=message, do_remember=do_remember, details=details, stream=stream,
+    agent_resp = agent.chat(message=message, history=history, do_remember=do_remember, details=details, stream=stream,
                             use_kb=use_kb, kb_search_config=kb_search_config,
                             fake_chat=fake_chat, llm_gen_config=llm_gen_config)
     return agent_resp
 
 
-def clear_agent(name:str) ->None:
+def list_agents() -> List[XAgent]:
+    """列出所有Agent的名称
+
+    Returns:
+        List[str]: Agent的名称列表
+    """
+    agents = []
+    for agent_config_name in os.listdir(AGENT_DIR):
+        # 加载agent
+        agent_name = agent_config_name.replace(".json", "")
+        try:
+            agent = get_agent(name=agent_name)
+            agents.append(agent)
+        except Exception as e:
+            logger.warning(f"fail to load agent {agent_name} with error:{e}")
+            # raise e
+    return agents
+
+
+def clear_agent(name: str) -> None:
     """清空agent的历史对话记录
 
     Args:
         name (str): agent的名称
     """
     logger.info(f"clear memory of {name}")
     agent = get_agent(name=name)
     agent.clear_memory()
 
 
-def delete_agent(name:str) ->None:
+def delete_agent(name: str) -> None:
     logger.info(f"clear memory of {name}")
     agent = get_agent(name=name)
     agent.delete(AGENT_DIR)
-
```

### Comparing `xagent-0.0.9/xagents/agent/memory.py` & `xagent-240513/xagents/agent/memory.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/agent/xagent.py` & `xagent-240513/xagents/agent/xagent.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 import os
 import copy
-import shutil
 from typing import Generator, List, Optional
 
 from pydantic import BaseModel, Field
 
 from agit.common import LLMResp
+from xagents.util import save_format
 from xagents.model.common import LLMGenConfig
 from xagents.agent.common import AbstractAgent, AgentResp, KBConfig, WebSearchResp
 from xagents.config import LOG_DIR
 from xagents.kb.common import RecalledChunk
 from xagents.kb.api import KBSearchConfig, get_knowledge_base
 from xagents.model.api import get_llm_model
 from xagents.agent.memory import BaseMemory
-from xagents.tool.api import invoke_tool_call
+from xagents.tool.api import get_tools, invoke_tool_call
 from xagents.tool.core import BaseTool, ToolCall, ToolDesc
-from snippets import dump, load
+from snippets import dump, jload
 
 from loguru import logger
 
 agent_log_path = os.path.join(LOG_DIR, "xagent.log")
 
 
 class XAgentInfo(BaseModel):
@@ -89,58 +89,58 @@
         logger.debug(f"agent info:{self.get_info()}")
         dump(self.get_info().model_dump(), save_path)
 
     def delete(self, save_dir: str):
         save_path = self._get_agent_config_path(save_dir, self.name)
         if os.path.exists(save_path):
             logger.info(f"deleting agent:{self.name} from save_path:{save_path}")
-            shutil.rmtree(save_path)
+            os.remove(save_path)
 
     @classmethod
-    def load(cls, save_dir: str, name: str) -> "XAgent":
-        config_path = cls._get_agent_config_path(save_dir, name)
-        if not os.path.exists(config_path):
-            raise FileExistsError(f"config file {config_path} not found")
-
-        kwargs = load(config_path)
-        if kwargs.get("kb_config"):
-            kwargs["kb_config"] = KBConfig.model_validate(kwargs["kb_config"])
-        logger.debug(f"{kwargs=}")
+    def from_config(cls, config: str | dict) -> "XAgent":
+        config = jload(config) if isinstance(config, str) else config
+        if config.get("tools"):
+            tools = get_tools(config["tools"])
+            config["tools"] = tools
+        if config.get("kb_config"):
+            config["kb_config"] = KBConfig.model_validate(config["kb_config"])
 
-        return XAgent(**kwargs)
+        return XAgent(**config)
 
-    def chat(self, message: str, do_remember=True, details=False, stream=False,
+    def chat(self, message: str, history: List[dict] = None, do_remember=True, details=False, stream=False,
              use_kb=False, kb_search_config: KBSearchConfig = KBSearchConfig(),
-             fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig(), key_word=True, **kwargs) -> AgentResp:
+             fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig(), **kwargs) -> AgentResp:
 
         chunks = []
         if use_kb:
             if not self.kb or not self.kb_prompt_template:
                 logger.warning(f"agent:{self.name} has no related knowledge base, will not chat with kb! ")
                 prompt = message
                 chunks = None
             else:
                 logger.info("agent searching kb with kb_name")
                 chunks = self.search_kb(query=message, **kb_search_config.model_dump())
                 context = "\n".join(f"{idx+1}." + c.to_plain_text() for idx, c in enumerate(chunks))
-                prompt = self.kb_prompt_template.format(question=message, context=context)
+                prompt = save_format(template=self.kb_prompt_template, question=message, context=context)
+
+                # prompt = self.kb_prompt_template.format(question=message, context=context)
         else:
             prompt = message
             chunks = None
 
         web_search_result = None
         tool_calls = None
         if fake_chat:
             fake_resp = "这是MOCK的回答信息,如果需要真实回答,请设置fake_chat=False"
             llm_resp = (e for e in fake_resp) if stream else fake_resp
             tool_call = None
         else:
-            history = self.memory.to_llm_history()
+            history = history if history is not None else self.memory.to_llm_history()
             llm_resp: LLMResp = self.llm_model.generate(prompt=prompt, history=history, tools=self.tools, details=details, stream=stream,
-                                                        **llm_gen_config.model_dump(), key_word=key_word, **kwargs)
+                                                        **llm_gen_config.model_dump(), **kwargs)
 
             logger.debug(f"llm_resp_inner:{llm_resp}")
             # 调用tool
             tool_calls = copy.deepcopy(llm_resp.tool_calls)
             if tool_calls:
                 for tool_call in tool_calls:
                     logger.debug(f"calling tool:{tool_call.name}")
@@ -182,14 +182,17 @@
         logger.debug(f"remembering {role=}, {message=}")
         self.memory.remember(role, message)
 
     def clear_memory(self):
         # logger.info("clearing memory")
         self.memory.clear()
 
+    def __repr__(self) -> str:
+        return f"XAgent-{self.name}"
+
 
 if __name__ == "__main__":
     llm_config = dict(model_cls="GLM", name="glm", version="chatglm_turbo")
     memory_config = dict(size=10)
     agent = XAgent(name="xagent", llm_config=llm_config, memory_config=memory_config)
     resp = agent.chat("推荐三首歌", stream=True)
     for item in resp:
```

### Comparing `xagent-0.0.9/xagents/config.py` & `xagent-240513/xagents/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 
 TEMP_DIR = os.environ.get("XAGENT_TEMP_DIR", os.path.join(XAGENT_HOME, "tmp"))
 os.makedirs(TEMP_DIR, exist_ok=True)
 
 LOG_DIR = os.environ.get("XAGENT_LOG_DIR", os.path.join(XAGENT_HOME, "log"))
 os.makedirs(LOG_DIR, exist_ok=True)
 
+JOB_LOG_DIR = os.path.join(LOG_DIR, "jobs")
+os.makedirs(JOB_LOG_DIR, exist_ok=True)
+
 DB_DIR = os.environ.get("XAGENT_DB_DIR", os.path.join(XAGENT_HOME, "db"))
 os.makedirs(DB_DIR, exist_ok=True)
 
 AGENT_DIR = os.environ.get("XAGENT_AGENT_DIR", os.path.join(XAGENT_HOME, "agent"))
 os.makedirs(AGENT_DIR, exist_ok=True)
 
 DATA_DIR = os.path.join(XAGENT_HOME, "data")
@@ -49,23 +52,22 @@
 [搜索信息]
 {search_info}
 问题:
 {question}
 '''
 
 
-### Service相关
-### 最大job数（job用来处理知识库index任务）
-MAX_JOB_NUM=10
-### 用户鉴权配置
-USERNAME="zhipu"
-PASSWORD="zhipu"
-### xagent缓存数目
-XAGENT_CACHE_NUM=1000
-XAGENT_CACHE_EXPIRE_SECONDS=3600
-
+# Service相关
+# 最大job数（job用来处理知识库index任务）
+MAX_JOB_NUM = 10
+# 用户鉴权配置
+USERNAME = "zhipu"
+PASSWORD = "zhipu"
+# xagent缓存数目
+XAGENT_CACHE_NUM = 1000
+XAGENT_CACHE_EXPIRE_SECONDS = 3600
 
 
-### MinIO对象存储相关
+# MinIO对象存储相关
 MINIO_URL = os.environ.get("MINIO_URL", "10.50.130.151:9000")
-MINIO_ACCESS_KEY=os.environ.get("MINIO_ACCESS_KEY", 'l7RJ3QCGX6gt7M8zfN1v')
-MINIO_SECRET_KEY=os.environ.get("MINIO_SECRET_KEY", 'smGpFhcz0hLOup8V2s6SMkzgzxzJFtSJiuAuKFqS')
+MINIO_ACCESS_KEY = os.environ.get("MINIO_ACCESS_KEY", 'l7RJ3QCGX6gt7M8zfN1v')
+MINIO_SECRET_KEY = os.environ.get("MINIO_SECRET_KEY", 'smGpFhcz0hLOup8V2s6SMkzgzxzJFtSJiuAuKFqS')
```

### Comparing `xagent-0.0.9/xagents/kb/api.py` & `xagent-240513/xagents/kb/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,31 +12,33 @@
 from pydantic import BaseModel, Field
 from xagents.loader.common import Chunk
 from xagents.kb.kb_file import KnowledgeBaseFile
 from xagents.kb.kb import KnowledgeBase
 from xagents.config import *
 from xagents.kb.common import KnowledgeBaseInfo, KnowledgeBaseFileInfo, RecalledChunk, get_config_path, DistanceStrategy
 
+
 def list_knowledge_base_names() -> List[str]:
     """列出所有知识库名称
 
     Returns:
         str: 知识库名称列表
     """
     kb_names = os.listdir(KNOWLEDGE_BASE_DIR)
     return kb_names
 
+
 def list_knowledge_base_info() -> List[KnowledgeBaseInfo]:
     kb_infos = []
-    kb_names=  list_knowledge_base_names()
+    kb_names = list_knowledge_base_names()
     for name in kb_names:
         kb = get_knowledge_base(name)
         kb_infos.append(kb.get_info())
     return kb_infos
-    
+
 
 def get_knowledge_base(name: str) -> KnowledgeBase:
     """根据知识库名称获取知识库
 
     Args:
         name (str): 知识库名称
 
@@ -62,16 +64,16 @@
     kb = get_knowledge_base(name=name)
     return kb.get_info()
 
 
 def create_knowledge_base(name: str,
                           desc: str = None,
                           embedding_config: dict = dict(cls="ZhipuEmbedding"),
-                          vecstore_config: dict|List[dict] = dict(cls='XFAISS', distance_strategy=DistanceStrategy.MAX_INNER_PRODUCT)
-                          )->KnowledgeBase:
+                          vecstore_config: dict | List[dict] = dict(cls='XFAISS', distance_strategy=DistanceStrategy.MAX_INNER_PRODUCT)
+                          ) -> KnowledgeBase:
     """创建知识库
 
     Raises:
         ValueError: 知识库已经存在的异常
 
     Returns:
         _type_: _description_
@@ -98,59 +100,59 @@
         name (str): 知识库名称
 
     Returns:
         str: 删除消息
     """
     # delete knowledge base
     kb = get_knowledge_base(name=name)
-    kb.delete()    
+    kb.delete()
 
     # kb_dir = get_kb_dir(kb_name=name)
     # if os.path.exists(kb_dir):
     #     import shutil
     #     shutil.rmtree(path=kb_dir)
     msg = f'【{name}】deleted.'
     return msg
 
 
-def reindex_knowledge_base(name: str, reindex=True, batch_size=16) -> str:
+def reindex_knowledge_base(name: str, batch_size=16) -> str:
     """重新构建知识库索引
 
     Args:
         name (str): 知识库名称
-        reindex(bool): 对于已经索引好的文件是否重新embedding
         batch_size(int): 调用embedding的时候的batch_size（对于开发平台api,是并发度）
     """
     kb = get_knowledge_base(name=name)
-    kb.rebuild_index(reindex=reindex, batch_size=batch_size)
+    kb.rebuild_index(batch_size=batch_size)
     msg = f"知识库【{name}】重建索引成功"
     return msg
 
 
 class KBSearchConfig(BaseModel):
-    top_k:int = Field(default=3, description="返回几个chunk")
-    score_threshold:float = Field(default=0., description="分数阈值")
-    do_split_query:bool = Field(default=False, description="是否分词")
-    file_names:List[str] = Field(default=[], description="需要筛选的知识库文件文件名列表")
-    rerank_config:dict = Field(default={}, description="rerank的配置")
-    do_expand:bool = Field(default=False, description="对结果是否进行上下文扩展")
-    expand_len:int = Field(default=500, description="上下文扩展的长度")
-    forward_rate:float = Field(default=0.5, description="上下文扩展向下扩展的比例")
-    
+    top_k: int = Field(default=3, description="返回几个chunk")
+    score_threshold: float = Field(default=0., description="分数阈值")
+    do_split_query: bool = Field(default=False, description="是否分词")
+    file_names: List[str] = Field(default=[], description="需要筛选的知识库文件文件名列表")
+    rerank_config: dict = Field(default={}, description="rerank的配置")
+    do_expand: bool = Field(default=False, description="对结果是否进行上下文扩展")
+    expand_len: int = Field(default=500, description="上下文扩展的长度")
+    forward_rate: float = Field(default=0.5, description="上下文扩展向下扩展的比例")
+
 
 def search_knowledge_base(name: str,
                           query: str, top_k: int = 3, score_threshold: float = None,
                           do_split_query=False, file_names: List[str] = [], rerank_config: dict = {},
                           do_expand=False, expand_len: int = 500, forward_rate: float = 0.5) -> List[RecalledChunk]:
     kb = get_knowledge_base(name=name)
-    
+
     chunks = kb.search(query=query, top_k=top_k, score_threshold=score_threshold, do_split_query=do_split_query,
                        file_names=file_names, rerank_config=rerank_config, do_expand=do_expand, expand_len=expand_len, forward_rate=forward_rate)
     return chunks
 
+
 def list_kb_files(kb_name: str) -> List[KnowledgeBaseFile]:
     kb = get_knowledge_base(kb_name)
     kb_files = kb.list_kb_files()
     return kb_files
 
 
 def list_kb_file_infos(kb_name: str) -> List[KnowledgeBaseFileInfo]:
@@ -169,17 +171,17 @@
 
 def get_kb_file_info(kb_name: str, file_name: str) -> KnowledgeBaseFileInfo:
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
     return kb_file.get_info()
 
 
 def create_kb_file(kb_name: str, file: UploadFile | str, do_cut=True, do_index=True,
-                   batch_size:int=16,
-                   upload_image:bool=False,
-                   ocr:bool=False,
+                   batch_size: int = 16,
+                   upload_image: bool = False,
+                   ocr: bool = False,
                    cut_config: dict = dict(separator='\n',
                                            max_len=200,
                                            min_len=10)) -> KnowledgeBaseFile:
     """创建知识库文件
     Args:
         kb_name (str): 知识库名称
         file (UploadFile | str): 知识库文件，UploadFile(fast_api)或者str(文件路径)
@@ -211,15 +213,15 @@
         content = file.file.read()
     with open(kb_file_path, "wb") as f:
         f.write(content)
     if do_cut:
         kb_file.cut(upload_image=upload_image, ocr=ocr, **cut_config)
     if do_index:
         kb = get_knowledge_base(name=kb_name)
-        kb.add_kb_file2index(kb_file=kb_file, reindex=True, do_save=True, batch_size=batch_size)
+        kb.add_kb_file2index(kb_file=kb_file, do_save=True, batch_size=batch_size)
     return kb_file
 
 
 def delete_kb_file(kb_name: str, file_name: str) -> str:
     """删除知识库文件
 
     Args:
@@ -235,101 +237,101 @@
     kb.remove_kb_file(kb_file=kb_file)
     return f"知识库文件【{file_name}】删除成功"
 
 
 def cut_kb_file(kb_name: str, file_name: str,
                 separator: str = '\n',
                 max_len: int = 200,
-                min_len: int = 10) -> int:
+                min_len: int = 10) -> dict:
     """切分文档，并且按照jsonl格式存储在chunk目录下
 
     Args:
         kb_name (str): 知识库名称
         file_name (str): 文件名称
-        separator (str, optional): 切分符. Defaults to '\n'.
-        max_len (int, optional): 最大切片长度. Defaults to 200.
-        min_len (int, optional): 最小切片长度. Defaults to 10.
+        separator (str, optional): 切分符. Defaults to '\n'
+        max_len (int, optional): 最大切片长度. Defaults to 200
+        min_len (int, optional): 最小切片长度. Defaults to 10
 
     Returns:
         int: 切片数目
     """
 
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
     chunk_num = kb_file.cut(separator=separator, max_len=max_len, min_len=min_len)
-    return chunk_num
+    return dict(chunk_num=chunk_num)
 
 
-def reindex_kb_file(kb_name: str, file_name: str, reindex=False,  batch_size=16) -> str:
+def reindex_kb_file(kb_name: str, file_name: str, batch_size=16) -> str:
     """添加知识库文件到索引中
 
     Args:
         kb_name (str): 知识库名称
         file_name (str): 知识库文件名称
-        reindex (bool, optional): 如果知识库文件已经存在，是否重新构建索引. Defaults to False.
-
     Returns:
         str: 构建成功的消息
     """
 
     kb = get_knowledge_base(kb_name)
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
-    indexes = kb.get_indexes()
-    kb.add_kb_file2index(indexes=indexes, kb_file=kb_file, reindex=reindex, do_save=True, batch_size=batch_size)
+    kb.add_kb_file2index(kb_file=kb_file, do_save=True, batch_size=batch_size)
     return f"更新知识库文件【{file_name}】到索引成功"
 
 
 def list_chunks(kb_name: str, file_name: str) -> List[Chunk]:
     """给定知识库文件，返回所有的chunk
 
     Args:
         kb_name (str): 知识库名称
         file_name (str): 知识库文件名称
 
     Returns:
         List[Chunk]: chunk列表
     """
-    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
-    chunks =  kb_file.list_chunks()
-    return chunks   
+    kb_file: KnowledgeBaseFile = get_kb_file(kb_name=kb_name, file_name=file_name)
+    chunks = kb_file.list_chunks()
+    return chunks
+
 
-def add_chunks(kb_name: str, file_name: str, chunks: List[Chunk], idx:int=None) -> str:
+def add_chunks(kb_name: str, file_name: str, chunks: List[Chunk], idx: int = None) -> str:
     """给定知识库文件，添加chunk
 
     Args:
         kb_name (str): 知识库名称
         file_name (str): 知识库文件名称
         chunk (Chunk): 待添加的chunk
         idx (_type_, optional): chunk添加的位置，None的话添加在最后. Defaults to None.
 
     Returns:
         str: 添加成功的消息
     """
-    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file: KnowledgeBaseFile = get_kb_file(kb_name=kb_name, file_name=file_name)
     kb_file.add_chunks(chunks=chunks, idx=idx)
-    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    kb: KnowledgeBase = get_knowledge_base(name=kb_name)
     kb.add_chunks2index(chunks=chunks, meta_info=dict(file_name=file_name), do_save=True)
-    message =f"添加{len(chunks)}chunk到知识库文件【{file_name}】成功" 
+    message = f"添加{len(chunks)}chunk到知识库文件【{file_name}】成功"
     return message
 
+
 def delete_chunks(kb_name: str, file_name: str, chunk_ids: List[str]) -> str:
 
-    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file: KnowledgeBaseFile = get_kb_file(kb_name=kb_name, file_name=file_name)
     kb_file.delete_chunks(ids=chunk_ids)
-    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    kb: KnowledgeBase = get_knowledge_base(name=kb_name)
     kb.remove_chunks_from_index(chunk_ids=chunk_ids)
-    message =f"从【{file_name}】删除{len(chunk_ids)}chunk成功" 
+    message = f"从【{file_name}】删除{len(chunk_ids)}chunk成功"
     return message
 
+
 def update_chunk(kb_name: str, file_name: str, chunk: Chunk) -> str:
-    kb_file:KnowledgeBaseFile= get_kb_file(kb_name=kb_name, file_name=file_name)
+    kb_file: KnowledgeBaseFile = get_kb_file(kb_name=kb_name, file_name=file_name)
     kb_file.update_chunk(chunk=chunk)
-    kb:KnowledgeBase = get_knowledge_base(name=kb_name)
+    kb: KnowledgeBase = get_knowledge_base(name=kb_name)
     logger.debug(f"{chunk=}")
     kb.add_chunks2index(chunks=[chunk], meta_info=dict(file_name=file_name), do_save=True)
-    
+
 
 if __name__ == "__main__":
     # print(list_knowledge_base_names())
     # print(list_vecstores())
     # print(list_distance_strategy())
     # chunk_len = cut_kb_file(kb_name="new_kb", file_name="requirements.txt")
     # print(chunk_len)
```

### Comparing `xagent-0.0.9/xagents/kb/common.py` & `xagent-240513/xagents/kb/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,73 +3,90 @@
 '''
 @Time    :   2023/12/11 15:39:40
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
-
 import enum
 from pydantic import BaseModel, Field
 
 
-from typing import List, Tuple
+from typing import List, Optional, Tuple
 
 from xagents.loader.common import Chunk
 from xagents.config import *
 from langchain_core.documents import Document
 from snippets import *
 
+
 def get_kb_dir(kb_name) -> str:
     return os.path.join(KNOWLEDGE_BASE_DIR, kb_name)
 
-def get_chunk_dir(kb_name)->str:
+
+def get_chunk_dir(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "chunk")
-def get_origin_dir(kb_name)->str:
+
+
+def get_origin_dir(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "origin")
-def get_id_dir(kb_name)->str:
+
+
+def get_id_dir(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "id")
-def get_inverted_id_dir(kb_name)->str:
+
+
+def get_inverted_id_dir(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "inverted_id")
 
-def get_index_dir(kb_name, index_name="index")->str:
+
+def get_index_dir(kb_name, index_name="index") -> str:
     return os.path.join(get_kb_dir(kb_name), index_name)
 
-def get_inverted_index_dir(kb_name)->str:
+
+def get_inverted_index_dir(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "inverted_index")
-def get_config_path(kb_name)->str:
+
+
+def get_config_path(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "config.json")
 
+
 def get_chunk_path(kb_name, file_name) -> str:
     return os.path.join(get_chunk_dir(kb_name), file_name+".jsonl")
 
+
 def get_status_path(kb_name) -> str:
     return os.path.join(get_kb_dir(kb_name), "status.json")
 
+
 def get_origin_path(kb_name, file_name) -> str:
     return os.path.join(get_origin_dir(kb_name), file_name)
 
+
 def get_id_path(kb_name, file_name) -> str:
     return os.path.join(get_id_dir(kb_name), file_name+".jsonl")
+
+
 def get_inverted_id_path(kb_name, file_name) -> str:
     return os.path.join(get_inverted_id_dir(kb_name), file_name+".jsonl")
 
+
 class DistanceStrategy(str, enum.Enum):
     """Enumerator of the Distance strategies for calculating distances
     between vectors."""
 
     EUCLIDEAN_DISTANCE = "EUCLIDEAN_DISTANCE"
     MAX_INNER_PRODUCT = "MAX_INNER_PRODUCT"
 
 
-
 def chunk2document(chunk: Chunk, metadata: dict = dict()) -> Document:
     _metadata = copy.copy(metadata)
     if chunk.search_content:
-        page_content= chunk.search_content,
+        page_content = chunk.search_content,
         _metadata.update(content=chunk.content)
     else:
         page_content = chunk.content
     _metadata.update(page_idx=chunk.page_idx, id=chunk.id)
     return Document(page_content=page_content, metadata=_metadata)
 
 # # 知识库中的切片
@@ -105,45 +122,44 @@
     #     return hash(self) == hash(__value)
 
 
 # 召回的切片
 class RecalledChunk(Chunk):
     query: str = Field(description="召回chunk的query")
     score: float = Field(description="召回chunk的分数")
-    file_name:str = Field(description="知识库文件名称")
+    file_name: str = Field(description="知识库文件名称")
     forwards: List[Chunk] = Field(description="chunk的下文扩展", default=[])
     backwards: List[Chunk] = Field(description="chunk的上文扩展", default=[])
     index_cls: str = Field(description="索引类型", default=None)
 
     @classmethod
-    def from_document(cls, document: Document, query: str, score: float, index_cls:str) -> "RecalledChunk":
+    def from_document(cls, document: Document, query: str, score: float, index_cls: str) -> "RecalledChunk":
         """从langchain的Document构造过来
 
         Args:
             document (Document): langchain的Document
             query (str): 相关问题
             score (float): 召回得分
 
         Returns:
             _type_: RecalledChunk
         """
-    
+
         content = document.metadata.pop("content", None)
         item = dict(content=content, search_content=document.page_content) if content else dict(content=document.page_content)
         # logger.debug(f"meta:{document.metadata}")
         item.update(document.metadata)
         return cls(**item, query=query, score=score, index_cls=index_cls)
-    
+
     def __hash__(self) -> int:
         return hash((self.file_name, self.id))
 
     def __eq__(self, __value: object) -> bool:
         return hash(self) == hash(__value)
 
-
     def get_content(self):
         if self.search_content:
             return self.search_content + "\n" + self.content
 
         return self.content
 
     def to_plain_text(self):
@@ -185,29 +201,28 @@
         if forwards_len:
             forwards_str = "\n".join([f"{chunk.content}" for idx, chunk in enumerate(self.forwards)])
             if max_len:
                 forwards_str = forwards_str[:max_len]+"..."
             forwards_str = f"下文[{forwards_len}]字\n\n{forwards_str}"
 
         return backwards_str, forwards_str
+
     @property
     def total_len(self):
         return sum(len(c.content) for c in self.backwards+[self]+self.forwards)
 
 
-
 class KnowledgeBaseInfo(BaseModel):
     name: str = Field(description="知识库名称")
     desc: str = Field(description="知识库描述")
     embedding_config: dict = Field(description="embedding模型配置")
-    vecstore_config: dict|list[dict] = Field(description="向量存储配置")
-    file_num:int = Field(description="知识库文件数量")
-
+    vecstore_config: dict | list[dict] = Field(description="向量存储配置")
+    file_num: int = Field(description="知识库文件数量")
 
 
 # 知识库文件类
 class KnowledgeBaseFileInfo(BaseModel):
     kb_name: str = Field(description="知识库名称")
     file_name: str = Field(description="知识库文件名称")
-    is_cut:bool = Field(description="是否已经切片")
-    is_indexed:bool = Field(description="是否已经索引")
-
+    is_cut: bool = Field(description="是否已经切片")
+    is_indexed: bool = Field(description="是否已经索引")
+    chunk_num: Optional[int] = Field(description="切片数量", default=None)
```

### Comparing `xagent-0.0.9/xagents/kb/kb.py` & `xagent-240513/xagents/kb/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from xagents.model.api import get_embd_model, get_rerank_model
 from xagents.kb.common import KnowledgeBaseInfo, RecalledChunk, chunk2document, get_chunk_dir, get_chunk_path, get_config_path, get_index_dir, get_kb_dir, get_origin_dir, get_status_path
 from snippets import load, log_cost_time, dump, jload, jdump
 
 
 class KnowledgeBase():
 
-    def __init__(self, name: str, desc, embedding_config: dict, vecstore_config: dict|List[dict]):
+    def __init__(self, name: str, desc, embedding_config: dict, vecstore_config: dict | List[dict]):
         self.name = name
         self.desc = desc
         self.embedding_config = embedding_config
         self.vecstore_config = vecstore_config if isinstance(vecstore_config, list) else [vecstore_config]
         self.indexes = []
         self._build_dirs()
         self._save_config()
@@ -53,15 +53,15 @@
     def _build_dirs(self):
         self.kb_dir = get_kb_dir(self.name)
         self.origin_dir = get_origin_dir(self.name)
 
         self.chunk_dir = get_chunk_dir(self.name)
         self.config_path = get_config_path(self.name)
         self.status_path = get_status_path(self.name)
-        
+
         os.makedirs(self.origin_dir, exist_ok=True)
         os.makedirs(self.chunk_dir, exist_ok=True)
         if not os.path.exists(self.config_path):
             jdump(dict(), self.status_path)
 
     def _save_config(self):
         dump(self._get_config(), self.config_path)
@@ -81,105 +81,99 @@
                 if vecstore_cls.need_embd():
                     embedding_model = get_embd_model(self.embedding_config)
                     config.update(embedding=embedding_model)
                 if vecstore_cls == XES:
                     if "es_index" not in config:
                         config.update(es_index=f"{self.name}")
 
-                    
                 logger.debug(f"creating index:{vecstore_cls} with config:{config}")
                 index = vecstore_cls.from_config(config)
                 self.indexes.append(index)
         return self.indexes
-            
+
     def list_kb_files(self) -> List[KnowledgeBaseFile]:
         kb_files = []
         for file_name in os.listdir(self.origin_dir):
             kb_file = KnowledgeBaseFile(kb_name=self.name, file_name=file_name)
             kb_files.append(kb_file)
         return kb_files
 
     def remove_kb_file(self, kb_file: KnowledgeBaseFile):
         """
         删除文档
         """
         assert kb_file.kb_name == self.name
-        ## 从索引中删除
+        # 从索引中删除
         self.remove_kb_file_from_index(kb_file=kb_file)
         # 删除kb文件
         kb_file.delete()
 
     def remove_kb_file_from_index(self, kb_file: KnowledgeBaseFile):
         ids = kb_file.get_chunk_ids()
-        self.remove_chunks_from_index(ids)      
-            
+        self.remove_chunks_from_index(ids)
+
     def remove_chunks_from_index(self, chunk_ids):
         for index in self.get_indexes():
             logger.info(f"deleting {len(chunk_ids)} chunks from index:{index}")
-            index.delete(chunk_ids) 
+            index.delete(chunk_ids)
             if index.is_local():
                 index.save()
 
-    def add_chunks2index(self, chunks:List[Chunk], meta_info:dict, reindex=False, do_save=False, batch_size=16):
+    def add_chunks2index(self, chunks: List[Chunk], meta_info: dict, do_save=False, batch_size=16):
         indexes = self.get_indexes()
-        documents = [chunk2document(chunk, meta_info) for chunk in chunks if chunk.content]
+        chunks = [chunk for chunk in chunks if chunk.content]
+        documents = [chunk2document(chunk, meta_info) for chunk in chunks]
 
-        ids = [chunk.id for chunk in chunks if chunk.content]
-        # 添加新的index        
+        ids = [chunk.id for chunk in chunks]
+        # 添加新的index
         for index in indexes:
             embd_model = index.embeddings
             if embd_model:
                 if hasattr(embd_model, "batch_size"):
                     logger.debug(f"setting embedding model batch size to {batch_size}")
                     setattr(embd_model, "batch_size", batch_size)
                 else:
-                    logger.warning(f"{embd_model.__class__} has no attribute batch_size, set to default value {batch_size}") 
+                    logger.warning(f"{embd_model.__class__} has no attribute batch_size, set to default value {batch_size}")
             logger.debug(f"updating {len(ids)} documents to index:{index}")
             index.delete(ids=ids)
             index.add_documents(documents=documents, ids=ids)
 
             if index.is_local() and do_save:
-                
-            # TODO 为何isinstance判断不work？
-            # if isinstance(index, LocalVecStore) and do_save:
                 logger.info(f"saving to index dir:{index.local_dir}")
                 index.save()
-        
 
-    def add_kb_file2index(self,  kb_file: KnowledgeBaseFile, reindex=False, do_save=False, batch_size=16):
+    def add_kb_file2index(self,  kb_file: KnowledgeBaseFile, do_save=False, batch_size=16):
         if not kb_file.is_cut:
             logger.warning(f"{kb_file.file_name} is not cut, please cut it first")
             return
         chunks = kb_file.list_chunks()
         kb_file.set_index_status(False)
-        self.add_chunks2index(chunks=chunks, meta_info=dict(file_name=kb_file.file_name), reindex=reindex, do_save=do_save, batch_size=batch_size)
+        self.add_chunks2index(chunks=chunks, meta_info=dict(file_name=kb_file.file_name), do_save=do_save, batch_size=batch_size)
         kb_file.set_index_status(True)
 
     @log_cost_time(name="rebuild_index")
-    def rebuild_index(self, reindex:bool, batch_size:int):
+    def rebuild_index(self, batch_size: int):
         """
         重新构建向量知识库
         """
         indexes = self.get_indexes()
         kb_files = self.list_kb_files()
         for kb_file in kb_files:
-            self.add_kb_file2index(kb_file=kb_file, reindex=reindex, do_save=False, batch_size=batch_size)
+            self.add_kb_file2index(kb_file=kb_file, do_save=False, batch_size=batch_size)
         for index in indexes:
             if isinstance(index, LocalVecStore):
                 index.save()
-                
+
     def delete(self):
         """删除知识库"""
         for index in self.get_indexes():
             index.delete_all()
         import shutil
         shutil.rmtree(path=self.kb_dir)
 
-
-
     @log_cost_time(name="kb_search")
     def search(self, query: str, top_k: int = 3, score_threshold: float = None,
                do_split_query=False, file_names: List[str] = None, rerank_config: dict = {},
                do_expand=False, expand_len: int = 500, forward_rate: float = 0.5) -> List[RecalledChunk]:
         """知识库检索
 
         Args:
@@ -203,29 +197,30 @@
         _filter = dict()
         if file_names:
             _filter = dict(file_name=file_names)
 
         # 每个子query做检索
         indexes = self.get_indexes()
         for query in queries:
-            
+
             for index in indexes:
                 score_threshold = index.convert_score(score_threshold)
                 logger.debug(f"searching {query} with vecstore_cls: {index.__class__.__name__}, {_filter=}, {top_k=}, {score_threshold=}")
                 docs_with_score = index.similarity_search_with_score(query, k=top_k, score_threshold=score_threshold, filter=_filter)
                 logger.debug(f"{docs_with_score=}")
-                tmp_recalled_chunks = [RecalledChunk.from_document(d, score= index.convert_score(s), query=query, index_cls=index.__class__.__name__) for d, s in docs_with_score]
+                tmp_recalled_chunks = [RecalledChunk.from_document(d, score=index.convert_score(
+                    s), query=query, index_cls=index.__class__.__name__) for d, s in docs_with_score]
                 recalled_chunks.extend(tmp_recalled_chunks)
 
         # 去重，避免召回相同切片
         origin_recall_num = len(recalled_chunks)
-        recalled_chunks = list(sorted(set(recalled_chunks), key=lambda x:x.score, reverse=True))
+        recalled_chunks = list(sorted(set(recalled_chunks), key=lambda x: x.score, reverse=True))
         logger.info(f"{len(recalled_chunks)} distinct recalled from {len(queries)} queries and {len(indexes)} indexes, {origin_recall_num-len(recalled_chunks)} duplicated")
 
-        #精排
+        # 精排
         if rerank_config:
             recalled_chunks = rerank(recalled_chunks, rerank_config)
         recalled_chunks = recalled_chunks[:top_k]
         logger.info(f"get {len(recalled_chunks)} reranked chunks after sort")
 
         # 上下文扩展
         if do_expand:
@@ -251,39 +246,40 @@
         for chunk in recalled_chunks:
             similarity = rerank_model.cal_similarity(chunk.query, chunk.content)
             chunk.score = similarity
 
     recalled_chunks.sort(key=lambda x: x.score, reverse=True)
     return recalled_chunks
 
+
 def split_query(query: str, do_split_query=False) -> List[str]:
     """切割query"""
     if do_split_query:
         rs = [e.strip() for e in re.split("\?|？", query) if e.strip()]
         logger.debug(f"split origin query into {len(rs)} queries")
 
         return rs
     else:
         # 不需要切分也转成list形式，方便后续统一处理
         return [query]
 
 
 # 扩展上下文到给定的长度
-#TODO 扩展时，避免重复的chunk
-def expand_chunk(chunk: RecalledChunk, kb_name:str, expand_len: int, forward_rate=0.5) -> RecalledChunk:
+# TODO 扩展时，避免重复的chunk
+def expand_chunk(chunk: RecalledChunk, kb_name: str, expand_len: int, forward_rate=0.5) -> RecalledChunk:
     logger.debug(f"expanding chunk {chunk}")
     chunk_path = get_chunk_path(kb_name, chunk.file_name)
     chunk_dicts = load(chunk_path)
     chunk_idx = None
-    
+
     for idx, ele in enumerate(chunk_dicts):
         if ele["id"] == chunk.id:
             chunk_idx = idx
             break
-        
+
     if chunk_idx is None:
         logger.warning(f"chunk {chunk} not found in {chunk_path}")
         return chunk
 
     to_expand = expand_len - len(chunk.content)
     if to_expand <= 0:
         return chunk
@@ -293,37 +289,37 @@
     logger.debug(f"expand chunk with :{forward_len=}, {backward_len=}, origin_len:{len(chunk.content)}")
     backwards, forwards = [], []
 
     # 查找前面的chunk
     idx = chunk_idx-1
     while idx >= 0:
         if backward_len <= 0:
-            break        
+            break
         tmp_chunk = copy.copy(chunk_dicts[idx])
-        if tmp_chunk["content_type"] ==ContentType.TEXT:
-            chunk_len = min (len(tmp_chunk["content"]), backward_len)
+        if tmp_chunk["content_type"] == ContentType.TEXT:
+            chunk_len = min(len(tmp_chunk["content"]), backward_len)
             tmp_chunk["content"] = tmp_chunk["content"][-chunk_len:]
-            to_add:Chunk = Chunk(**tmp_chunk)
+            to_add: Chunk = Chunk(**tmp_chunk)
             backwards.append(to_add)
             backward_len -= chunk_len
         idx -= 1
-        
+
     backwards.reverse()
 
     idx = chunk_idx + 1
-    # logger.debug(f"{idx=}, {len(chunk_dicts)=}, {forward_len=}") 
+    # logger.debug(f"{idx=}, {len(chunk_dicts)=}, {forward_len=}")
     while idx < len(chunk_dicts):
         if forward_len <= 0:
-            break        
+            break
 
         tmp_chunk = copy.copy(chunk_dicts[idx])
-        if tmp_chunk["content_type"] ==ContentType.TEXT:
-            chunk_len = min (len(tmp_chunk["content"]), forward_len)
+        if tmp_chunk["content_type"] == ContentType.TEXT:
+            chunk_len = min(len(tmp_chunk["content"]), forward_len)
             tmp_chunk["content"] = tmp_chunk["content"][:chunk_len]
-            to_add:Chunk = Chunk(**tmp_chunk)
+            to_add: Chunk = Chunk(**tmp_chunk)
             forwards.append(to_add)
             forward_len -= chunk_len
         idx += 1
 
     chunk.backwards = backwards
     chunk.forwards = forwards
     logger.debug(f"expand done with {len(backwards)} backward chunks and {len(forwards)} forward chunks, total_len:{chunk.total_len}")
```

### Comparing `xagent-0.0.9/xagents/kb/kb_file.py` & `xagent-240513/xagents/kb/kb_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,47 +25,46 @@
         self.chunk_path = get_chunk_path(self.kb_name, self.file_name)
         self.origin_path = get_origin_path(self.kb_name, self.file_name)
 
     @property
     def is_cut(self) -> bool:
         return os.path.exists(self.chunk_path)
 
-
     @property
     def chunk_num(self) -> int:
         if not self.is_cut:
             return 0
         chunks = load(self.chunk_path)
         return len(chunks)
-    
-    def set_index_status(self, is_indexed:bool):
+
+    def set_index_status(self, is_indexed: bool):
         logger.debug(f"setting {self.file_name}'s is_indexed value to {is_indexed}")
         status_path = get_status_path(self.kb_name)
         status = jload(status_path)
         if self.file_name not in status:
             status[self.file_name] = {}
-        status[self.file_name]["indexed"] = is_indexed      
-        logger.debug(f"{status=}")   
+        status[self.file_name]["indexed"] = is_indexed
+        # logger.debug(f"{status=}")
         jdump(status, status_path)
-        
 
     @property
-    def is_indexed(self)->bool:
+    def is_indexed(self) -> bool:
         status_path = get_status_path(self.kb_name)
         rs = jload(status_path).get(self.file_name, {}).get("indexed", False)
         return rs
-        
+
     def get_info(self):
-        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut, is_indexed=self.is_indexed)
+        return KnowledgeBaseFileInfo(kb_name=self.kb_name, file_name=self.file_name, is_cut=self.is_cut, chunk_num=self.chunk_num, is_indexed=self.is_indexed)
 
     def cut(self, *args, **kwargs) -> List[Chunk]:
         logger.info(f"start cut file: {self.file_name}")
         chunks: List[Chunk] = parse_file(file_path=self.origin_path, *args, **kwargs)
         self._save_chunks(chunks=chunks)
-    
+        return len(chunks)
+
     def _save_chunks(self, chunks: List[Chunk]):
         chunk_json = [chunk.to_json() for chunk in chunks]
         dump(chunk_json, self.chunk_path)
         return chunks
 
     def list_chunks(self) -> List[Chunk]:
         """
@@ -79,44 +78,43 @@
         chunks = [Chunk.from_dict(ele) for ele in chunk_dicts]
         return chunks
 
     def get_chunk_ids(self) -> List[str]:
         chunks = self.list_chunks()
         chunk_ids = [c.id for c in chunks]
         return chunk_ids
-    
+
     def get_chunk(self, idx: int) -> Chunk:
         chunks = self.list_chunks()
         if idx < 0 or idx >= len(chunks):
             raise Exception(f"chunk index out of range, idx: {idx}, len: {len(chunks)}")
-        return chunks[idx]  
+        return chunks[idx]
 
-    def add_chunks(self, chunks: List[Chunk], idx:int= None):
+    def add_chunks(self, chunks: List[Chunk], idx: int = None):
         origin_chunks = self.list_chunks()
         if idx is None:
             idx = len(chunks)
         chunks = origin_chunks[:idx] + chunks + origin_chunks[idx:]
         self._save_chunks(chunks)
 
-    def delete_chunks(self, ids:List[str]):
+    def delete_chunks(self, ids: List[str]):
         chunks = self.list_chunks()
         remain_chunks = [c for c in chunks if c.id not in ids]
         self._save_chunks(remain_chunks)
 
-    
-    def update_chunk(self, chunk:Chunk)->bool:
+    def update_chunk(self, chunk: Chunk) -> bool:
         # do delete
-        
+
         chunks = self.list_chunks()
         for idx, c in enumerate(chunks):
             if c.id == chunk.id:
                 chunks[idx] = chunk
                 break
         self._save_chunks(chunks)
-    
+
     def delete(self):
         """
         删除知识库文档
         """
         for path in [self.origin_path, self.chunk_path]:
             if os.path.exists(path):
                 os.remove(path)
```

### Comparing `xagent-0.0.9/xagents/kb/vector_store.py` & `xagent-240513/xagents/kb/vector_store.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/api.py` & `xagent-240513/xagents/loader/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from loguru import logger
 from typing import Iterable, List, Type
 from xagents.loader.pdf_loader import PDFLoader
 from xagents.loader.docx_loader import DOCXLoader
 from xagents.loader.doc_loader import DOCLoader
 from xagents.loader.csv_loader import CSVLoader
 from xagents.loader.excel_loader import EXCELLoader
+from xagents.loader.xls_loader import XLSLoader
 from xagents.loader.pptx_loader import PPTXLoader
 from xagents.loader.ppt_loader import PPTLoader
 
 from xagents.loader.markdown_loader import MarkDownLoader
 from xagents.loader.json_loader import JSONLoader
 from xagents.loader.jsonl_loader import JSONLLoader
 from xagents.loader.common import Chunk, AbstractLoader
@@ -30,14 +31,15 @@
     "pdf": PDFLoader,
     "markdown": MarkDownLoader,
     "md": MarkDownLoader,
     "json": JSONLoader,
     "jsonl": JSONLLoader,
     "csv": CSVLoader,
     "xlsx": EXCELLoader,
+    "xls": XLSLoader,
     "txt": MarkDownLoader,
     "docx": DOCXLoader,
     "doc": DOCLoader,
     "pptx": PPTXLoader,
     "ppt": PPTLoader,
     "": MarkDownLoader
 }
```

### Comparing `xagent-0.0.9/xagents/loader/common.py` & `xagent-240513/xagents/loader/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 from abc import abstractmethod
 import enum
+import time
 import uuid
 from pathlib import Path
 from typing import Iterable, List, Optional, Tuple
 
 from pydantic import BaseModel, Field, ConfigDict, validator
 from pandas import DataFrame
 from numpy import ndarray
@@ -121,15 +122,15 @@
             yield chunk
     if acc:
         yield TextChunk(content=acc, page_idx=cur_page_idx)
             
     
 
 def get_image_name_path(kf_file_name:str, page_idx:int, image_idx:int)->Tuple[str, str]:
-    image_name =f"{Path(kf_file_name).stem}-page{page_idx}-image{image_idx}.png"
+    image_name =f"{Path(kf_file_name).stem}-page{page_idx}-image{image_idx}-time{time.time()}.png"
     file_path = os.path.join(TEMP_DIR, "extracted_images", image_name)
     os.makedirs(os.path.dirname(file_path), exist_ok=True)
     return image_name, file_path
 
 def data2markdown(data:ndarray|DataFrame)->str:
     if isinstance(data, ndarray):
         data = DataFrame(data)
```

### Comparing `xagent-0.0.9/xagents/loader/csv_loader.py` & `xagent-240513/xagents/loader/csv_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/doc_loader.py` & `xagent-240513/xagents/loader/doc_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/docx_loader.py` & `xagent-240513/xagents/loader/docx_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/excel_loader.py` & `xagent-240513/xagents/loader/excel_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/json_loader.py` & `xagent-240513/xagents/loader/json_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/jsonl_loader.py` & `xagent-240513/xagents/loader/jsonl_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/markdown_loader.py` & `xagent-240513/xagents/loader/markdown_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/pdf_loader.py` & `xagent-240513/xagents/loader/pdf_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,22 +13,20 @@
 
 from xagents.loader.utils import upload_to_minio, image2text
 from xagents.config import *
 from xagents.loader.common import BBox, Chunk, TableChunk, TextChunk, ImageChunk, get_image_name_path, merge_chunks, AbstractLoader
 from pdfplumber.page import Page
 
 
+def analyse_page(idx: int, page: Page, file_name: str, upload_image: bool, ocr: bool) -> Iterable[Chunk]:
 
-
-def analyse_page(idx:int, page:Page, file_name:str, upload_image:bool, ocr:bool)->Iterable[Chunk]:
-            
-    chunks:List[Tuple[Chunk, BBox]] = []  # List to store all content with their position
+    chunks: List[Tuple[Chunk, BBox]] = []  # List to store all content with their position
 
     # 抽取文本
-    for line in  page.extract_text_lines(x_tolerance=3, y_tolerance=3):
+    for line in page.extract_text_lines(x_tolerance=3, y_tolerance=3):
         chunks.append((TextChunk(content=line['text'], page_idx=idx), BBox(x0=line["x0"], y0=line["top"], x1=line["x1"], y1=line["bottom"])))
 
     tables = page.extract_tables()
     for table in tables:
         bbox = BBox(x0=0, x1=0, y0=0, y1=0)
         # logger.info(f"table: {table}")
 
@@ -37,57 +35,52 @@
 
     # Extract images and add to content list
     page_image = page.to_image().original
     for i, image in enumerate(page.images):
         bbox = BBox(x0=image['x0'], y0=image['top'], x1=image['x1'], y1=image['bottom'])
         # pil_image = Image.open(page_image.annotated)
         image = page_image.crop(bbox.to_tuple())
-        
-        
-        image_name, image_path =get_image_name_path(file_name, idx, i)     
+
+        image_name, image_path = get_image_name_path(file_name, idx, i)
         if upload_image:
             os.makedirs(os.path.dirname(image_path), exist_ok=True)
             image.save(image_path, format="PNG")
-            url= upload_to_minio(image_path)
+            url = upload_to_minio(image_path)
         else:
-            url=None
+            url = None
         if ocr:
             content = image2text(image)
         else:
             content = None
         chunks.append((ImageChunk(url=url, content=content, image_name=image_name, page_idx=idx), bbox))
-        
+
     chunks.sort(key=lambda x: x[1].sort_key)  # Sort by top y coordinate, then by left x coordinate
     yield from (x[0] for x in chunks)
 
 
-
 class PDFLoader(AbstractLoader):
     def load(self, file_path: str, start_page=1, end_page=None, upload_image=True, ocr=False) -> Iterable[Chunk]:
         import pdfplumber
 
-        logger.info(f"loading pdf file {file_path} from {start_page} to {end_page}, {upload_image=}, {ocr=}")
+        logger.info(f"loading pdf file {file_path} from {start_page=} to {end_page=}, {upload_image=}, {ocr=}")
         pages = pdfplumber.open(file_path)
         for idx, page in enumerate(pages.pages, start=1):
             if idx < start_page:
                 continue
             if end_page and idx > end_page:
                 break
             chunks = analyse_page(idx, page, os.path.basename(file_path), upload_image=upload_image, ocr=ocr)
             yield from merge_chunks(chunks=chunks)
 
-            
-
 
 if __name__ == "__main__":
     from xagents.config import XAGENT_HOME
     import sys
     import pdfplumber
     logger.add(sys.stdout)
     doc_path = os.path.join(XAGENT_HOME, "data/kb_file/image_table.pdf")
     pages = pdfplumber.open(doc_path)
     pages = list(pages.pages)
     contents = analyse_page(pages[4])
     for content in contents:
-        
-        print(content)    
 
+        print(content)
```

### Comparing `xagent-0.0.9/xagents/loader/ppt_loader.py` & `xagent-240513/xagents/loader/ppt_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/pptx_loader.py` & `xagent-240513/xagents/loader/pptx_loader.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/structed.py` & `xagent-240513/xagents/loader/structed.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/loader/utils.py` & `xagent-240513/xagents/loader/utils.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/model/api.py` & `xagent-240513/xagents/model/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/model/common.py` & `xagent-240513/xagents/model/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,44 +13,47 @@
 from agit.llm import LLMResp
 from agit.common import ToolCall
 
 from langchain_core.embeddings import Embeddings
 from pydantic import BaseModel, Field
 
 
-
-
 StrOrGen = Union[str, Generator]
 
+
 class LLMGenConfig(BaseModel):
-    system:Optional[str] = Field(description="系统信息", default=None)
+    system: Optional[str] = Field(description="系统信息", default=None)
     temperature: float = Field(default=0.95, ge=0, le=1, description="生成文本的温度")
     top_p: float = Field(default=0.7, ge=0, le=1, description="生成文本的top_p")
+    max_tokens: int = Field(default=2048, ge=1, description="生成文本的最大长度")
+    do_sample: bool = Field(default=True, description="是否使用采样")
+
 
 class LLMGen(BaseModel):
     content: StrOrGen = Field(description="生成的文本内容, 字符串或生成器")
     tool_call: Optional[ToolCall] = Field(description="工具调用")
     detail: dict = Field()
-    
+
 
 class LLM:
     """语言模型的基类
     """
-    def __init__(self, version: str, name: str=None):
+
+    def __init__(self, version: str, name: str = None):
         """初始化函数
 
         Args:
             name (str): LLM的名称
             version (str): 模型版本
         """
-        self.name = name if name else self.__class__.__name__ +"-" + version
+        self.name = name if name else self.__class__.__name__ + "-" + version
         self.version = version
 
     @abstractmethod
-    def generate(self, prompt:str, history=[], system:str=None, stream=True, **kwargs)->LLMResp:
+    def generate(self, prompt: str, history=[], system: str = None, stream=True, **kwargs) -> LLMResp:
         """生成结果
 
         Args:
             prompt (str): 给LLM的提示词
             history (list, optional): 历史message列表. Defaults to [].
             system (_type_, optional): system信息. Defaults to None.
             stream (bool, optional): 是否返回generator. Defaults to True.
@@ -58,30 +61,28 @@
             Tuple[ToolCall,StrOrGen]: ToolCall:工具调用实例，可以为空, StrOrGen:模型回复内容，字符串或generator
         """
         raise NotImplementedError
 
     @classmethod
     def list_version(cls):
         raise NotImplementedError
-    
+
     def __str__(self):
         return f"[{self.name}]-{self.version}"
 
     def __repr__(self):
         return self.__str__()
 
 
 class EMBD(Embeddings):
     def get_dim(self) -> int:
         raise NotImplementedError
 
+
 class Reranker:
     def __init__(self, name: str, version: str):
         self.name = name
         self.version = version
 
     @abstractmethod
-    def cal_similarity(self, text1:str, text2:str)->float:
+    def cal_similarity(self, text1: str, text2: str) -> float:
         raise NotImplementedError
-
-    
-
```

### Comparing `xagent-0.0.9/xagents/model/local.py` & `xagent-240513/xagents/model/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def __init__(self,  url="http://hz-model.bigmodel.cn/embedding-models/v2/embeddings", batch_size=16, norm=True, dim=1024):
         self.batch_size = batch_size
         self.norm = norm
         self.url = url
         self.dim=dim
 
     def embed_documents(self, texts: List[str]) -> List[List[float]]:
-        logger.info(f"embedding {len(texts)} with {self.batch_size=}")
+        logger.info(f"embedding {len(texts)} texts with {self.batch_size=}")
         embeddings = call_embedding(text=texts,model_or_url=self.url, embd_type=EMBD_TYPE.LOCAL,
                                     norm=self.norm, batch_size=self.batch_size)
         
         return embeddings
 
     def embed_query(self, text: str) -> List[float]:
         embedding = call_embedding(text=text,model_or_url=self.url, embd_type=EMBD_TYPE.LOCAL,
```

### Comparing `xagent-0.0.9/xagents/model/openai.py` & `xagent-240513/xagents/model/openai.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/model/zhipu.py` & `xagent-240513/xagents/model/zhipu.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/tool/api.py` & `xagent-240513/xagents/tool/api.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/tool/common_tool.py` & `xagent-240513/xagents/tool/common_tool.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/tool/web_search.py` & `xagent-240513/xagents/tool/web_search.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.9/xagents/util.py` & `xagent-240513/xagents/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
 
 from functools import wraps
 from typing import Callable
 
 from fastapi.params import Body
 
-from loguru import logger
 
-
-def parse_body(func:Callable):
+def parse_body(func: Callable):
     @wraps(func)
     def wrapped(**kwargs):
         print(f"{kwargs=}")
-        for k,v in kwargs.items():
+        for k, v in kwargs.items():
             if isinstance(v, Body):
                 kwargs[k] = v.default
         return func(**kwargs)
     return wrapped
 
 
-
-
+def save_format(template: str, **kwargs):
+    for k, v in kwargs.items():
+        template = template.replace(k, v)
+    return template
```

