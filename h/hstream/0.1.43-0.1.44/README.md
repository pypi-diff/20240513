# Comparing `tmp/hstream-0.1.43.tar.gz` & `tmp/hstream-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.43.tar", max compression
+gzip compressed data, was "hstream-0.1.44.tar", max compression
```

## Comparing `hstream-0.1.43.tar` & `hstream-0.1.44.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.43/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.43/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.43/hstream/__main__.py
--rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.43/hstream/cli.py
--rw-r--r--   0        0        0    16867 2024-05-12 11:26:20.932004 hstream-0.1.43/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.43/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.43/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.43/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.43/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.43/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7383 2024-05-12 11:26:20.934057 hstream-0.1.43/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.43/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.43/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.43/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-13 11:31:46.608195 hstream-0.1.43/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.43/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.43/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.43/hstream/hs.py
--rw-r--r--   0        0        0      573 2024-05-13 11:44:10.747542 hstream-0.1.43/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.43/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.43/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.43/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.43/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-13 11:44:32.149779 hstream-0.1.43/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.43/PKG-INFO
+-rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.44/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.44/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.44/hstream/__main__.py
+-rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.44/hstream/cli.py
+-rw-r--r--   0        0        0    16867 2024-05-12 11:26:20.932004 hstream-0.1.44/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.44/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.44/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.44/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.44/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.44/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7431 2024-05-13 11:57:51.932618 hstream-0.1.44/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.44/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.44/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.44/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-13 11:31:46.608195 hstream-0.1.44/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.44/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.44/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.44/hstream/hs.py
+-rw-r--r--   0        0        0      573 2024-05-13 11:44:10.747542 hstream-0.1.44/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.44/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.44/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.44/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.44/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-13 11:58:01.379787 hstream-0.1.44/pyproject.toml
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.44/PKG-INFO
```

### Comparing `hstream-0.1.43/README.md` & `hstream-0.1.44/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/cli.py` & `hstream-0.1.44/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/components/components.py` & `hstream-0.1.44/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/components/styling_components.py` & `hstream-0.1.44/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/django_server/hs/session_utils.py` & `hstream-0.1.44/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/django_server/hs/views.py` & `hstream-0.1.44/hstream/django_server/hs/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,17 @@
             sleep(0.1)
     else:
         set_session_var(request, "hs_script_should_stop", True)
     set_session_var(request, "hs_html", "")
 
 
 def index(request: HttpRequest):
-    request.session.clear()
-    request.session.save()
+    if len(request.session.keys()) > 0:
+        request.session.clear()
+        request.session.save()
     request_server_stop_running_user_script(request, wait=True)
     set_session_var(request, "hs_html_last_sent", "")
     return HttpResponse(format_html())
 
 
 def run_hs(request):
     if get_session_var(request, "hs_script_running", False):
```

### Comparing `hstream-0.1.43/hstream/django_server/manage.py` & `hstream-0.1.44/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/django_server/root/settings.py` & `hstream-0.1.44/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/django_server/root/urls.py` & `hstream-0.1.44/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/hs.py` & `hstream-0.1.44/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/run.py` & `hstream-0.1.44/hstream/run.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/templates/format_html.html` & `hstream-0.1.44/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/hstream/utils.py` & `hstream-0.1.44/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.43/pyproject.toml` & `hstream-0.1.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.43"
+version = "0.1.44"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.43/PKG-INFO` & `hstream-0.1.44/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.43
+Version: 0.1.44
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

