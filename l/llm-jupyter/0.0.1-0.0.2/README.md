# Comparing `tmp/llm_jupyter-0.0.1.tar.gz` & `tmp/llm_jupyter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_jupyter-0.0.1.tar", last modified: Sun May 12 15:56:51 2024, max compression
+gzip compressed data, was "llm_jupyter-0.0.2.tar", last modified: Sun May 12 16:28:25 2024, max compression
```

## Comparing `llm_jupyter-0.0.1.tar` & `llm_jupyter-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:56:51.659815 llm_jupyter-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 15:56:44.000000 llm_jupyter-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-12 15:56:51.659815 llm_jupyter-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-05-12 15:56:44.000000 llm_jupyter-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:56:51.659815 llm_jupyter-0.0.1/llm_jupyter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 15:56:51.000000 llm_jupyter-0.0.1/llm_jupyter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-12 15:56:44.000000 llm_jupyter-0.0.1/llm_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-12 15:56:44.000000 llm_jupyter-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 15:56:51.659815 llm_jupyter-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 15:56:51.659815 llm_jupyter-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-12 15:56:44.000000 llm_jupyter-0.0.1/tests/test_ipython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:25.551441 llm_jupyter-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 16:28:17.000000 llm_jupyter-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-12 16:28:25.551441 llm_jupyter-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-12 16:28:17.000000 llm_jupyter-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:25.551441 llm_jupyter-0.0.2/llm_jupyter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-12 16:28:25.000000 llm_jupyter-0.0.2/llm_jupyter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-12 16:28:17.000000 llm_jupyter-0.0.2/llm_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-12 16:28:17.000000 llm_jupyter-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 16:28:25.551441 llm_jupyter-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 16:28:25.547441 llm_jupyter-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-12 16:28:17.000000 llm_jupyter-0.0.2/tests/test_ipython.py
```

### Comparing `llm_jupyter-0.0.1/LICENSE` & `llm_jupyter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_jupyter-0.0.1/PKG-INFO` & `llm_jupyter-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: llm-jupyter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Run a IPython interpreter in the LLM virtual environment
 Author: Simon Willison
+Author-email: Lucas Rangel Cezimbra <lucas@cezimbra.tec.br>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/lucasrcezimbra/llm-jupyter
 Project-URL: Changelog, https://github.com/lucasrcezimbra/llm-jupyter/releases
 Project-URL: Issues, https://github.com/lucasrcezimbra/llm-jupyter/issues
 Project-URL: CI, https://github.com/lucasrcezimbra/llm-jupyter/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -48,16 +49,17 @@
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
+pip install -e .[test]
 ```
 Now install the dependencies and test dependencies:
 ```bash
 llm install -e '.[test]'
 ```
 To run the tests:
 ```bash
```

### Comparing `llm_jupyter-0.0.1/README.md` & `llm_jupyter-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,17 @@
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
+pip install -e .[test]
 ```
 Now install the dependencies and test dependencies:
 ```bash
 llm install -e '.[test]'
 ```
 To run the tests:
 ```bash
```

### Comparing `llm_jupyter-0.0.1/llm_jupyter.egg-info/PKG-INFO` & `llm_jupyter-0.0.2/llm_jupyter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: llm-jupyter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Run a IPython interpreter in the LLM virtual environment
 Author: Simon Willison
+Author-email: Lucas Rangel Cezimbra <lucas@cezimbra.tec.br>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/lucasrcezimbra/llm-jupyter
 Project-URL: Changelog, https://github.com/lucasrcezimbra/llm-jupyter/releases
 Project-URL: Issues, https://github.com/lucasrcezimbra/llm-jupyter/issues
 Project-URL: CI, https://github.com/lucasrcezimbra/llm-jupyter/actions
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
@@ -48,16 +49,17 @@
 
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 git clone git@github.com:lucasrcezimbra/llm-jupyter.git
 cd llm-jupyter
-python3 -m venv .venv
+python -m venv .venv
 source .venv/bin/activate
+pip install -e .[test]
 ```
 Now install the dependencies and test dependencies:
 ```bash
 llm install -e '.[test]'
 ```
 To run the tests:
 ```bash
```

### Comparing `llm_jupyter-0.0.1/pyproject.toml` & `llm_jupyter-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [project]
 name = "llm-jupyter"
-version = "0.0.1"
+version = "0.0.2"
 description = "Run a IPython interpreter in the LLM virtual environment"
 readme = "README.md"
-authors = [{name = "Simon Willison"}]
+authors = [
+  {name = "Lucas Rangel Cezimbra", email="lucas@cezimbra.tec.br"},
+  {name = "Simon Willison"},
+]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "ipython",
     "llm",
```

