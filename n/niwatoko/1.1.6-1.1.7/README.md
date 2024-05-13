# Comparing `tmp/niwatoko-1.1.6.tar.gz` & `tmp/niwatoko-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niwatoko-1.1.6.tar", last modified: Sat May 11 23:28:44 2024, max compression
+gzip compressed data, was "niwatoko-1.1.7.tar", last modified: Mon May 13 18:17:32 2024, max compression
```

## Comparing `niwatoko-1.1.6.tar` & `niwatoko-1.1.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.232966 niwatoko-1.1.6/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.6/LICENSE
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 23:28:44.232694 niwatoko-1.1.6/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-11 04:01:06.000000 niwatoko-1.1.6/README.md
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.225777 niwatoko-1.1.6/niwatoko/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.6/niwatoko/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     9002 2024-05-11 23:27:49.000000 niwatoko-1.1.6/niwatoko/cli.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.224492 niwatoko-1.1.6/niwatoko/foundation_model/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.224529 niwatoko-1.1.6/niwatoko/foundation_model/interpretation/
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.226961 niwatoko-1.1.6/niwatoko/foundation_model/interpretation/llm/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.6/niwatoko/foundation_model/interpretation/llm/claude.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1428 2024-05-08 23:04:24.000000 niwatoko-1.1.6/niwatoko/foundation_model/interpretation/llm/gpt.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.227237 niwatoko-1.1.6/niwatoko/grammar/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.6/niwatoko/grammar/system.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.6/niwatoko/temp.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.226579 niwatoko-1.1.6/niwatoko.egg-info/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/PKG-INFO
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/SOURCES.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/dependency_links.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/entry_points.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/requires.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-11 23:28:44.000000 niwatoko-1.1.6/niwatoko.egg-info/top_level.txt
--rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-11 23:28:44.233017 niwatoko-1.1.6/setup.cfg
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-11 23:28:34.000000 niwatoko-1.1.6/setup.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.228896 niwatoko-1.1.6/tests/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.6/tests/README.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.6/tests/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.6/tests/test_compiler.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.6/tests/test_compiler.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.6/tests/test_compiler_v1_2.py
-drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-11 23:28:44.232265 niwatoko-1.1.6/tests/test_docs/
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.6/tests/test_docs/__init__.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.6/tests/test_docs/output copy.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-11 00:55:54.000000 niwatoko-1.1.6/tests/test_docs/output.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-11 00:56:05.000000 niwatoko-1.1.6/tests/test_docs/output.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.6/tests/test_docs/output_.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.6/tests/test_docs/test_doc1.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.6/tests/test_docs/test_doc2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.6/tests/test_docs/test_doc3.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.6/tests/test_docs/test_gen_github_issue.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.6/tests/test_docs/test_gen_grimoire.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.6/tests/test_docs/test_gen_grimoire2.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.6/tests/test_docs/test_gen_grimoire_en.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.6/tests/test_docs/test_gen_zoltraak_pypi.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.6/tests/test_docs/test_import_function.md
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.6/tests/test_interpreter.py
--rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.6/tests/test_parser.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.883598 niwatoko-1.1.7/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    11356 2024-05-07 05:52:57.000000 niwatoko-1.1.7/LICENSE
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-13 18:17:32.883193 niwatoko-1.1.7/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    15972 2024-05-11 04:01:06.000000 niwatoko-1.1.7/README.md
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.874852 niwatoko-1.1.7/niwatoko/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      166 2024-05-07 22:46:07.000000 niwatoko-1.1.7/niwatoko/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     9359 2024-05-13 18:14:42.000000 niwatoko-1.1.7/niwatoko/cli.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.873567 niwatoko-1.1.7/niwatoko/foundation_model/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.873604 niwatoko-1.1.7/niwatoko/foundation_model/interpretation/
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.876089 niwatoko-1.1.7/niwatoko/foundation_model/interpretation/llm/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1346 2024-05-08 23:04:24.000000 niwatoko-1.1.7/niwatoko/foundation_model/interpretation/llm/claude.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2266 2024-05-13 18:02:08.000000 niwatoko-1.1.7/niwatoko/foundation_model/interpretation/llm/gpt.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.876462 niwatoko-1.1.7/niwatoko/grammar/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)      685 2024-05-08 23:04:24.000000 niwatoko-1.1.7/niwatoko/grammar/system.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       33 2024-05-11 00:20:33.000000 niwatoko-1.1.7/niwatoko/temp.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.875744 niwatoko-1.1.7/niwatoko.egg-info/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)    16858 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/PKG-INFO
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1026 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/SOURCES.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)        1 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/dependency_links.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       47 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/entry_points.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       34 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/requires.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       15 2024-05-13 18:17:32.000000 niwatoko-1.1.7/niwatoko.egg-info/top_level.txt
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)       38 2024-05-13 18:17:32.883636 niwatoko-1.1.7/setup.cfg
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1697 2024-05-13 18:16:59.000000 niwatoko-1.1.7/setup.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.878999 niwatoko-1.1.7/tests/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5897 2024-05-08 23:04:24.000000 niwatoko-1.1.7/tests/README.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2077 2024-05-07 02:46:41.000000 niwatoko-1.1.7/tests/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3754 2024-05-08 23:03:26.000000 niwatoko-1.1.7/tests/test_compiler.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4529 2024-05-08 23:03:26.000000 niwatoko-1.1.7/tests/test_compiler.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3940 2024-05-08 23:04:26.000000 niwatoko-1.1.7/tests/test_compiler_v1_2.py
+drwxr-xr-x   0 motokidaisuke   (501) staff       (20)        0 2024-05-13 18:17:32.882632 niwatoko-1.1.7/tests/test_docs/
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2747 2024-05-07 02:46:41.000000 niwatoko-1.1.7/tests/test_docs/__init__.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2030 2024-05-11 00:20:33.000000 niwatoko-1.1.7/tests/test_docs/output copy.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     3118 2024-05-11 00:55:54.000000 niwatoko-1.1.7/tests/test_docs/output.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     4172 2024-05-11 00:56:05.000000 niwatoko-1.1.7/tests/test_docs/output.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1733 2024-05-11 00:20:33.000000 niwatoko-1.1.7/tests/test_docs/output_.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2609 2024-05-07 05:48:44.000000 niwatoko-1.1.7/tests/test_docs/test_doc1.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2853 2024-05-07 05:48:44.000000 niwatoko-1.1.7/tests/test_docs/test_doc2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2625 2024-05-07 05:48:44.000000 niwatoko-1.1.7/tests/test_docs/test_doc3.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1678 2024-05-07 22:46:07.000000 niwatoko-1.1.7/tests/test_docs/test_gen_github_issue.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1950 2024-05-07 22:46:07.000000 niwatoko-1.1.7/tests/test_docs/test_gen_grimoire.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1909 2024-05-07 22:46:07.000000 niwatoko-1.1.7/tests/test_docs/test_gen_grimoire2.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     1850 2024-05-07 22:46:07.000000 niwatoko-1.1.7/tests/test_docs/test_gen_grimoire_en.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     5307 2024-05-07 05:52:23.000000 niwatoko-1.1.7/tests/test_docs/test_gen_zoltraak_pypi.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     6179 2024-05-11 00:20:33.000000 niwatoko-1.1.7/tests/test_docs/test_import_function.md
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2216 2024-05-07 02:46:41.000000 niwatoko-1.1.7/tests/test_interpreter.py
+-rw-r--r--   0 motokidaisuke   (501) staff       (20)     2632 2024-05-07 02:46:41.000000 niwatoko-1.1.7/tests/test_parser.py
```

### Comparing `niwatoko-1.1.6/LICENSE` & `niwatoko-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/PKG-INFO` & `niwatoko-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.6
+Version: 1.1.7
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.6/README.md` & `niwatoko-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/niwatoko/cli.py` & `niwatoko-1.1.7/niwatoko/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import subprocess
 import click
 import os
 from niwatoko.foundation_model.interpretation.llm.claude import generate_response
 from niwatoko.foundation_model.interpretation.llm.gpt import generate_response as gpt_generate_response
