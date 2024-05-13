# Comparing `tmp/task_processing-0.9.1.tar.gz` & `tmp/task_processing-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/task_processing-0.9.1.tar", last modified: Tue Aug 16 00:54:37 2022, max compression
+gzip compressed data, was "task_processing-1.0.0.tar", last modified: Mon May 13 18:02:38 2024, max compression
```

## Comparing `task_processing-0.9.1.tar` & `task_processing-1.0.0.tar`

### file list

```diff
@@ -1,61 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-16 00:54:37.000000 task_processing-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-16 00:54:37.000000 task_processing-0.9.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/runners/
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/promise.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)     2148 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/async_runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/runners/subscription.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4798 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/task_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/mesos/
--rw-r--r--   0 runner    (1001) docker     (121)     5349 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/translator.py
--rw-r--r--   0 runner    (1001) docker     (121)     5540 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/retrying_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1829 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     3329 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)    26780 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/execution_framework.py
--rw-r--r--   0 runner    (1001) docker     (121)     8931 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/logging_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1876 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_task_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5264 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/timeout_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4908 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/task_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/mesos_pod_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/mesos/resource_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/persistence/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/file_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     2793 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/dynamodb_persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13074 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/task_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1789 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8135 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/kube_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    27449 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/kubernetes_pod_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8912 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/plugins/stateful/
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/stateful/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/plugins/stateful/stateful_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)     1582 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/task_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)     2544 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/event.py
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-08-16 00:54:17.000000 task_processing-0.9.1/task_processing/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-16 00:54:17.000000 task_processing-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1530 2022-08-16 00:54:17.000000 task_processing-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-16 00:54:37.000000 task_processing-0.9.1/task_processing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3568 2022-08-16 00:54:17.000000 task_processing-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.897953 task_processing-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 18:02:23.000000 task_processing-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-13 18:02:38.897953 task_processing-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-13 18:02:23.000000 task_processing-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 18:02:38.897953 task_processing-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-13 18:02:23.000000 task_processing-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.893953 task_processing-1.0.0/task_processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.893953 task_processing-1.0.0/task_processing/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/interfaces/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/interfaces/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/interfaces/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/interfaces/task_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.893953 task_processing-1.0.0/task_processing/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.897953 task_processing-1.0.0/task_processing/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/kube_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29676 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/kubernetes_pod_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/task_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11838 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/plugins/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.897953 task_processing-1.0.0/task_processing/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/runners/async_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/runners/promise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/runners/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/runners/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/task_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-13 18:02:23.000000 task_processing-1.0.0/task_processing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:02:38.897953 task_processing-1.0.0/task_processing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-13 18:02:38.000000 task_processing-1.0.0/task_processing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-13 18:02:38.000000 task_processing-1.0.0/task_processing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:02:38.000000 task_processing-1.0.0/task_processing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-13 18:02:38.000000 task_processing-1.0.0/task_processing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 18:02:38.000000 task_processing-1.0.0/task_processing.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `task_processing-0.9.1/task_processing/runners/promise.py` & `task_processing-1.0.0/task_processing/runners/promise.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.1/task_processing/runners/sync.py` & `task_processing-1.0.0/task_processing/runners/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,16 @@
     def run(self, task_config):
         self.executor.run(task_config)
         event_queue = self.executor.get_event_queue()
 
         while True:
             event = event_queue.get()
 
-            if event.kind == 'control' and \
-               event.message == 'stop':
-                log.info('Stop event received: {}'.format(event))
+            if event.kind == "control" and event.message == "stop":
+                log.info("Stop event received: {}".format(event))
                 return event
 
             if event.task_id != task_config.task_id:
                 event_queue.put(event)
                 time.sleep(1)  # hope somebody else picks it up?
                 continue
```

### Comparing `task_processing-0.9.1/task_processing/runners/async_runner.py` & `task_processing-1.0.0/task_processing/runners/async_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import traceback
 from collections import namedtuple
 from queue import Empty
 from threading import Thread
 
 from task_processing.interfaces.runner import Runner
 
-EventHandler = namedtuple('EventHandler', ['predicate', 'cb'])
+EventHandler = namedtuple("EventHandler", ["predicate", "cb"])
 
 log = logging.getLogger(__name__)
 
 
 class AsyncError(Exception):
     pass
 
@@ -50,16 +50,15 @@
                 return
 
             try:
                 event = event_queue.get(True, 10)
 
                 # TODO: have a default callback? raise exception when this
                 # event is ignored?
-                if event.kind == 'control' and \
-                   event.message == 'stop':
+                if event.kind == "control" and event.message == "stop":
                     self.stopping = True
                     continue
 
                 for cb in self.callbacks:
                     if cb.predicate(event):
                         try:
                             cb.cb(event)
```

### Comparing `task_processing-0.9.1/task_processing/runners/subscription.py` & `task_processing-1.0.0/task_processing/runners/subscription.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.1/task_processing/task_processor.py` & `task_processing-1.0.0/task_processing/task_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,37 +19,39 @@
 
     We use this to allow the registry and plugins to dynamically
     change their behaviors. Currently just the plugins registering executors
     """
 
     def register_task_executor(self, name, task_executor_cls):
         """Helper method for adding an executor"""
-        return self.transform(
-            ('task_executors', name), lambda _: task_executor_cls
-        )
+        return self.transform(("task_executors", name), lambda _: task_executor_cls)
 
     def register_deprecated_task_executor(self, name, task_executor_cls):
         """Helper method for adding an deprecated executor"""
         return self.transform(
-            ('deprecated_task_executors', name), lambda _: task_executor_cls
+            ("deprecated_task_executors", name), lambda _: task_executor_cls
         )
 
     def _executor_invariant(task_executors):
         """Invariant that task_executors must be TaskExecutors"""
         return (
             all(issubclass(v, TaskExecutor) for v in task_executors.values()),
-            'task_executors must always be a TaskExecutor'
+            "task_executors must always be a TaskExecutor",
         )
 
     task_executors = field(
-        type=PMap, initial=m(), factory=pmap,
+        type=PMap,
+        initial=m(),
+        factory=pmap,
         invariant=_executor_invariant,
     )
     deprecated_task_executors = field(
-        type=PMap, initial=m(), factory=pmap,
+        type=PMap,
+        initial=m(),
+        factory=pmap,
         invariant=_executor_invariant,
     )
     """
     A map of task executor names (str) to a class definition which implements
     :class:`task_processing.interfaces.TaskExecutor`
     """
 
@@ -94,18 +96,16 @@
             # Any PMap in the registry ought have no duplicate keys,
             # if they do that means two plugins tried to define the same
             # executor or something
             if type(old) == PMap:
                 conflicts = set(old.keys()) & set(new.keys())
                 if conflicts:
                     raise ValueError(
-                        '{0} is trying to register elements that already '
-                        'exist in the registry: {1}'.format(
-                            plugin_name, conflicts
-                        )
+                        "{0} is trying to register elements that already "
+                        "exist in the registry: {1}".format(plugin_name, conflicts)
                     )
             return old.update(new)
 
         self.registry = self.registry.update_with(
             conflict_check, plugin_update, name_update
         )
 
@@ -116,20 +116,21 @@
         :param dict provider_config: The arguments needed to instantiate
             the provider.
         """
         if provider in self.registry.task_executors:
             return self.registry.task_executors[provider]
         elif provider in self.registry.deprecated_task_executors:
             log.warning(
-                f'{provider} is a deprecated executor and will be removed in the future')
+                f"{provider} is a deprecated executor and will be removed in the future"
+            )
             return self.registry.deprecated_task_executors[provider]
         else:
             raise ValueError(
-                '{0} provider not registered; available providers: {1}'.format(
-                    provider, self.registry.task_executors.keys().tolist()
+                "{0} provider not registered; available providers: {1}".format(
+                    provider, list(self.registry.task_executors.keys())
                 )
             )
 
     def executor_from_config(self, provider, provider_config=None):
         if provider_config is None:
             provider_config = dict()
```

### Comparing `task_processing-0.9.1/task_processing/plugins/persistence/dynamodb_persistence.py` & `task_processing-1.0.0/task_processing/interfaces/event.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,85 @@
-import decimal
-
-import boto3.session as bsession
-from boto3.dynamodb.conditions import Key
-from pyrsistent import thaw
-
-from task_processing.interfaces.persistence import Persister
-
-
-class DynamoDBPersister(Persister):
-    def __init__(self, table_name, endpoint_url=None, session=None):
-        self.table_name = table_name
-        if not session:
-            session = bsession.Session()
-        self.ddb_client = session.client(
-            service_name='dynamodb',
-            endpoint_url=endpoint_url,
-        )
-        self.table = session.resource(
-            endpoint_url=endpoint_url,
-            service_name='dynamodb'
-        ).Table(table_name)
-
-    def read(self, task_id, comparison_operator='EQ'):
-        res = self.table.query(
-            KeyConditionExpression=Key('task_id').eq(task_id)
-        )
-        return [self.item_to_event(item) for item in res['Items']]
-
-    def write(self, event):
-        if event.kind == 'control':
-            return None
-        return self.ddb_client.put_item(
-            TableName=self.table_name,
-            Item=self._event_to_item(event)['M']
-        )
-
-    def _event_to_item(self, e):
-        raw = thaw(e)
-        if type(raw) is dict:
-            resp = {}
-            for k, v in raw.items():
-                if type(v) is str:
-                    resp[k] = {
-                        'S': v
-                    }
-                elif type(v) is bool:
-                    resp[k] = {
-                        'BOOL': v
-                    }
-                elif isinstance(v, (int, float)):
-                    resp[k] = {
-                        'N': str(v)
-                    }
-                elif type(v) is dict:
-                    resp[k] = self._event_to_item(v)
-                elif type(v) is list:
-                    if len(v) > 0:
-                        vals = []
-                        for i in v:
-                            vals.append(self._event_to_item(i))
-                        resp[k] = {
-                            'L': vals
-                        }
-            return {'M': resp}
-        elif type(raw) is str:
-            return {
-                'S': raw
-            }
-        elif type(raw) in [int, float]:
-            return {
-                'N': str(raw)
-            }
-        else:
-            print("Missed converting key %s type %s" % (raw, type(raw)))
-
-    def item_to_event(self, obj):
-        return self._replace_decimals(obj)
-
-    def _replace_decimals(self, obj):
-        if isinstance(obj, list):
-            return [self._replace_decimals(x) for x in obj]
-        elif isinstance(obj, dict):
-            return {k: self._replace_decimals(v) for k, v in obj.items()}
-        elif isinstance(obj, decimal.Decimal):
-            return float(obj)
+import json
+import uuid
+from typing import Any
+
+from pyrsistent import field
+from pyrsistent import freeze
+from pyrsistent import m
+from pyrsistent import PMap
+from pyrsistent import pmap
+from pyrsistent import PRecord
+
+EVENT_KINDS = {"task", "control"}
+EVENT_TASK_ATTRS = {"task_id", "task_config"}
+
+
+class Event(PRecord):
+    def __invariant__(self):
+        if self.kind != "task":
+            return True, "Not a task event"
+
+        missing_attrs = EVENT_TASK_ATTRS - set(self.keys())
+        if missing_attrs:
+            return False, "Missing task attributes: {}".format(missing_attrs)
+
+        return True, "Task is valid"
+
+    kind = field(
+        type=str,
+        mandatory=True,
+        invariant=lambda x: (x in EVENT_KINDS, "kind not in {}".format(EVENT_KINDS)),
+    )
+    # we store timestamps as seconds since epoch.
+    # use time.time() to generate
+    timestamp = field(type=float, initial=0.0)
+    # reference to platform-specific event object
+    raw: Any = field(mandatory=True, initial=None)
+    # free-form dictionary for stack-specific data
+    extensions = field(type=PMap, initial=m(), factory=pmap)
+    # is this the last event for a task?
+    terminal = field(type=bool, initial=False)
+
+    # task-specific fields
+    # task_id this event pertains to
+    task_id = field(type=(str, type(None)), initial=None)
+    # task config dict that sourced the task this event refers to
+    task_config = field(
+        invariant=lambda x: (isinstance(x, PMap), "task_config must inherit from PMap"),
+        factory=lambda x: pmap(x) if not isinstance(x, PMap) else x,
+        initial=m(),
+    )
+    # the task finished with exit code 0
+    success = field(type=(bool, type(None)), initial=None)
+    # platform-specific event type
+    platform_type = field(type=(str, type(None)), initial=None)
+
+    # control events
+    message = field(type=(str, type(None)), initial=None)
+
+
+def task_event(**kwargs):
+    kwargs.setdefault("kind", "task")
+    return Event(**kwargs)
+
+
+def control_event(**kwargs):
+    kwargs.setdefault("kind", "control")
+    return Event(**kwargs)
+
+
+def json_serializer(o):
+    if isinstance(o, uuid.UUID):
+        return o.hex
+    return json.JSONEncoder.default(o)
+
+
+def json_deserializer(dct):
+    for k, v in dct.items():
+        if k == "uuid":
+            try:
+                dct[k] = uuid.UUID(hex=v)
+            except ValueError:
+                dct[k] = freeze(v)
         else:
-            return obj
+            dct[k] = freeze(v)
+    return dct
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/task_metadata.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/task_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     TASK_FAILED = auto()
     TASK_UNKNOWN = auto()
     TASK_LOST = auto()
 
 
 class KubernetesTaskMetadata(PRecord):
     # what box this task/Pod was scheduled onto
-    node_name: str = field(type=str, initial='')
+    node_name: str = field(type=str, initial="")
 
     # the config used to launch this task/Pod
     task_config: KubernetesTaskConfig = field(type=KubernetesTaskConfig, mandatory=True)
 
     task_state: KubernetesTaskState = field(type=KubernetesTaskState, mandatory=True)
     # List of state to when that state was entered (stored as a timestamp)
     task_state_history: PVectorType[Tuple[KubernetesTaskState, float]] = field(
-        type=PVector, factory=pvector, mandatory=True)
+        type=PVector, factory=pvector, mandatory=True
+    )
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/task_config.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/task_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 import secrets
 import string
 from itertools import chain
