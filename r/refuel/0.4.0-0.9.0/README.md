# Comparing `tmp/refuel-0.4.0.tar.gz` & `tmp/refuel-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refuel-0.4.0.tar", last modified: Mon Jan 23 03:14:29 2023, max compression
+gzip compressed data, was "refuel-0.9.0.tar", last modified: Thu Mar  2 20:10:31 2023, max compression
```

## Comparing `refuel-0.4.0.tar` & `refuel-0.9.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-01-23 03:14:29.969393 refuel-0.4.0/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1485 2022-06-07 21:55:30.000000 refuel-0.4.0/LICENSE.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       24 2022-12-01 01:34:30.000000 refuel-0.4.0/MANIFEST.in
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6680 2023-01-23 03:14:29.969476 refuel-0.4.0/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4594 2023-01-20 17:38:13.000000 refuel-0.4.0/README.md
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      311 2023-01-03 07:31:52.000000 refuel-0.4.0/pyproject.toml
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-01-23 03:14:29.968182 refuel-0.4.0/refuel/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       89 2023-01-03 07:31:52.000000 refuel-0.4.0/refuel/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)    16680 2023-01-21 16:56:56.000000 refuel-0.4.0/refuel/client.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-01-23 03:14:29.969174 refuel-0.4.0/refuel/tests/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        0 2022-12-01 01:34:30.000000 refuel-0.4.0/refuel/tests/__init__.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      186 2022-12-01 01:34:30.000000 refuel-0.4.0/refuel/tests/conftest.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       84 2022-12-01 01:34:30.000000 refuel-0.4.0/refuel/tests/test_client.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     4615 2023-01-20 17:38:13.000000 refuel-0.4.0/refuel/types.py
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      556 2023-01-03 07:31:52.000000 refuel-0.4.0/refuel/utils.py
-drwxr-xr-x   0 rishabhbhargava   (501) staff       (20)        0 2023-01-23 03:14:29.968722 refuel-0.4.0/refuel.egg-info/
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     6680 2023-01-23 03:14:29.000000 refuel-0.4.0/refuel.egg-info/PKG-INFO
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      379 2023-01-23 03:14:29.000000 refuel-0.4.0/refuel.egg-info/SOURCES.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        1 2023-01-23 03:14:29.000000 refuel-0.4.0/refuel.egg-info/dependency_links.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       51 2023-01-23 03:14:29.000000 refuel-0.4.0/refuel.egg-info/requires.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)        7 2023-01-23 03:14:29.000000 refuel-0.4.0/refuel.egg-info/top_level.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)       51 2022-09-16 08:13:25.000000 refuel-0.4.0/requirements.txt
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)      310 2023-01-23 03:14:29.969721 refuel-0.4.0/setup.cfg
--rw-r--r--   0 rishabhbhargava   (501) staff       (20)     1139 2023-01-23 03:14:26.000000 refuel-0.4.0/setup.py
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-03-02 20:10:31.957573 refuel-0.9.0/
+-rw-r--r--   0 pc         (501) staff       (20)     1485 2022-10-10 21:17:55.000000 refuel-0.9.0/LICENSE.txt
+-rw-r--r--   0 pc         (501) staff       (20)       24 2022-11-30 21:14:57.000000 refuel-0.9.0/MANIFEST.in
+-rw-r--r--   0 pc         (501) staff       (20)     5255 2023-03-02 20:10:31.957632 refuel-0.9.0/PKG-INFO
+-rw-r--r--   0 pc         (501) staff       (20)     4594 2023-01-19 20:25:53.000000 refuel-0.9.0/README.md
+-rw-r--r--   0 pc         (501) staff       (20)      311 2022-12-29 18:43:33.000000 refuel-0.9.0/pyproject.toml
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-03-02 20:10:31.956368 refuel-0.9.0/refuel/
+-rw-r--r--   0 pc         (501) staff       (20)       89 2022-12-29 18:43:33.000000 refuel-0.9.0/refuel/__init__.py
+-rw-r--r--   0 pc         (501) staff       (20)    18026 2023-02-27 20:50:37.000000 refuel-0.9.0/refuel/client.py
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-03-02 20:10:31.957382 refuel-0.9.0/refuel/tests/
+-rw-r--r--   0 pc         (501) staff       (20)        0 2022-11-30 21:14:57.000000 refuel-0.9.0/refuel/tests/__init__.py
+-rw-r--r--   0 pc         (501) staff       (20)      186 2022-11-30 21:14:57.000000 refuel-0.9.0/refuel/tests/conftest.py
+-rw-r--r--   0 pc         (501) staff       (20)       84 2022-11-30 21:14:57.000000 refuel-0.9.0/refuel/tests/test_client.py
+-rw-r--r--   0 pc         (501) staff       (20)     4936 2023-02-10 21:40:23.000000 refuel-0.9.0/refuel/types.py
+-rw-r--r--   0 pc         (501) staff       (20)     1892 2023-02-27 20:50:37.000000 refuel-0.9.0/refuel/utils.py
+drwxr-xr-x   0 pc         (501) staff       (20)        0 2023-03-02 20:10:31.956933 refuel-0.9.0/refuel.egg-info/
+-rw-r--r--   0 pc         (501) staff       (20)     5255 2023-03-02 20:10:31.000000 refuel-0.9.0/refuel.egg-info/PKG-INFO
+-rw-r--r--   0 pc         (501) staff       (20)      379 2023-03-02 20:10:31.000000 refuel-0.9.0/refuel.egg-info/SOURCES.txt
+-rw-r--r--   0 pc         (501) staff       (20)        1 2023-03-02 20:10:31.000000 refuel-0.9.0/refuel.egg-info/dependency_links.txt
+-rw-r--r--   0 pc         (501) staff       (20)       62 2023-03-02 20:10:31.000000 refuel-0.9.0/refuel.egg-info/requires.txt
+-rw-r--r--   0 pc         (501) staff       (20)        7 2023-03-02 20:10:31.000000 refuel-0.9.0/refuel.egg-info/top_level.txt
+-rw-r--r--   0 pc         (501) staff       (20)       62 2023-02-27 20:50:37.000000 refuel-0.9.0/requirements.txt
+-rw-r--r--   0 pc         (501) staff       (20)      310 2023-03-02 20:10:31.957880 refuel-0.9.0/setup.cfg
+-rw-r--r--   0 pc         (501) staff       (20)     1139 2023-03-02 20:10:23.000000 refuel-0.9.0/setup.py
```

### Comparing `refuel-0.4.0/LICENSE.txt` & `refuel-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `refuel-0.4.0/PKG-INFO` & `refuel-0.9.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,199 +1,202 @@
 Metadata-Version: 2.1
 Name: refuel
-Version: 0.4.0
+Version: 0.9.0
 Summary: Library to log your Machine Learning datasets to Refuel Platform
 Home-page: UNKNOWN
 Author: Refuel.ai
 Author-email: support@refuel.ai
 Maintainer: Refuel.ai
 Maintainer-email: support@refuel.ai
 License: BSD 3-clause
-Description: 
-        # Refuel Python API
-        
-        <p align="center"><img height="250" src="https://user-images.githubusercontent.com/1568137/172486199-f4eddb09-7c58-4841-8f3c-60f647079073.png"></p>
-        
-        This is the [Refuel.ai](https://www.refuel.ai/) Python client library. The primary use for this library is to log your machine learning datasets to the Refuel platform. More features coming soon!
-        
-        # Installation
-        You can install this library using `pip`:
-        
-        ```bash
-        pip install refuel
-        ```
-        
-        # Usage
-        
-        Make sure you have a valid API key from Refuel (shared with your team during onboarding). Contact us at support@refuel.ai if you need help. 
-        
-        ## Initialization:
-        
-        Initialize the Refuel client with your API key. This can be done in one of two ways:
-        
-        ```python
-        import refuel
-        
-        # Assuming you've set `REFUEL_API_KEY` in your env,
-        # init() will pick it up automatically
-        refuel_client = refuel.init()
-        ```
-        
-        Alternatively, specify it as an explicit option:
-        ```python
-        import refuel
-        
-        options = {
-            "api_key": "<YOUR_API_KEY>"
-        }
-        
-        refuel_client = refuel.init(**options)
-        ```
-        
-        ## Logging data
-        
-        ### Log a single prediction event (no ground truth)
-        
-        ```python
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id1', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.42, -0.13, ...]},
-            y_pred={'scores': {'cat': 0.92, 'dog': 0.08}, 'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a single prediction event (with ground truth)
-        
-        ```python
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id2', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.35, -0.27, ...]},
-            y_pred={'scores': {'cat': 0.12, 'dog': 0.88}, 'label': 'dog'},
-            y_true={'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a single prediction event (ground truth becomes available at a later point)
-        
-        ```python
-        # This will be joined with the rest of the event logged previously
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id1'},
-            y_true={'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a batch of prediction events
-        
-        ```python
-        # List of events to be logged. 
-        events = [{'x': ..., 'y_pred': ..., 'y_true': ..., 'metadata': ...}]
-        
-        refuel_client.log_batch(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            events=events
-        )
-        ```
-        
-        ### Log a dataset stored in S3 with an s3 uri
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='s3://bucket/path/to/object.type',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        ### Log a dataset stored in GCS with a GCS uri
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='gs://bucket/path/to/object.type',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        
-        ### Log a dataset stored in S3 or GCS with a pre-signed url
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='https://bucket.s3.amazonaws.com/path/to/object.type?AWSAccessKeyId=1234&Signature=1234',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        
-        ## Querying data
-        
-        ### Query events table
-        
-        ```python
-        # Query events directly from a dataset
-        refuel_client.query_events(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            order_by="ordering-column",
-            offset=1234,
-            max_events=1234
-        )
-        ```
-        
-        ### Query annotation queue
-        
-        ```python
-        # Query events from the annotation queue
-        refuel_client.query_annotation_queue(
-            model_name='my-model-name',
-            queue_name='my-queue-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            order_by="ordering-column",
-            offset=1234,
-            max_events=1234
-        )
-        ```
-        
-        ### Query similar events
-        
-        ```python
-        # Query events similar to passed event
-        refuel_client.query_similar_events(
-            model_name='my-model-name',
-            refuel_uuid='refuel-uuid',
-            embedding_column='embedding-column',
-            dataset_name='my-dataset-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            max_events=1234
-        )
-        ```
-        
-        # Questions?
-        
-        Reach out to us at support@refuel.ai with any questions!
-        
-        ![Tests](https://github.com/refuel-ai/refuel-python/actions/workflows/test.yml/badge.svg)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Refuel Python API
+
+<p align="center"><img height="250" src="https://user-images.githubusercontent.com/1568137/172486199-f4eddb09-7c58-4841-8f3c-60f647079073.png"></p>
+
+This is the [Refuel.ai](https://www.refuel.ai/) Python client library. The primary use for this library is to log your machine learning datasets to the Refuel platform. More features coming soon!
+
+# Installation
+You can install this library using `pip`:
+
+```bash
+pip install refuel
+```
+
+# Usage
+
+Make sure you have a valid API key from Refuel (shared with your team during onboarding). Contact us at support@refuel.ai if you need help. 
+
+## Initialization:
+
+Initialize the Refuel client with your API key. This can be done in one of two ways:
+
+```python
+import refuel
+
+# Assuming you've set `REFUEL_API_KEY` in your env,
+# init() will pick it up automatically
+refuel_client = refuel.init()
+```
+
+Alternatively, specify it as an explicit option:
+```python
+import refuel
+
+options = {
+    "api_key": "<YOUR_API_KEY>"
+}
+
+refuel_client = refuel.init(**options)
+```
+
+## Logging data
+
+### Log a single prediction event (no ground truth)
+
+```python
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id1', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.42, -0.13, ...]},
+    y_pred={'scores': {'cat': 0.92, 'dog': 0.08}, 'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a single prediction event (with ground truth)
+
+```python
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id2', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.35, -0.27, ...]},
+    y_pred={'scores': {'cat': 0.12, 'dog': 0.88}, 'label': 'dog'},
+    y_true={'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a single prediction event (ground truth becomes available at a later point)
+
+```python
+# This will be joined with the rest of the event logged previously
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id1'},
+    y_true={'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a batch of prediction events
+
+```python
+# List of events to be logged. 
+events = [{'x': ..., 'y_pred': ..., 'y_true': ..., 'metadata': ...}]
+
+refuel_client.log_batch(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    events=events
+)
+```
+
+### Log a dataset stored in S3 with an s3 uri
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='s3://bucket/path/to/object.type',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+### Log a dataset stored in GCS with a GCS uri
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='gs://bucket/path/to/object.type',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+
+### Log a dataset stored in S3 or GCS with a pre-signed url
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='https://bucket.s3.amazonaws.com/path/to/object.type?AWSAccessKeyId=1234&Signature=1234',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+
+## Querying data
+
+### Query events table
+
+```python
+# Query events directly from a dataset
+refuel_client.query_events(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    order_by="ordering-column",
+    offset=1234,
+    max_events=1234
+)
+```
+
+### Query annotation queue
+
+```python
+# Query events from the annotation queue
+refuel_client.query_annotation_queue(
+    model_name='my-model-name',
+    queue_name='my-queue-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    order_by="ordering-column",
+    offset=1234,
+    max_events=1234
+)
+```
+
+### Query similar events
+
+```python
+# Query events similar to passed event
+refuel_client.query_similar_events(
+    model_name='my-model-name',
+    refuel_uuid='refuel-uuid',
+    embedding_column='embedding-column',
+    dataset_name='my-dataset-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    max_events=1234
+)
+```
+
+# Questions?
+
+Reach out to us at support@refuel.ai with any questions!
+
+![Tests](https://github.com/refuel-ai/refuel-python/actions/workflows/test.yml/badge.svg)
+
```

### Comparing `refuel-0.4.0/README.md` & `refuel-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `refuel-0.4.0/refuel/client.py` & `refuel-0.9.0/refuel/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 from typing import Dict, List
 
 import pandas as pd
 from loguru import logger
 from requests_futures.sessions import FuturesSession
 
 from refuel.types import DatasetEvent, Event, EventBatch
-from refuel.utils import DATE_FOURTEEN_DAYS_AGO, DATE_TOMORROW
+from refuel.utils import DATE_FOURTEEN_DAYS_AGO, DATE_TOMORROW, validate_event_schema
 
 
 class RefuelClient:
     # Default config settings
     API_BASE_URL = "https://api.refuel.ai"
     API_KEY_ENV_VARIABLE = "REFUEL_API_KEY"
     TIMEOUT_SECS = 15
     MAX_RETRIES = 3
     MAX_WORKERS = 4
     DT_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
     MAX_BYTES_PER_BATCH = 3000000  # 3 MB
     MAX_EVENTS_PER_BATCH = 100
     DEFAULT_QUEUE_NAME = "default"
     DEFAULT_DATASET_NAME = "default"
+    DEFAULT_VERSION_NAME = "default"
     DEFAULT_ORDERING = "recent"
     DEFAULT_MAX_QUERY_EVENTS = 1000000
     QUERY_STEP_SIZE = 100
 
     def __init__(
         self,
         api_key: str = None,
@@ -95,25 +96,28 @@
         self,
         model_name: str,
         x: Dict,
         y_pred: Dict = None,
         y_true: Dict = None,
         metadata: Dict = None,
         dataset_name: str = DEFAULT_DATASET_NAME,
+        version: str = DEFAULT_VERSION_NAME,
+        validate_data: bool = False,
     ) -> pyfutures.Future:
         """
         Log individual events to the Refuel platform.
 
         Args:
             model_name (str): _description_
             dataset_name (str): _description_
             x (dict): _description_
             y_pred (dict): _description_. Defaults to None.
             y_true (dict, optional): _description_. Defaults to None.
             metadata (dict, optional): _description_. Defaults to None.
+            version (str, optional): model versioning. Defaults to "default".
 
         Returns:
             pyfutures.Future: _description_
         """
         if not self._api_key:
             logger.error(
                 f"API Key is absent or invalid: {self._api_key}. No event was logged"
@@ -121,27 +125,46 @@
             return None
         if model_name not in self._init_context.get("models", []):
             logger.error(f"Model name: {model_name} does not exist for this team")
             return None
 
         client_timestamp = datetime.utcnow().strftime(self.DT_FORMAT)
         event = Event(
-            model_name, dataset_name, client_timestamp, x, y_pred, y_true, metadata
+            model_name,
+            dataset_name,
+            client_timestamp,
+            x,
+            y_pred,
+            y_true,
+            metadata,
+            version,
         )
+        if validate_data:
+            schema = self._init_context.get("schemas", {}).get(model_name, {})
+            if schema:
+                validate_event_schema(event, schema)
+            else:
+                logger.info(f"No model schema found. Skipping data validation.")
         return self._post(url=self._api_base_url + "/log", body=event.serialize())
 
     def log_batch(
-        self, model_name: str, events: List, dataset_name: str = DEFAULT_DATASET_NAME
+        self,
+        model_name: str,
+        events: List,
+        dataset_name: str = DEFAULT_DATASET_NAME,
+        version: str = "default",
+        validate_data: bool = False,
     ) -> List[pyfutures.Future]:
         """_summary_
 
         Args:
             model_name (str): _description_
             dataset_name (str): _description_
             events (List): _description_
+            version: (str): model version. Defaults to "default"
 
         Returns:
             List[pyfutures.Future]: _description_
         """
         if not self._api_key:
             logger.error(
                 f"API Key is absent or invalid: {self._api_key}. No event was logged"
@@ -151,32 +174,47 @@
             logger.error(f"Model name: {model_name} does not exist for this team")
             return None
 
         client_timestamp = datetime.utcnow().strftime(self.DT_FORMAT)
         chunks = self._chunkify_events(events)
         futures = []
         for chunk in chunks:
-            batch = EventBatch(model_name, dataset_name, client_timestamp, chunk)
+            batch = EventBatch(
+                model_name, dataset_name, client_timestamp, chunk, version
+            )
+            if validate_data:
+                schema = self._init_context.get("schemas", {}).get(model_name, {})
+                if schema:
+                    for e in batch.serialize():
+                        validate_event_schema(e, schema)
+                else:
+                    logger.info(f"No model schema found. Skipping data validation.")
             futures.append(
                 self._post(
                     url=self._api_base_url + "/log_batch", body=batch.serialize()
                 )
             )
         return futures
 
     def log_dataset(
-        self, model_name: str, dataset_name: str, cloud_uri: str, dataset_config: dict
+        self,
+        model_name: str,
+        dataset_name: str,
+        cloud_uri: str,
+        dataset_config: dict,
+        version: str = "default",
     ) -> pyfutures.Future:
         """Log dataset to the Refuel platform.
 
         Args:
             model_name (str): model to log dataset to
             dataset_name (str): name of dataset
             cloud_uri (str): cloud uri or presigned url to dataset
             dataset_config (dict): configuration for the dataset
+            version (str): model version. Defaults to "default"
 
         Returns:
             pyfutures.Future:
         """
         if not self._api_key:
             logger.error(
                 f"API Key is absent or invalid: {self._api_key}. No event was logged"
@@ -185,17 +223,21 @@
         if model_name not in self._init_context.get("models", []):
             logger.error(f"Model name: {model_name} does not exist for this team")
             return None
 
         client_timestamp = datetime.utcnow().strftime(self.DT_FORMAT)
 
         dataset_event = DatasetEvent(
-            model_name, dataset_name, client_timestamp, cloud_uri, dataset_config
+            model_name,
+            dataset_name,
+            client_timestamp,
+            cloud_uri,
+            dataset_config,
+            version,
         )
-
         return self._post(
             url=self._api_base_url + "/log_dataset", body=dataset_event.serialize()
         )
 
     def _event_count_helper(self, url: str, params: Dict = None) -> int:
         model_name = params.get("model_name", None)
         if not self._api_key:
```

### Comparing `refuel-0.4.0/refuel/types.py` & `refuel-0.9.0/refuel/types.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         model_name: str,
         dataset_name: str,
         client_timestamp: str,
         x: Dict,
         y_pred: Dict,
         y_true: Dict,
         metadata: Dict,
+        version: str,
     ) -> None:
         """
         Args:
             model_name (str): _description_
             x (dict): _description_
             y_pred (dict): _description_
             y_true (dict): _description_
@@ -68,31 +69,38 @@
             "model_name": self.model_name,
             "dataset_name": self.dataset_name,
             "x": self.x,
             "y_pred": self.y_pred,
             "y_true": self.y_true,
             "metadata": self.metadata,
             "refuel_client_timestamp": self.client_timestamp,
+            "version": self.version,
         }
         return json.dumps(data, cls=RefuelJSONEncoder)
 
 
 class EventBatch(BaseLoggingObj):
     def __init__(
-        self, model_name: str, dataset_name: str, client_timestamp: str, events: List
+        self,
+        model_name: str,
+        dataset_name: str,
+        client_timestamp: str,
+        events: List,
+        version: str,
     ) -> None:
         """_summary_
 
         Args:
             model_name (str): _description_
             client_timestamp (str): _description_
             events (List): _description_
         """
         super().__init__(model_name, dataset_name, client_timestamp)
         self.events = events
+        self.version = version
 
     def serialize(self) -> List:
         if not self.model_name:
             logger.error(
                 f"No model name specified for logging event: {self.model_name}"
             )
             return []
@@ -104,39 +112,43 @@
                     "model_name": self.model_name,
                     "dataset_name": self.dataset_name,
                     "x": event.get("x"),
                     "y_pred": event.get("y_pred"),
                     "y_true": event.get("y_true"),
                     "metadata": event.get("metadata"),
                     "refuel_client_timestamp": self.client_timestamp,
+                    "version": self.version,
                 }
             )
         return json.dumps(data, cls=RefuelJSONEncoder)
 
 
 class DatasetEvent(BaseLoggingObj):
     def __init__(
         self,
         model_name: str,
         dataset_name: str,
         client_timestamp: str,
         cloud_uri: str,
         dataset_config: dict,
+        version: str,
     ) -> None:
         """_summary_
 
         Args:
             model_name (str): model dataset belongs to
             dataset_name (str): name of the dataset
             client_timestamp (str): provided timestamp
             cloud_uri (str): cloud uri or pre-signed uri to dataset in cloud storage
+            version (str): model version
         """
         super().__init__(model_name, dataset_name, client_timestamp)
         self.cloud_uri = cloud_uri
         self.dataset_config = dataset_config
+        self.version = version
         self.dataset_config.setdefault("type", "CSV")
         self.dataset_config.setdefault("delimiter", ",")
 
     def serialize(self) -> List:
         if not self.model_name:
             logger.error(
                 f"No model name specified for logging event: {self.model_name}"
@@ -145,10 +157,11 @@
 
         data = {
             "model_name": self.model_name,
             "dataset_name": self.dataset_name,
             "cloud_uri": self.cloud_uri,
             "dataset_config": json.dumps(self.dataset_config),
             "refuel_client_timestamp": self.client_timestamp,
+            "version": self.version,
         }
 
         return json.dumps(data)
```

### Comparing `refuel-0.4.0/refuel.egg-info/PKG-INFO` & `refuel-0.9.0/refuel.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,199 +1,202 @@
 Metadata-Version: 2.1
 Name: refuel
-Version: 0.4.0
+Version: 0.9.0
 Summary: Library to log your Machine Learning datasets to Refuel Platform
 Home-page: UNKNOWN
 Author: Refuel.ai
 Author-email: support@refuel.ai
 Maintainer: Refuel.ai
 Maintainer-email: support@refuel.ai
 License: BSD 3-clause
-Description: 
-        # Refuel Python API
-        
-        <p align="center"><img height="250" src="https://user-images.githubusercontent.com/1568137/172486199-f4eddb09-7c58-4841-8f3c-60f647079073.png"></p>
-        
-        This is the [Refuel.ai](https://www.refuel.ai/) Python client library. The primary use for this library is to log your machine learning datasets to the Refuel platform. More features coming soon!
-        
-        # Installation
-        You can install this library using `pip`:
-        
-        ```bash
-        pip install refuel
-        ```
-        
-        # Usage
-        
-        Make sure you have a valid API key from Refuel (shared with your team during onboarding). Contact us at support@refuel.ai if you need help. 
-        
-        ## Initialization:
-        
-        Initialize the Refuel client with your API key. This can be done in one of two ways:
-        
-        ```python
-        import refuel
-        
-        # Assuming you've set `REFUEL_API_KEY` in your env,
-        # init() will pick it up automatically
-        refuel_client = refuel.init()
-        ```
-        
-        Alternatively, specify it as an explicit option:
-        ```python
-        import refuel
-        
-        options = {
-            "api_key": "<YOUR_API_KEY>"
-        }
-        
-        refuel_client = refuel.init(**options)
-        ```
-        
-        ## Logging data
-        
-        ### Log a single prediction event (no ground truth)
-        
-        ```python
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id1', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.42, -0.13, ...]},
-            y_pred={'scores': {'cat': 0.92, 'dog': 0.08}, 'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a single prediction event (with ground truth)
-        
-        ```python
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id2', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.35, -0.27, ...]},
-            y_pred={'scores': {'cat': 0.12, 'dog': 0.88}, 'label': 'dog'},
-            y_true={'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a single prediction event (ground truth becomes available at a later point)
-        
-        ```python
-        # This will be joined with the rest of the event logged previously
-        refuel_client.log(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            x={'id': 'id1'},
-            y_true={'label': 'cat'},
-            metadata={'camera_id': 'camera1'}
-        )
-        ```
-        
-        ### Log a batch of prediction events
-        
-        ```python
-        # List of events to be logged. 
-        events = [{'x': ..., 'y_pred': ..., 'y_true': ..., 'metadata': ...}]
-        
-        refuel_client.log_batch(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            events=events
-        )
-        ```
-        
-        ### Log a dataset stored in S3 with an s3 uri
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='s3://bucket/path/to/object.type',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        ### Log a dataset stored in GCS with a GCS uri
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='gs://bucket/path/to/object.type',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        
-        ### Log a dataset stored in S3 or GCS with a pre-signed url
-        
-        ```python
-        refuel_client.log_dataset(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            cloud_uri='https://bucket.s3.amazonaws.com/path/to/object.type?AWSAccessKeyId=1234&Signature=1234',
-            dataset_config={'type': 'CSV', 'delimiter': '\t'}
-        )
-        ```
-        
-        ## Querying data
-        
-        ### Query events table
-        
-        ```python
-        # Query events directly from a dataset
-        refuel_client.query_events(
-            model_name='my-model-name',
-            dataset_name='my-dataset-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            order_by="ordering-column",
-            offset=1234,
-            max_events=1234
-        )
-        ```
-        
-        ### Query annotation queue
-        
-        ```python
-        # Query events from the annotation queue
-        refuel_client.query_annotation_queue(
-            model_name='my-model-name',
-            queue_name='my-queue-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            order_by="ordering-column",
-            offset=1234,
-            max_events=1234
-        )
-        ```
-        
-        ### Query similar events
-        
-        ```python
-        # Query events similar to passed event
-        refuel_client.query_similar_events(
-            model_name='my-model-name',
-            refuel_uuid='refuel-uuid',
-            embedding_column='embedding-column',
-            dataset_name='my-dataset-name',
-            time_start='2022-07-01',
-            time_end='2022-08-02.',
-            filters=[{"field": "column-name", "operator": "=", "value": "1"}],
-            max_events=1234
-        )
-        ```
-        
-        # Questions?
-        
-        Reach out to us at support@refuel.ai with any questions!
-        
-        ![Tests](https://github.com/refuel-ai/refuel-python/actions/workflows/test.yml/badge.svg)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Refuel Python API
+
+<p align="center"><img height="250" src="https://user-images.githubusercontent.com/1568137/172486199-f4eddb09-7c58-4841-8f3c-60f647079073.png"></p>
+
+This is the [Refuel.ai](https://www.refuel.ai/) Python client library. The primary use for this library is to log your machine learning datasets to the Refuel platform. More features coming soon!
+
+# Installation
+You can install this library using `pip`:
+
+```bash
+pip install refuel
+```
+
+# Usage
+
+Make sure you have a valid API key from Refuel (shared with your team during onboarding). Contact us at support@refuel.ai if you need help. 
+
+## Initialization:
+
+Initialize the Refuel client with your API key. This can be done in one of two ways:
+
+```python
+import refuel
+
+# Assuming you've set `REFUEL_API_KEY` in your env,
+# init() will pick it up automatically
+refuel_client = refuel.init()
+```
+
+Alternatively, specify it as an explicit option:
+```python
+import refuel
+
+options = {
+    "api_key": "<YOUR_API_KEY>"
+}
+
+refuel_client = refuel.init(**options)
+```
+
+## Logging data
+
+### Log a single prediction event (no ground truth)
+
+```python
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id1', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.42, -0.13, ...]},
+    y_pred={'scores': {'cat': 0.92, 'dog': 0.08}, 'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a single prediction event (with ground truth)
+
+```python
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id2', 'image_url': 's3://<bucket>/<path>', 'embedding': [0.35, -0.27, ...]},
+    y_pred={'scores': {'cat': 0.12, 'dog': 0.88}, 'label': 'dog'},
+    y_true={'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a single prediction event (ground truth becomes available at a later point)
+
+```python
+# This will be joined with the rest of the event logged previously
+refuel_client.log(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    x={'id': 'id1'},
+    y_true={'label': 'cat'},
+    metadata={'camera_id': 'camera1'}
+)
+```
+
+### Log a batch of prediction events
+
+```python
+# List of events to be logged. 
+events = [{'x': ..., 'y_pred': ..., 'y_true': ..., 'metadata': ...}]
+
+refuel_client.log_batch(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    events=events
+)
+```
+
+### Log a dataset stored in S3 with an s3 uri
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='s3://bucket/path/to/object.type',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+### Log a dataset stored in GCS with a GCS uri
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='gs://bucket/path/to/object.type',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+
+### Log a dataset stored in S3 or GCS with a pre-signed url
+
+```python
+refuel_client.log_dataset(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    cloud_uri='https://bucket.s3.amazonaws.com/path/to/object.type?AWSAccessKeyId=1234&Signature=1234',
+    dataset_config={'type': 'CSV', 'delimiter': '\t'}
+)
+```
+
+## Querying data
+
+### Query events table
+
+```python
+# Query events directly from a dataset
+refuel_client.query_events(
+    model_name='my-model-name',
+    dataset_name='my-dataset-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    order_by="ordering-column",
+    offset=1234,
+    max_events=1234
+)
+```
+
+### Query annotation queue
+
+```python
+# Query events from the annotation queue
+refuel_client.query_annotation_queue(
+    model_name='my-model-name',
+    queue_name='my-queue-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    order_by="ordering-column",
+    offset=1234,
+    max_events=1234
+)
+```
+
+### Query similar events
+
+```python
+# Query events similar to passed event
+refuel_client.query_similar_events(
+    model_name='my-model-name',
+    refuel_uuid='refuel-uuid',
+    embedding_column='embedding-column',
+    dataset_name='my-dataset-name',
+    time_start='2022-07-01',
+    time_end='2022-08-02.',
+    filters=[{"field": "column-name", "operator": "=", "value": "1"}],
+    max_events=1234
+)
+```
+
+# Questions?
+
+Reach out to us at support@refuel.ai with any questions!
+
+![Tests](https://github.com/refuel-ai/refuel-python/actions/workflows/test.yml/badge.svg)
+
```

### Comparing `refuel-0.4.0/setup.py` & `refuel-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     install_requires = requirements.read().split("\n")
 
 with open(os.path.join(current_file_path, "README.md"), encoding="utf-8") as rd:
     long_description = "\n" + rd.read()
 
 setup(
     name="refuel",
-    version="0.4.0",
+    version="0.9.0",
     maintainer="Refuel.ai",
     author="Refuel.ai",
     maintainer_email="support@refuel.ai",
     author_email="support@refuel.ai",
     packages=find_packages(),
     description="Library to log your Machine Learning datasets to Refuel Platform",
     long_description=long_description,
```

