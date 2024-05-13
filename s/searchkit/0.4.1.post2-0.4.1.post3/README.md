# Comparing `tmp/searchkit-0.4.1.post2.tar.gz` & `tmp/searchkit-0.4.1.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.4.1.post2.tar", last modified: Thu Apr 25 16:34:39 2024, max compression
+gzip compressed data, was "searchkit-0.4.1.post3.tar", last modified: Sun May 12 15:51:17 2024, max compression
```

## Comparing `searchkit-0.4.1.post2.tar` & `searchkit-0.4.1.post3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.4.1.post2/LICENSE
--rw-r--r--   0 user1     (1000) user1     (1000)     4503 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     4205 2023-05-24 13:53:26.000000 searchkit-0.4.1.post2/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-31 12:54:07.000000 searchkit-0.4.1.post2/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-31 12:54:07.000000 searchkit-0.4.1.post2/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    36146 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      491 2024-04-25 16:30:45.000000 searchkit-0.4.1.post2/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    51527 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4053 2023-12-15 13:29:03.000000 searchkit-0.4.1.post2/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/searchkit.egg-info/
--rw-r--r--   0 user1     (1000) user1     (1000)     4503 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      468 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       21 2024-04-25 16:34:39.000000 searchkit-0.4.1.post2/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       76 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.4.1.post2/setup.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/tests/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1.post2/tests/__init__.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2024-04-25 16:34:39.153411 searchkit-0.4.1.post2/tests/unit/
--rw-rw-r--   0 user1     (1000) user1     (1000)        0 2023-01-10 10:25:51.000000 searchkit-0.4.1.post2/tests/unit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    38115 2024-04-22 09:54:35.000000 searchkit-0.4.1.post2/tests/unit/test_search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    32883 2023-12-15 13:30:40.000000 searchkit-0.4.1.post2/tests/unit/test_search_constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      871 2023-09-20 12:14:30.000000 searchkit-0.4.1.post2/tests/unit/test_utils.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     1319 2023-09-13 12:24:12.000000 searchkit-0.4.1.post2/tests/unit/utils.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    11357 2023-01-26 18:19:39.000000 searchkit-0.4.1.post3/LICENSE
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4205 2023-05-24 17:19:57.000000 searchkit-0.4.1.post3/README.md
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      734 2023-05-13 07:02:21.000000 searchkit-0.4.1.post3/pyproject.toml
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/searchkit/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      121 2023-05-13 07:02:21.000000 searchkit-0.4.1.post3/searchkit/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    36146 2024-04-21 15:19:37.000000 searchkit-0.4.1.post3/searchkit/constraints.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      491 2024-05-09 19:54:10.000000 searchkit-0.4.1.post3/searchkit/log.py
+-rwxrwxr-x   0 gizmo     (1000) gizmo     (1000)    56385 2024-05-12 15:37:51.000000 searchkit-0.4.1.post3/searchkit/search.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     4053 2023-12-15 20:01:02.000000 searchkit-0.4.1.post3/searchkit/utils.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/searchkit.egg-info/
+-rw-r--r--   0 gizmo     (1000) gizmo     (1000)     4503 2024-05-12 15:51:17.000000 searchkit-0.4.1.post3/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      468 2024-05-12 15:51:17.000000 searchkit-0.4.1.post3/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        1 2024-05-12 15:51:17.000000 searchkit-0.4.1.post3/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       57 2024-05-12 15:51:17.000000 searchkit-0.4.1.post3/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       21 2024-05-12 15:51:17.000000 searchkit-0.4.1.post3/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       76 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/setup.cfg
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)       54 2023-01-29 21:19:04.000000 searchkit-0.4.1.post3/setup.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/tests/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post3/tests/__init__.py
+drwxrwxr-x   0 gizmo     (1000) gizmo     (1000)        0 2024-05-12 15:51:17.685225 searchkit-0.4.1.post3/tests/unit/
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)        0 2023-01-26 18:19:39.000000 searchkit-0.4.1.post3/tests/unit/__init__.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    38383 2024-05-11 09:10:51.000000 searchkit-0.4.1.post3/tests/unit/test_search.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)    32883 2023-12-15 20:01:02.000000 searchkit-0.4.1.post3/tests/unit/test_search_constraints.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)      871 2023-09-24 18:41:22.000000 searchkit-0.4.1.post3/tests/unit/test_utils.py
+-rw-rw-r--   0 gizmo     (1000) gizmo     (1000)     1319 2023-09-16 14:38:19.000000 searchkit-0.4.1.post3/tests/unit/utils.py
```

### Comparing `searchkit-0.4.1.post2/LICENSE` & `searchkit-0.4.1.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/PKG-INFO` & `searchkit-0.4.1.post3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1.post2
+Version: 0.4.1.post3
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1.post2/README.md` & `searchkit-0.4.1.post3/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/pyproject.toml` & `searchkit-0.4.1.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/searchkit/constraints.py` & `searchkit-0.4.1.post3/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/searchkit/search.py` & `searchkit-0.4.1.post3/searchkit/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import concurrent.futures
+import copy
 import glob
 import gzip
 import multiprocessing
 import os
 import queue
 import re
 import signal
