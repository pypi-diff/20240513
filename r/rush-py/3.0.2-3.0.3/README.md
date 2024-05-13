# Comparing `tmp/rush_py-3.0.2.tar.gz` & `tmp/rush_py-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rush_py-3.0.2.tar", max compression
+gzip compressed data, was "rush_py-3.0.3.tar", max compression
```

## Comparing `rush_py-3.0.2.tar` & `rush_py-3.0.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     9914 2024-04-14 07:42:20.019580 rush_py-3.0.2/README.md
--rw-r--r--   0        0        0     2769 2024-05-06 08:49:16.695069 rush_py-3.0.2/pyproject.toml
--rw-r--r--   0        0        0      481 2024-03-25 07:43:11.134075 rush_py-3.0.2/rush/__init__.py
--rw-r--r--   0        0        0     1965 2024-04-25 04:28:44.728279 rush_py-3.0.2/rush/async_utils.py
--rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.2/rush/data.py
--rw-r--r--   0        0        0     1326 2024-04-17 04:40:42.341556 rush_py-3.0.2/rush/doc.py
--rw-r--r--   0        0        0     7663 2024-04-16 06:00:37.048276 rush_py-3.0.2/rush/graphql_client/__init__.py
--rw-r--r--   0        0        0      267 2024-04-16 06:00:36.589255 rush_py-3.0.2/rush/graphql_client/argument.py
--rw-r--r--   0        0        0     1036 2024-04-16 06:00:36.599256 rush_py-3.0.2/rush/graphql_client/arguments.py
--rw-r--r--   0        0        0    12272 2024-04-17 02:47:58.375356 rush_py-3.0.2/rush/graphql_client/async_base_client.py
--rw-r--r--   0        0        0      620 2024-04-16 06:00:36.758263 rush_py-3.0.2/rush/graphql_client/base_model.py
--rw-r--r--   0        0        0      174 2024-04-16 06:00:36.547253 rush_py-3.0.2/rush/graphql_client/cancel_module_instance.py
--rw-r--r--   0        0        0    28860 2024-04-17 02:47:58.496361 rush_py-3.0.2/rush/graphql_client/client.py
--rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.2/rush/graphql_client/create_entity.py
--rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.2/rush/graphql_client/create_experiment.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.2/rush/graphql_client/create_project.py
--rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.2/rush/graphql_client/create_protein.py
--rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.2/rush/graphql_client/create_protein_conformer.py
--rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.2/rush/graphql_client/create_smol.py
--rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.2/rush/graphql_client/create_smol_conformer.py
--rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.2/rush/graphql_client/create_smol_tautomer.py
--rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.2/rush/graphql_client/create_structure.py
--rw-r--r--   0        0        0      341 2024-04-16 06:00:36.551254 rush_py-3.0.2/rush/graphql_client/delete_module_instance.py
--rw-r--r--   0        0        0      255 2024-04-16 06:00:36.554254 rush_py-3.0.2/rush/graphql_client/deploy.py
--rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.2/rush/graphql_client/entity.py
--rw-r--r--   0        0        0     1477 2024-04-17 04:40:42.341556 rush_py-3.0.2/rush/graphql_client/enums.py
--rw-r--r--   0        0        0     2411 2024-04-16 06:00:36.757263 rush_py-3.0.2/rush/graphql_client/exceptions.py
--rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.2/rush/graphql_client/experiment.py
--rw-r--r--   0        0        0     3769 2024-04-16 06:00:36.757263 rush_py-3.0.2/rush/graphql_client/fragments.py
--rw-r--r--   0        0        0     5332 2024-04-16 06:00:36.545253 rush_py-3.0.2/rush/graphql_client/input_types.py
--rw-r--r--   0        0        0      825 2024-04-16 06:00:36.607256 rush_py-3.0.2/rush/graphql_client/latest_modules.py
--rw-r--r--   0        0        0     2004 2024-04-17 02:47:58.096344 rush_py-3.0.2/rush/graphql_client/module_instance_details.py
--rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.2/rush/graphql_client/module_instance_full.py
--rw-r--r--   0        0        0      354 2024-04-16 06:00:36.634257 rush_py-3.0.2/rush/graphql_client/module_instance_minimal.py
--rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.2/rush/graphql_client/module_instance_status.py
--rw-r--r--   0        0        0     3104 2024-04-17 02:47:58.134345 rush_py-3.0.2/rush/graphql_client/module_instances.py
--rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.2/rush/graphql_client/module_instances_full.py
--rw-r--r--   0        0        0      686 2024-04-16 06:00:36.615257 rush_py-3.0.2/rush/graphql_client/modules.py
--rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.2/rush/graphql_client/object.py
--rw-r--r--   0        0        0      292 2024-04-16 06:00:36.640258 rush_py-3.0.2/rush/graphql_client/object_contents.py
--rw-r--r--   0        0        0      243 2024-04-16 06:00:36.637258 rush_py-3.0.2/rush/graphql_client/object_url.py
--rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.2/rush/graphql_client/project.py
--rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.2/rush/graphql_client/protein.py
--rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.2/rush/graphql_client/protein_conformer.py
--rw-r--r--   0        0        0      234 2024-04-16 06:00:36.643258 rush_py-3.0.2/rush/graphql_client/retry.py
--rw-r--r--   0        0        0      340 2024-04-16 06:00:36.649258 rush_py-3.0.2/rush/graphql_client/run.py
--rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.2/rush/graphql_client/smol.py
--rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.2/rush/graphql_client/smol_conformer.py
--rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.2/rush/graphql_client/smol_tautomer.py
--rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.2/rush/graphql_client/structure.py
--rw-r--r--   0        0        0      161 2024-04-16 06:00:36.651258 rush_py-3.0.2/rush/graphql_client/tag.py
--rw-r--r--   0        0        0      381 2024-04-16 06:00:36.655259 rush_py-3.0.2/rush/graphql_client/track_utilization.py
--rw-r--r--   0        0        0      165 2024-04-16 06:00:36.658259 rush_py-3.0.2/rush/graphql_client/untag.py
--rw-r--r--   0        0        0      414 2024-04-16 06:00:36.681260 rush_py-3.0.2/rush/graphql_client/update_module_instance.py
--rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.2/rush/graphql_client/upload.py
--rw-r--r--   0        0        0      321 2024-04-16 06:00:36.685260 rush_py-3.0.2/rush/graphql_client/upload_arg.py
--rw-r--r--   0        0        0      506 2024-04-16 06:00:36.691260 rush_py-3.0.2/rush/graphql_client/upload_object.py
--rw-r--r--   0        0        0     1226 2024-03-25 07:43:11.134075 rush_py-3.0.2/rush/legacy_types.py
--rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.2/rush/local.py
--rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.2/rush/protocols.py
--rw-r--r--   0        0        0    66188 2024-05-06 07:32:38.957574 rush_py-3.0.2/rush/provider.py
--rw-r--r--   0        0        0      300 2024-04-25 04:28:44.729279 rush_py-3.0.2/rush/tests/test_provider.py
--rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.2/rush/tests/test_typedef.py
--rw-r--r--   0        0        0    10193 2024-04-12 08:48:59.536260 rush_py-3.0.2/rush/typedef.py
--rw-r--r--   0        0        0      747 2024-04-07 11:51:36.271482 rush_py-3.0.2/rush/types.py
--rw-r--r--   0        0        0    10796 1970-01-01 00:00:00.000000 rush_py-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0    10746 2024-05-13 08:03:28.789167 rush_py-3.0.3/README.md
+-rw-r--r--   0        0        0     2809 2024-05-13 08:04:04.072836 rush_py-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0      481 2024-05-12 08:15:13.090389 rush_py-3.0.3/rush/__init__.py
+-rw-r--r--   0        0        0     1965 2024-05-12 08:15:13.090389 rush_py-3.0.3/rush/async_utils.py
+-rw-r--r--   0        0        0       23 2024-01-29 10:45:57.136914 rush_py-3.0.3/rush/data.py
+-rw-r--r--   0        0        0     1353 2024-05-12 08:16:05.403773 rush_py-3.0.3/rush/doc.py
+-rw-r--r--   0        0        0     7663 2024-05-12 08:15:13.090389 rush_py-3.0.3/rush/graphql_client/__init__.py
+-rw-r--r--   0        0        0      267 2024-05-12 08:15:13.090389 rush_py-3.0.3/rush/graphql_client/argument.py
+-rw-r--r--   0        0        0     1036 2024-05-12 08:15:13.090389 rush_py-3.0.3/rush/graphql_client/arguments.py
+-rw-r--r--   0        0        0    12381 2024-05-12 08:16:05.403773 rush_py-3.0.3/rush/graphql_client/async_base_client.py
+-rw-r--r--   0        0        0      620 2024-04-16 06:00:36.758263 rush_py-3.0.3/rush/graphql_client/base_model.py
+-rw-r--r--   0        0        0      174 2024-04-16 06:00:36.547253 rush_py-3.0.3/rush/graphql_client/cancel_module_instance.py
+-rw-r--r--   0        0        0    28860 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/client.py
+-rw-r--r--   0        0        0      253 2024-02-28 07:01:47.459725 rush_py-3.0.3/rush/graphql_client/create_entity.py
+-rw-r--r--   0        0        0      277 2024-02-28 07:01:47.461725 rush_py-3.0.3/rush/graphql_client/create_experiment.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.463725 rush_py-3.0.3/rush/graphql_client/create_project.py
+-rw-r--r--   0        0        0      259 2024-02-28 07:01:47.467725 rush_py-3.0.3/rush/graphql_client/create_protein.py
+-rw-r--r--   0        0        0      314 2024-02-28 07:01:47.465725 rush_py-3.0.3/rush/graphql_client/create_protein_conformer.py
+-rw-r--r--   0        0        0      241 2024-02-28 07:01:47.566729 rush_py-3.0.3/rush/graphql_client/create_smol.py
+-rw-r--r--   0        0        0      296 2024-02-28 07:01:47.564729 rush_py-3.0.3/rush/graphql_client/create_smol_conformer.py
+-rw-r--r--   0        0        0      290 2024-02-28 07:01:47.568729 rush_py-3.0.3/rush/graphql_client/create_smol_tautomer.py
+-rw-r--r--   0        0        0      271 2024-02-28 07:01:47.570730 rush_py-3.0.3/rush/graphql_client/create_structure.py
+-rw-r--r--   0        0        0      341 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/delete_module_instance.py
+-rw-r--r--   0        0        0      255 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/deploy.py
+-rw-r--r--   0        0        0      510 2024-02-28 07:01:47.506727 rush_py-3.0.3/rush/graphql_client/entity.py
+-rw-r--r--   0        0        0     1477 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/enums.py
+-rw-r--r--   0        0        0     2411 2024-04-16 06:00:36.757263 rush_py-3.0.3/rush/graphql_client/exceptions.py
+-rw-r--r--   0        0        0      679 2024-02-28 07:01:47.557729 rush_py-3.0.3/rush/graphql_client/experiment.py
+-rw-r--r--   0        0        0     3769 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/fragments.py
+-rw-r--r--   0        0        0     5332 2024-05-12 08:15:13.091389 rush_py-3.0.3/rush/graphql_client/input_types.py
+-rw-r--r--   0        0        0      825 2024-05-12 08:15:13.092389 rush_py-3.0.3/rush/graphql_client/latest_modules.py
+-rw-r--r--   0        0        0     2004 2024-05-12 08:15:13.092389 rush_py-3.0.3/rush/graphql_client/module_instance_details.py
+-rw-r--r--   0        0        0     4300 2024-01-29 10:45:57.143915 rush_py-3.0.3/rush/graphql_client/module_instance_full.py
+-rw-r--r--   0        0        0      354 2024-05-12 08:15:13.092389 rush_py-3.0.3/rush/graphql_client/module_instance_minimal.py
+-rw-r--r--   0        0        0      403 2024-01-29 10:45:57.144914 rush_py-3.0.3/rush/graphql_client/module_instance_status.py
+-rw-r--r--   0        0        0     3104 2024-05-12 08:15:13.092389 rush_py-3.0.3/rush/graphql_client/module_instances.py
+-rw-r--r--   0        0        0     2804 2024-01-29 10:45:57.145915 rush_py-3.0.3/rush/graphql_client/module_instances_full.py
+-rw-r--r--   0        0        0      686 2024-05-12 08:15:13.092389 rush_py-3.0.3/rush/graphql_client/modules.py
+-rw-r--r--   0        0        0      160 2024-02-13 05:21:55.039019 rush_py-3.0.3/rush/graphql_client/object.py
+-rw-r--r--   0        0        0      292 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/object_contents.py
+-rw-r--r--   0        0        0      243 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/object_url.py
+-rw-r--r--   0        0        0     2121 2024-02-28 07:01:47.518727 rush_py-3.0.3/rush/graphql_client/project.py
+-rw-r--r--   0        0        0      604 2024-02-28 07:01:47.523728 rush_py-3.0.3/rush/graphql_client/protein.py
+-rw-r--r--   0        0        0      687 2024-02-28 07:01:47.528728 rush_py-3.0.3/rush/graphql_client/protein_conformer.py
+-rw-r--r--   0        0        0      234 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/retry.py
+-rw-r--r--   0        0        0      340 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/run.py
+-rw-r--r--   0        0        0      571 2024-02-28 07:01:47.533728 rush_py-3.0.3/rush/graphql_client/smol.py
+-rw-r--r--   0        0        0      657 2024-02-28 07:01:47.537728 rush_py-3.0.3/rush/graphql_client/smol_conformer.py
+-rw-r--r--   0        0        0      662 2024-02-28 07:01:47.543728 rush_py-3.0.3/rush/graphql_client/smol_tautomer.py
+-rw-r--r--   0        0        0     1139 2024-02-28 07:01:47.551729 rush_py-3.0.3/rush/graphql_client/structure.py
+-rw-r--r--   0        0        0      161 2024-04-16 06:00:36.651258 rush_py-3.0.3/rush/graphql_client/tag.py
+-rw-r--r--   0        0        0      381 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/track_utilization.py
+-rw-r--r--   0        0        0      165 2024-04-16 06:00:36.658259 rush_py-3.0.3/rush/graphql_client/untag.py
+-rw-r--r--   0        0        0      414 2024-05-12 08:15:13.093389 rush_py-3.0.3/rush/graphql_client/update_module_instance.py
+-rw-r--r--   0        0        0      328 2024-01-29 10:45:57.148915 rush_py-3.0.3/rush/graphql_client/upload.py
+-rw-r--r--   0        0        0      321 2024-05-12 08:15:13.094389 rush_py-3.0.3/rush/graphql_client/upload_arg.py
+-rw-r--r--   0        0        0      506 2024-05-12 08:15:13.094389 rush_py-3.0.3/rush/graphql_client/upload_object.py
+-rw-r--r--   0        0        0     1226 2024-05-12 08:15:13.094389 rush_py-3.0.3/rush/legacy_types.py
+-rw-r--r--   0        0        0     7403 2024-02-16 09:06:54.345722 rush_py-3.0.3/rush/local.py
+-rw-r--r--   0        0        0     5733 2024-02-16 09:06:54.345722 rush_py-3.0.3/rush/protocols.py
+-rw-r--r--   0        0        0    66330 2024-05-13 08:03:28.820169 rush_py-3.0.3/rush/provider.py
+-rw-r--r--   0        0        0      300 2024-05-12 08:15:13.094389 rush_py-3.0.3/rush/tests/test_provider.py
+-rw-r--r--   0        0        0     1070 2024-02-01 03:43:42.619708 rush_py-3.0.3/rush/tests/test_typedef.py
+-rw-r--r--   0        0        0    10193 2024-05-12 08:28:07.892647 rush_py-3.0.3/rush/typedef.py
+-rw-r--r--   0        0        0      747 2024-05-12 08:15:13.095389 rush_py-3.0.3/rush/types.py
+-rw-r--r--   0        0        0    11668 1970-01-01 00:00:00.000000 rush_py-3.0.3/PKG-INFO
```

### Comparing `rush_py-3.0.2/pyproject.toml` & `rush_py-3.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 [tool.poetry]
 name = "rush-py"
