# Comparing `tmp/django-df-notifications-1.2.8.tar.gz` & `tmp/django-df-notifications-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-df-notifications-1.2.8.tar", last modified: Tue Dec 19 16:03:47 2023, max compression
+gzip compressed data, was "django-df-notifications-1.2.9.tar", last modified: Fri Dec 22 14:06:54 2023, max compression
```

## Comparing `django-df-notifications-1.2.8.tar` & `django-df-notifications-1.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:47.105135 django-df-notifications-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-12-19 16:03:47.101135 django-df-notifications-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:47.097135 django-df-notifications-1.2.8/df_notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/channels.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/context_processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:47.097135 django-df-notifications-1.2.8/df_notifications/drf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/drf/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:47.101135 django-df-notifications-1.2.8/df_notifications/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0004_pushactioncategory_pushaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0005_alter_pushactioncategory_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0006_alter_userdevice_registration_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0007_custompushmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/0008_alter_custompushmessage_action_url_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/df_notifications/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 16:03:47.101135 django-df-notifications-1.2.8/django_df_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-12-19 16:03:47.000000 django-df-notifications-1.2.8/django_df_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-19 16:03:47.000000 django-df-notifications-1.2.8/django_df_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 16:03:47.000000 django-df-notifications-1.2.8/django_df_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-19 16:03:47.000000 django-df-notifications-1.2.8/django_df_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-19 16:03:47.000000 django-df-notifications-1.2.8/django_df_notifications.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 16:03:47.105135 django-df-notifications-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-19 16:03:37.000000 django-df-notifications-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:54.662034 django-df-notifications-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-12-22 14:06:54.662034 django-df-notifications-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:54.658034 django-df-notifications-1.2.9/df_notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/context_processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:54.658034 django-df-notifications-1.2.9/df_notifications/drf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/drf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:54.658034 django-df-notifications-1.2.9/df_notifications/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0004_pushactioncategory_pushaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0005_alter_pushactioncategory_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0006_alter_userdevice_registration_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0007_custompushmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/0008_alter_custompushmessage_action_url_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/df_notifications/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-22 14:06:54.662034 django-df-notifications-1.2.9/django_df_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2023-12-22 14:06:54.000000 django-df-notifications-1.2.9/django_df_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-22 14:06:54.000000 django-df-notifications-1.2.9/django_df_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-22 14:06:54.000000 django-df-notifications-1.2.9/django_df_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2023-12-22 14:06:54.000000 django-df-notifications-1.2.9/django_df_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-22 14:06:54.000000 django-df-notifications-1.2.9/django_df_notifications.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 14:06:54.662034 django-df-notifications-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-22 14:06:46.000000 django-df-notifications-1.2.9/setup.py
```

### Comparing `django-df-notifications-1.2.8/LICENSE` & `django-df-notifications-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/PKG-INFO` & `django-df-notifications-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-notifications
-Version: 1.2.8
+Version: 1.2.9
 Summary: Opinionated Django Omnichannel Notifications.
 Author-email: Apexive OSS <open-source@apexive.com>
 Project-URL: homepage, https://apexive.com/
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: djangorestframework
-Requires-Dist: django-df-api-drf
+Requires-Dist: django-df-api-drf>=1.0.3
 Requires-Dist: firebase_admin
 Requires-Dist: requests
 Requires-Dist: django_slack
 Requires-Dist: fcm_django>=1.0.15
 Requires-Dist: celery
 Requires-Dist: django-import-export
 Requires-Dist: django-celery-beat
```

### Comparing `django-df-notifications-1.2.8/README.md` & `django-df-notifications-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/admin.py` & `django-df-notifications-1.2.9/df_notifications/admin.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/channels.py` & `django-df-notifications-1.2.9/df_notifications/channels.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import json
 import logging
 from typing import Dict, Iterable
 
 import requests
+from df_api_drf.resolvers import site_url
 from django.core.mail import EmailMultiAlternatives
 from django.utils import timezone
 from django_slack import slack_message
 from firebase_admin.firestore import client
