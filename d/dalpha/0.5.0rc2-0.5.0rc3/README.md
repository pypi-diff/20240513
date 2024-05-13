# Comparing `tmp/dalpha-0.5.0rc2.tar.gz` & `tmp/dalpha-0.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.0rc2.tar", max compression
+gzip compressed data, was "dalpha-0.5.0rc3.tar", max compression
```

## Comparing `dalpha-0.5.0rc2.tar` & `dalpha-0.5.0rc3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc2/README.md
--rw-r--r--   0        0        0     1966 2024-05-11 06:19:40.367843 dalpha-0.5.0rc2/dalpha/__init__.py
--rw-r--r--   0        0        0     8170 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc2/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/dto.py
--rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/exception.py
--rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc2/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc2/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6601 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc3/README.md
+-rw-r--r--   0        0        0     1966 2024-05-11 06:19:40.367843 dalpha-0.5.0rc3/dalpha/__init__.py
+-rw-r--r--   0        0        0     8194 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc3/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/dto.py
+-rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/exception.py
+-rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.0rc3/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc3/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc3/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6625 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc3/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc3/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc3/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-13 09:40:01.895738 dalpha-0.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc3/PKG-INFO
```

### Comparing `dalpha-0.5.0rc2/README.md` & `dalpha-0.5.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/__init__.py` & `dalpha-0.5.0rc3/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/agent.py` & `dalpha-0.5.0rc3/dalpha/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys, os
 import time
 import sentry_sdk
 from dataclasses import asdict
+from typing import List
 
 from dalpha.backend_cli import BackendCli
 from dalpha.message_consumer import EvaluateItem, KafkaMessageConsumer, RawMessageConsumer, SqsMessageConsumer
 from dalpha.signal_handler import get_shutdown_requested
 from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
 from dalpha.logging import logger
 from dalpha.logging.events import Event
@@ -131,15 +132,15 @@
         if mock:
             logger.info(
                 "return mock",
                 data = self.mock
             )
             return self.mock
 
-        ret: list[EvaluateItem] = self.message_consumer.poll()
+        ret: List[EvaluateItem] = self.message_consumer.poll()
         if len(ret) == 0:
             # 가져온 메세지가 없으면 None 반환
             return None
         elif len(ret) == 1:
             # 가져온 메세지가 1개면 list 형태가 아닌 낱개로 반환
             logger.info(
                 message = f"return evaluate item: {ret[0]}",
```

### Comparing `dalpha-0.5.0rc2/dalpha/backend_cli.py` & `dalpha-0.5.0rc3/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/cobra_cls.py` & `dalpha-0.5.0rc3/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/context.py` & `dalpha-0.5.0rc3/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/data_update_cls.py` & `dalpha-0.5.0rc3/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/dto.py` & `dalpha-0.5.0rc3/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/exception.py` & `dalpha-0.5.0rc3/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/inference_cls.py` & `dalpha-0.5.0rc3/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/logging/__init__.py` & `dalpha-0.5.0rc3/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/logging/log_formatter.py` & `dalpha-0.5.0rc3/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/logging/utils.py` & `dalpha-0.5.0rc3/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/message_consumer.py` & `dalpha-0.5.0rc3/dalpha/message_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import time
 from typing import Optional
 from dalpha.backend_cli import BackendCli
 from dalpha.logging import logger
 from pydantic import BaseModel
 from abc import ABCMeta, abstractmethod
+from typing import List
 
 from dalpha.logging.events import Event
 
 class EvaluateItem(BaseModel):
     id: int
     evaluateGroupId: Optional[int]
     accountId: int
@@ -25,15 +26,15 @@
         inferenceApiId = message.get("inferenceApiId"),
         key = message.get("key"),
         metadata = message.get("metadata")
     )
 
 class MessageConsumer(metaclass=ABCMeta):
     @abstractmethod
-    def poll(self, records: int = 1, timeout_ms: int = 5000) -> list[EvaluateItem]:
+    def poll(self, records: int = 1, timeout_ms: int = 5000) -> List[EvaluateItem]:
         pass
 
     @abstractmethod
     def commit(self, id):
         pass
 
     @abstractmethod
@@ -43,15 +44,15 @@
 class KafkaMessageConsumer(MessageConsumer):
     def __init__(self, api_id: int, backend_cli: BackendCli, kafka_topic: str):
         self.kafka_topic = kafka_topic
         from dalpha.kafka_cli import get_consumer
         self.kafka_consumer = get_consumer(self.kafka_topic, api_id)
         self.backend_cli = backend_cli
 
-    def poll(self, records: int = 1, timeout_ms: int = 5000) -> list[EvaluateItem]:
+    def poll(self, records: int = 1, timeout_ms: int = 5000) -> List[EvaluateItem]:
         record = self.kafka_consumer.poll(
             timeout_ms=timeout_ms,
             max_records=records,
             update_offsets=False,
         )
         
         ret = []
@@ -108,15 +109,15 @@
                 self.sqs_consumer.delete_message_batch(
                     QueueUrl = self.queue_url,
                     Entries = group
                 )
             except Exception as e:
                 logger.error(f"Error while deleting messages\n{e}")
 
-    def poll(self, records: int = 1) -> list[EvaluateItem]:
+    def poll(self, records: int = 1) -> List[EvaluateItem]:
         # sqs로부터 메시지를 가져옴
         response = self.sqs_consumer.receive_message(
             QueueUrl = self.queue_url,
             MaxNumberOfMessages = records  # 가져올 메시지의 최대 수 (1개 이상 설정 가능)
         )
         evaluate_items = []
         invalid_messages = []
@@ -164,15 +165,15 @@
 class RawMessageConsumer(MessageConsumer):
     def __init__(self, api_id: int, backend_cli: BackendCli, **kwargs):
         self.api_id = api_id
         self.token = kwargs.get("token")
         self.backend_cli = backend_cli
         
 
-    def poll(self, records: int = 1, timeout_ms: int = 5000) -> list[EvaluateItem]:
+    def poll(self, records: int = 1, timeout_ms: int = 5000) -> List[EvaluateItem]:
         time.sleep(0.2)
         poll_result = self.backend_cli.poll()
         if poll_result:  
             logger.info(
                 message = "return poll item",
                 event = Event.POLL,
                 data = poll_result
```

### Comparing `dalpha-0.5.0rc2/dalpha/openai_cls.py` & `dalpha-0.5.0rc3/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/redis_cli.py` & `dalpha-0.5.0rc3/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/redis_cls.py` & `dalpha-0.5.0rc3/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/request.py` & `dalpha-0.5.0rc3/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/s3.py` & `dalpha-0.5.0rc3/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/slack.py` & `dalpha-0.5.0rc3/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/dalpha/update_agent.py` & `dalpha-0.5.0rc3/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc2/pyproject.toml` & `dalpha-0.5.0rc3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.0rc2"
+version = "0.5.0rc3"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.0rc2"
+version = "0.5.0rc3"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.0rc2/PKG-INFO` & `dalpha-0.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.0rc2
+Version: 0.5.0rc3
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