@@ -16,14 +17,15 @@
 
 from searchkit.log import log
 from searchkit.constraints import CouldNotApplyConstraint
 
 RESULTS_QUEUE_TIMEOUT = 60
 MAX_QUEUE_RETRIES = 10
 RS_LOCK = multiprocessing.Lock()
+NUM_BUFFERED_RESULTS = 100
 
 
 def rs_locked(f):
     def _rs_locked_inner(*args, **kwargs):
         with RS_LOCK:
             return f(*args, **kwargs)
 
@@ -110,14 +112,17 @@
         for pattern in self.patterns:
             ret = pattern.match(line)
             if ret:
                 break
 
         return ret
 
+    def __repr__(self):
+        return ', '.join([str(p) for p in self.patterns])
+
 
 class SequenceSearchDef(SearchDefBase):
 
     def __init__(self, start, tag, end=None, body=None, **kwargs):
         """
         Sequence search definition.
 
@@ -225,93 +230,125 @@
             self.data[sid] = [result]
 
     def remove(self, sid):
         if sid in self.data:
             del self.data[sid]
 
 
-class ResultStoreBase(UserDict):
+class ResultStoreBase(UserList):
+    """
+    This class is used to de-duplicate values stored in search results such
+    that allowing their reference to be saved in the result for later lookup.
+    """
 
     def __init__(self):
-        self.head = 0
-        self.index = {}
-        self.meta = {}
-        self.data = {}
+        self.counters = {}
+        self.value_store = self.data = []
+        self.tag_store = []
+        self.sequence_id_store = []
 
     def __getitem__(self, result_id):
-        return self.data.get(result_id)
+        if result_id >= len(self.value_store):
+            return None
 
-    def increment_head(self):
-        """ Incrementing differs for proxied vs. raw types so we leave this to
-        implementations to figure out. """
-        self.head += 1
+        return self.value_store[result_id]
 
     @property
-    def num_deduped(self):
-        counters = self.meta.values()
+    def parts_deduped(self):
+        counters = self.counters.values()
         return sum(counters) - len(counters)
 
-    def add(self, value):
-        _id = self.index.get(value)
-        if _id is not None:
-            self.meta[_id] += 1
-            return _id
-
-        _id = self.head
-        self.data[_id] = value
-        self.meta[_id] = 1
-        self.index[value] = _id
-        self.increment_head()
-        return _id
+    @property
+    def parts_non_deduped(self):
+        return len(self.value_store)
+
+    def _get_value_index(self, value, store):
+        """
+        If the value is not None and not already saved, save it.
+
+        Returns the position of the value in the store or -1 if it is None.
+        """
+        if value is None:
+            return -1
+
+        if value in store:
+            return store.index(value)
+
+        store.append(value)
+        return len(store) - 1
+
+    def add(self, tag, sequence_id, value):
+        """
+        Ensure the given values are saved in the store and return their
+        position.
+
+        Returns a tuple of references to the position in the store of each
+        value. A ref value of -1 indicates that the value does not exist and is
+        not stored.
+
+        @param tag: optional search tag
+        @param sequence_id: optional sequence search id
+        @param value: search result value
+        """
+        value_idx = self._get_value_index(value, self.value_store)
+        if value_idx >= 0:
+            # increment global counter
+            if value_idx not in self.counters:
+                self.counters[value_idx] = 1
+            else:
+                self.counters[value_idx] += 1
+
+        tag_idx = self._get_value_index(tag, self.tag_store)
+        sequence_id_idx = self._get_value_index(sequence_id,
+                                                self.sequence_id_store)
+        return tag_idx, sequence_id_idx, value_idx
 
 
 class ResultStoreSimple(ResultStoreBase):
     """ Store for use when sharing between processes is not needed. """
 
 
 class ResultStoreParallel(ResultStoreBase):
     """ Store for use when sharing between processes is required. """
 
     def __init__(self, mgr):
-        self._head = mgr.Value('i', 0)
-        self.meta = mgr.dict()
-        self.index = mgr.dict()
-        self.data = mgr.dict()
+        self.counters = mgr.dict()
+        self.value_store = self.data = mgr.list()
+        self.tag_store = mgr.list()
+        self.sequence_id_store = mgr.list()
 
     @rs_locked
     def __getitem__(self, result_id):
         return super().__getitem__(result_id)
 
-    @property
-    def head(self):
-        return self._head.value
-
-    def increment_head(self):
-        self._head.value = self.head + 1
+    @rs_locked
+    def add(self, *args, **kwargs):
+        return super().add(*args, **kwargs)
 
+    @property
     @rs_locked
-    def add(self, value):
-        return super().add(value)
+    def parts_deduped(self):
+        return super().parts_deduped
 
     @property
     @rs_locked
-    def num_deduped(self):
-        return super().num_deduped
+    def parts_non_deduped(self):
+        return super().parts_non_deduped
 
     @rs_locked
     def unproxy_results(self):
         """
         Converts internal stores to unproxied types so they can be accessed
         once their manager is gone.
         """
-        log.debug("unproxying results store (data=%s)", len(self.data))
-        self._head = self._head.value
-        self.data = self.data.copy()
-        self.meta = self.meta.copy()
-        self.index = self.index.copy()
+        log.debug("unproxying results store (data=%s)", len(self.value_store))
+        self.value_store = self.data = copy.deepcopy(self.data)
+        self.tag_store = copy.deepcopy(self.tag_store)
+        self.sequence_id_store = copy.deepcopy(self.sequence_id_store)
+        self.counters = self.counters.copy()
 
 
 class ResultFieldInfo(UserDict):
 
     def __init__(self, fields):
         """
         @param fields: list or dictionary of field names. If a dictionary is
