# Comparing `tmp/pype-schema-0.5.0.tar.gz` & `tmp/pype-schema-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pype-schema-0.5.0.tar", last modified: Tue Mar 12 21:44:35 2024, max compression
+gzip compressed data, was "pype-schema-0.5.1.tar", last modified: Mon May 13 21:55:38 2024, max compression
```

## Comparing `pype-schema-0.5.0.tar` & `pype-schema-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:44:35.883263 pype-schema-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-12 21:44:31.000000 pype-schema-0.5.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35666 2024-03-12 21:44:31.000000 pype-schema-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-12 21:44:31.000000 pype-schema-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-12 21:44:35.883263 pype-schema-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-03-12 21:44:31.000000 pype-schema-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:44:35.883263 pype-schema-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/connection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/node.rst
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/operations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/parse_json.rst
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/tag.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/units.rst
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-12 21:44:31.000000 pype-schema-0.5.0/docs/visualize.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:44:35.883263 pype-schema-0.5.0/pype_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19237 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:44:35.883263 pype-schema-0.5.0/pype_schema/data/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/data/sample.json
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/data/unit_definitions.txt
--rw-r--r--   0 runner    (1001) docker     (127)    75841 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    51278 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    16258 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    24287 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-03-12 21:44:31.000000 pype-schema-0.5.0/pype_schema/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 21:44:35.883263 pype-schema-0.5.0/pype_schema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-12 21:44:35.000000 pype-schema-0.5.0/pype_schema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-12 21:44:35.883263 pype-schema-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-03-12 21:44:31.000000 pype-schema-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.954998 pype-schema-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-13 21:55:34.000000 pype-schema-0.5.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35666 2024-05-13 21:55:34.000000 pype-schema-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-13 21:55:34.000000 pype-schema-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-13 21:55:38.954998 pype-schema-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-13 21:55:34.000000 pype-schema-0.5.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.950997 pype-schema-0.5.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.950997 pype-schema-0.5.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    38105 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/_static/ng-imports.png
+-rw-r--r--   0 runner    (1001) docker     (127)   148441 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/_static/utility-graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)   188016 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/_static/wwtp-graph.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/advanced.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/hello.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    72961 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/json_rep.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/node.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/operations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/parse_json.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/tag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/units.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 21:55:34.000000 pype-schema-0.5.1/docs/visualize.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.950997 pype-schema-0.5.1/pype_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25210 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.954998 pype-schema-0.5.1/pype_schema/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20139 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/data/sample.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/data/sample_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/data/unit_definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    92113 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58655 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16369 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24753 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-13 21:55:34.000000 pype-schema-0.5.1/pype_schema/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:55:38.954998 pype-schema-0.5.1/pype_schema.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 21:55:38.000000 pype-schema-0.5.1/pype_schema.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-13 21:55:38.954998 pype-schema-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-13 21:55:34.000000 pype-schema-0.5.1/setup.py
```

### Comparing `pype-schema-0.5.0/CONTRIBUTING.rst` & `pype-schema-0.5.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/LICENSE` & `pype-schema-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/PKG-INFO` & `pype-schema-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pype-schema
-Version: 0.5.0
+Version: 0.5.1
 Summary: Class hierarchy to represent configurations of process engineering systems.
 Home-page: https://github.com/we3lab/pype-schema
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: pype-schema
 Platform: UNKNOWN
@@ -70,11 +70,15 @@
 5. ``black pype_schema``
 
   This will reformat the code according to strict style guidelines.
 
 Legal Documents
 ===============
 
+This work was funded by the `Center for Integrated Facility Engineering <https://cife.stanford.edu/>`_ at Stanford University as a
+a part of CIFE Seed Proposal 2023-02
+`Formal proofs of safe operating limits at wastewater resource recovery facilities <https://cife.stanford.edu/formal-proofs-safe-operating-limits-wastewater-resource-recovery-facilities>`_.
+
 - `LICENSE <https://github.com/we3lab/pype-schema/blob/main/LICENSE/>`_
 - `CONTRIBUTING <https://github.com/we3lab/pype-schema/blob/main/CONTRIBUTING.rst/>`_
```

### Comparing `pype-schema-0.5.0/docs/Makefile` & `pype-schema-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/docs/conf.py` & `pype-schema-0.5.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "PyPES"
-copyright = "2022, WE3 Lab"
+copyright = "2024, WE3 Lab"
 author = "WE3 Lab"
 
 # The short X.Y version
 version = ""
 # The full version, including alpha/beta/rc tags
-release = "0.0"
+release = "0.5.1"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
@@ -88,15 +88,15 @@
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "alabaster"
+html_theme = "sphinx_rtd_theme"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
```

### Comparing `pype-schema-0.5.0/docs/make.bat` & `pype-schema-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/pype_schema/data/sample.json` & `pype-schema-0.5.1/pype_schema/data/sample.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9987822602999534%*

 * *Differences: {"'GasToBoiler'": "{'tags': {replace: OrderedDict([('BoilerGasPurchases', OrderedDict([('type', "*

 * *                  "'Flow'), ('units', 'SCFM'), ('contents', 'NaturalGas'), ('totalized', "*

 * *                  'False)]))])}}',*

 * * "'GasToCogen'": "{'tags': {replace: OrderedDict([('CogenGasPurchases', OrderedDict([('type', "*

 * *                 "'Flow'), ('units', 'SCFM'), ('contents', 'NaturalGas'), ('totalized', "*

 * *                 "False)]))])}, 'virtual_tags': {'NoGasPurchases': {'tags': "*

 * *                 "['Coge […]*

```diff
@@ -441,45 +441,52 @@
     },
     "GasToBoiler": {
         "bidirectional": false,
         "contents": "NaturalGas",
         "destination": "WWTP",
         "entry_point": "Boiler",
         "source": "PowerGrid",
-        "tags": {},
+        "tags": {
+            "BoilerGasPurchases": {
+                "contents": "NaturalGas",
+                "totalized": false,
+                "type": "Flow",
+                "units": "SCFM"
+            }
+        },
         "type": "Pipe"
     },
     "GasToCogen": {
         "bidirectional": false,
         "contents": "NaturalGas",
         "destination": "WWTP",
         "entry_point": "Cogenerator",
         "source": "PowerGrid",
         "tags": {
-            "GasPurchases": {
+            "CogenGasPurchases": {
                 "contents": "NaturalGas",
                 "totalized": false,
                 "type": "Flow",
                 "units": "SCFM"
             }
         },
         "type": "Pipe",
         "virtual_tags": {
             "NoGasPurchases": {
                 "operations": "lambda x: x==0",
                 "tags": [
-                    "GasPurchases"
+                    "CogenGasPurchases"
                 ],
                 "type": "RunStatus",
                 "units": null
             },
             "NoGasPurchasesList": {
                 "operations": "lambda x: [x_==0 for x_ in x]",
                 "tags": [
-                    "GasPurchases"
+                    "CogenGasPurchases"
                 ],
                 "type": "RunStatus",
                 "units": null
             }
         }
     },
     "GravityThickener": {
@@ -917,22 +924,22 @@
             "units": "kilowatt * hour / SCFM"
         },
         "GrossGasProduction": {
             "contents": "GasBlend",
             "operations": "lambda x,y: x + y",
             "tags": [
                 "CombinedDigesterGasFlow",
-                "GasPurchases"
+                "CogenGasPurchases"
             ],
             "units": "SCFM"
         },
         "GrossGasProductionList": {
             "contents": "GasBlend",
             "operations": "lambda x,y: [sum(z) for z in zip(x,y)]",
             "tags": [
                 "CombinedDigesterGasFlow",
-                "GasPurchases"
+                "CogenGasPurchases"
             ],
             "units": "SCFM"
         }
     }
 }
```

### Comparing `pype-schema-0.5.0/pype_schema/node.py` & `pype-schema-0.5.1/pype_schema/node.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,30 @@
+import warnings
 from abc import ABC
 from . import utils
 from .tag import Tag, VirtualTag
 
 
+EFFICIENCY_ATTRS = ["thermal_efficiency", "electrical_efficiency", "rte"]
+
+CAPACITY_ATTRS = [
+    "volume",
+    "energy_capacity",
+    "discharge_rate",
+    "charge_rate",
+    "min_flow",
+    "max_flow",
+    "design_flow",
+    "min_gen",
+    "max_gen",
+    "design_gen",
+    "power_rating",
+]
+
+
 class Node(ABC):
     """Abstract class for all nodes
 
     Attributes
     ----------
     id : str
         Node ID
@@ -30,29 +48,95 @@
         return (
             f"<pype_schema.node.Node id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} "
             f"tags:{self.tags}>\n"
         )
 
-    def set_flow_rate(self, min, max, avg):
-        """Set the minimum, maximum, and average flow rate of the node
+    def set_flow_rate(self, min, max, design):
+        """Set the minimum, maximum, and design flow rate of the node
 
         Parameters
         ----------
         min : int
             Minimum flow rate through the node
 
         max : int
             Maximum flow rate through the node
 
-        avg : int
-            Average flow rate through the node
+        design : int
+            Design flow rate through the node
         """
-        self.flow_rate = (min, max, avg)
+        warnings.warn(
+            "Please switch from `flow_rate` tuple to separate "
+            + "`min_flow`, `max_flow` and `design_flow` attributes",
+            DeprecationWarning,
+        )
+        self.flow_rate = (min, max, design)
+        self._min_flow = min
+        self._max_flow = max
+        self._design_flow = design
+
+    def get_min_flow(self):
+        try:
+            return self._min_flow
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `flow_rate` tuple to new `min_flow` attribute",
+                DeprecationWarning,
+            )
+            return self.flow_rate[0]
+
+    def set_min_flow(self, min_flow):
+        self._min_flow = min_flow
+
+    def del_min_flow(self):
+        del self._min_flow
+        if hasattr(self, "flow_rate"):
+            self.flow_rate = (None, self.flow_rate[1], self.flow_rate[2])
+
+    def get_max_flow(self):
+        try:
+            return self._max_flow
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `flow_rate` tuple to new `max_flow` attribute",
+                DeprecationWarning,
+            )
+            return self.flow_rate[1]
+
+    def set_max_flow(self, max_flow):
+        self._max_flow = max_flow
+
+    def del_max_flow(self):
+        del self._max_flow
+        if hasattr(self, "flow_rate"):
+            self.flow_rate = (self.flow_rate[0], None, self.flow_rate[2])
+
+    def get_design_flow(self):
+        try:
+            return self._design_flow
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `flow_rate` tuple to new `design_flow` attribute",
+                DeprecationWarning,
+            )
+            return self.flow_rate[2]
+
+    def set_design_flow(self, design_flow):
+        self._design_flow = design_flow
+
+    def del_design_flow(self):
+        del self._design_flow
+        if hasattr(self, "flow_rate"):
+            self.flow_rate = (self.flow_rate[0], self.flow_rate[1], None)
+
+    min_flow = property(get_min_flow, set_min_flow, del_min_flow)
+    max_flow = property(get_max_flow, set_max_flow, del_max_flow)
+    design_flow = property(get_design_flow, set_design_flow, del_design_flow)
 
     def set_contents(self, contents, attribute="input_contents"):
         """Set the input or output contents of a node
 
         Parameters
         ----------
         contents : ContentsType or list of ContentsType
@@ -66,14 +150,46 @@
         elif isinstance(contents, list) or contents is None:
             setattr(self, attribute, contents)
         else:
             raise TypeError(
                 "'contents' must be either ContentsType or list of ContentsType"
             )
 
+    def get_efficiencies(self):
+        """Gets a dictionary of efficiency-related attributes
+
+        Returns
+        -------
+        dict
+            Dictionary of attribute names and values
+        """
+        result = {}
+        for attr in EFFICIENCY_ATTRS:
+            try:
+                result[attr] = getattr(self, attr)
+            except AttributeError:
+                pass
+        return result
+
+    def get_capacities(self):
+        """Gets a dictionary of capacity-related attributes
+
+        Returns
+        -------
+        dict
+            Dictionary of attribute names and values
+        """
+        result = {}
+        for attr in CAPACITY_ATTRS:
+            try:
+                result[attr] = getattr(self, attr)
+            except AttributeError:
+                pass
+        return result
+
     def add_tag(self, tag):
         """Adds a tag to the node
 
         Parameters
         ----------
         tag : Tag
             Tag object to add to the node
