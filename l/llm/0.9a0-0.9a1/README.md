# Comparing `tmp/llm-0.9a0.tar.gz` & `tmp/llm-0.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm-0.9a0.tar", last modified: Sat Sep  2 17:55:36 2023, max compression
+gzip compressed data, was "llm-0.9a1.tar", last modified: Mon Sep  4 01:29:28 2023, max compression
```

## Comparing `llm-0.9a0.tar` & `llm-0.9a1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:55:36.951825 llm-0.9a0/
--rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-09-02 17:55:17.000000 llm-0.9a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       23 2023-09-02 17:55:17.000000 llm-0.9a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     3591 2023-09-02 17:55:36.951825 llm-0.9a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2949 2023-09-02 17:55:17.000000 llm-0.9a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:55:36.951825 llm-0.9a0/llm/
--rw-r--r--   0 runner    (1001) docker     (999)     7215 2023-09-02 17:55:17.000000 llm-0.9a0/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       59 2023-09-02 17:55:17.000000 llm-0.9a0/llm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)    34089 2023-09-02 17:55:17.000000 llm-0.9a0/llm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:55:36.951825 llm-0.9a0/llm/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-02 17:55:17.000000 llm-0.9a0/llm/default_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    11561 2023-09-02 17:55:17.000000 llm-0.9a0/llm/default_plugins/openai_models.py
--rw-r--r--   0 runner    (1001) docker     (999)     8885 2023-09-02 17:55:17.000000 llm-0.9a0/llm/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (999)      649 2023-09-02 17:55:17.000000 llm-0.9a0/llm/embeddings_migrations.py
--rw-r--r--   0 runner    (1001) docker     (999)      214 2023-09-02 17:55:17.000000 llm-0.9a0/llm/errors.py
--rw-r--r--   0 runner    (1001) docker     (999)      492 2023-09-02 17:55:17.000000 llm-0.9a0/llm/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (999)     4836 2023-09-02 17:55:17.000000 llm-0.9a0/llm/migrations.py
--rw-r--r--   0 runner    (1001) docker     (999)     9356 2023-09-02 17:55:17.000000 llm-0.9a0/llm/models.py
--rw-r--r--   0 runner    (1001) docker     (999)      419 2023-09-02 17:55:17.000000 llm-0.9a0/llm/plugins.py
--rw-r--r--   0 runner    (1001) docker     (999)     1848 2023-09-02 17:55:17.000000 llm-0.9a0/llm/templates.py
--rw-r--r--   0 runner    (1001) docker     (999)      721 2023-09-02 17:55:17.000000 llm-0.9a0/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 17:55:36.951825 llm-0.9a0/llm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     3591 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       36 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      225 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        4 2023-09-02 17:55:36.000000 llm-0.9a0/llm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-02 17:55:36.951825 llm-0.9a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1665 2023-09-02 17:55:17.000000 llm-0.9a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 01:29:28.887634 llm-0.9a1/
+-rw-r--r--   0 runner    (1001) docker     (999)    11357 2023-09-04 01:29:11.000000 llm-0.9a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)       23 2023-09-04 01:29:11.000000 llm-0.9a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     3734 2023-09-04 01:29:28.887634 llm-0.9a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     3092 2023-09-04 01:29:11.000000 llm-0.9a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 01:29:28.883634 llm-0.9a1/llm/
+-rw-r--r--   0 runner    (1001) docker     (999)     7422 2023-09-04 01:29:11.000000 llm-0.9a1/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)       59 2023-09-04 01:29:11.000000 llm-0.9a1/llm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    41282 2023-09-04 01:29:11.000000 llm-0.9a1/llm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 01:29:28.883634 llm-0.9a1/llm/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-04 01:29:11.000000 llm-0.9a1/llm/default_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11561 2023-09-04 01:29:11.000000 llm-0.9a1/llm/default_plugins/openai_models.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11332 2023-09-04 01:29:11.000000 llm-0.9a1/llm/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2254 2023-09-04 01:29:11.000000 llm-0.9a1/llm/embeddings_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (999)      214 2023-09-04 01:29:11.000000 llm-0.9a1/llm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (999)      498 2023-09-04 01:29:11.000000 llm-0.9a1/llm/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4836 2023-09-04 01:29:11.000000 llm-0.9a1/llm/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (999)     9356 2023-09-04 01:29:11.000000 llm-0.9a1/llm/models.py
+-rw-r--r--   0 runner    (1001) docker     (999)      419 2023-09-04 01:29:11.000000 llm-0.9a1/llm/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1848 2023-09-04 01:29:11.000000 llm-0.9a1/llm/templates.py
+-rw-r--r--   0 runner    (1001) docker     (999)      721 2023-09-04 01:29:11.000000 llm-0.9a1/llm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-04 01:29:28.883634 llm-0.9a1/llm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     3734 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)      469 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       36 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      232 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        4 2023-09-04 01:29:28.000000 llm-0.9a1/llm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-04 01:29:28.887634 llm-0.9a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     1672 2023-09-04 01:29:11.000000 llm-0.9a1/setup.py
```

### Comparing `llm-0.9a0/LICENSE` & `llm-0.9a1/LICENSE`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/PKG-INFO` & `llm-0.9a1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.9a0
+Version: 0.9a1
 Summary: A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
@@ -18,14 +18,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
 [![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://datasette.io/discord-llm)
+[![Homebrew](https://img.shields.io/homebrew/installs/dy/llm?color=yellow&label=homebrew&logo=homebrew)](https://formulae.brew.sh/formula/llm)
 
 A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 
 Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
 
 Background on this project:
 - [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/)
```

