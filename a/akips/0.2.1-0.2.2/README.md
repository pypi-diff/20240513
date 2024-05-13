# Comparing `tmp/akips-0.2.1.tar.gz` & `tmp/akips-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akips-0.2.1.tar", max compression
+gzip compressed data, was "akips-0.2.2.tar", max compression
```

## Comparing `akips-0.2.1.tar` & `akips-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.2.1/LICENSE
--rw-r--r--   0        0        0     1458 2023-09-25 15:32:31.817902 akips-0.2.1/README.md
--rw-r--r--   0        0        0    11909 2024-04-11 13:35:55.005243 akips-0.2.1/akips/__init__.py
--rw-r--r--   0        0        0      254 2023-09-22 19:01:52.560879 akips-0.2.1/akips/exceptions.py
--rw-r--r--   0        0        0      515 2024-04-12 13:28:36.079283 akips-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 akips-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-09-21 01:11:03.608768 akips-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1458 2023-09-25 15:32:31.817902 akips-0.2.2/README.md
+-rw-r--r--   0        0        0    13027 2024-05-02 18:18:47.198493 akips-0.2.2/akips/__init__.py
+-rw-r--r--   0        0        0      254 2023-09-22 19:01:52.560879 akips-0.2.2/akips/exceptions.py
+-rw-r--r--   0        0        0      515 2024-05-13 16:08:05.304440 akips-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 akips-0.2.2/PKG-INFO
```

### Comparing `akips-0.2.1/LICENSE` & `akips-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `akips-0.2.1/README.md` & `akips-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `akips-0.2.1/akips/__init__.py` & `akips-0.2.2/akips/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ''' Base module '''
-__version__ = '0.1.5'
+__version__ = '0.2.2'
 
 import io
 import re
 import logging
 from datetime import datetime
 import requests
 import pytz
@@ -226,20 +226,20 @@
                         'details': match.group(7),
                     }
                     data.append(entry)
             logger.debug("Found {} events of type {} in akips".format(len(data), type))
             return data
         return None
 
-    ### Time-series commands
+    # Time-series commands
 
     def get_series(self, period='last1h', device='*', attribute='*', group_filter='any', groups=[], get_dict=True):
         ''' Pull a series of values.  Command syntax:
-            cseries avg 
-            time {time filter] type parent child attribute
+            cseries avg
+            time {time filter} type parent child attribute
             [any|all|not group {group name} ...] '''
         params = {
             'cmds': f'cseries avg time {period} * {device} * {attribute}'
         }
         if groups:
             group_list = " ".join(groups)
             params['cmds'] += f" {group_filter} group {group_list}"
@@ -254,22 +254,44 @@
                 # parse each row as a list, will have a column header row
                 reader = csv.reader(buff)
             csv_to_list = [row for row in reader]
             logger.debug("Found {} series entries".format(len(csv_to_list)))
             return csv_to_list
         return None
 
-    ### Base operations
+    def get_aggregate(self, operator='avg', interval='300', period='last1h', device='*', attribute='*', group_filter='any', groups=[]):
+        ''' Aggregate stats in intervals over a period of time. Command syntax:
+            aggregate interval {avg|total seconds}
+            time {time filter} type parent child attribute
+            [any|all|not group {group name} ...] '''
+        params = {
+            'cmds': f'aggregate interval {operator} {interval} time {period} * {device} * {attribute}'
+        }
+        if groups:
+            group_list = " ".join(groups)
+            params['cmds'] += f" {group_filter} group {group_list}"
+        text = self._get(params=params)
+        if text:
+            # Text should be one CSV line followed by one blank line
+            lines = text.split('\n')
+            values = lines[0].split(',')
+            logger.debug("Found {} aggregate values".format(len(values)))
+            return values
+        return None
+
+    # Base operations
 
     def _get(self, section='/api-db/', params=None, timeout=30):
         ''' Call HTTP GET against the AKiPS server '''
         server_url = 'https://' + self.server + section
         params['username'] = self.username
         params['password'] = self.password
 
+        if 'cmds' in params:
+            logger.debug("akips command: {}".format(params['cmds']))
         try:
             r = self.session.get(server_url, params=params, verify=self.verify, timeout=timeout)
             r.raise_for_status()
         except requests.exceptions.HTTPError as errh:
             logger.error(errh)
             raise
         except requests.exceptions.ConnectionError as errc:
@@ -283,8 +305,9 @@
             raise
 
         # AKiPS can return a raw error message if something fails
         if re.match(r'^ERROR:', r.text):
             logger.error("Web API request failed: {}".format(r.text))
             raise AkipsError(message=r.text)
         else:
+            logger.debug("akips output: {}".format(r.text))
             return r.text
```

### Comparing `akips-0.2.1/pyproject.toml` & `akips-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "akips"
-version = "0.2.1"
+version = "0.2.2"
 description = "Module to interact with the AKiPS Network Monitoring Software API interface"
 authors = ["William E Whitaker <will.whitaker@unc.edu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/wwhitaker/akips"
 
 [tool.poetry.dependencies]
```

### Comparing `akips-0.2.1/PKG-INFO` & `akips-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: akips
-Version: 0.2.1
+Version: 0.2.2
 Summary: Module to interact with the AKiPS Network Monitoring Software API interface
 Home-page: https://github.com/wwhitaker/akips
 License: MIT
 Author: William E Whitaker
 Author-email: will.whitaker@unc.edu
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

