# Comparing `tmp/hstream-0.1.47.tar.gz` & `tmp/hstream-0.1.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hstream-0.1.47.tar", max compression
+gzip compressed data, was "hstream-0.1.48.tar", max compression
```

## Comparing `hstream-0.1.47.tar` & `hstream-0.1.48.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.47/README.md
--rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.47/hstream/__init__.py
--rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.47/hstream/__main__.py
--rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.47/hstream/cli.py
--rw-r--r--   0        0        0    16890 2024-05-13 12:17:18.055215 hstream-0.1.47/hstream/components/components.py
--rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.47/hstream/components/styling_components.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.47/hstream/django_server/hs/__init__.py
--rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.47/hstream/django_server/hs/apps.py
--rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.47/hstream/django_server/hs/session_utils.py
--rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.47/hstream/django_server/hs/urls.py
--rw-r--r--   0        0        0     7546 2024-05-13 13:23:45.236155 hstream-0.1.47/hstream/django_server/hs/views.py
--rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.47/hstream/django_server/manage.py
--rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.47/hstream/django_server/root/__init__.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.47/hstream/django_server/root/asgi.py
--rw-r--r--   0        0        0     3218 2024-05-13 12:18:29.663642 hstream-0.1.47/hstream/django_server/root/settings.py
--rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.47/hstream/django_server/root/urls.py
--rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.47/hstream/django_server/root/wsgi.py
--rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.47/hstream/hs.py
--rw-r--r--   0        0        0      569 2024-05-13 12:18:29.651176 hstream-0.1.47/hstream/run.py
--rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.47/hstream/template.py
--rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.47/hstream/templates/error_html.html
--rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.47/hstream/templates/format_html.html
--rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.47/hstream/utils.py
--rw-r--r--   0        0        0      646 2024-05-13 13:23:59.160655 hstream-0.1.47/pyproject.toml
--rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.47/PKG-INFO
+-rw-r--r--   0        0        0     4232 2024-05-12 11:26:27.408478 hstream-0.1.48/README.md
+-rw-r--r--   0        0        0       53 2024-05-09 13:05:58.281504 hstream-0.1.48/hstream/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-12 11:26:20.930757 hstream-0.1.48/hstream/__main__.py
+-rw-r--r--   0        0        0     2109 2024-05-12 11:26:20.931172 hstream-0.1.48/hstream/cli.py
+-rw-r--r--   0        0        0    16890 2024-05-13 12:17:18.055215 hstream-0.1.48/hstream/components/components.py
+-rw-r--r--   0        0        0     4625 2024-05-12 11:26:20.932358 hstream-0.1.48/hstream/components/styling_components.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.932458 hstream-0.1.48/hstream/django_server/hs/__init__.py
+-rw-r--r--   0        0        0      136 2024-05-12 11:26:20.933121 hstream-0.1.48/hstream/django_server/hs/apps.py
+-rw-r--r--   0        0        0      749 2024-05-12 11:26:20.933435 hstream-0.1.48/hstream/django_server/hs/session_utils.py
+-rw-r--r--   0        0        0      424 2024-05-12 11:26:20.933722 hstream-0.1.48/hstream/django_server/hs/urls.py
+-rw-r--r--   0        0        0     7579 2024-05-13 14:07:38.675320 hstream-0.1.48/hstream/django_server/hs/views.py
+-rwxr-xr-x   0        0        0      661 2024-05-12 11:26:20.934370 hstream-0.1.48/hstream/django_server/manage.py
+-rw-r--r--   0        0        0        0 2024-05-12 11:26:20.934433 hstream-0.1.48/hstream/django_server/root/__init__.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.934747 hstream-0.1.48/hstream/django_server/root/asgi.py
+-rw-r--r--   0        0        0     3218 2024-05-13 12:18:29.663642 hstream-0.1.48/hstream/django_server/root/settings.py
+-rw-r--r--   0        0        0      802 2024-05-12 11:26:20.935930 hstream-0.1.48/hstream/django_server/root/urls.py
+-rw-r--r--   0        0        0      381 2024-05-12 11:26:20.936295 hstream-0.1.48/hstream/django_server/root/wsgi.py
+-rw-r--r--   0        0        0      683 2024-05-12 11:26:20.936728 hstream-0.1.48/hstream/hs.py
+-rw-r--r--   0        0        0      569 2024-05-13 12:18:29.651176 hstream-0.1.48/hstream/run.py
+-rw-r--r--   0        0        0      394 2024-05-09 13:05:58.283832 hstream-0.1.48/hstream/template.py
+-rw-r--r--   0        0        0      162 2024-05-12 11:26:20.937259 hstream-0.1.48/hstream/templates/error_html.html
+-rw-r--r--   0        0        0     2446 2024-05-12 11:26:20.937650 hstream-0.1.48/hstream/templates/format_html.html
+-rw-r--r--   0        0        0     2466 2024-05-12 11:26:20.937995 hstream-0.1.48/hstream/utils.py
+-rw-r--r--   0        0        0      646 2024-05-13 14:07:46.288349 hstream-0.1.48/pyproject.toml
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 hstream-0.1.48/PKG-INFO
```

### Comparing `hstream-0.1.47/README.md` & `hstream-0.1.48/README.md`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/cli.py` & `hstream-0.1.48/hstream/cli.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/components/components.py` & `hstream-0.1.48/hstream/components/components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/components/styling_components.py` & `hstream-0.1.48/hstream/components/styling_components.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/django_server/hs/session_utils.py` & `hstream-0.1.48/hstream/django_server/hs/session_utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/django_server/hs/views.py` & `hstream-0.1.48/hstream/django_server/hs/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         for old_key, old_value in prev_hs_ids_and_content.items():
             if old_key in get_session_var(request, "hs_html_partial_keys_updated", []):
                 break
             new_value = current_hs_ids_and_content.get(old_key, False)
             if new_value:
                 if old_value != new_value:
                     set_session_var(
+                        request,
                         "hs_html_partial_keys_updated",
                         get_session_var(request, "hs_html_partial_keys_updated", [])
                         + [old_key],
                     )
                     response.headers["HX-Target"] = f"#{old_key}"
                     response.headers["HX-Reswap"] = "innerHTML"
                     print("partial html sent")
```

### Comparing `hstream-0.1.47/hstream/django_server/manage.py` & `hstream-0.1.48/hstream/django_server/manage.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/django_server/root/settings.py` & `hstream-0.1.48/hstream/django_server/root/settings.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/django_server/root/urls.py` & `hstream-0.1.48/hstream/django_server/root/urls.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/hs.py` & `hstream-0.1.48/hstream/hs.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/run.py` & `hstream-0.1.48/hstream/run.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/templates/format_html.html` & `hstream-0.1.48/hstream/templates/format_html.html`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/hstream/utils.py` & `hstream-0.1.48/hstream/utils.py`

 * *Files identical despite different names*

### Comparing `hstream-0.1.47/pyproject.toml` & `hstream-0.1.48/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hstream"
-version = "0.1.47"
+version = "0.1.48"
 description = ""
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 hstream = "hstream.cli:cli"
```

### Comparing `hstream-0.1.47/PKG-INFO` & `hstream-0.1.48/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hstream
-Version: 0.1.47
+Version: 0.1.48
 Summary: 
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

