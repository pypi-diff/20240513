# Comparing `tmp/hstream-0.1.45.tar.gz` & `tmp/hstream-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.45.tar", max compression
+gzip compressed data, was "hstream-0.1.46.tar", max compression
```

## Comparing `hstream-0.1.45.tar` & `hstream-0.1.46.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.45/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.45/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.45/hstream/__main__.py
--rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.45/hstream/cli.py
--rw-r--r--   0        0        0    16890 2024-05-13 12:17:18.055215 hstream-0.1.45/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.45/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.45/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.45/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.45/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.45/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7431 2024-05-13 11:57:51.932618 hstream-0.1.45/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.45/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.45/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.45/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-13 11:31:46.608195 hstream-0.1.45/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.45/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.45/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.45/hstream/hs.py
--rw-r--r--   0        0        0      573 2024-05-13 11:44:10.747542 hstream-0.1.45/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.45/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.45/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.45/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.45/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-13 12:18:02.313958 hstream-0.1.45/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.45/PKG-INFO
+-rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.46/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.46/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.46/hstream/__main__.py
+-rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.46/hstream/cli.py
+-rw-r--r--   0        0        0    16890 2024-05-13 12:17:18.055215 hstream-0.1.46/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.46/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.46/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.46/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.46/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.46/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7465 2024-05-13 12:57:35.606802 hstream-0.1.46/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.46/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.46/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.46/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-13 12:18:29.663642 hstream-0.1.46/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.46/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.46/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.46/hstream/hs.py
+-rw-r--r--   0        0        0      569 2024-05-13 12:18:29.651176 hstream-0.1.46/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.46/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.46/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.46/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.46/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-13 12:58:37.456015 hstream-0.1.46/pyproject.toml
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.46/PKG-INFO
```

### Comparing `hstream-0.1.45/README.md` & `hstream-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/cli.py` & `hstream-0.1.46/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/components/components.py` & `hstream-0.1.46/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/components/styling_components.py` & `hstream-0.1.46/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/django_server/hs/session_utils.py` & `hstream-0.1.46/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/django_server/hs/views.py` & `hstream-0.1.46/hstream/django_server/hs/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 from time import sleep
-
+import os
 from django.http import HttpRequest, HttpResponse
 
 from hstream.hs import hs as hs_type
 from hstream.template import error_html, format_html
 from hstream.utils import pick_a_strategy, split_code_into_blocks
 
 from .session_utils import get_session_var, set_session_var
@@ -22,26 +22,26 @@
 
 def index(request: HttpRequest):
     if len(request.session.keys()) > 0:
         request.session.clear()
         request.session.save()
     request_server_stop_running_user_script(request, wait=True)
     set_session_var(request, "hs_html_last_sent", "")
+    set_session_var(request, "hs_html", "")
     return HttpResponse(format_html())
 
 
 def run_hs(request):
     if get_session_var(request, "hs_script_running", False):
         HttpResponse("already running")
     set_session_var(request, "hs_script_running", True)
     try:
-        import os
+        
 
         # TODO: I'm sure theres a way to pass this filename from django through the cli :thinking
-        print(os.environ["HS_FILE_TO_RUN"])
         hs: hs_type = run_user_code_and_return_hs_instance(
             os.environ["HS_FILE_TO_RUN"], request
         )
     except Exception as e:
         set_session_var(request, "hs_script_running", False)
         set_session_var(
             request,
@@ -157,14 +157,15 @@
                 set_session_var(request, "hs_html", html)
             except:  # noqa #E722
                 pass
     except Exception as e:
         e.args = (f"Line: {line}, code: {block}", *e.args)
         raise e
     finally:
+        users_hs_instance.clear()
         set_session_var(request, "hs_script_should_stop", False)
     return users_hs_instance
 
 
 def set_component_value(
     request: HttpRequest,
 ):
```

### Comparing `hstream-0.1.45/hstream/django_server/manage.py` & `hstream-0.1.46/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/django_server/root/settings.py` & `hstream-0.1.46/hstream/django_server/root/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # SECURITY WARNING: keep the secret key used in production secret!
 SECRET_KEY = "django-insecure-l=@v_lw4ndrq3#=8)v+_^a@$=5c_8a_sajq9n-2#ea#@p%o3fw"
 
 # SECURITY WARNING: don't run with debug turned on in production!
 DEBUG = True
 
-ALLOWED_HOSTS = ['*']
+ALLOWED_HOSTS = ["*"]
 
 
 # Application definition
 
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
```

### Comparing `hstream-0.1.45/hstream/django_server/root/urls.py` & `hstream-0.1.46/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/hs.py` & `hstream-0.1.46/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/run.py` & `hstream-0.1.46/hstream/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 import hstream
 
 
 def run_server(
     file: Path, other_paths: Dict[str, Path] = False, hs_root_path: str = "/"
 ):
     path_to_hstream_dir = os.path.dirname(os.path.abspath(hstream.__file__))
-    
+
     os.system(f"python {path_to_hstream_dir}/django_server/manage.py migrate")
     os.environ["HS_FILE_TO_RUN"] = str(file)
     command = f"python {path_to_hstream_dir}/django_server/manage.py runserver"
-    if os.environ.get('PORT', False):
+    if os.environ.get("PORT", False):
         command += f" 0.0.0.0:{os.environ['PORT']}"
     os.system(command)
```

### Comparing `hstream-0.1.45/hstream/templates/format_html.html` & `hstream-0.1.46/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/hstream/utils.py` & `hstream-0.1.46/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.45/pyproject.toml` & `hstream-0.1.46/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.45"
+version = "0.1.46"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.45/PKG-INFO` & `hstream-0.1.46/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.45
+Version: 0.1.46
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

