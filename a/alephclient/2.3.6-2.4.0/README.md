# Comparing `tmp/alephclient-2.3.6.tar.gz` & `tmp/alephclient-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alephclient-2.3.6.tar", last modified: Wed Jun 28 11:41:48 2023, max compression
+gzip compressed data, was "alephclient-2.4.0.tar", last modified: Mon May 13 11:14:41 2024, max compression
```

## Comparing `alephclient-2.3.6.tar` & `alephclient-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:41:48.718828 alephclient-2.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-28 11:41:30.000000 alephclient-2.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-28 11:41:48.718828 alephclient-2.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-28 11:41:30.000000 alephclient-2.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:41:48.718828 alephclient-2.3.6/alephclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/crawldir.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/fetchdir.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-28 11:41:30.000000 alephclient-2.3.6/alephclient/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 11:41:48.718828 alephclient-2.3.6/alephclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 11:41:48.000000 alephclient-2.3.6/alephclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-28 11:41:48.718828 alephclient-2.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-28 11:41:30.000000 alephclient-2.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:14:41.348843 alephclient-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-13 11:14:24.000000 alephclient-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 11:14:41.348843 alephclient-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-13 11:14:24.000000 alephclient-2.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:14:41.348843 alephclient-2.4.0/alephclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/crawldir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/fetchdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 11:14:24.000000 alephclient-2.4.0/alephclient/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 11:14:41.348843 alephclient-2.4.0/alephclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 11:14:41.000000 alephclient-2.4.0/alephclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 11:14:41.352844 alephclient-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 11:14:24.000000 alephclient-2.4.0/setup.py
```

### Comparing `alephclient-2.3.6/LICENSE` & `alephclient-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alephclient-2.3.6/alephclient/api.py` & `alephclient-2.4.0/alephclient/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+import importlib
 import json
 import uuid
 import logging
-import pkg_resources
 from itertools import count
 from pathlib import Path
 from urllib.parse import urlencode, urljoin
 from banal import ensure_dict, ensure_list
 from requests import RequestException, Session
 from requests.exceptions import HTTPError
 from requests_toolbelt import MultipartEncoder  # type: ignore
@@ -13,15 +13,15 @@
 
 from alephclient import settings
 from alephclient.errors import AlephException
 from alephclient.util import backoff, prop_push
 
 log = logging.getLogger(__name__)
 MIME = "application/octet-stream"
-VERSION = pkg_resources.get_distribution("alephclient").version
+VERSION = importlib.metadata.version("alephclient")
 
 
 class APIResultSet(object):
     def __init__(self, api: "AlephAPI", url: str):
         self.api = api
         self.url = url
         self.current = 0
@@ -222,14 +222,19 @@
 
     def get_entity(self, entity_id: str, publisher: bool = False) -> Dict:
         """Get a single entity by ID."""
         url = self._make_url(f"entities/{entity_id}")
         entity = self._request("GET", url)
         return self._patch_entity(entity, publisher)
 
+    def delete_entity(self, entity_id: str) -> Dict:
+        """Delete a single entity by ID."""
+        url = self._make_url(f"entities/{entity_id}")
+        return self._request("DELETE", url)
+
     def get_collection_by_foreign_id(self, foreign_id: str) -> Optional[Dict]:
         """Get a dict representing a collection based on its foreign ID."""
         if foreign_id is None:
             return None
         filters = [("foreign_id", foreign_id)]
         for coll in self.filter_collections(filters=filters):
             return coll
@@ -333,18 +338,23 @@
     def _bulk_chunk(
         self,
         collection_id: str,
         chunk: List,
         entityset_id: Optional[str] = None,
         force: bool = False,
         unsafe: bool = False,
+        cleaned: bool = False,
     ):
         for attempt in count(1):
             url = self._make_url(f"collections/{collection_id}/_bulk")
-            params = {"unsafe": unsafe, "entityset_id": entityset_id}
+            params = {"entityset_id": entityset_id}
+            if unsafe:
+                params["safe"] = "false"
+            if cleaned:
+                params["clean"] = "false"
             try:
                 response = self.session.post(url, json=chunk, params=params)
                 response.raise_for_status()
                 return
             except (RequestException, HTTPError) as exc:
                 ae = AlephException(exc)
                 if not ae.transient or attempt > self.retries:
```

### Comparing `alephclient-2.3.6/alephclient/cli.py` & `alephclient-2.4.0/alephclient/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     "-p",
     "--parallel",
     default=1,
     show_default=True,
     type=click.IntRange(1),
     help="maximum number of parallel uploads",
 )
-@click.option("-f", "--foreign-id", required=True, help="foreign_id of the collection")
+@click.option("-f", "--foreign-id", required=True, help="foreign-id of the collection")
 @click.argument("path", type=click.Path(exists=True))
 @click.pass_context
 def crawldir(
     ctx,
     path,
     foreign_id,
     language=None,
@@ -233,14 +233,27 @@
         )
     except AlephException as exc:
         raise click.ClickException(exc.message)
     except BrokenPipeError:
         raise click.Abort()
 
 
+@cli.command("delete-entity")
+@click.argument("entity_id", required=True)
+@click.pass_context
+def delete_entity(ctx, entity_id):
+    """Delete a single entity from standard input"""
+    api = ctx.obj['api']
+    entity_id = entity_id.strip()
+    try:
+        api.delete_entity(entity_id)
+    except Exception as exc:
+        raise click.ClickException(exc.message)
+
+
 @cli.command("write-entities")
 @click.option("-i", "--infile", type=click.File("r"), default="-")
 @click.option("-f", "--foreign-id", required=True, help="foreign_id of the collection")
 @click.option(
     "-e", "--entityset", "entityset_id", help="add entities to the given entity set"
 )
 @click.option(
@@ -250,25 +263,29 @@
     type=click.INT,
     help="chunk size when sending to API",
 )
 @click.option(
     "--force", is_flag=True, default=False, help="continue after server errors"
 )
 @click.option(
-    "--unsafe", is_flag=True, default=False, help="disable server-side validation"
+    "--unsafe", is_flag=True, default=False, help="allow references to archive hashes"
+)
+@click.option(
+    "--cleaned", is_flag=True, default=False, help="disable server-side validation for all types"
 )
 @click.pass_context
 def write_entities(
     ctx,
     infile,
     foreign_id,
     entityset_id=None,
     chunksize=1000,
     force=False,
     unsafe=False,
+    cleaned=False
 ):
     """Read entities from standard input and index them."""
     api = ctx.obj["api"]
     try:
         collection = api.load_collection_by_foreign_id(foreign_id)
 
         def read_json_stream(stream):
@@ -284,14 +301,15 @@
 
         api.write_entities(
             collection.get("id"),
             read_json_stream(infile),
             chunk_size=chunksize,
             unsafe=unsafe,
             force=force,
+            cleaned=cleaned,
             entityset_id=entityset_id,
         )
     except AlephException as exc:
         raise click.ClickException(exc.message)
     except BrokenPipeError:
         raise click.Abort()
```

### Comparing `alephclient-2.3.6/alephclient/crawldir.py` & `alephclient-2.4.0/alephclient/crawldir.py`

 * *Files identical despite different names*

### Comparing `alephclient-2.3.6/alephclient/errors.py` & `alephclient-2.4.0/alephclient/errors.py`

 * *Files identical despite different names*

### Comparing `alephclient-2.3.6/alephclient/fetchdir.py` & `alephclient-2.4.0/alephclient/fetchdir.py`

 * *Files identical despite different names*

### Comparing `alephclient-2.3.6/alephclient/util.py` & `alephclient-2.4.0/alephclient/util.py`

 * *Files identical despite different names*

### Comparing `alephclient-2.3.6/setup.py` & `alephclient-2.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="alephclient",
-    version="2.3.6",
+    version="2.4.0",
     description="Command-line client for Aleph API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="http://github.com/alephdata/alephclient",
     license="MIT",
@@ -30,13 +30,15 @@
     ],
     extras_require={
         "dev": [
             "mypy",
             "wheel",
             "pytest",
             "pytest-mock >= 1.10.0",
+            "types-requests",
+            "types-setuptools",
         ]
     },
     entry_points={
         "console_scripts": ["alephclient = alephclient.cli:cli"],
     },
 )
```