-from firebase_admin.messaging import Message, Notification
+from firebase_admin.messaging import (
+    Message,
+    Notification,
+    WebpushConfig,
+    WebpushFCMOptions,
+)
 from otp_twilio.models import TwilioSMSDevice
 
 
 class BaseChannel:
     template_parts = ["subject.txt", "body.txt", "body.html", "data.json"]
 
     def send(self, users: Iterable, context: Dict[str, str]) -> None:
@@ -50,25 +56,34 @@
         try:
             devices = context["devices_queryset"]
         except KeyError:
             from df_notifications.models import UserDevice
 
             devices = UserDevice.objects.all()
 
-        data = json.loads(context["data.json"])
-        devices.filter(user__in=users).send_message(
-            Message(
+        if users:
+            data = json.loads(context["data.json"])
+            message = Message(
                 notification=Notification(
                     title=context["subject.txt"],
                     body=context["body.txt"],
                     image=data.get("image"),
                 ),
                 data=data,
-            ),
-        )
+            )
+            if action_url := data.get("action_url"):
+                message.webpush = WebpushConfig(
+                    fcm_options=WebpushFCMOptions(
+                        link=site_url(
+                            user=next(iter(users)),
+                        )
+                        + action_url
+                    )
+                )
+            devices.filter(user__in=users).send_message(message)
 
 
 class JSONPostWebhookChannel(BaseChannel):
     template_parts = ["subject.txt", "body.txt", "data.json"]
 
     def send(self, users: Iterable, context: Dict[str, str]) -> None:
         requests.post(
```

### Comparing `django-df-notifications-1.2.8/df_notifications/decorators.py` & `django-df-notifications-1.2.9/df_notifications/decorators.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/drf/serializers.py` & `django-df-notifications-1.2.9/df_notifications/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/drf/viewsets.py` & `django-df-notifications-1.2.9/df_notifications/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0001_initial.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0002_remove_notificationhistory_df_notifica_templat_fc63aa_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0003_remove_notificationhistory_df_notifica_templat_ec4b48_idx_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0004_pushactioncategory_pushaction.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0004_pushactioncategory_pushaction.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0007_custompushmessage.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0007_custompushmessage.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/migrations/0008_alter_custompushmessage_action_url_and_more.py` & `django-df-notifications-1.2.9/df_notifications/migrations/0008_alter_custompushmessage_action_url_and_more.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/models.py` & `django-df-notifications-1.2.9/df_notifications/models.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/settings.py` & `django-df-notifications-1.2.9/df_notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/df_notifications/tasks.py` & `django-df-notifications-1.2.9/df_notifications/tasks.py`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/django_df_notifications.egg-info/PKG-INFO` & `django-df-notifications-1.2.9/django_df_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-notifications
-Version: 1.2.8
+Version: 1.2.9
 Summary: Opinionated Django Omnichannel Notifications.
 Author-email: Apexive OSS <open-source@apexive.com>
 Project-URL: homepage, https://apexive.com/
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django
 Requires-Dist: djangorestframework
-Requires-Dist: django-df-api-drf
+Requires-Dist: django-df-api-drf>=1.0.3
 Requires-Dist: firebase_admin
 Requires-Dist: requests
 Requires-Dist: django_slack
 Requires-Dist: fcm_django>=1.0.15
 Requires-Dist: celery
 Requires-Dist: django-import-export
 Requires-Dist: django-celery-beat
```

### Comparing `django-df-notifications-1.2.8/django_df_notifications.egg-info/SOURCES.txt` & `django-df-notifications-1.2.9/django_df_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-df-notifications-1.2.8/pyproject.toml` & `django-df-notifications-1.2.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "django-df-notifications"
 description = "Opinionated Django Omnichannel Notifications."
 readme = "README.md"
-version = "1.2.8"
+version = "1.2.9"
 authors = [
     { name = "Apexive OSS", email = "open-source@apexive.com" },
 ]
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 3.2",
@@ -23,15 +23,15 @@
 ]
 requires-python = ">=3.9"
 urls = { homepage = "https://apexive.com/" }
 
 dependencies = [
     "django",
     "djangorestframework",
-    "django-df-api-drf",
+    "django-df-api-drf>=1.0.3",
     "firebase_admin",
     "requests",
     "django_slack",
     "fcm_django>=1.0.15",
     "celery",
     "django-import-export",
     "django-celery-beat",
```