+from typing import Any
 from typing import Mapping
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
 
 from pyrsistent import field
@@ -17,34 +18,40 @@
 from pyrsistent import v
 
 from task_processing.plugins.kubernetes.types import DockerVolume
 from task_processing.plugins.kubernetes.types import EmptyVolume
 from task_processing.plugins.kubernetes.types import NodeAffinity
 from task_processing.plugins.kubernetes.types import NodeAffinityOperator
 from task_processing.plugins.kubernetes.types import ObjectFieldSelectorSource
+from task_processing.plugins.kubernetes.types import SecretVolume
+from task_processing.plugins.kubernetes.types import SecretVolumeItem
 from task_processing.plugins.kubernetes.utils import get_sanitised_kubernetes_name
+from task_processing.plugins.kubernetes.utils import mode_to_int
+
 if TYPE_CHECKING:
     from task_processing.plugins.kubernetes.types import SecretEnvSource
 
 from task_processing.interfaces.task_executor import DefaultTaskConfigInterface
 
 POD_SUFFIX_ALPHABET = string.ascii_lowercase + string.digits
 POD_SUFFIX_LENGTH = 6
 # The max length is actually 253, but https://github.com/kubernetes/kubernetes/issues/91410 means
 # that the effective limit is actually:
 # 255 - 63 - 37 - 2 = 153
 # or (max filename length) - (max namespace length) -(pod UID length) - (separators)
 # but let's give ourselves a little buffer so we'll round down a bit
 MAX_POD_NAME_LENGTH = 150
 MAX_DNS_SUBDOMAIN_NAME_LENGTH = 253
-VALID_DNS_SUBDOMAIN_NAME_REGEX = '^[a-z0-9]([-a-z0-9.]*[a-z0-9])?$'
+VALID_DNS_SUBDOMAIN_NAME_REGEX = "^[a-z0-9]([-a-z0-9.]*[a-z0-9])?$"
 VALID_EMPTY_VOLUME_KEYS = set(EmptyVolume.__annotations__.keys())
 VALID_VOLUME_KEYS = set(DockerVolume.__annotations__.keys())
-VALID_SECRET_ENV_KEYS = {'secret_name', 'key'}
-VALID_FIELD_SELECTOR_ENV_KEYS = {'field_path'}
+VALID_SECRET_VOLUME_KEYS = set(SecretVolume.__annotations__.keys())
+VALID_SECRET_VOLUME_ITEM_KEYS = set(SecretVolumeItem.__annotations__.keys())
+VALID_SECRET_ENV_KEYS = {"secret_name", "key"}
+VALID_FIELD_SELECTOR_ENV_KEYS = {"field_path"}
 VALID_CAPABILITIES = {
     "AUDIT_CONTROL",
     "AUDIT_READ",
     "AUDIT_WRITE",
     "BLOCK_SUSPEND",
     "CHOWN",
     "DAC_OVERRIDE",
@@ -99,117 +106,165 @@
 }
 VALID_DOCKER_VOLUME_MODES = {"RW", "RO"}
 VALID_DOCKER_VOLUME_MEDIUM = {"Memory", None}
 REQUIRED_NODE_AFFINITY_KEYS = set(NodeAffinity.__annotations__.keys())
 
 
 def _generate_pod_suffix() -> str:
-    return ''.join(secrets.choice(POD_SUFFIX_ALPHABET) for i in range(POD_SUFFIX_LENGTH))
+    return "".join(
+        secrets.choice(POD_SUFFIX_ALPHABET) for i in range(POD_SUFFIX_LENGTH)
+    )
 
 
 def _valid_volumes(volumes: Sequence[DockerVolume]) -> Tuple[bool, Optional[str]]:
     for volume in volumes:
         if set(volume.keys()) != VALID_VOLUME_KEYS:
             return (
                 False,
-                f'Invalid volume format, must only contain following keys: '
-                f'{VALID_VOLUME_KEYS}, got: {volume.keys()}'
+                f"Invalid volume format, must only contain following keys: "
+                f"{VALID_VOLUME_KEYS}, got: {volume.keys()}",
             )
         if volume["mode"] not in VALID_DOCKER_VOLUME_MODES:
             return (
                 False,
                 f"Invalid mode for volume, must be one of {VALID_DOCKER_VOLUME_MODES}",
             )
     return (True, None)
 
 
 def _valid_empty_volumes(volumes: Sequence[EmptyVolume]) -> Tuple[bool, Optional[str]]:
     for volume in volumes:
         if set(volume.keys()) != VALID_EMPTY_VOLUME_KEYS:
             return (
                 False,
-                f'Invalid empty volume format, must only contain following keys: '
-                f'{VALID_EMPTY_VOLUME_KEYS}, got: {volume.keys()}'
+                f"Invalid empty volume format, must only contain following keys: "
+                f"{VALID_EMPTY_VOLUME_KEYS}, got: {volume.keys()}",
             )
-        if volume['medium'] not in VALID_DOCKER_VOLUME_MEDIUM:
+        if volume["medium"] not in VALID_DOCKER_VOLUME_MEDIUM:
             return (
                 False,
                 f"Invalid medium for empty volume, must be one of {VALID_DOCKER_VOLUME_MEDIUM}",
             )
     return (True, None)
 
 
