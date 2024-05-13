# Comparing `tmp/harmon_ai-1.2.0.tar.gz` & `tmp/harmon_ai-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmon_ai-1.2.0.tar", last modified: Mon May 13 12:53:58 2024, max compression
+gzip compressed data, was "harmon_ai-1.3.0.tar", last modified: Mon May 13 14:46:22 2024, max compression
```

## Comparing `harmon_ai-1.2.0.tar` & `harmon_ai-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/harmon_ai/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/harmon_ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/harmon_ai/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/harmon_ai/harmon_ai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/harmon_ai/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/harmon_ai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/harmon_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-13 12:53:58.000000 harmon_ai-1.2.0/harmon_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 12:53:58.000000 harmon_ai-1.2.0/harmon_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:53:58.000000 harmon_ai-1.2.0/harmon_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 12:53:58.000000 harmon_ai-1.2.0/harmon_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 12:53:58.000000 harmon_ai-1.2.0/harmon_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:53:58.652256 harmon_ai-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-13 12:53:54.000000 harmon_ai-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:46:22.324424 harmon_ai-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-13 14:46:22.324424 harmon_ai-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:46:22.320424 harmon_ai-1.3.0/harmon_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/harmon_ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/harmon_ai/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/harmon_ai/harmon_ai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:46:22.320424 harmon_ai-1.3.0/harmon_ai/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/harmon_ai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:46:22.320424 harmon_ai-1.3.0/harmon_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6416 2024-05-13 14:46:22.000000 harmon_ai-1.3.0/harmon_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-13 14:46:22.000000 harmon_ai-1.3.0/harmon_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:46:22.000000 harmon_ai-1.3.0/harmon_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-13 14:46:22.000000 harmon_ai-1.3.0/harmon_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-13 14:46:22.000000 harmon_ai-1.3.0/harmon_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:46:22.324424 harmon_ai-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 14:46:17.000000 harmon_ai-1.3.0/setup.py
```

### Comparing `harmon_ai-1.2.0/LICENSE` & `harmon_ai-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harmon_ai-1.2.0/PKG-INFO` & `harmon_ai-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: harmon_ai
-Version: 1.2.0
+Version: 1.3.0
+Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -66,70 +67,60 @@
 
 このテンプレートを活用することで、リポジトリ作成時の初期コストを抑えつつ、品質と開発速度を担保することができます。AI時代の開発スタイルを先取りした、生産性の高いテンプレートとしてご利用ください。
 
 ## 🎥 デモ
 
 HarmonAI IIのデモアプリケーションは、GitHub Actionsと連携し、自動的にデプロイされています。デモアプリを体験することで、HarmonAI IIの機能を直感的に理解することができます。
 
+（準備中。。。）
+
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
 
 ## 🚀 使い方
 
 ### インストール
-HarmonAI IIのインストール手順は以下の通りです:
-
-1. リポジトリをクローンします: `git clone https://github.com/Sunwood-ai-labs/HarmonAI_II.git`
-2. 必要な依存関係をインストールします: `pip install -r requirements.txt`
-
-### 使用方法
-HarmonAI IIの使用方法は以下の通りです:
+HarmonAI IIは、以下のコマンドでインストールできます:
 
 ```bash
-git lfs install
-git lfs track "*.png"
-git lfs track "*.gif" 
-git lfs track "*.jpeg"
-git lfs track "*.jpg"
-git lfs track "*.mp4"
+pip install harmon_ai
 ```
 
-リポジトリ名を適切に変更してください:
+### 使用方法
+HarmonAI IIは、コマンドラインインターフェース(CLI)から簡単に使用できます。以下のコマンドを実行することで、プロジェクトのREADMEファイルを生成できます:
 
 ```bash
-run: git push --force https://MakiAi:$HF_TOKEN@huggingface.co/spaces/MakiAi/HarmonAI_II main
+harmon-ai --repo_name=HarmonAI_II --owner_name=Sunwood-ai-labs --package_name=harmon_ai --icon_url=https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg --title="Harmon AI"
 ```
 
