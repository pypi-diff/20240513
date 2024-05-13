# Comparing `tmp/shelloracle-1.3.1.tar.gz` & `tmp/shelloracle-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelloracle-1.3.1.tar", last modified: Sat Apr 27 18:20:22 2024, max compression
+gzip compressed data, was "shelloracle-1.4.0.tar", last modified: Mon May 13 21:48:47 2024, max compression
```

## Comparing `shelloracle-1.3.1.tar` & `shelloracle-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.973976 shelloracle-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-27 18:20:18.000000 shelloracle-1.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-27 18:20:18.000000 shelloracle-1.3.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-27 18:20:18.000000 shelloracle-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-27 18:20:18.000000 shelloracle-1.3.1/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 18:20:18.000000 shelloracle-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-27 18:20:22.977976 shelloracle-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-27 18:20:18.000000 shelloracle-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-27 18:20:18.000000 shelloracle-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 18:20:22.981976 shelloracle-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.973976 shelloracle-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/src/shelloracle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5428 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/src/shelloracle/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/providers/localai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/providers/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/providers/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/src/shelloracle/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/shell/shelloracle.bash
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/shell/shelloracle.zsh
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-27 18:20:18.000000 shelloracle-1.3.1/src/shelloracle/shelloracle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/src/shelloracle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5838 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-27 18:20:22.000000 shelloracle-1.3.1/src/shelloracle.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 18:20:22.977976 shelloracle-1.3.1/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 18:20:18.000000 shelloracle-1.3.1/tests/providers/test_ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-27 18:20:18.000000 shelloracle-1.3.1/tests/providers/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-27 18:20:18.000000 shelloracle-1.3.1/tests/test_shelloracle.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-27 18:20:18.000000 shelloracle-1.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.736650 shelloracle-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.728650 shelloracle-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.728650 shelloracle-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 21:48:40.000000 shelloracle-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 21:48:40.000000 shelloracle-1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-13 21:48:40.000000 shelloracle-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 21:48:40.000000 shelloracle-1.4.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-13 21:48:40.000000 shelloracle-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-13 21:48:47.736650 shelloracle-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-05-13 21:48:40.000000 shelloracle-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-13 21:48:40.000000 shelloracle-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:48:47.736650 shelloracle-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.728650 shelloracle-1.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/src/shelloracle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/src/shelloracle/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/providers/localai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/providers/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/src/shelloracle/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/shell/shelloracle.bash
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/shell/shelloracle.zsh
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/shelloracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-13 21:48:40.000000 shelloracle-1.4.0/src/shelloracle/tty_log_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/src/shelloracle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 21:48:47.000000 shelloracle-1.4.0/src/shelloracle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:48:47.732650 shelloracle-1.4.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/providers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/providers/test_localai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/providers/test_ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/providers/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tests/test_shelloracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-13 21:48:40.000000 shelloracle-1.4.0/tox.ini
```

### Comparing `shelloracle-1.3.1/.github/workflows/release.yml` & `shelloracle-1.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/.github/workflows/tests.yml` & `shelloracle-1.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/.gitignore` & `shelloracle-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/LICENSE` & `shelloracle-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/PKG-INFO` & `shelloracle-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.3.1
+Version: 1.4.0
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -22,14 +22,20 @@
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: openai
 Requires-Dist: prompt-toolkit
 Requires-Dist: yaspin
 Requires-Dist: tomlkit
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
+Provides-Extra: tests
+Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-sugar; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
 
 <p align="center">
   <img src="https://i.imgur.com/IsQYInJ.png" alt="ShellOracle logo"/>
 </p>
 
 <h1 align="center">ShellOracle</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shelloracle Version: 1.3.1 Summary: ShellOracle is
+Metadata-Version: 2.1 Name: shelloracle Version: 1.4.0 Summary: ShellOracle is
 a pluggable terminal utility that takes a natural language description of a
 command and substitutes it into your terminal buffer. Author-email: Daniel
 Copley
 proton.me> Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git Project-
 URL: Issues, https://github.com/djcopley/ShellOracle/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
