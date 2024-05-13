# Comparing `tmp/poetry_plugin_dotenv-2.1.5.tar.gz` & `tmp/poetry_plugin_dotenv-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_dotenv-2.1.5.tar", max compression
+gzip compressed data, was "poetry_plugin_dotenv-2.1.6.tar", max compression
```

## Comparing `poetry_plugin_dotenv-2.1.5.tar` & `poetry_plugin_dotenv-2.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1077 2024-05-09 09:41:02.197175 poetry_plugin_dotenv-2.1.5/LICENSE
--rw-r--r--   0        0        0     8724 2024-05-09 09:41:02.197175 poetry_plugin_dotenv-2.1.5/README.md
--rw-r--r--   0        0        0     6955 2024-05-09 09:41:23.029021 poetry_plugin_dotenv-2.1.5/pyproject.toml
--rw-r--r--   0        0        0      778 2024-05-09 09:41:23.029021 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0     3051 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/config.py
--rw-r--r--   0        0        0      335 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/__init__.py
--rw-r--r--   0        0        0     5421 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/core.py
--rw-r--r--   0        0        0     6005 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/parsers.py
--rw-r--r--   0        0        0     1572 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/variables.py
--rw-r--r--   0        0        0     1558 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/logger.py
--rw-r--r--   0        0        0     1999 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0        0 2024-05-09 09:41:02.209175 poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/py.typed
--rw-r--r--   0        0        0    10727 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-13 07:28:03.819683 poetry_plugin_dotenv-2.1.6/LICENSE
+-rw-r--r--   0        0        0     8766 2024-05-13 07:28:03.819683 poetry_plugin_dotenv-2.1.6/README.md
+-rw-r--r--   0        0        0     6955 2024-05-13 07:28:24.151808 poetry_plugin_dotenv-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0      778 2024-05-13 07:28:24.151808 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0     3051 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/config.py
+-rw-r--r--   0        0        0      335 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/__init__.py
+-rw-r--r--   0        0        0     5421 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/core.py
+-rw-r--r--   0        0        0     6005 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/parsers.py
+-rw-r--r--   0        0        0     1572 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/variables.py
+-rw-r--r--   0        0        0     1558 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/logger.py
+-rw-r--r--   0        0        0     1999 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0        0 2024-05-13 07:28:03.831683 poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/py.typed
+-rw-r--r--   0        0        0    10769 1970-01-01 00:00:00.000000 poetry_plugin_dotenv-2.1.6/PKG-INFO
```

### Comparing `poetry_plugin_dotenv-2.1.5/LICENSE` & `poetry_plugin_dotenv-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/README.md` & `poetry_plugin_dotenv-2.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,15 @@
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
 ### Features
 
 - Doesn't require any dependencies
 - Supports templates, interpolating variables using POSIX variable expansions
 - Fully type safe
+- Supports multiple configuration sources
 - 100% test coverage and "A" grade for maintainability
 
 ## Installation
 
 ```bash
 poetry self add poetry-plugin-dotenv
 ```