@@ -341,73 +378,116 @@
                 return _field
 
         raise FileSearchException("field with index {} not found in mapping".
                                   format(index))
 
 
 class SearchResultBase(UserList):
+    META_OFFSET_TAG = 0
+    META_OFFSET_SEQ_ID = 1
 
-    def get(self, field):
-        """
-        Retrieve result part value by index or name.
+    PART_OFFSET_IDX = 0
+    PART_OFFSET_VALUE = 1
+    PART_OFFSET_FIELD = 2
 
-        @param field: integer index of string field name.
-        """
+    @abc.abstractmethod
+    def __init__(self):
+        self.results_store = None
+        self.linenumber = None
+        self.section_id = None
+
+    def _get_store_id(self, field):
         for part in self.data:
             store_id = None
-            if isinstance(field, str):
-                if part['name'] == field:
-                    store_id = part['store_id']
-            elif part['idx'] == field:
-                store_id = part['store_id']
+            # Entry has format: (<idx>, <tag_id>, <store id>, <field name>)
+            if len(part) > self.PART_OFFSET_FIELD and isinstance(field, str):
+                if part[self.PART_OFFSET_FIELD] != field:
+                    continue
+            elif part[self.PART_OFFSET_IDX] != field:
+                continue
 
+            store_id = part[self.PART_OFFSET_VALUE]
             if store_id is not None:
-                return self.results_store.get(store_id)
+                return store_id
 
-    def __getattr__(self, name):
-        if name != 'field_info':
-            if self.field_info and name in self.field_info:
-                return self.get(name)
+    def get(self, field):
+        """
+        Retrieve result part value by index or name.
 
-        raise AttributeError("'{}' object has no attribute '{}'".
-                             format(self.__class__.__name__, name))
+        @param field: integer index of string field name.
+        """
+        store_id = self._get_store_id(field)
+        if store_id is not None:
+            return self.results_store[store_id]
 
     def __iter__(self):
         """ Only return part values when iterating over this object. """
         for part in self.data:
-            yield self.results_store.get(part['store_id'])
+            yield self.results_store[part[self.PART_OFFSET_VALUE]]
 
     def __repr__(self):
-        r_list = ["{}='{}'".format(rp['idx'],
-                                   self.results_store.get(rp['store_id']))
+        r_list = ["{}='{}'".
+                  format(rp[self.PART_OFFSET_IDX],
+                         self.results_store[rp[self.PART_OFFSET_VALUE]])
                   for rp in self.data]
         return ("ln:{} {} (section={})".
-                format(self.linenumber, ", ".join(r_list),
-                       self.section_id))
+                format(self.linenumber, ", ".join(r_list), self.section_id))
 
 
 class SearchResultMinimal(SearchResultBase):
 
-    def __init__(self, result_id, data, linenumber, source_id, tag,
-                 sequence_id, sequence_section_id, field_info):
+    def __init__(self, data, metadata, linenumber, source_id,
+                 sequence_section_id, field_info):
         """
         This is a minimised representation of a SearchResult object so as to
         reduce its size as much as possible before putting on the results
         queue.
+
+        IMPORTANT: this class must contain as few attributes as possible and
+        their values must be as small as possible. For large values that need
+        to be shared, we de-duplicate using ResultStoreBase implementations.
+
+        Do not store references to shared objects.
         """
-        self.id = result_id
-        self.data = data
+        self.data = data[:]
+        self.metadata = metadata[:]
         self.linenumber = linenumber
         self.source_id = source_id
-        self.tag = tag
-        self.sequence_id = sequence_id
         self.section_id = sequence_section_id
-        self.field_info = field_info
+        if field_info:
+            self.field_names = list(field_info)
+        else:
+            self.field_names = None
+
         self.results_store = None
 
+    def __getattr__(self, name):
+        if name != 'field_names':
+            if self.field_names and name in self.field_names:
+                return self.get(name)
+
+        raise AttributeError("'{}' object has no attribute '{}'".
+                             format(self.__class__.__name__, name))
+
+    @property
+    def tag(self):
+        idx = self.metadata[self.META_OFFSET_TAG]
+        if idx < 0:
+            return
+
+        return self.results_store.tag_store[idx]
+
+    @property
+    def sequence_id(self):
+        idx = self.metadata[self.META_OFFSET_SEQ_ID]
+        if idx < 0:
+            return
+
+        return self.results_store.sequence_id_store[idx]
+
     def register_results_store(self, store):
         """
         Register a ResultsStore with this result. This is used to re-register
         the store once the result has been received by the main process.
 
         @param store: ResultsStore object
         """
@@ -441,15 +521,15 @@
                                           "but no section id provided")
 
             self.sequence_id = search_def.sequence_def.id
 
         self.field_info = search_def.field_info
 
         if not search_def.store_result_contents:
-            log.debug("store_contents is False - skipping save")
+            log.debug("store_contents is False - skipping save value")
             return
 
         self.store_result(result)
 
     def store_result(self, result):
         num_groups = len(result.groups())
         # NOTE: this does not include group(0)
@@ -460,86 +540,84 @@
                 self._save_part(i, result.group(i))
         else:
             log.debug("Saving full search result is inefficient and can lead "
                       "to high memory usage. Use sub groups if possible. "
                       "(tag=%s)", self.tag)
             self._save_part(0, result.group(0))
 
-    @cached_property
-    def id(self):
-        """ Unique Result ID """
-        id_string = "{}-{}-{}".format(uuid.uuid4(), self.source_id,
-                                      self.linenumber)
-        if self.sequence_id:
-            id_string = "{}-{}-{}".format(id_string,
-                                          self.sequence_id,
-                                          self.section_id)
-        return id_string
+    @property
+    def metadata(self):
+        tag_id, seq_id, _ = self.results_store.add(self.tag, self.sequence_id,
+                                                   value=None)
+        return (tag_id, seq_id)
 
-    def _save_part(self, part_index, value):
+    def _save_part(self, part_index, value=None):
         name = None
