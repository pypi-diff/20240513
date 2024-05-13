# Comparing `tmp/taxidTools-2.2.3.tar.gz` & `tmp/taxidtools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taxidTools-2.2.3.tar", last modified: Fri Oct  8 09:52:54 2021, max compression
+gzip compressed data, was "taxidtools-2.3.0.tar", last modified: Mon May 13 09:11:41 2024, max compression
```

## Comparing `taxidTools-2.2.3.tar` & `taxidtools-2.3.0.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 09:52:54.411311 taxidTools-2.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1501 2021-10-08 09:52:45.000000 taxidTools-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-10-08 09:52:54.411311 taxidTools-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1954 2021-10-08 09:52:45.000000 taxidTools-2.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-10-08 09:52:45.000000 taxidTools-2.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-08 09:52:54.411311 taxidTools-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-10-08 09:52:45.000000 taxidTools-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 09:52:54.411311 taxidTools-2.2.3/taxidTools/
--rw-r--r--   0 runner    (1001) docker     (121)     3850 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/Lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/Node.py
--rw-r--r--   0 runner    (1001) docker     (121)    24660 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/Taxonomy.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-10-08 09:52:45.000000 taxidTools-2.2.3/taxidTools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-08 09:52:54.411311 taxidTools-2.2.3/taxidTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2506 2021-10-08 09:52:54.000000 taxidTools-2.2.3/taxidTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      310 2021-10-08 09:52:54.000000 taxidTools-2.2.3/taxidTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-08 09:52:54.000000 taxidTools-2.2.3/taxidTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-10-08 09:52:54.000000 taxidTools-2.2.3/taxidTools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:11:41.991666 taxidtools-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-13 09:11:38.000000 taxidtools-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-13 09:11:41.987666 taxidtools-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 09:11:38.000000 taxidtools-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-13 09:11:38.000000 taxidtools-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:11:41.991666 taxidtools-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 09:11:38.000000 taxidtools-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:11:41.987666 taxidtools-2.3.0/taxidTools/
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/Lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/Taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-13 09:11:38.000000 taxidtools-2.3.0/taxidTools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:11:41.987666 taxidtools-2.3.0/taxidTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-13 09:11:41.000000 taxidtools-2.3.0/taxidTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-13 09:11:41.000000 taxidtools-2.3.0/taxidTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:11:41.000000 taxidtools-2.3.0/taxidTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 09:11:41.000000 taxidtools-2.3.0/taxidTools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:11:41.987666 taxidtools-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-13 09:11:38.000000 taxidtools-2.3.0/tests/test_Lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-13 09:11:38.000000 taxidtools-2.3.0/tests/test_Node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-13 09:11:38.000000 taxidtools-2.3.0/tests/test_Taxonomy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-13 09:11:38.000000 taxidtools-2.3.0/tests/test_complextree.py
```

### Comparing `taxidTools-2.2.3/LICENSE` & `taxidtools-2.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2021, Gregoire Denay.
+Copyright 2024, Gregoire Denay.
 
 Redistribution and use in source and binary forms, with or without 
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this 
 list of conditions and the following disclaimer.
