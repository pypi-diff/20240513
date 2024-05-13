# Comparing `tmp/midas-store-1.0.0rc6.tar.gz` & `tmp/midas-store-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-store-1.0.0rc6.tar", last modified: Thu May  5 14:00:21 2022, max compression
+gzip compressed data, was "midas-store-1.0.1.tar", last modified: Mon May 13 12:37:07 2024, max compression
```

## Comparing `midas-store-1.0.0rc6.tar` & `midas-store-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 stephan   (1000) wheel      (998)        0 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/
--rwxr-xr-x   0 stephan   (1000) wheel      (998)     7648 2022-04-28 07:17:47.000000 midas-store-1.0.0rc6/LICENSE
--rw-r--r--   0 stephan   (1000) wheel      (998)     2920 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/PKG-INFO
--rwxr-xr-x   0 stephan   (1000) wheel      (998)     1976 2022-04-28 07:17:47.000000 midas-store-1.0.0rc6/README.md
-drwxr-xr-x   0 stephan   (1000) wheel      (998)        0 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/midas/
-drwxr-xr-x   0 stephan   (1000) wheel      (998)        0 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/midas/modules/
-drwxr-xr-x   0 stephan   (1000) wheel      (998)        0 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/midas/modules/store/
--rwxr-xr-x   0 stephan   (1000) wheel      (998)       50 2022-05-05 13:47:32.000000 midas-store-1.0.0rc6/midas/modules/store/__init__.py
--rwxr-xr-x   0 stephan   (1000) wheel      (998)      257 2022-05-05 13:53:59.000000 midas-store-1.0.0rc6/midas/modules/store/meta.py
--rwxr-xr-x   0 stephan   (1000) wheel      (998)     2269 2022-05-05 13:52:39.000000 midas-store-1.0.0rc6/midas/modules/store/module.py
--rwxr-xr-x   0 stephan   (1000) wheel      (998)     8255 2022-05-05 13:53:47.000000 midas-store-1.0.0rc6/midas/modules/store/simulator.py
-drwxr-xr-x   0 stephan   (1000) wheel      (998)        0 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/midas_store.egg-info/
--rw-r--r--   0 stephan   (1000) wheel      (998)     2920 2022-05-05 14:00:20.000000 midas-store-1.0.0rc6/midas_store.egg-info/PKG-INFO
--rw-r--r--   0 stephan   (1000) wheel      (998)      323 2022-05-05 14:00:21.000000 midas-store-1.0.0rc6/midas_store.egg-info/SOURCES.txt
--rw-r--r--   0 stephan   (1000) wheel      (998)        1 2022-05-05 14:00:20.000000 midas-store-1.0.0rc6/midas_store.egg-info/dependency_links.txt
--rw-r--r--   0 stephan   (1000) wheel      (998)      120 2022-05-05 14:00:21.000000 midas-store-1.0.0rc6/midas_store.egg-info/requires.txt
--rw-r--r--   0 stephan   (1000) wheel      (998)        6 2022-05-05 14:00:21.000000 midas-store-1.0.0rc6/midas_store.egg-info/top_level.txt
--rw-r--r--   0 stephan   (1000) wheel      (998)       38 2022-05-05 14:00:21.239686 midas-store-1.0.0rc6/setup.cfg
--rwxr-xr-x   0 stephan   (1000) wheel      (998)     1608 2022-05-05 13:59:48.000000 midas-store-1.0.0rc6/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.173159 midas-store-1.0.1/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     7648 2024-05-03 13:32:33.000000 midas-store-1.0.1/LICENSE
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2898 2024-05-13 12:37:07.173159 midas-store-1.0.1/PKG-INFO
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1976 2024-05-03 13:32:33.000000 midas-store-1.0.1/README.md
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.169826 midas-store-1.0.1/midas/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.169826 midas-store-1.0.1/midas/modules/
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.169826 midas-store-1.0.1/midas/modules/store/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)       50 2024-05-03 13:32:33.000000 midas-store-1.0.1/midas/modules/store/__init__.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)      257 2024-05-03 13:32:33.000000 midas-store-1.0.1/midas/modules/store/meta.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     2269 2024-05-03 13:32:33.000000 midas-store-1.0.1/midas/modules/store/module.py
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     8532 2024-05-13 12:36:28.000000 midas-store-1.0.1/midas/modules/store/simulator.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.173159 midas-store-1.0.1/midas_store.egg-info/
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)     2898 2024-05-13 12:37:07.000000 midas-store-1.0.1/midas_store.egg-info/PKG-INFO
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      348 2024-05-13 12:37:07.000000 midas-store-1.0.1/midas_store.egg-info/SOURCES.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        1 2024-05-13 12:37:07.000000 midas-store-1.0.1/midas_store.egg-info/dependency_links.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)      120 2024-05-13 12:37:07.000000 midas-store-1.0.1/midas_store.egg-info/requires.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)        6 2024-05-13 12:37:07.000000 midas-store-1.0.1/midas_store.egg-info/top_level.txt
+-rw-r--r--   0 sbalduin  (1000) wheel      (998)       38 2024-05-13 12:37:07.173159 midas-store-1.0.1/setup.cfg
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     1608 2024-05-03 13:32:33.000000 midas-store-1.0.1/setup.py
+drwxr-xr-x   0 sbalduin  (1000) wheel      (998)        0 2024-05-13 12:37:07.173159 midas-store-1.0.1/tests/
+-rwxr-xr-x   0 sbalduin  (1000) wheel      (998)     6246 2024-05-03 13:32:33.000000 midas-store-1.0.1/tests/test_midas_hdf5.py
```

### Comparing `midas-store-1.0.0rc6/LICENSE` & `midas-store-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-store-1.0.0rc6/PKG-INFO` & `midas-store-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: midas-store
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: A database simulator that stores every input.
 Home-page: https://gitlab.com/midas-mosaik/midas-store
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -84,8 +83,7 @@
 store = store_sim.Database(filename="path/to/my_db.hdf5", buffer_size=0, overwrite=False)
 ```
 
 Afterwards, you can define `world.connect(other_entity, store, attrs)` as you like.
 
 ## License
 This software is released under the GNU Lesser General Public License (LGPL). See the license file for more information about the details.
-
```

