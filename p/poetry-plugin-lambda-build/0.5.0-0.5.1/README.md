# Comparing `tmp/poetry_plugin_lambda_build-0.5.0.tar.gz` & `tmp/poetry_plugin_lambda_build-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.5.0.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.5.1.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.5.0.tar` & `poetry_plugin_lambda_build-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/LICENSE
--rw-r--r--   0        0        0     5519 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0      891 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/commands.py
--rw-r--r--   0        0        0     2862 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     3877 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/parameters.py
--rw-r--r--   0        0        0     2041 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0    11409 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0     6752 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/requirements.py
--rw-r--r--   0        0        0     2120 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0     9831 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/walker.py
--rw-r--r--   0        0        0      767 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0     1042 2024-05-08 13:30:39.097909 poetry_plugin_lambda_build-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     6229 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-13 13:03:56.467161 poetry_plugin_lambda_build-0.5.1/LICENSE
+-rw-r--r--   0        0        0     5519 2024-05-13 13:03:56.467161 poetry_plugin_lambda_build-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0      913 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/commands.py
+-rw-r--r--   0        0        0     2862 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     3877 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/parameters.py
+-rw-r--r--   0        0        0     2041 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0    11409 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0     6752 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/requirements.py
+-rw-r--r--   0        0        0     2120 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0     9831 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/walker.py
+-rw-r--r--   0        0        0      767 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0     1042 2024-05-13 13:03:56.471161 poetry_plugin_lambda_build-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6229 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.5.1/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.5.0/LICENSE` & `poetry_plugin_lambda_build-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/README.md` & `poetry_plugin_lambda_build-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/commands.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/commands.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from poetry_plugin_lambda_build.utils import join_cmds
 
 MKDIR = "mkdir -p {output_dir}"
 INSTALL_DEPS_CMD_TMPL = "pip install -q -t {output_dir} --no-cache-dir -r {requirements}"
 INSTALL_POETRY_CMD = "pip install poetry --quiet --upgrade pip"
 BUILD_PACKAGE_CMD = "poetry build -q"
-INSTALL_WHL_CMD_TMPL = "poetry run pip install -q -t {output_dir} --find-links=dist {package_name} --no-cache-dir --upgrade"
-INSTALL_WHL_NO_DEPS_CMD_TMPL = "poetry run pip install -q -t {output_dir} --find-links=dist {package_name} --no-cache-dir --no-deps --upgrade"
+INSTALL_WHL_CMD_TMPL = "poetry run pip install -q -t {output_dir} --no-index --find-links=dist {package_name} --no-cache-dir --upgrade"
+INSTALL_WHL_NO_DEPS_CMD_TMPL = "poetry run pip install -q -t {output_dir} --no-index --find-links=dist {package_name} --no-cache-dir --no-deps --upgrade"
 
 
 INSTALL_DEPS_CMD_IN_CONTAINER_TMPL = join_cmds(MKDIR, INSTALL_DEPS_CMD_TMPL)
 
 BUILD_N_INSTALL_CMD_TMPL = join_cmds(
     INSTALL_POETRY_CMD,
     BUILD_PACKAGE_CMD,
```

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/docker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/parameters.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/parameters.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/recipes.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/requirements.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/utils.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/walker.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.5.1/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.5.0/pyproject.toml` & `poetry_plugin_lambda_build-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.5.0"
+version = "0.5.1"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michal Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docker = "^7.0.0"
```

### Comparing `poetry_plugin_lambda_build-0.5.0/PKG-INFO` & `poetry_plugin_lambda_build-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.5.0
+Version: 0.5.1
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