+生成されたREADMEファイルは、プロジェクトのルートディレクトリに `README.md` として保存されます。
+
 ### カスタマイズ
 HarmonAI IIは、ユーザーのニーズに合わせてカスタマイズ可能です。設定ファイルを編集することで、プロジェクトの動作を柔軟に調整できます。
 
 ## 📝 アップデート
 
+### v1.3.0 (2024-05-13)
+- SNSテンプレートの追加とSNSバッジ生成機能の実装
+- CLIの強化とREADMEの更新
+- GitHub Actionsトリガーの更新
+- リファクタリングとコードのクリーンアップ
+
 ### v1.2.0 (2024-05-13)
-- `harmon_ai`パッケージの刷新
-  - `harmon_ai`クラスの実装
-  - テンプレートファイルの読み込みと置換機能の追加
-- コマンドラインインターフェース(CLI)の導入
-  - `argparse`を使用したCLIオプションの定義
-  - 生成されたREADMEファイルの出力機能の追加
+- `harmon_ai`パッケージの刷新とCLIの導入
 - READMEテンプレートファイルの拡充
-  - バッジ、重要メッセージ、README構造、セクションのテンプレートの追加
 - `harmon_ai`クラスのテストケースの実装
 - パッケージのセットアップ設定の更新
-- PyPIへのパッケージ公開ワークフローの追加
 
 ### v1.1.0 (2024-04-24)
-- フロントページの作成
-- READMEの全体的な改善
+- フロントページの作成とREADMEの改善
 - GitHub Actionsを使用したHugging Face hubへの自動シンク機能の追加
-- .gitignoreと.SourceSageignoreの更新
-- プロジェクト名を「HarmonAI」から「HarmonAI_II」に変更
+- プロジェクト名の変更
 
 ### v1.0.0 (2024-04-20)
-- 初回リリース
-- 基本的な機能を実装
+- 初回リリースと基本的な機能の実装
 
 ## 🤝 コントリビューション
 HarmonAI IIへのご協力は大歓迎です！バグ報告、機能要求、プルリクエストなどを通じて、プロジェクトの改善にご協力ください。詳細は[CONTRIBUTING.md](CONTRIBUTING.md)をご覧ください。
 
 ## 📄 ライセンス
 HarmonAI IIは[MIT License](LICENSE)の下でリリースされています。
```

### Comparing `harmon_ai-1.2.0/README.md` & `harmon_ai-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,70 +52,60 @@
 
 このテンプレートを活用することで、リポジトリ作成時の初期コストを抑えつつ、品質と開発速度を担保することができます。AI時代の開発スタイルを先取りした、生産性の高いテンプレートとしてご利用ください。
 
 ## 🎥 デモ
 
 HarmonAI IIのデモアプリケーションは、GitHub Actionsと連携し、自動的にデプロイされています。デモアプリを体験することで、HarmonAI IIの機能を直感的に理解することができます。
 
+（準備中。。。）
+
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
 
 ## 🚀 使い方
 
 ### インストール
-HarmonAI IIのインストール手順は以下の通りです:
-
-1. リポジトリをクローンします: `git clone https://github.com/Sunwood-ai-labs/HarmonAI_II.git`
-2. 必要な依存関係をインストールします: `pip install -r requirements.txt`
-
-### 使用方法
-HarmonAI IIの使用方法は以下の通りです:
+HarmonAI IIは、以下のコマンドでインストールできます:
 
 ```bash
-git lfs install
-git lfs track "*.png"
-git lfs track "*.gif" 
-git lfs track "*.jpeg"
-git lfs track "*.jpg"
-git lfs track "*.mp4"
+pip install harmon_ai
 ```
 