### Comparing `midas-store-1.0.0rc6/README.md` & `midas-store-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `midas-store-1.0.0rc6/midas/modules/store/module.py` & `midas-store-1.0.1/midas/modules/store/module.py`

 * *Files identical despite different names*

### Comparing `midas-store-1.0.0rc6/midas/modules/store/simulator.py` & `midas-store-1.0.1/midas/modules/store/simulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import os
 import threading
 
 import mosaik_api
+import numpy as np
 import pandas as pd
 from midas.util.logging import set_and_init_logger
 
 from . import LOG
 from .meta import META
 
 pd.set_option("io.hdf.default_format", "table")
@@ -120,14 +122,18 @@
             for src_id, val in src_ids.items():
                 sid, eid = src_id.split(".")
                 key = f"{eid}___{attr}".replace("-", "__")
                 sid = sid.replace("-", "__")
 
                 current.setdefault(sid, dict())
                 current[sid].setdefault("cols", list()).append(key)
+                if isinstance(val, (list, dict, np.ndarray)):
+                    val = json.dumps(val)
+                elif isinstance(val, pd.DataFrame):
+                    val = val.to_json()
                 current[sid].setdefault("vals", list()).append(val)
 
         if self._worker is not None:
             LOG.debug("Waiting for the store worker to finish...")
             self._worker.join()
             LOG.debug("Clearing current database.")
             self.database = dict()
@@ -173,26 +179,28 @@
             LOG.warning("Database is empty. Unable to write anything to disk.")
             return
 
         errors = list()
         for sid, data in self.database.items():
             try:
                 data.index += self.saved_rows
-                data.to_hdf(self.filename, sid, format="table", append=append)
+                data.to_hdf(
+                    self.filename, key=sid, format="table", append=append
+                )
             except Exception:
                 LOG.info(
                     "Couldn't save data of simulator %s. Trying to load "
                     "existing data and append manually. ",
                     sid,
                 )
                 try:
-                    edata = pd.read_hdf(self.filename, sid)
+                    edata = pd.read_hdf(self.filename, key=sid)
                     edata = pd.concat([edata, data])
                     edata.to_hdf(
-                        self.filename, sid, format="table", append=False
+                        self.filename, key=sid, format="table", append=False
                     )
                     LOG.info(
                         "Successfully appended the data. One reason could be "
                         "that some values have inconsistent types, e.g., are "
                         "int in the one step and float in the other. As long "
                         "as this is not fixed, this message will probably "
                         "re-appear."
```

### Comparing `midas-store-1.0.0rc6/midas_store.egg-info/PKG-INFO` & `midas-store-1.0.1/midas_store.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: midas-store
-Version: 1.0.0rc6
+Version: 1.0.1
 Summary: A database simulator that stores every input.
 Home-page: https://gitlab.com/midas-mosaik/midas-store
 Author: Stephan Balduin
 Author-email: stephan.balduin@offis.de
 License: LGPL
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -84,8 +83,7 @@
 store = store_sim.Database(filename="path/to/my_db.hdf5", buffer_size=0, overwrite=False)
 ```
 
 Afterwards, you can define `world.connect(other_entity, store, attrs)` as you like.
 
 ## License
 This software is released under the GNU Lesser General Public License (LGPL). See the license file for more information about the details.
-
```

### Comparing `midas-store-1.0.0rc6/setup.py` & `midas-store-1.0.1/setup.py`

 * *Files identical despite different names*

