# Comparing `tmp/dalpha-0.5.0rc1.tar.gz` & `tmp/dalpha-0.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.0rc1.tar", max compression
+gzip compressed data, was "dalpha-0.5.0rc2.tar", max compression
```

## Comparing `dalpha-0.5.0rc1.tar` & `dalpha-0.5.0rc2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc1/README.md
--rw-r--r--   0        0        0     1966 2024-05-11 06:19:40.367843 dalpha-0.5.0rc1/dalpha/__init__.py
--rw-r--r--   0        0        0     8158 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc1/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc1/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc1/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc1/dalpha/dto.py
--rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/exception.py
--rw-r--r--   0        0        0     6136 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc1/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc1/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc1/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc1/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc1/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc1/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc1/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc1/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc1/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-11 07:46:50.314364 dalpha-0.5.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.0rc2/README.md
+-rw-r--r--   0        0        0     1966 2024-05-11 06:19:40.367843 dalpha-0.5.0rc2/dalpha/__init__.py
+-rw-r--r--   0        0        0     8170 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/agent.py
+-rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.0rc2/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/dto.py
+-rw-r--r--   0        0        0      579 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/exception.py
+-rw-r--r--   0        0        0     6022 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.0rc2/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.0rc2/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6601 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.0rc2/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.0rc2/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/slack.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.0rc2/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-13 09:17:22.448483 dalpha-0.5.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.0rc2/PKG-INFO
```

### Comparing `dalpha-0.5.0rc1/README.md` & `dalpha-0.5.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/__init__.py` & `dalpha-0.5.0rc2/dalpha/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/agent.py` & `dalpha-0.5.0rc2/dalpha/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                 return
             if inference_time == None and self.poll_time != None:
                 inference_time = time.time() - self.poll_time
                 self.poll_time = None
             self.message_consumer.commit(evaluate_id)
             if log:
                 logger.info(
-                    message = "validate payload",
+                    message = f"validate payload - {output}",
                     event = Event.VALIDATE,
                     properties = {
                         "evaluate_id": evaluate_id,
                         "inference_time": inference_time,
                     },
                     data = output
                 )
```

### Comparing `dalpha-0.5.0rc1/dalpha/backend_cli.py` & `dalpha-0.5.0rc2/dalpha/backend_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/cobra_cls.py` & `dalpha-0.5.0rc2/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/context.py` & `dalpha-0.5.0rc2/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/data_update_cls.py` & `dalpha-0.5.0rc2/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/dto.py` & `dalpha-0.5.0rc2/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/exception.py` & `dalpha-0.5.0rc2/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/inference_cls.py` & `dalpha-0.5.0rc2/dalpha/inference_cls.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,26 +11,24 @@
 from dalpha.logging import logger
 
 
 class DalphaAI:
     def __init__(
         self,
         api_id: int,
-        inference: Callable[[Agent, Dict, int, int, bool], InferenceResult],
+        inference: Callable[[Agent, Dict, Dict, int, int], InferenceResult],
         load_globals: Callable[[], Dict],
         mock_file: Optional[str],
         mocks_file: Optional[str],
-        debug: bool,
     ):
         self.wait_flag = True
 
         self.agent = Agent(api_id=api_id)
         self.inference = inference
         self.globals = load_globals()
-        self.debug = debug
 
         self.is_mock, self.mock_info, self.mocks = self._init_mock(mock_file=mock_file, mocks_file=mocks_file)
 
     def _init_mock(
         self, mock_file: bool, mocks_file: bool
     ) -> Tuple[bool, Union[str, Literal["NO MOCK"]], List[Dict[str, any]]]:
         MOCK_STRUCTURE = "mock/mock_structure.json"
@@ -103,15 +101,15 @@
     def _pipeline(self):
         # poll input_json
         try:
             input_json = self._poll_input()
         except WaitException:
             return
 
-        logger.info(f"\n\033[31m\n\t| DEBUG MODE : {self.debug}\n\t| MOCK DATA : {self.mock_info}\n\033[0m")
+        logger.info(f"\n\033[31m\n\t| MOCK DATA : {self.mock_info}\n\033[0m")
         logger.info("processing...")
 
         try:
             # read input.
             # dynamic-type 으로 만든 경우 metadata가 input과 같습니다.
             eval_id, account_id, metadata = (
                 input_json["id"],
@@ -131,16 +129,15 @@
             inference_start_time = time.time()
 
             inference_result: InferenceResult = self.inference(
                 agent=self.agent,
                 globals=self.globals,
                 metadata=metadata,
                 eval_id=eval_id,
-                account_id=account_id,
-                debug=self.debug,
+                account_id=account_id
             )
             inference_end_time = time.time()
             logger.info(f"AI inference is done. Time taken: {inference_end_time - inference_start_time:.2f} sec")
         except ExpectedError as expected_error:
             self.agent.validate_error(evaluate_id=eval_id, output=expected_error.error_json, mock=self.is_mock, error_code=expected_error.error_code)
             self.wait_flag = True
             return
```

### Comparing `dalpha-0.5.0rc1/dalpha/logging/__init__.py` & `dalpha-0.5.0rc2/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/logging/log_formatter.py` & `dalpha-0.5.0rc2/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/logging/utils.py` & `dalpha-0.5.0rc2/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/message_consumer.py` & `dalpha-0.5.0rc2/dalpha/message_consumer.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,20 +167,20 @@
         self.token = kwargs.get("token")
         self.backend_cli = backend_cli
         
 
     def poll(self, records: int = 1, timeout_ms: int = 5000) -> list[EvaluateItem]:
         time.sleep(0.2)
         poll_result = self.backend_cli.poll()
-        logger.info(
-            message = "return poll item",
-            event = Event.POLL,
-            data = poll_result
-        )
-        if poll_result:
+        if poll_result:  
+            logger.info(
+                message = "return poll item",
+                event = Event.POLL,
+                data = poll_result
+            )
             return [to_evaluate_item(poll_result)]
         else:
             return []
 
     def commit(self, id):
         pass
```

### Comparing `dalpha-0.5.0rc1/dalpha/openai_cls.py` & `dalpha-0.5.0rc2/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/redis_cli.py` & `dalpha-0.5.0rc2/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/redis_cls.py` & `dalpha-0.5.0rc2/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/request.py` & `dalpha-0.5.0rc2/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/s3.py` & `dalpha-0.5.0rc2/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/slack.py` & `dalpha-0.5.0rc2/dalpha/slack.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/dalpha/update_agent.py` & `dalpha-0.5.0rc2/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.0rc1/pyproject.toml` & `dalpha-0.5.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.0rc1"
+version = "0.5.0rc2"
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
-version = "0.5.0rc1"
+version = "0.5.0rc2"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.0rc1/PKG-INFO` & `dalpha-0.5.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.0rc1
+Version: 0.5.0rc2
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