-def _valid_secret_envs(secret_envs: Mapping[str, "SecretEnvSource"]) -> Tuple[bool, Optional[str]]:
+def _valid_secret_volumes(
+    volumes: Sequence[SecretVolume],
+) -> Tuple[bool, Optional[str]]:
+    for volume in volumes:
+        if set(volume.keys()) != VALID_SECRET_VOLUME_KEYS:
+            return (
+                False,
+                f"Invalid volume format, must only contain following keys: "
+                f"{VALID_SECRET_VOLUME_KEYS}, got: {volume.keys()}",
+            )
+
+        if volume["default_mode"] is not None:
+            try:
+                mode_to_int(volume["default_mode"])
+            except (TypeError, ValueError):
+                return (
+                    False,
+                    "Invalid mode for volume, expected octal value (as a string). "
+                    f"Got {volume['default_mode']}",
+                )
+
+        if volume["items"]:
+            for item in volume["items"]:
+                if set(item.keys()) != VALID_SECRET_VOLUME_ITEM_KEYS:
+                    return (
+                        False,
+                        f"Invalid secret item format, must only contain following keys: "
+                        f"{VALID_SECRET_VOLUME_ITEM_KEYS}, got: {item.keys()}",
+                    )
+
+                if item["mode"] is not None:
+                    try:
+                        mode_to_int(item["mode"])
+                    except (TypeError, ValueError):
+                        return (
+                            False,
+                            "Invalid mode for item, expected octal value (as a string). "
+                            f"Got {item['mode']}",
+                        )
+
+    return (True, None)
+
+
+def _valid_secret_envs(
+    secret_envs: Mapping[str, "SecretEnvSource"]
+) -> Tuple[bool, Optional[str]]:
     # Note we are not validating existence of secret in k8s here, leave that to creation of pod
     for key, value in secret_envs.items():
         if set(value.keys()) != VALID_SECRET_ENV_KEYS:
             return (
                 False,
-                f'Invalid secret environment variable {key}, must only contain following keys: '
-                f'{VALID_SECRET_ENV_KEYS}, got: {value.keys()}'
+                f"Invalid secret environment variable {key}, must only contain following keys: "
+                f"{VALID_SECRET_ENV_KEYS}, got: {value.keys()}",
             )
     return (True, None)
 
 
 def _valid_field_selector_envs(
     field_selector_envs: Mapping[str, "ObjectFieldSelectorSource"],
 ) -> Tuple[bool, Optional[str]]:
     # Note we are not validating existence of the path referenced by the field selector here,
     # leave that to creation of pod
     for key, value in field_selector_envs.items():
         if set(value.keys()) != VALID_FIELD_SELECTOR_ENV_KEYS:
             return (
                 False,
-                f'Invalid field selector environment variable {key}, must only contain following '
-                f'keys: {VALID_FIELD_SELECTOR_ENV_KEYS}, got: {value.keys()}'
+                f"Invalid field selector environment variable {key}, must only contain following "
+                f"keys: {VALID_FIELD_SELECTOR_ENV_KEYS}, got: {value.keys()}",
             )
     return (True, None)
 
 
 def _valid_capabilities(capabilities: Sequence[str]) -> Tuple[bool, Optional[str]]:
     if (set(capabilities) & VALID_CAPABILITIES) != set(capabilities):
         return (
             False,
             f"Invalid capabilities - got {capabilities} but expected only values from "
             f"{VALID_CAPABILITIES}",
         )
     return (True, None)
 
 
-def _valid_node_affinities(affinities: Sequence["NodeAffinity"]) -> Tuple[bool, Optional[str]]:
+def _valid_node_affinities(
+    affinities: Sequence["NodeAffinity"],
+) -> Tuple[bool, Optional[str]]:
     for aff in affinities:
         missing_keys = REQUIRED_NODE_AFFINITY_KEYS.difference(set(aff.keys()))
         if missing_keys:
             return (
                 False,
-                f"Invalid node affinity: got {aff} but missing keys {missing_keys}"
+                f"Invalid node affinity: got {aff} but missing keys {missing_keys}",
             )
 
         op, val = aff["operator"], aff["value"]
         if op not in NodeAffinityOperator:
             valid_operators = list(o.value for o in NodeAffinityOperator)
             return (
                 False,
                 f"Invalid node affinity operator: got '{op}', "
                 f"but expected one of: {valid_operators}",
             )
 
-        elif (
-            op in {NodeAffinityOperator.IN, NodeAffinityOperator.NOT_IN} and
-            type(val) not in {list, tuple}
-        ):
+        elif op in {NodeAffinityOperator.IN, NodeAffinityOperator.NOT_IN} and type(
+            val
+        ) not in {list, tuple}:
             return (
                 False,
                 "Invalid node affinity value: "
-                f"got non-list value '{val}' for affinity operator '{op}'"
+                f"got non-list value '{val}' for affinity operator '{op}'",
             )
 
         elif (
-            op in {NodeAffinityOperator.GT, NodeAffinityOperator.LT} and
-            type(val) != int
+            op in {NodeAffinityOperator.GT, NodeAffinityOperator.LT}
+            and type(val) != int
         ):
             return (
                 False,
                 "Invalid node affinity value: "
                 f"got non-int value '{val}' for affinity operator '{op}'",
             )
 
@@ -229,98 +284,130 @@
     if service_account_name is None:
         return ((True, "No account name provided"),)
 
     valid_length = 1 <= len(service_account_name) <= MAX_DNS_SUBDOMAIN_NAME_LENGTH
     valid_name = bool(re.match(VALID_DNS_SUBDOMAIN_NAME_REGEX, service_account_name))
 
     return (
-        (valid_length, f'Account name length must be >=1,<={MAX_DNS_SUBDOMAIN_NAME_LENGTH}.'),
-        (valid_name, 'Account names must be valid DNS subdomain names.'),
+        (
+            valid_length,
+            f"Account name length must be >=1,<={MAX_DNS_SUBDOMAIN_NAME_LENGTH}.",
+        ),
+        (valid_name, "Account names must be valid DNS subdomain names."),
     )
 
 
+def _float_or_none(val: Any) -> Optional[float]:
+    return float(val) if val is not None else None
+
+
 class KubernetesTaskConfig(DefaultTaskConfigInterface):
     def __invariant__(self) -> Tuple[Tuple[bool, str], ...]:
         valid_length = len(self.pod_name) <= MAX_POD_NAME_LENGTH
         valid_name = bool(re.match(VALID_DNS_SUBDOMAIN_NAME_REGEX, self.pod_name))
 
-        all_ports = list(chain.from_iterable(
-            [self.ports] + [container.ports for container in self.extra_containers.values()]))
+        all_ports = list(
+            chain.from_iterable(
+                [self.ports]
+                + [container.ports for container in self.extra_containers.values()]
+            )
+        )
         duplicate_ports = bool(len(set(all_ports)) == len(all_ports))
 
         return (
-            (valid_length, f'Pod name must have up to {MAX_POD_NAME_LENGTH} characters.'),
-            (valid_name, 'Must comply with Kubernetes pod naming standards.'),
-            (duplicate_ports, 'Containers must define unique ports.'),
+            (
+                valid_length,
+                f"Pod name must have up to {MAX_POD_NAME_LENGTH} characters.",
+            ),
+            (valid_name, "Must comply with Kubernetes pod naming standards."),
+            (duplicate_ports, "Containers must define unique ports."),
         )
 
     uuid = field(type=str, initial=_generate_pod_suffix)  # type: ignore
     name = field(type=str, initial="default")
     # Hardcoded for the time being
     restart_policy = "Never"
     # By default, the retrying executor retries 3 times. This task option
     # overrides the executor setting.
     retries = field(
         type=int,
         factory=int,
         mandatory=False,
-        invariant=lambda r: (r >= 0, 'retries >= 0')
+        invariant=lambda r: (r >= 0, "retries >= 0"),
     )
 
     image = field(type=str, mandatory=True)
     command = field(
         type=str,
         mandatory=True,
-        invariant=lambda cmd: (cmd.strip() != '', 'empty command is not allowed')
+        invariant=lambda cmd: (cmd.strip() != "", "empty command is not allowed"),
     )
     volumes = field(
         type=PVector if not TYPE_CHECKING else PVector["DockerVolume"],
         initial=v(),
         factory=pvector,
         invariant=_valid_volumes,
     )