```

#### html2text {}

```diff
@@ -9,26 +9,26 @@
 - [Usage and Configuration](#usage-and-configuration) - [Configuration via
 file](#configuration-via-file) - [Configuration via environment variables]
 (#configuration-via-environment-variables) - [Lookup hierarchy](#lookup-
 hierarchy) - [Examples](#examples) ## Overview `poetry-plugin-dotenv` - is the
 plugin that automatically loads environment variables from a dotenv file into
 the environment before `poetry` commands are run. ### Features - Doesn't
 require any dependencies - Supports templates, interpolating variables using
-POSIX variable expansions - Fully type safe - 100% test coverage and "A" grade
-for maintainability ## Installation ```bash poetry self add poetry-plugin-
-dotenv ``` ## Usage and Configuration By default, the plugin will load the
-`.env` file from the current working directory or "higher directories". To
-prevent `poetry` from loading the dotenv file, set the `ignore` option. If your
-dotenv file is located in a different path or has a different name you may set
-the `location`. `ignore` option can accept the next values: - As True: `y / yes
-/ t / on / 1 / true` - As False: `n / no / f / off / 0 / false` ###
-Configuration via file The plugin is able to read project-specific default
-values for its options from a `pyproject.toml` file. By default, `poetry-
-plugin-dotenv` looks for `pyproject.toml` containing a `
-[tool.poetry.plugins.dotenv]` section. Example `pyproject.toml`: ```toml
+POSIX variable expansions - Fully type safe - Supports multiple configuration
+sources - 100% test coverage and "A" grade for maintainability ## Installation
+```bash poetry self add poetry-plugin-dotenv ``` ## Usage and Configuration By
+default, the plugin will load the `.env` file from the current working
+directory or "higher directories". To prevent `poetry` from loading the dotenv
+file, set the `ignore` option. If your dotenv file is located in a different
+path or has a different name you may set the `location`. `ignore` option can
+accept the next values: - As True: `y / yes / t / on / 1 / true` - As False: `n
+/ no / f / off / 0 / false` ### Configuration via file The plugin is able to
+read project-specific default values for its options from a `pyproject.toml`
+file. By default, `poetry-plugin-dotenv` looks for `pyproject.toml` containing
+a `[tool.poetry.plugins.dotenv]` section. Example `pyproject.toml`: ```toml
 [tool.poetry.plugins.dotenv] ignore = "false" location = ".env.dev" ``` >
 [!IMPORTANT] > Due to the default `poetry` parser, options in the plugins
 sections should be always strings. ### Configuration via environment variables
 `poetry-plugin-dotenv` supports the following configuration options via
 environment variables. - `POETRY_PLUGIN_DOTENV_LOCATION` -
 `POETRY_PLUGIN_DOTENV_IGNORE` > [!IMPORTANT] > Due to the nature of environment
 variables, options should be always strings. ### Lookup hierarchy A
```

### Comparing `poetry_plugin_dotenv-2.1.5/pyproject.toml` & `poetry_plugin_dotenv-2.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-dotenv"
-version = "2.1.5"
+version = "2.1.6"
 description = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 license = "MIT"
 authors = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 maintainers = ["Volodymyr Pivoshenko <volodymyr.pivoshenko@gmail.com>"]
 keywords = [
   "python",
   "pypi",
```

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/__init__.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."""
 
 __title__ = "poetry-plugin-dotenv"
 __summary__ = "poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run."
 __uri__ = "https://github.com/pivoshenko/poetry-plugin-dotenv"
 
-__version__ = "2.1.5"
+__version__ = "2.1.6"
 
 __author__ = "Volodymyr Pivoshenko"
 __email__ = "volodymyr.pivoshenko@gmail.com"
 
 __license__ = "MIT"
 __copyright__ = "Copyright 2023, Volodymyr Pivoshenko"
```

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/config.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/config.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/core.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/core.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/parsers.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/parsers.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/dotenv/variables.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/dotenv/variables.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/logger.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/logger.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/src/poetry_plugin_dotenv/plugin.py` & `poetry_plugin_dotenv-2.1.6/src/poetry_plugin_dotenv/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_dotenv-2.1.5/PKG-INFO` & `poetry_plugin_dotenv-2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-dotenv
-Version: 2.1.5
+Version: 2.1.6
 Summary: poetry-plugin-dotenv - is the plugin that automatically loads environment variables from a dotenv file into the environment before poetry commands are run.
 Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv
 License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-plugins,env,dotenv,config,configuration,configuration-management,cross-platform,hacktoberfest
 Author: Volodymyr Pivoshenko
 Author-email: volodymyr.pivoshenko@gmail.com
 Maintainer: Volodymyr Pivoshenko
@@ -134,14 +134,15 @@
 `poetry-plugin-dotenv` - is the plugin that automatically loads environment variables from a dotenv file into the environment before `poetry` commands are run.
 
 ### Features
 
 - Doesn't require any dependencies
 - Supports templates, interpolating variables using POSIX variable expansions
 - Fully type safe
+- Supports multiple configuration sources
 - 100% test coverage and "A" grade for maintainability
 
 ## Installation
 
 ```bash
 poetry self add poetry-plugin-dotenv
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.5 Summary:
+Metadata-Version: 2.1 Name: poetry-plugin-dotenv Version: 2.1.6 Summary:
 poetry-plugin-dotenv - is the plugin that automatically loads environment
 variables from a dotenv file into the environment before poetry commands are
 run. Home-page: https://github.com/pivoshenko/poetry-plugin-dotenv License: MIT
 Keywords: python,pypi,poetry,plugin,plugins,poetry-plugin,poetry-
 plugins,env,dotenv,config,configuration,configuration-management,cross-
 platform,hacktoberfest Author: Volodymyr Pivoshenko Author-email:
 volodymyr.pivoshenko@gmail.com Maintainer: Volodymyr Pivoshenko Maintainer-
@@ -36,26 +36,26 @@
 - [Usage and Configuration](#usage-and-configuration) - [Configuration via
 file](#configuration-via-file) - [Configuration via environment variables]
 (#configuration-via-environment-variables) - [Lookup hierarchy](#lookup-
 hierarchy) - [Examples](#examples) ## Overview `poetry-plugin-dotenv` - is the
 plugin that automatically loads environment variables from a dotenv file into
 the environment before `poetry` commands are run. ### Features - Doesn't
 require any dependencies - Supports templates, interpolating variables using
-POSIX variable expansions - Fully type safe - 100% test coverage and "A" grade
-for maintainability ## Installation ```bash poetry self add poetry-plugin-
-dotenv ``` ## Usage and Configuration By default, the plugin will load the
-`.env` file from the current working directory or "higher directories". To
-prevent `poetry` from loading the dotenv file, set the `ignore` option. If your
-dotenv file is located in a different path or has a different name you may set
-the `location`. `ignore` option can accept the next values: - As True: `y / yes
-/ t / on / 1 / true` - As False: `n / no / f / off / 0 / false` ###
-Configuration via file The plugin is able to read project-specific default
-values for its options from a `pyproject.toml` file. By default, `poetry-
-plugin-dotenv` looks for `pyproject.toml` containing a `
-[tool.poetry.plugins.dotenv]` section. Example `pyproject.toml`: ```toml
+POSIX variable expansions - Fully type safe - Supports multiple configuration
+sources - 100% test coverage and "A" grade for maintainability ## Installation
+```bash poetry self add poetry-plugin-dotenv ``` ## Usage and Configuration By
+default, the plugin will load the `.env` file from the current working
+directory or "higher directories". To prevent `poetry` from loading the dotenv
+file, set the `ignore` option. If your dotenv file is located in a different
+path or has a different name you may set the `location`. `ignore` option can
+accept the next values: - As True: `y / yes / t / on / 1 / true` - As False: `n
+/ no / f / off / 0 / false` ### Configuration via file The plugin is able to
+read project-specific default values for its options from a `pyproject.toml`
+file. By default, `poetry-plugin-dotenv` looks for `pyproject.toml` containing
+a `[tool.poetry.plugins.dotenv]` section. Example `pyproject.toml`: ```toml
 [tool.poetry.plugins.dotenv] ignore = "false" location = ".env.dev" ``` >
 [!IMPORTANT] > Due to the default `poetry` parser, options in the plugins
 sections should be always strings. ### Configuration via environment variables
 `poetry-plugin-dotenv` supports the following configuration options via
 environment variables. - `POETRY_PLUGIN_DOTENV_LOCATION` -
 `POETRY_PLUGIN_DOTENV_IGNORE` > [!IMPORTANT] > Due to the nature of environment
 variables, options should be always strings. ### Lookup hierarchy A
```

