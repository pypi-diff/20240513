# Comparing `tmp/django-df-auth-1.0.8.tar.gz` & `tmp/django-df-auth-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-df-auth-1.0.8.tar", last modified: Wed Dec 27 15:19:04 2023, max compression
+gzip compressed data, was "django-df-auth-1.0.9.tar", last modified: Thu Mar 14 13:35:10 2024, max compression
```

## Comparing `django-df-auth-1.0.8.tar` & `django-df-auth-1.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.800240 django-df-auth-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2023-12-27 15:19:04.800240 django-df-auth-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.796240 django-df-auth-1.0.8/df_auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.796240 django-df-auth-1.0.8/df_auth/drf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/drf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15578 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/drf/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/drf/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/drf/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.796240 django-df-auth-1.0.8/df_auth/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/migrations/0002_alter_user2fa_user_userregistration.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/migrations/0003_alter_userregistration_is_registering.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/remote_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.796240 django-df-auth-1.0.8/df_auth/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/templatetags/auth_magic_link.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/df_auth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 15:19:04.800240 django-df-auth-1.0.8/django_df_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2023-12-27 15:19:04.000000 django-df-auth-1.0.8/django_df_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2023-12-27 15:19:04.000000 django-df-auth-1.0.8/django_df_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 15:19:04.000000 django-df-auth-1.0.8/django_df_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-27 15:19:04.000000 django-df-auth-1.0.8/django_df_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-27 15:19:04.000000 django-df-auth-1.0.8/django_df_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 15:19:04.800240 django-df-auth-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 15:18:52.000000 django-df-auth-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.769815 django-df-auth-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-14 13:35:10.769815 django-df-auth-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.765815 django-df-auth-1.0.9/df_auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5040 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.765815 django-df-auth-1.0.9/df_auth/drf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/drf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15578 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/drf/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/drf/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/drf/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.765815 django-df-auth-1.0.9/df_auth/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/migrations/0002_alter_user2fa_user_userregistration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/migrations/0003_alter_userregistration_is_registering.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/remote_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.765815 django-df-auth-1.0.9/df_auth/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/templatetags/auth_magic_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/df_auth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 13:35:10.765815 django-df-auth-1.0.9/django_df_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-03-14 13:35:10.000000 django-df-auth-1.0.9/django_df_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-14 13:35:10.000000 django-df-auth-1.0.9/django_df_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 13:35:10.000000 django-df-auth-1.0.9/django_df_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-14 13:35:10.000000 django-df-auth-1.0.9/django_df_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-14 13:35:10.000000 django-df-auth-1.0.9/django_df_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:35:10.769815 django-df-auth-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 13:35:00.000000 django-df-auth-1.0.9/setup.py
```

### Comparing `django-df-auth-1.0.8/LICENSE` & `django-df-auth-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/PKG-INFO` & `django-df-auth-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-auth
-Version: 1.0.8
+Version: 1.0.9
 Summary: Opinionated Django REST auth endpoints for JWT authentication and social accounts.
 Author-email: Apexive OSS <open-source@apexive.com>
 License: MIT License
         
         Copyright (c) 2022 Apexive.com
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-df-auth-1.0.8/README.md` & `django-df-auth-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/admin.py` & `django-df-auth-1.0.9/df_auth/admin.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/backends.py` & `django-df-auth-1.0.9/df_auth/backends.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Type
+from typing import Any, Dict, Optional, Type
 
 from df_api_drf.resolvers import client_url
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.http import HttpRequest
 from django_otp.models import SideChannelDevice
 from django_otp.plugins.otp_email.models import EmailDevice
@@ -127,21 +127,24 @@
     identity_field = "email"
     device_identity_field = "email"
     DeviceModel = EmailDevice
 
     def send_challenge(
         self, device: EmailDevice, request: HttpRequest, **kwargs: Any
     ) -> None:
-        device.generate_challenge(
-            {
-                "username": device.email,
-                "base_url": client_url(request=request, user=device.user)
-                + api_settings.SITE_LOGIN_URL,
-                "redirect_path": kwargs.get("redirect_path", ""),
-            }
-        )
+        device.generate_challenge(self.extra_context(device, request, **kwargs))
+
+    def extra_context(
+        self, device: EmailDevice, request: HttpRequest, **kwargs: Any
+    ) -> Dict[str, Any]:
+        return {
+            "username": device.email,
+            "base_url": client_url(request=request, user=device.user)
+            + api_settings.SITE_LOGIN_URL,
+            "redirect_path": kwargs.get("redirect_path", ""),
+        }
 
 
 class TwilioSMSOTPBackend(BaseOTPBackend):
     identity_field = "phone_number"
     device_identity_field = "number"
     DeviceModel = TwilioSMSDevice
```

### Comparing `django-df-auth-1.0.8/df_auth/defaults.py` & `django-df-auth-1.0.9/df_auth/defaults.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/drf/serializers.py` & `django-df-auth-1.0.9/df_auth/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/drf/urls.py` & `django-df-auth-1.0.9/df_auth/drf/urls.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/drf/viewsets.py` & `django-df-auth-1.0.9/df_auth/drf/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/exceptions.py` & `django-df-auth-1.0.9/df_auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/managers.py` & `django-df-auth-1.0.9/df_auth/managers.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/migrations/0001_initial.py` & `django-df-auth-1.0.9/df_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/migrations/0002_alter_user2fa_user_userregistration.py` & `django-df-auth-1.0.9/df_auth/migrations/0002_alter_user2fa_user_userregistration.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/models.py` & `django-df-auth-1.0.9/df_auth/models.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/permissions.py` & `django-df-auth-1.0.9/df_auth/permissions.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/remote_config.py` & `django-df-auth-1.0.9/df_auth/remote_config.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/settings.py` & `django-df-auth-1.0.9/df_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/templatetags/auth_magic_link.py` & `django-df-auth-1.0.9/df_auth/templatetags/auth_magic_link.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/df_auth/utils.py` & `django-df-auth-1.0.9/df_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/django_df_auth.egg-info/PKG-INFO` & `django-df-auth-1.0.9/django_df_auth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-df-auth
-Version: 1.0.8
+Version: 1.0.9
 Summary: Opinionated Django REST auth endpoints for JWT authentication and social accounts.
 Author-email: Apexive OSS <open-source@apexive.com>
 License: MIT License
         
         Copyright (c) 2022 Apexive.com
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-df-auth-1.0.8/django_df_auth.egg-info/SOURCES.txt` & `django-df-auth-1.0.9/django_df_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-df-auth-1.0.8/pyproject.toml` & `django-df-auth-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-df-auth"
-version = "1.0.8"
+version = "1.0.9"
 description = "Opinionated Django REST auth endpoints for JWT authentication and social accounts."
 readme = "README.md"
 authors = [{name = "Apexive OSS", email = "open-source@apexive.com"}]
 license = { file = "LICENSE" }
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
```

