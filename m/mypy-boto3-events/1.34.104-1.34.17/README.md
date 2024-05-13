# Comparing `tmp/mypy_boto3_events-1.34.104.tar.gz` & `tmp/mypy-boto3-events-1.34.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_events-1.34.104.tar", last modified: Mon May 13 19:18:07 2024, max compression
+gzip compressed data, was "mypy-boto3-events-1.34.17.tar", last modified: Thu Jan 11 20:25:52 2024, max compression
```

## Comparing `mypy_boto3_events-1.34.104.tar` & `mypy-boto3-events-1.34.17.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.224496 mypy_boto3_events-1.34.104/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-13 19:18:07.224496 mypy_boto3_events-1.34.104/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11466 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.220497 mypy_boto3_events-1.34.104/mypy_boto3_events/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38697 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38694 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    62279 2024-05-13 19:17:53.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    62279 2024-05-13 19:17:53.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/mypy_boto3_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:18:07.224496 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 19:18:07.000000 mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:18:07.224496 mypy_boto3_events-1.34.104/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-13 19:17:52.000000 mypy_boto3_events-1.34.104/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:52.512401 mypy-boto3-events-1.34.17/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-01-11 20:25:52.512401 mypy-boto3-events-1.34.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:52.512401 mypy-boto3-events-1.34.17/mypy_boto3_events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37858 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37855 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-01-11 20:25:24.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51558 2024-01-11 20:25:25.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51558 2024-01-11 20:25:24.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/mypy_boto3_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 20:25:52.512401 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13021 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-11 20:25:52.000000 mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 20:25:52.512401 mypy-boto3-events-1.34.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-11 20:25:23.000000 mypy-boto3-events-1.34.17/setup.py
```

### Comparing `mypy_boto3_events-1.34.104/LICENSE` & `mypy-boto3-events-1.34.17/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/PKG-INFO` & `mypy-boto3-events-1.34.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.34.104
-Summary: Type annotations for boto3.EventBridge 1.34.104 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.17
+Summary: Type annotations for boto3.EventBridge 1.34.17 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_events-1.34.104/README.md` & `mypy-boto3-events-1.34.17/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/__init__.py` & `mypy-boto3-events-1.34.17/mypy_boto3_events/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/__init__.pyi` & `mypy-boto3-events-1.34.17/mypy_boto3_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/client.py` & `mypy-boto3-events-1.34.17/mypy_boto3_events/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     CreateApiDestinationResponseTypeDef,
     CreateArchiveResponseTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     CreateConnectionResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceResponseTypeDef,
-    DeadLetterConfigTypeDef,
     DeauthorizeConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DescribeApiDestinationResponseTypeDef,
     DescribeArchiveResponseTypeDef,
     DescribeConnectionResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     DescribeEventBusResponseTypeDef,
@@ -72,28 +71,27 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationUnionTypeDef,
+    ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TestEventPatternResponseTypeDef,
     TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
