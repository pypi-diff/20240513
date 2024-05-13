# Comparing `tmp/messages_local-0.0.50.tar.gz` & `tmp/messages_local-0.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "messages_local-0.0.50.tar", last modified: Wed May  8 02:10:14 2024, max compression
+gzip compressed data, was "messages_local-0.0.51.tar", last modified: Mon May 13 14:11:50 2024, max compression
```

## Comparing `messages_local-0.0.50.tar` & `messages_local-0.0.51.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.658078 messages_local-0.0.50/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 02:10:14.658078 messages_local-0.0.50/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-08 02:09:35.000000 messages_local-0.0.50/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-08 02:09:35.000000 messages_local-0.0.50/messages_local/src/MessagesLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 02:09:35.000000 messages_local-0.0.50/messages_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 02:10:14.654078 messages_local-0.0.50/messages_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-08 02:10:14.000000 messages_local-0.0.50/messages_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-08 02:09:35.000000 messages_local-0.0.50/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 02:10:14.658078 messages_local-0.0.50/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-08 02:09:35.000000 messages_local-0.0.50/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 14:11:50.206893 messages_local-0.0.51/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 14:11:20.000000 messages_local-0.0.51/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.202893 messages_local-0.0.51/messages_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/messages_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-05-13 14:11:20.000000 messages_local-0.0.51/messages_local/src/MessagesLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:20.000000 messages_local-0.0.51/messages_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:11:50.206893 messages_local-0.0.51/messages_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 14:11:50.000000 messages_local-0.0.51/messages_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-13 14:11:20.000000 messages_local-0.0.51/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:11:50.206893 messages_local-0.0.51/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-13 14:11:20.000000 messages_local-0.0.51/setup.py
```

### Comparing `messages_local-0.0.50/PKG-INFO` & `messages_local-0.0.51/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.50
+Version: 0.0.51
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.4
 Requires-Dist: message-local>=0.0.121
 Requires-Dist: whatsapp-message-vonage-local>=0.0.19
-Requires-Dist: whataspp-inforu-local>=0.0.12
+Requires-Dist: whataspp-message-inforu-local>=0.0.12
 Requires-Dist: sms-message-aws-sns-local>=0.0.35
 Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.50/README.md` & `messages_local-0.0.51/README.md`

 * *Files identical despite different names*

### Comparing `messages_local-0.0.50/messages_local/src/MessagesLocal.py` & `messages_local-0.0.51/messages_local/src/MessagesLocal.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     INFORU_MESSAGE_PROVIDER_ID, VONAGE_MESSAGE_PROVIDER_ID)
 from message_local.MessageChannels import MessageChannel
 from message_local.MessageImportance import MessageImportance
 from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
 from queue_worker_local.queue_worker import QueueWorker
 from sms_message_aws_sns_local.sms_message_aws_sns import SmsMessageAwsSnsLocal
-from whataspp_inforu_local.WhatsAppMessageInforuLocal import WhatsAppMessageInforuLocal
+from whataspp_message_inforu_local.WhatsAppMessageInforuLocal import WhatsAppMessageInforuLocal
 from whatsapp_message_vonage_local.vonage_whatsapp_message_local import WhatsAppMessageVonageLocal
 
 # TODO Replace Magic Number with enum in a separate file in this repo which will be created by Sql2Code in the future
 MESSAGES_API_TYPE_ID = 5
 # TODO What is this action?
 SEND_SYNC_ACTION_ID = 15
 MESSAGE_LOCAL_PYTHON_COMPONENT_ID = 259
