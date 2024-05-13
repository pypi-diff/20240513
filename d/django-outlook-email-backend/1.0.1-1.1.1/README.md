# Comparing `tmp/django_outlook_email_backend-1.0.1.tar.gz` & `tmp/django_outlook_email_backend-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-1.0.1.tar", last modified: Wed May  1 13:32:50 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.1.1.tar", last modified: Mon May 13 12:26:59 2024, max compression
```

## Comparing `django_outlook_email_backend-1.0.1.tar` & `django_outlook_email_backend-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:50.038606 django_outlook_email_backend-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-01 13:32:50.038606 django_outlook_email_backend-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:50.034605 django_outlook_email_backend-1.0.1/django_outlook_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/django_outlook_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/django_outlook_email/django_outlook_email_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:50.034605 django_outlook_email_backend-1.0.1/django_outlook_email/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/django_outlook_email/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/django_outlook_email/exceptions/microsoft_graph_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:32:50.038606 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-01 13:32:50.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-01 13:32:50.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:32:50.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 13:32:50.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 13:32:50.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:32:49.000000 django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:32:50.038606 django_outlook_email_backend-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-01 13:32:46.000000 django_outlook_email_backend-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:59.650758 django_outlook_email_backend-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-13 12:26:59.650758 django_outlook_email_backend-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:59.646758 django_outlook_email_backend-1.1.1/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:59.646758 django_outlook_email_backend-1.1.1/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:59.646758 django_outlook_email_backend-1.1.1/django_outlook_email/senders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/senders/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/senders/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/senders/json_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/django_outlook_email/senders/mime_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 12:26:59.650758 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 12:26:59.000000 django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 12:26:59.650758 django_outlook_email_backend-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 12:26:55.000000 django_outlook_email_backend-1.1.1/setup.py
```

### Comparing `django_outlook_email_backend-1.0.1/PKG-INFO` & `django_outlook_email_backend-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.0.1
+Version: 1.1.1
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests~=2.25
 Requires-Dist: msal==1.*
 
 # Django outlook email backend
 ### Outlook api email backend for Django
 
 ## Requirements
@@ -25,21 +26,26 @@
 - Django 5.0, 4.2
 
 ## Installation
 Install using pip...
 ```commandline
 pip install django-outlook-email-backend
 ```
-Add  `'OUTLOOK_CREDENTIALS'` in `'settings.py'`  
+Add  `'OUTLOOK_CREDENTIALS'` in `settings.py`  
 ```python
 OUTLOOK_CREDENTIALS = {
     'OUTLOOK_CLIENT_ID': "XXXXX",
     'OUTLOOK_CLIENT_SECRET': "XXXXX",
     'OUTLOOK_TENANT_ID': "XXXXX",
 }
 ```
 
-Add  `'EMAIL_BACKEND'` in `'settings.py'`  
+Add  `'EMAIL_BACKEND'` in `settings.py`  
 
 ```python
 EMAIL_BACKEND = "django_outlook_email.django_outlook_email_backend.OutlookEmailBackend"
 ``` 
+
+if you want to use json instead of mime the add the following line in in `settings.py`
+```python
+OUTLOOK_CREDENTIALS["OUTLOOK_SEND_FORMAT"] = "json"
+```
```

### Comparing `django_outlook_email_backend-1.0.1/django_outlook_email/django_outlook_email_backend.py` & `django_outlook_email_backend-1.1.1/django_outlook_email/django_outlook_email_backend.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 import msal
 import requests
 from django.core.mail.message import sanitize_address
 from django.conf import settings
 from django.core.mail.backends.base import BaseEmailBackend
 
 from django_outlook_email.exceptions.microsoft_graph_exceptions import MicrosoftGraphException
+from django_outlook_email.senders.json_sender import JsonSender
+from django_outlook_email.senders.mime_sender import MimeSender
 
 
 class OutlookEmailBackend(BaseEmailBackend):
 
     access_token = None
     client_id = settings.OUTLOOK_CREDENTIALS["OUTLOOK_CLIENT_ID"]
     client_secret = settings.OUTLOOK_CREDENTIALS["OUTLOOK_CLIENT_SECRET"]
     tenant_id = settings.OUTLOOK_CREDENTIALS["OUTLOOK_TENANT_ID"]
+    send_format = settings.OUTLOOK_CREDENTIALS.get("OUTLOOK_SEND_FORMAT")
 
 
     def send_messages(self, email_messages):
         self._set_access_token()
         if not email_messages:
             return 0
         num_sent = 0
@@ -39,34 +42,13 @@
             scopes=["https://graph.microsoft.com/.default"]
         )
 
         self.access_token = result["access_token"]
 
 
     def _send(self, email_message):
-        if not email_message.recipients():
-            return False
-        encoding = email_message.encoding or settings.DEFAULT_CHARSET
-        from_email = sanitize_address(email_message.from_email, encoding)
-
-        message = email_message.message()
-
-        try:
-            response = requests.post(
-                "https://graph.microsoft.com/v1.0/users/"+from_email+"/sendMail",
-                data=base64.b64encode(message.as_bytes(linesep="\r\n")),
-
-                headers={"Authorization": "Bearer " + self.access_token, "Content-type": "text/plain"}
-            )
-        except requests.exceptions.RequestException:
-            if not self.fail_silently:
-                raise
-            return False
-
-        if response.status_code == 202:
-            return True
+        if self.send_format == "json":
+            sender = JsonSender(self.access_token, self.fail_silently)
         else:
-            if not self.fail_silently:
-                raise MicrosoftGraphException(response.status_code, response.content)
-            return False
-
+            sender = MimeSender(self.access_token, self.fail_silently)
+        sender.send(email_message)
```

### Comparing `django_outlook_email_backend-1.0.1/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-1.1.1/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.0.1
+Version: 1.1.1
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: requests~=2.25
 Requires-Dist: msal==1.*
 
 # Django outlook email backend
 ### Outlook api email backend for Django
 
 ## Requirements
@@ -25,21 +26,26 @@
 - Django 5.0, 4.2
 
 ## Installation
 Install using pip...
 ```commandline
 pip install django-outlook-email-backend
 ```
-Add  `'OUTLOOK_CREDENTIALS'` in `'settings.py'`  
+Add  `'OUTLOOK_CREDENTIALS'` in `settings.py`  
 ```python
 OUTLOOK_CREDENTIALS = {
     'OUTLOOK_CLIENT_ID': "XXXXX",
     'OUTLOOK_CLIENT_SECRET': "XXXXX",
     'OUTLOOK_TENANT_ID': "XXXXX",
 }
 ```
 
-Add  `'EMAIL_BACKEND'` in `'settings.py'`  
+Add  `'EMAIL_BACKEND'` in `settings.py`  
 
 ```python
 EMAIL_BACKEND = "django_outlook_email.django_outlook_email_backend.OutlookEmailBackend"
 ``` 
+
+if you want to use json instead of mime the add the following line in in `settings.py`
+```python
+OUTLOOK_CREDENTIALS["OUTLOOK_SEND_FORMAT"] = "json"
+```
```

### Comparing `django_outlook_email_backend-1.0.1/setup.py` & `django_outlook_email_backend-1.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django_outlook_email-backend',
-    version='1.0.1',
+    version='1.1.1',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
@@ -16,10 +16,10 @@
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     url='https://github.com/enley-es/django-outlook-email-backend',
-    packages=["django_outlook_email","django_outlook_email.exceptions"],
+    packages=["django_outlook_email","django_outlook_email.exceptions", "django_outlook_email.senders"],
     install_requires = ['requests~=2.25', 'msal==1.*']
 )
```

