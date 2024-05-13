# Comparing `tmp/mlcbase-1.1.0rc1.tar.gz` & `tmp/mlcbase-1.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcbase-1.1.0rc1.tar", last modified: Sat Apr 20 15:53:37 2024, max compression
+gzip compressed data, was "mlcbase-1.2.0a1.tar", last modified: Mon May 13 14:17:51 2024, max compression
```

## Comparing `mlcbase-1.1.0rc1.tar` & `mlcbase-1.2.0a1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:37.793937 mlcbase-1.1.0rc1/
--rw-rw-rw-   0        0        0       45 2024-04-20 14:59:21.000000 mlcbase-1.1.0rc1/CHANGELOG.md
--rw-rw-rw-   0        0        0    11558 2024-04-20 07:09:17.000000 mlcbase-1.1.0rc1/LICENSE
--rw-rw-rw-   0        0        0       80 2024-04-20 15:53:21.000000 mlcbase-1.1.0rc1/MANIFEST.in
--rw-rw-rw-   0        0        0    17340 2024-04-20 15:53:37.792685 mlcbase-1.1.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2024-04-20 14:56:59.000000 mlcbase-1.1.0rc1/README.md
--rw-rw-rw-   0        0        0     1038 2024-04-20 15:42:43.000000 mlcbase-1.1.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-20 15:53:37.793937 mlcbase-1.1.0rc1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:37.774738 mlcbase-1.1.0rc1/src/
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:37.788097 mlcbase-1.1.0rc1/src/mlcbase/
--rw-rw-rw-   0        0        0     2800 2024-04-20 13:14:21.000000 mlcbase-1.1.0rc1/src/mlcbase/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-20 07:06:20.000000 mlcbase-1.1.0rc1/src/mlcbase/conifg.py
--rw-rw-rw-   0        0        0    18080 2024-04-20 07:06:24.000000 mlcbase-1.1.0rc1/src/mlcbase/database.py
--rw-rw-rw-   0        0        0    12109 2024-04-20 07:10:17.000000 mlcbase-1.1.0rc1/src/mlcbase/email.py
--rw-rw-rw-   0        0        0     2420 2024-04-20 07:07:58.000000 mlcbase-1.1.0rc1/src/mlcbase/encrypt_password.py
--rw-rw-rw-   0        0        0     6510 2024-04-20 07:07:54.000000 mlcbase-1.1.0rc1/src/mlcbase/entrypt_aes.py
--rw-rw-rw-   0        0        0    21304 2024-04-20 07:08:56.000000 mlcbase-1.1.0rc1/src/mlcbase/entrypt_rsa.py
--rw-rw-rw-   0        0        0     8787 2024-04-20 07:09:27.000000 mlcbase-1.1.0rc1/src/mlcbase/file.py
--rw-rw-rw-   0        0        0     6617 2024-04-20 07:10:23.000000 mlcbase-1.1.0rc1/src/mlcbase/loading.py
--rw-rw-rw-   0        0        0     9801 2024-04-20 07:21:17.000000 mlcbase-1.1.0rc1/src/mlcbase/logger.py
--rw-rw-rw-   0        0        0     3159 2024-04-20 07:20:31.000000 mlcbase-1.1.0rc1/src/mlcbase/misc.py
--rw-rw-rw-   0        0        0    23141 2024-04-20 11:23:15.000000 mlcbase-1.1.0rc1/src/mlcbase/remote_connect.py
--rw-rw-rw-   0        0        0     6371 2024-04-20 07:21:50.000000 mlcbase-1.1.0rc1/src/mlcbase/timer.py
--rw-rw-rw-   0        0        0     2698 2024-04-20 07:22:20.000000 mlcbase-1.1.0rc1/src/mlcbase/vault.py
--rw-rw-rw-   0        0        0     8942 2024-04-20 07:22:39.000000 mlcbase-1.1.0rc1/src/mlcbase/version.py
-drwxrwxrwx   0        0        0        0 2024-04-20 15:53:37.791669 mlcbase-1.1.0rc1/src/mlcbase.egg-info/
--rw-rw-rw-   0        0        0    17340 2024-04-20 15:53:37.000000 mlcbase-1.1.0rc1/src/mlcbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      588 2024-04-20 15:53:37.000000 mlcbase-1.1.0rc1/src/mlcbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 15:53:37.000000 mlcbase-1.1.0rc1/src/mlcbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2024-04-20 15:53:37.000000 mlcbase-1.1.0rc1/src/mlcbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-20 15:53:37.000000 mlcbase-1.1.0rc1/src/mlcbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:17:51.089435 mlcbase-1.2.0a1/
+-rw-rw-rw-   0        0        0    11558 2024-04-20 07:09:17.000000 mlcbase-1.2.0a1/LICENSE
+-rw-rw-rw-   0        0        0       41 2024-04-29 12:08:22.000000 mlcbase-1.2.0a1/MANIFEST.in
+-rw-rw-rw-   0        0        0    19305 2024-05-13 14:17:51.087447 mlcbase-1.2.0a1/PKG-INFO
+-rw-rw-rw-   0        0        0     5184 2024-05-13 14:15:59.000000 mlcbase-1.2.0a1/README.md
+-rw-rw-rw-   0        0        0     1042 2024-05-13 14:16:23.000000 mlcbase-1.2.0a1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:17:51.090434 mlcbase-1.2.0a1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:17:50.923011 mlcbase-1.2.0a1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:17:51.066834 mlcbase-1.2.0a1/src/mlcbase/
+-rw-rw-rw-   0        0        0     3550 2024-05-13 13:55:42.000000 mlcbase-1.2.0a1/src/mlcbase/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-20 07:06:20.000000 mlcbase-1.2.0a1/src/mlcbase/conifg.py
+-rw-rw-rw-   0        0        0    43359 2024-05-02 12:58:59.000000 mlcbase-1.2.0a1/src/mlcbase/database.py
+-rw-rw-rw-   0        0        0    12331 2024-05-06 12:05:35.000000 mlcbase-1.2.0a1/src/mlcbase/email.py
+-rw-rw-rw-   0        0        0     2420 2024-04-20 07:07:58.000000 mlcbase-1.2.0a1/src/mlcbase/encrypt_password.py
+-rw-rw-rw-   0        0        0     7376 2024-05-04 14:09:41.000000 mlcbase-1.2.0a1/src/mlcbase/entrypt_aes.py
+-rw-rw-rw-   0        0        0    22460 2024-05-04 14:15:41.000000 mlcbase-1.2.0a1/src/mlcbase/entrypt_rsa.py
+-rw-rw-rw-   0        0        0    12943 2024-05-03 12:38:06.000000 mlcbase-1.2.0a1/src/mlcbase/file.py
+-rw-rw-rw-   0        0        0     6854 2024-05-06 13:08:38.000000 mlcbase-1.2.0a1/src/mlcbase/image_io.py
+-rw-rw-rw-   0        0        0    12081 2024-05-12 13:37:00.000000 mlcbase-1.2.0a1/src/mlcbase/loading.py
+-rw-rw-rw-   0        0        0    10177 2024-05-08 11:36:12.000000 mlcbase-1.2.0a1/src/mlcbase/logger.py
+-rw-rw-rw-   0        0        0     6507 2024-05-13 13:55:14.000000 mlcbase-1.2.0a1/src/mlcbase/misc.py
+-rw-rw-rw-   0        0        0    13433 2024-05-05 09:46:56.000000 mlcbase-1.2.0a1/src/mlcbase/otp.py
+-rw-rw-rw-   0        0        0    23510 2024-05-06 08:58:30.000000 mlcbase-1.2.0a1/src/mlcbase/remote_connect.py
+-rw-rw-rw-   0        0        0     6392 2024-05-02 15:04:32.000000 mlcbase-1.2.0a1/src/mlcbase/timer.py
+-rw-rw-rw-   0        0        0   179912 2024-05-13 12:03:42.000000 mlcbase-1.2.0a1/src/mlcbase/vault.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:17:51.084403 mlcbase-1.2.0a1/src/mlcbase.egg-info/
+-rw-rw-rw-   0        0        0    19305 2024-05-13 14:17:50.000000 mlcbase-1.2.0a1/src/mlcbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      595 2024-05-13 14:17:50.000000 mlcbase-1.2.0a1/src/mlcbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:17:50.000000 mlcbase-1.2.0a1/src/mlcbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2024-05-13 14:17:50.000000 mlcbase-1.2.0a1/src/mlcbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-13 14:17:50.000000 mlcbase-1.2.0a1/src/mlcbase.egg-info/top_level.txt
```

### Comparing `mlcbase-1.1.0rc1/LICENSE` & `mlcbase-1.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcbase-1.1.0rc1/PKG-INFO` & `mlcbase-1.2.0a1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mlcbase
-Version: 1.1.0rc1
+Version: 1.2.0a1
 Summary: The base module of all MuLingCloud modules and applications.
-Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>, Zilin Yang <876497115@qq.com>
+Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -214,35 +214,34 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: loguru
 Requires-Dist: pytz
 Requires-Dist: prettytable
 Requires-Dist: pyyaml
-Requires-Dist: xmltodict
 Requires-Dist: rsa
 Requires-Dist: pycryptodome
+Requires-Dist: requests
 Requires-Dist: paramiko
 Requires-Dist: PyMySQL
-Requires-Dist: hvac
+Requires-Dist: pyotp
+Requires-Dist: qrcode[pil]
+Requires-Dist: opencv-python
+Requires-Dist: matplotlib
 
 <div align="center">
     <img src="https://lychee.weimingchen.net:1130/uploads/original/dc/0e/eae6786c5d68d4a564f8e3f60157.png" width="100%" />
 </div>
 
 <div align="center">