-リポジトリ名を適切に変更してください:
+### 使用方法
+HarmonAI IIは、コマンドラインインターフェース(CLI)から簡単に使用できます。以下のコマンドを実行することで、プロジェクトのREADMEファイルを生成できます:
 
 ```bash
-run: git push --force https://MakiAi:$HF_TOKEN@huggingface.co/spaces/MakiAi/HarmonAI_II main
+harmon-ai --repo_name=HarmonAI_II --owner_name=Sunwood-ai-labs --package_name=harmon_ai --icon_url=https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg --title="Harmon AI"
 ```
 
+生成されたREADMEファイルは、プロジェクトのルートディレクトリに `README.md` として保存されます。
+
 ### カスタマイズ
 HarmonAI IIは、ユーザーのニーズに合わせてカスタマイズ可能です。設定ファイルを編集することで、プロジェクトの動作を柔軟に調整できます。
 
 ## 📝 アップデート
 
+### v1.3.0 (2024-05-13)
+- SNSテンプレートの追加とSNSバッジ生成機能の実装
+- CLIの強化とREADMEの更新
+- GitHub Actionsトリガーの更新
+- リファクタリングとコードのクリーンアップ
+
 ### v1.2.0 (2024-05-13)
-- `harmon_ai`パッケージの刷新
-  - `harmon_ai`クラスの実装
-  - テンプレートファイルの読み込みと置換機能の追加
-- コマンドラインインターフェース(CLI)の導入
-  - `argparse`を使用したCLIオプションの定義
-  - 生成されたREADMEファイルの出力機能の追加
+- `harmon_ai`パッケージの刷新とCLIの導入
 - READMEテンプレートファイルの拡充
-  - バッジ、重要メッセージ、README構造、セクションのテンプレートの追加
 - `harmon_ai`クラスのテストケースの実装
 - パッケージのセットアップ設定の更新
-- PyPIへのパッケージ公開ワークフローの追加
 
 ### v1.1.0 (2024-04-24)
-- フロントページの作成
-- READMEの全体的な改善
+- フロントページの作成とREADMEの改善
 - GitHub Actionsを使用したHugging Face hubへの自動シンク機能の追加
-- .gitignoreと.SourceSageignoreの更新
-- プロジェクト名を「HarmonAI」から「HarmonAI_II」に変更
+- プロジェクト名の変更
 
 ### v1.0.0 (2024-04-20)
-- 初回リリース
-- 基本的な機能を実装
+- 初回リリースと基本的な機能の実装
 
 ## 🤝 コントリビューション
 HarmonAI IIへのご協力は大歓迎です！バグ報告、機能要求、プルリクエストなどを通じて、プロジェクトの改善にご協力ください。詳細は[CONTRIBUTING.md](CONTRIBUTING.md)をご覧ください。
 
 ## 📄 ライセンス
 HarmonAI IIは[MIT License](LICENSE)の下でリリースされています。
```

### Comparing `harmon_ai-1.2.0/harmon_ai.egg-info/PKG-INFO` & `harmon_ai-1.3.0/harmon_ai.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: harmon_ai
-Version: 1.2.0
+Version: 1.3.0
+Home-page: https://github.com/your_username/gaiah
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -66,70 +67,60 @@
 
 このテンプレートを活用することで、リポジトリ作成時の初期コストを抑えつつ、品質と開発速度を担保することができます。AI時代の開発スタイルを先取りした、生産性の高いテンプレートとしてご利用ください。
 
 ## 🎥 デモ
 
 HarmonAI IIのデモアプリケーションは、GitHub Actionsと連携し、自動的にデプロイされています。デモアプリを体験することで、HarmonAI IIの機能を直感的に理解することができます。
 
+（準備中。。。）
+
 [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/MakiAi/HarmonAI_II)
 
 ## 🚀 使い方
 
 ### インストール