@@ -11,15 +11,18 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: httpx Requires-Dist: openai Requires-Dist: prompt-
 toolkit Requires-Dist: yaspin Requires-Dist: tomlkit Requires-Dist:
-tomli>=1.1.0; python_version < "3.11"
+tomli>=1.1.0; python_version < "3.11" Provides-Extra: tests Requires-Dist: tox;
+extra == "tests" Requires-Dist: pytest; extra == "tests" Requires-Dist: pytest-
+sugar; extra == "tests" Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
                               [ShellOracle logo]
                            ************ SShheellllOOrraaccllee ************
        _[_T_e_s_t_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_o_w_n_l_o_a_d_s_]
 ShellOracle is an innovative terminal utility designed for intelligent shell
 command generation, bringing a new level of efficiency to your command-line
 interactions. ShellOracle currently supports Ollama, LocalAI, and OpenAI! !
 [ShellOracle](https://i.imgur.com/GJX3eEq.gif) Show your support for
```

### Comparing `shelloracle-1.3.1/README.md` & `shelloracle-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/pyproject.toml` & `shelloracle-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -31,28 +31,37 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
 ]
 
+[project.optional-dependencies]
+tests = [
+    "tox",
+    "pytest",
+    "pytest-sugar",
+    "pytest-asyncio",
+    "pytest-httpx"
+]
+
+[project.scripts]
+shor = "shelloracle.__main__:main"
+
+[project.urls]
+Homepage = "https://github.com/djcopley/ShellOracle"
+Repository = "https://github.com/djcopley/ShellOracle.git"
+Issues = "https://github.com/djcopley/ShellOracle/issues"
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 addopts = [
     "--import-mode=importlib",
 ]
-
-[project.scripts]
-shor = "shelloracle.__main__:main"
-
-[project.urls]
-Homepage = "https://github.com/djcopley/ShellOracle"
-Repository = "https://github.com/djcopley/ShellOracle.git"
-Issues = "https://github.com/djcopley/ShellOracle/issues"
```

### Comparing `shelloracle-1.3.1/src/shelloracle/bootstrap.py` & `shelloracle-1.4.0/src/shelloracle/bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 import tomlkit
 from prompt_toolkit import print_formatted_text, prompt
 from prompt_toolkit.completion import WordCompleter
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.shortcuts import confirm
 
-from .config import Configuration, shelloracle_home
 from .providers import Provider, Setting, list_providers, get_provider
+from .settings import Settings
 
 
 class UserError(Exception):
     ...
 
 
 def print_info(info: str) -> None:
@@ -114,15 +114,16 @@
     config.add("provider", provider_table)
 
     provider_configuration_table = tomlkit.table()
     for setting, value in settings.items():
         provider_configuration_table.add(setting, value)
     provider_table.add(provider.name, provider_configuration_table)
 
-    with Configuration.filepath.open("w") as config_file:
+    filepath = Settings.shelloracle_home / "config.toml"
+    with filepath.open("w") as config_file:
         tomlkit.dump(config, config_file)
 
 
 def install_keybindings() -> None:
     if not (shells := get_installed_shells()):
         print_warning("Cannot install keybindings: no compatible shells found. "
                       f"Supported shells: {', '.join(supported_shells)}")
```

### Comparing `shelloracle-1.3.1/src/shelloracle/providers/__init__.py` & `shelloracle-1.4.0/src/shelloracle/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/src/shelloracle/providers/localai.py` & `shelloracle-1.4.0/src/shelloracle/providers/localai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections.abc import AsyncIterator
 
 from openai import APIError
-from openai import AsyncOpenAI as OpenAIClient
+from openai import AsyncOpenAI
 
 from . import Provider, ProviderError, Setting, system_prompt
 
 
 class LocalAI(Provider):
     name = "LocalAI"
 
@@ -15,15 +15,15 @@
 
     @property
     def endpoint(self) -> str:
         return f"http://{self.host}:{self.port}"
 
     def __init__(self):
         # Use a placeholder API key so the client will work
