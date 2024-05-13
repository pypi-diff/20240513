# Comparing `tmp/jsm_user_services-1.5.1.tar.gz` & `tmp/jsm_user_services-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsm_user_services-1.5.1.tar", max compression
+gzip compressed data, was "jsm_user_services-1.5.2.tar", max compression
```

## Comparing `jsm_user_services-1.5.1.tar` & `jsm_user_services-1.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/LICENSE
--rw-r--r--   0        0        0    10313 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/README.md
--rw-r--r--   0        0        0       54 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/__init__.py
--rw-r--r--   0        0        0      107 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/apps.py
--rw-r--r--   0        0        0        0 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/decorators/__init__.py
--rw-r--r--   0        0        0     3795 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/decorators/lgpd.py
--rw-r--r--   0        0        0     5933 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/decorators/lgpd_utils.py
--rw-r--r--   0        0        0        0 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/drf_tools/__init__.py
--rw-r--r--   0        0        0     3087 2024-05-09 19:48:05.863281 jsm_user_services-1.5.1/jsm_user_services/drf_tools/authentications.py
--rw-r--r--   0        0        0      451 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/drf_tools/exceptions.py
--rw-r--r--   0        0        0     2475 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/drf_tools/helpers.py
--rw-r--r--   0        0        0    15151 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/drf_tools/permissions.py
--rw-r--r--   0        0        0      692 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/exception.py
--rw-r--r--   0        0        0        0 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/flask_module/__init__.py
--rw-r--r--   0        0        0     3476 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/flask_module/middleware.py
--rw-r--r--   0        0        0     3292 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/middleware.py
--rw-r--r--   0        0        0        0 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/services/__init__.py
--rw-r--r--   0        0        0     4247 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/services/everest.py
--rw-r--r--   0        0        0     1996 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/services/google.py
--rw-r--r--   0        0        0     6210 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/services/user.py
--rw-r--r--   0        0        0     2436 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/settings.py
--rw-r--r--   0        0        0        0 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/auth_jwt.py
--rw-r--r--   0        0        0      866 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/email_utils.py
--rw-r--r--   0        0        0     2333 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/http_utils.py
--rw-r--r--   0        0        0      304 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/import_utils.py
--rw-r--r--   0        0        0      415 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/local_threading_utils.py
--rw-r--r--   0        0        0      268 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/logging_utils.py
--rw-r--r--   0        0        0     2185 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/request_id.py
--rw-r--r--   0        0        0      618 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/settings_utils.py
--rw-r--r--   0        0        0      237 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/jsm_user_services/support/string_utils.py
--rw-r--r--   0        0        0     1633 2024-05-09 19:48:05.867281 jsm_user_services-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 jsm_user_services-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/LICENSE
+-rw-r--r--   0        0        0    10313 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/README.md
+-rw-r--r--   0        0        0       54 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/apps.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/decorators/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/decorators/lgpd.py
+-rw-r--r--   0        0        0     5933 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/decorators/lgpd_utils.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/drf_tools/__init__.py
+-rw-r--r--   0        0        0     3161 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/drf_tools/authentications.py
+-rw-r--r--   0        0        0      451 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/drf_tools/exceptions.py
+-rw-r--r--   0        0        0     2475 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/drf_tools/helpers.py
+-rw-r--r--   0        0        0    15151 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/drf_tools/permissions.py
+-rw-r--r--   0        0        0      692 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/exception.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/flask_module/__init__.py
+-rw-r--r--   0        0        0     3476 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/flask_module/middleware.py
+-rw-r--r--   0        0        0     3292 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/services/__init__.py
+-rw-r--r--   0        0        0     4247 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/services/everest.py
+-rw-r--r--   0        0        0     1996 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/services/google.py
+-rw-r--r--   0        0        0     6210 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/services/user.py
+-rw-r--r--   0        0        0     2436 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/settings.py
+-rw-r--r--   0        0        0        0 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/auth_jwt.py
+-rw-r--r--   0        0        0      866 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/email_utils.py
+-rw-r--r--   0        0        0     2333 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/http_utils.py
+-rw-r--r--   0        0        0      304 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/import_utils.py
+-rw-r--r--   0        0        0      415 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/local_threading_utils.py
+-rw-r--r--   0        0        0      268 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/logging_utils.py
+-rw-r--r--   0        0        0     2185 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/request_id.py
+-rw-r--r--   0        0        0      618 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/settings_utils.py
+-rw-r--r--   0        0        0      237 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/jsm_user_services/support/string_utils.py
+-rw-r--r--   0        0        0     1633 2024-05-13 18:20:12.782505 jsm_user_services-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    11344 1970-01-01 00:00:00.000000 jsm_user_services-1.5.2/PKG-INFO
```

### Comparing `jsm_user_services-1.5.1/LICENSE` & `jsm_user_services-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/README.md` & `jsm_user_services-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/decorators/lgpd.py` & `jsm_user_services-1.5.2/jsm_user_services/decorators/lgpd.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/decorators/lgpd_utils.py` & `jsm_user_services-1.5.2/jsm_user_services/decorators/lgpd_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/drf_tools/authentications.py` & `jsm_user_services-1.5.2/jsm_user_services/drf_tools/authentications.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,11 +77,12 @@
 
         try:
             payload = get_decoded_oauth_token(token)
             current_timestamp = int(time.time())
             is_token_expired = "exp" in payload and current_timestamp > payload["exp"]
             is_sub_claim_in_payload = "sub" in payload
             if not is_token_expired and is_sub_claim_in_payload:
-                return True
+                return (AnonymousUser(), token)
+            else:
+                raise CustomInvalidToken()
         except jwt.DecodeError:
-            return False
-        return False
+            raise CustomInvalidToken()
```

### Comparing `jsm_user_services-1.5.1/jsm_user_services/drf_tools/helpers.py` & `jsm_user_services-1.5.2/jsm_user_services/drf_tools/helpers.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/drf_tools/permissions.py` & `jsm_user_services-1.5.2/jsm_user_services/drf_tools/permissions.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/exception.py` & `jsm_user_services-1.5.2/jsm_user_services/exception.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/flask_module/middleware.py` & `jsm_user_services-1.5.2/jsm_user_services/flask_module/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/middleware.py` & `jsm_user_services-1.5.2/jsm_user_services/middleware.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/services/everest.py` & `jsm_user_services-1.5.2/jsm_user_services/services/everest.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/services/google.py` & `jsm_user_services-1.5.2/jsm_user_services/services/google.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/services/user.py` & `jsm_user_services-1.5.2/jsm_user_services/services/user.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/settings.py` & `jsm_user_services-1.5.2/jsm_user_services/settings.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/support/auth_jwt.py` & `jsm_user_services-1.5.2/jsm_user_services/support/auth_jwt.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/support/email_utils.py` & `jsm_user_services-1.5.2/jsm_user_services/support/email_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/support/http_utils.py` & `jsm_user_services-1.5.2/jsm_user_services/support/http_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/support/request_id.py` & `jsm_user_services-1.5.2/jsm_user_services/support/request_id.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/jsm_user_services/support/settings_utils.py` & `jsm_user_services-1.5.2/jsm_user_services/support/settings_utils.py`

 * *Files identical despite different names*

### Comparing `jsm_user_services-1.5.1/pyproject.toml` & `jsm_user_services-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jsm-user-services"
-version = "1.5.1"
+version = "1.5.2"
 description = "Middleware to intercept JWT auth token and more utils functions"
 authors = ["Juntos Somos Mais <labs@juntossomosmais.com.br>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "jsm_user_services"}]
 classifiers=[
     "Programming Language :: Python",
```

### Comparing `jsm_user_services-1.5.1/PKG-INFO` & `jsm_user_services-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsm-user-services
-Version: 1.5.1
+Version: 1.5.2
 Summary: Middleware to intercept JWT auth token and more utils functions
 License: MIT
 Author: Juntos Somos Mais
 Author-email: labs@juntossomosmais.com.br
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

