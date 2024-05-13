# Comparing `tmp/macromol_census-0.1.0.tar.gz` & `tmp/macromol_census-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macromol_census-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "macromol_census-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `macromol_census-0.1.0.tar` & `macromol_census-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1639 2024-05-01 19:50:25.336606 macromol_census-0.1.0/README.rst
--rw-r--r--   0        0        0      639 2024-05-01 19:50:26.120612 macromol_census-0.1.0/macromol_census/__init__.py
--rw-r--r--   0        0        0    27001 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/database_io.py
--rw-r--r--   0        0        0      452 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/error.py
--rw-r--r--   0        0        0     4435 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/extract_fasta.py
--rw-r--r--   0        0        0     3242 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/extract_nonredundant_assemblies.py
--rw-r--r--   0        0        0     4122 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/find_identical_branched_entities.py
--rw-r--r--   0        0        0      537 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/find_identical_ligands.py
--rw-r--r--   0        0        0      867 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_blacklist.py
--rw-r--r--   0        0        0     2002 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_chemicals.py
--rw-r--r--   0        0        0     2448 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_entity_clusters.py
--rw-r--r--   0        0        0     1543 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_nonspecific_ligands.py
--rw-r--r--   0        0        0    12017 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_structures.py
--rw-r--r--   0        0        0     3760 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/ingest_validation.py
--rw-r--r--   0        0        0      477 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/init.py
--rw-r--r--   0        0        0    20951 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/pick_assemblies.py
--rw-r--r--   0        0        0     5664 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/rank_assemblies.py
--rw-r--r--   0        0        0     2647 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/rank_structures.py
--rw-r--r--   0        0        0     2859 2024-05-01 19:50:25.340606 macromol_census-0.1.0/macromol_census/util.py
--rw-r--r--   0        0        0     2994 2024-05-01 19:50:25.340606 macromol_census-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 macromol_census-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1639 2024-05-13 19:01:48.494324 macromol_census-0.2.0/README.rst
+-rw-r--r--   0        0        0      639 2024-05-13 19:01:49.262323 macromol_census-0.2.0/macromol_census/__init__.py
+-rw-r--r--   0        0        0    27001 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/database_io.py
+-rw-r--r--   0        0        0      452 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/error.py
+-rw-r--r--   0        0        0     4435 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/extract_fasta.py
+-rw-r--r--   0        0        0     3242 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/extract_nonredundant_assemblies.py
+-rw-r--r--   0        0        0     4122 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/find_identical_branched_entities.py
+-rw-r--r--   0        0        0      537 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/find_identical_ligands.py
+-rw-r--r--   0        0        0      867 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_blacklist.py
+-rw-r--r--   0        0        0     2002 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_chemicals.py
+-rw-r--r--   0        0        0     2448 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_entity_clusters.py
+-rw-r--r--   0        0        0     1543 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_nonspecific_ligands.py
+-rw-r--r--   0        0        0    12017 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_structures.py
+-rw-r--r--   0        0        0     3760 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/ingest_validation.py
+-rw-r--r--   0        0        0      477 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/init.py
+-rw-r--r--   0        0        0    20988 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/pick_assemblies.py
+-rw-r--r--   0        0        0     5664 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/rank_assemblies.py
+-rw-r--r--   0        0        0     2647 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/rank_structures.py
+-rw-r--r--   0        0        0     2859 2024-05-13 19:01:48.494324 macromol_census-0.2.0/macromol_census/util.py
+-rw-r--r--   0        0        0     2994 2024-05-13 19:01:48.494324 macromol_census-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2956 1970-01-01 00:00:00.000000 macromol_census-0.2.0/PKG-INFO
```

### Comparing `macromol_census-0.1.0/README.rst` & `macromol_census-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/__init__.py` & `macromol_census-0.2.0/macromol_census/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tools for creating machine-learning datasets from macromolecular structure 
 data.
 """
 
-__version__ = '0.1.0'
+__version__ = '0.2.0'
 
 from .database_io import *
 from .init import *
 from .ingest_structures import *
 from .ingest_chemicals import *
 from .ingest_validation import *
 from .ingest_blacklist import *
```

### Comparing `macromol_census-0.1.0/macromol_census/database_io.py` & `macromol_census-0.2.0/macromol_census/database_io.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/extract_fasta.py` & `macromol_census-0.2.0/macromol_census/extract_fasta.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/extract_nonredundant_assemblies.py` & `macromol_census-0.2.0/macromol_census/extract_nonredundant_assemblies.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/find_identical_branched_entities.py` & `macromol_census-0.2.0/macromol_census/find_identical_branched_entities.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/find_identical_ligands.py` & `macromol_census-0.2.0/macromol_census/find_identical_ligands.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_blacklist.py` & `macromol_census-0.2.0/macromol_census/ingest_blacklist.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_chemicals.py` & `macromol_census-0.2.0/macromol_census/ingest_chemicals.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_entity_clusters.py` & `macromol_census-0.2.0/macromol_census/ingest_entity_clusters.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_nonspecific_ligands.py` & `macromol_census-0.2.0/macromol_census/ingest_nonspecific_ligands.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_structures.py` & `macromol_census-0.2.0/macromol_census/ingest_structures.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/ingest_validation.py` & `macromol_census-0.2.0/macromol_census/ingest_validation.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/pick_assemblies.py` & `macromol_census-0.2.0/macromol_census/pick_assemblies.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 from .util import tquiet
 from dataclasses import dataclass
 from itertools import combinations, combinations_with_replacement
 from more_itertools import one, flatten
 from functools import reduce, cached_property
 from tqdm import tqdm
 
-from typing import TypeAlias, Callable
+from typing import TypeAlias, TypeVar, Callable
 from collections.abc import Iterable
 
 Subchain: TypeAlias = tuple[str, int]
+K, C = TypeVar('K'), TypeVar('C')
 
 class Visitor:
     """
     The default implementation doesn't actually do any filtering.
     """
 
     def __init__(self, structure):
@@ -569,15 +570,15 @@
             candidates,
             iter_keys,
             cluster_from_key,
             accepted_candidate_indices,
             accepted_cluster_pairs,
     )
 
-def _accept_nonredundant_candidates[K, C](
+def _accept_nonredundant_candidates(
         candidates: list[Candidate],
         iter_keys: Callable[[Candidate], Iterable[K]],
         cluster_from_key: Callable[[K], C],
         accepted_candidate_indices: set[int],
         accepted_clusters: set[C],
 ):
     groups = {}
```

### Comparing `macromol_census-0.1.0/macromol_census/rank_assemblies.py` & `macromol_census-0.2.0/macromol_census/rank_assemblies.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/rank_structures.py` & `macromol_census-0.2.0/macromol_census/rank_structures.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/macromol_census/util.py` & `macromol_census-0.2.0/macromol_census/util.py`

 * *Files identical despite different names*

### Comparing `macromol_census-0.1.0/pyproject.toml` & `macromol_census-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [project]
 name = "macromol_census"
 authors = [
   {name = "Kale Kundert", email = "kale@thekunderts.net"},
 ]
 readme = 'README.rst'
 dynamic = ["version", "description"]
-requires-python = "~=3.12"
+requires-python = "~=3.10"
 classifiers = [
   'Programming Language :: Python :: 3',
 ]
 dependencies = [
   'biopython',
   'docopt',
```

### Comparing `macromol_census-0.1.0/PKG-INFO` & `macromol_census-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: macromol_census
-Version: 0.1.0
+Version: 0.2.0
 Summary: Tools for creating machine-learning datasets from macromolecular structure 
 Author-email: Kale Kundert <kale@thekunderts.net>
-Requires-Python: ~=3.12
+Requires-Python: ~=3.10
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: biopython
 Requires-Dist: docopt
 Requires-Dist: duckdb>=0.10.0
 Requires-Dist: gemmi
 Requires-Dist: more_itertools
```