+    secret_volumes = field(
+        type=PVector if not TYPE_CHECKING else PVector["SecretVolume"],
+        initial=v(),
+        factory=pvector,
+        invariant=_valid_secret_volumes,
+    )
 
     extra_containers = field(
         type=PMap if not TYPE_CHECKING else PMap[str, "KubernetesTaskConfig"],
         initial=m(),
         factory=pmap,
         invariant=lambda containers: (
             not any([container.extra_containers for container in containers.values()]),
-            'extra_containers cannot have extra_containers',
+            "extra_containers cannot have extra_containers",
         ),
     )
 
     cpus = field(
-        type=float,
-        initial=0.1,
-        factory=float,
-        invariant=lambda c: (c > 0, 'cpus > 0'))
+        type=float, initial=0.1, factory=float, invariant=lambda c: (c > 0, "cpus > 0")
+    )
+    cpus_request = field(
+        type=(float, type(None)),
+        factory=_float_or_none,
+        invariant=lambda c: (c is None or c > 0, "cpus_request > 0"),
+        initial=None,
+    )
+
     memory = field(
         type=float,
         initial=128.0,
         factory=float,
-        invariant=lambda m: (m >= 32, 'mem is >= 32'))
+        invariant=lambda m: (m >= 32, "mem is >= 32"),
+    )
+    memory_request = field(
+        type=(float, type(None)),
+        factory=_float_or_none,
+        invariant=lambda m: (m is None or m >= 32, "mem_request >= 32"),
+        initial=None,
+    )
+
     disk = field(
-        type=float,
-        initial=10.0,
-        factory=float,
-        invariant=lambda d: (d > 0, 'disk > 0'))
+        type=float, initial=10.0, factory=float, invariant=lambda d: (d > 0, "disk > 0")
+    )
+
     environment = field(
         type=PMap if not TYPE_CHECKING else PMap[str, str],
         initial=m(),
         factory=pmap,
     )
     secret_environment = field(
-        type=PMap if not TYPE_CHECKING else PMap[str, 'SecretEnvSource'],
+        type=PMap if not TYPE_CHECKING else PMap[str, "SecretEnvSource"],
         initial=m(),
         factory=pmap,
         invariant=_valid_secret_envs,
     )
     field_selector_environment = field(
-        type=PMap if not TYPE_CHECKING else PMap[str, 'ObjectFieldSelectorSource'],
+        type=PMap if not TYPE_CHECKING else PMap[str, "ObjectFieldSelectorSource"],
         initial=m(),
         factory=pmap,
         invariant=_valid_field_selector_envs,
     )
     cap_add = field(
         type=PVector if not TYPE_CHECKING else PVector[str],
         initial=v(),
@@ -359,15 +446,18 @@
         factory=pmap,
     )
     fs_group = field(
         type=int,
         # this is the `nobody` user at Yelp, which is what we should always be using
         # and, as such, is probably the best default to add here.
         initial=65534,
-        invariant=lambda group: (0 <= group <= 65534, 'fs_group must be >= 0 and <= 65,534'),
+        invariant=lambda group: (
+            0 <= group <= 65534,
+            "fs_group must be >= 0 and <= 65,534",
+        ),
     )
     service_account_name = field(
         type=(str, type(None)),
         initial=None,
         invariant=_valid_service_account_name,
     )
     ports = field(
@@ -379,21 +469,37 @@
     empty_volumes = field(
         type=PVector if not TYPE_CHECKING else PVector["EmptyVolume"],
         initial=v(),
         factory=pvector,
         invariant=_valid_empty_volumes,
     )
 
+    stdin = field(
+        type=bool,
+        initial=False,
+        mandatory=False,
+    )
+    stdin_once = field(
+        type=bool,
+        initial=False,
+        mandatory=False,
+    )
+    tty = field(
+        type=bool,
+        initial=False,
+        mandatory=False,
+    )
+
     @property
     def pod_name(self) -> str:
         return get_sanitised_kubernetes_name(
-            f'{self.name}.{self.uuid}',  # type: ignore
+            f"{self.name}.{self.uuid}",  # type: ignore
             length_limit=MAX_POD_NAME_LENGTH,
         )
 
     def set_pod_name(self, pod_name: str):
         try:
-            name, uuid = pod_name.rsplit('.', maxsplit=1)
+            name, uuid = pod_name.rsplit(".", maxsplit=1)
         except ValueError:
-            raise ValueError(f'Invalid format for pod_name {pod_name}')
+            raise ValueError(f"Invalid format for pod_name {pod_name}")
 
         return self.set(name=name, uuid=uuid)
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/types.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import enum
 from typing import Any
 from typing import Dict
+from typing import List
 from typing import Optional
 
 from kubernetes.client import V1Pod
 from typing_extensions import TypedDict
 
 
 class DockerVolume(TypedDict):
@@ -15,14 +16,28 @@
 
 class EmptyVolume(TypedDict):
     container_path: str
     medium: Optional[str]  # XXX: Optional[Literal["Memory"]] In this case
     size: Optional[str]  # XXX: implement a validator for this
 
 
+class SecretVolumeItem(TypedDict):
+    key: str
+    path: str
+    mode: Optional[str]  # octal permissions mode
+
+
+class SecretVolume(TypedDict):
+    secret_volume_name: str
+    secret_name: str
+    container_path: str
+    default_mode: Optional[str]  # octal permissions mode
+    items: List[SecretVolumeItem]
+
+
 class SecretEnvSource(TypedDict):
     secret_name: str  # full name of k8s secret resource
     key: str
 
 
 class ObjectFieldSelectorSource(TypedDict):
     field_path: str  # full field path - e.g., status.podIP
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/kube_client.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/kube_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,28 @@
 
 class ExceededMaxAttempts(Exception):
     pass
 
 
 class KubeClient:
     def __init__(
-        self,
-        kubeconfig_path: Optional[str] = None,
-        user_agent: Optional[str] = None
+        self, kubeconfig_path: Optional[str] = None, user_agent: Optional[str] = None
     ) -> None:
         kubeconfig_path = kubeconfig_path or os.environ.get("KUBECONFIG")
         if kubeconfig_path is None:
             raise ValueError(
                 "No kubeconfig specified: set a KUBECONFIG environment variable "
                 "or pass a value for `kubeconfig_path`!"
             )
 
         self.kubeconfig_path = kubeconfig_path
         self.kubecontext = os.environ.get("KUBECONTEXT")
 
         kube_config.load_kube_config(
-            config_file=self.kubeconfig_path,
-            context=self.kubecontext
+            config_file=self.kubeconfig_path, context=self.kubecontext
         )
 
         self.user_agent = user_agent
         self.initialize_api_client()
 
     def initialize_api_client(self) -> None:
         self.api_client = kube_client.ApiClient()
@@ -57,16 +54,15 @@
 
         Since we rotate certs regularly internally and the kubernetes clientlib doesn't
         automatically watch for changes to the certs specified by the kubeconfig file, we
         need to manually reload said file as well as recreate any API classes (as otherwise
         they don't pick up the new configuration)
         """
         kube_config.load_kube_config(
-            config_file=self.kubeconfig_path,
-            context=self.kubecontext
+            config_file=self.kubeconfig_path, context=self.kubecontext
         )
         self.initialize_api_client()
         self.core = kube_client.CoreV1Api(self.api_client)
 
     def maybe_reload_on_exception(self, exception: Exception) -> bool:
         """
         Small wrapper around KubeClient::reload_kubeconfig() to centralize when to reload kubeconfig
@@ -79,15 +75,17 @@
             if exception.status == HTTPStatus.UNAUTHORIZED.value:
                 logger.info(
                     "Recieved UNAUTHORIZED response from apiserver - assuming certs have "
                     "expired and reloading."
                 )
                 self.reload_kubeconfig()
                 return True
-            logger.info(f"Recieved HTTP {exception.status} from apiserver, not reloading certs.")
+            logger.info(
+                f"Recieved HTTP {exception.status} from apiserver, not reloading certs."
+            )
         return False
 
     def terminate_pod(
         self,
         namespace: str,
         pod_name: str,
         attempts: int = DEFAULT_ATTEMPTS,
@@ -106,38 +104,45 @@
                     namespace=namespace,
                     # attempt to delete immediately - Pods launched by task_processing
                     # shouldn't need time to clean-up/drain
                     grace_period_seconds=0,
                     # this is the default, but explcitly request background deletion of releated
                     # objects. see:
                     # https://kubernetes.io/docs/concepts/workloads/controllers/garbage-collection/
-                    propagation_policy="Background"
+                    propagation_policy="Background",
                 )
                 # this is not ideal, but the k8s clientlib should return the status of the request
                 # as a string that is either "Success" or "Failure" (or we could potentially use
                 # `code` instead but it's not exactly documented what HTTP return codes will be
                 # used)...however, due to https://github.com/kubernetes-client/python/issues/1523
                 # the V1Status.status returned by delete_namespaced_pod is not accurate and thus
                 # we assume that if no exception was thrown, we were able to successfully send
                 # the termination request.
                 return True
             except ApiException as e:
+                if e.status == 404:
+                    logger.info(
+                        f"Found no pods matching {pod_name} - returning success since we're in the desired state."
+                    )
+                    return True
                 if not self.maybe_reload_on_exception(exception=e) and attempts:
                     logger.exception(
                         f"Failed to request termination for {pod_name} due to unhandled API "
                         "exception, retrying."
                     )
                 attempts -= 1
             except Exception:
                 logger.exception(
                     f"Failed to request termination for {pod_name} due to unhandled exception."
                 )
                 return False
 
-        logger.info(f"Ran out of retries attempting to request termination of {pod_name}.")
+        logger.info(
+            f"Ran out of retries attempting to request termination of {pod_name}."
+        )
         return False
 
     def create_pod(
         self,
         namespace: str,
         pod: V1Pod,
         attempts: int = DEFAULT_ATTEMPTS,
@@ -170,34 +175,40 @@
                 )
                 return False
 
         logger.info(f"Ran out of retries attempting to create {pod.metadata.name}.")
         return False
 
     def get_pod(
-        self, namespace: str, pod_name: str, attempts: int = DEFAULT_ATTEMPTS,
+        self,
+        namespace: str,
+        pod_name: str,
+        attempts: int = DEFAULT_ATTEMPTS,
     ) -> Optional[V1Pod]:
         max_attempts = attempts
         while attempts:
             try:
                 pod = self.core.read_namespaced_pod(
-                    namespace=namespace, name=pod_name,
+                    namespace=namespace,
+                    name=pod_name,
                 )
                 return pod
             except ApiException as e:
                 # Unknown pod throws ApiException w/ 404
                 if e.status == 404:
                     logger.info(f"Found no pods matching {pod_name}.")
                     return None
                 if not self.maybe_reload_on_exception(exception=e) and attempts:
                     logger.debug(
                         f"Failed to fetch pod {pod_name} due to unhandled API exception, retrying",
-                        exc_info=True
+                        exc_info=True,
                     )
                 attempts -= 1
             except Exception:
                 logger.exception(
                     f"Failed to fetch pod {pod_name} due to unhandled exception."
                 )
                 raise
         logger.info(f"Ran out of retries attempting to fetch pod {pod_name}.")
-        raise ExceededMaxAttempts(f'Retried fetching pod {pod_name} {max_attempts} times.')
+        raise ExceededMaxAttempts(
+            f"Retried fetching pod {pod_name} {max_attempts} times."
+        )
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/kubernetes_pod_executor.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/kubernetes_pod_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,20 +25,24 @@
 from task_processing.interfaces.event import Event
 from task_processing.interfaces.event import task_event
 from task_processing.plugins.kubernetes.kube_client import KubeClient
 from task_processing.plugins.kubernetes.task_config import KubernetesTaskConfig
 from task_processing.plugins.kubernetes.task_metadata import KubernetesTaskMetadata
 from task_processing.plugins.kubernetes.task_metadata import KubernetesTaskState
 from task_processing.plugins.kubernetes.types import PodEvent
-from task_processing.plugins.kubernetes.utils import get_capabilities_for_capability_changes
+from task_processing.plugins.kubernetes.utils import (
+    get_capabilities_for_capability_changes,
+)
 from task_processing.plugins.kubernetes.utils import get_kubernetes_empty_volume_mounts
 from task_processing.plugins.kubernetes.utils import get_kubernetes_env_vars
+from task_processing.plugins.kubernetes.utils import get_kubernetes_secret_volume_mounts
 from task_processing.plugins.kubernetes.utils import get_kubernetes_volume_mounts
 from task_processing.plugins.kubernetes.utils import get_node_affinity
 from task_processing.plugins.kubernetes.utils import get_pod_empty_volumes
+from task_processing.plugins.kubernetes.utils import get_pod_secret_volumes
 from task_processing.plugins.kubernetes.utils import get_pod_volumes
 from task_processing.plugins.kubernetes.utils import get_sanitised_kubernetes_name
 
 logger = logging.getLogger(__name__)
 
 POD_WATCH_THREAD_JOIN_TIMEOUT_S = 1.0
 POD_EVENT_THREAD_JOIN_TIMEOUT_S = 1.0
@@ -57,26 +61,29 @@
     def __init__(
         self,
         namespace: str,
         version: Optional[str] = None,
         kubeconfig_path: Optional[str] = None,
         task_configs: Optional[Collection[KubernetesTaskConfig]] = [],
         emit_events_without_state_transitions: bool = False,
-
     ) -> None:
         if not version:
             version = "unknown_task_processing"
         user_agent = f"{namespace}/v{version}"
-        self.kube_client = KubeClient(kubeconfig_path=kubeconfig_path, user_agent=user_agent)
+        self.kube_client = KubeClient(
+            kubeconfig_path=kubeconfig_path, user_agent=user_agent
+        )
         self.namespace = namespace
 
         # Pod modified events that did not result in a pod state transition are usually not
         # forwarded, but some consumers are interested in container state changes. This
         # variable controls whether such additional pod modified events are forwarded.
-        self.emit_events_without_state_transitions = emit_events_without_state_transitions
+        self.emit_events_without_state_transitions = (
+            emit_events_without_state_transitions
+        )
 
         self.stopping = False
         self.task_metadata: PMap[str, KubernetesTaskMetadata] = pmap()
 
         self.task_metadata_lock = threading.RLock()
         if task_configs:
             for task_config in task_configs:
@@ -106,33 +113,31 @@
 
         self.pending_event_processing_thread = threading.Thread(
             target=self._pending_event_processing_loop,
         )
         self.pending_event_processing_thread.start()
 
     def _initialize_existing_task(self, task_config: KubernetesTaskConfig) -> None:
-        """ Generates task_metadata in UNKNOWN state for an existing KubernetesTaskConfig.
-            Used during initialization or recovery for a task"""
+        """Generates task_metadata in UNKNOWN state for an existing KubernetesTaskConfig.
+        Used during initialization or recovery for a task"""
         pod_name = task_config.pod_name
-        logger.debug(
-            f"Initializing task metadata for known pod {pod_name}"
-        )
+        logger.debug(f"Initializing task metadata for known pod {pod_name}")
         # We are initiating with UNKNOWN state on initial load, then leave
         # matching tasks to running/completed pods in reconcile()
         with self.task_metadata_lock:
             self.task_metadata = self.task_metadata.set(
                 pod_name,
                 KubernetesTaskMetadata(
                     task_config=task_config,
-                    node_name='UNKNOWN',
+                    node_name="UNKNOWN",
                     task_state=KubernetesTaskState.TASK_UNKNOWN,
                     task_state_history=v(
                         (KubernetesTaskState.TASK_UNKNOWN, time.time())
                     ),
-                )
+                ),
             )
 
     def _pod_event_watch_loop(self) -> None:
         logger.debug(f"Starting watching Pod events for namespace={self.namespace}.")
         # TODO(TASKPROC-243): we'll need to correctly handle resourceVersion expiration for the case
         # where the gap between task_proc shutting down and coming back up is long enough for data
         # to have expired from etcd as well as actually restarting from the last resourceVersion in
@@ -140,16 +145,15 @@
         # TODO: Do LIST + WATCH if we're not starting from a known/good resourceVersion to
         # guarantee that we always get ordered events (starting from a resourceVersion of 0)
         # has no such guarantees that the initial events will be ordered in any meaningful way
         # see: https://github.com/kubernetes/kubernetes/issues/74022
         while not self.stopping:
             try:
                 for pod_event in self.watch.stream(
-                    self.kube_client.core.list_namespaced_pod,
-                    self.namespace
+                    self.kube_client.core.list_namespaced_pod, self.namespace
                 ):
                     # it's possible that we've received an event after we've already set the stop
                     # flag since Watch streams block forever, so re-check if we've stopped before
                     # queueing any pending events
                     if not self.stopping:
                         logger.debug("Adding Pod event to pending event queue.")
                         self.pending_events.put(pod_event)
@@ -164,52 +168,54 @@
             except Exception:
                 # we want to avoid a potentially misleading log message should we encounter
                 # an exception when we want to shutdown this thread since nothing of value
                 # will be lost anyway (example scenario: we've called stop() on an idle cluster
                 # but the Watch is still blocking and eventually gets disconnected)
                 if not self.stopping:
                     logger.exception(
-                        "Exception encountered while watching Pod events - restarting watch!")
+                        "Exception encountered while watching Pod events - restarting watch!"
+                    )
         logger.debug("Exiting Pod event watcher - stop requested.")
 
     def __handle_deleted_pod_event(self, event: PodEvent) -> None:
         pod = event["object"]
         pod_name = pod.metadata.name
         task_metadata = self.task_metadata[pod_name]
