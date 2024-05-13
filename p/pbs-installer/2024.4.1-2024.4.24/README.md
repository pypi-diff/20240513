# Comparing `tmp/pbs_installer-2024.4.1.tar.gz` & `tmp/pbs_installer-2024.4.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbs_installer-2024.4.1.tar", last modified: Mon Apr  1 02:46:11 2024, max compression
+gzip compressed data, was "pbs_installer-2024.4.24.tar", last modified: Mon May 13 09:36:53 2024, max compression
```

## Comparing `pbs_installer-2024.4.1.tar` & `pbs_installer-2024.4.24.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1059 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/LICENSE
--rw-r--r--   0        0        0      391 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/README.md
--rw-r--r--   0        0        0     1022 2024-04-01 02:46:11.161678 pbs_installer-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0      243 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/src/pbs_installer/__init__.py
--rw-r--r--   0        0        0     2877 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/src/pbs_installer/__main__.py
--rw-r--r--   0        0        0     6754 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/src/pbs_installer/_install.py
--rw-r--r--   0        0        0     3473 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/src/pbs_installer/_utils.py
--rw-r--r--   0        0        0   198713 2024-04-01 02:46:03.221740 pbs_installer-2024.4.1/src/pbs_installer/_versions.py
--rw-r--r--   0        0        0        0 2024-04-01 02:46:03.225740 pbs_installer-2024.4.1/tests/__init__.py
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 pbs_installer-2024.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-07-13 11:33:35.913905 pbs_installer-2024.4.24/LICENSE
+-rw-r--r--   0        0        0      391 2024-03-22 02:31:41.423897 pbs_installer-2024.4.24/README.md
+-rw-r--r--   0        0        0     1129 2024-05-13 09:36:53.984359 pbs_installer-2024.4.24/pyproject.toml
+-rw-r--r--   0        0        0      243 2024-03-22 01:49:50.221948 pbs_installer-2024.4.24/src/pbs_installer/__init__.py
+-rw-r--r--   0        0        0     2893 2024-05-13 09:36:41.819543 pbs_installer-2024.4.24/src/pbs_installer/__main__.py
+-rw-r--r--   0        0        0     6916 2024-05-13 09:36:41.820251 pbs_installer-2024.4.24/src/pbs_installer/_install.py
+-rw-r--r--   0        0        0     3473 2024-04-01 02:39:38.324322 pbs_installer-2024.4.24/src/pbs_installer/_utils.py
+-rw-r--r--   0        0        0   219162 2024-05-13 09:36:41.821659 pbs_installer-2024.4.24/src/pbs_installer/_versions.py
+-rw-r--r--   0        0        0        0 2024-05-13 09:36:41.821790 pbs_installer-2024.4.24/src/pbs_installer/py.typed
+-rw-r--r--   0        0        0        0 2023-07-13 08:54:47.350150 pbs_installer-2024.4.24/tests/__init__.py
+-rw-r--r--   0        0        0      990 1970-01-01 00:00:00.000000 pbs_installer-2024.4.24/PKG-INFO
```

### Comparing `pbs_installer-2024.4.1/LICENSE` & `pbs_installer-2024.4.24/LICENSE`

 * *Files identical despite different names*

### Comparing `pbs_installer-2024.4.1/pyproject.toml` & `pbs_installer-2024.4.24/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Installer for Python Build Standalone"
 authors = [
     { name = "Frost Ming", email = "me@frostming.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "2024.4.1"
+version = "2024.4.24"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/frostming/pbs-installer"
 Documentation = "http://pbs-installer.readthedocs.io"
@@ -44,16 +44,27 @@
 
 [tool.pdm.dev-dependencies]
 doc = [
     "mkdocs>=1.5.3",
     "mkdocs-material>=9.5.14",
     "mkdocstrings[python]>=0.24",
 ]
+dev = [
+    "mypy>=1.9.0",
+]
 
 [tool.ruff]
 line-length = 100
 target-version = "py310"
 
 [tool.ruff.lint]
 extend-select = [
     "I",
 ]
+
+[tool.mypy]
+strict = true
+files = [
+    "src",
+    "tests",
+]
+pretty = true
```

### Comparing `pbs_installer-2024.4.1/src/pbs_installer/__main__.py` & `pbs_installer-2024.4.24/src/pbs_installer/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from collections.abc import Sequence
 from typing import Any
 
 from ._install import install
 from ._utils import get_available_arch_platforms
 
 
-def _setup_logger(verbose: bool):
+def _setup_logger(verbose: bool) -> None:
     logger = logging.getLogger("pbs_installer")
     handler = logging.StreamHandler()
     handler.setFormatter(logging.Formatter("%(levelname)s: %(message)s"))
     logger.addHandler(handler)
     logger.setLevel(logging.DEBUG if verbose else logging.WARNING)
 
 
@@ -42,15 +42,15 @@
     def list_versions(self) -> None:
         from ._versions import PYTHON_VERSIONS
 
         for version in PYTHON_VERSIONS:
             print(f"- {version}")
 
 
-def main():
+def main() -> None:
     archs, platforms = get_available_arch_platforms()
     parser = ArgumentParser("pbs-install", description="Installer for Python Build Standalone")
     install_group = parser.add_argument_group("Install Arguments")
     install_group.add_argument(
         "version", help="The version of Python to install, e.g. 3.8, 3.10.4, pypy@3.10"
     )
     install_group.add_argument(
```

### Comparing `pbs_installer-2024.4.1/src/pbs_installer/_install.py` & `pbs_installer-2024.4.24/src/pbs_installer/_install.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from __future__ import annotations
 
 import hashlib
 import logging
 import os
 import tempfile
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import TYPE_CHECKING, Optional, Tuple, cast
 from urllib.parse import unquote
 
 from ._utils import PythonVersion, get_arch_platform
 
 if TYPE_CHECKING:
     import httpx
     from _typeshed import StrPath
 
+    from typing import Literal
+
+    PythonImplementation = Literal["cpython", "pypy"]
+
 logger = logging.getLogger(__name__)
 THIS_ARCH, THIS_PLATFORM = get_arch_platform()
 PythonFile = Tuple[str, Optional[str]]
 
 
 def _get_headers() -> dict[str, str] | None:
     TOKEN = os.getenv("GITHUB_TOKEN")
@@ -28,15 +32,15 @@
     }
 
 
 def get_download_link(
     request: str,
     arch: str = THIS_ARCH,
     platform: str = THIS_PLATFORM,
-    implementation: str = "cpython",
+    implementation: PythonImplementation = "cpython",
     build_dir: bool = False,
 ) -> tuple[PythonVersion, PythonFile]:
     """Get the download URL matching the given requested version.
 
     Parameters:
         request: The version of Python to install, e.g. 3.8,3.10.4
         arch: The architecture to install, e.g. x86_64, arm64
@@ -136,14 +140,15 @@
         original_filename = str(filename)
     logger.debug(
         "Extracting file %s to %s with original filename %s",
         filename,
         destination,
         original_filename,
     )
+    filename = cast(str, filename)
     if original_filename.endswith(".zst"):
         unpack_zst(filename, destination)
     elif original_filename.endswith(".zip"):
         unpack_zip(filename, destination)
     else:
         unpack_tar(filename, destination)
 
@@ -151,15 +156,15 @@
 def install(
     request: str,
     destination: StrPath,
     version_dir: bool = False,
     client: httpx.Client | None = None,
     arch: str | None = None,
     platform: str | None = None,
-    implementation: str = "cpython",
+    implementation: PythonImplementation = "cpython",
     build_dir: bool = False,
 ) -> None:
     """Download and install the requested python version.
 
     Note: Extras required
         `pbs-installer[all]` must be installed to use this function.
```

### Comparing `pbs_installer-2024.4.1/src/pbs_installer/_utils.py` & `pbs_installer-2024.4.24/src/pbs_installer/_utils.py`

 * *Files identical despite different names*

### Comparing `pbs_installer-2024.4.1/src/pbs_installer/_versions.py` & `pbs_installer-2024.4.24/src/pbs_installer/_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,62 @@
 # @Generated by find_versions.py. DO NOT EDIT.
 from __future__ import annotations
 from ._utils import PythonVersion
 
-PYTHON_VERSIONS: dict[PythonVersion, dict[tuple[str, str], tuple[str, str | None]]] = {
+PYTHON_VERSIONS: dict[PythonVersion, dict[tuple[str, str, bool], tuple[str, str | None]]] = {
+    PythonVersion("cpython", 3, 12, 3): {
+        ("macos", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "fa2b8c377f17dfb097a93c0fba217d93075a7ceba0cc877066e95be969e6b73d",
+        ),
+        ("macos", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-aarch64-apple-darwin-install_only.tar.gz",
+            "ccc40e5af329ef2af81350db2a88bbd6c17b56676e82d62048c15d548401519e",
+        ),
+        ("linux", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-aarch64-unknown-linux-gnu-lto-full.tar.zst",
+            "a4f17d1e3b4ea0e4c2a3664f232c0857979522936af582f7de92b57050220f74",
+        ),
+        ("linux", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-aarch64-unknown-linux-gnu-install_only.tar.gz",
+            "ec8126de97945e629cca9aedc80a29c4ae2992c9d69f2655e27ae73906ba187d",
+        ),
+        ("windows", "x86", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-i686-pc-windows-msvc-install_only.tar.gz",
+            "bd723ad1aa05551627715a428660250f0e74db0f1421b03f399235772057ef55",
+        ),
+        ("windows", "x86", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-i686-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "31bb3f579f3dcbbf3bf1dc71a188112e821cdfc77d21c9dbfe82ea78538110e1",
+        ),
+        ("macos", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "e49da3f702da08a3e38d01c776cc2356e427217681964ff64a7880507e224a3c",
+        ),
+        ("macos", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-apple-darwin-install_only.tar.gz",
+            "c37a22fca8f57d4471e3708de6d13097668c5f160067f264bb2b18f524c890c8",
+        ),
+        ("windows", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-pc-windows-msvc-install_only.tar.gz",
+            "f7cfa4ad072feb4578c8afca5ba9a54ad591d665a441dd0d63aa366edbe19279",
+        ),
+        ("windows", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "776568c92c5f3b47dbf5f17c1c58578f70d75a32654419a158aa8bdc6f95b09a",
+        ),
+        ("linux", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-unknown-linux-gnu-pgo%2Blto-full.tar.zst",
+            "e51f6676a24c3551657347ef97963164eac801df0a62afcba8e0e28ebb62acee",
+        ),
+        ("linux", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.12.3%2B20240415-x86_64-unknown-linux-gnu-install_only.tar.gz",
+            "a73ba777b5d55ca89edef709e6b8521e3f3d4289581f174c8699adfb608d09d6",
+        ),
+    },
     PythonVersion("cpython", 3, 12, 2): {
         ("macos", "aarch64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.12.2%2B20240224-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
             "2afcc8b25c55793f6ceb0bef2e547e101f53c9e25a0fe0332320e5381a1f0fdb",
         ),
         ("macos", "aarch64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.12.2%2B20240224-aarch64-apple-darwin-install_only.tar.gz",
@@ -149,14 +199,64 @@
             "5ce861907a2751a3a7395b1aaada830c2b072acc03f3dd0bcbaaa2b7a9166fc0",
         ),
         ("linux", "x86_64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20231002/cpython-3.12.0%2B20231002-x86_64-unknown-linux-gnu-install_only.tar.gz",
             "e51a5293f214053ddb4645b2c9f84542e2ef86870b8655704367bd4b29d39fe9",
         ),
     },
+    PythonVersion("cpython", 3, 11, 9): {
+        ("macos", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "9a59eb9e8e509e742a25cada7b2c1123a56022081d91a8fbe48015cf495b0d0f",
+        ),
+        ("macos", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-aarch64-apple-darwin-install_only.tar.gz",
+            "7af7058f7c268b4d87ed7e08c2c7844ef8460863b3e679db3afdce8bb1eedfae",
+        ),
+        ("linux", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-aarch64-unknown-linux-gnu-lto-full.tar.zst",
+            "c9f5e493c686ed8a5c38d1748c45fed18dc9b6faa70794d9cc9bb32489cc0b77",
+        ),
+        ("linux", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-aarch64-unknown-linux-gnu-install_only.tar.gz",
+            "b3a7199ac2615d75fb906e5ba556432efcf24baf8651fc70370d9f052d4069ee",
+        ),
+        ("windows", "x86", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-i686-pc-windows-msvc-install_only.tar.gz",
+            "b121267975dc2abfbdfcd60c55df2dcc2fb8e321ac07ae1a29f877cc111d3963",
+        ),
+        ("windows", "x86", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-i686-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "f0405bb7e19e4dbf7db290c224fc4aa333d3e16e0ed571f0794becac620fa26a",
+        ),
+        ("macos", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "b1b156ceed6bc53c3c8816b3b5c3983d2c7070a8a42558b9c6dd730faec164e2",
+        ),
+        ("macos", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-apple-darwin-install_only.tar.gz",
+            "9afd734f63a23783cf0257bef25c9231ffc80e7747486dc54cf72f325213fd15",
+        ),
+        ("windows", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-pc-windows-msvc-install_only.tar.gz",
+            "368474c69f476e7de4adaf50b61d9fcf6ec8b4db88cc43c5f71c860b3cd29c69",
+        ),
+        ("windows", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "25344b08303f72ba2a37c33aa240fbd2c8d5a41bcce79cff63923b3d778c645c",
+        ),
+        ("linux", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-unknown-linux-gnu-pgo%2Blto-full.tar.zst",
+            "1c5038da28a4379c065db85116594524010f30e653307c53bb9694e4e710d2c7",
+        ),
+        ("linux", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.11.9%2B20240415-x86_64-unknown-linux-gnu-install_only.tar.gz",
+            "78b1c16a9fd032997ba92a60f46a64f795cd18ff335659dfdf6096df277b24d5",
+        ),
+    },
     PythonVersion("cpython", 3, 11, 8): {
         ("macos", "aarch64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.11.8%2B20240224-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
             "c0650884b929253b8688797d1955850f6e339bf0428b3d935f62ab3159f66362",
         ),
         ("macos", "aarch64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.11.8%2B20240224-aarch64-apple-darwin-install_only.tar.gz",
@@ -531,14 +631,64 @@
             "02332441cb610b1e1aa2d2972e261e2910cc6a950b7973cac22c0759a93c5fcd",
         ),
         ("linux", "x86_64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20230116/cpython-3.11.1%2B20230116-x86_64-unknown-linux-gnu-install_only.tar.gz",
             "02a551fefab3750effd0e156c25446547c238688a32fabde2995c941c03a6423",
         ),
     },
+    PythonVersion("cpython", 3, 10, 14): {
+        ("macos", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "fa95c3a18e29234cf10c0befa2f08246307cab7f473ccc1804845be3caab076d",
+        ),
+        ("macos", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-aarch64-apple-darwin-install_only.tar.gz",
+            "389da793b7666e9310908b4fe3ddcf0a20b55727fcb384c7c49b01bb21716f89",
+        ),
+        ("linux", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-aarch64-unknown-linux-gnu-lto-full.tar.zst",
+            "630bbbba148557bf670fbd65eb7fcd3c212cac45387d135c02799a13967d0f3d",
+        ),
+        ("linux", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-aarch64-unknown-linux-gnu-install_only.tar.gz",
+            "2f9f26c430df19d6d2a25ac3f2a8e74106d32b9951b85f95218ceeb13d52e952",
+        ),
+        ("windows", "x86", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-i686-pc-windows-msvc-install_only.tar.gz",
+            "a71c6b00c167012d23c05ecba22222a560c0191ad21b46f32d89895037dad973",
+        ),
+        ("windows", "x86", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-i686-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "4fafd723944ae98611005caf0ad7dbb262e02c61ddfa7c45f0d097f0965839a8",
+        ),
+        ("macos", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "cc3fa88159a50d639dff84af9ffe2a50d6eda41b51037c755b5a13b88ce50153",
+        ),
+        ("macos", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-apple-darwin-install_only.tar.gz",
+            "8e27ec6f27b3a27be892c7a9db1e278c858acd9d90c1114013fe5587cd6fc5e6",
+        ),
+        ("windows", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-pc-windows-msvc-install_only.tar.gz",
+            "186b5632fb2fa5b5e6eee4110ce9bbb0349f52bb2163d2a1f5188b1d8eb1b5f3",
+        ),
+        ("windows", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "abc3041f0de7e700229c0628dfcba7ba1d15c8b2924621add7baf1554a088768",
+        ),
+        ("linux", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-unknown-linux-gnu-pgo%2Blto-full.tar.zst",
+            "add8cc6cbb4f2a3f8af2272e62b7604f7529a8c357c0af0f8a9f7d3dd444ef1e",
+        ),
+        ("linux", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.10.14%2B20240415-x86_64-unknown-linux-gnu-install_only.tar.gz",
+            "c83c5485659250ef4e4fedb8e7f7b97bc99cc8cf5a1b11d0d1a98d347a43411d",
+        ),
+    },
     PythonVersion("cpython", 3, 10, 13): {
         ("macos", "aarch64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.10.13%2B20240224-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
             "57b83a4aa32bdbe7611f1290313ef24f2574dff5fa59181c0ccb26c14c688b73",
         ),
         ("macos", "aarch64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.10.13%2B20240224-aarch64-apple-darwin-install_only.tar.gz",
@@ -1215,14 +1365,64 @@
             None,
         ),
         ("linux", "x86_64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20211017/cpython-3.10.0-x86_64-unknown-linux-gnu-install_only-20211017T1616.tar.gz",
             None,
         ),
     },
+    PythonVersion("cpython", 3, 9, 19): {
+        ("macos", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "04fd532cfba9b3184a94feaf689bd6147759f1d34ddd674e8b2c146b37a994b1",
+        ),
+        ("macos", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-aarch64-apple-darwin-install_only.tar.gz",
+            "2671bb4ffd036f03076c8aa41e3828c4c16a602e93e2249a8e7b28fd83fdde51",
+        ),
+        ("linux", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-aarch64-unknown-linux-gnu-lto-full.tar.zst",
+            "c462b6f2ab7d87b1000972ff6c1e797c86a1306cceee02cdcc81cd2240f44d34",
+        ),
+        ("linux", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-aarch64-unknown-linux-gnu-install_only.tar.gz",
+            "b18ad819f04c5b2cff6ffa95dd59263d00dcd6f5633d11e43685b4017469cb1c",
+        ),
+        ("windows", "x86", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-i686-pc-windows-msvc-install_only.tar.gz",
+            "683349c1d46ea0aebe5861dde2acdff0b7ea54fc37072a0d3f47d6164b802783",
+        ),
+        ("windows", "x86", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-i686-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "7e6edb16a3973fbb894f3cf4f60a34e22645e84621ec61c622cf4c5a2f4bf2a2",
+        ),
+        ("macos", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "2bb4ed2fc03bb05ac6680b8c11d3c64f7a7dd24b80089c5ad85a91ea4a1795aa",
+        ),
+        ("macos", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-apple-darwin-install_only.tar.gz",
+            "627d903588c0e69ed8b941ba9f91e070e38105a627c5b8c730267744760dca84",
+        ),
+        ("windows", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-pc-windows-msvc-install_only.tar.gz",
+            "9b46faee13e37d8bfa4c02de3775ca3d5dec9378697d755b750fd37788179286",
+        ),
+        ("windows", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "e3611b5699c97bf5ac289e3636e8f932fb177997ee69a81b0c2b15c766ca6f13",
+        ),
+        ("linux", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-unknown-linux-gnu-pgo%2Blto-full.tar.zst",
+            "e1a07336705b58215f8ea138f4abee4640b1baa018e84a9ed44d9a47c7bfa0c8",
+        ),
+        ("linux", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.9.19%2B20240415-x86_64-unknown-linux-gnu-install_only.tar.gz",
+            "00f698873804863dedc0e2b2c2cc4303b49ab0703af2e5883e11340cb8079d0f",
+        ),
+    },
     PythonVersion("cpython", 3, 9, 18): {
         ("macos", "aarch64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.9.18%2B20240224-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
             "579f9b68bbb3a915cbab9682e4d3c253bc96b0556b8a860982c49c25c61f974a",
         ),
         ("macos", "aarch64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.9.18%2B20240224-aarch64-apple-darwin-install_only.tar.gz",
@@ -1965,14 +2165,64 @@
             None,
         ),
         ("linux", "x86_64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20201020/cpython-3.9.0-x86_64-unknown-linux-gnu-pgo-20201020T0627.tar.zst",
             None,
         ),
     },
+    PythonVersion("cpython", 3, 8, 19): {
+        ("macos", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "08cf698453d0a3080426a70dbb43220e915eb4401a9ea0fc798f9f27a3bf7f88",
+        ),
+        ("macos", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-aarch64-apple-darwin-install_only.tar.gz",
+            "eae09ed83ee66353c0cee435ea2d3e4868bd0537214803fb256a1a2928710bc0",
+        ),
+        ("linux", "aarch64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-aarch64-unknown-linux-gnu-lto-full.tar.zst",
+            "31415fdb0d8ea48f09d4a7e0e007f0dd77809be67f5e73ec803f6856d491c542",
+        ),
+        ("linux", "aarch64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-aarch64-unknown-linux-gnu-install_only.tar.gz",
+            "5bde36c53a9a511a1618f159abed77264392eb054edeb57bb5740f6335db34a3",
+        ),
+        ("windows", "x86", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-i686-pc-windows-msvc-install_only.tar.gz",
+            "43766b4ced11b3c4cb0acf60cbfe8e88c6d3d4540192c3fff1463cd131c7473f",
+        ),
+        ("windows", "x86", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-i686-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "d1776a6eecc3bcf549fdbd7adcc9a1ee6e0f0dfaa8ad77f055f5972882d0d227",
+        ),
+        ("macos", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-apple-darwin-pgo%2Blto-full.tar.zst",
+            "e011239aec57e2074093a31f6fb3fee036671ab777fb9764e32bfdb869a80652",
+        ),
+        ("macos", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-apple-darwin-install_only.tar.gz",
+            "05f0c488d84f7590afb6f5d192f071df80584339dda581b6186effc6cd690f6b",
+        ),
+        ("windows", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-pc-windows-msvc-install_only.tar.gz",
+            "ee95c27e5d9de165e77c280ad4d7b51b0dab9567e7e233fc3acf72363870a168",
+        ),
+        ("windows", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-pc-windows-msvc-shared-pgo-full.tar.zst",
+            "ff0812147ab19101c219d0648cf0dbe22b3612decd6034c286451dafe5fe5134",
+        ),
+        ("linux", "x86_64", False): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-unknown-linux-gnu-pgo%2Blto-full.tar.zst",
+            "778a2f806278f033c683b224aa595775c369717d477e0152b1293c9677ba9377",
+        ),
+        ("linux", "x86_64", True): (
+            "https://github.com/indygreg/python-build-standalone/releases/download/20240415/cpython-3.8.19%2B20240415-x86_64-unknown-linux-gnu-install_only.tar.gz",
+            "b33feb5ce0d7f9c4aca8621a9d231dfd9d2f6e26eccb56b63f07041ff573d5a5",
+        ),
+    },
     PythonVersion("cpython", 3, 8, 18): {
         ("macos", "aarch64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.8.18%2B20240224-aarch64-apple-darwin-pgo%2Blto-full.tar.zst",
             "c732c068cddcd6a008c1d6d8e35802f5bdc7323bd2eb64e77210d3d5fe4740c2",
         ),
         ("macos", "aarch64", True): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20240224/cpython-3.8.18%2B20240224-aarch64-apple-darwin-install_only.tar.gz",
@@ -2647,14 +2897,40 @@
     },
     PythonVersion("cpython", 3, 7, 1): {
         ("linux", "x86_64", False): (
             "https://github.com/indygreg/python-build-standalone/releases/download/20181218/cpython-3.7.1-linux64-20181218T1905.tar.zst",
             None,
         )
     },
+    PythonVersion("pypy", 3, 10, 14): {
+        ("linux", "aarch64", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-aarch64.tar.bz2",
+            "fc720999bc5050e1d3706b3b6445e695cf42bfc71ebc7c88ed6bb88828b1d385",
+        ),
+        ("linux", "x86", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-linux32.tar.bz2",
+            "0df48aa780159e879ac89a805d143e4a6cd1b842f98046f5a3f865814bfaa2a4",
+        ),
+        ("linux", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-linux64.tar.bz2",
+            "404e6180d6caf9258eaab0c02c72018e9aa8eb03ab9094a0ff17ee5e3b265ac1",
+        ),
+        ("macos", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-macos_x86_64.tar.bz2",
+            "490f2c6ba2489f405444f3b4ad42166da6e2eb73489a9535b206067eaaf21737",
+        ),
+        ("macos", "aarch64", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-macos_arm64.tar.bz2",
+            "6c003376667a95c7a228544649677b9927b8210d6444b901817aad24b8719b93",
+        ),
+        ("windows", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.10-v7.3.16-win64.zip",
+            "e08415a2f35c6ecf2342b504bdfde11e4c5eca3fc5ef7fd2214ff064a5a54396",
+        ),
+    },
     PythonVersion("pypy", 3, 10, 13): {
         ("linux", "aarch64", True): (
             "https://downloads.python.org/pypy/pypy3.10-v7.3.15-aarch64.tar.bz2",
             "52146fccaf64e87e71d178dda8de63c01577ec3923073dc69e1519622bcacb74",
         ),
         ("linux", "x86", True): (
             "https://downloads.python.org/pypy/pypy3.10-v7.3.15-linux32.tar.bz2",
@@ -2699,14 +2975,40 @@
             "45671b1e9437f95ccd790af10dbeb57733cca1ed9661463b727d3c4f5caa7ba0",
         ),
         ("windows", "x86_64", True): (
             "https://downloads.python.org/pypy/pypy3.10-v7.3.12-win64.zip",
             "8c3b1d34fb99100e230e94560410a38d450dc844effbee9ea183518e4aff595c",
         ),
     },
+    PythonVersion("pypy", 3, 9, 19): {
+        ("linux", "aarch64", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-aarch64.tar.bz2",
+            "de3f2ed3581b30555ac0dd3e4df78a262ec736a36fb2e8f28259f8539b278ef4",
+        ),
+        ("linux", "x86", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-linux32.tar.bz2",
+            "583b6d6dd4e8c07cbc04da04a7ec2bdfa6674825289c2378c5e018d5abe779ea",
+        ),
+        ("linux", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-linux64.tar.bz2",
+            "16f9c5b808c848516e742986e826b833cdbeda09ad8764e8704595adbe791b23",
+        ),
+        ("macos", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-macos_x86_64.tar.bz2",
+            "fda015431621e7e5aa16359d114f2c45a77ed936992c1efff86302e768a6b21c",
+        ),
+        ("macos", "aarch64", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-macos_arm64.tar.bz2",
+            "88f824e7a2d676440d09bc90fc959ae0fd3557d7e2f14bfbbe53d41d159a47fe",
+        ),
+        ("windows", "x86_64", True): (
+            "https://downloads.python.org/pypy/pypy3.9-v7.3.16-win64.zip",
+            "06ec12a5e964dc0ad33e6f380185a4d295178dce6d6df512f508e7aee00a1323",
+        ),
+    },
     PythonVersion("pypy", 3, 9, 18): {
         ("linux", "aarch64", True): (
             "https://downloads.python.org/pypy/pypy3.9-v7.3.15-aarch64.tar.bz2",
             "03e35fcba290454bb0ccf7ee57fb42d1e63108d10d593776a382c0a2fe355de0",
         ),
         ("linux", "x86", True): (
             "https://downloads.python.org/pypy/pypy3.9-v7.3.15-linux32.tar.bz2",
```

### Comparing `pbs_installer-2024.4.1/PKG-INFO` & `pbs_installer-2024.4.24/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbs-installer
-Version: 2024.4.1
+Version: 2024.4.24
 Summary: Installer for Python Build Standalone
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Project-URL: Repository, https://github.com/frostming/pbs-installer
 Project-URL: Documentation, http://pbs-installer.readthedocs.io
 Requires-Python: >=3.8
 Provides-Extra: download
```

