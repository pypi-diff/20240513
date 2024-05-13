# Comparing `tmp/dig_ass_chat_protos-1.0.0.tar.gz` & `tmp/dig_ass_chat_protos-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-1.0.0.tar", last modified: Thu May  2 11:13:02 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-1.0.1.tar", last modified: Mon May 13 14:30:09 2024, max compression
```

## Comparing `dig_ass_chat_protos-1.0.0.tar` & `dig_ass_chat_protos-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-1.0.0/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-1.0.0/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.123752 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2174 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1377 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3102 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1095 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-1.0.0/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:09.880782 dig_ass_chat_protos-1.0.1/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-1.0.1/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-13 14:30:09.880782 dig_ass_chat_protos-1.0.1/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-1.0.1/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:09.876782 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2174 2024-05-13 14:30:08.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1377 2024-05-13 14:30:08.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3102 2024-05-13 14:30:08.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-13 14:27:05.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1086 2024-05-13 14:05:04.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-13 14:30:09.880782 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      371 2024-05-13 14:30:09.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-05-13 14:30:09.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-13 14:30:09.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       57 2024-05-13 14:30:09.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-13 14:30:09.000000 dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       56 2024-05-13 14:20:32.000000 dig_ass_chat_protos-1.0.1/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-13 14:30:09.880782 dig_ass_chat_protos-1.0.1/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.1/setup.py
```

### Comparing `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py` & `dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi` & `dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py` & `dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/client.py` & `dig_ass_chat_protos-1.0.1/dig_ass_chat_protos/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 )
 from dig_ass_chat_protos.DigitalAssistantChatManager_pb2 import (
     DigitalAssistantChatManagerRequest,
     DigitalAssistantChatManagerResponse,
     OuterContextItem,
 )
 
-from .abstract_client import AbstractClient
+from agi_med_utils.abstract_client import AbstractClient
 
 
 class ChatManagerClient(AbstractClient):
     def __init__(self, address) -> None:
         super().__init__(address)
         self._stub = DigitalAssistantChatManagerStub(self._channel)
 
@@ -22,11 +22,9 @@
                 Sex=outer_context['Sex'],
                 Age=outer_context['Age'],
                 UserId=outer_context['UserId'],
                 SessionId=outer_context['SessionId'],
                 ClientId=outer_context['ClientId'],
             ),
         )
-        response: DigitalAssistantChatManagerResponse = self._stub.GetTextResponse(
-            request
-        )
+        response: DigitalAssistantChatManagerResponse = self._stub.GetTextResponse(request)
         return response.Text
```

### Comparing `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/SOURCES.txt` & `dig_ass_chat_protos-1.0.1/dig_ass_chat_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-1.0.0/setup.py` & `dig_ass_chat_protos-1.0.1/setup.py`

 * *Files identical despite different names*

