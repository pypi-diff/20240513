# Comparing `tmp/konoha-5.5.5.tar.gz` & `tmp/konoha-5.5.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konoha-5.5.5.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `konoha-5.5.5.tar` & `konoha-5.5.6a0.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0     1067 2024-02-20 12:37:50.871023 konoha-5.5.5/LICENSE
--rw-r--r--   0        0        0     7222 2024-02-20 12:37:50.871023 konoha-5.5.5/README.md
--rw-r--r--   0        0        0     1676 2024-02-20 12:37:50.879023 konoha-5.5.5/pyproject.toml
--rw-r--r--   0        0        0      212 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/__init__.py
--rw-r--r--   0        0        0      373 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/api/server.py
--rw-r--r--   0        0        0     1979 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/api/v1/batch_tokenization.py
--rw-r--r--   0        0        0     2192 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/api/v1/tokenization.py
--rw-r--r--   0        0        0        0 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/data/__init__.py
--rw-r--r--   0        0        0     2276 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/data/resource.py
--rw-r--r--   0        0        0     4440 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/data/token.py
--rw-r--r--   0        0        0        0 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/py.typed
--rw-r--r--   0        0        0     1414 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/sentence_tokenizer.py
--rw-r--r--   0        0        0     6017 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizer.py
--rw-r--r--   0        0        0      519 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/__init__.py
--rw-r--r--   0        0        0      298 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/character_tokenizer.py
--rw-r--r--   0        0        0     1111 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/janome_tokenizer.py
--rw-r--r--   0        0        0      246 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/konoha_api_tokenizer.py
--rw-r--r--   0        0        0     1335 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/kytea_tokenizer.py
--rw-r--r--   0        0        0     3818 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/mecab_tokenizer.py
--rw-r--r--   0        0        0      544 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/nagisa_tokenizer.py
--rw-r--r--   0        0        0      643 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/sentencepiece_tokenizer.py
--rw-r--r--   0        0        0     1807 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/sudachi_tokenizer.py
--rw-r--r--   0        0        0      530 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/tokenizer.py
--rw-r--r--   0        0        0      401 2024-02-20 12:37:50.879023 konoha-5.5.5/src/konoha/word_tokenizers/whitespace_tokenizer.py
--rw-r--r--   0        0        0     8866 1970-01-01 00:00:00.000000 konoha-5.5.5/PKG-INFO
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/py.typed
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/sentence_tokenizer.py
+-rw-r--r--   0        0        0     6018 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/__init__.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/__init__.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/batch_tokenization.py
+-rw-r--r--   0        0        0     2192 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/api/v1/tokenization.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/resource.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/data/token.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/__init__.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/character_tokenizer.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/janome_tokenizer.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/konoha_api_tokenizer.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/kytea_tokenizer.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/mecab_tokenizer.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/nagisa_tokenizer.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/sentencepiece_tokenizer.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/sudachi_tokenizer.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/tokenizer.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 konoha-5.5.6a0/konoha/word_tokenizers/whitespace_tokenizer.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 konoha-5.5.6a0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 konoha-5.5.6a0/LICENSE
+-rw-r--r--   0        0        0     7222 2020-02-02 00:00:00.000000 konoha-5.5.6a0/README.md
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 konoha-5.5.6a0/pyproject.toml
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 konoha-5.5.6a0/PKG-INFO
```

### Comparing `konoha-5.5.5/LICENSE` & `konoha-5.5.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/README.md` & `konoha-5.5.6a0/README.md`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/api/v1/batch_tokenization.py` & `konoha-5.5.6a0/konoha/api/v1/batch_tokenization.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/api/v1/tokenization.py` & `konoha-5.5.6a0/konoha/api/v1/tokenization.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/data/resource.py` & `konoha-5.5.6a0/konoha/data/resource.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/data/token.py` & `konoha-5.5.6a0/konoha/data/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Token class."""
+
 from typing import Dict
 from typing import List
 from typing import Optional
 
 
 class Token:
     """Token class for konoha."""
```

### Comparing `konoha-5.5.5/src/konoha/sentence_tokenizer.py` & `konoha-5.5.6a0/konoha/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Word Level Tokenizer."""
+
 import warnings
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import requests
```

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/__init__.py` & `konoha-5.5.6a0/konoha/word_tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/janome_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/janome_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/kytea_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/kytea_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/mecab_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/mecab_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/nagisa_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/nagisa_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/sentencepiece_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/sudachi_tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/sudachi_tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/src/konoha/word_tokenizers/tokenizer.py` & `konoha-5.5.6a0/konoha/word_tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `konoha-5.5.5/PKG-INFO` & `konoha-5.5.6a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: konoha
-Version: 5.5.5
-Summary: A tiny sentence/word tokenizer for Japanese text written in Python
-License: MIT
-Author: himkt
-Author-email: himkt@klis.tsukuba.ac.jp
-Requires-Python: >=3.8.0,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
+Version: 5.5.6a0
+Summary: Add your description here
+Author-email: himkt <himkt@klis.tsukuba.ac.jp>
+License-Expression: MIT
+License-File: LICENSE
+Requires-Python: >=3.8
+Requires-Dist: requests<3.0.0
 Provides-Extra: all
