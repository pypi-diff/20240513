# Comparing `tmp/latentscope-0.2.1.tar.gz` & `tmp/latentscope-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latentscope-0.2.1.tar", last modified: Fri May  3 22:31:04 2024, max compression
+gzip compressed data, was "latentscope-0.2.2.tar", last modified: Mon May 13 13:33:24 2024, max compression
```

## Comparing `latentscope-0.2.1.tar` & `latentscope-0.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.982173 latentscope-0.2.1/
--rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.1/LICENSE
--rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-03 22:31:04.981852 latentscope-0.2.1/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)    12893 2024-05-01 21:43:52.000000 latentscope-0.2.1/README.md
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.972285 latentscope-0.2.1/latentscope/
--rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-05-02 18:24:50.000000 latentscope-0.2.1/latentscope/__version__.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.973663 latentscope-0.2.1/latentscope/models/
--rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.1/latentscope/models/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.1/latentscope/models/chat_models.json
--rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.1/latentscope/models/embedding_models.json
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.975321 latentscope-0.2.1/latentscope/models/providers/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.1/latentscope/models/providers/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.1/latentscope/models/providers/base.py
--rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.1/latentscope/models/providers/cohereai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.1/latentscope/models/providers/mistralai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.1/latentscope/models/providers/nltk.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.1/latentscope/models/providers/openai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.1/latentscope/models/providers/togetherai.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.1/latentscope/models/providers/transformers.py
--rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.1/latentscope/models/providers/voyageai.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.976654 latentscope-0.2.1/latentscope/scripts/
--rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.1/latentscope/scripts/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.1/latentscope/scripts/cluster-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.1/latentscope/scripts/cluster.py
--rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.1/latentscope/scripts/embed.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/scripts/ingest.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.1/latentscope/scripts/label_clusters.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6306 2024-05-02 18:45:04.000000 latentscope-0.2.1/latentscope/scripts/scope.py
--rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.1/latentscope/scripts/umapper-1d.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.1/latentscope/scripts/umapper.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.977505 latentscope-0.2.1/latentscope/server/
--rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.1/latentscope/server/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.1/latentscope/server/app.py
--rw-r--r--   0 enjalot    (501) staff       (20)     5645 2024-05-02 18:44:22.000000 latentscope-0.2.1/latentscope/server/bulk.py
--rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/server/datasets.py
--rw-r--r--   0 enjalot    (501) staff       (20)    13927 2024-05-02 18:50:28.000000 latentscope-0.2.1/latentscope/server/jobs.py
--rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.1/latentscope/server/search.py
--rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.1/latentscope/server/tags.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.977744 latentscope-0.2.1/latentscope/util/
--rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.1/latentscope/util/__init__.py
--rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.1/latentscope/util/configuration.py
-drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-03 22:31:04.973299 latentscope-0.2.1/latentscope.egg-info/
--rw-r--r--   0 enjalot    (501) staff       (20)    18797 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/PKG-INFO
--rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/SOURCES.txt
--rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/dependency_links.txt
--rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/entry_points.txt
--rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/requires.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-03 22:31:04.000000 latentscope-0.2.1/latentscope.egg-info/top_level.txt
--rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-03 22:31:04.982235 latentscope-0.2.1/setup.cfg
--rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.1/setup.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.076438 latentscope-0.2.2/
+-rw-r--r--   0 enjalot    (501) staff       (20)     1068 2024-02-16 15:11:38.000000 latentscope-0.2.2/LICENSE
+-rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-13 13:33:24.076208 latentscope-0.2.2/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)    12878 2024-05-13 13:19:12.000000 latentscope-0.2.2/README.md
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.068332 latentscope-0.2.2/latentscope/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2032 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)       22 2024-05-13 13:33:08.000000 latentscope-0.2.2/latentscope/__version__.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.069414 latentscope-0.2.2/latentscope/models/
+-rw-r--r--   0 enjalot    (501) staff       (20)     2993 2024-03-19 19:02:11.000000 latentscope-0.2.2/latentscope/models/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1792 2024-03-19 18:27:46.000000 latentscope-0.2.2/latentscope/models/chat_models.json
+-rw-r--r--   0 enjalot    (501) staff       (20)     6432 2024-03-18 16:42:28.000000 latentscope-0.2.2/latentscope/models/embedding_models.json
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.070438 latentscope-0.2.2/latentscope/models/providers/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-12 13:46:58.000000 latentscope-0.2.2/latentscope/models/providers/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      694 2024-01-25 14:33:56.000000 latentscope-0.2.2/latentscope/models/providers/base.py
+-rw-r--r--   0 enjalot    (501) staff       (20)      705 2024-03-19 18:57:45.000000 latentscope-0.2.2/latentscope/models/providers/cohereai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1993 2024-03-19 18:58:41.000000 latentscope-0.2.2/latentscope/models/providers/mistralai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1147 2024-03-19 18:59:56.000000 latentscope-0.2.2/latentscope/models/providers/nltk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2053 2024-03-19 18:57:31.000000 latentscope-0.2.2/latentscope/models/providers/openai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1145 2024-03-19 19:00:13.000000 latentscope-0.2.2/latentscope/models/providers/togetherai.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3726 2024-03-19 18:55:22.000000 latentscope-0.2.2/latentscope/models/providers/transformers.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     1329 2024-03-19 19:00:29.000000 latentscope-0.2.2/latentscope/models/providers/voyageai.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.071406 latentscope-0.2.2/latentscope/scripts/
+-rw-r--r--   0 enjalot    (501) staff       (20)        0 2024-02-03 13:56:57.000000 latentscope-0.2.2/latentscope/scripts/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3893 2024-01-10 15:27:46.000000 latentscope-0.2.2/latentscope/scripts/cluster-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7056 2024-03-19 19:11:37.000000 latentscope-0.2.2/latentscope/scripts/cluster.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    12774 2024-03-20 19:26:26.000000 latentscope-0.2.2/latentscope/scripts/embed.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6907 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/scripts/ingest.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7529 2024-03-19 19:14:07.000000 latentscope-0.2.2/latentscope/scripts/label_clusters.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6306 2024-05-02 18:45:04.000000 latentscope-0.2.2/latentscope/scripts/scope.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     2651 2024-01-20 15:57:31.000000 latentscope-0.2.2/latentscope/scripts/umapper-1d.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7489 2024-03-19 19:13:27.000000 latentscope-0.2.2/latentscope/scripts/umapper.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.072146 latentscope-0.2.2/latentscope/server/
+-rw-r--r--   0 enjalot    (501) staff       (20)      827 2024-02-12 13:27:13.000000 latentscope-0.2.2/latentscope/server/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7964 2024-04-25 14:48:04.000000 latentscope-0.2.2/latentscope/server/app.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     5645 2024-05-02 18:44:22.000000 latentscope-0.2.2/latentscope/server/bulk.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    11284 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/server/datasets.py
+-rw-r--r--   0 enjalot    (501) staff       (20)    13927 2024-05-02 18:50:28.000000 latentscope-0.2.2/latentscope/server/jobs.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     6370 2024-03-01 17:16:49.000000 latentscope-0.2.2/latentscope/server/search.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     7653 2024-04-25 14:11:19.000000 latentscope-0.2.2/latentscope/server/tags.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.072354 latentscope-0.2.2/latentscope/util/
+-rw-r--r--   0 enjalot    (501) staff       (20)      173 2024-03-05 19:19:01.000000 latentscope-0.2.2/latentscope/util/__init__.py
+-rw-r--r--   0 enjalot    (501) staff       (20)     3360 2024-03-05 19:17:14.000000 latentscope-0.2.2/latentscope/util/configuration.py
+drwxr-xr-x   0 enjalot    (501) staff       (20)        0 2024-05-13 13:33:24.069023 latentscope-0.2.2/latentscope.egg-info/
+-rw-r--r--   0 enjalot    (501) staff       (20)    18782 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/PKG-INFO
+-rw-r--r--   0 enjalot    (501) staff       (20)     1312 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/SOURCES.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)        1 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/dependency_links.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)      549 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/entry_points.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)     3006 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/requires.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       12 2024-05-13 13:33:24.000000 latentscope-0.2.2/latentscope.egg-info/top_level.txt
+-rw-r--r--   0 enjalot    (501) staff       (20)       38 2024-05-13 13:33:24.076476 latentscope-0.2.2/setup.cfg
+-rw-r--r--   0 enjalot    (501) staff       (20)     3865 2024-04-25 14:11:19.000000 latentscope-0.2.2/setup.py
```

### Comparing `latentscope-0.2.1/LICENSE` & `latentscope-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/PKG-INFO` & `latentscope-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
@@ -198,15 +198,15 @@
 3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
 4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
 
 ## Example Analysis
 What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
 * Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
 * Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
-* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
+* Explore 50,000 [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws) spanning two hundred years.
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
@@ -219,15 +219,15 @@
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
 
 See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
-from latentscope import ls
+import latentscope as ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
 ls.ingest("dadabase", df, text_column="joke")
 ls.serve()
 ```
```

### Comparing `latentscope-0.2.1/README.md` & `latentscope-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
 4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
 
 ## Example Analysis
 What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
 * Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
 * Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
-* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
+* Explore 50,000 [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws) spanning two hundred years.
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
@@ -40,15 +40,15 @@
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
 
 See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
-from latentscope import ls
+import latentscope as ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
 ls.ingest("dadabase", df, text_column="joke")
 ls.serve()
 ```
```

### Comparing `latentscope-0.2.1/latentscope/__init__.py` & `latentscope-0.2.2/latentscope/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/__init__.py` & `latentscope-0.2.2/latentscope/models/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/chat_models.json` & `latentscope-0.2.2/latentscope/models/chat_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/embedding_models.json` & `latentscope-0.2.2/latentscope/models/embedding_models.json`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/base.py` & `latentscope-0.2.2/latentscope/models/providers/base.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/cohereai.py` & `latentscope-0.2.2/latentscope/models/providers/cohereai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/mistralai.py` & `latentscope-0.2.2/latentscope/models/providers/mistralai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/nltk.py` & `latentscope-0.2.2/latentscope/models/providers/nltk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/openai.py` & `latentscope-0.2.2/latentscope/models/providers/openai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/togetherai.py` & `latentscope-0.2.2/latentscope/models/providers/togetherai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/transformers.py` & `latentscope-0.2.2/latentscope/models/providers/transformers.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/models/providers/voyageai.py` & `latentscope-0.2.2/latentscope/models/providers/voyageai.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/cluster-1d.py` & `latentscope-0.2.2/latentscope/scripts/cluster-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/cluster.py` & `latentscope-0.2.2/latentscope/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/embed.py` & `latentscope-0.2.2/latentscope/scripts/embed.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/ingest.py` & `latentscope-0.2.2/latentscope/scripts/ingest.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/label_clusters.py` & `latentscope-0.2.2/latentscope/scripts/label_clusters.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/scope.py` & `latentscope-0.2.2/latentscope/scripts/scope.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/umapper-1d.py` & `latentscope-0.2.2/latentscope/scripts/umapper-1d.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/scripts/umapper.py` & `latentscope-0.2.2/latentscope/scripts/umapper.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/__init__.py` & `latentscope-0.2.2/latentscope/server/__init__.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/app.py` & `latentscope-0.2.2/latentscope/server/app.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/bulk.py` & `latentscope-0.2.2/latentscope/server/bulk.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/datasets.py` & `latentscope-0.2.2/latentscope/server/datasets.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/jobs.py` & `latentscope-0.2.2/latentscope/server/jobs.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/search.py` & `latentscope-0.2.2/latentscope/server/search.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/server/tags.py` & `latentscope-0.2.2/latentscope/server/tags.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope/util/configuration.py` & `latentscope-0.2.2/latentscope/util/configuration.py`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope.egg-info/PKG-INFO` & `latentscope-0.2.2/latentscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latentscope
-Version: 0.2.1
+Version: 0.2.2
 Summary: Quickly embed, project, cluster and explore a dataset.
 Home-page: https://github.com/enjalot/latent-scope
 Project-URL: Source, https://github.com/enjalot/latent-scope
 Project-URL: Tracker, https://github.com/enjalot/latent-scope/issues
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: accelerate==0.26.1
@@ -198,15 +198,15 @@
 3. [Explore and Curate](https://enjalot.github.io/latent-scope/explore-and-curate)
 4. [Exporting Data](https://enjalot.github.io/latent-scope/export-data)
 
 ## Example Analysis
 What can you do with Latent Scope? The following examples demonstrate the kinds of perspective and insights you can gain from your unstructured text data.
 * Explore free-responses from surveys in this [datavis survey analysis](https://enjalot.github.io/latent-scope/datavis-survey)
 * Cluster thousands of [GitHub issues and PRs](https://enjalot.github.io/latent-scope/plot-issues)
-* Sort through two hundred years and tens of thousands of [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws)
+* Explore 50,000 [US Federal laws](https://enjalot.github.io/latent-scope/us-federal-laws) spanning two hundred years.
 
 
 ### Quick Start
 To get started, install the [latent-scope module](https://pypi.org/project/latentscope/) and run the server via the Command Line:
 
 ```bash
 python -m venv venv
@@ -219,15 +219,15 @@
 Then open your browser to http://localhost:5001 and start processing your first dataset!  
 
 See the [Your First Scope](https://enjalot.github.io/latent-scope/your-first-scope) guide for a detailed walk-through of the process.
 
 ### Python interface
 You can also ingest data from a Pandas dataframe using the Python interface:
 ```python
-from latentscope import ls
+import latentscope as ls
 df = pd.read_parquet("...")
 ls.init("~/latent-scope-data") # you can also pass in openai_key="XXX", mistral_key="XXX" etc.)
 ls.ingest("dadabase", df, text_column="joke")
 ls.serve()
 ```
```

### Comparing `latentscope-0.2.1/latentscope.egg-info/SOURCES.txt` & `latentscope-0.2.2/latentscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope.egg-info/entry_points.txt` & `latentscope-0.2.2/latentscope.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/latentscope.egg-info/requires.txt` & `latentscope-0.2.2/latentscope.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `latentscope-0.2.1/setup.py` & `latentscope-0.2.2/setup.py`

 * *Files identical despite different names*

