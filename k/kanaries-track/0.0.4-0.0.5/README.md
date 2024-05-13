# Comparing `tmp/kanaries_track-0.0.4.tar.gz` & `tmp/kanaries_track-0.0.5.tar.gz`

## Comparing `kanaries_track-0.0.4.tar` & `kanaries_track-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/kanaries_track/__init__.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/kanaries_track/client.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/kanaries_track/config.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/kanaries_track/request.py
--rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/LICENSE
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/README.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 kanaries_track-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/kanaries_track/__init__.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/kanaries_track/client.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/kanaries_track/config.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/kanaries_track/request.py
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/LICENSE
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/README.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 kanaries_track-0.0.5/PKG-INFO
```

### Comparing `kanaries_track-0.0.4/kanaries_track/__init__.py` & `kanaries_track-0.0.5/kanaries_track/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging as _logging
 
 from .client import get_client as _get_client
 from .config import config
 
 
 __all__ = ["track", "config"]
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 _logger = _logging.getLogger("kanaries_track")
 
 _log_stream_handler = _logging.StreamHandler()
 _log_stream_handler.setFormatter(
     _logging.Formatter("%(asctime)s-%(threadName)s-%(levelname)s: %(message)s")
 )
```

### Comparing `kanaries_track-0.0.4/kanaries_track/client.py` & `kanaries_track-0.0.5/kanaries_track/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 break
             try:
                 event = self.event_queue.get(block=True, timeout=self.upload_interval_seconds - elapsed_seconds)
                 events.append(event)
             except queue.Empty:
                 break
             except Exception as e:
-                logger.error("Failed to get event from queue: %s", str(e))
+                logger.debug("Failed to get event from queue: %s", str(e))
 
         logger.debug("invoke uploading events, event count: %s", len(events))
         if events:
             self.request_client.track(events)
 
 
 class Client:
```

### Comparing `kanaries_track-0.0.4/kanaries_track/request.py` & `kanaries_track-0.0.5/kanaries_track/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,8 +51,8 @@
     def track(self, events: List[Dict[str, Any]]):
         """Send events to kanaries-track server"""
         logger.debug("send requests to server, event count: %s", len(events))
         try:
             resp = self._post("/ingest/track", events)
             logger.debug("track resp: %s", resp.text)
         except Exception as e:
-            logger.error("Failed to send events to server: %s", str(e))
+            logger.debug("Failed to send events to server: %s", str(e))
```

### Comparing `kanaries_track-0.0.4/.gitignore` & `kanaries_track-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `kanaries_track-0.0.4/LICENSE` & `kanaries_track-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kanaries_track-0.0.4/pyproject.toml` & `kanaries_track-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kanaries_track-0.0.4/PKG-INFO` & `kanaries_track-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: kanaries_track
-Version: 0.0.4
+Version: 0.0.5
 Summary: kanaries_track: track to kanaries data infra
 Project-URL: homepage, https://github.com/Kanaries/kanaries-track
 Project-URL: repository, https://github.com/Kanaries/kanaries-track
 Author-email: kanaries <support@kanaries.net>
 License-File: LICENSE
 Keywords: kanaries,track
 Classifier: License :: OSI Approved :: Apache Software License
```