+Requires-Dist: boto3~=1.34.0; extra == 'all'
+Requires-Dist: fastapi<1.0.0; extra == 'all'
+Requires-Dist: janome~=0.5.0; extra == 'all'
+Requires-Dist: kytea~=0.1.0; extra == 'all'
+Requires-Dist: nagisa~=0.2.10; extra == 'all'
+Requires-Dist: natto-py~=1.0.0; extra == 'all'
+Requires-Dist: sentencepiece~=0.1.85; extra == 'all'
+Requires-Dist: sudachidict-core==20230927; extra == 'all'
+Requires-Dist: uvicorn<0.26.0; extra == 'all'
 Provides-Extra: janome
+Requires-Dist: janome~=0.5.0; extra == 'janome'
 Provides-Extra: kytea
+Requires-Dist: kytea~=0.1.0; extra == 'kytea'
 Provides-Extra: mecab
+Requires-Dist: natto-py~=1.0.0; extra == 'mecab'
 Provides-Extra: nagisa
+Requires-Dist: nagisa~=0.2.10; extra == 'nagisa'
 Provides-Extra: remote
+Requires-Dist: boto3~=1.34.0; extra == 'remote'
 Provides-Extra: sentencepiece
+Requires-Dist: sentencepiece~=0.1.85; extra == 'sentencepiece'
 Provides-Extra: server
+Requires-Dist: fastapi<1.0.0; extra == 'server'
+Requires-Dist: uvicorn<0.26.0; extra == 'server'
 Provides-Extra: sudachi
-Requires-Dist: boto3 (>=1.34.0,<2.0.0) ; extra == "remote" or extra == "all"
-Requires-Dist: fastapi (<1.0.0) ; extra == "server" or extra == "all"
-Requires-Dist: janome (>=0.5.0,<0.6.0) ; extra == "janome" or extra == "all"
-Requires-Dist: kytea (>=0.1.8,<0.2.0) ; extra == "kytea" or extra == "all"
-Requires-Dist: nagisa (>=0.2.10,<0.3.0) ; extra == "nagisa" or extra == "all"
-Requires-Dist: natto-py (>=1.0.0,<2.0.0) ; extra == "mecab" or extra == "all"
-Requires-Dist: requests (<3.0.0)
-Requires-Dist: sentencepiece (>=0.1.85,<0.2.0) ; extra == "sentencepiece" or extra == "all"
-Requires-Dist: sudachidict-core (==20230927) ; extra == "sudachi" or extra == "all"
-Requires-Dist: sudachipy (>=0.6.8,<0.7.0) ; extra == "sudachi" or extra == "all"
-Requires-Dist: uvicorn (<0.26.0) ; extra == "server" or extra == "all"
+Requires-Dist: sudachidict-core==20230927; extra == 'sudachi'
+Requires-Dist: sudachipy~=0.6.8; extra == 'sudachi'
 Description-Content-Type: text/markdown
 
 # 🌿 Konoha: Simple wrapper of Japanese Tokenizers
 
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/himkt/konoha/blob/main/example/Konoha_Example.ipynb)
 <p align="center"><img src="https://user-images.githubusercontent.com/5164000/120913279-e7d62380-c6d0-11eb-8d17-6571277cdf27.gif" width="95%"></p>
 