@@ -657,17 +773,17 @@
         exit_point_type=None,
         entry_point_type=None,
         contents_type=None,
         tag_type=None,
         obj_type=None,
         recurse=False,
     ):
-        """Selects from this Node all Connection or Tag objects
+        """Selects from this Node all Node, Connection, or Tag objects
         which match source/destination node class, unit ID, and contents.
-        (If none given, returns all objects in the Node.)
+        (If none given, returns all objects in `self`)
 
         Parameters
         ----------
         source_id : str
             Optional id of the source node to filter by. None by default
 
         dest_id : str
@@ -699,34 +815,34 @@
 
         contents_type : ContentsType
             Optional contents to filter by. None by default
 
         tag_type : TagType
             Optional tag type to filter by. None by default
 
-        obj_type : [Node, Connection, Tag]
+        obj_type : [Node, Connection, VirtualTag, Tag]
             The type of object to filter by. None by default
 
         recurse : bool
             Whether to search for objects within nodes. False by default
 
         Raises
         ------
         ValueError
             When a source/destination node type is provided to subset tags
 
         TypeError
             When the objects to select among are not of
-            type {'pype_schema.Tag' or `pype_schema.Connection`}
+            type {`pype_schema.Tag`, `pype_schema.Connection`, `pype_schema.Node`}
 
         Returns
         -------
         list
-            List of `Tag` or `Connection` objects subset according to source/destination
-            id and `contents_type`
+            List of `Tag`, `Connection`, or `Node` objects subset according to
+            source/destination `id` and `contents_type`
         """
         selected_objs = []
         # Select according to source/destination node type/id
         for tag in self.get_all_tags(virtual=True, recurse=recurse):
             if isinstance(tag, VirtualTag):
                 if self.select_virtual_tags(
                     tag,
@@ -856,15 +972,15 @@
 
     nodes : dict of Node
         nodes in the network, e.g. pumps, tanks, or facilities
 
     connections : dict of Connections
         connections in the network, e.g. pipes
 
-    units: int, default 1
+    num_units: int, default 1
         Number of units in the network
 
     Attributes
     ----------
     id : str
         Network ID
 
@@ -878,55 +994,59 @@
         Data tags associated with this network
 
     nodes : dict of Node
         nodes in the network, e.g. pumps, tanks, or facilities
 
     connections : dict of Connections
         connections in the network, e.g. pipes
+
+    num_units : int
+        Number of networks running in parallel
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         tags={},
         nodes={},
         connections={},
-        units=1,
+        num_units=1,
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.tags = tags
         self.nodes = nodes
         self.connections = connections
-        self.units = units
+        self.num_units = num_units
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Network id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} tags:{self.tags} "
             f"nodes:{self.nodes} connections:{self.connections}>\n"
-            f"units:{self.units}>\n"
+            f"num_units:{self.num_units}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.tags == other.tags
             and self.nodes == other.nodes
             and self.connections == other.connections
+            and self.num_units == other.num_units
         )
 
     def add_node(self, node):
         """Adds a node to the network
 
         Parameters
         ----------
@@ -1014,25 +1134,25 @@
 
     input_contents : ContentsType or list of ContentsType
         Contents entering the network.
 
     output_contents : ContentsType or list of ContentsType
         Contents leaving the network.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the facility
 
-    min_flow : int
+    min_flow : pint.Quantity or int
         Minimum flow rate through the facility
 
-    max_flow : int
+    max_flow : pint.Quantity or int
         Maximum flow rate through the facility
 
-    avg_flow : int
-        Average flow rate through the facility
+    design_flow : pint.Quantity or int
+        Design flow rate through the facility
 
     tags : dict of Tag
         Data tags associated with this facility
 
     nodes : dict of Node
         nodes in the facility, e.g. pumps, tanks, or processes
 
@@ -1046,22 +1166,28 @@
 
     input_contents : list of ContentsType
         Contents entering the facility.
 
     output_contents : list of ContentsType
         Contents leaving the facility.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the facility in meters above sea level
 
     tags : dict of Tag
         Data tags associated with this facility
 
-    flow_rate : tuple
-        Tuple of minimum, maximum, and average facility flow rate
+    min_flow : pint.Quantity or int
+        Minimum flow rate through the facility
+
+    max_flow : pint.Quantity or int
+        Maximum flow rate through the facility
+
+    design_flow : pint.Quantity or int
+        Design flow rate through the facility
 
     nodes : dict of Node
         nodes in the facility, e.g. pumps, tanks, or processes
 
     connections : dict of Connections
         connections in the facility, e.g. pipes
     """
@@ -1070,34 +1196,37 @@
         self,
         id,
         input_contents,
         output_contents,
         elevation,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         tags={},
         nodes={},
         connections={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.elevation = elevation
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
         self.nodes = nodes
         self.connections = connections
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Facility id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} elevation:{self.elevation} "
-            f"flow_rate:{self.flow_rate} tags:{self.tags} "
+            f"min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} tags:{self.tags} "
             f"nodes:{self.nodes} connections:{self.connections}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
@@ -1105,16 +1234,18 @@
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.elevation == other.elevation
             and self.nodes == other.nodes
             and self.connections == other.connections
-            and self.flow_rate == other.flow_rate
             and self.tags == other.tags
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
         )
 
 
 class Pump(Node):
     """
     Parameters
     ----------
@@ -1123,31 +1254,31 @@
 
     input_contents : ContentsType or list of ContentsType
         Contents entering the pump
 
     output_contents : ContentsType or list of ContentsType
         Contents leaving the pump
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the pump in meters above sea level
 
-    horsepower : int
-        Horsepower of a single pump
+    power_rating : pint.Quantity or int
+        Rated power of a single pump (in horsepower)
 
     num_units : int
         Number of pumps running in parallel
 
-    min_flow : int
+    min_flow : pint.Quantity or int
         Minimum flow rate supplied by the pump
 
-    max_flow : int
+    max_flow : pint.Quantity or int
         Maximum flow rate supplied by the pump
 
-    avg_flow : int
-        Average flow rate supplied by the pump
+    design_flow : pint.Quantity or int
+        Design flow rate supplied by the pump
 
     pump_type : PumpType
         Type of pump (either VFD or constant)
 
     tags : dict of Tag
         Data tags associated with this pump
 
@@ -1158,110 +1289,145 @@
 
     input_contents : list of ContentsType
         Contents entering the pump
 
     output_contents : list of ContentsType
         Contents leaving the pump
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the pump in meters above sea level
 
-    horsepower : int
-        Horsepower of a single pump
+    power_rating : pint.Quantity or int
+        Rated power of a single pump (in horsepower)
 
     num_units : int
         Number of pumps running in parallel
 
-    flow_rate : tuple
-        Tuple of minimum, maximum, and average pump flow rate
+    min_flow : pint.Quantity or int
+        Minimum flow rate supplied by the pump
+
+    max_flow : pint.Quantity or int
+        Maximum flow rate supplied by the pump
+
+    design_flow : pint.Quantity or int
+        Design flow rate supplied by the pump
 
     pump_type : PumpType
         Type of pump (either VFD or constant)
 
     tags : dict of Tag
         Data tags associated with this pump
 
-    energy_efficiency : function
+    pump_curve : function
         Function which takes in the current flow rate and returns the energy
         required to pump at that rate
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
+        elevation,
         min_flow,
         max_flow,
-        avg_flow,
-        elevation,
-        horsepower,
+        design_flow,
+        power_rating,
         num_units,
         pump_type=utils.PumpType.Constant,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.elevation = elevation
         self.pump_type = pump_type
-        self.horsepower = horsepower
+        self.power_rating = power_rating
         self.num_units = num_units
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
-        self.set_energy_efficiency(None)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
+        self.set_pump_curve(None)
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Pump id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} "
-            f"flow_rate:{self.flow_rate} elevation:{self.elevation} "
-            f"horsepower:{self.horsepower} num_units:{self.num_units} "
+            f"min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} elevation:{self.elevation} "
+            f"power_rating:{self.power_rating} num_units:{self.num_units} "
             f"tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.elevation == other.elevation
             and self.pump_type == other.pump_type
