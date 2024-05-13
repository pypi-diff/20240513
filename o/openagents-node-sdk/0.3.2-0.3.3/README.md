# Comparing `tmp/openagents_node_sdk-0.3.2.tar.gz` & `tmp/openagents_node_sdk-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_node_sdk-0.3.2.tar", last modified: Sat May 11 07:58:14 2024, max compression
+gzip compressed data, was "openagents_node_sdk-0.3.3.tar", last modified: Mon May 13 08:51:08 2024, max compression
```

## Comparing `openagents_node_sdk-0.3.2.tar` & `openagents_node_sdk-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:58:14.842841 openagents_node_sdk-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 07:58:14.842841 openagents_node_sdk-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:58:14.838841 openagents_node_sdk-0.3.2/openagents/
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/Disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/DiskReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/DiskWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/JobContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/JobRunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/NodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/OpenAgentsNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/RunnerConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/openagents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 07:58:14.838841 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-11 07:58:14.000000 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-11 07:58:14.000000 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 07:58:14.000000 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-11 07:58:14.000000 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-11 07:58:14.000000 openagents_node_sdk-0.3.2/openagents_node_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 07:58:14.842841 openagents_node_sdk-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-11 07:58:12.000000 openagents_node_sdk-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:51:08.334108 openagents_node_sdk-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 08:51:08.334108 openagents_node_sdk-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:51:08.334108 openagents_node_sdk-0.3.3/openagents/
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/Disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/DiskReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/DiskWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/JobContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/JobRunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/NodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15191 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/OpenAgentsNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/RunnerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/openagents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:51:08.334108 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-13 08:51:08.000000 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 08:51:08.000000 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:51:08.000000 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 08:51:08.000000 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 08:51:08.000000 openagents_node_sdk-0.3.3/openagents_node_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:51:08.334108 openagents_node_sdk-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 08:51:05.000000 openagents_node_sdk-0.3.3/setup.py
```

### Comparing `openagents_node_sdk-0.3.2/LICENSE` & `openagents_node_sdk-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/README.md` & `openagents_node_sdk-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,21 +19,21 @@
     def __init__(self):
         # Set the runner metadata, template and filter
         super().__init__(\
             RunnerConfig(
                 meta={
                     "kind":5003,
                     "name":"My Action",
-                    "description":"This is a new action"
+                    "description":"This is a new action",
                     "tos": "https://example.com/tos",
                     "privacy": "https://example.com/privacy",
                     "picture": "https://example.com/icon.png",
-                    "tags": ["tag1","tag2"]
+                    "tags": ["tag1","tag2"],
                     "website": "https://example.com",
-                    "author": "John Doe",
+                    "author": "John Doe"
                 },
                 filter={
                     "filterByKind":5003,
                     #AND
                     "filterByRunOn": "my-new-action"
                 },
                 template="""
```

### Comparing `openagents_node_sdk-0.3.2/openagents/Disk.py` & `openagents_node_sdk-0.3.3/openagents/Disk.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/DiskReader.py` & `openagents_node_sdk-0.3.3/openagents/DiskReader.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/DiskWriter.py` & `openagents_node_sdk-0.3.3/openagents/DiskWriter.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/JobContext.py` & `openagents_node_sdk-0.3.3/openagents/JobContext.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/JobRunner.py` & `openagents_node_sdk-0.3.3/openagents/JobRunner.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/Logger.py` & `openagents_node_sdk-0.3.3/openagents/Logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,38 +42,38 @@
             level (LogLevel): The level of the log.
             message (str): The message to log.
             timestamp (int): The timestamp of the log. Defaults to the current time.
         """
         log_entry = {
             'level': level,
             '_timestamp': timestamp or int(time.time()*1000),
-            'message': message
+            'log': message
         }
         meta=self.options["meta"] if "meta" in self.options else {}
         for key in meta:
             log_entry[key]=meta[key]
 
         self.buffer.put(log_entry)
         if self.buffer.qsize() >= self.batchSize:
-            with self.wait:
-                self.wait.notify_all()
+            self.wait.notify_all()
         
     def close(self):
         """
         Immediately flush all the logs to OpenObserve and shutdown the logger.
         """
+        while not self.buffer.empty():
+            self.wait.notify_all()
+            print("Flushing logs... waiting...")
+            time.sleep(0.1)
         self.flushThread.shutdown()
-        if not self.buffer.empty():
-            batch = []
-            while not self.buffer.empty():
-                batch.append(self.buffer.get())
-            self._flushToOpenObserve(batch)
             
         
     def _flushToOpenObserve(self, batch):
+        if len(batch) == 0:
+            return
         try:
             url = self.options["baseUrl"]+"/api/"+self.options["org"]+"/"+self.options["stream"]+"/_json"   
             basicAuth = self.options["auth"]
             if not isinstance(basicAuth, str):
                 if "username" in basicAuth and "password" in basicAuth:
                     basicAuth = basicAuth["username"]+":"+basicAuth["password"]
                     basicAuth = base64.b64encode(basicAuth.encode()).decode()
@@ -86,19 +86,21 @@
                 print("Error flushing log "+str(res.status_code))
         except Exception as e:
             print("Error flushing log "+str(e))
 
 
     def flushLoop(self):
         while True:
-            with self.wait:
-                self.wait.wait(self.flushInterval/1000)
+            self.wait.wait(self.flushInterval/1000)
             batch = []
-            while not self.buffer.empty():
-                batch.append(self.buffer.get())         
+            while not self.buffer.empty() and len(batch) < self.batchSize:
+                try:
+                    batch.append(self.buffer.get(block=False))
+                except queue.Empty:
+                    break         
             self._flushToOpenObserve(batch)
 
 
     
 
 
 class Logger :
@@ -131,16 +133,16 @@
         self.name=name or "main"
         self.runnerLogger=runnerLogger
         self.logLevel=None
         self.oobsLogger=None
         self.version=version
         self.jobId=jobId
         
-        logLevelName = os.getenv('LOG_LEVEL', "debug")
-        oobsLogLevelName= os.getenv('OPENOBSERVE_LOGLEVEL', logLevelName)
+        logLevelName = os.getenv('LOG_LEVEL', "finer" if not os.getenv('PRODUCTION', None) else "info")
+        oobsLogLevelName= os.getenv('OPENOBSERVE_LOGLEVEL', "info")
 
         self.logLevel = self._levelToValue(logLevelName)
         self.oobsLogLevel = self._levelToValue(oobsLogLevelName)
         
         if level and self._levelToValue(level) > self.logLevel:
             self.logLevel = self._levelToValue(level)
```

### Comparing `openagents_node_sdk-0.3.2/openagents/NodeConfig.py` & `openagents_node_sdk-0.3.3/openagents/NodeConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/OpenAgentsNode.py` & `openagents_node_sdk-0.3.3/openagents/OpenAgentsNode.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/openagents/RunnerConfig.py` & `openagents_node_sdk-0.3.3/openagents/RunnerConfig.py`

 * *Files identical despite different names*

### Comparing `openagents_node_sdk-0.3.2/setup.py` & `openagents_node_sdk-0.3.3/setup.py`

 * *Files identical despite different names*

