# Comparing `tmp/django_outlook_email_backend-1.1.3.tar.gz` & `tmp/django_outlook_email_backend-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_outlook_email_backend-1.1.3.tar", last modified: Mon May 13 14:40:42 2024, max compression
+gzip compressed data, was "django_outlook_email_backend-1.1.4.tar", last modified: Mon May 13 14:41:18 2024, max compression
```

## Comparing `django_outlook_email_backend-1.1.3.tar` & `django_outlook_email_backend-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/django_outlook_email/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/django_outlook_email_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/django_outlook_email/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/exceptions/microsoft_graph_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/django_outlook_email/senders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/senders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/senders/base_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/senders/content_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/senders/json_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/django_outlook_email/senders/mime_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:40:42.000000 django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:40:42.582777 django_outlook_email_backend-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 14:40:36.000000 django_outlook_email_backend-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/django_outlook_email/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/django_outlook_email_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/django_outlook_email/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/exceptions/microsoft_graph_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/django_outlook_email/senders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/senders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/senders/base_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/senders/content_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/senders/json_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/django_outlook_email/senders/mime_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 14:41:18.000000 django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 14:41:18.803169 django_outlook_email_backend-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 14:41:13.000000 django_outlook_email_backend-1.1.4/setup.py
```

### Comparing `django_outlook_email_backend-1.1.3/LICENSE` & `django_outlook_email_backend-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/PKG-INFO` & `django_outlook_email_backend-1.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.3/README.md` & `django_outlook_email_backend-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email/django_outlook_email_backend.py` & `django_outlook_email_backend-1.1.4/django_outlook_email/django_outlook_email_backend.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email/senders/content_types.py` & `django_outlook_email_backend-1.1.4/django_outlook_email/senders/content_types.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email/senders/json_sender.py` & `django_outlook_email_backend-1.1.4/django_outlook_email/senders/json_sender.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email/senders/mime_sender.py` & `django_outlook_email_backend-1.1.4/django_outlook_email/senders/mime_sender.py`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/PKG-INFO` & `django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_outlook_email-backend
-Version: 1.1.3
+Version: 1.1.4
 Summary: Ouauth2 outlook email backend for Django
 Home-page: https://github.com/enley-es/django-outlook-email-backend
 Author: Marc Claramunt
 Author-email: mclaramunt@enley.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_outlook_email_backend-1.1.3/django_outlook_email_backend.egg-info/SOURCES.txt` & `django_outlook_email_backend-1.1.4/django_outlook_email_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_outlook_email_backend-1.1.3/setup.py` & `django_outlook_email_backend-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django_outlook_email-backend',
-    version='1.1.3',
+    version='1.1.4',
     description='Ouauth2 outlook email backend for Django',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Marc Claramunt',
     author_email='mclaramunt@enley.com',
     license='MIT',
     zip_safe=True,
```