-        self.client = OpenAIClient(api_key="sk-xxx", base_url=self.endpoint)
+        self.client = AsyncOpenAI(api_key="sk-xxx", base_url=self.endpoint)
 
     async def generate(self, prompt: str) -> AsyncIterator[str]:
         try:
             stream = await self.client.chat.completions.create(
                 model=self.model,
                 messages=[
                     {"role": "system", "content": system_prompt},
```

### Comparing `shelloracle-1.3.1/src/shelloracle/providers/ollama.py` & `shelloracle-1.4.0/src/shelloracle/providers/ollama.py`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/src/shelloracle/providers/openai.py` & `shelloracle-1.4.0/src/shelloracle/providers/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from collections.abc import AsyncIterator
 
-from openai import APIError
-from openai import AsyncOpenAI as OpenAIClient
+from openai import AsyncOpenAI, APIError
 
 from . import Provider, ProviderError, Setting, system_prompt
 
 
 class OpenAI(Provider):
     name = "OpenAI"
 
     api_key = Setting(default="")
     model = Setting(default="gpt-3.5-turbo")
 
     def __init__(self):
         if not self.api_key:
             raise ProviderError("No API key provided")
-        self.client = OpenAIClient(api_key=self.api_key)
+        self.client = AsyncOpenAI(api_key=self.api_key)
 
     async def generate(self, prompt: str) -> AsyncIterator[str]:
         try:
             stream = await self.client.chat.completions.create(
                 model=self.model,
                 messages=[
                     {"role": "system", "content": system_prompt},
```

### Comparing `shelloracle-1.3.1/src/shelloracle/shell/shelloracle.bash` & `shelloracle-1.4.0/src/shelloracle/shell/shelloracle.bash`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/src/shelloracle/shell/shelloracle.zsh` & `shelloracle-1.4.0/src/shelloracle/shell/shelloracle.zsh`

 * *Files identical despite different names*

### Comparing `shelloracle-1.3.1/src/shelloracle/shelloracle.py` & `shelloracle-1.4.0/src/shelloracle/shelloracle.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import asyncio
 import logging
 import os
 import sys
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-from prompt_toolkit import PromptSession, print_formatted_text
+from prompt_toolkit import PromptSession
 from prompt_toolkit.application import create_app_session_from_tty
-from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.history import FileHistory
 from prompt_toolkit.patch_stdout import patch_stdout
 from yaspin import yaspin
 from yaspin.spinners import Spinners
 
 from .config import get_config
 from .providers import get_provider
@@ -25,16 +24,14 @@
 
 
 async def prompt_user(default_prompt: str | None = None) -> str:
     # stdin doesn't exist when running as a zle widget
     with create_app_session_from_tty(), patch_stdout():
         history_file = Path.home() / ".shelloracle_history"
         prompt_session: PromptSession = PromptSession(history=FileHistory(str(history_file)))
-        # Can I do this with one of the builtin methods?
-        # I tried a few (including cursor_down) with limited success
         prompt_session.output.write_raw("\033[E")
         return await prompt_session.prompt_async("> ", default=default_prompt or "")
 
 
 def get_query_from_pipe() -> str | None:
     """Get a query from stdin pipe.
 
@@ -98,10 +95,8 @@
     :returns: None
     """
     try:
         asyncio.run(shelloracle())
     except (KeyboardInterrupt, asyncio.exceptions.CancelledError):
         return
     except Exception as err:
-        logger.exception("An unhandled exception occurred")
-        with create_app_session_from_tty():
-            print_formatted_text(FormattedText([("ansired", f"\n{err}")]))
+        logger.error("An error occurred: %s", err)
```

### Comparing `shelloracle-1.3.1/src/shelloracle.egg-info/PKG-INFO` & `shelloracle-1.4.0/src/shelloracle.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelloracle
-Version: 1.3.1
+Version: 1.4.0
 Summary: ShellOracle is a pluggable terminal utility that takes a natural language description of a command and substitutes it into your terminal buffer.
 Author-email: Daniel Copley <djcopley@proton.me>
 Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git
 Project-URL: Issues, https://github.com/djcopley/ShellOracle/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -22,14 +22,20 @@
 License-File: LICENSE
 Requires-Dist: httpx
 Requires-Dist: openai
 Requires-Dist: prompt-toolkit
 Requires-Dist: yaspin
 Requires-Dist: tomlkit
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
+Provides-Extra: tests
+Requires-Dist: tox; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-sugar; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
 
 <p align="center">
   <img src="https://i.imgur.com/IsQYInJ.png" alt="ShellOracle logo"/>
 </p>
 
 <h1 align="center">ShellOracle</h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shelloracle Version: 1.3.1 Summary: ShellOracle is
+Metadata-Version: 2.1 Name: shelloracle Version: 1.4.0 Summary: ShellOracle is
 a pluggable terminal utility that takes a natural language description of a
 command and substitutes it into your terminal buffer. Author-email: Daniel
 Copley
 proton.me> Project-URL: Homepage, https://github.com/djcopley/ShellOracle
 Project-URL: Repository, https://github.com/djcopley/ShellOracle.git Project-
 URL: Issues, https://github.com/djcopley/ShellOracle/issues Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
@@ -11,15 +11,18 @@
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: httpx Requires-Dist: openai Requires-Dist: prompt-
 toolkit Requires-Dist: yaspin Requires-Dist: tomlkit Requires-Dist:
-tomli>=1.1.0; python_version < "3.11"
+tomli>=1.1.0; python_version < "3.11" Provides-Extra: tests Requires-Dist: tox;
+extra == "tests" Requires-Dist: pytest; extra == "tests" Requires-Dist: pytest-
+sugar; extra == "tests" Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
                               [ShellOracle logo]
                            ************ SShheellllOOrraaccllee ************
        _[_T_e_s_t_s_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_P_I_ _S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_s_]_[_D_o_w_n_l_o_a_d_s_]
 ShellOracle is an innovative terminal utility designed for intelligent shell
 command generation, bringing a new level of efficiency to your command-line
 interactions. ShellOracle currently supports Ollama, LocalAI, and OpenAI! !
 [ShellOracle](https://i.imgur.com/GJX3eEq.gif) Show your support for
```

### Comparing `shelloracle-1.3.1/src/shelloracle.egg-info/SOURCES.txt` & `shelloracle-1.4.0/src/shelloracle.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,29 @@
 tox.ini
 .github/workflows/release.yml
 .github/workflows/tests.yml
 src/shelloracle/__init__.py
 src/shelloracle/__main__.py
 src/shelloracle/bootstrap.py
 src/shelloracle/config.py
+src/shelloracle/settings.py
 src/shelloracle/shelloracle.py
+src/shelloracle/tty_log_handler.py
 src/shelloracle.egg-info/PKG-INFO
 src/shelloracle.egg-info/SOURCES.txt
 src/shelloracle.egg-info/dependency_links.txt
 src/shelloracle.egg-info/entry_points.txt
 src/shelloracle.egg-info/requires.txt
 src/shelloracle.egg-info/top_level.txt
 src/shelloracle/providers/__init__.py
 src/shelloracle/providers/localai.py
 src/shelloracle/providers/ollama.py
 src/shelloracle/providers/openai.py
 src/shelloracle/shell/shelloracle.bash
 src/shelloracle/shell/shelloracle.zsh
+tests/conftest.py
+tests/test_config.py
 tests/test_shelloracle.py
+tests/providers/conftest.py
+tests/providers/test_localai.py
 tests/providers/test_ollama.py
 tests/providers/test_openai.py
```

### Comparing `shelloracle-1.3.1/tests/test_shelloracle.py` & `shelloracle-1.4.0/tests/test_shelloracle.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import sys
-from unittest.mock import MagicMock, call
+from unittest.mock import call, MagicMock
 
 import pytest
 from yaspin.spinners import Spinners
 
 from shelloracle.shelloracle import get_query_from_pipe, spinner
```