-        if value is not None and self.field_info:
-            name = self.field_info.index_to_name(part_index - 1)
-            value = self.field_info.ensure_type(name, value)
-
-        store_id = self.results_store.add(value)
-        self.data.append({'idx': part_index, 'store_id': store_id,
-                          'name': name})
+        if value is not None:
+            if self.field_info:
+                name = self.field_info.index_to_name(part_index - 1)
+                value = self.field_info.ensure_type(name, value)
+
+        _, _, store_id = self.results_store.add(self.tag, self.sequence_id,
+                                                value)
+        if name is None:
+            entry = (part_index, store_id)
+        else:
+            entry = (part_index, store_id, name)
+
+        self.data.append(entry)
 
     @cached_property
     def export(self):
         """ Export the smallest possible representation of this object. """
-        return SearchResultMinimal(self.id, self.data, self.linenumber,
-                                   self.source_id, self.tag,
-                                   self.sequence_id, self.section_id,
-                                   self.field_info)
+        return SearchResultMinimal(self.data, self.metadata,
+                                   self.linenumber, self.source_id,
+                                   self.section_id, self.field_info)
 
 
 class SearchResultsCollection(UserDict):
 
     def __init__(self, search_catalog, results_store):
         self.search_catalog = search_catalog
         self.results_store = results_store
         self.reset()
 
     @property
     def data(self):
         results = {}
-        for path, ids in self._results_by_path.items():
-            results[path] = [self._results_by_id[id] for id in ids]
+        for path, _results in self._results_by_path.items():
+            results[path] = _results
 
         return results
 
     @property
     def all(self):
-        for r in self._results_by_id.values():
-            yield r
+        for results in self._results_by_path.values():
+            for r in results:
+                yield r
 
     def reset(self):
         self._results_by_path = {}
-        self._results_by_id = {}
 
     @property
     def files(self):
         return list(self._results_by_path.keys())
 
     def add(self, result):
         result.register_results_store(self.results_store)
         # resolve
         path = self.search_catalog.source_id_to_path(result.source_id)
-        self._results_by_id[result.id] = result
         if path not in self._results_by_path:
-            self._results_by_path[path] = [result.id]
+            self._results_by_path[path] = [result]
         else:
-            self._results_by_path[path].append(result.id)
+            self._results_by_path[path].append(result)
 
     def find_by_path(self, path):
         """ Return results for a given path. """
-        results = self._results_by_path.get(path, [])
-        return [self._results_by_id[id] for id in results]
+        return self._results_by_path.get(path, [])
 
     def find_by_tag(self, tag, path=None):
         """ Return results matched by tag.
 
         @param tag: tag used to identify search results.
         @param path: optional path used to filter results to only include those
                      matched from a given path.
@@ -571,15 +649,15 @@
 
         sequences = []
         for _path in paths:
             for result in self.find_by_path(_path):
                 if result.sequence_id is None:
                     continue
 
-                sequences.append(result.id)
+                sequences.append(result)
 
         return sequences
 
     def find_sequence_by_tag(self, tag, path=None):
         """ Find results for the sequence search(es) identified from tag.
 
         Returns a dictionary of "sections" i.e. complete sequences matched