-        raw_event = event['raw_object']
+        raw_event = event["raw_object"]
 
         logger.info(f"Removing {pod_name} from state and emitting 'killed' event.")
 
         self.task_metadata = self.task_metadata.discard(pod_name)
         self.event_queue.put(
             task_event(
                 task_id=pod_name,
                 terminal=True,
                 success=False,
                 timestamp=time.time(),
                 raw=raw_event,
                 task_config=task_metadata.task_config,
-                platform_type="killed"
+                platform_type="killed",
             )
         )
 
     def __handle_modified_pod_event(self, event: PodEvent) -> None:
         pod = event["object"]
         self.__update_modified_pod(pod=pod, event=event)
 
     def __update_modified_pod(self, pod: V1Pod, event: Optional[PodEvent]) -> None:
-        """ Called during reconciliation and normal event handling """
+        """Called during reconciliation and normal event handling"""
         pod_name = pod.metadata.name
         task_metadata = self.task_metadata[pod_name]
+        event_type = event["type"] if event else "null"
 
-        raw_event = event['raw_object'] if event else None
+        raw_event = event["raw_object"] if event else None
 
         if pod.status.phase not in SUPPORTED_POD_MODIFIED_EVENT_PHASES:
             logger.debug(
-                f"Got a MODIFIED event for {pod_name} for unhandled phase: "
+                f"Got a {event_type} event for {pod_name} for unhandled phase: "
                 f"{pod.status.phase} - ignoring."
             )
             return
 
         if (
             pod.status.phase in {"Succeeded", "Failed"}
             and task_metadata.task_state is KubernetesTaskState.TASK_PENDING
@@ -221,25 +227,25 @@
             self.task_metadata = self.task_metadata.set(
                 pod_name,
                 task_metadata.set(
                     node_name=pod.spec.node_name,
                     task_state=KubernetesTaskState.TASK_RUNNING,
                     task_state_history=task_metadata.task_state_history.append(
                         (KubernetesTaskState.TASK_RUNNING, time.time()),
-                    )
-                )
+                    ),
+                ),
             )
             self.event_queue.put(
                 task_event(
                     task_id=pod_name,
                     terminal=False,
                     timestamp=time.time(),
                     raw=raw_event,
                     task_config=task_metadata.task_config,
-                    platform_type="running"
+                    platform_type="running",
                 )
             )
 
         if (
             pod.status.phase == "Succeeded"
             and task_metadata.task_state is not KubernetesTaskState.TASK_FINISHED
         ):