```

### Comparing `taxidTools-2.2.3/PKG-INFO` & `taxidtools-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: taxidTools
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Python Toolkit for Taxonomy
 Home-page: https://github.com/CVUA-RRW/taxidTools
 Author: Gregoire Denay
 Author-email: gregoire.denay@cvua-rrw.de
 License: BSD License
 Project-URL: Bug Tracker, https://github.com/CVUA-RRW/taxidTools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TaxidTools - A Python Toolkit for Taxonomy
 
 [![Python package](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml)
-![PyPI - License](https://img.shields.io/pypi/l/Django?style=plastic)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
-[![DOI](https://zenodo.org/badge/300595196.svg)](https://zenodo.org/badge/latestdoi/300595196)
+[![PyPI - License](https://img.shields.io/pypi/l/Django?style=flat)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/taxidtools.svg)](https://anaconda.org/conda-forge/taxidtools)
+[![Pypi Version](https://img.shields.io/pypi/v/taxidTools?style=flat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5556006.svg)](https://doi.org/10.5281/zenodo.5556006)
 
 ## Overview
 
 Provides a set of classes and tools to work with taxonomy data.
 Although built to work with the NCBI Taxdump files it can also work with other taxonomy definitions.
 Currently impelemented:
 * Easily load the NCBI taxdump files
@@ -39,16 +40,20 @@
 ## Requirements
 
 Python >= 3.9 
 Optionally some taxonomy definiton files usch as the [Taxdump definition files](https://ftp.ncbi.nlm.nih.gov/pub/taxonomy/new_taxdump/) from the NCBI server.
 
 ## Installation
 
+Install from pip or conda :
+
 ```bash
 python3 -m pip install taxidTools
+
+conda install -c conda-forge taxidtools
 ```
 
 Clone or copy the github repository to your project for the developement version.
 
 ## Usage 
 
 Check our [homepage](https://cvua-rrw.github.io/taxidTools/index.html) !
@@ -68,9 +73,7 @@
 
 Grégoire Denay, Chemisches- und Veterinär-Untersuchungsamt Rhein-Ruhr-Wupper 
 
 <gregoire.denay@cvua-rrw.de>
 
 
 
-
-
```

### Comparing `taxidTools-2.2.3/README.md` & `taxidtools-2.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # TaxidTools - A Python Toolkit for Taxonomy
 
 [![Python package](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml)
-![PyPI - License](https://img.shields.io/pypi/l/Django?style=plastic)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
-[![DOI](https://zenodo.org/badge/300595196.svg)](https://zenodo.org/badge/latestdoi/300595196)
+[![PyPI - License](https://img.shields.io/pypi/l/Django?style=flat)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/taxidtools.svg)](https://anaconda.org/conda-forge/taxidtools)
+[![Pypi Version](https://img.shields.io/pypi/v/taxidTools?style=flat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5556006.svg)](https://doi.org/10.5281/zenodo.5556006)
 
 ## Overview
 
 Provides a set of classes and tools to work with taxonomy data.
 Although built to work with the NCBI Taxdump files it can also work with other taxonomy definitions.
 Currently impelemented:
 * Easily load the NCBI taxdump files
@@ -22,16 +24,20 @@
 ## Requirements
 
 Python >= 3.9 
 Optionally some taxonomy definiton files usch as the [Taxdump definition files](https://ftp.ncbi.nlm.nih.gov/pub/taxonomy/new_taxdump/) from the NCBI server.
 
 ## Installation
 
+Install from pip or conda :
+
 ```bash
 python3 -m pip install taxidTools
+
+conda install -c conda-forge taxidtools
 ```
 
 Clone or copy the github repository to your project for the developement version.
 
 ## Usage 
 
 Check our [homepage](https://cvua-rrw.github.io/taxidTools/index.html) !
```

### Comparing `taxidTools-2.2.3/setup.py` & `taxidtools-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `taxidTools-2.2.3/taxidTools/Lineage.py` & `taxidtools-2.3.0/taxidTools/Lineage.py`

 * *Files identical despite different names*

### Comparing `taxidTools-2.2.3/taxidTools/Node.py` & `taxidtools-2.3.0/taxidTools/Node.py`

 * *Files identical despite different names*

### Comparing `taxidTools-2.2.3/taxidTools/Taxonomy.py` & `taxidtools-2.3.0/taxidTools/Taxonomy.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Union, Iterator, Optional
 from collections import UserDict, Counter
 from copy import copy
 import json 
 from .Node import Node, DummyNode, _BaseNode
 from .Lineage import Lineage
 from .utils import linne
+from .exceptions import InvalidNodeError
 
 
 class Taxonomy(UserDict):
     """
     Store Taxonomy nodes
     
     A Taxonomy is instanciated as a dictionnary and 
@@ -77,14 +78,20 @@
         super().__init__(*args, **kwargs)
         # create name dict for backward lookup
         self._namedict = {}
         for k, v in self.items():
             if v.name:
                 self._namedict[v.name] = k
     
+    def __getitem__(self, key: str) -> Node:
+        try:
+            return super().__getitem__(key)
+        except KeyError:
+            raise InvalidNodeError(f"There is no Node with taxid '{key}' in this Taxonomy")
+    
     @classmethod
     def from_list(cls, node_list: list[_BaseNode]) -> Taxonomy:
         """
         Create a Taxonomy object from a list of Nodes
         
         Convert a list of Nodes into a valid Taxonomy object 
         where each Node can be accessed using its taxid as key.
@@ -717,18 +724,42 @@
     ----------
     path:
         Path of file to load
     
     See Also
     --------
     Taxonomy.write
+    load_ncbi
     """
     return Taxonomy.from_json(path)
 
 
+def load_ncbi(nodes: str, rankedlineage: str) -> Taxonomy:
+    """
+    Load a Taxonomy from the NCBI`s taxdump files
+
+    Parameters
+    ----------
+    nodes: 
+        Path to the nodes.dmp file
+    rankedlineage: 
+        Path to the rankedlineage.dmp file
+    
+    Examples
+    --------
+    >>> tax = load_ncbi("nodes.dmp', 'rankedlineage.dmp')
+
+    See Also
+    --------
+    Taxonomy.from_taxdump
+    load
+    """
+    return Taxonomy.from_taxdump(nodes, rankedlineage)
+
+
 def _parse_dump(filepath: str) -> Iterator:
     """
     Dump file line iterator, returns a yields of fields
     """
     with open(filepath, 'r') as dmp:
         for line in dmp:
             yield [item.strip() for item in line.split("|")]
```

### Comparing `taxidTools-2.2.3/taxidTools/__init__.py` & `taxidtools-2.3.0/taxidTools/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .Node import Node, DummyNode
-from .Taxonomy import Taxonomy, load
+from .Taxonomy import Taxonomy, load, load_ncbi
 from .Lineage import Lineage
 from .utils import linne
+from .exceptions import TaxonomyError, InvalidNodeError
 from .__version__ import __version__, __title__, __description__
 from .__version__ import __author__, __author_email__, __licence__
 from .__version__ import __url__
 
 __all__ = ['Node', 'DummyNode',
-           'Taxonomy', 'load',
+           'Taxonomy', 'load', 'load_ncbi'
            'Lineage',
            'linne',
+           'TaxonomyError', 'InvalidNodeError',
            '__version__',
            '__title__',
            '__description__',
            '__author__',
            '__author_email__',
            '__licence__',
            '__url__'
```

### Comparing `taxidTools-2.2.3/taxidTools/utils.py` & `taxidtools-2.3.0/taxidTools/utils.py`

 * *Files identical despite different names*

### Comparing `taxidTools-2.2.3/taxidTools.egg-info/PKG-INFO` & `taxidtools-2.3.0/taxidTools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: taxidTools
-Version: 2.2.3
+Version: 2.3.0
 Summary: A Python Toolkit for Taxonomy
 Home-page: https://github.com/CVUA-RRW/taxidTools
 Author: Gregoire Denay
 Author-email: gregoire.denay@cvua-rrw.de
 License: BSD License
 Project-URL: Bug Tracker, https://github.com/CVUA-RRW/taxidTools/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TaxidTools - A Python Toolkit for Taxonomy
 
 [![Python package](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml/badge.svg?branch=main)](https://github.com/CVUA-RRW/taxidTools/actions/workflows/python-package.yml)
-![PyPI - License](https://img.shields.io/pypi/l/Django?style=plastic)
-![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
-[![DOI](https://zenodo.org/badge/300595196.svg)](https://zenodo.org/badge/latestdoi/300595196)
+[![PyPI - License](https://img.shields.io/pypi/l/Django?style=flat)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/CVUA-RRW/taxidTools)
+[![Conda Version](https://img.shields.io/conda/vn/conda-forge/taxidtools.svg)](https://anaconda.org/conda-forge/taxidtools)
+[![Pypi Version](https://img.shields.io/pypi/v/taxidTools?style=flat)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5556006.svg)](https://doi.org/10.5281/zenodo.5556006)
 
 ## Overview
 
 Provides a set of classes and tools to work with taxonomy data.
 Although built to work with the NCBI Taxdump files it can also work with other taxonomy definitions.
 Currently impelemented:
 * Easily load the NCBI taxdump files
@@ -39,16 +40,20 @@
 ## Requirements
 
 Python >= 3.9 
 Optionally some taxonomy definiton files usch as the [Taxdump definition files](https://ftp.ncbi.nlm.nih.gov/pub/taxonomy/new_taxdump/) from the NCBI server.
 
 ## Installation
 
+Install from pip or conda :
+
 ```bash
 python3 -m pip install taxidTools
+
+conda install -c conda-forge taxidtools
 ```
 
 Clone or copy the github repository to your project for the developement version.
 
 ## Usage 
 
 Check our [homepage](https://cvua-rrw.github.io/taxidTools/index.html) !
@@ -68,9 +73,7 @@
 
 Grégoire Denay, Chemisches- und Veterinär-Untersuchungsamt Rhein-Ruhr-Wupper 
 
 <gregoire.denay@cvua-rrw.de>
 
 
 
-
-
```