-version = "3.0.2"
+version = "3.0.3"
 description = "Python SDK for interacting with the QDX Rush API and modules"
 authors = ["Ryan Swart <ryan.swart@qdx.co>", "Sean Laguna <sean.laguna@qdx.co>"]
 readme = "README.md"
 packages = [{ include = "rush" }]
 documentation = "https://talo.github.io/rush-py"
 homepage = "https://rush.qdx.co"
 
 [tool.poetry.scripts]
 # rush = "rush.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
+
+aiofiles = "^23.2.1"
+backoff = "^2.2.1"
 httpx = "^0.26.0"
+nest-asyncio = "^1.6.0"
 pdb-tools = "^2.5.0"
 pydantic = "^2.6.0"
 typing-extensions = "^4.9.0"
 websockets = "^12"
-aiofiles = "^23.2.1"
-nest-asyncio = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
 ariadne-codegen = "0.13.0"
 black = { extras = ["jupyter"], version = "~=23.9.1" }
 flake8 = "~=6.1.0"
 isort = "~=5.12.0"
 jupyter-contrib-nbextensions = "^0.7.0"
@@ -35,14 +37,15 @@
 pip = "~=23.2.1"
 py3Dmol = "^2.0.4"
 pytest = "~=7.4.3"
 pytest-xdist = "~=3.3.1"
 qdx-py = ">0.6.2"
 pickleshare = "^0.7.5"
 jupyterlab-lsp = "^5.1.0"