@@ -251,15 +257,15 @@
                 task_event(
                     task_id=pod_name,
                     terminal=True,
                     success=True,
                     timestamp=time.time(),
                     raw=raw_event,
                     task_config=task_metadata.task_config,
-                    platform_type="finished"
+                    platform_type="finished",
                 )
             )
             return
 
         elif (
             pod.status.phase == "Failed"
             and task_metadata.task_state is not KubernetesTaskState.TASK_FAILED
@@ -270,15 +276,15 @@
                 task_event(
                     task_id=pod_name,
                     terminal=True,
                     success=False,
                     timestamp=time.time(),
                     raw=raw_event,
                     task_config=task_metadata.task_config,
-                    platform_type="failed"
+                    platform_type="failed",
                 )
             )
             return
 
         elif (
             pod.status.phase == "Running"
             and task_metadata.task_state is not KubernetesTaskState.TASK_RUNNING
@@ -287,58 +293,58 @@
             self.task_metadata = self.task_metadata.set(
                 pod_name,
                 task_metadata.set(
                     node_name=pod.spec.node_name,
                     task_state=KubernetesTaskState.TASK_RUNNING,
                     task_state_history=task_metadata.task_state_history.append(
                         (KubernetesTaskState.TASK_RUNNING, time.time()),
-                    )
-                )
+                    ),
+                ),
             )
             self.event_queue.put(
                 task_event(
                     task_id=pod_name,
                     terminal=False,
                     timestamp=time.time(),
                     raw=raw_event,
                     task_config=task_metadata.task_config,
-                    platform_type="running"
+                    platform_type="running",
                 )
             )
             return
 
         # XXX: figure out how to handle this correctly (and when this actually
         # happens - we were unable to cajole k8s into giving us an event with an Unknown
         # phase)
         elif (
             pod.status.phase == "Unknown"
             and task_metadata.task_state is not KubernetesTaskState.TASK_LOST
         ):
             logger.info(
-                f"Got a MODIFIED event for {pod_name} with unknown phase, host likely "
+                f"Got a {event_type} event for {pod_name} with unknown phase, host likely "
                 "unexpectedly died"
             )
             self.task_metadata = self.task_metadata.set(
                 pod_name,
                 task_metadata.set(
                     node_name=pod.spec.node_name,
                     task_state=KubernetesTaskState.TASK_LOST,
                     task_state_history=task_metadata.task_state_history.append(
                         (KubernetesTaskState.TASK_LOST, time.time()),
-                    )
-                )
+                    ),
+                ),
             )
             self.event_queue.put(
                 task_event(
                     task_id=pod_name,
                     terminal=False,
                     timestamp=time.time(),
                     raw=raw_event,
                     task_config=task_metadata.task_config,
-                    platform_type="lost"
+                    platform_type="lost",
                 )
             )
             return
 
         if self.emit_events_without_state_transitions:
             self.event_queue.put(
                 task_event(
@@ -348,15 +354,15 @@
                     raw=raw_event,
                     task_config=task_metadata.task_config,
                     platform_type="running",
                 )
             )
         else:
             logger.info(
-                f"Ignoring MODIFIED event for {pod_name} as it did not result "
+                f"Ignoring {event_type} event for {pod_name} as it did not result "
                 "in a state transition",
             )
 
     def _process_pod_event(self, event: PodEvent) -> None:
         """
         Router for handling Pod events based on event type. Currently, we only look at
         MODIFIED and DELETED events (we ignore ADDED since we handle all processing for
@@ -368,28 +374,32 @@
         don't have any value for us.
 
         """
         pod = event["object"]
         pod_name = pod.metadata.name
         with self.task_metadata_lock:
             if pod_name not in self.task_metadata:
-                logger.info(f"Ignoring event for {pod_name} - Pod not tracked by task_processing.")
+                logger.info(
+                    f"Ignoring event for {pod_name} - Pod not tracked by task_processing."
+                )
                 return None
 
             # this should only ever be run for Pods that were killed either by operator
             # action (e.g., kubectl delete pod) or by calling kill() - completed/failed
             # Pods will be removed from task_processing's metadata store
             elif event["type"] == "DELETED":
                 self.__handle_deleted_pod_event(event)
 
-            elif event["type"] == "MODIFIED":
+            elif event["type"] in {"MODIFIED", "ADDED"}:
                 self.__handle_modified_pod_event(event)
 
             else:
-                logger.warning(f"Got unknown event type for {pod_name}: {event['type']}")
+                logger.warning(
+                    f"Got unknown event type for {pod_name}: {event['type']}"
+                )
 
     def _pending_event_processing_loop(self) -> None:
         """
         Run in a thread to process PodEvents enqueued by the k8s event watcher thread.
         """
         logger.debug("Starting Pod event processing.")
         event = None
@@ -412,79 +422,102 @@
 
             try:
                 self.pending_events.task_done()
             except ValueError:
                 # this should never happen since the only codepath that should ever get
                 # here is after a successful get() - but just in case, we don't want to
                 # have this thread die because of this
-                logger.error("task_done() called on pending events queue too many times!")
+                logger.error(
+                    "task_done() called on pending events queue too many times!"
+                )
 
         logger.debug("Exiting Pod event processing - stop requested.")
 
     def _create_container_definition(
         self,
         name: str,
         task_config: KubernetesTaskConfig,
     ) -> V1Container:
         volume_mounts = (
             get_kubernetes_volume_mounts(task_config.volumes)
             + get_kubernetes_empty_volume_mounts(task_config.empty_volumes)
+            + get_kubernetes_secret_volume_mounts(task_config.secret_volumes)
         )
 
         capabilities = get_capabilities_for_capability_changes(
             cap_add=task_config.cap_add,
             cap_drop=task_config.cap_drop,
         )
 
         security_context = None
         if capabilities is not None or task_config.privileged is not None:
             security_context = V1SecurityContext(
                 capabilities=capabilities,
                 privileged=task_config.privileged,
             )
 
+        requests = {}
+        # we need to explictly omit these if not set as k8s
+        # (or the python clientlib) will actually set the
+        # request to None instead of equal to the limit
+        if task_config.cpus_request is not None:
+            requests["cpu"] = task_config.cpus_request
+        if task_config.memory_request is not None:
+            requests["memory"] = f"{task_config.memory_request}Mi"
+
+        limits = {
+            "cpu": task_config.cpus,
+            "memory": f"{task_config.memory}Mi",
+            "ephemeral-storage": f"{task_config.disk}Mi",
+        }
+        resources = V1ResourceRequirements(
+            limits=limits,
+            # None is the default for an empty V1ResourceRequirements
+            requests=requests if requests else None,
+        )
+
         return V1Container(
             image=task_config.image,
             name=name,
             command=["/bin/sh", "-c"],
             args=[task_config.command],
             security_context=security_context,
-            resources=V1ResourceRequirements(
-                limits={
-                    "cpu": task_config.cpus,
-                    "memory": f"{task_config.memory}Mi",
-                    "ephemeral-storage": f"{task_config.disk}Mi",
-                }
-            ),
+            resources=resources,
             env=get_kubernetes_env_vars(
                 environment=task_config.environment,
                 secret_environment=task_config.secret_environment,
                 field_selector_environment=task_config.field_selector_environment,
             ),
             volume_mounts=volume_mounts,
             ports=[V1ContainerPort(container_port=port) for port in task_config.ports],
+            stdin=task_config.stdin,
+            stdin_once=task_config.stdin_once,
+            tty=task_config.tty,
         )
 
     def run(self, task_config: KubernetesTaskConfig) -> Optional[str]:
         try:
             # XXX: we were initially planning on using the name from KubernetesTaskConfig here,
             # but its too easy to go over the length limit for container names (63 characters),
             # so we're just hardcoding something for now since container names aren't used for
             # anything at the moment
             containers = [self._create_container_definition("main", task_config)]
 
             for name, nested_config in task_config.extra_containers.items():
-                containers.append(self._create_container_definition(
-                    get_sanitised_kubernetes_name(name, length_limit=63),
-                    nested_config,
-                ))
+                containers.append(
+                    self._create_container_definition(
+                        get_sanitised_kubernetes_name(name, length_limit=63),
+                        nested_config,
+                    )
+                )
 
             volumes = (
                 get_pod_volumes(task_config.volumes)
                 + get_pod_empty_volumes(task_config.empty_volumes)
+                + get_pod_secret_volumes(task_config.secret_volumes)
             )
 
             pod = V1Pod(
                 metadata=V1ObjectMeta(
                     name=task_config.pod_name,
                     namespace=self.namespace,
                     labels=dict(task_config.labels),
@@ -551,63 +584,83 @@
 
         if pod_name not in self.task_metadata:
             self._initialize_existing_task(task_config)
 
         with self.task_metadata_lock:
             task_metadata = self.task_metadata[pod_name]
             self.task_metadata = self.task_metadata.set(
-                pod_name,
-                task_metadata.set(
-                    task_config=task_config
-                )
+                pod_name, task_metadata.set(task_config=task_config)
             )
 
             if not pod:
                 # Pod has gone away while restarting
                 logger.info(
                     f"Pod {pod_name} for task {task_config.name} was no longer found. "
                     "Marking as LOST"
                 )
                 self.task_metadata = self.task_metadata.set(
                     pod_name,
                     task_metadata.set(
                         task_state=KubernetesTaskState.TASK_LOST,
                         task_state_history=task_metadata.task_state_history.append(
                             (KubernetesTaskState.TASK_LOST, time.time()),
-                        )
-                    )
+                        ),
+                    ),
                 )
                 self.event_queue.put(
                     task_event(
                         task_id=pod_name,
                         terminal=False,
                         timestamp=time.time(),
                         raw=None,
                         task_config=task_metadata.task_config,
-                        platform_type="lost"
+                        platform_type="lost",
                     )
                 )
             else:
                 # Treat like a modified pod
                 self.__update_modified_pod(pod=pod, event=None)
 
     def kill(self, task_id: str) -> bool:
         """
         Terminate a Pod by name.
 
         This function will request that Kubernetes delete the named Pod and will return
         True if the Pod termination request was succesfully emitted or False otherwise.
         """
