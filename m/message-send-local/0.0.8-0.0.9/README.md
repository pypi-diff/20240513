# Comparing `tmp/message-send-local-0.0.8.tar.gz` & `tmp/message-send-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "message-send-local-0.0.8.tar", last modified: Sun Dec 31 21:18:39 2023, max compression
+gzip compressed data, was "message-send-local-0.0.9.tar", last modified: Wed Jan  3 16:43:48 2024, max compression
```

## Comparing `message-send-local-0.0.8.tar` & `message-send-local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 21:18:39.408015 message-send-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-31 21:18:39.408015 message-send-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-31 21:18:04.000000 message-send-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 21:18:39.408015 message-send-local-0.0.8/message_send_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2023-12-31 21:18:39.000000 message-send-local-0.0.8/message_send_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-31 21:18:39.000000 message-send-local-0.0.8/message_send_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 21:18:39.000000 message-send-local-0.0.8/message_send_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-31 21:18:39.000000 message-send-local-0.0.8/message_send_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-31 21:18:39.000000 message-send-local-0.0.8/message_send_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 21:18:39.404015 message-send-local-0.0.8/message_send_platform_invitation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 21:18:39.404015 message-send-local-0.0.8/message_send_platform_invitation/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-31 21:18:04.000000 message-send-local-0.0.8/message_send_platform_invitation/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2023-12-31 21:18:04.000000 message-send-local-0.0.8/message_send_platform_invitation/src/campaign_message_send.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-12-31 21:18:04.000000 message-send-local-0.0.8/message_send_platform_invitation/src/country_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-31 21:18:04.000000 message-send-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 21:18:39.408015 message-send-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-12-31 21:18:04.000000 message-send-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:43:48.224810 message-send-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-03 16:43:48.224810 message-send-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-01-03 16:43:04.000000 message-send-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:43:48.224810 message-send-local-0.0.9/message_send_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-03 16:43:48.000000 message-send-local-0.0.9/message_send_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-03 16:43:48.000000 message-send-local-0.0.9/message_send_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 16:43:48.000000 message-send-local-0.0.9/message_send_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-03 16:43:48.000000 message-send-local-0.0.9/message_send_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-03 16:43:48.000000 message-send-local-0.0.9/message_send_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:43:48.220810 message-send-local-0.0.9/message_send_platform_invitation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 16:43:48.224810 message-send-local-0.0.9/message_send_platform_invitation/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-03 16:43:04.000000 message-send-local-0.0.9/message_send_platform_invitation/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-01-03 16:43:04.000000 message-send-local-0.0.9/message_send_platform_invitation/src/campaign_message_send.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-01-03 16:43:04.000000 message-send-local-0.0.9/message_send_platform_invitation/src/country_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-03 16:43:04.000000 message-send-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 16:43:48.224810 message-send-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-03 16:43:04.000000 message-send-local-0.0.9/setup.py
```

### Comparing `message-send-local-0.0.8/PKG-INFO` & `message-send-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-send-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles message_send_platform_invitation Python
 Home-page: https://github.com/circles-zone/message-send-platform-invitation-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `message-send-local-0.0.8/README.md` & `message-send-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `message-send-local-0.0.8/message_send_local.egg-info/PKG-INFO` & `message-send-local-0.0.9/message_send_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: message-send-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles message_send_platform_invitation Python
 Home-page: https://github.com/circles-zone/message-send-platform-invitation-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `message-send-local-0.0.8/message_send_platform_invitation/src/campaign_message_send.py` & `message-send-local-0.0.9/message_send_platform_invitation/src/campaign_message_send.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """imports"""
 from typing import List
+from datetime import datetime
 
 from circles_local_database_python.connector import Connector
 from circles_local_database_python.generic_crud_ml import GenericCRUDML
 from logger_local.Logger import Logger
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from message_local.Recipient import Recipient
 from messages_local.MessagesLocal import MessagesLocal