+rdkit = "^2023.9.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool]
```

### Comparing `rush_py-3.0.2/rush/async_utils.py` & `rush_py-3.0.3/rush/async_utils.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/doc.py` & `rush_py-3.0.3/rush/doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3.12
 # flake8: noqa
-import asyncio
 from typing import Any as _Any
 
+from rush.async_utils import asyncio_run
+
 from . import provider, types
 
 type Any = _Any
 "@private"
 
 type Conformer = dict[str, Any]
 """ A Conformer represents a biochemical structure. It is documented in:  
@@ -33,13 +34,13 @@
 As an output argument, you can expect:
   - a URL for non-JSON files,
   - a `Conformer` or `Record` (i.e. `dict`) for JSON files, or
   - the expected containers or values for other types (`list`, `float`, et cetera).
 """
 
 _x = provider.Provider()
-_fns = asyncio.run(_x.get_module_functions(tags=["rush-py-v3.0.0"]))
+_fns = asyncio_run(_x.get_module_functions(tags=["rush-py-v3.0.0"]))
 RushProvider = type(
     "RushProvider",
     (provider.Provider,),
     _fns | {n: getattr(_x, n) for n in dir(_x)},
 )
```

### Comparing `rush_py-3.0.2/rush/graphql_client/__init__.py` & `rush_py-3.0.3/rush/graphql_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/arguments.py` & `rush_py-3.0.3/rush/graphql_client/arguments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/async_base_client.py` & `rush_py-3.0.3/rush/graphql_client/async_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Generated by ariadne-codegen
 
 import enum
 import json
 from typing import IO, Any, AsyncIterator, Dict, List, Optional, Tuple, TypeVar, cast
 from uuid import uuid4
 