-        # NOTE: we're purposely not removing this task from `task_metadata` as we want
-        # to handle that with the Watch that we'll set to monitor each Pod for events.
-        # TODO(TASKPROC-242): actually handle termination events
-        return self.kube_client.terminate_pod(
+        terminated = self.kube_client.terminate_pod(
             namespace=self.namespace,
             pod_name=task_id,
         )
+        if terminated:
+            logger.info(
+                f"Successfully requested termination for {task_id}. "
+                "Emitting synthetic 'killed' event in case of Kubernetes event coalescion."
+            )
+            # we need to lock here since there will be other threads updating this metadata in response
+            # to k8s events
+            with self.task_metadata_lock:
+                # NOTE: it's possible that there'll also be a real DELETED event for this Pod
+                # but it should be safe to do this as _process_pod_event() will just ignore
+                # pods not in self.task_metadata
+                self.task_metadata = self.task_metadata.discard(task_id)
+                self.event_queue.put(
+                    task_event(
+                        task_id=task_id,
+                        terminal=True,
+                        success=False,
+                        timestamp=time.time(),
+                        raw=None,
+                        task_config=None,
+                        platform_type="killed",
+                    )
+                )
+        else:
+            logger.error(f"Failed to request termination for {task_id}.")
+        return terminated
 
     def stop(self) -> None:
         logger.debug("Preparing to stop all KubernetesPodExecutor threads.")
         self.stopping = True
 
         logger.debug("Signaling Pod event Watch to stop streaming events...")
         # make sure that we've stopped watching for events before calling join() - otherwise,
@@ -622,13 +675,15 @@
         logger.debug("Waiting for all pending PodEvents to be processed...")
         # once we've stopped updating the pending events queue, we then wait until we're done
         # processing any events we've received - this will wait until task_done() has been
         # called for every item placed in this queue
         self.pending_events.join()
         logger.debug("All pending PodEvents have been processed.")
         # and then give ourselves time to do any post-stop cleanup
-        self.pending_event_processing_thread.join(timeout=POD_EVENT_THREAD_JOIN_TIMEOUT_S)
+        self.pending_event_processing_thread.join(
+            timeout=POD_EVENT_THREAD_JOIN_TIMEOUT_S
+        )
 
         logger.debug("Done stopping KubernetesPodExecutor!")
 
     def get_event_queue(self) -> "Queue[Event]":
         return self.event_queue
```

### Comparing `task_processing-0.9.1/task_processing/plugins/kubernetes/utils.py` & `task_processing-1.0.0/task_processing/plugins/kubernetes/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,32 @@
 from typing import TYPE_CHECKING
 
 from kubernetes.client import V1Capabilities
 from kubernetes.client import V1EmptyDirVolumeSource
 from kubernetes.client import V1EnvVar
 from kubernetes.client import V1EnvVarSource
 from kubernetes.client import V1HostPathVolumeSource
+from kubernetes.client import V1KeyToPath
 from kubernetes.client import V1NodeAffinity
 from kubernetes.client import V1NodeSelector
 from kubernetes.client import V1NodeSelectorRequirement
 from kubernetes.client import V1NodeSelectorTerm
 from kubernetes.client import V1ObjectFieldSelector
 from kubernetes.client import V1SecretKeySelector
+from kubernetes.client import V1SecretVolumeSource
 from kubernetes.client import V1Volume
 from kubernetes.client import V1VolumeMount
 from pyrsistent.typing import PMap
 from pyrsistent.typing import PVector
 
 from task_processing.plugins.kubernetes.types import NodeAffinityOperator
+
 if TYPE_CHECKING:
     from task_processing.plugins.kubernetes.types import EmptyVolume
+    from task_processing.plugins.kubernetes.types import SecretVolume
     from task_processing.plugins.kubernetes.types import DockerVolume
     from task_processing.plugins.kubernetes.types import NodeAffinity
     from task_processing.plugins.kubernetes.types import SecretEnvSource
     from task_processing.plugins.kubernetes.types import ObjectFieldSelectorSource
 
 logger = logging.getLogger(__name__)
 
@@ -38,66 +42,67 @@
 ) -> Optional[V1Capabilities]:
     """
     Helper to take lists of capabilties to add/drop and turn them into the
     corresponding Kubernetes representation.
     """
     caps = {
         capability_type: capabilities
-        for (capability_type, capabilities)
-        in [("add", list(cap_add)), ("drop", list(cap_drop))]
+        for (capability_type, capabilities) in [
+            ("add", list(cap_add)),
+            ("drop", list(cap_drop)),
+        ]
         if capabilities
     }
     if caps:
         return V1Capabilities(**caps)
 
