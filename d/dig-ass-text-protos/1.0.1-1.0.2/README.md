# Comparing `tmp/dig_ass_text_protos-1.0.1.tar.gz` & `tmp/dig_ass_text_protos-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-1.0.1.tar", last modified: Thu May  2 14:36:39 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-1.0.2.tar", last modified: Mon May 13 14:30:25 2024, max compression
```

## Comparing `dig_ass_text_protos-1.0.1.tar` & `dig_ass_text_protos-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.1/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.1/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-02 14:36:37.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 14:35:07.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1646 2024-05-02 14:34:57.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 14:36:39.000000 dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.1/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 14:36:39.167640 dig_ass_text_protos-1.0.1/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.1/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:25.426040 dig_ass_text_protos-1.0.2/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.2/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-13 14:30:25.426040 dig_ass_text_protos-1.0.2/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.2/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:25.426040 dig_ass_text_protos-1.0.2/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-13 14:30:23.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-13 14:30:23.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-13 14:30:23.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:27:06.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1551 2024-05-13 14:05:20.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:25.426040 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-13 14:30:25.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-13 14:30:25.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:30:25.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:30:25.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-13 14:30:25.000000 dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:36.000000 dig_ass_text_protos-1.0.2/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:30:25.426040 dig_ass_text_protos-1.0.2/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.2/setup.py
```

### Comparing `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.1/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-1.0.2/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.1/dig_ass_text_protos/client.py` & `dig_ass_text_protos-1.0.2/dig_ass_text_protos/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     DigitalAssistantTextResponse,
     ChatItem,
     OuterContextItem,
     InnerContextItem,
     ReplicaItem,
 )
 
-from .abstract_client import AbstractClient
+from agi_med_utils.abstract_client import AbstractClient
 
 
 class TextClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantTextStub(self._channel)
 
@@ -25,20 +25,15 @@
                 OuterContext=OuterContextItem(
                     Sex=outer_context['Sex'],
                     Age=outer_context['Age'],
                     UserId=outer_context['UserId'],
                     SessionId=outer_context['SessionId'],
                     ClientId=outer_context['ClientId'],
                 ),
-                InnerContext=InnerContextItem(
-                    Replicas=[
-                        self.__rep_to_obj(replica)
-                        for replica in inner_context['Replicas']
-                    ]
-                ),
+                InnerContext=InnerContextItem(Replicas=[self.__rep_to_obj(replica) for replica in inner_context['Replicas']]),
             ),
         )
         response: DigitalAssistantTextResponse = self._stub.GetTextResponse(request)
         return response.Text
 
     def __rep_to_obj(self, replica_dict):
         return ReplicaItem(
```

### Comparing `dig_ass_text_protos-1.0.1/dig_ass_text_protos.egg-info/SOURCES.txt` & `dig_ass_text_protos-1.0.2/dig_ass_text_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-1.0.1/setup.py` & `dig_ass_text_protos-1.0.2/setup.py`

 * *Files identical despite different names*