@@ -602,16 +680,15 @@
         using the associated SequenceSearchDef object. Each section is a list
         of SearchResult objects representing start/body/end for that section.
 
         @param sequence_obj: SequenceSearch object
         @param path: optionally filter results for a given path.
         """
         _results = {}
-        for r in self._get_all_sequence_results(path=path):
-            result = self._results_by_id[r]
+        for result in self._get_all_sequence_results(path=path):
             s_id = result.sequence_id
             if s_id != sequence_obj.id:
                 continue
 
             section_id = result.section_id
             if section_id not in _results:
                 _results[section_id] = []
@@ -764,47 +841,80 @@
         try:
             return self._source_ids[s_id]
         except KeyError:
             log.exception("ALL PATHS:")
             log.error('\n'.join(list(self._source_ids.keys())))
 
     def _get_source_id(self, path):
-        for source_id, _path in self._source_ids.items():
-            if _path == path:
-                return source_id
-
-        source_id = str(uuid.uuid4())
-        while source_id in self._source_ids:
-            log.error("source id %s already exists - trying again", source_id)
-            source_id = str(uuid.uuid4())
+        if not self._source_ids:
+            source_id = 0
+        else:
+            for source_id, _path in self._source_ids.items():
+                if _path == path:
+                    return source_id
+
+            source_id = max(list(self._source_ids)) + 1
 
         log.debug("path=%s source_id=%s", path, source_id)
         self._source_ids[source_id] = path
         return source_id
 
     def __len__(self):
         return len(self._entries)
 
     def __iter__(self):
         for entry in self._entries.values():
             yield entry
 
+    def __repr__(self):
+        info = ""
+        for path, searches in self._entries.items():
+            info += "\n{}:\n    ".format(path)
+            entries = []
+            for key, val in searches.items():
+                entries.append("{}={}".format(key, val))
+
+            info += '\n    '.join(entries)
+
+        return info
+
 
 class SearchTask(object):
 
-    def __init__(self, info, constraints_manager, results_queue,
-                 results_store, decode_errors=None):
+    def __init__(self, info, constraints_manager, results_store,
+                 results_queue=None, results_collection=None,
+                 decode_errors=None):
+        """
+        Run search task on file.
+
+        @param info: dictionary containing information about what we are
+                     searching incl. path, searchdefs etc.
+        @param constraints_manager: SearchConstraintsManager object
+        @param results_store: ResultStoreSimple or ResultStoreParallel object
+        @param results_queue: optional multiprocessing.Queue. This must be
+                              provided if task is running in a child process.
+        @param results_collection: optional SearchResultsCollection. This must
+                                  be provided if task is not running in
+                                  parallel mode.
+        @param decode_errors: unicode decode error handling.
+        """
+        if results_queue is not None and results_collection is not None:
+            raise Exception("only one of results_queue and results_collection "
+                            "can be used with a SearchTask.")
+
         self.info = info
         self.stats = SearchTaskStats()
         self.constraints_manager = constraints_manager
         self.results_queue = results_queue
+        self.results_collection = results_collection
         self.results_store = results_store
         self.decode_kwargs = {}
         if decode_errors:
             self.decode_kwargs['errors'] = decode_errors
+        self.buffered_results = []
 
     @cached_property
     def id(self):
         return str(uuid.uuid4())
 
     @cached_property
     def search_defs_conditional(self):
@@ -818,21 +928,25 @@
             if s_def in self.search_defs_conditional:
                 alldefs[s_def] = False
 
         return alldefs
 
     def put_result(self, result):
         self.stats['results'] += 1
+        if self.results_collection is not None:
+            self.results_collection.add(result)
+            return
+
         max_tries = MAX_QUEUE_RETRIES
         while max_tries > 0:
             try:
                 if max_tries == MAX_QUEUE_RETRIES:
-                    self.results_queue.put_nowait(result.export)
+                    self.results_queue.put_nowait(result)
                 else:
-                    self.results_queue.put(result.export,
+                    self.results_queue.put(result,
                                            timeout=RESULTS_QUEUE_TIMEOUT)
 
                 break
             except queue.Full:
                 if max_tries == MAX_QUEUE_RETRIES:
                     msg = ("search task queue for '%s' is full - switching "
                            "to using blocking put with timeout")
@@ -845,27 +959,37 @@
 
                 max_tries -= 1
 
         if max_tries == 0:
             log.error("exceeded max number of retries (%s) to put results "
                       "data on the queue", MAX_QUEUE_RETRIES)
 
+    def _flush_results_buffer(self):
+        # log.debug("flushing results buffer (%s)", len(self.buffered_results))
+        for result in self.buffered_results:
+            self.put_result(result)
+
+        self.buffered_results = []
+
     def _simple_search(self, search_def, line, ln):
         """ Perform a simple search on line.
 
         @param search_def: SearchDef object
         @param line: current line (string)
         @param ln: current line number
         """
         ret = search_def.run(line)
         if not ret:
             return
 
-        self.put_result(SearchResult(ln, self.info['source_id'], ret,
-                                     search_def, self.results_store))
+        result = SearchResult(ln, self.info['source_id'], ret, search_def,
+                              self.results_store)
+        self.buffered_results.append(result.export)
+        if len(self.buffered_results) >= NUM_BUFFERED_RESULTS:
+            self._flush_results_buffer()
 
     def _sequence_search(self, seq_def, line, ln, sequence_results):
         """ Perform a sequence search on line.
 
         @param seq_def: SequenceSearchDef object
         @param line: current line (string)
         @param ln: current line number
@@ -964,15 +1088,17 @@
                         continue
 
                     seq_id = r.sequence_id
                     if seq_id in filter_section_id:
                         if r.section_id in filter_section_id[seq_id]:
                             continue
 
