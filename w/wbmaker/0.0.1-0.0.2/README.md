# Comparing `tmp/wbmaker-0.0.1.tar.gz` & `tmp/wbmaker-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbmaker-0.0.1.tar", max compression
+gzip compressed data, was "wbmaker-0.0.2.tar", max compression
```

## Comparing `wbmaker-0.0.1.tar` & `wbmaker-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-05-10 22:05:47.248777 wbmaker-0.0.1/LICENSE
--rw-r--r--   0        0        0      492 2024-05-10 22:11:14.772671 wbmaker-0.0.1/README.md
--rw-r--r--   0        0        0      475 2024-05-10 22:11:13.635477 wbmaker-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-10 22:05:47.250351 wbmaker-0.0.1/wbmaker/__init__.py
--rw-r--r--   0        0        0     4365 2024-05-10 22:05:47.250518 wbmaker-0.0.1/wbmaker/wb.py
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 wbmaker-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-10 22:05:47.248777 wbmaker-0.0.2/LICENSE
+-rw-r--r--   0        0        0      492 2024-05-10 22:11:14.772671 wbmaker-0.0.2/README.md
+-rw-r--r--   0        0        0      475 2024-05-13 18:16:58.427663 wbmaker-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-10 22:05:47.250351 wbmaker-0.0.2/wbmaker/__init__.py
+-rw-r--r--   0        0        0     4663 2024-05-13 18:16:48.198894 wbmaker-0.0.2/wbmaker/wb.py
+-rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 wbmaker-0.0.2/PKG-INFO
```

### Comparing `wbmaker-0.0.1/LICENSE` & `wbmaker-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wbmaker-0.0.1/wbmaker/wb.py` & `wbmaker-0.0.2/wbmaker/wb.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from urllib.parse import urlparse, parse_qs, quote
 from wikibaseintegrator.wbi_config import config as wbi_config
 from wikibaseintegrator import WikibaseIntegrator, wbi_login
 from wikibaseintegrator import models, datatypes
 from wikibaseintegrator.wbi_enums import WikibaseDatatype, ActionIfExists, WikibaseDatePrecision, WikibaseSnakType
 import mwclient
 from datetime import datetime
+from dateutil.parser import parse as parse_date
 
 class WB:
     def __init__(
         self, 
         config_file: str = 'config.ini',
         config_section: str = 'wb',
         cache_props: bool = True):
@@ -111,8 +112,16 @@
         props = self.sparql_query(q_props)
         props['pid'] = props['property'].str.split('/').str[-1]
 
         return props.set_index('propertyLabel')['pid'].to_dict()
 
 
     def wb_dt(self, dt=datetime.now()):
+        '''
+        Converts a string (or datetime object) to a proper Wikibase datetime string
+        '''
+        if not isinstance(dt, datetime):
+            try:
+                dt = parse_date(dt)
+            except:
+                return None
         return dt.strftime("+%Y-%m-%dT%H:%M:%SZ").split('T')[0] + 'T00:00:00Z'
```

### Comparing `wbmaker-0.0.1/PKG-INFO` & `wbmaker-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbmaker
-Version: 0.0.1
+Version: 0.0.2
 Summary: Establishes a connection to a Wikibase instance and provides methods for interacting with it.
 Author: Sky Bristol
 Author-email: skybristol@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