-    <a href="https://pypi.org/project/mlcbase">
-        <img src="https://img.shields.io/pypi/v/mlcbase" />
-    </a>
-    <a href="./LICENSE">
-        <img src="https://img.shields.io/github/license/wmchen/mlcbase.svg" />
-    </a>
-    <a href="https://weimingchen.net">
-        <img src="https://img.shields.io/badge/author-Weiming_Chen-royalblue" />
-    </a>
+
+[![PyPI](https://img.shields.io/pypi/v/mlcbase)](https://pypi.org/project/mlcbase/)
+[![License](https://img.shields.io/github/license/wmchen/mlcbase.svg)](https://www.apache.org/licenses/LICENSE-2.0)
+[![All Contributors](https://img.shields.io/github/all-contributors/wmchen/mlcbase?color=blue)](#contributors)
+
 </div>
 
 ## Introduction
 
 Welcome to use MuLingCloud. We aim to let everything easier.
 
 MLCBase is an open source Python library for multiple uses. It is the base module of all MuLingCloud modules and applications.
@@ -250,55 +249,59 @@
 Supported platforms:
 
 - 😄 Windows (Python 3.6+)
 - 😄 Linux (Python 3.7+)
 - MacOS (untested, maybe. I don't have a MacOS machine😫. Anyone can help me?)
 
 <details open>
-<summary>Features</summary>
-
-- **Version**
-
-    We define a `Version` class to manage the version of all MuLingCloud modules or applications. The instantiated versions can easily compare their order by using comparision operators, i.e. `==`, `!=`, `<`, `<=`, `>`, `>=`.
+<summary>Features (v1.2.0a1)</summary>
 
 - **Config Dictionary**
 
     We define a `ConfigDict` for more convenience usage. It is a type of dictionary inherited from `dict`. It has all the features of `dict` while including other more convenient features.
 
-- **Logger**
+- $\color{blue}{\textbf{update }}$ **Logger**
 
     We build a `Logger` for more convenience logging management. Actually, this is a slightly improvement based on [loguru](https://github.com/Delgan/loguru). Refer to [pylog](https://github.com/wmchen/pylog) for more information.
 
-- **Runtime Analysis**
+- $\color{blue}{\textbf{update }}$ **Runtime Analysis**
 
     We offer a simple way to evaluate functions in the Python project. All you need is to wrap the target function by a decorator.
 
-- **File Operations**
+- $\color{blue}{\textbf{update }}$ **File Operations**
+
+    We offer various features to make file operations easier. Besides, we offer a simple way to load and save JSON, YAML, and XML files.
+
+- $\color{red}{\textbf{new }}$ **Image IO**
+
+    We offer a simple way to load and save images.
+
+- $\color{red}{\textbf{new }}$ **One-Time Password**
 
-    We offer various features to make file operations easier.
+    We support two methods for OTP: Time-based One-Time Password (TOTP) and HMAC-based One-Time Password (HOTP).
 
-- **Encryption and Decryption**
+- $\color{blue}{\textbf{update }}$ **Encryption and Decryption**
 
     We offer various methods to encrypt and decrypt or verify text, files and passwords including RSA, AES and Hash.
 
-- **Database**
+- $\color{blue}{\textbf{update }}$ **Database**
 
-    We offer a simple way to operate the database including creating a data table, inserting data, deleting data, searching data, and updating data. Currently only supports MySQL backend, but other backends will be supported in the future.
+    We offer a simple way to operate the database. Supported database backend: MySQL, SQLite.
 
 - **Remote Connection**
 
     We support SSH and SFTP for remote connection.
 
-- **Email**
+- $\color{blue}{\textbf{update }}$ **Email**
 
     We offer a simple API to send email. Currently only supports SMTP (with SSL) server.
 
-- **HashiCorp Vault**
+- $\color{red}{\textbf{BREAKING CHANGE }}$ **HashiCorp Vault**
 
-    We offer a simple API to get secrets from [HashiCorp/Vault](https://developer.hashicorp.com/vault). Currently only supports the secret engine of `kv2`, but other type of secret engines will be supported in the future.
+    We offer several APIs to operate [HashiCorp/Vault](https://developer.hashicorp.com/vault) through HTTP requests. Supported authorization methods: token, username & password. Supported secret engines: KV v1, KV v2, TOTP, Transit.
 
 </details>
 
 ## Installation
 
 ```bash
 pip install mlcbase
@@ -312,10 +315,36 @@
 
 See all changes in [CHANGELOG](./CHANGELOG.md).
 
 ## Contributors
 
 We appreciate all the contributors who add new features or fix bugs, as well as the users who offer valuable feedback.
 
+We welcome all contributors, feel free to create an issue or file a pull request and join us! ❤️
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://weimingchen.net/"><img src="https://avatars.githubusercontent.com/u/33000375?v=4?s=100" width="100px;" alt="Weiming Chen"/><br /><sub><b>Weiming Chen</b></sub></a><br /><a href="https://github.com/wmchen/mlcbase/commits?author=wmchen" title="Code">💻</a> <a href="#ideas-wmchen" title="Ideas, Planning, & Feedback">🤔</a> <a href="#projectManagement-wmchen" title="Project Management">📆</a> <a href="https://github.com/wmchen/mlcbase/commits?author=wmchen" title="Tests">⚠️</a> <a href="#tutorial-wmchen" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.mulingcloud.com/author/yuanshuang-sun/"><img src="https://avatars.githubusercontent.com/u/32105419?v=4?s=100" width="100px;" alt="Yuanshuang Sun"/><br /><sub><b>Yuanshuang Sun</b></sub></a><br /><a href="#ideas-dcsasori" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/wmchen/mlcbase/commits?author=dcsasori" title="Tests">⚠️</a> <a href="#tutorial-dcsasori" title="Tutorials">✅</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+
 ## License
 
-This project is released under the [Apache 2.0 license](./LICENSE).
+This project is released under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0).
+
+## Repository
+
+- Github Repository: https://github.com/wmchen/mlcbase
+- GitLab Repository: https://gitlab.com/wm-chen/mlcbase
+- Gitee Repository: https://gitee.com/wm-chen/mlcbase
```

### Comparing `mlcbase-1.1.0rc1/pyproject.toml` & `mlcbase-1.2.0a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlcbase"
-version = "1.1.0.rc1"
+version = "1.2.0a1"
 authors = [
     {name = "Weiming Chen", email = "wm_chen@yeah.net"},
-    {name = "Yuanshuang Sun", email = "sunsun5544@126.com"},
-    {name = "Zilin Yang", email = "876497115@qq.com"}
+    {name = "Yuanshuang Sun", email = "sunsun5544@126.com"}
 ]
 description = "The base module of all MuLingCloud modules and applications."
 readme = {"file" = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 dependencies = [
     "colorama",
     "loguru",
     "pytz",
     "prettytable",
     "pyyaml",
-    "xmltodict",
     "rsa",
     "pycryptodome",
+    "requests",
     "paramiko",
     "PyMySQL",
-    "hvac"
+    "pyotp",
+    "qrcode[pil]",
+    "opencv-python",
+    "matplotlib",
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS",
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/__init__.py` & `mlcbase-1.2.0a1/src/mlcbase/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,44 +8,50 @@
 # 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .version import Version
 from .conifg import ConfigDict, is_config_dict
 from .logger import Logger
-from .timer import wrap_module_timer, delete_register_modules, runtime_analysis
-from .file import mkdir, listdir, get_file_size, get_dir_size, get_meta_info
+from .timer import wrap_module_timer, delete_register_modules, show_register_modules, runtime_analysis
+from .file import create, remove, listdir, get_file_size, get_dir_size, get_meta_info
 from .loading import load_json, save_json, load_yaml, save_yaml, load_xml, save_xml
+from .image_io import get_image_from_url, load_image, save_image
 from .encrypt_password import encrypt_password, verify_password
 from .entrypt_aes import aes_encrypt_text, aes_decrypt_text, aes_entrypt_file, aes_decrypt_file
 from .entrypt_rsa import (create_rsa_keys, rsa_encrypt_text, rsa_decrypt_text, rsa_sign_text,
                           rsa_verify_signature, rsa_encrypt_file, rsa_decrypt_file)
-from .vault import VaultAPI
-from .database import MySQLAPI
+from .otp import generate_otp_secret, generate_otp_code, verify_otp_code
+from .vault import (VaultDuration, VaultSecretEngineKV1, VaultSecretEngineKV2, VaultSecretEngineTOTP, 
+                    VaultSecretEngineTransit)
+from .database import MySQLAPI, SQLiteAPI
 from .remote_connect import SSH, SFTP
 from .email import SMTPAPI
 from .misc import (is_type, is_bytes, is_str, is_int, is_float, is_bool, is_list, is_dict,
-                   is_tuple, is_path, is_net_ok, random_hex)
+                   is_tuple, is_path, is_url, is_base64, random_hex, random_otp_secret, get_mac_address,
+                   is_canonical_version, parse_version)
 
 __all__ = [
     "Version", "ConfigDict", "is_config_dict", "Logger", "wrap_module_timer", "delete_register_modules", 
-    "runtime_analysis", "mkdir", "listdir", "get_file_size", "get_dir_size", "get_meta_info", "load_json", 
-    "save_json", "load_yaml", "save_yaml", "load_xml", "save_xml", "encrypt_password", "verify_password", 
-    "aes_encrypt_text", "aes_decrypt_text", "aes_entrypt_file", "aes_decrypt_file", "create_rsa_keys", 
-    "rsa_encrypt_text", "rsa_decrypt_text", "rsa_sign_text", "rsa_verify_signature", "rsa_encrypt_file", 
-    "rsa_decrypt_file", "VaultAPI", "MySQLAPI", "SSH", "SFTP", "SMTPAPI", "is_type", "is_bytes", 
-    "is_str", "is_int", "is_float", "is_bool", "is_list", "is_dict", "is_tuple", "is_path", 
-    "is_net_ok", "random_hex"
+    "runtime_analysis", "show_register_modules", "create", "remove", "listdir", "get_file_size", "get_dir_size", 
+    "get_meta_info", "load_json", "save_json", "load_yaml", "save_yaml", "load_xml", "save_xml", 
+    "get_image_from_url", "load_image", "save_image", "encrypt_password", "verify_password", "aes_encrypt_text", 
+    "aes_decrypt_text", "aes_entrypt_file", "aes_decrypt_file", "create_rsa_keys", "rsa_encrypt_text", 
+    "rsa_decrypt_text", "rsa_sign_text", "rsa_verify_signature", "rsa_encrypt_file", "rsa_decrypt_file", 
+    "generate_otp_secret", "generate_otp_code", "verify_otp_code", "VaultDuration", "VaultSecretEngineKV1", 
+    "VaultSecretEngineKV2", "VaultSecretEngineTOTP", "VaultSecretEngineTransit", "MySQLAPI", "SQLiteAPI", 
+    "SSH", "SFTP", "SMTPAPI", "is_type", "is_bytes", "is_str", "is_int", "is_float", "is_bool", "is_list", 
+    "is_dict", "is_tuple", "is_path", "is_url", "is_base64", "random_hex", "random_otp_secret", "get_mac_address",
+    "is_canonical_version", "parse_version"
 ]
 
 
-__version__ = "1.1.0.rc1"
+__version__ = "1.2.0a1"
 TYPE_NAME = "module"
 NAME = "mlcbase"
 DESCRIPTION = "The base module of all MuLingCloud modules and applications."
 
 
 if not hasattr(__import__(NAME), NAME):
     from colorama import Fore
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/conifg.py` & `mlcbase-1.2.0a1/src/mlcbase/conifg.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/email.py` & `mlcbase-1.2.0a1/src/mlcbase/email.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from email.utils import formataddr
 from email import encoders
 
 from .logger import Logger
 from .file import get_file_size
 from .conifg import ConfigDict
 from .remote_connect import SFTP
-from .misc import is_str, FileTooLargeError, FileUploadError
+from .misc import is_str, is_dict, FileTooLargeError, FileUploadError
 
 PathLikeType = Union[str, Path]
 
 
 class SMTPAPI:
     def __init__(self, 
                  host: str,
@@ -57,15 +57,15 @@
         """An api for SMTP server
 
         Args:
             host (str)
             port (int)
             name (str): sender name
             address (str): sender email address
-            password (str): _description_
+            password (str): the password or the authorize code
             timeout (int, optional): Defaults to 30 seconds.
             chunk_size (int, optional): large attachment chunk size. if large than the chunk_size, 
                                         the large attachment will upload to the remote sever rather 
                                         than attaching to the email message. Defaults to 30 (MB).
             work_dir (Optional[PathLikeType], optional): will save the log file to "work_dir/log/" if 
                                                          work_dir is specified. Defaults to None.
             logger (Optional[Logger], optional): Defaults to None.
@@ -94,27 +94,27 @@
     def send_email(self, 
                    receiver_name: Union[str, List[str]],
                    receiver_email: Union[str, List[str]],
                    subject: str,
                    content: str,
                    signature: Optional[str] = None,
                    attachment: Optional[Union[PathLikeType, List[PathLikeType]]] = None,
-                   remote_server_config: Optional[ConfigDict] = None,
+                   remote_server_config: Optional[dict] = None,
                    encoding: str = "utf-8"):
         """send email
 
         Args:
             receiver_name (Union[str, List[str]])
             receiver_email (Union[str, List[str]])
             subject (str): subject of the email
             content (str): content of the email (will be parsed to html)
             signature (Optional[str], optional): signature at the botom of the email message. Defaults to None.
             attachment (Optional[Union[PathLikeType, List[PathLikeType]]], optional): attachments' path. Defaults to None.
-            remote_server_config (Optional[ConfigDict], optional): config of the remote server, is required when the large 
-                                                                   attachments are included. Defaults to None.
+            remote_server_config (Optional[dict], optional): config of the remote server, is required when the large 
+                                                             attachments are included. Defaults to None.
             encoding (str, optional): Defaults to "utf-8".
             
         Form of remote_server_config:
         >>> remote_server_config = ConfigDict(host={host of remote server},
         >>>                                   port={port of remote server},
         >>>                                   user={username of remote server},
         >>>                                   password={password of remote server},
@@ -137,14 +137,18 @@
             raise smtplib.SMTPException("email server connection is not established")
         
         assert type(receiver_name) == type(receiver_email), "receiver_name and receiver_email should have the same type"
         if is_str(receiver_name):
             receiver_name = [receiver_name]
             receiver_email = [receiver_email]
         assert len(receiver_name) == len(receiver_email), "receiver_name and receiver_email should have the same length"
+        assert remote_server_config is None or is_dict(remote_server_config), \
+            "if remote_server_config is not None, it should be a dict"
+        if is_dict(remote_server_config):
+            remote_server_config = ConfigDict(remote_server_config)
         
         # distinguish attachments with chunk size
         if attachment is not None:
             if is_str(attachment):
                 attachment = [attachment]
             
             upload2remote = []
@@ -164,34 +168,34 @@
                     attach2email.append(str(Path(p).absolute()))
                 
             has_attachment = True
         else:
             has_attachment = False
         
         # upload large attachment to remote server
-        if has_attachment:
+        if has_attachment and len(upload2remote) > 0:
+            sftp_api = SFTP(host=remote_server_config.host,
+                            port=remote_server_config.port,
+                            user=remote_server_config.user,
+                            password=remote_server_config.password,
+                            work_dir=self.work_dir,
+                            logger=self.logger,
+                            quiet=self.quiet)
+            if sftp_api is None:
+                raise ConnectionError("remote server connect error")
+            
             save_dir = remote_server_config.save_director
             remote_platform = remote_server_config.remote_platform
             callback = remote_server_config.callback
-            if len(upload2remote) > 0:
-                sftp_api = SFTP(host=remote_server_config.host,
-                                port=remote_server_config.port,
-                                user=remote_server_config.user,
-                                password=remote_server_config.password,
-                                work_dir=self.work_dir,
-                                logger=self.logger,
-                                quiet=self.quiet)
-                if sftp_api is None:
-                    raise ConnectionError("remote server connect error")
-
-                for p in upload2remote:
-                    if not sftp_api.upload_file(p, os.path.join(save_dir, Path(p).name), remote_platform, callback):
-                        raise FileUploadError(f"{p} upload to remote server error")
-                
-                sftp_api.close()
+
+            for p in upload2remote:
+                if not sftp_api.upload_file(p, os.path.join(save_dir, Path(p).name), remote_platform, callback):
+                    raise FileUploadError(f"{p} upload to remote server error")
+            
+            sftp_api.close()
 
         # build email content and attachments
         for name, email in zip(receiver_name, receiver_email):
             message = MIMEMultipart()
             message["From"] = formataddr((self.__name, self.__address))
             message["To"] = formataddr((name, email))
             message["Subject"] = Header(subject, encoding).encode(encoding)
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/encrypt_password.py` & `mlcbase-1.2.0a1/src/mlcbase/encrypt_password.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/entrypt_aes.py` & `mlcbase-1.2.0a1/src/mlcbase/entrypt_aes.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,23 +24,24 @@
 
 from .logger import Logger
 from .misc import is_str, is_bytes
 
 PathLikeType = Union[str, Path]
 
 
-def __add_16(p: Union[str, bytes], encoding: str = "utf-8"):
-    assert is_str(p) or is_bytes(p), 'p must be str or bytes'
-    if is_str(p):
-        p = p.encode(encoding)
+def __completion(conent: Union[str, bytes], encoding: str = "utf-8"):
+    assert is_str(conent) or is_bytes(conent), 'conent must be str or bytes'
 
-    while len(p) % 16 != 0:
-        p += b'\x00'
+    if is_str(conent):
+        conent = conent.encode(encoding)
     
-    return p
+    while len(conent) % 16 != 0:
+        conent += b'\x00'
+    
+    return conent
 
 
 def aes_encrypt_text(plain_text: str,
                      key: Union[str, bytes],
                      iv: Optional[Union[str, bytes]] = None,
                      mode: int = AES.MODE_CBC,
                      encoding: str = "utf-8"):
@@ -52,19 +53,25 @@
         iv (Optional[Union[str, bytes]], optional): Defaults to None.
         mode (int, optional): Defaults to AES.MODE_CBC.
         encoding (str, optional): Defaults to "utf-8".
 
     Returns:
         bytes: cipher text
     """
+    assert is_str(key) or is_bytes(key), 'key must be str or bytes'
+    assert len(key) in [16, 24, 32], 'the length of key must be 16, 24 or 32'
+    assert iv is None or ((is_str(iv) or is_bytes(iv)) and len(iv) == 16), \
+        'when iv is not None, iv must be str or bytes, and the length of iv should be 16'
     assert mode in [AES.MODE_CBC, AES.MODE_ECB], 'currently only support AES.MODE_CBC or AES.MODE_ECB mode'
-    plain_text = __add_16(plain_text, encoding)
-    key = __add_16(key, encoding)
+
+    key = key.encode(encoding) if is_str(key) else key
     if iv is not None:
-        iv = __add_16(iv, encoding)
+        iv = iv.encode(encoding) if is_str(iv) else iv
+
+    plain_text = __completion(plain_text, encoding)
     
     if mode == AES.MODE_CBC:
         assert iv is not None, 'iv must be provided when using AES.MODE_CBC mode'
         cipher_text = AES.new(key, mode, iv).encrypt(plain_text)
 
     if mode == AES.MODE_ECB:
         cipher_text = AES.new(key, mode).encrypt(plain_text)
@@ -86,20 +93,25 @@
         iv (Optional[Union[str, bytes]], optional): Defaults to None.
         mode (int, optional): Defaults to AES.MODE_CBC.
         return_str (bool, optional): return a string if True, otherwise return a bytes.
                                      Defaults to True.
         encoding (str, optional): Defaults to "utf-8".
 
     Returns:
-        str: plain text
+        str or bytes: return a string if return_str is True, otherwise return a bytes
     """
+    assert is_str(key) or is_bytes(key), 'key must be str or bytes'
+    assert len(key) in [16, 24, 32], 'the length of key must be 16, 24 or 32'
+    assert iv is None or ((is_str(iv) or is_bytes(iv)) and len(iv) == 16), \
+        'when iv is not None, iv must be str or bytes, and the length of iv should be 16'
     assert mode in [AES.MODE_CBC, AES.MODE_ECB], 'currently only support AES.MODE_CBC or AES.MODE_ECB mode'
-    key = __add_16(key)
+
+    key = key.encode(encoding) if is_str(key) else key
     if iv is not None:
-        iv = __add_16(iv)
+        iv = iv.encode(encoding) if is_str(iv) else iv
     
     if mode == AES.MODE_CBC:
         assert iv is not None, 'iv must be provided when using AES.MODE_CBC mode'
         plain_text = AES.new(key, mode, iv).decrypt(cipher_text)
     
     if mode == AES.MODE_ECB:
         plain_text = AES.new(key, mode).decrypt(cipher_text)
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/entrypt_rsa.py` & `mlcbase-1.2.0a1/src/mlcbase/entrypt_rsa.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Thread.__init__(self)
         self.plain_text = plain_text
         self.public_key = public_key
         self.key_length = key_length
         self.cipher_text = None
 
     def run(self):
-        default_length = int(self.key_length / 8 - 11)
+        default_length = self.key_length // 8 - 11
         if len(self.plain_text) <= default_length:
             cipher_text = rsa.encrypt(self.plain_text, self.public_key)
         else:
             offset = 0
             cipher_text = []
             while len(self.plain_text) - offset > 0:
                 if len(self.plain_text) - offset > default_length:
@@ -53,20 +53,21 @@
                 else:
                     cipher_text.append(rsa.encrypt(self.plain_text[offset:], self.public_key))
                 offset += default_length
         self.cipher_text = cipher_text
 
 
 class _DecryptTextThread(Thread):
-    def __init__(self, cipher_text, private_key, encoding, return_str):
+    def __init__(self, cipher_text, private_key, encoding, return_str, key_length):
         Thread.__init__(self)
         self.cipher_text = cipher_text
         self.private_key = private_key
         self.encoding = encoding
         self.return_str = return_str
+        self.key_length = key_length
         self.plain_text = None
 
     def run(self):
         if is_list(self.cipher_text):
             if self.return_str:
                 plain_text = ""
             else:
@@ -76,57 +77,64 @@
                 if self.return_str:
                     plain_text += rsa.decrypt(c, self.private_key).decode(self.encoding)
                 else:
                     plain_text += rsa.decrypt(c, self.private_key)
         
         if is_bytes(self.cipher_text):
             length = len(self.cipher_text)
-            if length > 128:
+            chunk_length = self.key_length // 8
+            if length > chunk_length:
                 offset = 0
                 if self.return_str:
                     plain_text = ""
                 else:
                     plain_text = b""
 
                 while length - offset > 0:
-                    if length - offset > 128:
+                    if length - offset > chunk_length:
                         if self.return_str:
-                            plain_text += rsa.decrypt(self.cipher_text[offset:offset+128], self.private_key).decode(self.encoding)
+                            plain_text += rsa.decrypt(self.cipher_text[offset:offset+chunk_length], self.private_key).decode(self.encoding)
                         else:
-                            plain_text += rsa.decrypt(self.cipher_text[offset:offset+128], self.private_key)
+                            plain_text += rsa.decrypt(self.cipher_text[offset:offset+chunk_length], self.private_key)
                     else:
                         if self.return_str:
                             plain_text += rsa.decrypt(self.cipher_text[offset:], self.private_key).decode(self.encoding)
                         else:
                             plain_text += rsa.decrypt(self.cipher_text[offset:], self.private_key)
-                    offset += 128
+                    offset += chunk_length
             else:
                 if self.return_str:
                     plain_text = rsa.decrypt(self.cipher_text, self.private_key).decode(self.encoding)
                 else:
                     plain_text = rsa.decrypt(self.cipher_text, self.private_key)
         
         self.plain_text = plain_text
 
 
 def create_rsa_keys(public_path: Optional[PathLikeType] = None, 
                     private_path: Optional[PathLikeType] = None, 
-                    key_length: int = 1024,
+                    key_length: int = 2048,
                     return_keys: bool = False):
     """create a pair of rsa keys
 
     Args:
         public_path (Optional[PathLikeType], optional): Defaults to None.
         private_path (Optional[PathLikeType], optional): Defaults to None.
-        key_length (int, optional): Defaults to 1024.
+        key_length (int, optional): We force the length of key must be larger or equal to 2048 for safety resons. 
+                                    Common options including 2048, 3072, and 4096. Defaults to 2048.
         return_keys (bool, optional): Defaults to False.
 
     Returns:
         tuple or None: return a pair of rsa keys if return_keys is True, otherwise return None
     """
+    assert key_length >= 2048, "Force the key_length must be larger or equal to 2048 for safety resons"
+    assert key_length % 8 == 0, "The length of secret key must be a multiple of 8"
+    assert (public_path is not None and private_path is not None) or return_keys, \
+        "public_path and private_path must be provided if return_keys is False"
+
     (public_key, private_key) = rsa.newkeys(key_length)
     public_key = public_key.save_pkcs1("PEM")
     private_key = private_key.save_pkcs1("PEM")
     if public_path and private_path:
         assert public_path.endswith(".pem"), "public key file must be a PEM file"
         assert private_path.endswith(".pem"), "private key file must be a PEM file"
 
@@ -139,30 +147,31 @@
         return (public_key, private_key)
     else:
         return None
 
 
 def rsa_encrypt_text(plain_text: Union[str, bytes], 
                      public_key: Union[bytes, PathLikeType], 
-                     key_length: int = 1024,
+                     key_length: int = 2048,
                      num_threads: int = 1,
                      encoding: str = "utf-8"):
     """encrypt plain text with rsa public key
 
     Args:
         plain_text (Union[str, bytes])
         public_key (Union[bytes, PathLikeType)
-        key_length (int, optional): Defaults to 1024.
+        key_length (int, optional): Defaults to 2048.
         num_threads (int, optional): thread numbers to use, which is larger or equal to 1. 
-                                    Defaults to 1.
+                                     Defaults to 1.
         encoding (str, optional): Defaults to "utf-8".
 
     Returns:
         bytes or List[bytes]: cipher_text
     """
+    assert key_length % 8 == 0, "The length of secret key must be a multiple of 8"
     assert is_str(plain_text) or is_bytes(plain_text), "plain_text must be a string or bytes"
     assert is_str(public_key) or is_path(public_key) or is_bytes(public_key), \
         "public_key must be a bytes or a path"
 
     # load public key
     if is_str(public_key) or is_path(public_key):
         with open(public_key, "rb") as f:
@@ -172,15 +181,14 @@
     
     if is_str(plain_text):
         plain_text = plain_text.encode(encoding)
     
     # split plain_text into multiple threads
     if num_threads > 1:
         length = len(plain_text) // num_threads
-        # cipher_dict = {}
         threads = []
         for i in range(num_threads):
             if i < num_threads - 1:
                 thread = _EncryptTextThread(plain_text[i * length:(i + 1) * length], key, key_length)
             else:
                 thread = _EncryptTextThread(plain_text[i * length:], key, key_length)
             threads.append(thread)
@@ -190,15 +198,15 @@
         for thread in threads:
             thread.join()
             if is_list(thread.cipher_text):
                 cipher_text.extend(thread.cipher_text)
             if is_bytes(thread.cipher_text):
                 cipher_text.append(thread.cipher_text)
     else:
-        default_length = int(key_length / 8 - 11)
+        default_length = key_length // 8 - 11
         if len(plain_text) <= default_length:
             cipher_text = rsa.encrypt(plain_text, key)
         else:
             offset = 0
             cipher_text = []
             while len(plain_text) - offset > 0:
                 if len(plain_text) - offset > default_length:
@@ -208,31 +216,34 @@
                 offset += default_length
     
     return cipher_text
 
 
 def rsa_decrypt_text(cipher_text: Union[List[bytes], bytes],
                      private_key: Union[bytes, PathLikeType],
+                     key_length: int = 2048,
                      num_threads: int = 1,
                      return_str: bool = True,
                      encoding: str = "utf-8",):
     """decrypt cipher text with rsa private key
 
     Args:
         cipher_text (Union[List[bytes], bytes])
         private_key (Union[bytes, PathLikeType])
+        key_length (int, optional): Defaults to 2048.
         num_threads (int, optional): thread numbers to use, which is larger or equal to 1. 
                                     Defaults to 1.
         return_str (bool, optional): return a string if True, otherwise return a bytes.
                                      Defaults to True.
         encoding (str, optional): Defaults to "utf-8".
 
     Returns:
         str or bytes: return a string if return_str is True, otherwise return a bytes
     """
+    assert key_length % 8 == 0, "The length of secret key must be a multiple of 8"
     assert is_list(cipher_text) or is_bytes(cipher_text), "cipher_text must be a list or bytes"
     assert is_str(private_key) or is_path(private_key) or is_bytes(private_key), \
         "private_key must be a bytes or a path"
 
     # load private key
     if is_str(private_key) or is_path(private_key):
         with open(private_key, "rb") as f:
@@ -242,17 +253,17 @@
 
     # split cipher_text into multiple threads
     if num_threads > 1:
         length = len(cipher_text) // num_threads
         threads = []
         for i in range(num_threads):
             if i < num_threads - 1:
-                thread = _DecryptTextThread(cipher_text[i*length:(i+1)*length], key, encoding, return_str)
+                thread = _DecryptTextThread(cipher_text[i*length:(i+1)*length], key, encoding, return_str, key_length)
             else:
-                thread = _DecryptTextThread(cipher_text[i*length:], key, encoding, return_str)
+                thread = _DecryptTextThread(cipher_text[i*length:], key, encoding, return_str, key_length)
             threads.append(thread)
             thread.start()
             
         if return_str:
             plain_text = ""
         else:
             plain_text = b""
@@ -271,33 +282,34 @@
                 if return_str:
                     plain_text += rsa.decrypt(c, key).decode(encoding)
                 else:
                     plain_text += rsa.decrypt(c, key)
         
         if is_bytes(cipher_text):
             length = len(cipher_text)
-            if length > 128:
+            chunk_length = key_length // 8
+            if length > chunk_length:
                 offset = 0
                 if return_str:
                     plain_text = ""
                 else:
                     plain_text = b""
 
                 while length - offset > 0:
-                    if length - offset > 128:
+                    if length - offset > chunk_length:
                         if return_str:
-                            plain_text += rsa.decrypt(cipher_text[offset:offset+128], key).decode(encoding)
+                            plain_text += rsa.decrypt(cipher_text[offset:offset+chunk_length], key).decode(encoding)
                         else:
-                            plain_text += rsa.decrypt(cipher_text[offset:offset+128], key)
+                            plain_text += rsa.decrypt(cipher_text[offset:offset+chunk_length], key)
                     else:
                         if return_str:
                             plain_text += rsa.decrypt(cipher_text[offset:], key).decode(encoding)
                         else:
                             plain_text += rsa.decrypt(cipher_text[offset:], key)
-                    offset += 128
+                    offset += chunk_length
             else:
                 if return_str:
                     plain_text = rsa.decrypt(cipher_text, key).decode(encoding)
                 else:
                     plain_text = rsa.decrypt(cipher_text, key)
         
     return plain_text
@@ -309,14 +321,15 @@
                   encoding: str = "utf-8"):
     """sign plain text with rsa private key
 
     Args:
         plain_text (str)
         private_key (Union[bytes, PathLikeType])
         hash_method (str, optional): Defaults to 'SHA-512'.
+        encoding (str, optional): Defaults to "utf-8".
         
     Returns:
         bytes: signed cipher text
     """
     assert is_str(plain_text), "plain_text must be a string"
     assert is_str(private_key) or is_path(private_key) or is_bytes(private_key), \
         "private_key must be a bytes or a path"
@@ -330,59 +343,59 @@
     
     signed_cipher_text = rsa.sign(plain_text.encode(encoding), key, hash_method)
 
     return signed_cipher_text
 
 
 def rsa_verify_signature(plain_text: str,
-                         signed_cipher_text: bytes,
+                         signature: bytes,
                          public_key: Union[bytes, PathLikeType],
                          encoding: str = "utf-8"):
     """verify signature with rsa public key
 
     Args:
         plain_text (str)
-        signed_cipher_text (bytes)
+        signature (bytes)
         public_key (Union[bytes, PathLikeType])
         encoding (str, optional): Defaults to "utf-8".
 
     Returns:
         bool: return True if the signature match the plain text, otherwise return False
     """
     assert is_str(plain_text), "plain_text must be a string"
-    assert is_bytes(signed_cipher_text), "signed_cipher_text must be a bytes"
+    assert is_bytes(signature), "signed_cipher_text must be a bytes"
     
     if is_str(public_key) or is_path(public_key):
         with open(public_key, "rb") as f:
             key = rsa.PublicKey.load_pkcs1(f.read())
     else:
         key = rsa.PublicKey.load_pkcs1(public_key)
 
     try:
-        rsa.verify(plain_text.encode(encoding), signed_cipher_text, key)
+        rsa.verify(plain_text.encode(encoding), signature, key)
         return True
     except:
         return False
 
 
 def rsa_encrypt_file(plain_file_path: PathLikeType, 
                      crypto_save_path: PathLikeType, 
                      public_key: Union[bytes, PathLikeType], 
-                     key_length: int = 1024,
+                     key_length: int = 2048,
                      num_process: int = 1,
                      num_threads: int = 1,
                      encoding: str = "utf-8",
                      logger: Optional[Logger] = None):
     """encrypt file with rsa public key
 
     Args:
         plain_file_path (PathLikeType)
         crypto_save_path (PathLikeType)
         public_key (Union[bytes, PathLikeType])
-        key_length (int, optional): Defaults to 1024.
+        key_length (int, optional): Defaults to 2048.
         num_process (int, optional): number of processes. Defaults to 1.
         num_threads (int, optional): number of threads. Defaults to 1.
         encoding (str, optional): Defaults to "utf-8".
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
         bool: return True if the file is encrypted successfully, otherwise return False
@@ -451,24 +464,26 @@
             logger.error(f'rsa encrypt file error: {str(e)}')
         return False
 
 
 def rsa_decrypt_file(crypto_file_path: PathLikeType,
                      plain_save_path: PathLikeType,
                      private_key: Union[bytes, PathLikeType],
+                     key_length: int = 2048,
                      num_process: int = 1,
                      num_threads: int = 1,
                      encoding: str = "utf-8",
                      logger: Optional[Logger] = None):
     """decrypt file with rsa private key
 
     Args:
         crypto_file_path (PathLikeType)
         plain_save_path (PathLikeType)
         private_key (Union[bytes, PathLikeType])
+        key_length (int, optional): Defaults to 2048.
         num_process (int, optional): number of processes. Defaults to 1.
         num_threads (int, optional): number of threads. Defaults to 1.
         encoding (str, optional): Defaults to "utf-8".
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
         bool: return True if the file is decrypted successfully, otherwise return False
@@ -500,23 +515,23 @@
             
             # decrypt
             pool = mp.Pool(num_process)
             plain_list = []
             for i in range(num_process):
                 with open(str(crypto_file_path)+f".chunk.{i}", "rb") as f_chunk:
                     chunk = f_chunk.read()
-                    plain = pool.apply_async(rsa_decrypt_text, args=(chunk, private_key, num_threads, False, encoding, ))
+                    plain = pool.apply_async(rsa_decrypt_text, args=(chunk, private_key, key_length, num_threads, False, encoding, ))
                     plain_list.append(plain)
                 Path(str(crypto_file_path)+f".chunk.{i}").unlink()
             pool.close()
             pool.join()
         else:
             with open(crypto_file_path, 'rb') as f_chunk:
                 chunk = f_chunk.read()
-                plain_list = [rsa_decrypt_text(chunk, private_key, num_threads, False, encoding)]
+                plain_list = [rsa_decrypt_text(chunk, private_key, key_length, num_threads, False, encoding)]
         
         # save
         with open(plain_save_path, "wb") as f_save:
             for plain in plain_list:
                 if num_process > 1:
                     plain_text = plain.get()
                 else:
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/loading.py` & `mlcbase-1.2.0a1/src/mlcbase/image_io.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,189 +9,192 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-MuLingCloud base module: loading
-
-Support type: json, yaml, xml
+MuLingCloud base module: image io module
 
 Author: Weiming Chen
-Tester: Weiming Chen, Yuanshaung Sun
 """
-import json
+import base64
+import requests
+from io import BytesIO
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional, Union, Any
 
-import yaml
-import xmltodict
+import numpy as np
+import cv2
+import matplotlib.pyplot as plt
+from PIL import Image
 
 from .logger import Logger
 from .conifg import ConfigDict
-from .misc import is_dict, is_list, is_int
+from .misc import is_url, is_base64
 
 PathLikeType = Union[str, Path]
 
 
-def load_json(path: PathLikeType, logger: Optional[Logger] = None):
-    """load json file to a dict
-
-    Args:
-        path (PathLikeType)
+def get_image_from_url(url: str, 
+                       save_path: Optional[PathLikeType] = None,
+                       return_base64: bool = False,
+                       return_image: bool = False,
+                       backend: str = "cv2",
+                       logger: Optional[Logger] = None):
+    """get image from url
+
+    Args:
+        url (str)
+        save_path (Optional[str], optional): Defaults to None.
+        return_base64 (bool, optional): whether to return the image in base64 format. 
+                                        Defaults to False.
+        return_image (bool, optional): whether to return the image. Defaults to False.
+        backend (str, optional): backend of the image. Only used when return_image 
+                                 is True. Defaults to "cv2".
         logger (Optional[Logger], optional): Defaults to None.
 
-    Returns:
-        ConfigDict or None: return a ConfigDict if success, return None if fail
-    """
-    assert Path(path).exists(), 'json load error: the file is not exist'
-    assert Path(path).suffix == '.json', 'json load error: the suffix must be .json'
-
-    try:
-        with open(path, 'r') as f:
-            data = json.load(f)
-        return ConfigDict(data)
-    except OSError as e:
-        if logger is not None:
-            logger.error(f'json load error: {str(e)}')
-        return None
-    
-
-def save_json(data: Union[list, dict],
-              path: PathLikeType,
-              ensure_ascii: bool = True,
-              indent: Optional[int] = 4,
-              logger: Optional[Logger] = None,):
-    """save data to a json file
-
-    Args:
-        data (Union[List, Dict])
-        path (PathLikeType)
-        ensure_ascii (Optional[bool]): when ensure_ascii=False, allow non-ASCII characters in the file. 
-                                       Defaults to True.
-        indent (Optional[int]): spaces to use for indentation. Defaults to 4.
-        logger (Optional[Logger]): Defaults to None.
-
-    Returns:
-        bool: return True if success, return False if fail
-    """
-    assert is_dict(data) or is_list(data), 'json save error: the saving data must be "dict" or "list" type'
-    assert Path(path).suffix == '.json', 'json save error: the suffix must be .json'
-    if indent is not None:
-        assert is_int(indent), 'json save error: the indent must be "int" type'
-    
-    try:
-        with open(path, 'w') as f:
-            json.dump(data, f, ensure_ascii=ensure_ascii, indent=indent)
-        return True
-    except OSError as e:
-        if logger is not None:
-            logger.error(f'json save error: {str(e)}')
-        return False
-    
-
-def load_yaml(path: PathLikeType, logger: Optional[Logger] = None):
-    """load yaml file to a dict
-
-    Args:
-        path (PathLikeType)
-        logger (Optional[Logger], optional): Defaults to None.
+    Raises:
+        ValueError: if the url is invalid or get a error response from the url
 
     Returns:
-        ConfigDict or None: return a ConfigDict if success, return None if fail
+        dict: the image in the format of {"image": img, "base64": img_bs64}
     """
-    assert Path(path).exists(), 'yaml load error: the file is not exist'
-    assert Path(path).suffix == '.yaml', 'yaml load error: the suffix must be .yaml'
-
-    try:
-        with open(path, 'r') as f:
-            data = yaml.load(f, Loader=yaml.SafeLoader)
-        return ConfigDict(data)
-    except OSError as e:
+    if not is_url(url):
         if logger is not None:
-            logger.error(f'yaml load error: {str(e)}')
-        return None
+            logger.error(f"Invalid url: {url}")
+        raise ValueError(f"Invalid url: {url}")
+    assert backend in ["cv2", "pillow", "plt"], f"Invalid backend: {backend}"
     
-
-def save_yaml(data: dict, 
-              path: PathLikeType, 
-              allow_unicode: Optional[bool] = None,
-              logger: Optional[Logger] = None):
-    """save data to a yaml file
+    response = requests.get(url)
+    if response.status_code == 200:
+        img_bs64 = response.content
+
+        if save_path is not None:
+            with open(save_path, "wb") as f:
+                f.write(img_bs64)
+        
+        image_dict = ConfigDict()
+        if return_base64:
+            img = base64.b64encode(img_bs64)
+            image_dict.base64 = img
+
+        if return_image:
+            if backend == "cv2":
+                img = np.fromstring(img_bs64, np.uint8)
+                img = cv2.imdecode(img, cv2.IMREAD_UNCHANGED)
+                image_dict.image = img
+            
+            if backend == "pillow":
+                img = BytesIO(img_bs64)
+                img = Image.open(img)
+                image_dict.image = img
+
+            if backend == "plt":
+                img = np.fromstring(img_bs64, np.uint8)
+                img = cv2.imdecode(img, cv2.IMREAD_UNCHANGED)
+                if len(img.shape) == 3:
+                    if img.shape[2] == 3:
+                        img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+                    if img.shape[2] == 4:
+                        img = cv2.cvtColor(img, cv2.COLOR_BGRA2RGBA)
+                image_dict.image = img
+
+        return image_dict
+    else:
+        if logger is not None:
+            logger.error(f"Failed to get image from url: {url}")
+        raise ValueError(f"Failed to get image from url: {url}")
+
+
+def load_image(path: PathLikeType, 
+               backend: str = "cv2", 
+               logger: Optional[Logger] = None,
+               **kwargs):
+    """load an image
 
     Args:
-        data (dict)
-        path (PathLikeType)
-        allow_unicode (Optional[bool], optional): when allow_unicode=True, allow non-ASCII characters 
-                                                  in the file. Defaults to True.
+        path (str)
+        backend (str, optional): backend of the output image. Defaults to "cv2".
         logger (Optional[Logger], optional): Defaults to None.
 
-    Returns:
-        bool: return True if success, return False if fail
-    """
-    assert is_dict(data), 'yaml save error: the saving data must be "dict" type'
-    assert Path(path).suffix == '.yaml', 'yaml save error: the suffix must be .yaml'
-
-    try:
-        with open(path, 'w') as f:
-            yaml.dump(data, f, Dumper=yaml.SafeDumper, allow_unicode=allow_unicode)
-        return True
-    except OSError as e:
-        if logger is not None:
-            logger.error(f'yaml save error: {str(e)}')
-        return False
-
-
-def load_xml(path: PathLikeType, logger: Optional[Logger] = None):
-    """load xml file to a dict
-
-    Args:
-        path (PathLikeType)
-        logger (Optional[Logger], optional): Defaults to None.
+    Raises:
+        FileNotFoundError: if the path of the local image not exists
 
     Returns:
-        ConfigDict or None: return a dict if success, return None if fail
+        np.ndarray or PIL.Image or bytes: depends on the backend
     """
-    assert Path(path).exists(), 'xml load error: the file is not exist'
-    assert Path(path).suffix == '.xml', 'xml load error: the suffix must be .xml'
+    assert backend in ["cv2", "pillow", "plt", "base64"], f"Invalid backend: {backend}"
 
-    try:
-        with open(path, 'r') as f:
-            data = f.read()
-        data_orderedD = xmltodict.parse(data)
-        data_json = json.dumps(data_orderedD, indent=4)
-        data_dict = json.loads(data_json)
-        return ConfigDict(data_dict)
-    except OSError as e:
-        if logger is not None:
-            logger.error(f'xml load error: {str(e)}')
-        return None
+    if Path(path).exists():
+        is_local_path = True
+    else:
+        if not is_url(path):
+            if logger is not None:
+                logger.error(f"The URL {path} is not accessible.")
+            raise ConnectionError(f"The URL {path} is not accessible.")
+        is_local_path = False
     
-
-def save_xml(data: dict, 
-             path: PathLikeType, 
-             encoding: str = 'utf-8',
-             logger: Optional[Logger] = None,):
-    """save data to a xml file
-
-    Args:
-        data (dict)
-        path (PathLikeType)
-        encoding (str, optional): Defaults to 'utf-8'.
+    if is_local_path:
+        if backend == "cv2":
+            img = cv2.imread(path, kwargs.get("flags", cv2.IMREAD_UNCHANGED))
+        
+        if backend == "pillow":
+            img = Image.open(path, formats=kwargs.get("formats", None))
+
+        if backend == "plt":
+            img = plt.imread(path, format=kwargs.get("format", None))
+
+        if backend == "base64":
+            with open(path, "rb") as f:
+                img = base64.b64encode(f.read())
+    else:
+        if backend == "base64":
+            img = get_image_from_url(path, return_bs64=True, logger=logger).base64
+        else:
+            img = get_image_from_url(path, return_image=True, backend=backend, logger=logger).image
+
+    return img
+
+
+def save_image(img: Any, 
+               path: PathLikeType, 
+               backend: str = "cv2", 
+               logger: Optional[Logger] = None,
+               **kwargs):
+    """save an image to local device
+
+    Args:
+        img (Any)
+        path (str)
+        backend (str, optional): backend of the input image. Defaults to "cv2".
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
-        bool: return True if success, return False if fail
+        bool: return True if success, otherwise return False
     """
-    assert is_dict(data), 'xml save error: the saving data must be "dict" type'
-    assert Path(path).suffix == '.xml', 'xml save error: the suffix must be .xml'
-
+    assert backend in ["cv2", "pillow", "plt", "base64"], f"Invalid backend: {backend}"
+    
     try:
-        xml_data = xmltodict.unparse(data, pretty=True, encoding=encoding)
-        with open(path, 'w') as f:
-            f.write(xml_data)
+        if backend == "cv2":
+            cv2.imwrite(path, img)
+        
+        if backend == "pillow":
+            img.save(path, **kwargs)
+
+        if backend == "plt":
+            plt.imsave(path, img, **kwargs)
+        
+        if backend == "base64":
+            if not is_base64(img):
+                if logger is not None:
+                    logger.error("The input image is not in base64 format.")
+                raise TypeError("The input image is not in base64 format.")
+            
+            with open(path, "wb") as f:
+                img = base64.b64decode(img)
+                f.write(img)
         return True
     except OSError as e:
         if logger is not None:
-            logger.error(f'xml save error: {str(e)}')
+            logger.error(f"Failed to save image: {str(e)}")
         return False
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/logger.py` & `mlcbase-1.2.0a1/src/mlcbase/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,15 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 MuLingCloud base module: logger
 
-Repository: https://github.com/wmchen/pylog or https://gitee.com/wm-chen/pylog
+Repository: 
+- Github: https://github.com/wmchen/pylog
+- Gitee: https://gitee.com/wm-chen/pylog
 
 Author: Weiming Chen
 Tester: Weiming Chen, Yuanshaung Sun
 """
 import sys
 from datetime import datetime
 from pathlib import Path
@@ -129,83 +131,38 @@
             raise TypeError("only support 'str' and 'dict' type of format setting.")
         
     @staticmethod
     def get_now_time(timezone, timeformat):
         return datetime.now(tz=pytz.timezone(timezone)).strftime(timeformat)
 
     def get_elapsed(self, elapsedformat):
-        def format_time(e, format):
-            total_seconds = int((e.total_seconds() * 10**6 - e.microseconds) / 10**6)
-            smallest_scale = None
-
-            if "%d" in format:
-                days = (total_seconds - e.seconds) // 86400
-                smallest_scale = "%d"
-            else:
-                days = 0
-
-            if "%H" in format:
-                hours = (total_seconds-(days*86400)) // 3600
-                smallest_scale = "%H"
-            else:
-                hours = 0
-
-            if "%M" in format:
-                minutes = (total_seconds-(days*86400)-(hours*3600)) // 60
-                smallest_scale = "%M"
-            else:
-                minutes = 0
-                
-            if "%S" in format:
-                seconds = total_seconds - (days*86400) - (hours*3600) - (minutes*60)
-                smallest_scale = "%S"
-            else:
-                seconds = 0
-
-            if smallest_scale == "%d":
-                remain_second = total_seconds - (days*86400)
-                if remain_second > 0:
-                    days += remain_second / 86400
-            
-            if smallest_scale == "%H":
-                remain_second = total_seconds - (days*86400) - (hours*3600)
-                if remain_second > 0:
-                    fraction = str(remain_second / 3600)
-                    return str(days), f"{hours:02d}.{fraction[2:]}", f"{minutes:02d}", f"{seconds:02d}"
-            
-            if smallest_scale == "%M":
-                remain_second = total_seconds - (days*86400) - (hours*3600) - (minutes*60)
-                if remain_second > 0:
-                    fraction = str(remain_second / 60)
-                    return str(days), f"{hours:02d}", f"{minutes:02d}.{fraction[2:]}", f"{seconds:02d}"
-            
-            return str(days), f"{hours:02d}", f"{minutes:02d}", f"{seconds:02d}"
-
         elapsed = datetime.now() - self.start_time
-        days, hours, minutes, seconds = format_time(elapsed, elapsedformat)
+        days, hours, minutes, seconds, microsecond = self.__format_elapsed(elapsed, elapsedformat)
         
         elapsed_text = ""
         format_flag = False
         format_symbol = ""
         for ch in elapsedformat:
             if ch == "%":
                 format_flag = True
                 format_symbol += "%"
                 continue
 
             if format_flag:
                 format_symbol += ch
                 if format_symbol == "%d":
-                    elapsed_text += days
+                    elapsed_text += (days)
                 elif format_symbol == "%H":
                     elapsed_text += hours
                 elif format_symbol == "%M":
                     elapsed_text += minutes
                 elif format_symbol == "%S":
                     elapsed_text += seconds
+                elif format_symbol == "%f":
+                    elapsed_text += microsecond
                 else:
                     elapsed_text += format_symbol
                 format_symbol = ""
                 format_flag = False
             else:
                 elapsed_text += ch
                 
@@ -244,7 +201,82 @@
             self.logger.trace(msg)
 
     def set_quiet(self):
         self._quiet = True
 
     def set_activate(self):
         self._quiet = False
+
+    @staticmethod
+    def __format_elapsed(elapsed, timeformat):
+        if "%d" in timeformat:
+            has_day = True
+        else:
+            has_day = False
+
+        if "%H" in timeformat:
+            has_hour = True
+        else:
+            has_hour = False
+
+        if "%M" in timeformat:
+            has_minute = True
+        else:
+            has_minute = False
+        
+        if "%S" in timeformat:
+            has_second = True
+        else:
+            has_second = False
+
+        if "%f" in timeformat:
+            has_microsecond = True
+        else:
+            has_microsecond = False
+
+        delta_days = elapsed.days
+        delta_seconds = elapsed.seconds
+        microseconds = elapsed.microseconds
+        hours = delta_seconds // 3600
+        minute = (delta_seconds % 3600) // 60
+        seconds = delta_seconds % 60
+        show_day = 0
+        show_hour = 0
+        show_minute = 0
+        show_second = 0
+        show_microsecond = 0
+
+        # if %d not in timeformat, unsqueeze days to hours
+        if has_day:
+            show_day = delta_days
+        else:
+            hours += delta_days * 24
+
+        # if %H not in timeformat, unsqueeze hours to minutes
+        if has_hour:
+            show_hour = hours
+        else:
+            minute += hours * 60
+
+        # if %M not in timeformat, unsqueeze minutes to seconds
+        if has_minute:
+            show_minute = minute
+        else:
+            seconds += minute * 60
+
+        # if %S not in timeformat, unsqueeze seconds to microseconds
+        if has_second:
+            show_second = seconds
+        else:
+            microseconds += seconds * 10**6
+
+        # ignore microsecond when %f not exists in timeformat
+        if has_microsecond:
+            show_microsecond = microseconds
+
+        show_day = str(show_day)
+        show_hour = f"{show_hour:02d}"
+        show_minute = f"{show_minute:02d}"
+        show_second = f"{show_second:02d}"
+        show_microsecond = str(show_microsecond)
+
+        return show_day, show_hour, show_minute, show_second, show_microsecond
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/remote_connect.py` & `mlcbase-1.2.0a1/src/mlcbase/remote_connect.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,29 +11,32 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 MuLingCloud base module: remote connect
 
+Supported OS:
+- Linux
+- Windows
+
+TODO: support MacOS
+
 Author: Weiming Chen
 Tester: Weiming Chen, Yuanshaung Sun
-
-TODO:
-- support multiprocessing for SFTP uploading
 """
 import os
 from pathlib import Path
 from datetime import datetime
 from typing import Optional, Union, Callable
 
 import paramiko
 
 from .logger import Logger
-from .file import listdir, mkdir
+from .file import listdir, create
 from .misc import PlatformNotSupportError
 
 PathLikeType = Union[str, Path]
 
 
 class SSH:
     def __init__(self,
@@ -161,23 +164,23 @@
             self.logger.success('sftp connected to remote server.')
             return (sftp_client, ssh_client)
         except paramiko.SSHException as e:
             self.logger.error(f"sftp connect error: {str(e)}")
             return None
 
     def upload_file(self, 
-                    local_path: str,
-                    remote_path: str,
+                    local_path: PathLikeType,
+                    remote_path: PathLikeType,
                     remote_platform: str,
                     callback: Optional[Callable] = None):
         """upload a file to remote server
 
         Args:
-            local_path (str)
-            remote_path (str)
+            local_path (PathLikeType)
+            remote_path (PathLikeType)
             remote_platform (str)
             callback (Optional[Callable], optional): callback function. Defaults to None.
 
         Returns:
             bool: return True if success, otherwise return False
         """
         if self.__client is None:
@@ -204,23 +207,23 @@
             self.logger.success(f'file uploaded')
             return True
         except paramiko.SFTPError as e:
             self.logger.error(f"sftp upload file error: {str(e)}")
             return False
         
     def download_file(self,
-                      remote_path: str,
-                      local_path: str,
+                      remote_path: PathLikeType,
+                      local_path: PathLikeType,
                       remote_platform: str,
                       callback: Optional[Callable] = None):
         """download a file from remote server
 
         Args:
-            remote_path (str)
-            local_path (str)
+            remote_path (PathLikeType)
+            local_path (PathLikeType)
             remote_platform (str)
             callback (Optional[Callable], optional): callback function. Defaults to None.
 
         Returns:
             bool: return True if success, otherwise return False
         """
         if self.__client is None:
@@ -247,23 +250,23 @@
             self.logger.success(f'file downloaded')
             return True
         except paramiko.SFTPError as e:
             self.logger.error(f"sftp download file error: {str(e)}")
             return False
         
     def upload_dir(self,
-                   local_path: str,
-                   remote_path: str,
+                   local_path: PathLikeType,
+                   remote_path: PathLikeType,
                    remote_platform: str,
                    callback: Optional[Callable] = None):
         """upload a directory to remote server
 
         Args:
-            local_path (str)
-            remote_path (str)
+            local_path (PathLikeType)
+            remote_path (PathLikeType)
             remote_platform (str)
             callback (Optional[Callable], optional): callback function. Defaults to None.
 
         Returns:
             bool: return True if success, otherwise return False
         """
         if self.__client is None:
@@ -306,23 +309,23 @@
             self.logger.success(f'directory uploaded')
             return True
         except paramiko.SFTPError as e:
             self.logger.error(f"sftp upload directory error: {str(e)}")
             return False
         
     def download_dir(self,
-                     remote_path: str,
-                     local_path: str,
+                     remote_path: PathLikeType,
+                     local_path: PathLikeType,
                      remote_platform: str,
                      callback: Optional[Callable] = None):
         """download a directory from remote server
 
         Args:
-            remote_path (str)
-            local_path (str)
+            remote_path (PathLikeType)
+            local_path (PathLikeType)
             remote_platform (str)
             callback (Optional[Callable], optional): callback function. Defaults to None.
 
         Returns:
             bool: return True if success, otherwise return False
         """
         if self.__client is None:
@@ -341,15 +344,15 @@
         
         if not self.remote_is_dir(remote_path, remote_platform):
             self.logger.error('remote path is not a directory')
             return False
         
         self.logger.info(f'downloading directory: [REMOTE] {remote_path} -> [LOCAL] {local_path}')
         try:
-            if not mkdir(local_path, logger=self.logger):
+            if not create(local_path, ftype="dir", logger=self.logger):
                 self.logger.error(f'failed to create local directory: {local_path}')
                 return False
             
             remote_files = self.remote_listdir(remote_path, remote_platform, return_path=False)
             for f in remote_files:
                 remote_subfile_path = os.path.join(remote_path, f)
                 local_subfile_path = os.path.join(local_path, f)
@@ -366,19 +369,21 @@
             
             self.logger.success(f'directory downloaded')
             return True
         except paramiko.SFTPError as e:
             self.logger.error(f"sftp download directory error: {str(e)}")
             return False
         
-    def remote_exists(self, remote_path: str, remote_platform: str):
+    def remote_exists(self, 
+                      remote_path: PathLikeType, 
+                      remote_platform: str):
         """check if remote path exists
 
         Args:
-            remote_path (str)
+            remote_path (PathLikeType)
             remote_platform (str)
 
         Raises:
             paramiko.SFTPError: when sftp connection is not established
             PlatformNotSupportError: when remote platform is not supported
 
         Returns:
@@ -396,19 +401,21 @@
         
         try:
             self.__client[0].stat(remote_path)
             return True
         except:
             return False
         
-    def remote_is_file(self, remote_path: str, remote_platform: str):
+    def remote_is_file(self, 
+                       remote_path: PathLikeType, 
+                       remote_platform: str):
         """check if remote path is a file
 
         Args:
-            remote_path (str)
+            remote_path (PathLikeType)
             remote_platform (str)
 
         Raises:
             paramiko.SFTPError: when sftp connection is not established
             PlatformNotSupportError: when remote platform is not supported
 
         Returns:
@@ -427,19 +434,21 @@
         try:
             self.__client[0].listdir(remote_path)
             return False
         except:
             return True
         
         
-    def remote_is_dir(self, remote_path: str, remote_platform: str):
+    def remote_is_dir(self, 
+                      remote_path: PathLikeType, 
+                      remote_platform: str):
         """check if remote path is a directory
 
         Args:
-            remote_path (str)
+            remote_path (PathLikeType)
             remote_platform (str)
 
         Raises:
             paramiko.SFTPError: when sftp connection is not established
             PlatformNotSupportError: when remote platform is not supported
 
         Returns:
@@ -458,21 +467,21 @@
         try:
             self.__client[0].listdir(remote_path)
             return True
         except:
             return False
         
     def remote_mkdir(self, 
-                     remote_path: str, 
+                     remote_path: PathLikeType, 
                      remote_platform: str,
                      exist_ok: bool = True):
         """make a remote directory
 
         Args:
-            remote_path (str)
+            remote_path (PathLikeType)
             remote_platform (str)
             exist_ok (bool, optional): if True, the directory will not be created if 
                                        it already exists. Defaults to True.
 
         Raises:
             paramiko.SFTPError: when sftp connection is not established
             PlatformNotSupportError: when remote platform is not supported
@@ -512,21 +521,21 @@
         
         if status:
             self.logger.success(f'directory created')
         
         return status
     
     def remote_listdir(self,
-                       remote_path: str, 
+                       remote_path: PathLikeType, 
                        remote_platform: str,
                        return_path: bool = True):
         """list remote directory
 
         Args:
-            remote_path (str)
+            remote_path (PathLikeType)
             remote_platform (str)
             return_path (bool, optional): return the path of the remote file if True, 
                                           otherwise return the name of the remote file. 
                                           Defaults to True.
 
         Raises:
             paramiko.SFTPError: when sftp connection is not established
@@ -562,15 +571,14 @@
         
     @staticmethod
     def __format_path(path: str, platform: str):
         if platform == 'windows':
             path = path.replace('/', '\\')
         if platform == 'linux':
             path = path.replace('\\', '/')
-        # TODO: support MacOS
         return path
 
     def _set_logger(self, logger: Optional[Logger], quiet: bool):
         if logger is None:
             now_time = datetime.now().strftime('%Y%m%d-%H%M%S')
             logger = Logger()
             if self.work_dir is not None:
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase/timer.py` & `mlcbase-1.2.0a1/src/mlcbase/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 
     if name is None:
         _register_modules = {}
     else:
         assert name in _register_modules.keys(), f"module {name} is not registered"
         del _register_modules[name]
 
+def show_register_modules():
+    return list(_register_modules.keys())
+
 
 def runtime_analysis(start_time: datetime = None, 
                      end_time: datetime = None, 
                      unit: str = "ms"):
     """analysis runtime
 
     Args:
@@ -87,15 +90,14 @@
     for name, vaule in _register_modules.items():
         if vaule['elapsed'] == 0:
             continue
         module_list.append(dict(name=name, elapsed=vaule['elapsed'], calls=vaule['calls']))
     module_list.sort(key=lambda x: x['elapsed'], reverse=True)
 
     unit = unit.lower()
-    print(20*'-'+' Module Runtime Analysis '+20*'-')
     if start_time is not None or end_time is not None:
         total_runtime = int((end_time - start_time).total_seconds() * 10**6)
         if unit == "h":
             print_total_runtime = total_runtime / 10**6 / 3600
         elif unit == "min":
             print_total_runtime = total_runtime / 10**6 / 60
         elif unit == "s":
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase.egg-info/PKG-INFO` & `mlcbase-1.2.0a1/src/mlcbase.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: mlcbase
-Version: 1.1.0rc1
+Version: 1.2.0a1
 Summary: The base module of all MuLingCloud modules and applications.
-Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>, Zilin Yang <876497115@qq.com>
+Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
            1. Definitions.
@@ -214,35 +214,34 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
 Requires-Dist: loguru
 Requires-Dist: pytz
 Requires-Dist: prettytable
 Requires-Dist: pyyaml
-Requires-Dist: xmltodict
 Requires-Dist: rsa
 Requires-Dist: pycryptodome
+Requires-Dist: requests
 Requires-Dist: paramiko
 Requires-Dist: PyMySQL
-Requires-Dist: hvac
+Requires-Dist: pyotp
+Requires-Dist: qrcode[pil]
+Requires-Dist: opencv-python
+Requires-Dist: matplotlib
 
 <div align="center">
     <img src="https://lychee.weimingchen.net:1130/uploads/original/dc/0e/eae6786c5d68d4a564f8e3f60157.png" width="100%" />
 </div>
 
 <div align="center">
-    <a href="https://pypi.org/project/mlcbase">
-        <img src="https://img.shields.io/pypi/v/mlcbase" />
-    </a>
-    <a href="./LICENSE">
-        <img src="https://img.shields.io/github/license/wmchen/mlcbase.svg" />
-    </a>
-    <a href="https://weimingchen.net">
-        <img src="https://img.shields.io/badge/author-Weiming_Chen-royalblue" />
-    </a>
+
+[![PyPI](https://img.shields.io/pypi/v/mlcbase)](https://pypi.org/project/mlcbase/)
+[![License](https://img.shields.io/github/license/wmchen/mlcbase.svg)](https://www.apache.org/licenses/LICENSE-2.0)
+[![All Contributors](https://img.shields.io/github/all-contributors/wmchen/mlcbase?color=blue)](#contributors)
+
 </div>
 
 ## Introduction
 
 Welcome to use MuLingCloud. We aim to let everything easier.
 
 MLCBase is an open source Python library for multiple uses. It is the base module of all MuLingCloud modules and applications.
@@ -250,55 +249,59 @@
 Supported platforms:
 
 - 😄 Windows (Python 3.6+)
 - 😄 Linux (Python 3.7+)
 - MacOS (untested, maybe. I don't have a MacOS machine😫. Anyone can help me?)
 
 <details open>
-<summary>Features</summary>
-
-- **Version**
-
-    We define a `Version` class to manage the version of all MuLingCloud modules or applications. The instantiated versions can easily compare their order by using comparision operators, i.e. `==`, `!=`, `<`, `<=`, `>`, `>=`.
+<summary>Features (v1.2.0a1)</summary>
 
 - **Config Dictionary**
 
     We define a `ConfigDict` for more convenience usage. It is a type of dictionary inherited from `dict`. It has all the features of `dict` while including other more convenient features.
 
-- **Logger**
+- $\color{blue}{\textbf{update }}$ **Logger**
 
     We build a `Logger` for more convenience logging management. Actually, this is a slightly improvement based on [loguru](https://github.com/Delgan/loguru). Refer to [pylog](https://github.com/wmchen/pylog) for more information.
 
-- **Runtime Analysis**
+- $\color{blue}{\textbf{update }}$ **Runtime Analysis**
 
     We offer a simple way to evaluate functions in the Python project. All you need is to wrap the target function by a decorator.
 
-- **File Operations**
+- $\color{blue}{\textbf{update }}$ **File Operations**
+
+    We offer various features to make file operations easier. Besides, we offer a simple way to load and save JSON, YAML, and XML files.
+
+- $\color{red}{\textbf{new }}$ **Image IO**
+
+    We offer a simple way to load and save images.
+
+- $\color{red}{\textbf{new }}$ **One-Time Password**
 
-    We offer various features to make file operations easier.
+    We support two methods for OTP: Time-based One-Time Password (TOTP) and HMAC-based One-Time Password (HOTP).
 
-- **Encryption and Decryption**
+- $\color{blue}{\textbf{update }}$ **Encryption and Decryption**
 
     We offer various methods to encrypt and decrypt or verify text, files and passwords including RSA, AES and Hash.
 
-- **Database**
+- $\color{blue}{\textbf{update }}$ **Database**
 
-    We offer a simple way to operate the database including creating a data table, inserting data, deleting data, searching data, and updating data. Currently only supports MySQL backend, but other backends will be supported in the future.
+    We offer a simple way to operate the database. Supported database backend: MySQL, SQLite.
 
 - **Remote Connection**
 
     We support SSH and SFTP for remote connection.
 
-- **Email**
+- $\color{blue}{\textbf{update }}$ **Email**
 
     We offer a simple API to send email. Currently only supports SMTP (with SSL) server.
 
-- **HashiCorp Vault**
+- $\color{red}{\textbf{BREAKING CHANGE }}$ **HashiCorp Vault**
 
-    We offer a simple API to get secrets from [HashiCorp/Vault](https://developer.hashicorp.com/vault). Currently only supports the secret engine of `kv2`, but other type of secret engines will be supported in the future.
+    We offer several APIs to operate [HashiCorp/Vault](https://developer.hashicorp.com/vault) through HTTP requests. Supported authorization methods: token, username & password. Supported secret engines: KV v1, KV v2, TOTP, Transit.
 
 </details>
 
 ## Installation
 
 ```bash
 pip install mlcbase
@@ -312,10 +315,36 @@
 
 See all changes in [CHANGELOG](./CHANGELOG.md).
 
 ## Contributors
 
 We appreciate all the contributors who add new features or fix bugs, as well as the users who offer valuable feedback.
 
+We welcome all contributors, feel free to create an issue or file a pull request and join us! ❤️
+
+<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
+<!-- prettier-ignore-start -->
+<!-- markdownlint-disable -->
+<table>
+  <tbody>
+    <tr>
+      <td align="center" valign="top" width="14.28%"><a href="https://weimingchen.net/"><img src="https://avatars.githubusercontent.com/u/33000375?v=4?s=100" width="100px;" alt="Weiming Chen"/><br /><sub><b>Weiming Chen</b></sub></a><br /><a href="https://github.com/wmchen/mlcbase/commits?author=wmchen" title="Code">💻</a> <a href="#ideas-wmchen" title="Ideas, Planning, & Feedback">🤔</a> <a href="#projectManagement-wmchen" title="Project Management">📆</a> <a href="https://github.com/wmchen/mlcbase/commits?author=wmchen" title="Tests">⚠️</a> <a href="#tutorial-wmchen" title="Tutorials">✅</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://www.mulingcloud.com/author/yuanshuang-sun/"><img src="https://avatars.githubusercontent.com/u/32105419?v=4?s=100" width="100px;" alt="Yuanshuang Sun"/><br /><sub><b>Yuanshuang Sun</b></sub></a><br /><a href="#ideas-dcsasori" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/wmchen/mlcbase/commits?author=dcsasori" title="Tests">⚠️</a> <a href="#tutorial-dcsasori" title="Tutorials">✅</a></td>
+    </tr>
+  </tbody>
+</table>
+
+<!-- markdownlint-restore -->
+<!-- prettier-ignore-end -->
+
+<!-- ALL-CONTRIBUTORS-LIST:END -->
+
+
 ## License
 
-This project is released under the [Apache 2.0 license](./LICENSE).
+This project is released under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0).
+
+## Repository
+
+- Github Repository: https://github.com/wmchen/mlcbase
+- GitLab Repository: https://gitlab.com/wm-chen/mlcbase
+- Gitee Repository: https://gitee.com/wm-chen/mlcbase
```

### Comparing `mlcbase-1.1.0rc1/src/mlcbase.egg-info/SOURCES.txt` & `mlcbase-1.2.0a1/src/mlcbase.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/mlcbase/__init__.py
 src/mlcbase/conifg.py
 src/mlcbase/database.py
 src/mlcbase/email.py
 src/mlcbase/encrypt_password.py
 src/mlcbase/entrypt_aes.py
 src/mlcbase/entrypt_rsa.py
 src/mlcbase/file.py
+src/mlcbase/image_io.py
 src/mlcbase/loading.py
 src/mlcbase/logger.py
 src/mlcbase/misc.py
+src/mlcbase/otp.py
 src/mlcbase/remote_connect.py
 src/mlcbase/timer.py
 src/mlcbase/vault.py
-src/mlcbase/version.py
 src/mlcbase.egg-info/PKG-INFO
 src/mlcbase.egg-info/SOURCES.txt
 src/mlcbase.egg-info/dependency_links.txt
 src/mlcbase.egg-info/requires.txt
 src/mlcbase.egg-info/top_level.txt
```