-    logger.info(
-        "No capabilities found, not creating a capabilities object"
-    )
+    logger.info("No capabilities found, not creating a capabilities object")
     return None
 
 
 def get_kubernetes_env_vars(
     environment: PMap[str, str],
-    secret_environment: PMap[str, 'SecretEnvSource'],
-    field_selector_environment: PMap[str, 'ObjectFieldSelectorSource'],
+    secret_environment: PMap[str, "SecretEnvSource"],
+    field_selector_environment: PMap[str, "ObjectFieldSelectorSource"],
 ) -> List[V1EnvVar]:
     """
     Given a dict of environment variables, transform them into the corresponding Kubernetes
     representation. This function will replace any secret placeholders with the value of
     the actual secret.
     """
     env_vars = [
-        V1EnvVar(name=key, value=value) for key, value
-        in environment.items() if key not in secret_environment.keys()
+        V1EnvVar(name=key, value=value)
+        for key, value in environment.items()
+        if key not in secret_environment.keys()
     ]
 
     secret_env_vars = [
-        V1EnvVar(name=key, value_from=V1EnvVarSource(
-            secret_key_ref=V1SecretKeySelector(
-                name=value["secret_name"],
-                key=value["key"],
-                optional=False,
+        V1EnvVar(
+            name=key,
+            value_from=V1EnvVarSource(
+                secret_key_ref=V1SecretKeySelector(
+                    name=value["secret_name"],
+                    key=value["key"],
+                    optional=False,
+                ),
             ),
-        ),
         )
-        for key, value
-        in secret_environment.items()
+        for key, value in secret_environment.items()
     ]
 
     field_selector_env_vars = [
         V1EnvVar(
             name=key,
             value_from=V1EnvVarSource(
                 field_ref=V1ObjectFieldSelector(
                     field_path=value["field_path"],
                 )
             ),
         )
-        for key, value
-        in field_selector_environment.items()
+        for key, value in field_selector_environment.items()
     ]
 
     return env_vars + secret_env_vars + field_selector_env_vars
 
 
 def get_sanitised_kubernetes_name(
     name: str,
@@ -127,15 +132,15 @@
 
     if length_limit and len(name) > length_limit:
         # for names that exceed the length limit, we'll remove 6 characters from
         # the part of the name that does fit in the limit in order to replace them with
         # -- (2 characters) and then a 4 character hash (which should help ensure uniqueness
         # after truncation).
         name = (
-            name[0:length_limit - 6]
+            name[0 : length_limit - 6]
             + "--"
             + hashlib.md5(name.encode("ascii")).hexdigest()[:4]
         )
     return name.lower()
 
 
 def get_sanitised_volume_name(volume_name: str, length_limit: int = 0) -> str:
@@ -150,88 +155,167 @@
         volume_name,
         replace_dots=True,
         replace_forward_slash=True,
         length_limit=length_limit,
     )
 
 
-def get_kubernetes_volume_mounts(volumes: PVector['DockerVolume']) -> List[V1VolumeMount]:
+def get_kubernetes_volume_mounts(
+    volumes: PVector["DockerVolume"],
+) -> List[V1VolumeMount]:
     """
     Given a list of volume mounts, return a list corresponding to the Kubernetes objects
     representing these mounts.
     """
     return [
         V1VolumeMount(
             mount_path=volume["container_path"],
             name=get_sanitised_volume_name(
-                f"host--{volume['host_path']}",
-                length_limit=63
+                f"host--{volume['host_path']}", length_limit=63
             ),
             read_only=volume.get("mode", "RO") == "RO",
         )
         for volume in volumes
     ]
 
 
-def get_pod_volumes(volumes: PVector['DockerVolume']) -> List[V1Volume]:
+def get_kubernetes_secret_volume_mounts(
+    volumes: PVector["SecretVolume"],
+) -> List[V1VolumeMount]:
+    """
+    Given a list of secret volume mounts, return a list corresponding to the Kubernetes objects
+    representing these mounts.
+    """
+    return [
+        V1VolumeMount(
+            mount_path=volume["container_path"],
+            name=get_sanitised_volume_name(
+                f"secret--{volume['secret_name']}", length_limit=63
+            ),
+            read_only=True,
+        )
+        for volume in volumes
+    ]
+
+
+def mode_to_int(mode: Optional[str]) -> Optional[int]:
+    """
+    Convert an octal number (in string form) to a base-10 integer.
+    """
+    return int(mode, base=8) if mode else None
+
+
+def _get_items_for_secret_volume(
+    secret_volume: "SecretVolume",
+) -> Optional[List[V1KeyToPath]]:
+    """
+    Helper get all items to be stored in a secret volume and turn them into the Kubernetes
+    representation.
+    """
+    if secret_volume["items"]:
+        return [
+            V1KeyToPath(
+                key=item["key"],
+                mode=mode_to_int(item.get("mode")),
+                path=item["path"],
+            )
+            for item in secret_volume["items"]
+        ]
+
+    return None
+
+
+def get_pod_secret_volumes(secret_volumes: PVector["SecretVolume"]) -> List[V1Volume]:
+    """
+    Given a list of secret volume mounts, return a list corresponding to the Kubernetes objects
+    needed to tie the mounts to a Pod (and have Kubernetes insert the actual secret contents)
+    """
+    unique_volumes: Dict[str, "SecretVolume"] = {
+        get_sanitised_volume_name(
+            f"secret--{volume['secret_name']}", length_limit=63
+        ): volume
+        for volume in secret_volumes
+    }
+
+    return [
+        V1Volume(
+            name=name,
+            secret=V1SecretVolumeSource(
+                # we're expecting to be passed the full name here as we can't really
+                # reconstruct it without adding even more information in something like
+                # a `type` field. the format here is `paasta-secret-{service}-{secret_name}`
+                # but for boto volumes, the format is `paasta-secret-boto-keys-{secret_name}`.
+                # rather than do this, we'll just make the caller give us the actual name of
+                # the volume (which is maybe something we should have done for all the other names?)
+                secret_name=volume["secret_volume_name"],
+                default_mode=mode_to_int(volume.get("default_mode")),
+                items=_get_items_for_secret_volume(volume),
+            ),
+        )
+        for name, volume in unique_volumes.items()
+    ]
+
+
+def get_pod_volumes(volumes: PVector["DockerVolume"]) -> List[V1Volume]:
     """
     Given a list of volume mounts, return a list corresponding to the Kubernetes objects needed to
     tie the mounts to a Pod.
     """
-    unique_volumes: Dict[str, 'DockerVolume'] = {
-        get_sanitised_volume_name(f"host--{volume['host_path']}", length_limit=63): volume
+    unique_volumes: Dict[str, "DockerVolume"] = {
+        get_sanitised_volume_name(
+            f"host--{volume['host_path']}", length_limit=63
+        ): volume
         for volume in volumes
     }
 
     return [
         V1Volume(
             host_path=V1HostPathVolumeSource(path=volume["host_path"]),
             name=name,
         )
         for name, volume in unique_volumes.items()
     ]
 
 
 def get_kubernetes_empty_volume_mounts(
-    empty_volumes: PVector['EmptyVolume']
+    empty_volumes: PVector["EmptyVolume"],
 ) -> List[V1VolumeMount]:
     """
     Given a list of empty volume mounts, return a list corresponding to
     the Kubernetes objects representing these mounts.
     """
     return [
         V1VolumeMount(
             mount_path=volume["container_path"],
             name=get_sanitised_volume_name(
-                f"empty--{volume['container_path']}",
-                length_limit=63
+                f"empty--{volume['container_path']}", length_limit=63
             ),
         )
         for volume in empty_volumes
     ]
 
 
-def get_pod_empty_volumes(
-    empty_volumes: PVector['EmptyVolume']
-) -> List[V1Volume]:
+def get_pod_empty_volumes(empty_volumes: PVector["EmptyVolume"]) -> List[V1Volume]:
     """
     Given a list of empty volume mounts, return a list corresponding to
     the Kubernetes objects needed to tie the mounts to a Pod.
     """
-    unique_volumes: Dict[str, 'EmptyVolume'] = {
-        get_sanitised_volume_name(f"empty--{volume['container_path']}", length_limit=63): volume
+    unique_volumes: Dict[str, "EmptyVolume"] = {
+        get_sanitised_volume_name(
+            f"empty--{volume['container_path']}", length_limit=63
+        ): volume
         for volume in empty_volumes
     }
 
     return [
         V1Volume(
             name=name,
             empty_dir=V1EmptyDirVolumeSource(
-                medium=volume['medium'],
-                size_limit=volume['size'],
+                medium=volume["medium"],
+                size_limit=volume["size"],
             ),
         )
         for name, volume in unique_volumes.items()
     ]
 
 
 def get_node_affinity(affinities: PVector["NodeAffinity"]) -> Optional[V1NodeAffinity]:
@@ -257,10 +341,12 @@
     # package into V1NodeAffinity
     if not match_expressions:
         return None
     return V1NodeAffinity(
         # this means that the selectors are only used during scheduling.
         # changing it while the pod is running will not cause an eviction.
         required_during_scheduling_ignored_during_execution=V1NodeSelector(
-            node_selector_terms=[V1NodeSelectorTerm(match_expressions=match_expressions)],
+            node_selector_terms=[
+                V1NodeSelectorTerm(match_expressions=match_expressions)
+            ],
         ),
     )
```

### Comparing `task_processing-0.9.1/task_processing/interfaces/task_executor.py` & `task_processing-1.0.0/task_processing/interfaces/task_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from pyrsistent import field
 from pyrsistent import PRecord
 
 
 class DefaultTaskConfigInterface(PRecord):
     uuid = field(type=uuid.UUID, initial=uuid.uuid4)
-    name = field(type=str, initial='default')
+    name = field(type=str, initial="default")
 
 
 class TaskExecutor(metaclass=abc.ABCMeta):
     """The core interface for Task Processing
     This is the class you want to implement to add a new TaskExecutor
     """
 
@@ -48,16 +48,15 @@
 
         :param str task_id: The task that you want to kill
         """
         pass
 
     @abc.abstractmethod
     def stop(self):
-        """Stop the executor stack
-        """
+        """Stop the executor stack"""
         pass
 
     @abc.abstractmethod
     def get_event_queue(self):
         """Get queue of events
 
         :returns: TBD
```

### Comparing `task_processing-0.9.1/task_processing/interfaces/runner.py` & `task_processing-1.0.0/task_processing/interfaces/runner.py`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.1/task_processing/metrics.py` & `task_processing-1.0.0/task_processing/metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 try:
     import yelp_meteorite
+
     METRICS_ENABLED = True
 except Exception:
     METRICS_ENABLED = False
 
 
 class _DummyMetricType:
     """
     Emulates a yelp_meteorite counter, gauge, or timer
     """
+
     def count(*args, **kwargs):
         pass
 
     set = count
     record = count
     start = count
     stop = count
@@ -23,26 +25,24 @@
 
 
 def create_counter(name, dimensions={}):
     if not METRICS_ENABLED:
         return
 
     if name not in _registered_metrics:
-        counter = yelp_meteorite.create_counter(
-            name, default_dimensions=dimensions)
+        counter = yelp_meteorite.create_counter(name, default_dimensions=dimensions)
         _registered_metrics[name] = counter
 
 
 def create_timer(name, dimensions={}):
     if not METRICS_ENABLED:
         return
 
     if name not in _registered_metrics:
-        timer = yelp_meteorite.create_timer(
-            name, default_dimensions=dimensions)
+        timer = yelp_meteorite.create_timer(name, default_dimensions=dimensions)
         _registered_metrics[name] = timer
 
 
 def get_metric(name):
     if METRICS_ENABLED:
         return _registered_metrics.get(name)
     else:
```

### Comparing `task_processing-0.9.1/task_processing/utils.py` & `task_processing-1.0.0/task_processing/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,32 +10,33 @@
     Enums in Python require that some methods be defined pre-construction if overrides are
     desired, so if we want to create an enum that sets the value of all members to the name
     of said members, we need to create an Enum class that overrides _generate_next_value_ such
     that when EnumBase does its magic, it sees this method.
 
     Based on the snippet in https://docs.python.org/3/library/enum.html#using-automatic-values
     """
+
     @staticmethod
     def _generate_next_value_(
         name: str,
         start: int,
         count: int,
         last_values: List[Any],
     ) -> str:
         """Override auto() to set all enum values to the name of the member"""
         return name
 
 
 def get_cluster_master_by_proxy(
     proxy_prefix,
     cluster,
-    services_file='/nail/etc/services/services.yaml',
+    services_file="/nail/etc/services/services.yaml",
 ):
-    with open(services_file, 'r') as istream:
+    with open(services_file, "r") as istream:
         services = yaml.load(istream)
 
-    proxy_name = 'task_processing.' + proxy_prefix + '_' + cluster
+    proxy_name = "task_processing." + proxy_prefix + "_" + cluster
     if proxy_name not in services:
-        raise KeyError('Cluster master {} was not found'.format(proxy_name))
+        raise KeyError("Cluster master {} was not found".format(proxy_name))
     else:
         addr_info = services[proxy_name]
-        return addr_info['host'] + ':' + str(addr_info['port'])
+        return addr_info["host"] + ":" + str(addr_info["port"])
```

### Comparing `task_processing-0.9.1/LICENSE` & `task_processing-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `task_processing-0.9.1/setup.py` & `task_processing-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from pathlib import Path
+
 from setuptools import find_packages
 from setuptools import setup
 
 import task_processing
 
+# read the contents of your README file
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
-    name='task_processing',
+    name="task_processing",
     version=task_processing.__version__,
-    provides=['task_processing'],
-    author='Task Processing',
-    author_email='team-taskproc@yelp.com',
-    description='Framework for task processing executors and configuration',
-    packages=find_packages(exclude=('tests*', "examples*")),
-    package_data={
-        "task_processing": ["py.typed"]
-    },
+    provides=["task_processing"],
+    author="Task Processing",
+    author_email="team-taskproc@yelp.com",
+    description="Framework for task processing executors and configuration",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    packages=find_packages(exclude=("tests*", "examples*")),
+    package_data={"task_processing": ["py.typed"]},
     install_requires=[
         # used for immutable data structures
-        'pyrsistent',
-        # until we can drop py36, used for things like TypedDicts
-        'typing-extensions',
+        "pyrsistent",
     ],
     extras_require={
-        # We can add the Mesos specific dependencies here
-        'mesos_executor': ['addict', 'pymesos>=0.2.14', 'requests'],
-        'metrics': ['yelp-meteorite'],
-        'persistence': ['boto3'],
-        'k8s': ['kubernetes']
-    }
+        "metrics": ["yelp-meteorite"],
+        "persistence": ["boto3"],
+        "k8s": ["kubernetes", "typing-extensions"],
+    },
 )
```

