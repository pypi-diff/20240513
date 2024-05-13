# Comparing `tmp/leafdb-1.0.2.tar.gz` & `tmp/leafdb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leafdb-1.0.2.tar", last modified: Thu May  9 10:36:18 2024, max compression
+gzip compressed data, was "leafdb-1.0.3.tar", last modified: Mon May 13 10:56:21 2024, max compression
```

## Comparing `leafdb-1.0.2.tar` & `leafdb-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-09 10:36:18.236874 leafdb-1.0.2/
--rw-r--r--   0 yhq        (501) staff       (20)      308 2024-05-09 10:36:18.236683 leafdb-1.0.2/PKG-INFO
-drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-09 10:36:18.236439 leafdb-1.0.2/leafdb.egg-info/
--rw-r--r--   0 yhq        (501) staff       (20)      308 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/PKG-INFO
--rw-r--r--   0 yhq        (501) staff       (20)      167 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/SOURCES.txt
--rw-r--r--   0 yhq        (501) staff       (20)        1 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/dependency_links.txt
--rw-r--r--   0 yhq        (501) staff       (20)       11 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/requires.txt
--rw-r--r--   0 yhq        (501) staff       (20)        7 2024-05-09 10:36:18.000000 leafdb-1.0.2/leafdb.egg-info/top_level.txt
--rw-r--r--   0 yhq        (501) staff       (20)    29790 2024-05-09 10:32:35.000000 leafdb-1.0.2/leafdb.py
--rw-r--r--   0 yhq        (501) staff       (20)       38 2024-05-09 10:36:18.236919 leafdb-1.0.2/setup.cfg
--rwx------   0 yhq        (501) staff       (20)      501 2024-05-09 10:35:19.000000 leafdb-1.0.2/setup.py
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-13 10:56:21.046800 leafdb-1.0.3/
+-rw-r--r--   0 yhq        (501) staff       (20)      312 2024-05-13 10:56:21.046622 leafdb-1.0.3/PKG-INFO
+drwxr-xr-x   0 yhq        (501) staff       (20)        0 2024-05-13 10:56:21.046437 leafdb-1.0.3/leafdb.egg-info/
+-rw-r--r--   0 yhq        (501) staff       (20)      312 2024-05-13 10:56:21.000000 leafdb-1.0.3/leafdb.egg-info/PKG-INFO
+-rw-r--r--   0 yhq        (501) staff       (20)      167 2024-05-13 10:56:21.000000 leafdb-1.0.3/leafdb.egg-info/SOURCES.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        1 2024-05-13 10:56:21.000000 leafdb-1.0.3/leafdb.egg-info/dependency_links.txt
+-rw-r--r--   0 yhq        (501) staff       (20)       15 2024-05-13 10:56:21.000000 leafdb-1.0.3/leafdb.egg-info/requires.txt
+-rw-r--r--   0 yhq        (501) staff       (20)        7 2024-05-13 10:56:21.000000 leafdb-1.0.3/leafdb.egg-info/top_level.txt
+-rw-r--r--   0 yhq        (501) staff       (20)    29695 2024-05-13 10:55:11.000000 leafdb-1.0.3/leafdb.py
+-rw-r--r--   0 yhq        (501) staff       (20)       38 2024-05-13 10:56:21.046839 leafdb-1.0.3/setup.cfg
+-rwx------   0 yhq        (501) staff       (20)      505 2024-05-13 10:55:34.000000 leafdb-1.0.3/setup.py
```

### Comparing `leafdb-1.0.2/leafdb.py` & `leafdb-1.0.3/leafdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
-__version__ = '1.0.2'
+__version__ = '1.0.3'
 
 __all__ = ["DbDialect", "database", "SQLConn", "SQLRow", "SQLRowCollection", "SQLParser", "Connection", "BaseDbs",
            "MultipleBaseDbs"]
 
 import os
 import re
 from collections import OrderedDict
@@ -318,22 +318,23 @@
         self.close()
 
     def __repr__(self):
         return '<Connection open={}>'.format(self.open)
 
     def query(self, query, fetchall=False, **params):
         # Execute the given query.
-        # cursor = self._conn.execute(text(query), **params)
         cursor = self._conn.execute(
             text(query).bindparams(**params)
-        )  # TODO: PARAMS GO HERE
+        )
+
+        if cursor.returns_rows:
+            row_gen = (SQLRow(cursor.keys(), row) for row in cursor)
+        else:
+            row_gen = iter(SQLRow([], []))
 
-        if not cursor.keys():  # Skip insert,update has none return values error
-        	return None
-        row_gen = (SQLRow(cursor.keys(), row) for row in cursor)
         results = SQLRowCollection(row_gen)
         if fetchall:
             results.list()
         return results
 
     def bulk_query(self, query, *multiparams):
         self._conn.execute(text(query), *multiparams)
@@ -389,20 +390,20 @@
             return query, kwargs
 
         return True, self.query(query, **kwargs)
 
     def multiple_insert(self, table, values, **kwargs):
         """同时插入多条数据"""
         if not isinstance(values, list):
-            return ValueError("values must be a list for dict.")
+            raise ValueError("values must be a list for dict.")
 
         if len(values) <= 0:
             if len(kwargs) > 0:
                 return self.insert(table, **kwargs)
-            return ValueError("values must be not empty.")
+            raise ValueError("values must be not empty.")
 
         _test = kwargs.pop("_test", False)
         query = SQLParser.insert(table, **values[0])
         if _test:
             return query, values
 
         return True, self.bulk_query(query, values)
```

