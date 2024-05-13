# Comparing `tmp/messages_local-0.0.51.tar.gz` & `tmp/messages_local-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.51.tar", last modified: Mon May 13 14:11:50 2024, max compression
+gzip compressed data, was "messages_local-0.0.52.tar", last modified: Mon May 13 20:23:42 2024, max compression
```

## Comparing `messages_local-0.0.51.tar` & `messages_local-0.0.52.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 14:11:50.206893 messages_local-0.0.51/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 14:11:20.000000 messages_local-0.0.51/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.202893 messages_local-0.0.51/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-05-13 14:11:20.000000 messages_local-0.0.51/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:20.000000 messages_local-0.0.51/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 14:11:20.000000 messages_local-0.0.51/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:11:50.206893 messages_local-0.0.51/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-13 14:11:20.000000 messages_local-0.0.51/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:42.578269 messages_local-0.0.52/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 20:23:42.578269 messages_local-0.0.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 20:23:06.000000 messages_local-0.0.52/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:42.574269 messages_local-0.0.52/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:42.578269 messages_local-0.0.52/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12237 2024-05-13 20:23:06.000000 messages_local-0.0.52/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:06.000000 messages_local-0.0.52/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:23:42.578269 messages_local-0.0.52/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 20:23:42.000000 messages_local-0.0.52/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 20:23:42.000000 messages_local-0.0.52/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:23:42.000000 messages_local-0.0.52/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 20:23:42.000000 messages_local-0.0.52/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 20:23:42.000000 messages_local-0.0.52/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 20:23:06.000000 messages_local-0.0.52/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:23:42.578269 messages_local-0.0.52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-13 20:23:06.000000 messages_local-0.0.52/setup.py
```

### Comparing `messages_local-0.0.51/PKG-INFO` & `messages_local-0.0.52/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.51
+Version: 0.0.52
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.51/README.md` & `messages_local-0.0.52/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.51/messages_local/src/MessagesLocal.py` & `messages_local-0.0.52/messages_local/src/MessagesLocal.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,21 +46,20 @@
         self.recipients = recipients
 
         self.default_original_body = default_original_body
         self.default_subject = default_subject
         self.default_importance = default_importance
         self.is_test_data = is_test_data
         self.label_crud = LabelsMessageLocal()
-        self.queue_worker = None  # This is called by the queue worker, so we can't init it here
+        self.queue_worker = None  # This is called by the queue worker, so we can't initiate it here
 
     def get_queue_worker(self):
-        self.queue_worker = self.queue_worker or QueueWorker(schema_name="message", table_name="message_table",
-                                                             view_name="message_outbox_view",
-                                                             column_name="message_id",
-                                                             is_test_data=self.is_test_data)
+        self.queue_worker = self.queue_worker or QueueWorker(
+            schema_name="message", table_name="message_table", view_name="message_outbox_view",
+            queue_item_id_column_name="message_id", is_test_data=self.is_test_data)
         return self.queue_worker
 
     @staticmethod
     def __send(recipient: Recipient, message_local: MessageLocal, importance: MessageImportance,
                campaign_id: int) -> list[int]:
         message_recipient_channel = message_local.get_message_channel(recipient)
         message_recipient_provider_id = message_local.get_message_provider_id(message_recipient_channel, recipient)
@@ -134,24 +133,20 @@
                                      sender_profile_id=sender_profile_id,
                                      is_test_data=self.is_test_data)
         for recipient in recipients:
             self.__send(recipient, message_local, importance, campaign_id)
             # TODO: should we send to multiple recipients outside this loop?
 
     # This method will push the messages to the queue in message_outbox_table
-    def send_scheduled(self, campaign_id: int = None, message_template_id: int = None,
-                       recipients: List[Recipient] = None,
-                       cc_recipients: List[Recipient] = None,
-                       bcc_recipients: List[Recipient] = None,
-                       request_datetime: datetime = None,
-                       importance: MessageImportance = None,
-                       requested_message_type: MessageChannel = None,
-                       start_timestamp: datetime = datetime.now(),
-                       sender_profile_id: int = None,
-                       is_require_moderator: bool = True) -> list[int]:
+    def send_scheduled(
+            self, *, campaign_id: int = None, message_template_id: int = None, is_require_moderator: bool = True,
+            recipients: List[Recipient] = None, cc_recipients: List[Recipient] = None,
+            bcc_recipients: List[Recipient] = None, request_datetime: datetime = None,
+            importance: MessageImportance = None, requested_message_type: MessageChannel = None,
+            start_timestamp: datetime = datetime.now(), sender_profile_id: int = None,) -> list[int]:
         """The message will be sent any time between start_timestamp and end_timestamp
         For every bcc_recipient, a message will be pushed to the queue with the same parameters
         (message_id per bcc_recipient, or one if none provided)
         """
         importance = importance or MessageImportance(self.default_importance)
         recipients = recipients or [Recipient(**recipient) for recipient in self.recipients]
         message_ids = []
```

### Comparing `messages_local-0.0.51/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.52/messages_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.51
+Version: 0.0.52
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `messages_local-0.0.51/setup.py` & `messages_local-0.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.51',  # https://pypi.org/project/messages-local
+    version='0.0.52',  # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
```