-            and self.horsepower == other.horsepower
+            and self.power_rating == other.power_rating
             and self.num_units == other.num_units
             and self.tags == other.tags
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
         )
 
     def set_pump_type(self, pump_type):
         """Set the pump curve to the given function
 
         Parameters
         ----------
         pump_type : PumpType
         """
         # TODO: check that pump_type is a valid enum
         self.pump_type = pump_type
 
-    def set_energy_efficiency(self, pump_curve):
+    def set_pump_curve(self, pump_curve):
         """Set the pump curve to the given function
 
         Parameters
         ----------
         pump_curve : function
             function which takes in the current flow rate and returns the energy
             required to pump at that rate
         """
         # TODO: type check that pump_curve is a function
-        self.energy_efficiency = pump_curve
+        self.pump_curve = pump_curve
+
+    def get_power_rating(self):
+        try:
+            return self._power_rating
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `horsepower` to new `power_rating` attribute",
+                DeprecationWarning,
+            )
+            return self.horsepower
+
+    def set_power_rating(self, power_rating):
+        self._power_rating = power_rating
+
+    def del_power_rating(self):
+        del self._power_rating
+        if hasattr(self, "horsepower"):
+            warnings.warn(
+                "Please switch from `horsepower` to new `power_rating` attribute",
+                DeprecationWarning,
+            )
+            del self.horsepower
+
+    power_rating = property(get_power_rating, set_power_rating, del_power_rating)
 
 
 class Tank(Node):
     """
     Parameters
     ----------
     id : str
@@ -1269,18 +1435,18 @@
 
     input_contents : ContentsType or list of ContentsType
         Contents entering the tank.
 
     output_contents : ContentsType or list of ContentsType
         Contents leaving the tank.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the tank in meters above sea level
 
-    volume : int
+    volume : pint.Quantity or int
         Volume of the tank in cubic meters
 
     tags : dict of Tag
         Data tags associated with this tank
 
     Attributes
     ----------
@@ -1289,18 +1455,18 @@
 
     input_contents : list of ContentsType
         Contents entering the tank.
 
     output_contents : list of ContentsType
         Contents leaving the tank.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the tank in meters above sea level
 
-    volume : int
+    volume : pint.Quantity or int
         Volume of the tank in cubic meters
 
     tags : dict of Tag
         Data tags associated with this tank
     """
 
     def __init__(
@@ -1351,18 +1517,18 @@
 
     input_contents : ContentsType or list of ContentsType
         Contents entering the reservoir.
 
     output_contents : ContentsType or list of ContentsType
         Contents leaving the reservoir.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the reservoir in meters above sea level
 
-    volume : int
+    volume : pint.Quantity or int
         Volume of the reservoir in cubic meters
 
     tags : dict of Tag
         Data tags associated with this reservoir
 
     Attributes
     ----------
@@ -1371,18 +1537,18 @@
 
     input_contents : list of ContentsType
         Contents entering the reservoir.
 
     output_contents : list of ContentsType
         Contents leaving the reservoir.
 
-    elevation : int
+    elevation : pint.Quantity or int
         Elevation of the reservoir in meters above sea level
 
-    volume : int
+    volume : pint.Quantity or int
         Volume of the reservoir in cubic meters
 
     tags : dict of Tag
         Data tags associated with this reservoir
     """
 
     def __init__(
@@ -1427,80 +1593,175 @@
 class Battery(Node):
     """
     Parameters
     ----------
     id : str
         Battery ID
 
-    capacity : int
-        Storage capacity of the battery in kWh
+    energy_capacity : int
+        Energy storage capacity of the battery in kWh
+
+    charge_rate : int
+        Maximum charge rate of the battery in kW
 
     discharge_rate : int
         Maximum discharge rate of the battery in kW
 
+    rte : float
+        Round trip efficiency of the battery
+
     tags : dict of Tag
         Data tags associated with this battery
 
     Attributes
     ----------
     id : str
         Battery ID
 
     input_contents : list of ContentsType
         Contents entering the battery.
 
     output_contents : list of ContentsType
         Contents leaving the battery.
 
-    capacity : int
-        Storage capacity of the battery in kWh
+    energy_capacity : int
+        Energy storage capacity of the battery in kWh
+
+    charge_rate : int
+        Maximum discharge rate of the battery in kW
 
     discharge_rate : int
         Maximum discharge rate of the battery in kW
 
+    rte : float
+        Round trip efficiency of the battery
+
+    leakage : pint.Quantity
+        Leakage of the battery as a Pint Quantity
+
     tags : dict of Tag
         Data tags associated with this battery
     """
 
     def __init__(
         self,
         id,
-        capacity,
+        energy_capacity,
+        charge_rate,
         discharge_rate,
+        rte,
+        leakage,
         tags={},
     ):
         self.id = id
         self.input_contents = [utils.ContentsType.Electricity]
         self.output_contents = [utils.ContentsType.Electricity]
-        self.capacity = capacity
+        self.energy_capacity = energy_capacity
+        self.charge_rate = charge_rate
         self.discharge_rate = discharge_rate
+        self.rte = rte
+        self.leakage = leakage
         self.tags = tags
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Battery id:{self.id} "
             f"input_contents:{self.input_contents} "
-            f"output_contents:{self.output_contents} capacity:{self.capacity} "
-            f"discharge_rate:{self.discharge_rate} tags:{self.tags}>\n"
+            f"output_contents:{self.output_contents} "
+            f"energy_capacity:{self.energy_capacity} "
+            f"discharge_rate:{self.charge_rate} discharge_rate:{self.discharge_rate }"
+            f"rte:{self.rte} leakage:{self.leakage} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
-            and self.capacity == other.capacity
+            and self.energy_capacity == other.energy_capacity
+            and self.charge_rate == other.charge_rate
             and self.discharge_rate == other.discharge_rate
+            and self.rte == other.rte
+            and self.leakage == other.leakage
             and self.tags == other.tags
         )
 
+    def get_rte(self):
+        try:
+            return self._rte
+        except AttributeError:
+            return None
+
+    def set_rte(self, rte):
+        self._rte = rte
+
+    def del_rte(self):
+        del self._rte
+
+    def get_leakage(self):
+        try:
+            return self._leakage
+        except AttributeError:
+            return None
+
+    def set_leakage(self, leakage):
+        self._leakage = leakage
+
+    def del_leakage(self):
+        del self._leakage
+
+    def get_energy_capacity(self):
+        try:
+            return self._energy_capacity
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `capacity` to new `energy_capacity` attribute",
+                DeprecationWarning,
+            )
+            return self.capacity
+
+    def set_energy_capacity(self, energy_capacity):
+        self._energy_capacity = energy_capacity
+
+    def del_energy_capacity(self):
+        del self._energy_capacity
+        if hasattr(self, "capacity"):
+            warnings.warn(
+                "Please switch from `capacity` to new `energy_capacity` attribute",
+                DeprecationWarning,
+            )
+            del self.capacity
+
+    def get_charge_rate(self):
+        try:
+            return self._charge_rate
+        except AttributeError:
+            warnings.warn(
+                "Please add `charge_rate` in addition to `discharge_rate` attribute",
+                DeprecationWarning,
+            )
+            return self.discharge_rate
+
+    def set_charge_rate(self, charge_rate):
+        self._charge_rate = charge_rate
+
+    def del_charge_rate(self):
+        del self._charge_rate
+
+    leakage = property(get_leakage, set_leakage, del_leakage)
+    rte = property(get_rte, set_rte, del_rte)
+    charge_rate = property(get_charge_rate, set_charge_rate, del_charge_rate)
+    energy_capacity = property(
+        get_energy_capacity, set_energy_capacity, del_energy_capacity
+    )
+
 
 class Digestion(Node):
     """
     Parameters
     ----------
     id : str
         Digester ID
@@ -1508,21 +1769,21 @@
     input_contents : ContentsType or list of ContentsType
         Contents entering the digester (e.g. biogas or wastewater)
 
     output_contents : ContentsType or list of ContentsType
         Contents leaving the digester (e.g. biogas or wastewater)
 
     min_flow : int
-        Minimum flow rate through the process
+        Minimum flow rate through the digester
 
     max_flow : int
-        Maximum flow rate through the process
+        Maximum flow rate through the digester
 
-    avg_flow : int
-        Average flow rate through the process
+    design_flow : int
+        Design flow rate through the digester
 
     num_units : int
         Number of digesters running in parallel
 
     volume : int
         Volume of the digester in cubic meters
 
@@ -1545,16 +1806,22 @@
 
     num_units : int
         Number of digesters running in parallel
 
     volume : int
         Volume of the digester in cubic meters
 
-    flow_rate : tuple
-        Tuple of minimum, maximum, and average digester flow rate
+    min_flow : int
+        Minimum flow rate through the digester
+
+    max_flow : int
+        Maximum flow rate through the digester
+
+    design_flow : int
+        Design flow rate through the digester
 
     digester_type : DigesterType
         Type of digestion (aerobic or anaerobic)
 
     tags : dict of Tag
         Data tags associated with this digester
     """
@@ -1562,35 +1829,38 @@
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         digester_type,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.digester_type = digester_type
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Digestion id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} "
+            f"volume:{self.volume} min_flow:{self.min_flow} "
+            f"max_flow:{self.max_flow} design_flow:{self.design_flow} "
             f"digester_type:{self.digester_type} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
@@ -1598,15 +1868,17 @@
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
             and self.digester_type == other.digester_type
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Cogeneration(Node):
     """
     Parameters
@@ -1619,16 +1891,16 @@
 
     min_gen : int
         Minimum generation capacity of a single cogenerator
 
     max_gen : int
         Maximum generation capacity of a single cogenerator
 
-    avg_gen : int
-        Average generation capacity of a single cogenerator
+    design_gen : int
+        Design generation capacity of a single cogenerator
 
     num_units : int
         Number of cogenerator units running in parallel
 
     tags : dict of Tag
         Data tags associated with this cogenerator
 
@@ -1640,16 +1912,22 @@
     input_contents : list of ContentsType
         Contents entering the cogenerator
         (biogas, natural gas, or a blend of the two)
 
     output_contents : list of ContentsType
         Contents leaving the cogenerator (Electricity)
 
-    gen_capacity : tuple
-        Minimum, maximum, and average generation capacity
+    min_gen : int
+        Minimum generation capacity of a single cogenerator
+
+    max_gen : int
+        Maximum generation capacity of a single cogenerator
+
+    design_gen : int
+        Average generation capacity of a single cogenerator
 
     num_units : int
         Number of cogenerator units running in parallel
 
     tags : dict of Tag
         Data tags associated with this cogenerator
 
@@ -1659,62 +1937,133 @@
 
     thermal_efficiency : function
         Function which takes in the current kWh and returns
         the thermal efficiency as a fraction
     """
 
     def __init__(
-        self, id, input_contents, min_gen, max_gen, avg_gen, num_units, tags={}
+        self, id, input_contents, min_gen, max_gen, design_gen, num_units, tags={}
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.output_contents = [utils.ContentsType.Electricity, utils.ContentsType.Heat]
         self.num_units = num_units
         self.tags = tags
-        self.set_gen_capacity(min_gen, max_gen, avg_gen)
+        self.min_gen = min_gen
+        self.max_gen = max_gen
+        self.design_gen = design_gen
         self.set_electrical_efficiency(None)
         self.set_thermal_efficiency(None)
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Cogeneration id:{self.id} "
             f"input_contents:{self.input_contents} "
-            f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"gen_capacity:{self.gen_capacity} tags:{self.tags}>\n"
+            f"output_contents:{self.output_contents} min_gen:{self.min_gen} "
+            f"max_gen:{self.max_gen} design_gen:{self.design_gen} "
+            f"num_units:{self.num_units} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
-            and self.gen_capacity == other.gen_capacity
+            and self.min_gen == other.min_gen
+            and self.max_gen == other.max_gen
+            and self.design_gen == other.design_gen
             and self.tags == other.tags
         )
 
-    def set_gen_capacity(self, min, max, avg):
+    def set_gen_capacity(self, min, max, design):
         """Set the minimum, maximum, and average generation capacity
 
         Parameters
         ----------
         min : int
             Minimum generation by a single cogenerator
 
         max : int
             Maximum generation by a single cogenerator
 
-        avg : int
-            Average generation by a single cogenerator
+        design : int
+            Design generation by a single cogenerator
         """
-        self.gen_capacity = (min, max, avg)
+        warnings.warn(
+            "Please switch from `gen_capacity` tuple to new separate "
+            + "`min_gen`, `max_gen` and `design_gen` attributes",
+            DeprecationWarning,
+        )
+        self.gen_capacity = (min, max, design)
+        self._min_gen = min
+        self._max_gen = max
+        self._design_gen = design
+
+    def get_min_gen(self):
+        try:
+            return self._min_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `min_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[0]
+
+    def set_min_gen(self, min_gen):
+        self._min_gen = min_gen
+
+    def del_min_gen(self):
+        del self._min_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity = (None, self.gen_capacity[1], self.gen_capacity[2])
+
+    def get_max_gen(self):
+        try:
+            return self._max_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `max_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[1]
+
+    def set_max_gen(self, max_gen):
+        self._max_gen = max_gen
+
+    def del_max_gen(self):
+        del self._max_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity = (self.gen_capacity[0], None, self.gen_capacity[2])
+
+    def get_design_gen(self):
+        try:
+            return self._design_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `design_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[2]
+
+    def set_design_gen(self, design_gen):
+        self._design_gen = design_gen
+
+    def del_design_gen(self):
+        del self._design_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity = (self.gen_capacity[0], self.gen_capacity[1], None)
+
+    min_gen = property(get_min_gen, set_min_gen, del_min_gen)
+    max_gen = property(get_max_gen, set_max_gen, del_max_gen)
+    design_gen = property(get_design_gen, set_design_gen, del_design_gen)
 
     def set_electrical_efficiency(self, efficiency_curve):
         """Set the cogeneration efficiency to the given function
 
         Parameters
         ----------
         efficiency_curve : function
@@ -1747,16 +2096,16 @@
 
     min_gen : int
         Minimum generation capacity of a single boiler
 
     max_gen : int
         Maximum generation capacity of a single boiler
 
-    avg_gen : int
-        Average generation capacity of a single boiler
+    design_gen : int
+        Design generation capacity of a single boiler
 
     num_units : int
         Number of boiler units running in parallel
 
     tags : dict of Tag
         Data tags associated with this boiler
 
@@ -1768,76 +2117,151 @@
     input_contents : list of ContentsType
         Contents entering the boiler
         (biogas, natural gas, or a blend of the two)
 
     output_contents : list of ContentsType
         Contents leaving the boiler (Electricity)
 
-    gen_capacity : tuple
-        Minimum, maximum, and average generation capacity
+    min_gen : int
+        Minimum generation capacity of a single boiler
+
+    max_gen : int
+        Maximum generation capacity of a single boiler
+
+    design_gen : int
+        Design generation capacity of a single boiler
+
 
     num_units : int
         Number of boiler units running in parallel
 
     tags : dict of Tag
         Data tags associated with this boiler
 
     thermal_efficiency : function
         Function which takes in the current kWh and returns
         the efficiency as a fraction
     """
 
     def __init__(
-        self, id, input_contents, min_gen, max_gen, avg_gen, num_units, tags={}
+        self, id, input_contents, min_gen, max_gen, design_gen, num_units, tags={}
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.output_contents = [utils.ContentsType.Heat]
         self.num_units = num_units
         self.tags = tags
-        self.set_gen_capacity(min_gen, max_gen, avg_gen)
+        self.min_gen = min_gen
+        self.max_gen = max_gen
+        self.design_gen = design_gen
         self.set_thermal_efficiency(None)
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Boiler id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"gen_capacity:{self.gen_capacity} tags:{self.tags}>\n"
+            f"min_gen:{self.min_gen} max_gen:{self.max_gen} "
+            f"design_gen:{self.design_gen} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
-            and self.gen_capacity == other.gen_capacity
+            and self.min_gen == other.min_gen
+            and self.max_gen == other.max_gen
+            and self.design_gen == other.design_gen
             and self.tags == other.tags
         )
 
-    def set_gen_capacity(self, min, max, avg):
+    def set_gen_capacity(self, min, max, design):
         """Set the minimum, maximum, and average generation capacity
 
         Parameters
         ----------
         min : int
             Minimum generation by a single cogenerator
 
         max : int
             Maximum generation by a single cogenerator
 
-        avg : int
-            Average generation by a single cogenerator
+        design : int
+            Design generation by a single cogenerator
         """
-        self.gen_capacity = (min, max, avg)
+        warnings.warn(
+            "Please switch from `gen_capacity` tuple to new separate "
+            + "`min_gen`, `max_gen` and `design_gen` attributes",
+            DeprecationWarning,
+        )
+        self.gen_capacity = (min, max, design)
+
+    def get_min_gen(self):
+        try:
+            return self._min_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `min_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[0]
+
+    def set_min_gen(self, min_gen):
+        self._min_gen = min_gen
+
+    def del_min_gen(self):
+        del self._min_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity[0] = None
+
+    def get_max_gen(self):
+        try:
+            return self._max_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `max_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[1]
+
+    def set_max_gen(self, max_gen):
+        self._max_gen = max_gen
+
+    def del_max_gen(self):
+        del self._max_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity[1] = None
+
+    def get_design_gen(self):
+        try:
+            return self._design_gen
+        except AttributeError:
+            warnings.warn(
+                "Please switch from `gen_capacity` tuple to new `design_gen` attribute",
+                DeprecationWarning,
+            )
+            return self.gen_capacity[2]
+
+    def set_design_gen(self, design_gen):
+        self._design_gen = design_gen
+
+    def del_design_gen(self):
+        del self._design_gen
+        if hasattr(self, "gen_capacity"):
+            self.gen_capacity[2] = None
+
+    min_gen = property(get_min_gen, set_min_gen, del_min_gen)
+    max_gen = property(get_max_gen, set_max_gen, del_max_gen)
+    design_gen = property(get_design_gen, set_design_gen, del_design_gen)
 
     def set_thermal_efficiency(self, efficiency_curve):
         """Set the cogeneration efficiency to the given function
 
         Parameters
         ----------
         efficiency_curve : function
@@ -1862,16 +2286,16 @@
 
     min_flow : int
         Minimum flow rate of a single clarifier
 
     max_flow : int
         Maximum flow rate of a single clarifier
 
-    avg_flow : int
-        Average flow rate of a single clarifier
+    design_flow : int
+        Design flow rate of a single clarifier
 
     num_units : int
         Number of clarifiers running in parallel
 
     volume : int
         Volume of the clarifier in cubic meters
 
@@ -1891,61 +2315,72 @@
 
     num_units : int
         Number of clarifiers running in parallel
 
     volume : int
         Volume of a single clarifier in cubic meters
 
-    flow_rate : tuple
-        Tuple of minimum, maximum, and average digester flow rate
+    min_flow : int
+        Minimum flow rate of a single clarifier
+
+    max_flow : int
+        Maximum flow rate of a single clarifier
+
+    design_flow : int
+        Design flow rate of a single clarifier
 
     tags : dict of Tag
         Data tags associated with this clarifier
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Clarification id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"volume:{self.volume} min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Filtration(Node):
     """
     Parameters
@@ -1961,16 +2396,16 @@
 
     min_flow : int
         Minimum flow rate of a single filter
 
     max_flow : int
         Maximum flow rate of a single filter
 
-    avg_flow : int
-        Average flow rate of a single filter
+    design_flow : int
+        Design flow rate of a single filter
 
     num_units : int
         Number of filters running in parallel
 
     volume : int
         Volume of a single filter in cubic meters
 
@@ -1990,61 +2425,72 @@
 
     num_units : int
         Number of filters running in parallel
 
     volume : int
         Volume of a single filter in cubic meters
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single filter
+
+    max_flow : int
+        Maximum flow rate of a single filter
+
+    design_flow : int
+        Design flow rate of a single filter
 
     tags : dict of Tag
         Data tags associated with this filter
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Filtration id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"volume:{self.volume} min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Screening(Node):
     """
     Parameters
@@ -2060,16 +2506,16 @@
 
     min_flow : int
         Minimum flow rate of a single screen
 
     max_flow : int
         Maximum flow rate of a single screen
 
-    avg_flow : int
-        Average flow rate of a single screen
+    design_flow : int
+        Design flow rate of a single screen
 
     num_units : int
         Number of screens running in parallel
 
     tags : dict of Tag
         Data tags associated with this screen
 
@@ -2083,58 +2529,69 @@
 
     output_contents : list of ContentsType
         Contents leaving the screen
 
     num_units : int
         Number of screens running in parallel
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single screen
+
+    max_flow : int
+        Maximum flow rate of a single screen
+
+    design_flow : int
+        Design flow rate of a single screen
 
     tags : dict of Tag
         Data tags associated with this screen
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Screening id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Conditioning(Node):
     """
     Parameters
@@ -2150,16 +2607,16 @@
 
     min_flow : int
         Minimum flow rate of a single biogas conditioner
 
     max_flow : int
         Maximum flow rate of a single biogas conditioner
 
-    avg_flow : int
-        Average flow rate of a single biogas conditioner
+    design_flow : int
+        Design flow rate of a single biogas conditioner
 
     num_units : int
         Number of biogas conditioners running in parallel
 
     tags : dict of Tag
         Data tags associated with this biogas conditioner
 
@@ -2173,58 +2630,69 @@
 
     output_contents : list of ContentsType
         Contents leaving the biogas conditioner
 
     num_units : int
         Number of biogas conditioners running in parallel
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single biogas conditioner
+
+    max_flow : int
+        Maximum flow rate of a single biogas conditioner
+
+    design_flow : int
+        Design flow rate of a single biogas conditioner
 
     tags : dict of Tag
         Data tags associated with this screen
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Conditioning id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"min_flow:{self.min_flow} max_flow:{self.max_flow} "
+            f"design_flow:{self.design_flow} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Thickening(Node):
     """
     Parameters
@@ -2240,16 +2708,16 @@
 
     min_flow : int
         Minimum flow rate of a single thickener
 
     max_flow : int
         Maximum flow rate of a single thickener
 
-    avg_flow : int
-        Average flow rate of a single thickener
+    design_flow : int
+        Design flow rate of a single thickener
 
     num_units : int
         Number of thickeners running in parallel
 
     volume : int
         Volume of a single thickener in cubic meters
 
@@ -2269,61 +2737,73 @@
 
     num_units : int
         Number of thickeners running in parallel
 
     volume : int
         Volume of a single thickener in cubic meters
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single thickener
+
+    max_flow : int
+        Maximum flow rate of a single thickener
+
+    design_flow : int
+        Design flow rate of a single thickener
 
     tags : dict of Tag
         Data tags associated with this thickener
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Thickening id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"volume:{self.volume} min_flow:{self.min_flow} "
+            f"max_flow:{self.max_flow} design_flow:{self.design_flow} "
+            f"tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Aeration(Node):
     """
     Parameters
@@ -2339,16 +2819,16 @@
 
     min_flow : int
         Minimum flow rate of a single aeration basin
 
     max_flow : int
         Maximum flow rate of a single aeration basin
 
-    avg_flow : int
-        Average flow rate of a single aeration basin
+    design_flow : int
+        Design flow rate of a single aeration basin
 
     num_units : int
         Number of aeration basins running in parallel
 
     volume : int
         Volume of a single aeration basin in cubic meters
 
@@ -2368,61 +2848,73 @@
 
     num_units : int
         Number of aeration basins running in parallel
 
     volume : int
         Volume of a single aeration basin in cubic meters
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single aeration basin
+
+    max_flow : int
+        Maximum flow rate of a single aeration basin
+
+    design_flow : int
+        Design flow rate of a single aeration basin
 
     tags : dict of Tag
         Data tags associated with this aerator
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Aeration id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"volume:{self.volume} min_flow:{self.min_flow} "
+            f"max_flow:{self.max_flow} design_flow:{self.design_flow} "
+            f"tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Chlorination(Node):
     """
     Parameters
@@ -2438,16 +2930,16 @@
 
     min_flow : int
         Minimum flow rate of a single chlorinator
 
     max_flow : int
         Maximum flow rate of a single chlorinator
 
-    avg_flow : int
-        Average flow rate of a single chlorinator
+    design_flow : int
+        Design flow rate of a single chlorinator
 
     num_units : int
         Number of chlorinators running in parallel
 
     volume : int
         Volume of a single chlorinator in cubic meters
 
@@ -2467,61 +2959,73 @@
 
     num_units : int
         Number of chlorinators running in parallel
 
     volume : int
         Volume of a single chlorinator in cubic meters
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single chlorinator
+
+    max_flow : int
+        Maximum flow rate of a single chlorinator
+
+    design_flow : int
+        Design flow rate of a single chlorinator
 
     tags : dict of Tag
         Data tags associated with this chlorinator
     """
 
     def __init__(
         self,
         id,
         input_contents,
         output_contents,
         min_flow,
         max_flow,
-        avg_flow,
+        design_flow,
         num_units,
         volume,
         tags={},
     ):
         self.id = id
         self.set_contents(input_contents, "input_contents")
         self.set_contents(output_contents, "output_contents")
         self.num_units = num_units
         self.volume = volume
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Chlorination id:{self.id} "
             f"input_contents:{self.input_contents} "
             f"output_contents:{self.output_contents} num_units:{self.num_units} "
-            f"volume:{self.volume} flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"volume:{self.volume} min_flow:{self.min_flow} "
+            f"max_flow:{self.max_flow} design_flow:{self.design_flow} "
+            f" tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.output_contents == other.output_contents
             and self.num_units == other.num_units
             and self.volume == other.volume
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
 
 
 class Flaring(Node):
     """
     Parameters
@@ -2534,16 +3038,16 @@
 
     min_flow : int
         Minimum flow rate of a single flare
 
     max_flow : int
         Maximum flow rate of a single flare
 
-    avg_flow : int
-        Average flow rate of a single flare
+    design_flow : int
+        Design flow rate of a single flare
 
     tags : dict of Tag
         Data tags associated with this flare
 
     Attributes
     ----------
     id : str
@@ -2551,40 +3055,51 @@
 
     input_contents : list of ContentsType
         Contents entering the flare
 
     num_units : int
         Number of flares running in parallel
 
-    flow_rate : tuple
-        Minimum, maximum, and average flow rate
+    min_flow : int
+        Minimum flow rate of a single flare
+
+    max_flow : int
+        Maximum flow rate of a single flare
+
+    design_flow : int
+        Design flow rate of a single flare
 
     tags : dict of Tag
         Data tags associated with this flare
     """
 
-    def __init__(self, id, num_units, min_flow, max_flow, avg_flow, tags={}):
+    def __init__(self, id, num_units, min_flow, max_flow, design_flow, tags={}):
         self.id = id
         self.input_contents = [utils.ContentsType.Biogas]
         self.num_units = num_units
         self.tags = tags
-        self.set_flow_rate(min_flow, max_flow, avg_flow)
+        self.min_flow = min_flow
+        self.max_flow = max_flow
+        self.design_flow = design_flow
 
     def __repr__(self):
         return (
             f"<pype_schema.node.Flaring id:{self.id} "
             f"input_contents:{self.input_contents} num_units:{self.num_units} "
-            f"flow_rate:{self.flow_rate} tags:{self.tags}>\n"
+            f"min_flow:{self.min_flow} max_flow:{self.max_flow}"
+            f"design_flow:{self.design_flow} tags:{self.tags}>\n"
         )
 
     def __eq__(self, other):
         # don't attempt to compare against unrelated types
         if not isinstance(other, self.__class__):
             return False
 
         return (
             self.id == other.id
             and self.input_contents == other.input_contents
             and self.num_units == other.num_units
-            and self.flow_rate == other.flow_rate
+            and self.min_flow == other.min_flow
+            and self.max_flow == other.max_flow
+            and self.design_flow == other.design_flow
             and self.tags == other.tags
         )
```

### Comparing `pype-schema-0.5.0/pype_schema/operations.py` & `pype-schema-0.5.1/pype_schema/operations.py`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/pype_schema/parse_json.py` & `pype-schema-0.5.1/pype_schema/parse_json.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import json
+import pint
+import warnings
 from .tag import TagType, Tag, VirtualTag, CONTENTLESS_TYPES
 from . import connection
 from . import node
 from . import utils
 
 
 class JSONParser:
@@ -226,60 +228,130 @@
 
         Returns
         -------
         Node
             a Python object with all the values from key `node_id`
         """
         (input_contents, output_contents) = self.parse_contents(node_id)
-        elevation = utils.parse_quantity(
-            self.config[node_id].get("elevation (meters)"), "m"
-        )
+        elevation = self.parse_unit_val_dict(self.config[node_id].get("elevation"))
+        # strings like `elevation (meters)` and `volume (cubic meters)`
+        # are included for backwards compatability
+        if elevation is None:
+            elevation = utils.parse_quantity(
+                self.config[node_id].get("elevation (meters)"), "m"
+            )
+            warnings.warn(
+                "Please switch to new dictionary syntax for elevation with units",
+                FutureWarning,
+            )
         num_units = self.config[node_id].get("num_units")
-        volume = utils.parse_quantity(
-            self.config[node_id].get("volume (cubic meters)"), "m3"
-        )
+        volume = self.parse_unit_val_dict(self.config[node_id].get("volume"))
+        if volume is None:
+            volume = utils.parse_quantity(
+                self.config[node_id].get("volume (cubic meters)"), "m3"
+            )
+            warnings.warn(
+                "Please switch to new dictionary syntax for volume with units",
+                FutureWarning,
+            )
 
-        min_flow, max_flow, avg_flow = self.parse_min_max_avg(
-            self.config[node_id].get("flowrate")
-        )
+        flowrate = self.config[node_id].get("flowrate")
+        if flowrate is None:
+            flowrate = self.config[node_id].get("flow_rate")
+
+        min_flow, max_flow, design_flow = self.parse_min_max_design(flowrate)
 
         # create correct type of node class
         if self.config[node_id]["type"] == "Network":
+            if num_units is None:
+                num_units = 1
+
             node_obj = node.Network(
                 node_id,
                 input_contents,
                 output_contents,
                 tags={},
                 nodes={},
                 connections={},
+                num_units=num_units,
             )
 
             for new_node in self.config[node_id]["nodes"]:
                 node_obj.add_node(self.create_node(new_node))
             for new_connection in self.config[node_id]["connections"]:
                 node_obj.add_connection(
                     self.create_connection(new_connection, node_obj)
                 )
         elif self.config[node_id]["type"] == "Battery":
-            capacity = utils.parse_quantity(
-                self.config[node_id].get("capacity (kWh)"), "kwh"
+            energy_capacity = self.parse_unit_val_dict(
+                self.config[node_id].get("energy_capacity")
             )
-            discharge_rate = utils.parse_quantity(
-                self.config[node_id].get("discharge_rate (kW)"), "kw"
+            discharge_rate = self.parse_unit_val_dict(
+                self.config[node_id].get("discharge_rate")
+            )
+            charge_rate = self.parse_unit_val_dict(
+                self.config[node_id].get("charge_rate")
+            )
+            if energy_capacity is None:
+                energy_capacity = utils.parse_quantity(
+                    self.config[node_id].get("capacity (kWh)"), "kwh"
+                )
+                warnings.warn(
+                    "Please switch to new dictionary syntax "
+                    + "for energy capacity with units",
+                    FutureWarning,
+                )
+            if discharge_rate is None:
+                discharge_rate = utils.parse_quantity(
+                    self.config[node_id].get("discharge_rate (kW)"), "kw"
+                )
+                warnings.warn(
+                    "Please switch to new dictionary syntax "
+                    + "for discharge rate with units",
+                    FutureWarning,
+                )
+            if charge_rate is None:
+                charge_rate = utils.parse_quantity(
+                    self.config[node_id].get("charge_rate (kW)"), "kw"
+                )
+                warnings.warn(
+                    "Please switch to new dictionary syntax for charge rate with units",
+                    FutureWarning,
+                )
+            # if either discharge or charge rate are null assume they are the same
+            if discharge_rate is None and charge_rate is None:
+                warnings.warn(
+                    "Battery object {} has no charge or discharge rate defined".format(
+                        node_id
+                    )
+                )
+            elif charge_rate is None:
+                charge_rate = discharge_rate
+            elif discharge_rate is None:
+                discharge_rate = charge_rate
+            rte = self.config[node_id].get("rte")
+            leakage = self.parse_unit_val_dict(self.config[node_id].get("leakage"))
+            node_obj = node.Battery(
+                node_id,
+                energy_capacity,
+                charge_rate,
+                discharge_rate,
+                rte,
+                leakage,
+                tags={},
             )
-            node_obj = node.Battery(node_id, capacity, discharge_rate, tags={})
         elif self.config[node_id]["type"] == "Facility":
             node_obj = node.Facility(
                 node_id,
                 input_contents,
                 output_contents,
                 elevation,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 tags={},
                 nodes={},
                 connections={},
             )
 
             for new_node in self.config[node_id]["nodes"]:
                 node_obj.add_node(self.create_node(new_node))
@@ -289,42 +361,56 @@
                 )
         elif self.config[node_id]["type"] == "Pump":
             pump_type = self.config[node_id].get("pump_type")
             if pump_type is None:
                 pump_type = utils.PumpType.Constant
             else:
                 pump_type = utils.PumpType[pump_type]
-            horsepower = utils.parse_quantity(
-                self.config[node_id].get("horsepower"), "hp"
+
+            power_rating = self.parse_unit_val_dict(
+                self.config[node_id].get("power_rating")
             )
+            if power_rating is None:
+                power_rating = utils.parse_quantity(
+                    self.config[node_id].get("horsepower"), "hp"
+                )
+                warnings.warn(
+                    "Please switch to new dictionary syntax "
+                    + "for power rating with units",
+                    FutureWarning,
+                )
             node_obj = node.Pump(
                 node_id,
                 input_contents,
                 output_contents,
+                elevation,
                 min_flow,
                 max_flow,
-                avg_flow,
-                elevation,
-                horsepower,
+                design_flow,
+                power_rating,
                 num_units,
                 pump_type=pump_type,
                 tags={},
             )
 
             efficiency = self.config[node_id].get("efficiency")
-            if efficiency:
+            if efficiency is None:
+                pump_curve = self.config[node_id].get("pump_curve")
+            else:
+                pump_curve = efficiency
+            if pump_curve:
 
                 def efficiency_curve(arg):
                     # TODO: fix this so that it interpolates between dictionary values
-                    if type(efficiency) is dict:
-                        return efficiency[arg]
+                    if type(pump_curve) is dict:
+                        return pump_curve[arg]
                     else:
-                        return float(efficiency)
+                        return float(pump_curve)
 
-                node_obj.set_energy_efficiency(efficiency_curve)
+                node_obj.set_pump_curve(efficiency_curve)
         elif self.config[node_id]["type"] == "Reservoir":
             node_obj = node.Reservoir(
                 node_id, input_contents, output_contents, elevation, volume, tags={}
             )
         elif self.config[node_id]["type"] == "Tank":
             node_obj = node.Tank(
                 node_id, input_contents, output_contents, elevation, volume, tags={}
@@ -332,46 +418,53 @@
         elif self.config[node_id]["type"] == "Aeration":
             node_obj = node.Aeration(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Clarification":
             node_obj = node.Clarification(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 tags={},
             )
         elif self.config[node_id]["type"] in ["Cogeneration", "Boiler"]:
-            min, max, avg = self.parse_min_max_avg(
-                self.config[node_id].get("generation_capacity")
-            )
+            gen_capacity = self.config[node_id].get("generation_capacity")
+            if gen_capacity is None:
+                self.config[node_id].get("gen_capacity")
+            min, max, design = self.parse_min_max_design(gen_capacity)
             if self.config[node_id]["type"] == "Cogeneration":
                 node_obj = node.Cogeneration(
-                    node_id, input_contents, min, max, avg, num_units, tags={}
+                    node_id, input_contents, min, max, design, num_units, tags={}
                 )
                 electrical_efficiency = self.config[node_id].get(
                     "electrical efficiency"
                 )
+                if electrical_efficiency is None:
+                    electrical_efficiency = self.config[node_id].get(
+                        "electrical_efficiency"
+                    )
                 thermal_efficiency = self.config[node_id].get("thermal efficiency")
+                if thermal_efficiency is None:
+                    thermal_efficiency = self.config[node_id].get("thermal_efficiency")
             else:
                 node_obj = node.Boiler(
-                    node_id, input_contents, min, max, avg, num_units, tags={}
+                    node_id, input_contents, min, max, design, num_units, tags={}
                 )
                 electrical_efficiency = None
                 thermal_efficiency = self.config[node_id].get("thermal efficiency")
 
             if electrical_efficiency:
 
                 def efficiency_curve(arg):
@@ -397,84 +490,84 @@
             digester_type = self.config[node_id].get("digester_type")
             node_obj = node.Digestion(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 utils.DigesterType[digester_type],
                 tags={},
             )
         elif self.config[node_id]["type"] == "Filtration":
             node_obj = node.Filtration(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Chlorination":
             node_obj = node.Chlorination(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Flaring":
             node_obj = node.Flaring(
                 node_id,
                 num_units,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Thickening":
             node_obj = node.Thickening(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 volume,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Screening":
             node_obj = node.Screening(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 tags={},
             )
         elif self.config[node_id]["type"] == "Conditioning":
             node_obj = node.Conditioning(
                 node_id,
                 input_contents,
                 output_contents,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 num_units,
                 tags={},
             )
         else:
             raise TypeError("Unsupported Node type: " + self.config[node_id]["type"])
 
         tags = self.config[node_id].get("tags")
@@ -554,39 +647,52 @@
         if dest_id:
             destination = node_obj.get_node(dest_id)
 
         entry_point = self.config[connection_id].get("entry_point")
         if entry_point:
             entry_point = destination.get_node(entry_point)
 
-        min_flow, max_flow, avg_flow = self.parse_min_max_avg(
-            self.config[connection_id].get("flowrate")
-        )
-        min_pres, max_pres, avg_pres = self.parse_min_max_avg(
+        flowrate = self.config[connection_id].get("flowrate")
+        if flowrate is None:
+            flowrate = self.config[connection_id].get("flow_rate")
+
+        min_flow, max_flow, design_flow = self.parse_min_max_design(flowrate)
+        min_pres, max_pres, design_pres = self.parse_min_max_design(
             self.config[connection_id].get("pressure")
         )
         lower, higher = self.parse_heating_values(
             self.config[connection_id].get("heating_values")
         )
 
         if self.config[connection_id]["type"] == "Pipe":
-            diameter = utils.parse_quantity(
-                self.config[connection_id].get("diameter (inches)"), "in"
+            diameter = self.parse_unit_val_dict(
+                self.config[connection_id].get("diameter")
             )
+            if diameter is None:
+                diameter = utils.parse_quantity(
+                    self.config[connection_id].get("diameter (inches)"), "in"
+                )
+                warnings.warn(
+                    "Please switch to new dictionary syntax for diamter with units",
+                    FutureWarning,
+                )
             connection_obj = connection.Pipe(
                 connection_id,
                 contents,
                 source,
                 destination,
                 min_flow,
                 max_flow,
-                avg_flow,
+                design_flow,
                 diameter=diameter,
                 lower_heating_value=lower,
                 higher_heating_value=higher,
+                min_pres=min_pres,
+                max_pres=max_pres,
+                design_pres=design_pres,
                 tags={},
                 bidirectional=bidirectional,
                 exit_point=exit_point,
                 entry_point=entry_point,
             )
         elif self.config[connection_id]["type"] == "Wire":
             connection_obj = connection.Wire(
@@ -979,69 +1085,131 @@
                     contents = obj.input_contents[0]
                 else:
                     raise ValueError("Ambiguous contents definition for tag " + tag_id)
 
         return contents
 
     @staticmethod
-    def parse_min_max_avg(min_max_avg):
+    def parse_min_max_design(min_max_design):
         """Converts a dictionary into a tuple of flow rates
 
         Parameters
         ----------
-        min_max_avg : dict
+        min_max_design : dict
             dictionary of the form {
                 ``min``: `int`
 
                 ``max``: `int`
 
-                ``avg``: `int`
+                ``design``: `int`
 
             }
 
         Returns
         -------
-        (Quantity, Quantity, Quantity) or (float, float, float)
+        (pint.Quantity, pint.Quantity, pint.Quantity) or (float, float, float)
             (min, max, and average) with the given Pint units as a tuple.
             If no units given, then returns a tuple of floats.
         """
-        if min_max_avg is None:
+        if min_max_design is None:
             return (None, None, None)
         else:
-            units = min_max_avg.get("units")
+            units = min_max_design.get("units")
+
+            # field name was changed from 'avg' to 'design'
+            # so this code is included for backwards compatability
+            design_val = min_max_design.get("design")
+            if design_val is None:
+                design_val = min_max_design.get("avg")
             if units:
                 return (
-                    utils.parse_quantity(min_max_avg.get("min"), units),
-                    utils.parse_quantity(min_max_avg.get("max"), units),
-                    utils.parse_quantity(min_max_avg.get("avg"), units),
+                    utils.parse_quantity(min_max_design.get("min"), units),
+                    utils.parse_quantity(min_max_design.get("max"), units),
+                    utils.parse_quantity(design_val, units),
                 )
             else:
                 return (
-                    min_max_avg.get("min"),
-                    min_max_avg.get("max"),
-                    min_max_avg.get("avg"),
+                    min_max_design.get("min"),
+                    min_max_design.get("max"),
+                    design_val,
                 )
 
     @staticmethod
+    def unit_val_to_dict(attribute):
+        """Converts the given attribute to dictionary of the form {
+                ``value``: ``float``
+
+                ``units``: `str`
+
+            }
+
+        Parameters
+        ----------
+        attribute : pint.Quantity or float
+            Attribute to represent as a dictionary
+
+        Returns
+        -------
+        dict
+            Dictionary with keys ``value`` and ``units``
+        """
+        if isinstance(attribute, pint.Quantity):
+            data_dict = {"value": attribute.magnitude, "units": str(attribute.units)}
+        else:
+            data_dict = {"value": attribute, "units": None}
+        return data_dict
+
+    @staticmethod
+    def parse_unit_val_dict(unit_dict):
+        """Converts a dictionary into a Pint Quantity
+
+        Parameters
+        ----------
+        unit_dict : dict
+            dictionary of the form {
+                ``value``: ``float``
+
+                ``units``: `str`
+
+            }
+
+        Returns
+        -------
+        pint.Quantity or float
+            Dictionary as a Pint Quantity (or float if no units are specified)
+        """
+        if unit_dict is not None:
+            val = unit_dict.get("value")
+            units = unit_dict.get("units")
+            if units is None:
+                return val
+            else:
+                return utils.parse_quantity(val, units)
+        else:
+            return None
+
+    @staticmethod
     def parse_heating_values(heating_vals):
         """Converts a dictionary into a tuple of flow rates
 
         Parameters
         ----------
         heating_vals : dict
             dictionary of the form {
                 ``lower``: `float`
 
                 ``higher``: `float`
 
+                ``units``: `str`
+
             }
 
         Returns
         -------
-        (Quantity, Quantity) or (float, float)
+        (pint.Quantity, pint.Quantity) or (float, float)
             (lower, higher) heating values as a tuple, with units applied.
             Given as a float if no units are specified
         """
         if heating_vals is None:
             return (None, None)
         else:
             units = heating_vals.get("units")
@@ -1089,15 +1257,15 @@
         tag_dict["type"] = tag_obj.tag_type.name
         if tag_obj.tag_type not in CONTENTLESS_TYPES:
             tag_dict["contents"] = tag_obj.contents.name
 
         return tag_dict
 
     @staticmethod
-    def min_max_avg_to_dict(obj, attribute):
+    def min_max_design_to_dict(obj, attribute):
         """Converts the flow rate tuple of a `Node` or `Connection` into a
         dictionary object
 
         Parameters
         ----------
         obj : Node or Connection
             object to get `attribute` of and convert it to a dictionary
@@ -1109,35 +1277,49 @@
         -------
         dict
             flow rate in the form {
                 ``min``: `float` or `int`
 
                 ``max``: `float` or `int`
 
-                ``avg``: `float` or `int`
+                ``design``: `float` or `int`
 
                 ``units``: `str`
 
             }
         """
-        min_max_avg_dict = {"min": None, "max": None, "avg": None, "units": None}
-        values = getattr(obj, attribute)
+        min_max_design_dict = {"min": None, "max": None, "design": None, "units": None}
+        # try/except for backwards compatability with flow_rate and gen_capacity tuples
+        try:
+            values = getattr(obj, attribute)
+        except AttributeError:
+            if attribute == "flow_rate":
+                suffix = "flow"
+            elif attribute == "gen_capacity":
+                suffix = "gen"
+            else:
+                suffix = attribute
+            values = (
+                getattr(obj, "min_" + suffix),
+                getattr(obj, "max_" + suffix),
+                getattr(obj, "design_" + suffix),
+            )
         if values[0] is not None:
-            min_max_avg_dict["min"] = values[0].magnitude
-            min_max_avg_dict["units"] = "{!s}".format(values[0].units)
+            min_max_design_dict["min"] = values[0].magnitude
+            min_max_design_dict["units"] = "{!s}".format(values[0].units)
 
         if values[1] is not None:
-            min_max_avg_dict["max"] = values[1].magnitude
-            min_max_avg_dict["units"] = "{!s}".format(values[1].units)
+            min_max_design_dict["max"] = values[1].magnitude
+            min_max_design_dict["units"] = "{!s}".format(values[1].units)
 
         if values[2] is not None:
-            min_max_avg_dict["avg"] = values[2].magnitude
-            min_max_avg_dict["units"] = "{!s}".format(values[2].units)
+            min_max_design_dict["design"] = values[2].magnitude
+            min_max_design_dict["units"] = "{!s}".format(values[2].units)
 
-        return min_max_avg_dict
+        return min_max_design_dict
 
     @staticmethod
     def conn_to_dict(conn_obj):
         """Converts a Connection object to a dictionary that can be
         parsed into JSON format
 
         Parameters
@@ -1160,32 +1342,34 @@
         if conn_obj.exit_point is not None:
             conn_dict["exit_point"] = conn_obj.exit_point.id
 
         if conn_obj.entry_point is not None:
             conn_dict["entry_point"] = conn_obj.entry_point.id
 
         if isinstance(conn_obj, connection.Pipe):
-            conn_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+            conn_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                 conn_obj, "flow_rate"
             )
-            conn_dict["pressure"] = JSONParser.min_max_avg_to_dict(conn_obj, "pressure")
+            conn_dict["pressure"] = JSONParser.min_max_design_to_dict(
+                conn_obj, "pressure"
+            )
 
             heat_dict = {"lower": None, "higher": None, "units": "BTU/scf"}
             if conn_obj.heating_values[0] is not None:
                 heat_dict["lower"] = conn_obj.heating_values[0].magnitude
                 heat_dict["units"] = "{!s}".format(conn_obj.heating_values[0].units)
 
             if conn_obj.heating_values[1] is not None:
                 heat_dict["higher"] = conn_obj.heating_values[1].magnitude
                 heat_dict["units"] = "{!s}".format(conn_obj.heating_values[1].units)
 
             conn_dict["heating_values"] = heat_dict
 
             if conn_obj.diameter is not None:
-                conn_dict["diameter (inches)"] = conn_obj.diameter.magnitude
+                conn_dict["diameter"] = JSONParser.unit_val_to_dict(conn_obj.diameter)
 
         # TODO: unsupported attribute: friction_coeff
 
         tag_dict = {}
         v_tag_dict = {}
         for tag_id, tag_obj in conn_obj.tags.items():
             if isinstance(tag_obj, Tag):
@@ -1242,73 +1426,82 @@
                 v_tag_dict[tag_id] = JSONParser.tag_to_dict(tag_obj)
 
         node_dict["tags"] = tag_dict
         node_dict["virtual_tags"] = v_tag_dict
 
         if isinstance(node_obj, (node.Tank, node.Reservoir)):
             if node_obj.elevation is not None:
-                node_dict["elevation (meters)"] = node_obj.elevation.magnitude
+                node_dict["elevation"] = JSONParser.unit_val_to_dict(node_obj.elevation)
 
             if node_obj.volume is not None:
-                node_dict["volume (cubic meters)"] = node_obj.volume.magnitude
+                node_dict["volume"] = JSONParser.unit_val_to_dict(node_obj.volume)
         elif isinstance(node_obj, node.Pump):
             if node_obj.elevation is not None:
-                node_dict["elevation (meters)"] = node_obj.elevation.magnitude
+                node_dict["elevation"] = JSONParser.unit_val_to_dict(node_obj.elevation)
 
-            if node_obj.horsepower is not None:
-                node_dict["horsepower"] = node_obj.horsepower.magnitude
+            if node_obj.power_rating is not None:
+                node_dict["power_rating"] = JSONParser.unit_val_to_dict(
+                    node_obj.power_rating
+                )
 
             if node_obj.pump_type is not None:
                 node_dict["pump_type"] = node_obj.pump_type.name
 
-            node_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+            node_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                 node_obj, "flow_rate"
             )
             node_dict["num_units"] = node_obj.num_units
         elif isinstance(node_obj, node.Digestion):
             if node_obj.volume is not None:
-                node_dict["volume (cubic meters)"] = node_obj.volume.magnitude
+                node_dict["volume"] = JSONParser.unit_val_to_dict(node_obj.volume)
 
             if node_obj.digester_type is not None:
                 node_dict["digester_type"] = node_obj.digester_type.name
 
-            node_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+            node_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                 node_obj, "flow_rate"
             )
             node_dict["num_units"] = node_obj.num_units
         elif isinstance(node_obj, (node.Cogeneration, node.Boiler)):
-            node_dict["generation_capacity"] = JSONParser.min_max_avg_to_dict(
+            node_dict["generation_capacity"] = JSONParser.min_max_design_to_dict(
                 node_obj, "gen_capacity"
             )
             node_dict["num_units"] = node_obj.num_units
         elif isinstance(
             node_obj,
             (
                 node.Chlorination,
                 node.Thickening,
                 node.Aeration,
                 node.Filtration,
                 node.Clarification,
             ),
         ):
             if node_obj.volume is not None:
-                node_dict["volume (cubic meters)"] = node_obj.volume.magnitude
+                node_dict["volume"] = JSONParser.unit_val_to_dict(node_obj.volume)
 
-            node_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+            node_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                 node_obj, "flow_rate"
             )
             node_dict["num_units"] = node_obj.num_units
         elif isinstance(node_obj, (node.Screening, node.Conditioning, node.Flaring)):
-            node_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+            node_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                 node_obj, "flow_rate"
             )
             node_dict["num_units"] = node_obj.num_units
         elif isinstance(node_obj, node.Battery):
-            node_dict["capacity (kWh)"] = node_obj.capacity.magnitude
-            node_dict["discharge_rate (kW)"] = node_obj.discharge_rate.magnitude
+            node_dict["energy_capacity"] = JSONParser.unit_val_to_dict(
+                node_obj.energy_capacity
+            )
+            node_dict["discharge_rate"] = JSONParser.unit_val_to_dict(
+                node_obj.discharge_rate
+            )
+            node_dict["charge_rate"] = JSONParser.unit_val_to_dict(node_obj.charge_rate)
+            node_dict["leakage"] = JSONParser.unit_val_to_dict(node_obj.leakage)
+            node_dict["rte"] = node_obj.rte
         elif isinstance(node_obj, node.Network):
             node_dict["type"] = type(node_obj).__name__
             node_dict["input_contents"] = [
                 contents.name for contents in node_obj.input_contents
             ]
             node_dict["output_contents"] = [
                 contents.name for contents in node_obj.output_contents
@@ -1317,17 +1510,19 @@
             node_dict["connections"] = []
             for subnode in node_obj.get_all_nodes(recurse=False):
                 node_dict["nodes"].append(subnode.id)
             for conn in node_obj.get_all_connections(recurse=False):
                 node_dict["connections"].append(conn.id)
             if isinstance(node_obj, node.Facility):
                 if node_obj.elevation is not None:
-                    node_dict["elevation (meters)"] = node_obj.elevation.magnitude
+                    node_dict["elevation"] = JSONParser.unit_val_to_dict(
+                        node_obj.elevation
+                    )
 
-                node_dict["flowrate"] = JSONParser.min_max_avg_to_dict(
+                node_dict["flowrate"] = JSONParser.min_max_design_to_dict(
                     node_obj, "flow_rate"
                 )
         else:
             raise TypeError("Unsupported type:", type(node_obj))
 
         return node_dict
```

### Comparing `pype-schema-0.5.0/pype_schema/tag.py` & `pype-schema-0.5.1/pype_schema/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,21 +29,26 @@
     Turbidity = auto()
     Rotation = auto()
     Efficiency = auto()
     StateOfCharge = auto()
     InFlow = auto()  # flow into a node
     OutFlow = auto()  # flow out of a node
     NetFlow = auto()  # net flow through a node
+    Speed = auto()
+    Frequency = auto()
+    Concentration = auto()
 
 
 CONTENTLESS_TYPES = [
     TagType.RunTime,
     TagType.RunStatus,
     TagType.Rotation,
     TagType.Efficiency,
+    TagType.Speed,
+    TagType.Frequency,
 ]
 
 
 class Tag:
     """Class to represent a SCADA or other data tag
 
     Parameters
```

### Comparing `pype-schema-0.5.0/pype_schema/units.py` & `pype-schema-0.5.1/pype_schema/units.py`

 * *Files identical despite different names*

### Comparing `pype-schema-0.5.0/pype_schema/utils.py` & `pype-schema-0.5.1/pype_schema/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     ----------
     value : float
 
     units : str
 
     Returns
     -------
-    Quantity
+    pint.Quantity
         a Pint Quantity with the given value and units
     """
     if value is not None:
         if units:
             return value * parse_units(units)
         else:
             return value
@@ -428,14 +428,22 @@
                 clean_units == "meters" or clean_units == "m" or clean_units == "meter"
             ):
                 return u.m
             elif (
                 clean_units == "inches" or clean_units == "in" or clean_units == "inch"
             ):
                 return u.inch
+            elif (
+                clean_units == "hz"
+                or clean_units == "hertz"
+                or clean_units == "1/s"
+                or clean_units == "1/second"
+                or clean_units == "1/sec"
+            ):
+                return u.Hz
             else:
                 raise UndefinedUnitError("Unsupported unit: " + units)
 
 
 class ContentsType(Enum):
     """Class to represent any possible contents,
     whether they are sludge, water, or gas"""
@@ -465,14 +473,21 @@
     Seawater = auto()
     SurfaceWater = auto()
     Groundwater = auto()
     Stormwater = auto()
     Heat = auto()
     Oil = auto()
     Grease = auto()
+    Chemical = auto()
+    Coagulant = auto()
+    Disinfectant = auto()
+    Deodorant = auto()
+    IndustrialWastewater = auto()
+    MunicipalWastewater = auto()
+    DisinfectedEffluent = auto()
 
 
 class PumpType(Enum):
     """Enum to represent constant vs. variable drive pumps"""
 
     Constant = auto()
     VFD = auto()
```

### Comparing `pype-schema-0.5.0/pype_schema/visualize.py` & `pype-schema-0.5.1/pype_schema/visualize.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,15 +129,15 @@
                 },
             )
             for legend_node in range(num_legend_nodes)
         ]
         g.add_nodes_from(legend_nodes)
 
         nt.from_nx(g)
-        nt.show(network.id + ".html", notebook=False)
+        nt.save_graph(network.id + ".html")
     else:
         # create legend
         custom_lines = []
         for color in colors:
             custom_lines.append(Line2D([0], [0], color=color, lw=4))
         fig, ax = plt.subplots()
         ax.legend(custom_lines, labels)
```

### Comparing `pype-schema-0.5.0/pype_schema.egg-info/PKG-INFO` & `pype-schema-0.5.1/pype_schema.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pype-schema
-Version: 0.5.0
+Version: 0.5.1
 Summary: Class hierarchy to represent configurations of process engineering systems.
 Home-page: https://github.com/we3lab/pype-schema
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: pype-schema
 Platform: UNKNOWN
@@ -70,11 +70,15 @@
 5. ``black pype_schema``
 
   This will reformat the code according to strict style guidelines.
 
 Legal Documents
 ===============
 
+This work was funded by the `Center for Integrated Facility Engineering <https://cife.stanford.edu/>`_ at Stanford University as a
+a part of CIFE Seed Proposal 2023-02
+`Formal proofs of safe operating limits at wastewater resource recovery facilities <https://cife.stanford.edu/formal-proofs-safe-operating-limits-wastewater-resource-recovery-facilities>`_.
+
 - `LICENSE <https://github.com/we3lab/pype-schema/blob/main/LICENSE/>`_
 - `CONTRIBUTING <https://github.com/we3lab/pype-schema/blob/main/CONTRIBUTING.rst/>`_
```

### Comparing `pype-schema-0.5.0/pype_schema.egg-info/SOURCES.txt` & `pype-schema-0.5.1/pype_schema.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -3,25 +3,31 @@
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 docs/CONTRIBUTING.rst
 docs/LICENSE.rst
 docs/Makefile
+docs/advanced.rst
 docs/conf.py
 docs/connection.rst
+docs/hello.rst
 docs/index.rst
+docs/json_rep.rst
 docs/make.bat
 docs/node.rst
 docs/operations.rst
 docs/parse_json.rst
 docs/tag.rst
 docs/units.rst
 docs/utils.rst
 docs/visualize.rst
+docs/_static/ng-imports.png
+docs/_static/utility-graph.png
+docs/_static/wwtp-graph.png
 pype_schema/__init__.py
 pype_schema/connection.py
 pype_schema/node.py
 pype_schema/operations.py
 pype_schema/parse_json.py
 pype_schema/tag.py
 pype_schema/units.py
@@ -31,8 +37,9 @@
 pype_schema.egg-info/SOURCES.txt
 pype_schema.egg-info/dependency_links.txt
 pype_schema.egg-info/not-zip-safe
 pype_schema.egg-info/requires.txt
 pype_schema.egg-info/top_level.txt
 pype_schema/data/__init__.py
 pype_schema/data/sample.json
+pype_schema/data/sample_data.csv
 pype_schema/data/unit_definitions.txt
```

### Comparing `pype-schema-0.5.0/pype_schema.egg-info/requires.txt` & `pype-schema-0.5.1/pype_schema.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,24 +18,26 @@
 flake8>=4.0.0
 codecov>=2.1.4
 pytest>=6.2.5
 pytest-cov>=3.0.0
 pytest-html>=3.1.1
 tox>=3.24.5
 Sphinx==7.0.1
+sphinx-rtd-theme==2.0.0
 
 [dev]
 black>=22.3.0
 flake8>=4.0.0
 codecov>=2.1.4
 pytest>=6.2.5
 pytest-cov>=3.0.0
 pytest-html>=3.1.1
 tox>=3.24.5
 Sphinx==7.0.1
+sphinx-rtd-theme==2.0.0
 
 [setup]
 
 [test]
 black>=22.3.0
 flake8>=4.0.0
 codecov>=2.1.4
```

### Comparing `pype-schema-0.5.0/setup.py` & `pype-schema-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 ]
 
 dev_requirements = [
     *setup_requirements,
     *test_requirements,
     "tox>=3.24.5",
     "Sphinx==7.0.1",
+    "sphinx-rtd-theme==2.0.0"
 ]
 
 requirements = [
     "pint>=0.19.2",
     "networkx>=2.8.5",
     "pyvis>=0.3.0",
     "matplotlib>=3.5.2",
@@ -64,10 +65,10 @@
     python_requires=">=3.9",
     install_requires=requirements,
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     extras_require=extra_requirements,
     test_suite="tests",
     url="https://github.com/we3lab/pype-schema",
-    version="0.5.0",
+    version="0.5.1",
     zip_safe=False,
 )
```