+from niwatoko.foundation_model.interpretation.llm.gpt import generate_response_gpt4o as gpt_generate_response_gpt4o
 import niwatoko
 import re
 from tqdm import tqdm
 import itertools
 import threading
 import sys
 import time
 
 @click.command()
 @click.argument('file_path', type=click.Path(exists=True), required=False)
-@click.option('-m', '--model', type=click.Choice(['openai', 'claude', 'claude-sonnet', 'claude-opus', 'claude-haiku']), default='claude-haiku', help='使用するモデルを選択します。')
+@click.option('-m', '--model', type=click.Choice(['openai', 'openai-gpt4o', 'claude', 'claude-sonnet', 'claude-opus', 'claude-haiku']), default='claude-haiku', help='使用するモデルを選択します。')
 @click.option('-o', '--output', type=click.Path(), help='生成されたコードの出力先ファイルを指定します。')
 @click.option('-v', '--version',  is_flag=True, help='バージョン情報を表示します。')
 
 def main(file_path, model, output, version):
     # print("file_path:", file_path)
     """
     自然言語のソースコードを読み込んで実行するコマンドラインインターフェース。
@@ -43,21 +44,27 @@
     print("実行中... (Processing...)")
 
     # ぐるぐるアニメーションを表示するスレッドを開始
     done = False
     spinner = threading.Thread(target=spin, args=(lambda: done,))
     spinner.start()
 
-    if model == 'openai':
+    if model == 'openai' or model == 'openai-gpt-turbo':
         generated_code = gpt_generate_response(
             model="gpt-4-turbo-2024-04-09",
             prompt=processed_content,
             max_tokens=1000,
             temperature=0.5,
         )
+    elif model == 'openai-gpt4o':
+        generated_code = gpt_generate_response_gpt4o(
+            prompt=processed_content,
+            max_tokens=2048,
+            temperature=0.5,
+        )
     else:
         if model == 'claude-sonnet':
             claude_model = 'claude-3-sonnet-20240229'
         elif model == 'claude-opus':
             claude_model = 'claude-3-opus-20240229'
         else:
             claude_model = 'claude-3-haiku-20240307'  # デフォルトはhaiku
```

### Comparing `niwatoko-1.1.6/niwatoko/foundation_model/interpretation/llm/claude.py` & `niwatoko-1.1.7/niwatoko/foundation_model/interpretation/llm/claude.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/niwatoko/foundation_model/interpretation/llm/gpt.py` & `niwatoko-1.1.7/niwatoko/foundation_model/interpretation/llm/gpt.py`

 * *Files 22% similar despite different names*

```diff
@@ -36,7 +36,31 @@
         messages=[
             {"role": "system", "content": system_prompt},
             {"role": "user", "content": prompt}
         ]
     )
 
     return chat_completion.choices[0].message.content.strip()
+
+def generate_response_gpt4o(prompt, max_tokens, temperature):
+    """
+    OpenAI APIを使用してGPT-4oモデルでプロンプトに対する応答を生成する関数。
+
+    Args:
+        prompt (str): 応答を生成するためのプロンプト。
+        max_tokens (int): 生成する最大トークン数。
+        temperature (float): 生成時のランダム性を制御する温度パラメータ（0から1の範囲）。
+
+    Returns:
+        str: 生成された応答テキスト。
+    """
+    response = client.chat.completions.create(
+        model="gpt-4o",
+        messages=[{"role": "user", "content": prompt}],
+        temperature=temperature,
+        max_tokens=max_tokens,
+        top_p=1,
+        frequency_penalty=0,
+        presence_penalty=0
+    )
+
+    return response.choices[0].message.content.strip()
```

### Comparing `niwatoko-1.1.6/niwatoko/grammar/system.md` & `niwatoko-1.1.7/niwatoko/grammar/system.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/niwatoko.egg-info/PKG-INFO` & `niwatoko-1.1.7/niwatoko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niwatoko
-Version: 1.1.6
+Version: 1.1.7
 Summary: 自然言語でプログラミングを行うことができる新しいプログラミング言語
 Home-page: https://niwatoko2.vercel.app/
 Author: dai-motoki
 Author-email: dai.motoki1123@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Japanese
```

### Comparing `niwatoko-1.1.6/niwatoko.egg-info/SOURCES.txt` & `niwatoko-1.1.7/niwatoko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/setup.py` & `niwatoko-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # niwatoko - 自然言語プログラミング言語のPythonパッケージのsetup.pyファイルです。
 # このファイルはパッケージのインストールや配布に必要な情報を含んでいます。
 
 from setuptools import setup, find_packages
 
 setup(
     name='niwatoko',
-    version='1.1.6',
+    version='1.1.7',
     description='自然言語でプログラミングを行うことができる新しいプログラミング言語',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='dai-motoki',
     author_email='dai.motoki1123@gmail.com',
     url='https://niwatoko2.vercel.app/',
     packages=find_packages(),
```

### Comparing `niwatoko-1.1.6/tests/README.md` & `niwatoko-1.1.7/tests/README.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/__init__.py` & `niwatoko-1.1.7/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_compiler.md` & `niwatoko-1.1.7/tests/test_compiler.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_compiler.py` & `niwatoko-1.1.7/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_compiler_v1_2.py` & `niwatoko-1.1.7/tests/test_compiler_v1_2.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/__init__.py` & `niwatoko-1.1.7/tests/test_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/output copy.md` & `niwatoko-1.1.7/tests/test_docs/output copy.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/output.md` & `niwatoko-1.1.7/tests/test_docs/output.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/output.py` & `niwatoko-1.1.7/tests/test_docs/output.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/output_.md` & `niwatoko-1.1.7/tests/test_docs/output_.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_doc1.md` & `niwatoko-1.1.7/tests/test_docs/test_doc1.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_doc2.md` & `niwatoko-1.1.7/tests/test_docs/test_doc2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_doc3.md` & `niwatoko-1.1.7/tests/test_docs/test_doc3.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_gen_github_issue.md` & `niwatoko-1.1.7/tests/test_docs/test_gen_github_issue.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_gen_grimoire.md` & `niwatoko-1.1.7/tests/test_docs/test_gen_grimoire.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_gen_grimoire2.md` & `niwatoko-1.1.7/tests/test_docs/test_gen_grimoire2.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_gen_grimoire_en.md` & `niwatoko-1.1.7/tests/test_docs/test_gen_grimoire_en.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_gen_zoltraak_pypi.md` & `niwatoko-1.1.7/tests/test_docs/test_gen_zoltraak_pypi.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_docs/test_import_function.md` & `niwatoko-1.1.7/tests/test_docs/test_import_function.md`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_interpreter.py` & `niwatoko-1.1.7/tests/test_interpreter.py`

 * *Files identical despite different names*

### Comparing `niwatoko-1.1.6/tests/test_parser.py` & `niwatoko-1.1.7/tests/test_parser.py`

 * *Files identical despite different names*