@@ -219,8 +221,7 @@
 
 - [トークナイザをいい感じに切り替えるライブラリ konoha を作った](https://qiita.com/klis/items/bb9ffa4d9c886af0f531)
 - [日本語解析ツール Konoha に AllenNLP 連携機能を実装した](https://qiita.com/klis/items/f1d29cb431d1bf879898)
 
 ## Acknowledgement
 
 Sentencepiece model used in test is provided by @yoheikikuta. Thanks!
-
```

#### html2text {}

```diff
@@ -1,32 +1,30 @@
-Metadata-Version: 2.1 Name: konoha Version: 5.5.5 Summary: A tiny sentence/word
-tokenizer for Japanese text written in Python License: MIT Author: himkt
-Author-email: himkt@klis.tsukuba.ac.jp Requires-Python: >=3.8.0,<4.0.0
-Classifier: License :: OSI Approved :: MIT License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12 Provides-Extra: all
-Provides-Extra: janome Provides-Extra: kytea Provides-Extra: mecab Provides-
-Extra: nagisa Provides-Extra: remote Provides-Extra: sentencepiece Provides-
-Extra: server Provides-Extra: sudachi Requires-Dist: boto3 (>=1.34.0,<2.0.0) ;
-extra == "remote" or extra == "all" Requires-Dist: fastapi (<1.0.0) ; extra ==
-"server" or extra == "all" Requires-Dist: janome (>=0.5.0,<0.6.0) ; extra ==
-"janome" or extra == "all" Requires-Dist: kytea (>=0.1.8,<0.2.0) ; extra ==
-"kytea" or extra == "all" Requires-Dist: nagisa (>=0.2.10,<0.3.0) ; extra ==
-"nagisa" or extra == "all" Requires-Dist: natto-py (>=1.0.0,<2.0.0) ; extra ==
-"mecab" or extra == "all" Requires-Dist: requests (<3.0.0) Requires-Dist:
-sentencepiece (>=0.1.85,<0.2.0) ; extra == "sentencepiece" or extra == "all"
-Requires-Dist: sudachidict-core (==20230927) ; extra == "sudachi" or extra ==
-"all" Requires-Dist: sudachipy (>=0.6.8,<0.7.0) ; extra == "sudachi" or extra
-== "all" Requires-Dist: uvicorn (<0.26.0) ; extra == "server" or extra == "all"
-Description-Content-Type: text/markdown # ð¿ Konoha: Simple wrapper of
-Japanese Tokenizers [![Open In Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/himkt/konoha/blob/
-main/example/Konoha_Example.ipynb)
+Metadata-Version: 2.3 Name: konoha Version: 5.5.6a0 Summary: Add your
+description here Author-email: himkt
+klis.tsukuba.ac.jp> License-Expression: MIT License-File: LICENSE Requires-
+Python: >=3.8 Requires-Dist: requests<3.0.0 Provides-Extra: all Requires-Dist:
+boto3~=1.34.0; extra == 'all' Requires-Dist: fastapi<1.0.0; extra == 'all'
+Requires-Dist: janome~=0.5.0; extra == 'all' Requires-Dist: kytea~=0.1.0; extra
+== 'all' Requires-Dist: nagisa~=0.2.10; extra == 'all' Requires-Dist: natto-
+py~=1.0.0; extra == 'all' Requires-Dist: sentencepiece~=0.1.85; extra == 'all'
+Requires-Dist: sudachidict-core==20230927; extra == 'all' Requires-Dist:
+uvicorn<0.26.0; extra == 'all' Provides-Extra: janome Requires-Dist:
+janome~=0.5.0; extra == 'janome' Provides-Extra: kytea Requires-Dist:
+kytea~=0.1.0; extra == 'kytea' Provides-Extra: mecab Requires-Dist: natto-
+py~=1.0.0; extra == 'mecab' Provides-Extra: nagisa Requires-Dist:
+nagisa~=0.2.10; extra == 'nagisa' Provides-Extra: remote Requires-Dist:
+boto3~=1.34.0; extra == 'remote' Provides-Extra: sentencepiece Requires-Dist:
+sentencepiece~=0.1.85; extra == 'sentencepiece' Provides-Extra: server
+Requires-Dist: fastapi<1.0.0; extra == 'server' Requires-Dist: uvicorn<0.26.0;
+extra == 'server' Provides-Extra: sudachi Requires-Dist: sudachidict-
+core==20230927; extra == 'sudachi' Requires-Dist: sudachipy~=0.6.8; extra ==
+'sudachi' Description-Content-Type: text/markdown # ð¿ Konoha: Simple wrapper
+of Japanese Tokenizers [![Open In Colab](https://colab.research.google.com/
+assets/colab-badge.svg)](https://colab.research.google.com/github/himkt/konoha/
+blob/main/example/Konoha_Example.ipynb)
   [https://user-images.githubusercontent.com/5164000/120913279-e7d62380-c6d0-
                           11eb-8d17-6571277cdf27.gif]
 [![GitHub stars](https://img.shields.io/github/stars/himkt/
 konoha?style=social)](https://github.com/himkt/konoha/stargazers) [![Downloads]
 (https://pepy.tech/badge/konoha)](https://pepy.tech/project/konoha) [!
 [Downloads](https://pepy.tech/badge/konoha/month)](https://pepy.tech/project/
 konoha/month) [![Downloads](https://pepy.tech/badge/konoha/week)](https://
```

