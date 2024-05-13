# Comparing `tmp/gaiah_toolkit-0.3.10.tar.gz` & `tmp/gaiah_toolkit-0.3.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaiah_toolkit-0.3.10.tar", last modified: Mon May 13 10:51:04 2024, max compression
+gzip compressed data, was "gaiah_toolkit-0.3.13.tar", last modified: Mon May 13 13:56:22 2024, max compression
```

## Comparing `gaiah_toolkit-0.3.10.tar` & `gaiah_toolkit-0.3.13.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:51:04.257550 gaiah_toolkit-0.3.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-13 10:51:04.257550 gaiah_toolkit-0.3.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6437 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:51:04.253549 gaiah_toolkit-0.3.10/gaiah/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/gaiah/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/gaiah/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/gaiah/gaiah.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/gaiah/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:51:04.257550 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 10:51:04.000000 gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 10:51:04.257550 gaiah_toolkit-0.3.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 10:51:04.257550 gaiah_toolkit-0.3.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 10:50:59.000000 gaiah_toolkit-0.3.10/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8863 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/gaiah/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7294 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/gaiah/gaiah.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 13:56:22.000000 gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:56:22.978658 gaiah_toolkit-0.3.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:56:22.974658 gaiah_toolkit-0.3.13/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-13 13:56:18.000000 gaiah_toolkit-0.3.13/tests/test_main.py
```

### Comparing `gaiah_toolkit-0.3.10/LICENSE` & `gaiah_toolkit-0.3.13/LICENSE`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.10/PKG-INFO` & `gaiah_toolkit-0.3.13/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiah_toolkit
-Version: 0.3.10
+Version: 0.3.13
 Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
@@ -53,15 +53,15 @@
 ## 🌟 はじめに
 
 Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
 
 ## 🚀 主な特徴
 
 - 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。
+- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
 - 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
 - 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
 - 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
 
 ## 📦 インストール
 
 Gaiahの使用を開始するには、次の手順に従ってください:
@@ -79,22 +79,65 @@
    pip install gitpython python-dotenv PyGithub termcolor art
    ```
 
 ## 🎉 使用方法
 
 ### CLI
 
-GaiahのCLI機能に
-
-より、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+```bash
+gaiah
 ```
+
+### 応用的な使い方
+
+特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
+
+```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md
 ```
 
+上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+
+## 🤝 コミットメッセージの一括自動コミット
+
+Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
+
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
+
+2. LLMは以下のような形式でコミットメッセージを生成します:
+
+   ```
+   Commit Messages フォーマット
+
+   ## Commit 1
+
+   ### README.md
+
+   ```commit-msg
+   📝 [docs] READMEに応用的な使い方セクションを追加
+
+   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
+   ```
+
+   ## Commit 2
+
+   ### gaiah/__init__.py
+
+   ```commit-msg
+   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+
+   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
+   ```
+   ```
+
+3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
+
+4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
+
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
 
 Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.10 Home-page: https://
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.13 Home-page: https://
 github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Version Control Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
 Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
@@ -42,18 +42,39 @@
 Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
 ## ð¦ ã¤ã³ã¹ãã¼ã«
 Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
 æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«
-ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-``` gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md ``` ## ð¤ è²¢ç®
+Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
+```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
+ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
+```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
+``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
+repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
+commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
+## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
+Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
+github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
+STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
+2.
+LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
+``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
+ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
+`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
+``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
+Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
+__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
+``` ``` 3.
+çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
+4.
+ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
+## ð¤ è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.10/README.md` & `gaiah_toolkit-0.3.13/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ## 🌟 はじめに
 
 Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
 
 ## 🚀 主な特徴
 
 - 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。
+- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
 - 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
 - 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
 - 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
 
 ## 📦 インストール
 
 Gaiahの使用を開始するには、次の手順に従ってください:
@@ -64,22 +64,65 @@
    pip install gitpython python-dotenv PyGithub termcolor art
    ```
 
 ## 🎉 使用方法
 
 ### CLI
 
-GaiahのCLI機能に
-
-より、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+```bash
+gaiah
 ```
+
+### 応用的な使い方
+
+特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
+
+```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md
 ```
 
+上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+
+## 🤝 コミットメッセージの一括自動コミット
+
+Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
+
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
+
+2. LLMは以下のような形式でコミットメッセージを生成します:
+
+   ```
+   Commit Messages フォーマット
+
+   ## Commit 1
+
+   ### README.md
+
+   ```commit-msg
+   📝 [docs] READMEに応用的な使い方セクションを追加
+
+   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
+   ```
+
+   ## Commit 2
+
+   ### gaiah/__init__.py
+
+   ```commit-msg
+   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+
+   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
+   ```
+   ```
+
+3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
+
+4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
+
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
 
 Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
