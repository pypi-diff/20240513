# Comparing `tmp/relari-0.1.4.tar.gz` & `tmp/relari-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relari-0.1.4.tar", max compression
+gzip compressed data, was "relari-0.1.5.tar", max compression
```

## Comparing `relari-0.1.4.tar` & `relari-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.4/README.md
--rw-r--r--   0        0        0      464 2024-04-06 00:54:47.959958 relari-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       45 2024-02-29 01:11:53.776218 relari-0.1.4/relari/__init__.py
--rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.4/relari/eval/__init__.py
--rw-r--r--   0        0        0     5563 2024-04-05 23:41:22.980593 relari-0.1.4/relari/eval/dataset.py
--rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.4/relari/eval/manager.py
--rw-r--r--   0        0        0     1669 2024-02-29 01:11:53.777735 relari-0.1.4/relari/eval/modules.py
--rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.4/relari/eval/pipeline.py
--rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.4/relari/eval/result_types.py
--rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.4/relari/eval/types.py
--rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.4/relari/eval/utils.py
--rw-r--r--   0        0        0     3920 2024-04-05 01:17:20.592928 relari-0.1.4/relari/relari_client.py
--rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2100 2024-02-29 01:27:03.863704 relari-0.1.5/README.md
+-rw-r--r--   0        0        0      464 2024-05-13 02:31:28.788172 relari-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       87 2024-05-12 03:52:38.259679 relari-0.1.5/relari/__init__.py
+-rw-r--r--   0        0        0      234 2024-05-12 04:09:15.157060 relari-0.1.5/relari/datatypes.py
+-rw-r--r--   0        0        0      199 2024-02-29 01:11:53.776623 relari-0.1.5/relari/eval/__init__.py
+-rw-r--r--   0        0        0     5563 2024-04-05 23:41:22.980593 relari-0.1.5/relari/eval/dataset.py
+-rw-r--r--   0        0        0     4790 2024-02-29 07:20:41.559538 relari-0.1.5/relari/eval/manager.py
+-rw-r--r--   0        0        0     1670 2024-05-11 23:31:38.795184 relari-0.1.5/relari/eval/modules.py
+-rw-r--r--   0        0        0     3413 2024-02-29 01:11:53.778019 relari-0.1.5/relari/eval/pipeline.py
+-rw-r--r--   0        0        0     1771 2024-02-29 01:11:53.778261 relari-0.1.5/relari/eval/result_types.py
+-rw-r--r--   0        0        0      123 2024-02-29 01:11:53.778488 relari-0.1.5/relari/eval/types.py
+-rw-r--r--   0        0        0     1106 2024-02-29 01:11:53.779119 relari-0.1.5/relari/eval/utils.py
+-rw-r--r--   0        0        0     5154 2024-05-12 04:49:31.332471 relari-0.1.5/relari/relari_client.py
+-rw-r--r--   0        0        0     2665 1970-01-01 00:00:00.000000 relari-0.1.5/PKG-INFO
```

### Comparing `relari-0.1.4/README.md` & `relari-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/eval/dataset.py` & `relari-0.1.5/relari/eval/dataset.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/eval/manager.py` & `relari-0.1.5/relari/eval/manager.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/eval/modules.py` & `relari-0.1.5/relari/eval/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     if isinstance(obj, DatasetField):
         return {"__class__":obj.__class__.__name__, "name": obj.name}
     elif isinstance(obj, Module):
         return  {"__class__":obj.__class__.__name__, "name": obj.name}
     elif isinstance(obj, type):
         return type_hint_to_str(obj)
     elif isinstance(obj, (list, tuple)):
-        return [serialize_input_type(x) for x in obj]
+        return [_serialize_input_type(x) for x in obj]
     else:
         raise TypeError(f"Object of type {type(obj).__name__} is not serializable")
 
 @dataclass(frozen=True, eq=True)
 class Module:
     name: str
     input: Union[Iterable[InputType], InputType, None]
```

### Comparing `relari-0.1.4/relari/eval/pipeline.py` & `relari-0.1.5/relari/eval/pipeline.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/eval/result_types.py` & `relari-0.1.5/relari/eval/result_types.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/eval/utils.py` & `relari-0.1.5/relari/eval/utils.py`

 * *Files identical despite different names*

### Comparing `relari-0.1.4/relari/relari_client.py` & `relari-0.1.5/relari/relari_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import os
-from typing import Optional, Dict
 import urllib
+from typing import Dict, List, Optional, Union, Any
+
 import requests
 from dotenv import load_dotenv
 
+from relari.datatypes import LabeledDatum
 from relari.eval.manager import eval_manager
 
 load_dotenv()
 
 
 class RelariClient:
     def __init__(self, api_key: Optional[str] = None, url="https://api.relari.ai/v1/"):
@@ -22,28 +24,27 @@
                 "Please set the environment variable RELARI_API_KEY or pass it as an argument."
             )
 
         self._headers = {"X-API-Key": self.api_key, "Content-Type": "application/json"}
         self.timeout = 10
         self.valid = self._validate()
 
-
     def status(self):
         try:
             response = requests.get(
                 urllib.parse.urljoin(self._api_url, "status"),
                 headers=self._headers,
                 timeout=self.timeout,
             )
         except requests.exceptions.Timeout:
             exit("Request timed out while trying to validate API key")
         if response.status_code != 200:
             return False
         return True
-        
+
     def _validate(self):
         try:
             response = requests.get(
                 urllib.parse.urljoin(self._api_url, "auth/"),
                 headers=self._headers,
                 timeout=self.timeout,
             )
@@ -98,12 +99,45 @@
         try:
             response = requests.post(
                 endpoint,
                 headers=self._headers,
                 data=json.dumps(payload),
                 timeout=self.timeout,
             )
+        except requests.exceptions.Timeout:
+            raise Exception("Request timed out while trying to run metric")
+        if response.status_code != 200:
+            raise Exception("Failed to run metric: " + response.text)
+        return response.json()
+
+    def run_metric_batch(
+        self,
+        metric_name: str,
+        args: List[Union[LabeledDatum, Dict[str, Any]]],
+        **kwargs
+    ):
+        # Mode 1: LabeledDatum
+        if "dataset" in kwargs and isinstance(args[0], LabeledDatum):
+            endpoint = urllib.parse.urljoin(self._api_url, "metrics/batch/dataset/")
+            payload = {
+                "metric": metric_name,
+                "dataset": kwargs["dataset"],
+                "kwargs": [x.asdict() for x in args],
+            }
+        else:
+            endpoint = urllib.parse.urljoin(self._api_url, "metrics/batch/")
+            payload = {
+                "metric": metric_name,
+                "kwargs": args,
+            }
+        try:
+            response = requests.post(
+                endpoint,
+                headers=self._headers,
+                data=json.dumps(payload),
+                timeout=self.timeout,
+            )
         except requests.exceptions.Timeout:
             raise Exception("Request timed out while trying to run metric")
         if response.status_code != 200:
             raise Exception("Failed to run metric: " + response.text)
         return response.json()
```

### Comparing `relari-0.1.4/PKG-INFO` & `relari-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relari
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Pasquale Antonante
 Author-email: pasquale@relari.ai
 Requires-Python: >=3.9.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