### Comparing `llm-0.9a0/README.md` & `llm-0.9a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
 [![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://datasette.io/discord-llm)
+[![Homebrew](https://img.shields.io/homebrew/installs/dy/llm?color=yellow&label=homebrew&logo=homebrew)](https://formulae.brew.sh/formula/llm)
 
 A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 
 Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
 
 Background on this project:
 - [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/)
```

### Comparing `llm-0.9a0/llm/__init__.py` & `llm-0.9a1/llm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def get_embedding_model(name):
     aliases = get_embedding_model_aliases()
     try:
         return aliases[name]
     except KeyError:
-        raise UnknownModelError("Unknown model: " + name)
+        raise UnknownModelError("Unknown model: " + str(name))
 
 
 def get_embedding_model_aliases() -> Dict[str, EmbeddingModel]:
     model_aliases = {}
     for model_with_aliases in get_embedding_models_with_aliases():
         for alias in model_with_aliases.aliases:
             model_aliases[alias] = model_with_aliases.model
@@ -204,16 +204,21 @@
         # We're going to write a valid JSON file in a moment:
         current = {}
     # Resolve model_id_or_alias to a model_id
     try:
         model = get_model(model_id_or_alias)
         model_id = model.model_id
     except UnknownModelError:
-        # Set the alias to the exact string they provided instead
-        model_id = model_id_or_alias
+        # Try to resolve it to an embedding model
+        try:
+            model = get_embedding_model(model_id_or_alias)
+            model_id = model.model_id
+        except UnknownModelError:
+            # Set the alias to the exact string they provided instead
+            model_id = model_id_or_alias
     current[alias] = model_id
     path.write_text(json.dumps(current, indent=4) + "\n")
 
 
 def remove_alias(alias):
     """
     Remove an alias.
```

### Comparing `llm-0.9a0/llm/cli.py` & `llm-0.9a1/llm/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import click
 from click_default_group import DefaultGroup
 from dataclasses import asdict
+import io
 import json
 from llm import (
     Collection,
     Conversation,
     Response,
     Template,
     UnknownModelError,
     encode,
     get_embedding_models_with_aliases,
+    get_embedding_model_aliases,
     get_embedding_model,
     get_key,
     get_plugins,
     get_model,
     get_model_aliases,
     get_models_with_aliases,
     user_dir,
@@ -25,28 +27,41 @@
 from .plugins import pm
 import base64
 import pathlib
 import pydantic
 from runpy import run_module
 import shutil
 import sqlite_utils
+from sqlite_utils.utils import rows_from_file, Format
 import sys
 import textwrap
 from typing import cast, Optional
 import warnings
 import yaml
 
 warnings.simplefilter("ignore", ResourceWarning)
 
 DEFAULT_MODEL = "gpt-3.5-turbo"
 DEFAULT_EMBEDDING_MODEL = "ada-002"
 
 DEFAULT_TEMPLATE = "prompt: "
 
 
+def _validate_metadata_json(ctx, param, value):
+    if value is None:
+        return value
+    try:
+        obj = json.loads(value)
+        if not isinstance(obj, dict):
+            raise click.BadParameter("Metadata must be a JSON object")
+        return obj
+    except json.JSONDecodeError:
+        raise click.BadParameter("Metadata must be valid JSON")
+
+
 @click.group(
     cls=DefaultGroup,
     default="prompt",
     default_if_no_args=True,
 )
 @click.version_option()
 def cli():
@@ -717,22 +732,31 @@
 @aliases.command(name="list")
 @click.option("json_", "--json", is_flag=True, help="Output as JSON")
 def aliases_list(json_):
     "List current aliases"
     to_output = []
     for alias, model in get_model_aliases().items():
         if alias != model.model_id:
-            to_output.append((alias, model.model_id))
+            to_output.append((alias, model.model_id, ""))
+    for alias, embedding_model in get_embedding_model_aliases().items():
+        if alias != embedding_model.model_id:
+            to_output.append((alias, embedding_model.model_id, "embedding"))
     if json_:
-        click.echo(json.dumps({key: value for key, value in to_output}, indent=4))
+        click.echo(
+            json.dumps({key: value for key, value, type_ in to_output}, indent=4)
+        )
         return
-    max_alias_length = max(len(a) for a, _ in to_output)
-    fmt = "{alias:<" + str(max_alias_length) + "} : {model_id}"
-    for alias, model_id in to_output:
-        click.echo(fmt.format(alias=alias, model_id=model_id))
+    max_alias_length = max(len(a) for a, _, _ in to_output)
+    fmt = "{alias:<" + str(max_alias_length) + "} : {model_id}{type_}"
+    for alias, model_id, type_ in to_output:
+        click.echo(
+            fmt.format(
+                alias=alias, model_id=model_id, type_=f" ({type_})" if type_ else ""
+            )
+        )
 
 
 @aliases.command(name="set")
 @click.argument("alias")
 @click.argument("model_id")
 def aliases_set(alias, model_id):
     """
@@ -881,21 +905,26 @@
 @click.option(
     "-c",
     "--content",
     help="Content to embed",
     type=click.Path(file_okay=True, allow_dash=False, dir_okay=False, writable=True),
 )
 @click.option(
+    "--metadata",
+    help="JSON object metadata to store",
+    callback=_validate_metadata_json,
+)
+@click.option(
     "format_",
     "-f",
     "--format",
     type=click.Choice(["json", "blob", "base64", "hex"]),
     help="Output format",
 )
-def embed(collection, id, input, model, store, database, content, format_):
+def embed(collection, id, input, model, store, database, content, metadata, format_):
     """Embed text and store or return the result"""
     if collection and not id:
         raise click.ClickException("Must provide both collection and id")
 
     if store and not collection:
         raise click.ClickException("Must provide collection when using --store")
 
@@ -906,24 +935,36 @@
         else:
             return sqlite_utils.Database(user_dir() / "embeddings.db")
 
     collection_obj = None
     model_obj = None
     if collection:
         db = get_db()
-        collection_obj = Collection(db, collection, model_id=model)
-        model_obj = collection_obj.model()
+        if Collection.exists(db, collection):
+            # Load existing collection and use its model
+            collection_obj = Collection(collection, db)
+            model_obj = collection_obj.model()
+        else:
+            # We will create a new one, but that means model is required
+            if not model:
+                model = get_default_embedding_model()
+                if model is None:
+                    raise click.ClickException(
+                        "You need to specify a model (no default model is set)"
+                    )
+            collection_obj = Collection(collection, db=db, model_id=model)
+            model_obj = collection_obj.model()
 
     if model_obj is None:
-        if not model:
-            model = get_default_embedding_model()
         try:
             model_obj = get_embedding_model(model)
-        except UnknownModelError as ex:
-            raise click.ClickException(str(ex))
+        except UnknownModelError:
+            raise click.ClickException(
+                "You need to specify a model (no default model is set)"
+            )
 
     show_output = True
     if collection and (format_ is None):
         show_output = False
 
     # Resolve input text
     if not content:
@@ -931,15 +972,15 @@
             # Read from stdin
             input = sys.stdin
         content = input.read()
     if not content:
         raise click.ClickException("No content provided")
 
     if collection_obj:
-        embedding = collection_obj.embed(id, content, store=store)
+        embedding = collection_obj.embed(id, content, metadata=metadata, store=store)
     else:
         embedding = model_obj.embed(content)
 
     if show_output:
         if format_ == "json" or format_ is None:
             click.echo(json.dumps(embedding))
         elif format_ == "blob":
@@ -948,14 +989,151 @@
             click.echo(base64.b64encode(encode(embedding)).decode("ascii"))
         elif format_ == "hex":
             click.echo(encode(embedding).hex())
 
 
 @cli.command()
 @click.argument("collection")
+@click.argument(
+    "input_path",
+    type=click.Path(exists=True, dir_okay=False, allow_dash=True, readable=True),
+    required=False,
+)
+@click.option(
+    "--format",
+    type=click.Choice(["json", "csv", "tsv", "nl"]),
+    help="Format of input file - defaults to auto-detect",
+)
+@click.option(
+    "--files",
+    type=(click.Path(file_okay=False, dir_okay=True, allow_dash=False), str),
+    multiple=True,
+    help="Embed files in this directory - specify directory and glob pattern",
+)
+@click.option("--sql", help="Read input using this SQL query")
+@click.option(
+    "--attach",
+    type=(str, click.Path(file_okay=True, dir_okay=False, allow_dash=False)),
+    multiple=True,
+    help="Additional databases to attach - specify alias and file path",
+)
+@click.option("--prefix", help="Prefix to add to the IDs", default="")
+@click.option("-m", "--model", help="Embedding model to use")
+@click.option("--store", is_flag=True, help="Store the text itself in the database")
+@click.option(
+    "-d",
+    "--database",
+    type=click.Path(file_okay=True, allow_dash=False, dir_okay=False, writable=True),
+    envvar="LLM_EMBEDDINGS_DB",
+)
+def embed_multi(
+    collection, input_path, format, files, sql, attach, prefix, model, store, database
+):
+    """
+    Store embeddings for multiple strings at once
+
+    Input can be CSV, TSV or a JSON list of objects.
+
+    The first column is treated as an ID - all other columns
+    are assumed to be text that should be concatenated together
+    in order to calculate the embeddings.
+
+    Input data can come from one of three sources:
+
+    \b
+    1. A CSV, JSON, TSV or JSON-nl file (including on standard input)
+    2. A SQL query against a SQLite database
+    3. A directory of files
+    """
+    if not input_path and not sql and not files:
+        raise click.UsageError("Either --sql or input path or --files is required")
+
+    if files:
+        if input_path or sql or format:
+            raise click.UsageError(
+                "Cannot use --files with --sql, input path or --format"
+            )
+
+    if database:
+        db = sqlite_utils.Database(database)
+    else:
+        db = sqlite_utils.Database(user_dir() / "embeddings.db")
+
+    for alias, attach_path in attach:
+        db.attach(alias, attach_path)
+
+    try:
+        collection_obj = Collection(
+            collection, db=db, model_id=model or get_default_embedding_model()
+        )
+    except ValueError:
+        raise click.ClickException(
+            "You need to specify a model (no default model is set)"
+        )
+
+    expected_length = None
+    if files:
+
+        def count_files():
+            i = 0
+            for directory, pattern in files:
+                for path in pathlib.Path(directory).glob(pattern):
+                    i += 1
+            return i
+
+        def iterate_files():
+            for directory, pattern in files:
+                for path in pathlib.Path(directory).glob(pattern):
+                    relative = path.relative_to(directory)
+                    yield {"id": str(relative), "content": path.read_text()}
+
+        expected_length = count_files()
+        rows = iterate_files()
+    elif sql:
+        rows = db.query(sql)
+        count_sql = "select count(*) as c from ({})".format(sql)
+        expected_length = next(db.query(count_sql))["c"]
+    else:
+
+        def load_rows(fp):
+            return rows_from_file(fp, Format[format.upper()] if format else None)[0]
+
+        try:
+            if input_path != "-":
+                # Read the file twice - first time is to get a count
+                expected_length = 0
+                with open(input_path, "rb") as fp:
+                    for _ in load_rows(fp):
+                        expected_length += 1
+
+            rows = load_rows(
+                open(input_path, "rb")
+                if input_path != "-"
+                else io.BufferedReader(sys.stdin.buffer)
+            )
+        except json.JSONDecodeError as ex:
+            raise click.ClickException(str(ex))
+
+    with click.progressbar(
+        rows, label="Embedding", show_percent=True, length=expected_length
+    ) as rows:
+
+        def tuples():
+            for row in rows:
+                values = list(row.values())
+                id = prefix + str(values[0])
+                text = " ".join(v or "" for v in values[1:])
+                yield id, text
+
+        # collection_obj.max_batch_size = 1
+        collection_obj.embed_multi(tuples(), store=store)
+
+
+@cli.command()
+@click.argument("collection")
 @click.argument("id", required=False)
 @click.option(
     "-i",
     "--input",
     type=click.File("r"),
     help="File to embed for comparison",
 )
@@ -991,15 +1169,15 @@
     else:
         db = sqlite_utils.Database(user_dir() / "embeddings.db")
 
     if not db["embeddings"].exists():
         raise click.ClickException("No embeddings table found in database")
 
     try:
-        collection_obj = Collection(db, collection, create=False)
+        collection_obj = Collection(collection, db, create=False)
     except Collection.DoesNotExist:
         raise click.ClickException("Collection does not exist")
 
     if id:
         try:
             results = collection_obj.similar_by_id(id, number)
         except Collection.DoesNotExist:
@@ -1037,23 +1215,33 @@
             s += " (aliases: {})".format(", ".join(model_with_aliases.aliases))
         output.append(s)
     click.echo("\n".join(output))
 
 
 @embed_models.command(name="default")
 @click.argument("model", required=False)
-def embed_models_default(model):
+@click.option(
+    "--remove-default", is_flag=True, help="Reset to specifying no default model"
+)
+def embed_models_default(model, remove_default):
     "Show or set the default embedding model"
-    if not model:
-        click.echo(get_default_embedding_model())
+    if not model and not remove_default:
+        default = get_default_embedding_model()
+        if default is None:
+            click.echo("<No default embedding model set>", err=True)
+        else:
+            click.echo(default)
         return
     # Validate it is a known model
     try:
-        model = get_embedding_model(model)
-        set_default_embedding_model(model.model_id)
+        if remove_default:
+            set_default_embedding_model(None)
+        else:
+            model = get_embedding_model(model)
+            set_default_embedding_model(model.model_id)
     except KeyError:
         raise click.ClickException("Unknown embedding model: {}".format(model))
 
 
 @cli.group()
 def embed_db():
     "Manage the embeddings database"
@@ -1101,14 +1289,41 @@
             click.echo(
                 "  {} embedding{}".format(
                     row["num_embeddings"], "s" if row["num_embeddings"] != 1 else ""
                 )
             )
 
 
+@embed_db.command(name="delete-collection")
+@click.argument("collection")
+@click.option(
+    "-d",
+    "--database",
+    type=click.Path(file_okay=True, allow_dash=False, dir_okay=False, writable=True),
+    envvar="LLM_EMBEDDINGS_DB",
+    help="Path to embeddings database",
+)
+def embed_db_delete_collection(collection, database):
+    """
+    Delete the specified collection
+
+    Example usage:
+
+    \b
+        llm embed-db delete-collection my-collection
+    """
+    database = database or (user_dir() / "embeddings.db")
+    db = sqlite_utils.Database(str(database))
+    try:
+        collection_obj = Collection(collection, db, create=False)
+    except Collection.DoesNotExist:
+        raise click.ClickException("Collection does not exist")
+    collection_obj.delete()
+
+
 def template_dir():
     path = user_dir() / "templates"
     path.mkdir(parents=True, exist_ok=True)
     return path
 
 
 def _truncate_string(s, max_length=100):
@@ -1123,19 +1338,22 @@
         return path.read_text().strip()
     else:
         return default
 
 
 def set_default_model(model, filename="default_model.txt"):
     path = user_dir() / filename
-    path.write_text(model)
+    if model is None and path.exists():
+        path.unlink()
+    else:
+        path.write_text(model)
 
 
 def get_default_embedding_model():
-    return get_default_model("default_embedding_model.txt", DEFAULT_EMBEDDING_MODEL)
+    return get_default_model("default_embedding_model.txt", None)
 
 
 def set_default_embedding_model(model):
     set_default_model(model, "default_embedding_model.txt")
 
 
 def logs_db_path():
```

### Comparing `llm-0.9a0/llm/default_plugins/openai_models.py` & `llm-0.9a1/llm/default_plugins/openai_models.py`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/llm/embeddings.py` & `llm-0.9a1/llm/embeddings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from .models import EmbeddingModel
 from .embeddings_migrations import embeddings_migrations
 from dataclasses import dataclass
+import hashlib
 from itertools import islice
 import json
 from sqlite_utils import Database
 from sqlite_utils.db import Table
+import time
 from typing import cast, Any, Dict, Iterable, List, Optional, Tuple
 
 
 @dataclass
 class Entry:
     id: str
     score: Optional[float]
@@ -20,16 +22,16 @@
     max_batch_size: int = 100
 
     class DoesNotExist(Exception):
         pass
 
     def __init__(
         self,
-        db: Database,
         name: str,
+        db: Optional[Database] = None,
         *,
         model: Optional[EmbeddingModel] = None,
         model_id: Optional[str] = None,
         create: bool = True,
     ) -> None:
         """
         A collection of embeddings
@@ -44,27 +46,32 @@
             name (str): Name of the collection
             model (llm.models.EmbeddingModel, optional): Embedding model to use
             model_id (str, optional): Alternatively, ID of the embedding model to use
             create (bool, optional): Whether to create the collection if it does not exist
         """
         import llm
 
-        self.db = db
+        self.db = db or Database(memory=True)
         self.name = name
         self._model = model
 
         embeddings_migrations.apply(self.db)
 
         rows = list(self.db["collections"].rows_where("name = ?", [self.name]))
         if rows:
             row = rows[0]
             self.id = row["id"]
             self.model_id = row["model"]
         else:
             if create:
+                # Collection does not exist, so model or model_id is required
+                if not model and not model_id:
+                    raise ValueError(
+                        "Either model= or model_id= must be provided when creating a new collection"
+                    )
                 # Create it
                 if model_id:
                     # Resolve alias
                     model = llm.get_embedding_model(model_id)
                     self._model = model
                 model_id = cast(EmbeddingModel, model).model_id
                 self.id = (
@@ -121,22 +128,29 @@
             id (str): ID for the text
             text (str): Text to be embedded
             metadata (dict, optional): Metadata to be stored
             store (bool, optional): Whether to store the text in the content column
         """
         from llm import encode
 
+        content_hash = self.content_hash(text)
+        if self.db["embeddings"].count_where(
+            "content_hash = ? and collection_id = ?", [content_hash, self.id]
+        ):
+            return
         embedding = self.model().embed(text)
         cast(Table, self.db["embeddings"]).insert(
             {
                 "collection_id": self.id,
                 "id": id,
                 "embedding": encode(embedding),
                 "content": text if store else None,
+                "content_hash": content_hash,
                 "metadata": json.dumps(metadata) if metadata else None,
+                "updated": int(time.time()),
             },
             replace=True,
         )
 
     def embed_multi(
         self, entries: Iterable[Tuple[str, str]], store: bool = False
     ) -> None:
@@ -170,26 +184,49 @@
         )
         iterator = iter(entries)
         collection_id = self.id
         while True:
             batch = list(islice(iterator, batch_size))
             if not batch:
                 break
-            embeddings = list(self.model().embed_multi(item[1] for item in batch))
+            # Calculate hashes first
+            items_and_hashes = [(item, self.content_hash(item[1])) for item in batch]
+            # Any of those hashes already exist?
+            existing_ids = [
+                row["id"]
+                for row in self.db.query(
+                    """
+                    select id from embeddings
+                    where collection_id = ? and content_hash in ({})
+                    """.format(
+                        ",".join("?" for _ in items_and_hashes)
+                    ),
+                    [collection_id]
+                    + [item_and_hash[1] for item_and_hash in items_and_hashes],
+                )
+            ]
+            filtered_batch = [item for item in batch if item[0] not in existing_ids]
+            embeddings = list(
+                self.model().embed_multi(item[1] for item in filtered_batch)
+            )
             with self.db.conn:
                 cast(Table, self.db["embeddings"]).insert_all(
                     (
                         {
                             "collection_id": collection_id,
                             "id": id,
                             "embedding": llm.encode(embedding),
                             "content": text if store else None,
+                            "content_hash": self.content_hash(text),
                             "metadata": json.dumps(metadata) if metadata else None,
+                            "updated": int(time.time()),
                         }
-                        for (embedding, (id, text, metadata)) in zip(embeddings, batch)
+                        for (embedding, (id, text, metadata)) in zip(
+                            embeddings, filtered_batch
+                        )
                     ),
                     replace=True,
                 )
 
     def similar_by_vector(
         self, vector: List[float], number: int = 10, skip_id: Optional[str] = None
     ) -> List[Entry]:
@@ -272,7 +309,31 @@
             number (int, optional): Number of similar items to return
 
         Returns:
             list: List of Entry objects
         """
         comparison_vector = self.model().embed(text)
         return self.similar_by_vector(comparison_vector, number)
+
+    @classmethod
+    def exists(cls, db: Database, name: str) -> bool:
+        """
+        Does this collection exist in the database?
+
+        Args:
+            name (str): Name of the collection
+        """
+        rows = list(db["collections"].rows_where("name = ?", [name]))
+        return bool(rows)
+
+    def delete(self):
+        """
+        Delete the collection and its embeddings from the database
+        """
+        with self.db.conn:
+            self.db.execute("delete from embeddings where collection_id = ?", [self.id])
+            self.db.execute("delete from collections where id = ?", [self.id])
+
+    @staticmethod
+    def content_hash(text: str) -> bytes:
+        "Hash content for deduplication. Override to change hashing behavior."
+        return hashlib.md5(text.encode("utf8")).digest()
```

### Comparing `llm-0.9a0/llm/migrations.py` & `llm-0.9a1/llm/migrations.py`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/llm/models.py` & `llm-0.9a1/llm/models.py`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/llm/templates.py` & `llm-0.9a1/llm/templates.py`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/llm/utils.py` & `llm-0.9a1/llm/utils.py`

 * *Files identical despite different names*

### Comparing `llm-0.9a0/llm.egg-info/PKG-INFO` & `llm-0.9a1/llm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm
-Version: 0.9a0
+Version: 0.9a1
 Summary: A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 Home-page: https://github.com/simonw/llm
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://llm.datasette.io/
 Project-URL: Issues, https://github.com/simonw/llm/issues
 Project-URL: CI, https://github.com/simonw/llm/actions
@@ -18,14 +18,15 @@
 
 [![PyPI](https://img.shields.io/pypi/v/llm.svg)](https://pypi.org/project/llm/)
 [![Documentation](https://readthedocs.org/projects/llm/badge/?version=latest)](https://llm.datasette.io/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/llm?include_prereleases&label=changelog)](https://llm.datasette.io/en/stable/changelog.html)
 [![Tests](https://github.com/simonw/llm/workflows/Test/badge.svg)](https://github.com/simonw/llm/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/llm/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/823971286308356157?label=discord)](https://datasette.io/discord-llm)
+[![Homebrew](https://img.shields.io/homebrew/installs/dy/llm?color=yellow&label=homebrew&logo=homebrew)](https://formulae.brew.sh/formula/llm)
 
 A CLI utility and Python library for interacting with Large Language Models, including OpenAI, PaLM and local models installed on your own machine.
 
 Full documentation: **[llm.datasette.io](https://llm.datasette.io/)**
 
 Background on this project:
 - [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/)
```

### Comparing `llm-0.9a0/setup.py` & `llm-0.9a1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = "0.9a0"
+VERSION = "0.9a1"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -36,15 +36,15 @@
         llm=llm.cli:cli
     """,
     install_requires=[
         "click",
         "openai",
         "click-default-group-wheel",
         "sqlite-utils>=3.35.0",
-        "sqlite-migrate",
+        "sqlite-migrate>=0.1a2",
         "pydantic>=1.10.2",
         "PyYAML",
         "pluggy",
         "python-ulid",
         "setuptools",
         "pip",
     ],
```

