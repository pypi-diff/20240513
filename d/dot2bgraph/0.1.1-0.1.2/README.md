# Comparing `tmp/dot2bgraph-0.1.1.tar.gz` & `tmp/dot2bgraph-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dot2bgraph-0.1.1.tar", last modified: Wed Oct 13 01:32:01 2021, max compression
+gzip compressed data, was "dot2bgraph-0.1.2.tar", last modified: Mon May 13 01:19:15 2024, max compression
```

## Comparing `dot2bgraph-0.1.1.tar` & `dot2bgraph-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,47 @@
-drwxr-xr-x   0 student    (501) staff       (20)        0 2021-10-13 01:32:01.004182 dot2bgraph-0.1.1/
--rw-r--r--   0 student    (501) staff       (20)    11347 2021-06-26 15:56:58.000000 dot2bgraph-0.1.1/LICENSE
--rw-r--r--   0 student    (501) staff       (20)     3381 2021-10-13 01:32:01.004376 dot2bgraph-0.1.1/PKG-INFO
--rw-r--r--   0 student    (501) staff       (20)     2293 2021-10-10 01:21:17.000000 dot2bgraph-0.1.1/README.md
-drwxr-xr-x   0 student    (501) staff       (20)        0 2021-10-13 01:32:00.958243 dot2bgraph-0.1.1/dot2bgraph/
--rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:50.000000 dot2bgraph-0.1.1/dot2bgraph/__init__.py
--rw-r--r--   0 student    (501) staff       (20)       72 2021-09-30 03:27:15.000000 dot2bgraph-0.1.1/dot2bgraph/__main__.py
-drwxr-xr-x   0 student    (501) staff       (20)        0 2021-10-13 01:32:00.994796 dot2bgraph-0.1.1/dot2bgraph/converter/
--rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:28.000000 dot2bgraph-0.1.1/dot2bgraph/converter/__init__.py
--rw-r--r--   0 student    (501) staff       (20)    17307 2021-10-06 00:38:26.000000 dot2bgraph-0.1.1/dot2bgraph/converter/directed.py
--rw-r--r--   0 student    (501) staff       (20)    19389 2021-10-06 00:47:51.000000 dot2bgraph-0.1.1/dot2bgraph/converter/grid.py
--rw-r--r--   0 student    (501) staff       (20)     6650 2021-10-05 23:58:37.000000 dot2bgraph-0.1.1/dot2bgraph/converter/node.py
--rw-r--r--   0 student    (501) staff       (20)     3978 2021-10-05 23:35:26.000000 dot2bgraph-0.1.1/dot2bgraph/converter/pack.py
--rw-r--r--   0 student    (501) staff       (20)     1669 2021-09-22 12:17:17.000000 dot2bgraph-0.1.1/dot2bgraph/image.py
--rw-r--r--   0 student    (501) staff       (20)    10735 2021-10-05 23:32:23.000000 dot2bgraph-0.1.1/dot2bgraph/locations.py
--rw-r--r--   0 student    (501) staff       (20)     2333 2021-10-10 00:07:38.000000 dot2bgraph-0.1.1/dot2bgraph/main.py
-drwxr-xr-x   0 student    (501) staff       (20)        0 2021-10-13 01:32:01.003390 dot2bgraph-0.1.1/dot2bgraph/utils/
--rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:40.000000 dot2bgraph-0.1.1/dot2bgraph/utils/__init__.py
--rw-r--r--   0 student    (501) staff       (20)      719 2021-09-22 12:17:10.000000 dot2bgraph-0.1.1/dot2bgraph/utils/color.py
--rw-r--r--   0 student    (501) staff       (20)     1548 2021-09-22 12:17:13.000000 dot2bgraph-0.1.1/dot2bgraph/utils/spinner.py
-drwxr-xr-x   0 student    (501) staff       (20)        0 2021-10-13 01:32:00.983038 dot2bgraph-0.1.1/dot2bgraph.egg-info/
--rw-r--r--   0 student    (501) staff       (20)     3381 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/PKG-INFO
--rw-r--r--   0 student    (501) staff       (20)      602 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/SOURCES.txt
--rw-r--r--   0 student    (501) staff       (20)        1 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/dependency_links.txt
--rw-r--r--   0 student    (501) staff       (20)       53 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/entry_points.txt
--rw-r--r--   0 student    (501) staff       (20)       39 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/requires.txt
--rw-r--r--   0 student    (501) staff       (20)       11 2021-10-13 01:32:00.000000 dot2bgraph-0.1.1/dot2bgraph.egg-info/top_level.txt
--rw-r--r--   0 student    (501) staff       (20)      100 2021-09-28 12:54:36.000000 dot2bgraph-0.1.1/pyproject.toml
--rw-r--r--   0 student    (501) staff       (20)      102 2021-10-13 01:32:01.006507 dot2bgraph-0.1.1/setup.cfg
--rw-r--r--   0 student    (501) staff       (20)     2358 2021-10-13 01:24:03.000000 dot2bgraph-0.1.1/setup.py
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.312686 dot2bgraph-0.1.2/
+-rw-r--r--   0 student    (501) staff       (20)      168 2024-05-09 23:27:33.000000 dot2bgraph-0.1.2/.gitignore
+-rw-r--r--   0 student    (501) staff       (20)      410 2021-10-12 23:34:15.000000 dot2bgraph-0.1.2/.travis.yml
+-rw-r--r--   0 student    (501) staff       (20)      490 2024-05-13 01:11:48.000000 dot2bgraph-0.1.2/CHANGELOG.md
+-rw-r--r--   0 student    (501) staff       (20)    11347 2021-06-26 15:56:58.000000 dot2bgraph-0.1.2/LICENSE
+-rw-r--r--   0 student    (501) staff       (20)    16935 2024-05-13 01:19:15.311231 dot2bgraph-0.1.2/PKG-INFO
+-rw-r--r--   0 student    (501) staff       (20)     2620 2024-05-09 23:27:01.000000 dot2bgraph-0.1.2/README.md
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.164658 dot2bgraph-0.1.2/dot2bgraph/
+-rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:50.000000 dot2bgraph-0.1.2/dot2bgraph/__init__.py
+-rw-r--r--   0 student    (501) staff       (20)       72 2021-09-30 03:27:15.000000 dot2bgraph-0.1.2/dot2bgraph/__main__.py
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.210489 dot2bgraph-0.1.2/dot2bgraph/converter/
+-rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:28.000000 dot2bgraph-0.1.2/dot2bgraph/converter/__init__.py
+-rw-r--r--   0 student    (501) staff       (20)    17307 2021-10-06 00:38:26.000000 dot2bgraph-0.1.2/dot2bgraph/converter/directed.py
+-rw-r--r--   0 student    (501) staff       (20)    19817 2024-05-09 12:29:37.000000 dot2bgraph-0.1.2/dot2bgraph/converter/grid.py
+-rw-r--r--   0 student    (501) staff       (20)     6650 2021-10-05 23:58:37.000000 dot2bgraph-0.1.2/dot2bgraph/converter/node.py
+-rw-r--r--   0 student    (501) staff       (20)     3978 2021-10-05 23:35:26.000000 dot2bgraph-0.1.2/dot2bgraph/converter/pack.py
+-rw-r--r--   0 student    (501) staff       (20)     1669 2021-09-22 12:17:17.000000 dot2bgraph-0.1.2/dot2bgraph/image.py
+-rw-r--r--   0 student    (501) staff       (20)    10735 2021-10-05 23:32:23.000000 dot2bgraph-0.1.2/dot2bgraph/locations.py
+-rw-r--r--   0 student    (501) staff       (20)     2333 2021-10-10 00:07:38.000000 dot2bgraph-0.1.2/dot2bgraph/main.py
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.220486 dot2bgraph-0.1.2/dot2bgraph/utils/
+-rw-r--r--   0 student    (501) staff       (20)        0 2021-09-25 02:27:40.000000 dot2bgraph-0.1.2/dot2bgraph/utils/__init__.py
+-rw-r--r--   0 student    (501) staff       (20)      719 2021-09-22 12:17:10.000000 dot2bgraph-0.1.2/dot2bgraph/utils/color.py
+-rw-r--r--   0 student    (501) staff       (20)     1548 2021-09-22 12:17:13.000000 dot2bgraph-0.1.2/dot2bgraph/utils/spinner.py
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.309024 dot2bgraph-0.1.2/dot2bgraph.egg-info/
+-rw-r--r--   0 student    (501) staff       (20)    16935 2024-05-13 01:19:14.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/PKG-INFO
+-rw-r--r--   0 student    (501) staff       (20)      880 2024-05-13 01:19:15.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 student    (501) staff       (20)        1 2024-05-13 01:19:14.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 student    (501) staff       (20)       52 2024-05-13 01:19:14.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/entry_points.txt
+-rw-r--r--   0 student    (501) staff       (20)       81 2024-05-13 01:19:14.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/requires.txt
+-rw-r--r--   0 student    (501) staff       (20)       11 2024-05-13 01:19:14.000000 dot2bgraph-0.1.2/dot2bgraph.egg-info/top_level.txt
+-rw-r--r--   0 student    (501) staff       (20)      301 2021-10-05 23:33:12.000000 dot2bgraph-0.1.2/mypy.ini
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.228335 dot2bgraph-0.1.2/offline/
+-rw-r--r--   0 student    (501) staff       (20)     1778 2022-01-05 02:18:32.000000 dot2bgraph-0.1.2/offline/random_dag.py
+-rw-r--r--   0 student    (501) staff       (20)     1479 2024-05-13 00:41:30.000000 dot2bgraph-0.1.2/pyproject.toml
+-rw-r--r--   0 student    (501) staff       (20)      758 2024-05-13 01:13:03.000000 dot2bgraph-0.1.2/release_checklist.md
+-rw-r--r--   0 student    (501) staff       (20)       38 2024-05-13 01:19:15.314279 dot2bgraph-0.1.2/setup.cfg
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.254885 dot2bgraph-0.1.2/tests/
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.303154 dot2bgraph-0.1.2/tests/converter/
+-rw-r--r--   0 student    (501) staff       (20)    23429 2021-09-25 22:22:29.000000 dot2bgraph-0.1.2/tests/converter/test_directed.py
+-rw-r--r--   0 student    (501) staff       (20)    33615 2022-01-06 01:45:20.000000 dot2bgraph-0.1.2/tests/converter/test_grid.py
+-rw-r--r--   0 student    (501) staff       (20)     4168 2021-09-25 22:22:17.000000 dot2bgraph-0.1.2/tests/converter/test_node.py
+-rw-r--r--   0 student    (501) staff       (20)     6848 2021-09-25 22:22:14.000000 dot2bgraph-0.1.2/tests/converter/test_pack.py
+-rw-r--r--   0 student    (501) staff       (20)      933 2021-09-25 22:22:01.000000 dot2bgraph-0.1.2/tests/test_image.py
+-rw-r--r--   0 student    (501) staff       (20)     9051 2021-10-12 23:24:21.000000 dot2bgraph-0.1.2/tests/test_locations.py
+-rw-r--r--   0 student    (501) staff       (20)     3993 2021-09-25 22:21:53.000000 dot2bgraph-0.1.2/tests/test_main.py
+drwxr-xr-x   0 student    (501) staff       (20)        0 2024-05-13 01:19:15.306656 dot2bgraph-0.1.2/tests/utils/
+-rw-r--r--   0 student    (501) staff       (20)      329 2021-09-25 22:22:06.000000 dot2bgraph-0.1.2/tests/utils/test_color.py
```

### Comparing `dot2bgraph-0.1.1/LICENSE` & `dot2bgraph-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/PKG-INFO` & `dot2bgraph-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: dot2bgraph
-Version: 0.1.1
-Summary: A CLI to convert dot files to bgraph format for visualization.
-Home-page: https://github.com/vasilyrud/dot2bgraph
-Author: Vasily Rudchenko
-Author-email: vasily.rudchenko.dev@gmail.com
-License: Apache Software License
-Keywords: graph,visualization,dot,bgraph,command,line,interface,cli,tool,convert
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # dot2bgraph [![PyPI](https://img.shields.io/pypi/v/dot2bgraph)](https://pypi.org/project/dot2bgraph) [![Travis (.com)](https://img.shields.io/travis/com/vasilyrud/dot2bgraph)](https://travis-ci.com/github/vasilyrud/dot2bgraph) [![Coveralls](https://img.shields.io/coveralls/github/vasilyrud/dot2bgraph)](https://coveralls.io/github/vasilyrud/dot2bgraph)
 
 `dot2bgraph` is a CLI utility to convert graphs in `dot` format to `bgraph` format, for visualization with tools like [bgrapher](https://github.com/vasilyrud/bgrapher).
 
 `dot2bgraph` supports a subset of `dot` features, tailored specifically to those that convert neatly to `bgraph` format. Other `dot` attributes that do not correlate to attributes supported by `bgraph` (e.g., shapes, label positions, etc.) are ignored.
 
 ## Installation
@@ -50,14 +24,16 @@
 
 Then, install `dot2bgraph`:
 
 ```
 pip install dot2bgraph
 ```
 
+With MacOS you may need to prepend `CFLAGS="-I$(brew --prefix graphviz)/include" LDFLAGS="-L$(brew --prefix graphviz)/lib"`
+
 ## Usage
 
 By default an input "file.dot" is converted to `bgraph` JSON format, which is outputted to stdout:
 
 ```
 dot2bgraph file.dot
 ```
@@ -86,20 +62,21 @@
 To save the tool's output (in whichever format) to a file, use `-o`.
 
 ## Development
 
 ### Install
 
 ```
-mkdir .venv
-pipenv shell
-pipenv install --dev -e .
-pipenv install -r requirements-dev.txt
+python3 -m venv .venv
+source .venv/bin/activate
+CFLAGS="-I$(brew --prefix graphviz)/include" LDFLAGS="-L$(brew --prefix graphviz)/lib" python3 -m pip install ".[dev]"
 ```
 
+With MacOS you may need to prepend `CFLAGS="-I$(brew --prefix graphviz)/include" LDFLAGS="-L$(brew --prefix graphviz)/lib"`
+
 ### Test
 
 #### Pytest
 
 ```
 python -m pytest -s --cov-report term-missing --cov=dot2bgraph
 ```
@@ -111,9 +88,7 @@
 ```
 
 #### Profile
 
 ```
 python -mcProfile -o dot2bgraph.prof dot2bgraph/__main__.py -f none <your_dot_file>
 ```
-
-
```

### Comparing `dot2bgraph-0.1.1/dot2bgraph/converter/directed.py` & `dot2bgraph-0.1.2/dot2bgraph/converter/directed.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/converter/grid.py` & `dot2bgraph-0.1.2/dot2bgraph/converter/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -385,60 +385,72 @@
 
         self._add_sub_grid(grid, use_x, use_y)
 
 class _SeenNodes:
     ''' Helper class to store info about nodes
     during traversal.
     '''
-    def __init__(self):
+    def __init__(self) -> None:
         self.nodes: Set[Node] = set()
 
         self.time: int = 0
         self.start:  Dict[Node,int] = {}
         self.finish: Dict[Node,int] = {}
 
 def _sources_per_conn_comp(conn_comp: Iterable[Node]) -> Set[Node]:
     ''' Find either the sources that are naturally
     sources or pick one source that is the least 
     connected inwards.
     Assume we are given a connected component.
     '''
     assert conn_comp, 'Got empty set of connected components to get sources from.'
+    num_prev = {node: len(list(node.local_prev)) for node in conn_comp}
+    num_next = {node: len(list(node.local_next)) for node in conn_comp}
 
     # Get node that doesn't have inward connections.
-    sources = {node for node in conn_comp if not node.prev}
-    if sources: return sources
-
-    # Otherwise, pick a node out of nodes with fewest inward connections 
-    # that also has the most outward connections.
-    min_inward  = min(len(node.prev) for node in conn_comp)
-    max_outward = max(len(node.next) for node in conn_comp)
-
+    sources = {node for node, prevs in num_prev.items() if not prevs}
+    if sources:
+        return sources
+
+    # Otherwise, find nodes with fewest inward connections.
+    min_inward  = min(num_prev.values())
+    # From these, pick one that has the most outward connections.
+    max_outward = max(nexts for node, nexts in num_next.items() 
+        if num_prev[node] == min_inward
+    )
+    # Get the first one of these, alphabetically
     for node in sorted(conn_comp, key=lambda n: n.name):
-        if (
-            len(node.prev) == min_inward and
-            len(node.next) == max_outward
+        if (num_prev[node] == min_inward and
+            num_next[node] == max_outward
         ):
             return {node}
 
     assert False, 'Somehow didn\'t find any source node.'
 
-def _get_conn_comp_dfs_recurse(node, seen, conn_comp):
+def _sinks_per_conn_comp(conn_comp: Iterable[Node]) -> Set[Node]:
+    ''' Get sinks, but only the ones that are "pure",
+    i.e., don't have any next edges.
+    '''
+    assert conn_comp, 'Got empty set of connected components to get sinks from.'
+    num_next = {node: len(list(node.local_next)) for node in conn_comp}
+
+    return {node for node, nexts in num_next.items() if not nexts}
+
+def _get_conn_comp_dfs_recurse(node: Node, seen: _SeenNodes, conn_comp: Set[Node]) -> None:
     seen.nodes.add(node)
     conn_comp.add(node)
 
     # Iterate over edges while ignoring directedness
     for next_node in chain(node.local_next, node.local_prev):
         if next_node in seen.nodes: continue
 
         _get_conn_comp_dfs_recurse(next_node, seen, conn_comp)
 
 def _sources(region: Region) -> Iterable[Node]:
-    ''' Get sources, one per connected component.
-    Return in alphabetical order.
+    ''' Get 1 or more sources.
     '''
     seen = _SeenNodes()
     sources = set()
 
     for node in region.nodes_sorted:
         if node in seen.nodes: continue
 
@@ -446,29 +458,26 @@
         _get_conn_comp_dfs_recurse(node, seen, conn_comp)
 
         sources |= _sources_per_conn_comp(conn_comp)
 
     return list(sorted(sources, key=lambda s: s.name))
 
 def _sinks(region: Region) -> Iterable[Node]:
-    ''' Get sinks, but only the ones that are "pure",
-    i.e., don't have any next edges.
-    Return in alphabetical order.
+    ''' Get 0 or more sinks.
     '''
     seen = _SeenNodes()
     sinks = set()
 
     for node in region.nodes_sorted:
         if node in seen.nodes: continue
 
         conn_comp: Set[Node] = set()
         _get_conn_comp_dfs_recurse(node, seen, conn_comp)
 
-        assert conn_comp, 'Got empty set of connected components to get sinks from.'
-        sinks |= {node for node in conn_comp if not node.next}
+        sinks |= _sinks_per_conn_comp(conn_comp)
 
     return list(sorted(sinks, key=lambda s: s.name))
 
 def _classify_edge(
     edge,
     edge_types,
     seen,
@@ -518,15 +527,15 @@
             )
 
     seen.time += 1
     seen.finish[cur_node] = seen.time
 
 def _get_edge_types(
     region: Region,
-):
+) -> EdgeTypes:
     ''' Classify edges in the graph.
 
     Call DFS to edge classification starting only
     at the source nodes.
 
     Assumes that source nodes will never be traversed
     to before they are used as sources.
```

### Comparing `dot2bgraph-0.1.1/dot2bgraph/converter/node.py` & `dot2bgraph-0.1.2/dot2bgraph/converter/node.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/converter/pack.py` & `dot2bgraph-0.1.2/dot2bgraph/converter/pack.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/image.py` & `dot2bgraph-0.1.2/dot2bgraph/image.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/locations.py` & `dot2bgraph-0.1.2/dot2bgraph/locations.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/main.py` & `dot2bgraph-0.1.2/dot2bgraph/main.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/utils/color.py` & `dot2bgraph-0.1.2/dot2bgraph/utils/color.py`

 * *Files identical despite different names*

### Comparing `dot2bgraph-0.1.1/dot2bgraph/utils/spinner.py` & `dot2bgraph-0.1.2/dot2bgraph/utils/spinner.py`

 * *Files identical despite different names*