-    UpdateEventBusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -236,22 +234,15 @@
         Creates a global endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#create_endpoint)
         """
 
     def create_event_bus(
-        self,
-        *,
-        Name: str,
-        EventSourceName: str = ...,
-        Description: str = ...,
-        KmsKeyIdentifier: str = ...,
-        DeadLetterConfig: DeadLetterConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...,
+        self, *, Name: str, EventSourceName: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEventBusResponseTypeDef:
         """
         Creates a new event bus within your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_event_bus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#create_event_bus)
         """
@@ -677,15 +668,15 @@
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
 
     def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if
         they are already associated with the
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
@@ -717,15 +708,15 @@
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
-        Destination: ReplayDestinationUnionTypeDef,
+        Destination: ReplayDestinationTypeDef,
         Description: str = ...,
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
@@ -818,29 +809,14 @@
         """
         Update an existing endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#update_endpoint)
         """
 
-    def update_event_bus(
-        self,
-        *,
-        Name: str = ...,
-        KmsKeyIdentifier: str = ...,
-        Description: str = ...,
-        DeadLetterConfig: DeadLetterConfigTypeDef = ...,
-    ) -> UpdateEventBusResponseTypeDef:
-        """
-        Updates the specified event bus.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_event_bus)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#update_event_bus)
-        """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rule_names_by_target"]
     ) -> ListRuleNamesByTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#get_paginator)
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/client.pyi` & `mypy-boto3-events-1.34.17/mypy_boto3_events/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     CreateApiDestinationResponseTypeDef,
     CreateArchiveResponseTypeDef,
     CreateConnectionAuthRequestParametersTypeDef,
     CreateConnectionResponseTypeDef,
     CreateEndpointResponseTypeDef,
     CreateEventBusResponseTypeDef,
     CreatePartnerEventSourceResponseTypeDef,
-    DeadLetterConfigTypeDef,
     DeauthorizeConnectionResponseTypeDef,
     DeleteConnectionResponseTypeDef,
     DescribeApiDestinationResponseTypeDef,
     DescribeArchiveResponseTypeDef,
     DescribeConnectionResponseTypeDef,
     DescribeEndpointResponseTypeDef,
     DescribeEventBusResponseTypeDef,
@@ -72,28 +71,27 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationUnionTypeDef,
+    ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TestEventPatternResponseTypeDef,
     TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
-    UpdateEventBusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -233,22 +231,15 @@
         Creates a global endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#create_endpoint)
         """
 
     def create_event_bus(
-        self,
-        *,
-        Name: str,
-        EventSourceName: str = ...,
-        Description: str = ...,
-        KmsKeyIdentifier: str = ...,
-        DeadLetterConfig: DeadLetterConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...,
+        self, *, Name: str, EventSourceName: str = ..., Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEventBusResponseTypeDef:
         """
         Creates a new event bus within your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_event_bus)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#create_event_bus)
         """
@@ -674,15 +665,15 @@
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#put_rule)
         """
 
     def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if
         they are already associated with the
         rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
@@ -714,15 +705,15 @@
     def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
-        Destination: ReplayDestinationUnionTypeDef,
+        Destination: ReplayDestinationTypeDef,
         Description: str = ...,
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#start_replay)
@@ -815,29 +806,14 @@
         """
         Update an existing endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_endpoint)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#update_endpoint)
         """
 
-    def update_event_bus(
-        self,
-        *,
-        Name: str = ...,
-        KmsKeyIdentifier: str = ...,
-        Description: str = ...,
-        DeadLetterConfig: DeadLetterConfigTypeDef = ...,
-    ) -> UpdateEventBusResponseTypeDef:
-        """
-        Updates the specified event bus.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_event_bus)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#update_event_bus)
-        """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_rule_names_by_target"]
     ) -> ListRuleNamesByTargetPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/client/#get_paginator)
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/literals.py` & `mypy-boto3-events-1.34.17/mypy_boto3_events/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -113,15 +112,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -139,15 +137,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -160,26 +157,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -240,14 +235,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -376,15 +372,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -422,21 +417,19 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
-    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/literals.pyi` & `mypy-boto3-events-1.34.17/mypy_boto3_events/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -113,15 +112,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -139,15 +137,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -160,26 +157,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -240,14 +235,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -376,15 +372,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -422,21 +417,19 @@
     "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
-    "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/paginator.py` & `mypy-boto3-events-1.34.17/mypy_boto3_events/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/paginator.pyi` & `mypy-boto3-events-1.34.17/mypy_boto3_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/type_defs.py` & `mypy-boto3-events-1.34.17/mypy_boto3_events/type_defs.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -48,16 +48,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "AppSyncParametersTypeDef",
     "ArchiveTypeDef",
-    "AwsVpcConfigurationExtraOutputTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
@@ -71,18 +69,18 @@
     "CreateApiDestinationRequestRequestTypeDef",
     "CreateArchiveRequestRequestTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
-    "DeadLetterConfigTypeDef",
     "TagTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
+    "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
@@ -91,29 +89,25 @@
     "DescribeArchiveRequestRequestTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationOutputTypeDef",
+    "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
-    "HttpParametersExtraOutputTypeDef",
-    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
-    "InputTransformerExtraOutputTypeDef",
-    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
@@ -130,68 +124,58 @@
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
     "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
-    "RedshiftDataParametersExtraOutputTypeDef",
-    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
-    "ReplayDestinationTypeDef",
     "RetryPolicyTypeDef",
-    "RunCommandTargetExtraOutputTypeDef",
-    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationExtraOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchParametersTypeDef",
     "CancelReplayResponseTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionResponseTypeDef",
+    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceResponseTypeDef",
     "DeauthorizeConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveResponseTypeDef",
+    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceResponseTypeDef",
     "DescribeRuleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
     "ListRuleNamesByTargetResponseTypeDef",
     "PutRuleResponseTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternResponseTypeDef",
     "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
-    "CreateEventBusResponseTypeDef",
-    "DescribeEventBusResponseTypeDef",
-    "UpdateEventBusRequestRequestTypeDef",
-    "UpdateEventBusResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
@@ -201,54 +185,44 @@
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
+    "StartReplayRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
-    "ReplayDestinationUnionTypeDef",
-    "StartReplayRequestRequestTypeDef",
-    "RunCommandParametersExtraOutputTypeDef",
-    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
-    "SageMakerPipelineParametersExtraOutputTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
-    "EcsParametersExtraOutputTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
-    "TargetExtraOutputTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "TargetUnionTypeDef",
+    "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -282,35 +256,19 @@
         "StateReason": NotRequired[str],
         "RetentionDays": NotRequired[int],
         "SizeBytes": NotRequired[int],
         "EventCount": NotRequired[int],
         "CreationTime": NotRequired[datetime],
     },
 )
-AwsVpcConfigurationExtraOutputTypeDef = TypedDict(
-    "AwsVpcConfigurationExtraOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "SecurityGroups": NotRequired[List[str]],
-        "AssignPublicIp": NotRequired[AssignPublicIpType],
-    },
-)
-AwsVpcConfigurationOutputTypeDef = TypedDict(
-    "AwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "SecurityGroups": NotRequired[List[str]],
-        "AssignPublicIp": NotRequired[AssignPublicIpType],
-    },
-)
 AwsVpcConfigurationTypeDef = TypedDict(
     "AwsVpcConfigurationTypeDef",
     {
-        "Subnets": Sequence[str],
-        "SecurityGroups": NotRequired[Sequence[str]],
+        "Subnets": List[str],
+        "SecurityGroups": NotRequired[List[str]],
         "AssignPublicIp": NotRequired[AssignPublicIpType],
     },
 )
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": NotRequired[int],
@@ -328,18 +286,18 @@
         "ReplayName": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 CapacityProviderStrategyItemTypeDef = TypedDict(
     "CapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
         "weight": NotRequired[int],
@@ -459,20 +417,14 @@
 )
 ReplicationConfigTypeDef = TypedDict(
     "ReplicationConfigTypeDef",
     {
         "State": NotRequired[ReplicationStateType],
     },
 )
-DeadLetterConfigTypeDef = TypedDict(
-    "DeadLetterConfigTypeDef",
-    {
-        "Arn": NotRequired[str],
-    },
-)
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -485,14 +437,20 @@
 )
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
+DeadLetterConfigTypeDef = TypedDict(
+    "DeadLetterConfigTypeDef",
+    {
+        "Arn": NotRequired[str],
+    },
+)
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
@@ -585,16 +543,16 @@
 )
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
-ReplayDestinationOutputTypeDef = TypedDict(
-    "ReplayDestinationOutputTypeDef",
+ReplayDestinationTypeDef = TypedDict(
+    "ReplayDestinationTypeDef",
     {
         "Arn": str,
         "FilterArns": NotRequired[List[str]],
     },
 )
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
@@ -632,18 +590,15 @@
     },
 )
 EventBusTypeDef = TypedDict(
     "EventBusTypeDef",
     {
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
-        "Description": NotRequired[str],
         "Policy": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
     },
 )
 EventSourceTypeDef = TypedDict(
     "EventSourceTypeDef",
     {
         "Arn": NotRequired[str],
         "CreatedBy": NotRequired[str],
@@ -661,57 +616,27 @@
 )
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
-HttpParametersExtraOutputTypeDef = TypedDict(
-    "HttpParametersExtraOutputTypeDef",
-    {
-        "PathParameterValues": NotRequired[List[str]],
-        "HeaderParameters": NotRequired[Dict[str, str]],
-        "QueryStringParameters": NotRequired[Dict[str, str]],
-    },
-)
-HttpParametersOutputTypeDef = TypedDict(
-    "HttpParametersOutputTypeDef",
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
     {
         "PathParameterValues": NotRequired[List[str]],
         "HeaderParameters": NotRequired[Dict[str, str]],
         "QueryStringParameters": NotRequired[Dict[str, str]],
     },
 )
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
-    {
-        "PathParameterValues": NotRequired[Sequence[str]],
-        "HeaderParameters": NotRequired[Mapping[str, str]],
-        "QueryStringParameters": NotRequired[Mapping[str, str]],
-    },
-)
-InputTransformerExtraOutputTypeDef = TypedDict(
-    "InputTransformerExtraOutputTypeDef",
-    {
-        "InputTemplate": str,
-        "InputPathsMap": NotRequired[Dict[str, str]],
-    },
-)
-InputTransformerOutputTypeDef = TypedDict(
-    "InputTransformerOutputTypeDef",
-    {
-        "InputTemplate": str,
-        "InputPathsMap": NotRequired[Dict[str, str]],
-    },
-)
 InputTransformerTypeDef = TypedDict(
     "InputTransformerTypeDef",
     {
         "InputTemplate": str,
-        "InputPathsMap": NotRequired[Mapping[str, str]],
+        "InputPathsMap": NotRequired[Dict[str, str]],
     },
 )
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
@@ -901,48 +826,24 @@
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": NotRequired[str],
         "ErrorCode": NotRequired[str],
         "ErrorMessage": NotRequired[str],
     },
 )
-RedshiftDataParametersExtraOutputTypeDef = TypedDict(
-    "RedshiftDataParametersExtraOutputTypeDef",
-    {
-        "Database": str,
-        "SecretManagerArn": NotRequired[str],
-        "DbUser": NotRequired[str],
-        "Sql": NotRequired[str],
-        "StatementName": NotRequired[str],
-        "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[List[str]],
-    },
-)
-RedshiftDataParametersOutputTypeDef = TypedDict(
-    "RedshiftDataParametersOutputTypeDef",
-    {
-        "Database": str,
-        "SecretManagerArn": NotRequired[str],
-        "DbUser": NotRequired[str],
-        "Sql": NotRequired[str],
-        "StatementName": NotRequired[str],
-        "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[List[str]],
-    },
-)
 RedshiftDataParametersTypeDef = TypedDict(
     "RedshiftDataParametersTypeDef",
     {
         "Database": str,
         "SecretManagerArn": NotRequired[str],
         "DbUser": NotRequired[str],
         "Sql": NotRequired[str],
         "StatementName": NotRequired[str],
         "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[Sequence[str]],
+        "Sqls": NotRequired[List[str]],
     },
 )
 RemovePermissionRequestRequestTypeDef = TypedDict(
     "RemovePermissionRequestRequestTypeDef",
     {
         "StatementId": NotRequired[str],
         "RemoveAllPermissions": NotRequired[bool],
@@ -962,47 +863,26 @@
     "RemoveTargetsResultEntryTypeDef",
     {
         "TargetId": NotRequired[str],
         "ErrorCode": NotRequired[str],
         "ErrorMessage": NotRequired[str],
     },
 )
-ReplayDestinationTypeDef = TypedDict(
-    "ReplayDestinationTypeDef",
-    {
-        "Arn": str,
-        "FilterArns": NotRequired[Sequence[str]],
-    },
-)
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": NotRequired[int],
         "MaximumEventAgeInSeconds": NotRequired[int],
     },
 )
-RunCommandTargetExtraOutputTypeDef = TypedDict(
-    "RunCommandTargetExtraOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
-RunCommandTargetOutputTypeDef = TypedDict(
-    "RunCommandTargetOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -1065,26 +945,14 @@
 UpdateConnectionOAuthClientRequestParametersTypeDef = TypedDict(
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": NotRequired[str],
         "ClientSecret": NotRequired[str],
     },
 )
-NetworkConfigurationExtraOutputTypeDef = TypedDict(
-    "NetworkConfigurationExtraOutputTypeDef",
-    {
-        "awsvpcConfiguration": NotRequired[AwsVpcConfigurationExtraOutputTypeDef],
-    },
-)
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": NotRequired[AwsVpcConfigurationOutputTypeDef],
-    },
-)
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": NotRequired[AwsVpcConfigurationTypeDef],
     },
 )
 BatchParametersTypeDef = TypedDict(
@@ -1131,14 +999,21 @@
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreatePartnerEventSourceResponseTypeDef = TypedDict(
     "CreatePartnerEventSourceResponseTypeDef",
     {
         "EventSourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1193,14 +1068,23 @@
         "RetentionDays": int,
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeEventSourceResponseTypeDef = TypedDict(
     "DescribeEventSourceResponseTypeDef",
     {
         "Arn": str,
         "CreatedBy": str,
         "CreationTime": datetime,
         "ExpirationTime": datetime,
@@ -1239,32 +1123,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListRuleNamesByTargetResponseTypeDef = TypedDict(
     "ListRuleNamesByTargetResponseTypeDef",
     {
         "RuleNames": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PutRuleResponseTypeDef = TypedDict(
     "PutRuleResponseTypeDef",
     {
         "RuleArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1325,90 +1209,35 @@
         "Action": NotRequired[str],
         "Principal": NotRequired[str],
         "StatementId": NotRequired[str],
         "Condition": NotRequired[ConditionTypeDef],
         "Policy": NotRequired[str],
     },
 )
-ConnectionHttpParametersOutputTypeDef = TypedDict(
-    "ConnectionHttpParametersOutputTypeDef",
-    {
-        "HeaderParameters": NotRequired[List[ConnectionHeaderParameterTypeDef]],
-        "QueryStringParameters": NotRequired[List[ConnectionQueryStringParameterTypeDef]],
-        "BodyParameters": NotRequired[List[ConnectionBodyParameterTypeDef]],
-    },
-)
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": NotRequired[Sequence[ConnectionHeaderParameterTypeDef]],
         "QueryStringParameters": NotRequired[Sequence[ConnectionQueryStringParameterTypeDef]],
         "BodyParameters": NotRequired[Sequence[ConnectionBodyParameterTypeDef]],
     },
 )
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
-    },
-)
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "Description": str,
-        "KmsKeyIdentifier": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "KmsKeyIdentifier": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "Policy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateEventBusRequestRequestTypeDef = TypedDict(
-    "UpdateEventBusRequestRequestTypeDef",
-    {
-        "Name": NotRequired[str],
-        "KmsKeyIdentifier": NotRequired[str],
-        "Description": NotRequired[str],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-    },
-)
-UpdateEventBusResponseTypeDef = TypedDict(
-    "UpdateEventBusResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "KmsKeyIdentifier": str,
-        "Description": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateEventBusRequestRequestTypeDef = TypedDict(
     "CreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
         "EventSourceName": NotRequired[str],
-        "Description": NotRequired[str],
-        "KmsKeyIdentifier": NotRequired[str],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
@@ -1440,68 +1269,68 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationOutputTypeDef,
+        "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
         "Secondary": SecondaryTypeDef,
     },
 )
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     {
         "TargetArn": str,
         "EventBusName": NotRequired[str],
@@ -1524,16 +1353,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": NotRequired[TimestampTypeDef],
         "Source": NotRequired[str],
@@ -1550,14 +1379,25 @@
         "Time": NotRequired[TimestampTypeDef],
         "Source": NotRequired[str],
         "Resources": NotRequired[Sequence[str]],
         "DetailType": NotRequired[str],
         "Detail": NotRequired[str],
     },
 )
+StartReplayRequestRequestTypeDef = TypedDict(
+    "StartReplayRequestRequestTypeDef",
+    {
+        "ReplayName": str,
+        "EventSourceArn": str,
+        "EventStartTime": TimestampTypeDef,
+        "EventEndTime": TimestampTypeDef,
+        "Destination": ReplayDestinationTypeDef,
+        "Description": NotRequired[str],
+    },
+)
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1582,126 +1422,52 @@
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
-StartReplayRequestRequestTypeDef = TypedDict(
-    "StartReplayRequestRequestTypeDef",
-    {
-        "ReplayName": str,
-        "EventSourceArn": str,
-        "EventStartTime": TimestampTypeDef,
-        "EventEndTime": TimestampTypeDef,
-        "Destination": ReplayDestinationTypeDef,
-        "Description": NotRequired[str],
-    },
-)
-RunCommandParametersExtraOutputTypeDef = TypedDict(
-    "RunCommandParametersExtraOutputTypeDef",
-    {
-        "RunCommandTargets": List[RunCommandTargetExtraOutputTypeDef],
-    },
-)
-RunCommandParametersOutputTypeDef = TypedDict(
-    "RunCommandParametersOutputTypeDef",
-    {
-        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
-    },
-)
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
-        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
-    },
-)
-SageMakerPipelineParametersExtraOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersExtraOutputTypeDef",
-    {
-        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
-    },
-)
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
-    {
-        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
+        "RunCommandTargets": List[RunCommandTargetTypeDef],
     },
 )
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
-        "PipelineParameterList": NotRequired[Sequence[SageMakerPipelineParameterTypeDef]],
-    },
-)
-EcsParametersExtraOutputTypeDef = TypedDict(
-    "EcsParametersExtraOutputTypeDef",
-    {
-        "TaskDefinitionArn": str,
-        "TaskCount": NotRequired[int],
-        "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationExtraOutputTypeDef],
-        "PlatformVersion": NotRequired[str],
-        "Group": NotRequired[str],
-        "CapacityProviderStrategy": NotRequired[List[CapacityProviderStrategyItemTypeDef]],
-        "EnableECSManagedTags": NotRequired[bool],
-        "EnableExecuteCommand": NotRequired[bool],
-        "PlacementConstraints": NotRequired[List[PlacementConstraintTypeDef]],
-        "PlacementStrategy": NotRequired[List[PlacementStrategyTypeDef]],
-        "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
-        "ReferenceId": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
     },
 )
-EcsParametersOutputTypeDef = TypedDict(
-    "EcsParametersOutputTypeDef",
+EcsParametersTypeDef = TypedDict(
+    "EcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
         "TaskCount": NotRequired[int],
         "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationOutputTypeDef],
+        "NetworkConfiguration": NotRequired[NetworkConfigurationTypeDef],
         "PlatformVersion": NotRequired[str],
         "Group": NotRequired[str],
         "CapacityProviderStrategy": NotRequired[List[CapacityProviderStrategyItemTypeDef]],
         "EnableECSManagedTags": NotRequired[bool],
         "EnableExecuteCommand": NotRequired[bool],
         "PlacementConstraints": NotRequired[List[PlacementConstraintTypeDef]],
         "PlacementStrategy": NotRequired[List[PlacementStrategyTypeDef]],
         "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
         "ReferenceId": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-EcsParametersTypeDef = TypedDict(
-    "EcsParametersTypeDef",
-    {
-        "TaskDefinitionArn": str,
-        "TaskCount": NotRequired[int],
-        "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationTypeDef],
-        "PlatformVersion": NotRequired[str],
-        "Group": NotRequired[str],
-        "CapacityProviderStrategy": NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],
-        "EnableECSManagedTags": NotRequired[bool],
-        "EnableExecuteCommand": NotRequired[bool],
-        "PlacementConstraints": NotRequired[Sequence[PlacementConstraintTypeDef]],
-        "PlacementStrategy": NotRequired[Sequence[PlacementStrategyTypeDef]],
-        "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
-        "ReferenceId": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": NotRequired[ConnectionOAuthClientResponseParametersTypeDef],
         "AuthorizationEndpoint": NotRequired[str],
         "HttpMethod": NotRequired[ConnectionOAuthHttpMethodType],
-        "OAuthHttpParameters": NotRequired[ConnectionHttpParametersOutputTypeDef],
+        "OAuthHttpParameters": NotRequired[ConnectionHttpParametersTypeDef],
     },
 )
 CreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionOAuthRequestParametersTypeDef",
     {
         "ClientParameters": CreateConnectionOAuthClientRequestParametersTypeDef,
         "AuthorizationEndpoint": str,
@@ -1733,58 +1499,14 @@
 )
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
     },
 )
-TargetExtraOutputTypeDef = TypedDict(
-    "TargetExtraOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "RoleArn": NotRequired[str],
-        "Input": NotRequired[str],
-        "InputPath": NotRequired[str],
-        "InputTransformer": NotRequired[InputTransformerExtraOutputTypeDef],
-        "KinesisParameters": NotRequired[KinesisParametersTypeDef],
-        "RunCommandParameters": NotRequired[RunCommandParametersExtraOutputTypeDef],
-        "EcsParameters": NotRequired[EcsParametersExtraOutputTypeDef],
-        "BatchParameters": NotRequired[BatchParametersTypeDef],
-        "SqsParameters": NotRequired[SqsParametersTypeDef],
-        "HttpParameters": NotRequired[HttpParametersExtraOutputTypeDef],
-        "RedshiftDataParameters": NotRequired[RedshiftDataParametersExtraOutputTypeDef],
-        "SageMakerPipelineParameters": NotRequired[SageMakerPipelineParametersExtraOutputTypeDef],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-        "RetryPolicy": NotRequired[RetryPolicyTypeDef],
-        "AppSyncParameters": NotRequired[AppSyncParametersTypeDef],
-    },
-)
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "RoleArn": NotRequired[str],
-        "Input": NotRequired[str],
-        "InputPath": NotRequired[str],
-        "InputTransformer": NotRequired[InputTransformerOutputTypeDef],
-        "KinesisParameters": NotRequired[KinesisParametersTypeDef],
-        "RunCommandParameters": NotRequired[RunCommandParametersOutputTypeDef],
-        "EcsParameters": NotRequired[EcsParametersOutputTypeDef],
-        "BatchParameters": NotRequired[BatchParametersTypeDef],
-        "SqsParameters": NotRequired[SqsParametersTypeDef],
-        "HttpParameters": NotRequired[HttpParametersOutputTypeDef],
-        "RedshiftDataParameters": NotRequired[RedshiftDataParametersOutputTypeDef],
-        "SageMakerPipelineParameters": NotRequired[SageMakerPipelineParametersOutputTypeDef],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-        "RetryPolicy": NotRequired[RetryPolicyTypeDef],
-        "AppSyncParameters": NotRequired[AppSyncParametersTypeDef],
-    },
-)
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "Id": str,
         "Arn": str,
         "RoleArn": NotRequired[str],
         "Input": NotRequired[str],
@@ -1805,15 +1527,15 @@
 )
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": NotRequired[ConnectionBasicAuthResponseParametersTypeDef],
         "OAuthParameters": NotRequired[ConnectionOAuthResponseParametersTypeDef],
         "ApiKeyAuthParameters": NotRequired[ConnectionApiKeyAuthResponseParametersTypeDef],
-        "InvocationHttpParameters": NotRequired[ConnectionHttpParametersOutputTypeDef],
+        "InvocationHttpParameters": NotRequired[ConnectionHttpParametersTypeDef],
     },
 )
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
         "BasicAuthParameters": NotRequired[CreateConnectionBasicAuthRequestParametersTypeDef],
         "OAuthParameters": NotRequired[CreateConnectionOAuthRequestParametersTypeDef],
@@ -1916,20 +1638,27 @@
         "State": EndpointStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
-TargetUnionTypeDef = Union[TargetTypeDef, TargetExtraOutputTypeDef]
+PutTargetsRequestRequestTypeDef = TypedDict(
+    "PutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetTypeDef],
+        "EventBusName": NotRequired[str],
+    },
+)
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -1961,19 +1690,11 @@
         "AuthParameters": NotRequired[UpdateConnectionAuthRequestParametersTypeDef],
     },
 )
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
-    },
-)
-PutTargetsRequestRequestTypeDef = TypedDict(
-    "PutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "EventBusName": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events/type_defs.pyi` & `mypy-boto3-events-1.34.17/mypy_boto3_events/type_defs.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -48,16 +48,14 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "AppSyncParametersTypeDef",
     "ArchiveTypeDef",
-    "AwsVpcConfigurationExtraOutputTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
@@ -71,18 +69,18 @@
     "CreateApiDestinationRequestRequestTypeDef",
     "CreateArchiveRequestRequestTypeDef",
     "CreateConnectionApiKeyAuthRequestParametersTypeDef",
     "CreateConnectionBasicAuthRequestParametersTypeDef",
     "CreateConnectionOAuthClientRequestParametersTypeDef",
     "EndpointEventBusTypeDef",
     "ReplicationConfigTypeDef",
-    "DeadLetterConfigTypeDef",
     "TagTypeDef",
     "CreatePartnerEventSourceRequestRequestTypeDef",
     "DeactivateEventSourceRequestRequestTypeDef",
+    "DeadLetterConfigTypeDef",
     "DeauthorizeConnectionRequestRequestTypeDef",
     "DeleteApiDestinationRequestRequestTypeDef",
     "DeleteArchiveRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteEndpointRequestRequestTypeDef",
     "DeleteEventBusRequestRequestTypeDef",
     "DeletePartnerEventSourceRequestRequestTypeDef",
@@ -91,29 +89,25 @@
     "DescribeArchiveRequestRequestTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationOutputTypeDef",
+    "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
-    "HttpParametersExtraOutputTypeDef",
-    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
-    "InputTransformerExtraOutputTypeDef",
-    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
@@ -130,68 +124,58 @@
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
     "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
-    "RedshiftDataParametersExtraOutputTypeDef",
-    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
-    "ReplayDestinationTypeDef",
     "RetryPolicyTypeDef",
-    "RunCommandTargetExtraOutputTypeDef",
-    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationExtraOutputTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchParametersTypeDef",
     "CancelReplayResponseTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionResponseTypeDef",
+    "CreateEventBusResponseTypeDef",
     "CreatePartnerEventSourceResponseTypeDef",
     "DeauthorizeConnectionResponseTypeDef",
     "DeleteConnectionResponseTypeDef",
     "DescribeApiDestinationResponseTypeDef",
     "DescribeArchiveResponseTypeDef",
+    "DescribeEventBusResponseTypeDef",
     "DescribeEventSourceResponseTypeDef",
     "DescribePartnerEventSourceResponseTypeDef",
     "DescribeRuleResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListApiDestinationsResponseTypeDef",
     "ListArchivesResponseTypeDef",
     "ListRuleNamesByTargetResponseTypeDef",
     "PutRuleResponseTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternResponseTypeDef",
     "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
-    "CreateEventBusResponseTypeDef",
-    "DescribeEventBusResponseTypeDef",
-    "UpdateEventBusRequestRequestTypeDef",
-    "UpdateEventBusResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
     "ListEventBusesResponseTypeDef",
     "ListEventSourcesResponseTypeDef",
@@ -201,54 +185,44 @@
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
+    "StartReplayRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
-    "ReplayDestinationUnionTypeDef",
-    "StartReplayRequestRequestTypeDef",
-    "RunCommandParametersExtraOutputTypeDef",
-    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
-    "SageMakerPipelineParametersExtraOutputTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
-    "EcsParametersExtraOutputTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
-    "TargetExtraOutputTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "TargetUnionTypeDef",
+    "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -282,35 +256,19 @@
         "StateReason": NotRequired[str],
         "RetentionDays": NotRequired[int],
         "SizeBytes": NotRequired[int],
         "EventCount": NotRequired[int],
         "CreationTime": NotRequired[datetime],
     },
 )
-AwsVpcConfigurationExtraOutputTypeDef = TypedDict(
-    "AwsVpcConfigurationExtraOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "SecurityGroups": NotRequired[List[str]],
-        "AssignPublicIp": NotRequired[AssignPublicIpType],
-    },
-)
-AwsVpcConfigurationOutputTypeDef = TypedDict(
-    "AwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-        "SecurityGroups": NotRequired[List[str]],
-        "AssignPublicIp": NotRequired[AssignPublicIpType],
-    },
-)
 AwsVpcConfigurationTypeDef = TypedDict(
     "AwsVpcConfigurationTypeDef",
     {
-        "Subnets": Sequence[str],
-        "SecurityGroups": NotRequired[Sequence[str]],
+        "Subnets": List[str],
+        "SecurityGroups": NotRequired[List[str]],
         "AssignPublicIp": NotRequired[AssignPublicIpType],
     },
 )
 BatchArrayPropertiesTypeDef = TypedDict(
     "BatchArrayPropertiesTypeDef",
     {
         "Size": NotRequired[int],
@@ -328,18 +286,18 @@
         "ReplayName": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 CapacityProviderStrategyItemTypeDef = TypedDict(
     "CapacityProviderStrategyItemTypeDef",
     {
         "capacityProvider": str,
         "weight": NotRequired[int],
@@ -459,20 +417,14 @@
 )
 ReplicationConfigTypeDef = TypedDict(
     "ReplicationConfigTypeDef",
     {
         "State": NotRequired[ReplicationStateType],
     },
 )
-DeadLetterConfigTypeDef = TypedDict(
-    "DeadLetterConfigTypeDef",
-    {
-        "Arn": NotRequired[str],
-    },
-)
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -485,14 +437,20 @@
 )
 DeactivateEventSourceRequestRequestTypeDef = TypedDict(
     "DeactivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
+DeadLetterConfigTypeDef = TypedDict(
+    "DeadLetterConfigTypeDef",
+    {
+        "Arn": NotRequired[str],
+    },
+)
 DeauthorizeConnectionRequestRequestTypeDef = TypedDict(
     "DeauthorizeConnectionRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 DeleteApiDestinationRequestRequestTypeDef = TypedDict(
@@ -585,16 +543,16 @@
 )
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
-ReplayDestinationOutputTypeDef = TypedDict(
-    "ReplayDestinationOutputTypeDef",
+ReplayDestinationTypeDef = TypedDict(
+    "ReplayDestinationTypeDef",
     {
         "Arn": str,
         "FilterArns": NotRequired[List[str]],
     },
 )
 DescribeRuleRequestRequestTypeDef = TypedDict(
     "DescribeRuleRequestRequestTypeDef",
@@ -632,18 +590,15 @@
     },
 )
 EventBusTypeDef = TypedDict(
     "EventBusTypeDef",
     {
         "Name": NotRequired[str],
         "Arn": NotRequired[str],
-        "Description": NotRequired[str],
         "Policy": NotRequired[str],
-        "CreationTime": NotRequired[datetime],
-        "LastModifiedTime": NotRequired[datetime],
     },
 )
 EventSourceTypeDef = TypedDict(
     "EventSourceTypeDef",
     {
         "Arn": NotRequired[str],
         "CreatedBy": NotRequired[str],
@@ -661,57 +616,27 @@
 )
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
-HttpParametersExtraOutputTypeDef = TypedDict(
-    "HttpParametersExtraOutputTypeDef",
-    {
-        "PathParameterValues": NotRequired[List[str]],
-        "HeaderParameters": NotRequired[Dict[str, str]],
-        "QueryStringParameters": NotRequired[Dict[str, str]],
-    },
-)
-HttpParametersOutputTypeDef = TypedDict(
-    "HttpParametersOutputTypeDef",
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
     {
         "PathParameterValues": NotRequired[List[str]],
         "HeaderParameters": NotRequired[Dict[str, str]],
         "QueryStringParameters": NotRequired[Dict[str, str]],
     },
 )
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
-    {
-        "PathParameterValues": NotRequired[Sequence[str]],
-        "HeaderParameters": NotRequired[Mapping[str, str]],
-        "QueryStringParameters": NotRequired[Mapping[str, str]],
-    },
-)
-InputTransformerExtraOutputTypeDef = TypedDict(
-    "InputTransformerExtraOutputTypeDef",
-    {
-        "InputTemplate": str,
-        "InputPathsMap": NotRequired[Dict[str, str]],
-    },
-)
-InputTransformerOutputTypeDef = TypedDict(
-    "InputTransformerOutputTypeDef",
-    {
-        "InputTemplate": str,
-        "InputPathsMap": NotRequired[Dict[str, str]],
-    },
-)
 InputTransformerTypeDef = TypedDict(
     "InputTransformerTypeDef",
     {
         "InputTemplate": str,
-        "InputPathsMap": NotRequired[Mapping[str, str]],
+        "InputPathsMap": NotRequired[Dict[str, str]],
     },
 )
 KinesisParametersTypeDef = TypedDict(
     "KinesisParametersTypeDef",
     {
         "PartitionKeyPath": str,
     },
@@ -901,48 +826,24 @@
     "PutTargetsResultEntryTypeDef",
     {
         "TargetId": NotRequired[str],
         "ErrorCode": NotRequired[str],
         "ErrorMessage": NotRequired[str],
     },
 )
-RedshiftDataParametersExtraOutputTypeDef = TypedDict(
-    "RedshiftDataParametersExtraOutputTypeDef",
-    {
-        "Database": str,
-        "SecretManagerArn": NotRequired[str],
-        "DbUser": NotRequired[str],
-        "Sql": NotRequired[str],
-        "StatementName": NotRequired[str],
-        "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[List[str]],
-    },
-)
-RedshiftDataParametersOutputTypeDef = TypedDict(
-    "RedshiftDataParametersOutputTypeDef",
-    {
-        "Database": str,
-        "SecretManagerArn": NotRequired[str],
-        "DbUser": NotRequired[str],
-        "Sql": NotRequired[str],
-        "StatementName": NotRequired[str],
-        "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[List[str]],
-    },
-)
 RedshiftDataParametersTypeDef = TypedDict(
     "RedshiftDataParametersTypeDef",
     {
         "Database": str,
         "SecretManagerArn": NotRequired[str],
         "DbUser": NotRequired[str],
         "Sql": NotRequired[str],
         "StatementName": NotRequired[str],
         "WithEvent": NotRequired[bool],
-        "Sqls": NotRequired[Sequence[str]],
+        "Sqls": NotRequired[List[str]],
     },
 )
 RemovePermissionRequestRequestTypeDef = TypedDict(
     "RemovePermissionRequestRequestTypeDef",
     {
         "StatementId": NotRequired[str],
         "RemoveAllPermissions": NotRequired[bool],
@@ -962,47 +863,26 @@
     "RemoveTargetsResultEntryTypeDef",
     {
         "TargetId": NotRequired[str],
         "ErrorCode": NotRequired[str],
         "ErrorMessage": NotRequired[str],
     },
 )
-ReplayDestinationTypeDef = TypedDict(
-    "ReplayDestinationTypeDef",
-    {
-        "Arn": str,
-        "FilterArns": NotRequired[Sequence[str]],
-    },
-)
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": NotRequired[int],
         "MaximumEventAgeInSeconds": NotRequired[int],
     },
 )
-RunCommandTargetExtraOutputTypeDef = TypedDict(
-    "RunCommandTargetExtraOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
-RunCommandTargetOutputTypeDef = TypedDict(
-    "RunCommandTargetOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
         "Value": str,
@@ -1065,26 +945,14 @@
 UpdateConnectionOAuthClientRequestParametersTypeDef = TypedDict(
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
     {
         "ClientID": NotRequired[str],
         "ClientSecret": NotRequired[str],
     },
 )
-NetworkConfigurationExtraOutputTypeDef = TypedDict(
-    "NetworkConfigurationExtraOutputTypeDef",
-    {
-        "awsvpcConfiguration": NotRequired[AwsVpcConfigurationExtraOutputTypeDef],
-    },
-)
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": NotRequired[AwsVpcConfigurationOutputTypeDef],
-    },
-)
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": NotRequired[AwsVpcConfigurationTypeDef],
     },
 )
 BatchParametersTypeDef = TypedDict(
@@ -1131,14 +999,21 @@
         "ConnectionArn": str,
         "ConnectionState": ConnectionStateType,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateEventBusResponseTypeDef = TypedDict(
+    "CreateEventBusResponseTypeDef",
+    {
+        "EventBusArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 CreatePartnerEventSourceResponseTypeDef = TypedDict(
     "CreatePartnerEventSourceResponseTypeDef",
     {
         "EventSourceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1193,14 +1068,23 @@
         "RetentionDays": int,
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeEventBusResponseTypeDef = TypedDict(
+    "DescribeEventBusResponseTypeDef",
+    {
+        "Name": str,
+        "Arn": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeEventSourceResponseTypeDef = TypedDict(
     "DescribeEventSourceResponseTypeDef",
     {
         "Arn": str,
         "CreatedBy": str,
         "CreationTime": datetime,
         "ExpirationTime": datetime,
@@ -1239,32 +1123,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApiDestinationsResponseTypeDef = TypedDict(
     "ListApiDestinationsResponseTypeDef",
     {
         "ApiDestinations": List[ApiDestinationTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListArchivesResponseTypeDef = TypedDict(
     "ListArchivesResponseTypeDef",
     {
         "Archives": List[ArchiveTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListRuleNamesByTargetResponseTypeDef = TypedDict(
     "ListRuleNamesByTargetResponseTypeDef",
     {
         "RuleNames": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PutRuleResponseTypeDef = TypedDict(
     "PutRuleResponseTypeDef",
     {
         "RuleArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1325,90 +1209,35 @@
         "Action": NotRequired[str],
         "Principal": NotRequired[str],
         "StatementId": NotRequired[str],
         "Condition": NotRequired[ConditionTypeDef],
         "Policy": NotRequired[str],
     },
 )
-ConnectionHttpParametersOutputTypeDef = TypedDict(
-    "ConnectionHttpParametersOutputTypeDef",
-    {
-        "HeaderParameters": NotRequired[List[ConnectionHeaderParameterTypeDef]],
-        "QueryStringParameters": NotRequired[List[ConnectionQueryStringParameterTypeDef]],
-        "BodyParameters": NotRequired[List[ConnectionBodyParameterTypeDef]],
-    },
-)
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": NotRequired[Sequence[ConnectionHeaderParameterTypeDef]],
         "QueryStringParameters": NotRequired[Sequence[ConnectionQueryStringParameterTypeDef]],
         "BodyParameters": NotRequired[Sequence[ConnectionBodyParameterTypeDef]],
     },
 )
 ListConnectionsResponseTypeDef = TypedDict(
     "ListConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
-    },
-)
-CreateEventBusResponseTypeDef = TypedDict(
-    "CreateEventBusResponseTypeDef",
-    {
-        "EventBusArn": str,
-        "Description": str,
-        "KmsKeyIdentifier": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeEventBusResponseTypeDef = TypedDict(
-    "DescribeEventBusResponseTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "Description": str,
-        "KmsKeyIdentifier": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "Policy": str,
-        "CreationTime": datetime,
-        "LastModifiedTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateEventBusRequestRequestTypeDef = TypedDict(
-    "UpdateEventBusRequestRequestTypeDef",
-    {
-        "Name": NotRequired[str],
-        "KmsKeyIdentifier": NotRequired[str],
-        "Description": NotRequired[str],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-    },
-)
-UpdateEventBusResponseTypeDef = TypedDict(
-    "UpdateEventBusResponseTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-        "KmsKeyIdentifier": str,
-        "Description": str,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 CreateEventBusRequestRequestTypeDef = TypedDict(
     "CreateEventBusRequestRequestTypeDef",
     {
         "Name": str,
         "EventSourceName": NotRequired[str],
-        "Description": NotRequired[str],
-        "KmsKeyIdentifier": NotRequired[str],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
@@ -1440,68 +1269,68 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationOutputTypeDef,
+        "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListEventBusesResponseTypeDef = TypedDict(
     "ListEventBusesResponseTypeDef",
     {
         "EventBuses": List[EventBusTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListEventSourcesResponseTypeDef = TypedDict(
     "ListEventSourcesResponseTypeDef",
     {
         "EventSources": List[EventSourceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 FailoverConfigTypeDef = TypedDict(
     "FailoverConfigTypeDef",
     {
         "Primary": PrimaryTypeDef,
         "Secondary": SecondaryTypeDef,
     },
 )
 ListPartnerEventSourceAccountsResponseTypeDef = TypedDict(
     "ListPartnerEventSourceAccountsResponseTypeDef",
     {
         "PartnerEventSourceAccounts": List[PartnerEventSourceAccountTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListPartnerEventSourcesResponseTypeDef = TypedDict(
     "ListPartnerEventSourcesResponseTypeDef",
     {
         "PartnerEventSources": List[PartnerEventSourceTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListReplaysResponseTypeDef = TypedDict(
     "ListReplaysResponseTypeDef",
     {
         "Replays": List[ReplayTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef = TypedDict(
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     {
         "TargetArn": str,
         "EventBusName": NotRequired[str],
@@ -1524,16 +1353,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "Rules": List[RuleTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PutEventsRequestEntryTypeDef = TypedDict(
     "PutEventsRequestEntryTypeDef",
     {
         "Time": NotRequired[TimestampTypeDef],
         "Source": NotRequired[str],
@@ -1550,14 +1379,25 @@
         "Time": NotRequired[TimestampTypeDef],
         "Source": NotRequired[str],
         "Resources": NotRequired[Sequence[str]],
         "DetailType": NotRequired[str],
         "Detail": NotRequired[str],
     },
 )
+StartReplayRequestRequestTypeDef = TypedDict(
+    "StartReplayRequestRequestTypeDef",
+    {
+        "ReplayName": str,
+        "EventSourceArn": str,
+        "EventStartTime": TimestampTypeDef,
+        "EventEndTime": TimestampTypeDef,
+        "Destination": ReplayDestinationTypeDef,
+        "Description": NotRequired[str],
+    },
+)
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1582,126 +1422,52 @@
     "RemoveTargetsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
-StartReplayRequestRequestTypeDef = TypedDict(
-    "StartReplayRequestRequestTypeDef",
-    {
-        "ReplayName": str,
-        "EventSourceArn": str,
-        "EventStartTime": TimestampTypeDef,
-        "EventEndTime": TimestampTypeDef,
-        "Destination": ReplayDestinationTypeDef,
-        "Description": NotRequired[str],
-    },
-)
-RunCommandParametersExtraOutputTypeDef = TypedDict(
-    "RunCommandParametersExtraOutputTypeDef",
-    {
-        "RunCommandTargets": List[RunCommandTargetExtraOutputTypeDef],
-    },
-)
-RunCommandParametersOutputTypeDef = TypedDict(
-    "RunCommandParametersOutputTypeDef",
-    {
-        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
-    },
-)
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
-        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
-    },
-)
-SageMakerPipelineParametersExtraOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersExtraOutputTypeDef",
-    {
-        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
-    },
-)
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
-    {
-        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
+        "RunCommandTargets": List[RunCommandTargetTypeDef],
     },
 )
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
-        "PipelineParameterList": NotRequired[Sequence[SageMakerPipelineParameterTypeDef]],
-    },
-)
-EcsParametersExtraOutputTypeDef = TypedDict(
-    "EcsParametersExtraOutputTypeDef",
-    {
-        "TaskDefinitionArn": str,
-        "TaskCount": NotRequired[int],
-        "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationExtraOutputTypeDef],
-        "PlatformVersion": NotRequired[str],
-        "Group": NotRequired[str],
-        "CapacityProviderStrategy": NotRequired[List[CapacityProviderStrategyItemTypeDef]],
-        "EnableECSManagedTags": NotRequired[bool],
-        "EnableExecuteCommand": NotRequired[bool],
-        "PlacementConstraints": NotRequired[List[PlacementConstraintTypeDef]],
-        "PlacementStrategy": NotRequired[List[PlacementStrategyTypeDef]],
-        "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
-        "ReferenceId": NotRequired[str],
-        "Tags": NotRequired[List[TagTypeDef]],
+        "PipelineParameterList": NotRequired[List[SageMakerPipelineParameterTypeDef]],
     },
 )
-EcsParametersOutputTypeDef = TypedDict(
-    "EcsParametersOutputTypeDef",
+EcsParametersTypeDef = TypedDict(
+    "EcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
         "TaskCount": NotRequired[int],
         "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationOutputTypeDef],
+        "NetworkConfiguration": NotRequired[NetworkConfigurationTypeDef],
         "PlatformVersion": NotRequired[str],
         "Group": NotRequired[str],
         "CapacityProviderStrategy": NotRequired[List[CapacityProviderStrategyItemTypeDef]],
         "EnableECSManagedTags": NotRequired[bool],
         "EnableExecuteCommand": NotRequired[bool],
         "PlacementConstraints": NotRequired[List[PlacementConstraintTypeDef]],
         "PlacementStrategy": NotRequired[List[PlacementStrategyTypeDef]],
         "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
         "ReferenceId": NotRequired[str],
         "Tags": NotRequired[List[TagTypeDef]],
     },
 )
-EcsParametersTypeDef = TypedDict(
-    "EcsParametersTypeDef",
-    {
-        "TaskDefinitionArn": str,
-        "TaskCount": NotRequired[int],
-        "LaunchType": NotRequired[LaunchTypeType],
-        "NetworkConfiguration": NotRequired[NetworkConfigurationTypeDef],
-        "PlatformVersion": NotRequired[str],
-        "Group": NotRequired[str],
-        "CapacityProviderStrategy": NotRequired[Sequence[CapacityProviderStrategyItemTypeDef]],
-        "EnableECSManagedTags": NotRequired[bool],
-        "EnableExecuteCommand": NotRequired[bool],
-        "PlacementConstraints": NotRequired[Sequence[PlacementConstraintTypeDef]],
-        "PlacementStrategy": NotRequired[Sequence[PlacementStrategyTypeDef]],
-        "PropagateTags": NotRequired[Literal["TASK_DEFINITION"]],
-        "ReferenceId": NotRequired[str],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": NotRequired[ConnectionOAuthClientResponseParametersTypeDef],
         "AuthorizationEndpoint": NotRequired[str],
         "HttpMethod": NotRequired[ConnectionOAuthHttpMethodType],
-        "OAuthHttpParameters": NotRequired[ConnectionHttpParametersOutputTypeDef],
+        "OAuthHttpParameters": NotRequired[ConnectionHttpParametersTypeDef],
     },
 )
 CreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionOAuthRequestParametersTypeDef",
     {
         "ClientParameters": CreateConnectionOAuthClientRequestParametersTypeDef,
         "AuthorizationEndpoint": str,
@@ -1733,58 +1499,14 @@
 )
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
     },
 )
-TargetExtraOutputTypeDef = TypedDict(
-    "TargetExtraOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "RoleArn": NotRequired[str],
-        "Input": NotRequired[str],
-        "InputPath": NotRequired[str],
-        "InputTransformer": NotRequired[InputTransformerExtraOutputTypeDef],
-        "KinesisParameters": NotRequired[KinesisParametersTypeDef],
-        "RunCommandParameters": NotRequired[RunCommandParametersExtraOutputTypeDef],
-        "EcsParameters": NotRequired[EcsParametersExtraOutputTypeDef],
-        "BatchParameters": NotRequired[BatchParametersTypeDef],
-        "SqsParameters": NotRequired[SqsParametersTypeDef],
-        "HttpParameters": NotRequired[HttpParametersExtraOutputTypeDef],
-        "RedshiftDataParameters": NotRequired[RedshiftDataParametersExtraOutputTypeDef],
-        "SageMakerPipelineParameters": NotRequired[SageMakerPipelineParametersExtraOutputTypeDef],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-        "RetryPolicy": NotRequired[RetryPolicyTypeDef],
-        "AppSyncParameters": NotRequired[AppSyncParametersTypeDef],
-    },
-)
-TargetOutputTypeDef = TypedDict(
-    "TargetOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "RoleArn": NotRequired[str],
-        "Input": NotRequired[str],
-        "InputPath": NotRequired[str],
-        "InputTransformer": NotRequired[InputTransformerOutputTypeDef],
-        "KinesisParameters": NotRequired[KinesisParametersTypeDef],
-        "RunCommandParameters": NotRequired[RunCommandParametersOutputTypeDef],
-        "EcsParameters": NotRequired[EcsParametersOutputTypeDef],
-        "BatchParameters": NotRequired[BatchParametersTypeDef],
-        "SqsParameters": NotRequired[SqsParametersTypeDef],
-        "HttpParameters": NotRequired[HttpParametersOutputTypeDef],
-        "RedshiftDataParameters": NotRequired[RedshiftDataParametersOutputTypeDef],
-        "SageMakerPipelineParameters": NotRequired[SageMakerPipelineParametersOutputTypeDef],
-        "DeadLetterConfig": NotRequired[DeadLetterConfigTypeDef],
-        "RetryPolicy": NotRequired[RetryPolicyTypeDef],
-        "AppSyncParameters": NotRequired[AppSyncParametersTypeDef],
-    },
-)
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "Id": str,
         "Arn": str,
         "RoleArn": NotRequired[str],
         "Input": NotRequired[str],
@@ -1805,15 +1527,15 @@
 )
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": NotRequired[ConnectionBasicAuthResponseParametersTypeDef],
         "OAuthParameters": NotRequired[ConnectionOAuthResponseParametersTypeDef],
         "ApiKeyAuthParameters": NotRequired[ConnectionApiKeyAuthResponseParametersTypeDef],
-        "InvocationHttpParameters": NotRequired[ConnectionHttpParametersOutputTypeDef],
+        "InvocationHttpParameters": NotRequired[ConnectionHttpParametersTypeDef],
     },
 )
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
         "BasicAuthParameters": NotRequired[CreateConnectionBasicAuthRequestParametersTypeDef],
         "OAuthParameters": NotRequired[CreateConnectionOAuthRequestParametersTypeDef],
@@ -1916,20 +1638,27 @@
         "State": EndpointStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
-TargetUnionTypeDef = Union[TargetTypeDef, TargetExtraOutputTypeDef]
+PutTargetsRequestRequestTypeDef = TypedDict(
+    "PutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetTypeDef],
+        "EventBusName": NotRequired[str],
+    },
+)
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -1961,19 +1690,11 @@
         "AuthParameters": NotRequired[UpdateConnectionAuthRequestParametersTypeDef],
     },
 )
 ListEndpointsResponseTypeDef = TypedDict(
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
-    },
-)
-PutTargetsRequestRequestTypeDef = TypedDict(
-    "PutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-        "EventBusName": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/PKG-INFO` & `mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-events
-Version: 1.34.104
-Summary: Type annotations for boto3.EventBridge 1.34.104 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.17
+Summary: Type annotations for boto3.EventBridge 1.34.17 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-events.svg?color=blue)](https://pypi.org/project/mypy-boto3-events)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-events)](https://pepy.tech/project/mypy-boto3-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EventBridge 1.34.104](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[boto3.EventBridge 1.34.17](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-events docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_events-1.34.104/mypy_boto3_events.egg-info/SOURCES.txt` & `mypy-boto3-events-1.34.17/mypy_boto3_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_events-1.34.104/setup.py` & `mypy-boto3-events-1.34.17/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,24 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-events",
-    version="1.34.104",
+    version="1.34.17",
     packages=["mypy_boto3_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.EventBridge 1.34.104 service generated with mypy-boto3-builder 7.24.0",
+    description=(
+        "Type annotations for boto3.EventBridge 1.34.17 service generated with mypy-boto3-builder"
+        " 7.23.1"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