```

#### html2text {}

```diff
@@ -36,18 +36,39 @@
 Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
 ## ð¦ ã¤ã³ã¹ãã¼ã«
 Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
 æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«
-ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-``` gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md ``` ## ð¤ è²¢ç®
+Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
+```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
+ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
+```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
+``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
+repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
+commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
+## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
+Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
+github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
+STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
+2.
+LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
+``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
+ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
+`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
+``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
+Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
+__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
+``` ``` 3.
+çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
+4.
+ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
+## ð¤ è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.10/gaiah/cli.py` & `gaiah_toolkit-0.3.13/gaiah/cli.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.10/gaiah/gaiah.py` & `gaiah_toolkit-0.3.13/gaiah/gaiah.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,33 +36,41 @@
         self.repo_dir = repo_dir
         self.commit_messages_path = commit_messages_path
         self.repo = Repo(repo_dir)
         self.current_branch = self.repo.active_branch.name
         print(colored("リポジトリオブジェクトが作成されました。", "cyan"))
         print(colored(f"現在のブランチ: {self.current_branch}", "cyan"))
 
+
     def unstage_files(self):
         """
         ステージにある全てのファイルをアンステージする
         """
         msg = "-" * 20 + " unstage " + "-" * 20
         print(colored(f"{msg}", "green"))
 
-        diff_index = self.repo.index.diff("HEAD")
-        staged_files = [diff.a_path for diff in diff_index]
-        if staged_files:
-            for file_path in staged_files:
-                try:
-                    subprocess.run(["git", "reset", "HEAD", file_path], check=True, cwd=self.repo_dir)
-                    print(colored(f"ファイル {file_path} がアンステージされました。", "green"))
-                except subprocess.CalledProcessError as e:
-                    print(colored(f"アンステージエラー: {e}", "red"))
-                    return False
-        else:
-            print(colored("ステージされたファイルはありません。", "magenta"))
+        try:
+            result = subprocess.run(
+                ["git", "diff", "--name-only", "--cached"],
+                cwd=self.repo_dir,
+                text=True,
+                capture_output=True,
+                check=True
+            )
+            staged_files = result.stdout.splitlines()
+
+            if staged_files:
+                subprocess.run(["git", "reset", "HEAD", "--"] + staged_files, cwd=self.repo_dir)
+                print(colored(f"ステージされたファイルをアンステージしました: {', '.join(staged_files)}", "green"))
+            else:
+                print(colored("ステージされたファイルはありません。", "magenta"))
+
+        except subprocess.CalledProcessError as e:
+            print(colored(f"アンステージエラー: {e}", "red"))
+            return False
 
         print(colored(f"-" * len(msg), "green"))
         return True
 
     def process_commits(self):
         try:
             with open(self.commit_messages_path, "r", encoding="utf-8") as file:
@@ -71,14 +79,17 @@
         except FileNotFoundError:
             print(colored(f"エラー: {self.commit_messages_path} が見つかりません。", "red"))
             return
         except UnicodeDecodeError:
             print(colored(f"エラー: {self.commit_messages_path} のデコードに失敗しました。ファイルがUTF-8で保存されていることを確認してください。", "red"))
             return
 
+        # すべてのファイルをアンステージ
+        self.unstage_files()
+
         commits = re.split(self.COMMIT_SECTION_REGEX, content)[1:]
 
         for commit in commits:
             filename_match = re.search(self.FILENAME_REGEX, commit)
             if filename_match:
                 filename = filename_match.group(1).strip()
                 print(colored(f"ファイル [{filename}] を処理中...", "blue"))
@@ -97,39 +108,35 @@
 
             self.process_file(filename, commit_message)
 
         self.push_to_remote()
 
     def process_file(self, filename, commit_message):
         try:
+            # ファイルのアクションを実行
+            if os.path.exists(os.path.join(self.repo_dir, filename)):
+                self.stage_file(filename, "modified")
+            else:
+                self.stage_file(filename, "deleted")
+
+            # 差分を確認
             result = subprocess.run(
-                ["git", "diff", "--name-status", "HEAD"],
+                ["git", "diff", "--staged", "--name-only"],
                 cwd=self.repo_dir,
                 text=True,
                 capture_output=True,
                 check=True
             )
 
-            lines = result.stdout.splitlines()
-            file_changed = False
-            for line in lines:
-                status, path = line.split(maxsplit=1)
-                if path == filename:
-                    file_changed = True
-                    if status == "A":
-                        self.stage_file(filename, "added")
-                    elif status == "D":
-                        self.stage_file(filename, "deleted")
-                    else:  # Modified or other changes
-                        self.stage_file(filename, "modified")
-
-            if file_changed:
+            changed_files = result.stdout.splitlines()
+            if filename in changed_files:
                 self.commit_changes(commit_message)
             else:
                 print(colored(f"ファイル {filename} に変更はありませんでした。", "magenta"))
+                self.unstage_file(filename)
 
         except subprocess.CalledProcessError as e:
             print(colored(f"Git コマンドの実行中にエラーが発生しました: {e}", "red"))
 
     def stage_file(self, filename, action):
         try:
             if action == "deleted":
```