-                self.put_result(r)
+                self.buffered_results.append(r.export)
+                if len(self.buffered_results) >= NUM_BUFFERED_RESULTS:
+                    self._flush_results_buffer()
 
     def _run_search(self, fd):
         """
         @param fd: open file descriptor
         """
         self.stats.reset()
         sequence_results = SequenceSearchResults()
@@ -1003,14 +1129,17 @@
 
                 if isinstance(s_def, SequenceSearchDef):
                     self._sequence_search(s_def, line, ln, sequence_results)
                 else:
                     self._simple_search(s_def, line, ln)
 
         self._process_sequence_results(sequence_results, ln)
+        # allow garbage collect
+        sequence_results = {}
+
         log.debug("completed search of %s lines", self.stats['lines_searched'])
         if self.search_defs_conditional:
             msg = "constraints stats {}:".format(fd.name)
             for sd in self.search_defs_conditional:
                 if sd.constraints:
                     for c in sd.constraints.values():
                         msg += "\n  id={}: {}".format(c.id, c.stats())
@@ -1039,17 +1168,19 @@
             # first assume compressed then plain
             with gzip.open(path, 'rb') as fd:
                 try:
                     # test if file is gzip
                     fd.read(1)
                     fd.seek(0)
                     stats = self._run_search(fd)
+                    self._flush_results_buffer()
                 except OSError:
                     with open(path, 'rb') as fd:
                         stats = self._run_search(fd)
+                        self._flush_results_buffer()
         except UnicodeDecodeError:
             log.exception("caught UnicodeDecodeError while searching %s", path)
             raise
         except EOFError as e:
             log.exception("")
             msg = ("an exception occurred while searching {} - {}".
                    format(path, e))
@@ -1072,15 +1203,16 @@
     def reset(self):
         self.data = {'searches': 0,
                      'searches_by_job': [],
                      'lines_searched': 0,
                      'jobs_completed': 0,
                      'total_jobs': 0,
                      'results': 0,
-                     'num_deduped': 0}
+                     'parts_deduped': 0,
+                     'parts_non_deduped': 0}
 
     def update(self, stats):  # pylint: disable=W0221
         if not stats:
             return
 
         for key, val in stats.items():
             self.data[key] += val
@@ -1339,31 +1471,30 @@
 
             try:
                 log.debug('sending SIGKILL to worker process %s', wpid)
                 os.kill(wpid, signal.SIGILL)
             except Exception:
                 log.debug('worker process %s already killed', wpid)
 
-    def _run_single(self, results, results_store):
+    def _run_single(self, results_collection, results_store):
         """ Run a single search using this process.
 
-        @param results: SearchResultsCollection object
+        @param results_collection: SearchResultsCollection object
+        @param results_store: ResultsStoreSimple object
         """
-        results_queue = multiprocessing.Queue()
         for info in self.catalog:
             task = SearchTask(info,
                               constraints_manager=self.constraints_manager,
-                              results_queue=results_queue,
+                              results_collection=results_collection,
                               results_store=results_store,
                               decode_errors=self.decode_errors)
             self.stats.update(task.execute())
 
         self.stats['jobs_completed'] = 1
         self.stats['total_jobs'] = 1
-        self._purge_results(results, results_queue, self.stats['results'])
 
     def _run_mp(self, mgr, results, results_store):
         """ Run searches in parallel.
 
         @param mgr: multiprocessing.Manager object
         @param results: SearchResultsCollection object
         """
@@ -1434,24 +1565,27 @@
             log.debug("catalog is empty - nothing to run")
             return SearchResultsCollection(self.catalog, ResultStoreSimple())
 
         self.stats['searches'] = sum([len(p['searches'])  # noqa, pylint: disable=R1728
                                       for p in self.catalog])
         self.stats['searches_by_job'] = [len(p['searches'])
                                          for p in self.catalog]
+        log.debug(repr(self.catalog))
         if len(self.files) > 1:
             log.debug("running searches (parallel=True)")
             with multiprocessing.Manager() as mgr:
                 rs = ResultStoreParallel(mgr)
                 results = SearchResultsCollection(self.catalog, rs)
                 self._run_mp(mgr, results, rs)
