# Comparing `tmp/literalai-0.0.600.tar.gz` & `tmp/literalai-0.0.601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.600.tar", last modified: Mon May  6 12:55:47 2024, max compression
+gzip compressed data, was "literalai-0.0.601.tar", last modified: Mon May 13 13:05:50 2024, max compression
```

## Comparing `literalai-0.0.600.tar` & `literalai-0.0.601.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-06 12:55:36.000000 literalai-0.0.600/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 12:55:47.387939 literalai-0.0.600/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-06 12:55:36.000000 literalai-0.0.600/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.383939 literalai-0.0.600/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    81961 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     9789 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-06 12:55:36.000000 literalai-0.0.600/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 12:55:47.000000 literalai-0.0.600/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 12:55:47.387939 literalai-0.0.600/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-06 12:55:36.000000 literalai-0.0.600/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:47.387939 literalai-0.0.600/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 12:55:36.000000 literalai-0.0.600/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 13:05:39.000000 literalai-0.0.601/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 13:05:50.921444 literalai-0.0.601/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-13 13:05:39.000000 literalai-0.0.601/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    84378 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20998 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12198 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-13 13:05:39.000000 literalai-0.0.601/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.917444 literalai-0.0.601/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 13:05:50.000000 literalai-0.0.601/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:05:50.921444 literalai-0.0.601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-13 13:05:39.000000 literalai-0.0.601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:50.921444 literalai-0.0.601/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:39.000000 literalai-0.0.601/tests/__init__.py
```

### Comparing `literalai-0.0.600/LICENSE` & `literalai-0.0.601/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/README.md` & `literalai-0.0.601/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/__init__.py` & `literalai-0.0.601/literalai/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     generations_order_by,
     scores_filters,
     scores_order_by,
     threads_filters,
     threads_order_by,
     users_filters,
 )
