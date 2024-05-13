# Comparing `tmp/hstream-0.1.4.tar.gz` & `tmp/hstream-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.4.tar", max compression
+gzip compressed data, was "hstream-0.1.41.tar", max compression
```

## Comparing `hstream-0.1.4.tar` & `hstream-0.1.41.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4131 2024-05-11 14:06:53.604734 hstream-0.1.4/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.4/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-11 14:02:16.202112 hstream-0.1.4/hstream/__main__.py
--rw-r--r--   0        0        0     2109 2024-05-11 14:10:39.299497 hstream-0.1.4/hstream/cli.py
--rw-r--r--   0        0        0    16867 2024-05-11 14:22:15.594502 hstream-0.1.4/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-11 14:10:39.299008 hstream-0.1.4/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-11 01:21:34.641755 hstream-0.1.4/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-11 14:02:16.204711 hstream-0.1.4/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      748 2024-05-12 09:19:29.979614 hstream-0.1.4/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-11 14:02:16.210066 hstream-0.1.4/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7383 2024-05-12 09:26:19.654212 hstream-0.1.4/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-11 14:10:39.338137 hstream-0.1.4/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-11 01:21:34.646562 hstream-0.1.4/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-11 14:02:16.217876 hstream-0.1.4/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3215 2024-05-11 14:02:16.237885 hstream-0.1.4/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-11 14:02:16.219668 hstream-0.1.4/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-11 14:02:16.221764 hstream-0.1.4/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-11 14:10:39.299423 hstream-0.1.4/hstream/hs.py
--rw-r--r--   0        0        0      377 2024-05-11 14:10:39.299336 hstream-0.1.4/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.4/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-11 14:06:53.529050 hstream-0.1.4/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-11 14:06:53.601647 hstream-0.1.4/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-11 14:15:58.798201 hstream-0.1.4/hstream/utils.py
--rw-r--r--   0        0        0      579 2024-05-12 09:26:45.222427 hstream-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 hstream-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.41/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.41/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.41/hstream/__main__.py
+-rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.41/hstream/cli.py
+-rw-r--r--   0        0        0    16867 2024-05-12 11:26:20.932004 hstream-0.1.41/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.41/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.41/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.41/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.41/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.41/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7383 2024-05-12 11:26:20.934057 hstream-0.1.41/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.41/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.41/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.41/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3215 2024-05-12 11:26:20.935119 hstream-0.1.41/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.41/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.41/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.41/hstream/hs.py
+-rw-r--r--   0        0        0      489 2024-05-13 10:56:43.517684 hstream-0.1.41/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.41/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.41/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.41/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.41/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-13 10:57:06.214475 hstream-0.1.41/pyproject.toml
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.41/PKG-INFO
```

### Comparing `hstream-0.1.4/README.md` & `hstream-0.1.41/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # HStream
 
-Convert your script to interactive python web app `user_said = hs.text_input("What would you like to say:")`
+Convert your script to interactive python web app like so:
 
-Powered by htmx enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
+    `user_said = hs.text_input("What would you like to say:")`
+
+Powered by [Django](https://github.com/django/django) + [htmx](https://github.com/bigskysoftware/htmx) enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
 
 # Usage
 
 `pip install hstream`
 
 `hstream init`
```

### Comparing `hstream-0.1.4/hstream/cli.py` & `hstream-0.1.41/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/components/components.py` & `hstream-0.1.41/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/components/styling_components.py` & `hstream-0.1.41/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/django_server/hs/session_utils.py` & `hstream-0.1.41/hstream/django_server/hs/session_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.http import HttpRequest
 
+
 def refresh_session(request: HttpRequest):
     from importlib import import_module
 
     from django.conf import settings
 
     engine = import_module(settings.SESSION_ENGINE)
     SessionStore = engine.SessionStore
```

### Comparing `hstream-0.1.4/hstream/django_server/hs/views.py` & `hstream-0.1.41/hstream/django_server/hs/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             try:
                 for var_name, var_value in namespace.items():
                     if var_value.__class__.__name__ == "hs":
                         users_hs_instance = var_value
                 html = users_hs_instance.doc.getvalue()
                 # TODO: if the script sets component values we should honour these as well
                 # for example a button reverting itself back to false after being clicked
-                request.session = namespace['__builtins__']['_hs_session']
+                request.session = namespace["__builtins__"]["_hs_session"]
                 set_session_var(request, "hs_html", html)
             except:  # noqa #E722
                 pass
     except Exception as e:
         e.args = (f"Line: {line}, code: {block}", *e.args)
         raise e
     finally:
```

### Comparing `hstream-0.1.4/hstream/django_server/manage.py` & `hstream-0.1.41/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/django_server/root/settings.py` & `hstream-0.1.41/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/django_server/root/urls.py` & `hstream-0.1.41/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/hs.py` & `hstream-0.1.41/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/templates/format_html.html` & `hstream-0.1.41/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/hstream/utils.py` & `hstream-0.1.41/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.4/pyproject.toml` & `hstream-0.1.41/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.4"
+version = "0.1.41"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
 
@@ -20,11 +20,14 @@
 black = "^24.4.2"
 ipykernel = "^6.29.4"
 pandas = "^2.2.2"
 ipdb = "^0.13.13"
 isort = "^5.13.2"
 pre-commit = "^3.7.1"
 ruff = "^0.4.4"
+pytest = "^8.2.0"
+python-dotenv = "^1.0.1"
+playwright = "^1.43.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hstream-0.1.4/PKG-INFO` & `hstream-0.1.41/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.4
+Version: 0.1.41
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,17 +14,19 @@
 Requires-Dist: django (>=5.0.6,<6.0.0)
 Requires-Dist: markdown (>=3.6,<4.0)
 Requires-Dist: yattag (>=1.15.2,<2.0.0)
 Description-Content-Type: text/markdown
 
 # HStream
 
-Convert your script to interactive python web app `user_said = hs.text_input("What would you like to say:")`
+Convert your script to interactive python web app like so:
 
-Powered by htmx enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
+    `user_said = hs.text_input("What would you like to say:")`
+
+Powered by [Django](https://github.com/django/django) + [htmx](https://github.com/bigskysoftware/htmx) enables easy app ejection to scale/extend once you've outgrown HStream. Inspired by [Streamlit](https://github.com/streamlit/streamlit).
 
 # Usage
 
 `pip install hstream`
 
 `hstream init`
```