-                self.stats['num_deduped'] = rs.num_deduped
+                self.stats['parts_deduped'] = rs.parts_deduped
+                self.stats['parts_non_deduped'] = rs.parts_non_deduped
                 rs.unproxy_results()
         else:
             log.debug("running searches (parallel=False)")
             rs = ResultStoreSimple()
             results = SearchResultsCollection(self.catalog, rs)
             self._run_single(results, rs)
-            self.stats['num_deduped'] = rs.num_deduped
+            self.stats['parts_deduped'] = rs.parts_deduped
+            self.stats['parts_non_deduped'] = rs.parts_non_deduped
 
         log.debug("filesearcher: completed (%s)", self.stats)
         return results
```

### Comparing `searchkit-0.4.1.post2/searchkit/utils.py` & `searchkit-0.4.1.post3/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/searchkit.egg-info/PKG-INFO` & `searchkit-0.4.1.post3/searchkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.4.1.post2
+Version: 0.4.1.post3
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: importlib-metadata; python_version >= "3.8"
 Requires-Dist: fasteners
```

### Comparing `searchkit-0.4.1.post2/tests/unit/test_search.py` & `searchkit-0.4.1.post3/tests/unit/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,16 @@
 
     def test_simple_search_many_files(self):
         f = FileSearcher()
         with tempfile.TemporaryDirectory() as dtmp:
             for i in range(1000):
                 with open(os.path.join(dtmp, str(i)), 'w') as fd:
                     fd.write("a key: foo bar\n")
+                    for i in range(1000):
+                        fd.write("some extra text\n")
                     fd.write("a key: bar foo\n")
 
             f.add(SearchDef(r'.+:\s+(\S+) \S+', tag='simple'), dtmp + '/*')
             results = f.run()
 
         self.assertEqual(len(results), 2000)
         self.assertEqual(len(results.find_by_tag('simple')), 2000)
@@ -335,15 +337,16 @@
                     # sequence search
                     f.add(seq, fpath)
 
                 results = f.run()
             finally:
                 shutil.rmtree(dtmp)
 
-            self.assertEqual(f.stats['num_deduped'], 40037)
+            self.assertEqual(f.stats['parts_deduped'], 40037)
+            self.assertEqual(f.stats['parts_non_deduped'], 3)
 
         self.assertEqual(len(results), 40040)
         self.assertEqual(len(results.find_by_tag('simple')), 20000)
         self.assertEqual(len(results.find_sequence_by_tag('myseq')), 20)
         for section in results.find_sequence_by_tag('myseq').values():
             for r in section:
                 if r.tag == seq.start_tag:
@@ -903,22 +906,25 @@
         results = s.run()
         results = results.find_by_tag('mysd')
         self.assertEqual([r.get(2) for r in results], ['L3', 'L4'])
 
     def test_search_result_index(self):
         sri = ResultStoreSimple()
         for val in ['foo', 'bar', 'foo']:
-            sri.add(val)
+            sri.add('atag', None, val)
 
-        self.assertEqual(sri, {0: 'foo', 1: 'bar'})
-        self.assertEqual(sri.meta, {0: 2, 1: 1})
+        self.assertEqual(sri, ['foo', 'bar'])
+        self.assertEqual(sri.counters, {0: 2, 1: 1})
+        self.assertEqual(sri.tag_store, ['atag'])
         self.assertEqual(sri[0], 'foo')
-        self.assertEqual(sri.get(1), 'bar')
-        self.assertEqual(sri.get(2), None)
-        self.assertEqual(sri.num_deduped, 1)
+
+        self.assertEqual(sri[1], 'bar')
+        self.assertEqual(sri[2], None)
+        self.assertEqual(sri.parts_deduped, 1)
+        self.assertEqual(sri.parts_non_deduped, 2)
 
     def test_search_unicode_decode_w_error(self):
         f = FileSearcher()
         with tempfile.TemporaryDirectory() as dtmp:
             fpath = os.path.join(dtmp, 'f1')
             with open(fpath, 'wb') as fd:
                 fd.write(b'\xe2')
```

### Comparing `searchkit-0.4.1.post2/tests/unit/test_search_constraints.py` & `searchkit-0.4.1.post3/tests/unit/test_search_constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/tests/unit/test_utils.py` & `searchkit-0.4.1.post3/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.4.1.post2/tests/unit/utils.py` & `searchkit-0.4.1.post3/tests/unit/utils.py`

 * *Files identical despite different names*