+
+from literalai.filter import steps_filters, steps_order_by
 from literalai.prompt import Prompt, ProviderSettings
 
 from .attachment_helpers import (
     AttachmentUpload,
     create_attachment_helper,
     delete_attachment_helper,
     get_attachment_helper,
@@ -62,14 +64,15 @@
     get_scores_helper,
     update_score_helper,
 )
 from .step_helpers import (
     create_step_helper,
     delete_step_helper,
     get_step_helper,
+    get_steps_helper,
     send_steps_helper,
     update_step_helper,
 )
 from .thread_helpers import (
     create_thread_helper,
     delete_thread_helper,
     get_thread_helper,
@@ -92,14 +95,15 @@
 import httpx
 
 from literalai.my_types import (
     Attachment,
     ChatGeneration,
     CompletionGeneration,
     GenerationMessage,
+    PaginatedResponse,
     Score,
     ScoreDict,
     ScoreType,
 )
 from literalai.step import Step, StepDict, StepType
 
 logger = logging.getLogger(__name__)
@@ -128,14 +132,32 @@
         return {
             "Content-Type": "application/json",
             "x-api-key": self.api_key,
             "x-client-name": "py-literal-client",
             "x-client-version": __version__,
         }
 
+    def _prepare_variables(self, variables: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Recursively checks and converts bytes objects in variables.
+        """
+
+        def handle_bytes(item):
+            if isinstance(item, bytes):
+                return "STRIPPED_BINARY_DATA"
+            elif isinstance(item, dict):
+                return {k: handle_bytes(v) for k, v in item.items()}
+            elif isinstance(item, list):
+                return [handle_bytes(i) for i in item]
+            elif isinstance(item, tuple):
+                return tuple(handle_bytes(i) for i in item)
+            return item
+
+        return handle_bytes(variables)
+
 
 class LiteralAPI(BaseLiteralAPI):
     R = TypeVar("R")
 
     def make_gql_call(
         self, description: str, query: str, variables: Dict[str, Any]
     ) -> Dict:
@@ -154,14 +176,16 @@
             Exception: If the GraphQL call fails or returns errors.
         """
 
         def raise_error(error):
             logger.error(f"Failed to {description}: {error}")
             raise Exception(error)
 
+        variables = self._prepare_variables(variables)
+
         with httpx.Client() as client:
             response = client.post(
                 self.graphql_endpoint,
                 json={"query": query, "variables": variables},
                 headers=self.headers,
                 timeout=10,
             )
@@ -349,15 +373,17 @@
             filters (Optional[threads_filters]): Filters to apply on the threads query.
             order_by (Optional[threads_order_by]): Order by clause for threads.
 
         Returns:
             A list of threads that match the criteria.
         """
         return self.gql_helper(
-            *get_threads_helper(first, after, before, filters, order_by, step_types_to_keep)
+            *get_threads_helper(
+                first, after, before, filters, order_by, step_types_to_keep
+            )
         )
 
     def list_threads(
         self,
         first: Optional[int] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
@@ -631,15 +657,17 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = (
+            {}
+        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
@@ -857,14 +885,39 @@
                 tags=tags,
                 start_time=start_time,
                 end_time=end_time,
                 parent_id=parent_id,
             )
         )
 
+    def get_steps(
+        self,
+        first: Optional[int] = None,
+        after: Optional[str] = None,
+        before: Optional[str] = None,
+        filters: Optional[steps_filters] = None,
+        order_by: Optional[steps_order_by] = None,
+    ) -> PaginatedResponse[Step]:
+        """
+        Fetches a list of steps based on pagination and optional filters.
+
+        Args:
+            first (Optional[int]): Number of steps to fetch.
+            after (Optional[str]): Cursor for pagination, fetch steps after this cursor.
+            before (Optional[str]): Cursor for pagination, fetch steps before this cursor.
+            filters (Optional[steps_filters]): Filters to apply on the steps query.
+            order_by (Optional[steps_order_by]): Order by clause for steps.
+
+        Returns:
+            A list of steps that match the criteria.
+        """
+        return self.gql_helper(
+            *get_steps_helper(first, after, before, filters, order_by)
+        )
+
     def get_step(
         self,
         id: str,
     ):
         """
         Retrieves a step by its ID.
 
@@ -1262,14 +1315,16 @@
             Exception: If the GraphQL call fails or returns errors.
         """
 
         def raise_error(error):
             logger.error(f"Failed to {description}: {error}")
             raise Exception(error)
 
+        variables = self._prepare_variables(variables)
+
         async with httpx.AsyncClient() as client:
             response = await client.post(
                 self.graphql_endpoint,
                 json={"query": query, "variables": variables},
                 headers=self.headers,
                 timeout=10,
             )
@@ -1461,15 +1516,17 @@
             filters (Optional[threads_filters]): Filters to apply to the thread query.
             order_by (Optional[threads_order_by]): Ordering criteria for the threads.
 
         Returns:
             The result of the GraphQL helper function for fetching threads.
         """
         return await self.gql_helper(
-            *get_threads_helper(first, after, before, filters, order_by, step_types_to_keep)
+            *get_threads_helper(
+                first, after, before, filters, order_by, step_types_to_keep
+            )
         )
 
     async def list_threads(
         self,
         first: Optional[int] = None,
         after: Optional[str] = None,
         before: Optional[str] = None,
@@ -1766,15 +1823,17 @@
         object_key: Optional[str] = fields.get("key")
         upload_type: Literal["raw", "multipart"] = request_dict.get(
             "uploadType", "multipart"
         )
         signed_url: Optional[str] = json_res.get("signedUrl")
 
         # Prepare form data
-        form_data = {}  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
+        form_data = (
+            {}
+        )  # type: Dict[str, Union[Tuple[Union[str, None], Any], Tuple[Union[str, None], Any, Any]]]
         for field_name, field_value in fields.items():
             form_data[field_name] = (None, field_value)
 
         # Add file to the form_data
         # Note: The content_type parameter is not needed here, as the correct MIME type should be set in the 'Content-Type' field from upload_details
         form_data["file"] = (id, content, mime)
 
@@ -1994,14 +2053,28 @@
                 tags=tags,
                 start_time=start_time,
                 end_time=end_time,
                 parent_id=parent_id,
             )
         )
 
+    async def get_steps(
+        self,
+        first: Optional[int] = None,
+        after: Optional[str] = None,
+        before: Optional[str] = None,
+        filters: Optional[steps_filters] = None,
+        order_by: Optional[steps_order_by] = None,
+    ) -> PaginatedResponse[Step]:
+        return await self.gql_helper(
+            *get_steps_helper(first, after, before, filters, order_by)
+        )
+
+    get_steps.__doc__ = LiteralAPI.get_steps.__doc__
+
     async def get_step(
         self,
         id: str,
     ):
         """
         Asynchronously retrieves a step by its ID.
 
@@ -2172,15 +2245,15 @@
         params: Optional[Dict] = None,
     ) -> "DatasetExperiment":
         sync_api = LiteralAPI(self.api_key, self.url)
 
         return await self.gql_helper(
             *create_experiment_helper(sync_api, dataset_id, name, prompt_id, params)
         )
-    
+
     create_experiment.__doc__ = LiteralAPI.create_experiment.__doc__
 
     async def create_experiment_item(
         self, experiment_item: DatasetExperimentItem
     ) -> DatasetExperimentItem:
         """
         Asynchronously creates an item within an experiment.
@@ -2350,9 +2423,9 @@
             return await self.gql_helper(*get_prompt_helper(sync_api, id=id))
         elif name:
             return await self.gql_helper(
                 *get_prompt_helper(sync_api, name=name, version=version)
             )
         else:
             raise ValueError("Either the `id` or the `name` must be provided.")
-    
+
     get_prompt.__doc__ = LiteralAPI.get_prompt.__doc__
```

### Comparing `literalai-0.0.600/literalai/api/attachment_helpers.py` & `literalai-0.0.601/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/dataset_helpers.py` & `literalai-0.0.601/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/generation_helpers.py` & `literalai-0.0.601/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/gql.py` & `literalai-0.0.601/literalai/api/gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 STEP_FIELDS = """
         id
         threadId
         parentId
         startTime
         endTime
         createdAt
+        participantIdentifier
         type
         error
         input
         output
         metadata
         scores {
             id
@@ -630,14 +631,56 @@
     + STEP_FIELDS
     + """
     }
 }
 """
 )
 
+GET_STEPS = (
+    """
+query GetSteps(
+    $after: ID,
+    $before: ID,
+    $cursorAnchor: DateTime,
+    $filters: [stepsInputType!],
+    $orderBy: StepsOrderByInput,
+    $first: Int,
+    $last: Int,
+    $projectId: String,
+    ) {
+    steps(
+        after: $after,
+        before: $before,
+        cursorAnchor: $cursorAnchor,
+        filters: $filters,
+        orderBy: $orderBy,
+        first: $first,
+        last: $last,
+        projectId: $projectId,
+        ) {
+        pageInfo {
+            startCursor
+            endCursor
+            hasNextPage
+            hasPreviousPage
+        }
+        totalCount
+        edges {
+            cursor
+            node {
+"""
+    + STEP_FIELDS
+    + """
+            }
+        }
+    }
+}
+"""
+)
+
 GET_STEP = (
     """
 query GetStep($id: String!) {
     step(id: $id) {"""
     + STEP_FIELDS
     + """
     }
```

### Comparing `literalai-0.0.600/literalai/api/prompt_helpers.py` & `literalai-0.0.601/literalai/api/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/score_helpers.py` & `literalai-0.0.601/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/api/step_helpers.py` & `literalai-0.0.601/literalai/api/user_helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,106 +1,89 @@
-from typing import Dict, List, Optional, Union
+from typing import Any, Dict, Optional
 
-from literalai.step import Step, StepDict, StepType
+from literalai.filter import users_filters
+from literalai.my_types import PaginatedResponse, User
 
 from . import gql
 
 
-def create_step_helper(
-    thread_id: Optional[str] = None,
-    type: Optional[StepType] = "undefined",
-    start_time: Optional[str] = None,
-    end_time: Optional[str] = None,
-    input: Optional[Dict] = None,
-    output: Optional[Dict] = None,
-    metadata: Optional[Dict] = None,
-    parent_id: Optional[str] = None,
-    name: Optional[str] = None,
-    tags: Optional[List[str]] = None,
+def get_users_helper(
+    first: Optional[int] = None,
+    after: Optional[str] = None,
+    before: Optional[str] = None,
+    filters: Optional[users_filters] = None,
 ):
-    variables = {
-        "threadId": thread_id,
-        "type": type,
-        "startTime": start_time,
-        "endTime": end_time,
-        "input": input,
-        "output": output,
-        "metadata": metadata,
-        "parentId": parent_id,
-        "name": name,
-        "tags": tags,
-    }
+    variables: Dict[str, Any] = {}
+
+    if first:
+        variables["first"] = first
+    if after:
+        variables["after"] = after
+    if before:
+        variables["before"] = before
+    if filters:
+        variables["filters"] = filters
 
     def process_response(response):
-        return Step.from_dict(response["data"]["createStep"])
+        response = response["data"]["participants"]
+        response["data"] = list(map(lambda x: x["node"], response["edges"]))
+        return PaginatedResponse[User].from_dict(response, User)
 
-    description = "create step"
+    description = "get users"
 
-    return gql.CREATE_STEP, description, variables, process_response
+    return gql.GET_PARTICIPANTS, description, variables, process_response
 
 
-def update_step_helper(
-    id: str,
-    type: Optional[StepType] = None,
-    input: Optional[str] = None,
-    output: Optional[str] = None,
-    metadata: Optional[Dict] = None,
-    name: Optional[str] = None,
-    tags: Optional[List[str]] = None,
-    start_time: Optional[str] = None,
-    end_time: Optional[str] = None,
-    parent_id: Optional[str] = None,
-):
-    variables = {
-        "id": id,
-        "type": type,
-        "input": input,
-        "output": output,
-        "metadata": metadata,
-        "name": name,
-        "tags": tags,
-        "startTime": start_time,
-        "endTime": end_time,
-        "parentId": parent_id,
-    }
+def create_user_helper(identifier: str, metadata: Optional[Dict] = None):
+    variables = {"identifier": identifier, "metadata": metadata}
 
     def process_response(response):
-        return Step.from_dict(response["data"]["updateStep"])
+        return User.from_dict(response["data"]["createParticipant"])
 
-    description = "update step"
+    description = "create user"
 
-    return gql.UPDATE_STEP, description, variables, process_response
+    return gql.CREATE_PARTICIPANT, description, variables, process_response
 
 
-def get_step_helper(id: str):
-    variables = {"id": id}
+def update_user_helper(
+    id: str, identifier: Optional[str] = None, metadata: Optional[Dict] = None
+):
+    variables = {"id": id, "identifier": identifier, "metadata": metadata}
+
+    # remove None values to prevent the API from removing existing values
+    variables = {k: v for k, v in variables.items() if v is not None}
 
     def process_response(response):
-        step = response["data"]["step"]
-        return Step.from_dict(step) if step else None
+        return User.from_dict(response["data"]["updateParticipant"])
 
-    description = "get step"
+    description = "update user"
 
-    return gql.GET_STEP, description, variables, process_response
+    return gql.UPDATE_PARTICIPANT, description, variables, process_response
 
 
-def delete_step_helper(id: str):
-    variables = {"id": id}
+def get_user_helper(id: Optional[str] = None, identifier: Optional[str] = None):
+    if id is None and identifier is None:
+        raise Exception("Either id or identifier must be provided")
+
+    if id is not None and identifier is not None:
+        raise Exception("Only one of id or identifier must be provided")
+
+    variables = {"id": id, "identifier": identifier}
 
     def process_response(response):
-        return bool(response["data"]["deleteStep"])
+        user = response["data"]["participant"]
+        return User.from_dict(user) if user else None
 
-    description = "delete step"
+    description = "get user"
 
-    return gql.DELETE_STEP, description, variables, process_response
+    return gql.GET_PARTICIPANT, description, variables, process_response
 
 
-def send_steps_helper(steps: List[Union[StepDict, "Step"]]):
-    query = gql.steps_query_builder(steps)
-    variables = gql.steps_variables_builder(steps)
+def delete_user_helper(id: str):
+    variables = {"id": id}
 
-    description = "send steps"
+    def process_response(response):
+        return response["data"]["deleteParticipant"]["id"]
 
-    def process_response(response: Dict):
-        return response
+    description = "delete user"
 
-    return query, description, variables, process_response
+    return gql.DELETE_PARTICIPANT, description, variables, process_response
```

### Comparing `literalai-0.0.600/literalai/api/thread_helpers.py` & `literalai-0.0.601/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/callback/langchain_callback.py` & `literalai-0.0.601/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/callback/llama_index_callback.py` & `literalai-0.0.601/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/client.py` & `literalai-0.0.601/literalai/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -107,33 +107,36 @@
         original_function=None,
         *,
         name: str = "",
         type: TrueStepType = "undefined",
         id: Optional[str] = None,
         parent_id: Optional[str] = None,
         thread_id: Optional[str] = None,
+        **kwargs,
     ):
         if original_function:
             return step_decorator(
                 self,
                 func=original_function,
                 name=name,
                 type=type,
                 id=id,
                 parent_id=parent_id,
                 thread_id=thread_id,
+                **kwargs,
             )
         else:
             return StepContextManager(
                 self,
                 name=name,
                 type=type,
                 id=id,
                 parent_id=parent_id,
                 thread_id=thread_id,
+                **kwargs,
             )
 
     def run(
         self,
         original_function=None,
         *,
         name: str = "",
@@ -181,22 +184,24 @@
     def start_step(
         self,
         name: str = "",
         type: Optional[TrueStepType] = None,
         id: Optional[str] = None,
         parent_id: Optional[str] = None,
         thread_id: Optional[str] = None,
+        **kwargs,
     ):
         step = Step(
             name=name,
             type=type,
             id=id,
             parent_id=parent_id,
             thread_id=thread_id,
             processor=self.event_processor,
+            **kwargs,
         )
         step.start()
         return step
 
     def get_current_step(self):
         active_steps = active_steps_var.get()
         if active_steps and len(active_steps) > 0:
```

### Comparing `literalai-0.0.600/literalai/dataset.py` & `literalai-0.0.601/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/dataset_experiment.py` & `literalai-0.0.601/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/dataset_item.py` & `literalai-0.0.601/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/event_processor.py` & `literalai-0.0.601/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/filter.py` & `literalai-0.0.601/literalai/filter.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,32 @@
     "scoreValue",
     "duration",
 ]
 threads_orderable_fields = Literal["createdAt", "tokenCount"]
 threads_filters = List[Filter[threads_filterable_fields]]
 threads_order_by = OrderBy[threads_orderable_fields]
 
+steps_filterable_fields = Literal[
+    "id",
+    "name",
+    "input",
+    "output",
+    "participantIdentifier",
+    "startTime",
+    "endTime",
+    "metadata",
+    "parentId",
+    "threadId",
+    "error",
+    "tags",
+]
+steps_orderable_fields = Literal["createdAt"]
+steps_filters = List[Filter[steps_filterable_fields]]
+steps_order_by = OrderBy[steps_orderable_fields]
+
 users_filterable_fields = Literal[
     "id",
     "createdAt",
     "identifier",
     "lastEngaged",
     "threadCount",
     "tokenCount",
```

### Comparing `literalai-0.0.600/literalai/helper.py` & `literalai-0.0.601/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/instrumentation/openai.py` & `literalai-0.0.601/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/message.py` & `literalai-0.0.601/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/my_types.py` & `literalai-0.0.601/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/prompt.py` & `literalai-0.0.601/literalai/prompt.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/requirements.py` & `literalai-0.0.601/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/step.py` & `literalai-0.0.601/literalai/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import inspect
+import json
 import uuid
 from copy import deepcopy
 from functools import wraps
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -81,14 +82,15 @@
         self,
         name: str = "",
         type: Optional[StepType] = None,
         id: Optional[str] = None,
         thread_id: Optional[str] = None,
         parent_id: Optional[str] = None,
         processor: Optional["EventProcessor"] = None,
+        tags: Optional[List[str]] = None,
     ):
         from time import sleep
 
         sleep(0.001)
         self.id = id or str(uuid.uuid4())
         self.start_time = utc_now()
         self.name = name
@@ -98,14 +100,16 @@
 
         # priority for thread_id: thread_id > parent_step.thread_id > active_thread
         self.thread_id = thread_id
 
         # priority for parent_id: parent_id > parent_step.id
         self.parent_id = parent_id
 
+        self.tags = tags
+
     def start(self):
         active_steps = active_steps_var.get()
         if len(active_steps) > 0:
             parent_step = active_steps[-1]
             if not self.parent_id:
                 self.parent_id = parent_step.id
             if not self.thread_id:
@@ -153,14 +157,17 @@
             "generation": self.generation.to_dict() if self.generation else None,
             "name": self.name,
             "tags": self.tags,
             "scores": [score.to_dict() for score in self.scores],
             "attachments": [attachment.to_dict() for attachment in self.attachments],
         }
 