-HarmonAI IIのインストール手順は以下の通りです:
-
-1. リポジトリをクローンします: `git clone https://github.com/Sunwood-ai-labs/HarmonAI_II.git`
-2. 必要な依存関係をインストールします: `pip install -r requirements.txt`
-
-### 使用方法
-HarmonAI IIの使用方法は以下の通りです:
+HarmonAI IIは、以下のコマンドでインストールできます:
 
 ```bash
-git lfs install
-git lfs track "*.png"
-git lfs track "*.gif" 
-git lfs track "*.jpeg"
-git lfs track "*.jpg"
-git lfs track "*.mp4"
+pip install harmon_ai
 ```
 
-リポジトリ名を適切に変更してください:
+### 使用方法
+HarmonAI IIは、コマンドラインインターフェース(CLI)から簡単に使用できます。以下のコマンドを実行することで、プロジェクトのREADMEファイルを生成できます:
 
 ```bash
-run: git push --force https://MakiAi:$HF_TOKEN@huggingface.co/spaces/MakiAi/HarmonAI_II main
+harmon-ai --repo_name=HarmonAI_II --owner_name=Sunwood-ai-labs --package_name=harmon_ai --icon_url=https://huggingface.co/datasets/MakiAi/IconAssets/resolve/main/HarmonAI_II_icon.jpeg --title="Harmon AI"
 ```
 
+生成されたREADMEファイルは、プロジェクトのルートディレクトリに `README.md` として保存されます。
+
 ### カスタマイズ
 HarmonAI IIは、ユーザーのニーズに合わせてカスタマイズ可能です。設定ファイルを編集することで、プロジェクトの動作を柔軟に調整できます。
 
 ## 📝 アップデート
 
+### v1.3.0 (2024-05-13)
+- SNSテンプレートの追加とSNSバッジ生成機能の実装
+- CLIの強化とREADMEの更新
+- GitHub Actionsトリガーの更新
+- リファクタリングとコードのクリーンアップ
+
 ### v1.2.0 (2024-05-13)
-- `harmon_ai`パッケージの刷新
-  - `harmon_ai`クラスの実装
-  - テンプレートファイルの読み込みと置換機能の追加
-- コマンドラインインターフェース(CLI)の導入
-  - `argparse`を使用したCLIオプションの定義
-  - 生成されたREADMEファイルの出力機能の追加
+- `harmon_ai`パッケージの刷新とCLIの導入
 - READMEテンプレートファイルの拡充
-  - バッジ、重要メッセージ、README構造、セクションのテンプレートの追加
 - `harmon_ai`クラスのテストケースの実装
 - パッケージのセットアップ設定の更新
-- PyPIへのパッケージ公開ワークフローの追加
 
 ### v1.1.0 (2024-04-24)
-- フロントページの作成
-- READMEの全体的な改善
+- フロントページの作成とREADMEの改善
 - GitHub Actionsを使用したHugging Face hubへの自動シンク機能の追加
-- .gitignoreと.SourceSageignoreの更新
-- プロジェクト名を「HarmonAI」から「HarmonAI_II」に変更
+- プロジェクト名の変更
 
 ### v1.0.0 (2024-04-20)
-- 初回リリース
-- 基本的な機能を実装
+- 初回リリースと基本的な機能の実装
 
 ## 🤝 コントリビューション
 HarmonAI IIへのご協力は大歓迎です！バグ報告、機能要求、プルリクエストなどを通じて、プロジェクトの改善にご協力ください。詳細は[CONTRIBUTING.md](CONTRIBUTING.md)をご覧ください。
 
 ## 📄 ライセンス
 HarmonAI IIは[MIT License](LICENSE)の下でリリースされています。
```

### Comparing `harmon_ai-1.2.0/setup.py` & `harmon_ai-1.3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="harmon_ai",
-    version="1.2.0",
+    version="1.3.0",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         # Add any dependencies here
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
         "console_scripts": [
             "harmon-ai = harmon_ai.cli:main"
         ]
     },
+    url="https://github.com/your_username/gaiah",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
```