### Comparing `gaiah_toolkit-0.3.10/gaiah_toolkit.egg-info/PKG-INFO` & `gaiah_toolkit-0.3.13/gaiah_toolkit.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaiah_toolkit
-Version: 0.3.10
+Version: 0.3.13
 Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Version Control
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: gitpython
@@ -53,15 +53,15 @@
 ## 🌟 はじめに
 
 Gaiahは、直感的でAIにやさしいメソッドを使用してGit操作を簡素化する革新的なPythonライブラリです。Gitリポジトリを制御するための高レベルなインターフェースを提供し、AIシステムがバージョン管理とシームレスに連携することを容易にします。新機能としてMarkdownから直接コミットを生成する機能が追加され、文書化されたコミットメッセージの管理がさらに効率的に行えます。
 
 ## 🚀 主な特徴
 
 - 🤖 **AIフレンドリー**: AI主導の開発プロセスの独自の要件に対応するメソッドとユーティリティを提供し、AIを念頭に置いて設計されています。
-- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。
+- 🌐 **リモートリポジトリのサポート**: リモートリポジトリとのシームレスな連携を可能にし、GitHubやその他のGitホスティングプラットフォームにリポジトリを作成、クローン、プッシュできるようにします。 
 - 📂 **リポジトリ管理**: 新しいリポジトリの初期化、ファイルの追加、コミットの作成、ブランチの管理をシンプルなPythonコードを介して簡単に行うことができます。
 - 🔧 **カスタマイズ**: 柔軟性とカスタマイズオプションを提供し、特定のニーズと設定に合わせてGitワークフローを調整できます。
 - 📘 **Markdownからのコミット生成**: Markdown形式のドキュメントから直接コミットを生成する機能を追加し、文書化されたコミットメッセージの効率的な管理を可能にします。
 
 ## 📦 インストール
 
 Gaiahの使用を開始するには、次の手順に従ってください:
@@ -79,22 +79,65 @@
    pip install gitpython python-dotenv PyGithub termcolor art
    ```
 
 ## 🎉 使用方法
 
 ### CLI
 
-GaiahのCLI機能に
-
-より、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+GaiahのCLI機能により、コマンドラインから直接Git操作を行うことができます。例えば、以下のコマンドを使用してリポジトリにコミットを追加することができます:
+```bash
+gaiah
 ```
+
+### 応用的な使い方
+
+特定のプロジェクトディレクトリでGaiahを使用する場合、以下のようにリポジトリの場所やコミットメッセージのファイルパスを指定できます:
+
+```bash
 gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md
 ```
 
+上記のコマンドでは、`--repo_dir`オプションでリポジトリのディレクトリを、`--commit_msg_path`オプションでコミットメッセージが記載されたMarkdownファイルのパスを指定しています。
+
+## 🤝 コミットメッセージの一括自動コミット
+
+Gaiahでは、LLMを用いて生成したコミットメッセージを一括自動コミットすることができます。以下の手順でコミットメッセージを生成し、コミットを行います:
+
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md)というフォーマットで、ステージング情報をLLMに渡します。
+
+2. LLMは以下のような形式でコミットメッセージを生成します:
+
+   ```
+   Commit Messages フォーマット
+
+   ## Commit 1
+
+   ### README.md
+
+   ```commit-msg
+   📝 [docs] READMEに応用的な使い方セクションを追加
+
+   - `README.md`ファイルに新たなセクションとして「応用的な使い方」を追加しました。これにより、ユーザーはGaiahを特定のプロジェクトディレクトリで使用する方法を具体的に学べるようになります。特に、リポジトリの指定やコミットメッセージのファイルパスを設定する具体的なコマンド例を示しています。  
+   ```
+
+   ## Commit 2
+
+   ### gaiah/__init__.py
+
+   ```commit-msg
+   🔖 [chore] Gaiahのバージョンを0.3.12に更新
+
+   - `gaiah/__init__.py`でのバージョン番号を0.3.11から0.3.12へ更新しました。この更新は、最新の機能改善とバグ修正をユーザーに提供するためのものです。
+   ```
+   ```
+
+3. 生成されたコミットメッセージを`.Gaiah.md`ファイルに貼り付けます。このファイルは、初回に`gaiah`コマンドを実行した際に自動で生成されます。
+
+4. 再度`gaiah`コマンドを実行すると、`.Gaiah.md`ファイルからコミットメッセージが読み込まれ、自動的にコミットとプッシュが行われます。
+
 ## 🤝 貢献
 
 Gaiahをさらに良くするために、コミュニティからの貢献を歓迎します。アイデア、提案、バグ報告がある場合は、[GitHubリポジトリ](https://github.com/Sunwood-ai-labs/Gaiah)で issue を開くか、プルリクエストを送信してください。
 
 ## 📄 ライセンス
 
 Gaiahは、[MITライセンス](https://opensource.org/licenses/MIT)の下でリリースされており、ライブラリの自由かつオープンソースでの使用、変更、配布が可能です。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.10 Home-page: https://
+Metadata-Version: 2.1 Name: gaiah_toolkit Version: 0.3.13 Home-page: https://
 github.com/your_username/gaiah Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers Classifier: Topic :: Software
 Development :: Version Control Description-Content-Type: text/markdown License-
 File: LICENSE Requires-Dist: gitpython Requires-Dist: python-dotenv Requires-
 Dist: PyGithub Requires-Dist: termcolor Requires-Dist: art
        [https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/
                                Gaiah_icon1.png]
@@ -42,18 +42,39 @@
 Markdownå½¢å¼ã®ãã­ã¥ã¡ã³ãããç´æ¥ã³ããããçæããæ©è½ãè¿½å ããææ¸åãããã³ãããã¡ãã»ã¼ã¸ã®å¹ççãªç®¡çãå¯è½ã«ãã¾ãã
 ## ð¦ ã¤ã³ã¹ãã¼ã«
 Gaiahã®ä½¿ç¨ãéå§ããã«ã¯ãæ¬¡ã®æé ã«å¾ã£ã¦ãã ãã: 1.
 æ°ããcondaç°å¢ãä½æãã¾ã: ``` conda create -n gaiah python=3.11
 ``` 2. condaç°å¢ãã¢ã¯ãã£ãã¼ããã¾ã: ``` conda activate gaiah
 ``` 3. å¿è¦ãªä¾å­é¢ä¿ãã¤ã³ã¹ãã¼ã«ãã¾ã: ``` pip install
 gitpython python-dotenv PyGithub termcolor art ``` ## ð ä½¿ç¨æ¹æ³ ### CLI
-Gaiahã®CLIæ©è½ã«
-ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
-``` gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
-gaiah --repo_dir="./" --commit_msg_path=./tmp2.md ``` ## ð¤ è²¢ç®
+Gaiahã®CLIæ©è½ã«ãããã³ãã³ãã©ã¤ã³ããç´æ¥Gitæä½ãè¡ããã¨ãã§ãã¾ããä¾ãã°ãä»¥ä¸ã®ã³ãã³ããä½¿ç¨ãã¦ãªãã¸ããªã«ã³ããããè¿½å ãããã¨ãã§ãã¾ã:
+```bash gaiah ``` ### å¿ç¨çãªä½¿ãæ¹
+ç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§Gaiahãä½¿ç¨ããå ´åãä»¥ä¸ã®ããã«ãªãã¸ããªã®å ´æãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãæå®ã§ãã¾ã:
+```bash gaiah --repo_dir="C:\\Prj\\Gaiah_Sample02" --commit_msg_path=./tmp2.md
+``` ä¸è¨ã®ã³ãã³ãã§ã¯ã`--
+repo_dir`ãªãã·ã§ã³ã§ãªãã¸ããªã®ãã£ã¬ã¯ããªãã`--
+commit_msg_path`ãªãã·ã§ã³ã§ã³ãããã¡ãã»ã¼ã¸ãè¨è¼ãããMarkdownãã¡ã¤ã«ã®ãã¹ãæå®ãã¦ãã¾ãã
+## ð¤ ã³ãããã¡ãã»ã¼ã¸ã®ä¸æ¬èªåã³ããã
+Gaiahã§ã¯ãLLMãç¨ãã¦çæããã³ãããã¡ãã»ã¼ã¸ãä¸æ¬èªåã³ããããããã¨ãã§ãã¾ããä»¥ä¸ã®æé ã§ã³ãããã¡ãã»ã¼ã¸ãçæããã³ããããè¡ãã¾ã:
+1. [sourcesage/config/STAGE_INFO/STAGE_INFO_TEMPLATE_GAIAH.md](https://
+github.com/Sunwood-ai-labs/SourceSage/blob/main/sourcesage/config/STAGE_INFO/
+STAGE_INFO_TEMPLATE_GAIAH.md)ã¨ãããã©ã¼ãããã§ãã¹ãã¼ã¸ã³ã°æå ±ãLLMã«æ¸¡ãã¾ãã
+2.
+LLMã¯ä»¥ä¸ã®ãããªå½¢å¼ã§ã³ãããã¡ãã»ã¼ã¸ãçæãã¾ã:
+``` Commit Messages ãã©ã¼ããã ## Commit 1 ### README.md ```commit-msg
+ð [docs] READMEã«å¿ç¨çãªä½¿ãæ¹ã»ã¯ã·ã§ã³ãè¿½å  -
+`README.md`ãã¡ã¤ã«ã«æ°ããªã»ã¯ã·ã§ã³ã¨ãã¦ãå¿ç¨çãªä½¿ãæ¹ããè¿½å ãã¾ãããããã«ãããã¦ã¼ã¶ã¼ã¯Gaiahãç¹å®ã®ãã­ã¸ã§ã¯ããã£ã¬ã¯ããªã§ä½¿ç¨ããæ¹æ³ãå·ä½çã«å­¦ã¹ãããã«ãªãã¾ããç¹ã«ããªãã¸ããªã®æå®ãã³ãããã¡ãã»ã¼ã¸ã®ãã¡ã¤ã«ãã¹ãè¨­å®ããå·ä½çãªã³ãã³ãä¾ãç¤ºãã¦ãã¾ãã
+``` ## Commit 2 ### gaiah/__init__.py ```commit-msg ð [chore]
+Gaiahã®ãã¼ã¸ã§ã³ã0.3.12ã«æ´æ° - `gaiah/
+__init__.py`ã§ã®ãã¼ã¸ã§ã³çªå·ã0.3.11ãã0.3.12ã¸æ´æ°ãã¾ããããã®æ´æ°ã¯ãææ°ã®æ©è½æ¹åã¨ãã°ä¿®æ­£ãã¦ã¼ã¶ã¼ã«æä¾ããããã®ãã®ã§ãã
+``` ``` 3.
+çæãããã³ãããã¡ãã»ã¼ã¸ã`.Gaiah.md`ãã¡ã¤ã«ã«è²¼ãä»ãã¾ãããã®ãã¡ã¤ã«ã¯ãååã«`gaiah`ã³ãã³ããå®è¡ããéã«èªåã§çæããã¾ãã
+4.
+ååº¦`gaiah`ã³ãã³ããå®è¡ããã¨ã`.Gaiah.md`ãã¡ã¤ã«ããã³ãããã¡ãã»ã¼ã¸ãèª­ã¿è¾¼ã¾ããèªåçã«ã³ãããã¨ããã·ã¥ãè¡ããã¾ãã
+## ð¤ è²¢ç®
 Gaiahãããã«è¯ãããããã«ãã³ãã¥ããã£ããã®è²¢ç®ãæ­è¿ãã¾ããã¢ã¤ãã¢ãææ¡ããã°å ±åãããå ´åã¯ã
 [GitHubãªãã¸ããª](https://github.com/Sunwood-ai-labs/Gaiah)ã§ issue
 ãéããããã«ãªã¯ã¨ã¹ããéä¿¡ãã¦ãã ããã ## ð
 ã©ã¤ã»ã³ã¹ Gaiahã¯ã[MITã©ã¤ã»ã³ã¹](https://opensource.org/
 licenses/
 MIT)ã®ä¸ã§ãªãªã¼ã¹ããã¦ãããã©ã¤ãã©ãªã®èªç±ãã¤ãªã¼ãã³ã½ã¼ã¹ã§ã®ä½¿ç¨ãå¤æ´ãéå¸ãå¯è½ã§ãã
 ## ð è¬è¾
```

### Comparing `gaiah_toolkit-0.3.10/setup.py` & `gaiah_toolkit-0.3.13/setup.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.10/tests/test_cli.py` & `gaiah_toolkit-0.3.13/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gaiah_toolkit-0.3.10/tests/test_main.py` & `gaiah_toolkit-0.3.13/tests/test_main.py`

 * *Files identical despite different names*