+    def __repr__(self):
+        return json.dumps(self.to_dict(), sort_keys=True, indent=4)
+
     @classmethod
     def from_dict(cls, step_dict: StepDict) -> "Step":
         name = step_dict.get("name") or ""
         step_type = step_dict.get("type", "undefined")
         thread_id = step_dict.get("threadId")
 
         step = cls(name=name, type=step_type, thread_id=thread_id)
@@ -201,21 +208,23 @@
         self,
         client: "BaseLiteralClient",
         name: str = "",
         type: TrueStepType = "undefined",
         id: Optional[str] = None,
         parent_id: Optional[str] = None,
         thread_id: Optional[str] = None,
+        **kwargs,
     ):
         self.client = client
         self.step_name = name
         self.step_type = type
         self.id = id
         self.parent_id = parent_id
         self.thread_id = thread_id
+        self.kwargs = kwargs
 
     def __call__(self, func):
         return step_decorator(
             self.client,
             func=func,
             name=self.step_name,
             ctx_manager=self,
@@ -224,14 +233,15 @@
     async def __aenter__(self):
         self.step = self.client.start_step(
             name=self.step_name,
             type=self.step_type,
             id=self.id,
             parent_id=self.parent_id,
             thread_id=self.thread_id,
+            **self.kwargs
         )
         return self.step
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             self.step.error = str(exc_val)
             await self.client.event_processor.aflush()
@@ -240,14 +250,15 @@
     def __enter__(self) -> Step:
         self.step = self.client.start_step(
             name=self.step_name,
             type=self.step_type,
             id=self.id,
             parent_id=self.parent_id,
             thread_id=self.thread_id,
+            **self.kwargs
         )
         return self.step
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if exc_type:
             self.step.error = str(exc_val)
             self.client.event_processor.flush()
@@ -259,25 +270,27 @@
     func: Callable,
     type: TrueStepType = "undefined",
     name: str = "",
     id: Optional[str] = None,
     parent_id: Optional[str] = None,
     thread_id: Optional[str] = None,
     ctx_manager: Optional[StepContextManager] = None,
+    **decorator_kwargs
 ):
     if not name:
         name = func.__name__
     if not ctx_manager:
         ctx_manager = StepContextManager(
             client=client,
             type=type,
             name=name,
             id=id,
             parent_id=parent_id,
             thread_id=thread_id,
+            **decorator_kwargs
         )
     else:
         ctx_manager.step_name = name
     # Handle async decorator
     if inspect.iscoroutinefunction(func):
 
         @wraps(func)
```

### Comparing `literalai-0.0.600/literalai/thread.py` & `literalai-0.0.601/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai/wrappers.py` & `literalai-0.0.601/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.600/literalai.egg-info/SOURCES.txt` & `literalai-0.0.601/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

