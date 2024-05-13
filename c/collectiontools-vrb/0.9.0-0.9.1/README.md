# Comparing `tmp/collectiontools_vrb-0.9.0.tar.gz` & `tmp/collectiontools_vrb-0.9.1.tar.gz`

## Comparing `collectiontools_vrb-0.9.0.tar` & `collectiontools_vrb-0.9.1.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/local_files/.gitignore
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/local_files/collection_translator_inverter_sample.json
--rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/src/collectiontools_vrb/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/src/collectiontools_vrb/__version__.py
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/src/collectiontools_vrb/collectiontranslator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/src/collectiontools_vrb/py.typed
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/LICENSE
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/README.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     9439 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/src/collectiontools_vrb/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/src/collectiontools_vrb/__version__.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/src/collectiontools_vrb/collectiontranslator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/src/collectiontools_vrb/py.typed
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/LICENSE
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 collectiontools_vrb-0.9.1/PKG-INFO
```

### Comparing `collectiontools_vrb-0.9.0/src/collectiontools_vrb/__init__.py` & `collectiontools_vrb-0.9.1/src/collectiontools_vrb/__init__.py`

 * *Files identical despite different names*

### Comparing `collectiontools_vrb-0.9.0/src/collectiontools_vrb/collectiontranslator.py` & `collectiontools_vrb-0.9.1/src/collectiontools_vrb/collectiontranslator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Any as Any
 
+# [ ] Check implementation of translate_str()
+
 class CollectionTranslator:
     """ Search strings, lists or dicts for placeholders using 
     a regular expression provided by the user. Replace the 
     matches with a value provided by a translator function, 
     which is as well provided by the user.
     For dicts and lists, the search is recursive.
     See constructor / functions for details.
```

### Comparing `collectiontools_vrb-0.9.0/LICENSE` & `collectiontools_vrb-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `collectiontools_vrb-0.9.0/README.md` & `collectiontools_vrb-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `collectiontools_vrb-0.9.0/pyproject.toml` & `collectiontools_vrb-0.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/v-r-b/collectiontools_vrb"
+Issues = "https://github.com/v-r-b/collectiontools_vrb/issues"
 
 [tool.hatch.version]
 path = "./src/collectiontools_vrb/__version__.py"
 
 [tool.hatch.build]
 exclude = [
   "/.*",
```

### Comparing `collectiontools_vrb-0.9.0/PKG-INFO` & `collectiontools_vrb-0.9.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.3
 Name: collectiontools_vrb
-Version: 0.9.0
+Version: 0.9.1
 Summary: Various tools to handle collection I/O and transformations
 Project-URL: Homepage, https://github.com/v-r-b/collectiontools_vrb
+Project-URL: Issues, https://github.com/v-r-b/collectiontools_vrb/issues
 Author-email: volker <volker@vrbdev.eu>
 Maintainer-email: volker <volker@vrbdev.eu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