@@ -51,15 +51,15 @@
         self.is_test_data = is_test_data
         self.label_crud = LabelsMessageLocal()
         self.queue_worker = None  # This is called by the queue worker, so we can't init it here
 
     def get_queue_worker(self):
         self.queue_worker = self.queue_worker or QueueWorker(schema_name="message", table_name="message_table",
                                                              view_name="message_outbox_view",
-                                                             id_column_name="message_id",
+                                                             column_name="message_id",
                                                              is_test_data=self.is_test_data)
         return self.queue_worker
 
     @staticmethod
     def __send(recipient: Recipient, message_local: MessageLocal, importance: MessageImportance,
                campaign_id: int) -> list[int]:
         message_recipient_channel = message_local.get_message_channel(recipient)
@@ -88,32 +88,32 @@
             init_kwargs = {"subject": message_local.get_subject_text_after_template_processing(recipient)}
             message_local.__class__ = EmailMessageAwsSesLocal
 
         else:
             # TODO We need to add to the message Recipient country, message plain text length after template,
             #  message HTML length after template, number of attachments, attachments' types and sizes.
             compound_message_dict = message_local.get_compound_message_dict()
-            data_json = {"channel_id": message_recipient_channel,
+            data_dict = {"channel_id": message_recipient_channel,
                          "provider_id": message_recipient_provider_id,
                          "recipient": recipient,
                          "compound_message_dict": compound_message_dict,
                          "compound_message_length": len(compound_message_dict),
                          "importance": importance,
                          "campaign_id": campaign_id
                          }
-            error_message = "Don't know which MessageLocal class to use." + " Data: " + str(data_json)
-            # data_json will be printed anyway, as the meta logger prints the object & local variables
+            error_message = "Don't know which MessageLocal class to use." + " Data: " + str(data_dict)
+            # data_dict will be printed anyway, as the meta logger prints the object & local variables
             raise Exception(error_message)
 
         message_local.__init__(**init_kwargs)
         return message_local.send(**send_kwargs)
 
     # This method should be used by Queue Worker
     # Make sure send_sync has all the parameters in the function_parameters_json below
-    def send_sync(self, message_id: int, campaign_id: int,
+    def send_sync(self, *, campaign_id: int = None, message_id: int = None,
                   recipients: List[dict] = None,
                   cc_recipients: List[dict] = None,
                   bcc_recipients: List[dict] = None,
                   request_datetime: str = None,
                   # TODO What is exactly the operational meaning of start_timestamp?
                   #  There is start_timestamp, when the message can be sent?
                   start_timestamp: datetime = datetime.now(),
```

### Comparing `messages_local-0.0.50/messages_local.egg-info/PKG-INFO` & `messages_local-0.0.51/messages_local.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: messages-local
-Version: 0.0.50
+Version: 0.0.51
 Home-page: https://github.com/circles-zone/messages-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: item-local>=0.0.9
 Requires-Dist: queue-worker-local>=0.0.37
 Requires-Dist: label-message-local>=0.0.4
 Requires-Dist: message-local>=0.0.121
 Requires-Dist: whatsapp-message-vonage-local>=0.0.19
-Requires-Dist: whataspp-inforu-local>=0.0.12
+Requires-Dist: whataspp-message-inforu-local>=0.0.12
 Requires-Dist: sms-message-aws-sns-local>=0.0.35
 Requires-Dist: email-message-aws-ses-local>=0.0.13
 
 messages-local
```

### Comparing `messages_local-0.0.50/setup.py` & `messages_local-0.0.51/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "messages-local"
 
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.50',  # https://pypi.org/project/messages-local
+    version='0.0.51',  # https://pypi.org/project/messages-local
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="messages-local",
@@ -22,12 +22,12 @@
     ],
     install_requires=[
         "item-local>=0.0.9",
         "queue-worker-local>=0.0.37",
         "label-message-local>=0.0.4",
         "message-local>=0.0.121",
         "whatsapp-message-vonage-local>=0.0.19",
-        "whataspp-inforu-local>=0.0.12",
+        "whataspp-message-inforu-local>=0.0.12",
         "sms-message-aws-sns-local>=0.0.35",
         "email-message-aws-ses-local>=0.0.13"
     ]
 )
```