+from variable_local.message_template import MessageTemplate
 
 MESSAGE_SEND_PLATFORM_INVITATION_LOCAL_PYTHON_COMPONENT_ID = 243
 MESSAGE_SEND_PLATFORM_INVITATION_LOCAL_PYTHON_COMPONENT_COMPONENT_NAME = "message-send-platform-invitation-local-python"
 DEVELOPER_EMAIL = 'jenya.b@circ.zone'
 object1 = {
     'component_id': MESSAGE_SEND_PLATFORM_INVITATION_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': MESSAGE_SEND_PLATFORM_INVITATION_LOCAL_PYTHON_COMPONENT_COMPONENT_NAME,
@@ -21,14 +23,16 @@
 
 
 class CampaignMessageSend(GenericCRUDML):
     """Message send platform class"""
 
     def __init__(self, schema_name="message", connection: Connector = None) -> None:
         super().__init__(default_schema_name=schema_name, connection=connection)
+        self.message_template = MessageTemplate()
+        self.messages_local = MessagesLocal()
 
     def __get_potential_person_list_by_campaign_id_limit(self, campaign_id: int,
                                                          recipient_limit: int = 100) -> List[Recipient]:
         """return list of person id """
         logger.start(f"get potential person list by campaign id={campaign_id}")
 
         recipient_limit_left = recipient_limit
@@ -48,38 +52,30 @@
         self.cursor.execute(query_for_relevant_criteria_for_campaign, (campaign_id,))
         results = []
         for row in self.cursor.fetchall():
             min_age, max_age, gender_list_id, group_list_id, minimal_days = row
             logger.info(object={"min_age": min_age, "max_age": max_age, "gender_list_id": gender_list_id,
                                 "group_list_id": group_list_id, "minimal_days": minimal_days})
             # profile_id didn't receive messages from this campaign for campaign.minimal_days
-            where = ("""user.profile_id NOT IN (
+            criteria_json = {"min_age": min_age, "max_age": max_age, "gender_list_id": gender_list_id,
+                             "group_list_id": group_list_id, "minimal_days": minimal_days}
+            where = self.message_template.get_where_by_criteria(criteria_json)
+            where += (""" AND user.profile_id NOT IN (
                        SELECT user.profile_id FROM message.message_outbox_view 
                            WHERE campaign_id = %s AND updated_timestamp >= NOW() - INTERVAL %s DAY
                        )"""
-                     )
-            if min_age is not None:
-                where += f" AND TIMESTAMPDIFF(YEAR, person_birthday_date, CURDATE()) >= {min_age}"
-            if max_age is not None:
-                where += f" AND TIMESTAMPDIFF(YEAR, person_birthday_date, CURDATE()) <= {max_age}"
-
-            if gender_list_id is not None:
-                where += " AND profile_gender_id " + self.sql_in_list_by_entity_list_id(
-                    schema_name="profile", entity_name="gender", entity_list_id=gender_list_id)
-
-            if group_list_id is not None:
-                where += " AND group_profile.group_id " + self.sql_in_list_by_entity_list_id(
-                    schema_name="`group`", entity_name="group", entity_list_id=group_list_id)
+                      )
 
             query_for_potentials_receipients = f"""
                 SELECT DISTINCT user_id, person_id, user_main_email, user.profile_id, 
                    profile_phone_full_number_normalized, profile_preferred_lang_code
                  FROM user.user_general_view AS user
-                    JOIN group_profile.group_profile_table AS group_profile on group_profile.profile_id = user.profile_id
-                  WHERE {where} LIMIT {recipient_limit_left}
+                    JOIN group_profile.group_profile_table AS group_profile 
+                        on group_profile.profile_id = user.profile_id
+                  WHERE {where} LIMIT 1
                 """
             logger.info(object={"query_for_potentials_receipients": query_for_potentials_receipients,
                                 "campaign_id": campaign_id, "minimal_days": minimal_days})
 
             self.cursor.execute(query_for_potentials_receipients, (campaign_id, minimal_days))
 
             recieved_results = self.cursor.fetchall()
@@ -123,36 +119,52 @@
         invitations_sent_in_the_last_24_hours = int(self.__get_number_of_invitations_sent_in_the_last_24_hours(
             campaign_id) * additional_invitations_multiplier + additional_invitations_amount)
         logger.end(f"number_of_invitations_to_send={invitations_sent_in_the_last_24_hours}")
         return invitations_sent_in_the_last_24_hours
 
     def send_message_by_campaign_id(self, campaign_id: int,
                                     additional_invitations_multiplier: float = 1.01,
-                                    additional_invitations_amount: int = 1) -> None:
+                                    additional_invitations_amount: int = 1,
+                                    request_datetime: datetime = None,
+                                    requested_message_type: int = None,
+                                    importance=None) -> list[int]:
         logger.start(object={"campaign_id": campaign_id,
                              "additional_invitations_multiplier": additional_invitations_multiplier,
                              "additional_invitations_amount": additional_invitations_amount})
         count = self.__get_number_of_invitations_to_send_by_campain_id_multiplier(
             campaign_id=campaign_id,
             additional_invitations_multiplier=additional_invitations_multiplier,
             additional_invitations_amount=additional_invitations_amount)
         person_list = self.__get_potential_person_list_by_campaign_id_limit(campaign_id, count)
-        query = """
-            SELECT campaign_table.message_template_id, message_template.message_template_ml_table.sms_body_template
-            FROM campaign.campaign_table JOIN message_template.message_template_ml_table
-                ON campaign_table.message_template_id = message_template_ml_table.message_template_id
-            WHERE campaign_table.campaign_id = %s
-        """
-        self.cursor.execute(query, (campaign_id,))
-        text_template = self.cursor.fetchall()
+
+        logger.info(object={"person_list": person_list})
+        # query = """
+        #     SELECT campaign_table.message_template_id, message_template.message_template_ml_table.sms_body_template
+        #     FROM campaign.campaign_table JOIN message_template.message_template_ml_table
+        #         ON campaign_table.message_template_id = message_template_ml_table.message_template_id
+        #     WHERE campaign_table.campaign_id = %s
+        # """
+        # self.cursor.execute(query, (campaign_id,))
+        # text_template = self.cursor.fetchall()
         #  we have to call the constructor every time, as the work related to body/recipients is done there,
         #  and we have new body & recipients per campaign
-        return_value = MessagesLocal().send_scheduled(to_recipients=person_list, original_body=text_template,
-                                                      campaign_id=campaign_id)
-        logger.end(object={"return_value": return_value})
+
+        # message_dict contains a list of dicts, each with the following keys:
+        # ["sms_body_template", "email_subject_template", "email_body_html_template",
+        # "whatsapp_body_template", "question_id", "question_type_id", "question_title", "question_type_name"]
+
+        message_ids = self.messages_local.send_scheduled(
+            to_recipients=person_list,
+            request_datetime=request_datetime,
+            importance=importance,
+            campaign_id=campaign_id,
+            requested_message_type=requested_message_type
+        )
+        logger.end(object={"message_ids": message_ids})
+        return message_ids
 
     def send_to_all_campaigns(self, additional_invitations_multiplier: float = 1.01,
                               additional_invitations_amount: int = 1) -> None:
         """send to all campaigns"""
         logger.start(object={"additional_invitations_multiplier": additional_invitations_multiplier,
                              "additional_invitations_amount": additional_invitations_amount})
         self.cursor.execute("SELECT campaign_id FROM campaign.campaign_table WHERE NOW() >= start_timestamp "
```

### Comparing `message-send-local-0.0.8/message_send_platform_invitation/src/country_constants.py` & `message-send-local-0.0.9/message_send_platform_invitation/src/country_constants.py`

 * *Files identical despite different names*

### Comparing `message-send-local-0.0.8/pyproject.toml` & `message-send-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `message-send-local-0.0.8/setup.py` & `message-send-local-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 PACKAGE_NAME = "message-send-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = "message_send_platform_invitation"
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',  # https://pypi.org/project/message-send-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles message_send_platform_invitation Python",
     long_description="PyPI Package for Circles message_send_platform_invitation Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/message-send-platform-invitation-local-python-package",
     packages=[package_dir],
```