+import backoff
 import httpx
 from pydantic import BaseModel
 from pydantic_core import to_jsonable_python
 
 from .base_model import UNSET, Upload
 from .exceptions import (
     GraphQLClientGraphQLMultiError,
@@ -86,14 +87,15 @@
         self,
         exc_type: object,
         exc_val: object,
         exc_tb: object,
     ) -> None:
         await self.http_client.aclose()
 
+    @backoff.on_exception(backoff.expo, (httpx.ReadTimeout, httpx.ConnectError), max_time=60)
     async def execute(
         self,
         query: str,
         operation_name: Optional[str] = None,
         variables: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> httpx.Response:
```

### Comparing `rush_py-3.0.2/rush/graphql_client/base_model.py` & `rush_py-3.0.3/rush/graphql_client/base_model.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/client.py` & `rush_py-3.0.3/rush/graphql_client/client.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/enums.py` & `rush_py-3.0.3/rush/graphql_client/enums.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/exceptions.py` & `rush_py-3.0.3/rush/graphql_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/experiment.py` & `rush_py-3.0.3/rush/graphql_client/experiment.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/fragments.py` & `rush_py-3.0.3/rush/graphql_client/fragments.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/input_types.py` & `rush_py-3.0.3/rush/graphql_client/input_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/latest_modules.py` & `rush_py-3.0.3/rush/graphql_client/latest_modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/module_instance_details.py` & `rush_py-3.0.3/rush/graphql_client/module_instance_details.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/module_instance_full.py` & `rush_py-3.0.3/rush/graphql_client/module_instance_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/module_instances.py` & `rush_py-3.0.3/rush/graphql_client/module_instances.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/module_instances_full.py` & `rush_py-3.0.3/rush/graphql_client/module_instances_full.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/modules.py` & `rush_py-3.0.3/rush/graphql_client/modules.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/project.py` & `rush_py-3.0.3/rush/graphql_client/project.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/protein.py` & `rush_py-3.0.3/rush/graphql_client/protein.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/protein_conformer.py` & `rush_py-3.0.3/rush/graphql_client/protein_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/smol.py` & `rush_py-3.0.3/rush/graphql_client/smol.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/smol_conformer.py` & `rush_py-3.0.3/rush/graphql_client/smol_conformer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/smol_tautomer.py` & `rush_py-3.0.3/rush/graphql_client/smol_tautomer.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/graphql_client/structure.py` & `rush_py-3.0.3/rush/graphql_client/structure.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/legacy_types.py` & `rush_py-3.0.3/rush/legacy_types.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/local.py` & `rush_py-3.0.3/rush/local.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/protocols.py` & `rush_py-3.0.3/rush/protocols.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/provider.py` & `rush_py-3.0.3/rush/provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,19 +503,22 @@
                 filename = str(path)
             if filename and self.workspace:
                 if not (self.workspace / "objects").exists():
                     (self.workspace / "objects").mkdir()
                 filepath = self.workspace / "objects" / filename
 
                 if filepath.exists() and not overwrite:
-                    raise FileExistsError(f"File {filename} already exists in workspace")
+                    # warn user that file is being restored
+                    self.logger.warning(f"File {filename} already exists in workspace")
+                    return filepath
 
         if filepath:
             if filepath.exists() and not overwrite:
-                raise FileExistsError(f"File {filename} already exists in workspace")
+                self.logger.warning(f"File {filename} already exists in workspace")
+                return filepath
             if obj and isinstance(obj, ObjectContentsObjectPath):
                 json.dump(obj.contents, open(filepath, "w"), indent=2)
             elif obj:
                 with httpx.stream(method="get", url=obj.url) as r:
                     r.raise_for_status()
 
                     buf = ""
@@ -1589,15 +1592,15 @@
         access_token, url, workspace, batch_tags, logger, restore_by_default=restore_by_default
     )
     if not LOOP.is_running() and not asyncio.get_event_loop().is_running():
         _LOOP_THREAD = threading.Thread(target=start_background_loop, args=(LOOP,), daemon=True)
         _LOOP_THREAD.start()
 
     # functions that don't get called internally can be overridden with blocking versions
-    blockable_functions = ("nuke", "status", "logs", "retry", "tag")
+    blockable_functions = ("nuke", "status", "logs", "retry", "tag", "update_modules")
     built_fns = asyncio_run(provider.get_module_functions(names=module_names, tags=module_tags))
     # for each async function in the provider, create a blocking version
     blocking_versions: dict[str, Callable[..., Any]] = {}
     for name, func in provider.__dict__.items():
         if (
             asyncio.iscoroutinefunction(func)
             or inspect.iscoroutine(func)
```

### Comparing `rush_py-3.0.2/rush/tests/test_typedef.py` & `rush_py-3.0.3/rush/tests/test_typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/typedef.py` & `rush_py-3.0.3/rush/typedef.py`

 * *Files identical despite different names*

### Comparing `rush_py-3.0.2/rush/types.py` & `rush_py-3.0.3/rush/types.py`

 * *Files identical despite different names*

