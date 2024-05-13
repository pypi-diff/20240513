# Comparing `tmp/django_viewrouter-0.1.2.tar.gz` & `tmp/django_viewrouter-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_viewrouter-0.1.2.tar", max compression
+gzip compressed data, was "django_viewrouter-0.1.3.tar", max compression
```

## Comparing `django_viewrouter-0.1.2.tar` & `django_viewrouter-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3496 2024-05-03 08:51:49.119346 django_viewrouter-0.1.2/README.md
--rw-r--r--   0        0        0      343 2024-05-10 10:31:43.224648 django_viewrouter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-03 08:51:49.119346 django_viewrouter-0.1.2/viewrouter/__init__.py
--rw-r--r--   0        0        0     4135 2024-05-10 10:30:02.478653 django_viewrouter-0.1.2/viewrouter/routers.py
--rw-r--r--   0        0        0       82 2024-05-03 08:51:49.119346 django_viewrouter-0.1.2/viewrouter/templates/viewrouter/actionview_index.html
--rw-r--r--   0        0        0     5025 2024-05-03 08:51:49.119346 django_viewrouter-0.1.2/viewrouter/tests.py
--rw-r--r--   0        0        0     3003 2024-05-03 08:51:49.119346 django_viewrouter-0.1.2/viewrouter/views.py
--rw-r--r--   0        0        0     3938 1970-01-01 00:00:00.000000 django_viewrouter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3496 2024-05-03 08:51:49.119346 django_viewrouter-0.1.3/README.md
+-rw-r--r--   0        0        0      344 2024-05-13 09:55:54.759770 django_viewrouter-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-03 08:51:49.119346 django_viewrouter-0.1.3/viewrouter/__init__.py
+-rw-r--r--   0        0        0     4135 2024-05-10 10:30:02.478653 django_viewrouter-0.1.3/viewrouter/routers.py
+-rw-r--r--   0        0        0       82 2024-05-03 08:51:49.119346 django_viewrouter-0.1.3/viewrouter/templates/viewrouter/actionview_index.html
+-rw-r--r--   0        0        0     5025 2024-05-03 08:51:49.119346 django_viewrouter-0.1.3/viewrouter/tests.py
+-rw-r--r--   0        0        0     3003 2024-05-03 08:51:49.119346 django_viewrouter-0.1.3/viewrouter/views.py
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 django_viewrouter-0.1.3/PKG-INFO
```

### Comparing `django_viewrouter-0.1.2/README.md` & `django_viewrouter-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.2/viewrouter/routers.py` & `django_viewrouter-0.1.3/viewrouter/routers.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.2/viewrouter/tests.py` & `django_viewrouter-0.1.3/viewrouter/tests.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.2/viewrouter/views.py` & `django_viewrouter-0.1.3/viewrouter/views.py`

 * *Files identical despite different names*

### Comparing `django_viewrouter-0.1.2/PKG-INFO` & `django_viewrouter-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django-viewrouter
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
 Author: Kamal Mustafa
 Author-email: k4ml@github.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=3.0,<4.0)
+Requires-Dist: Django (>=3.0)
 Description-Content-Type: text/markdown
 
 Rails style controller dispatch method for Django class based views. Instead
 of dispatching incoming http request to HTTP verbs such as 'GET', 'POST',
 'DELETE' etc, it dispatch to more familiar CRUD action such as create, update,
 delete, and delete. For browser based apps, I found the CRUD action make
 more sense, after all in the browser we only limited to GET and POST so not much gain to split our request handler into proper HTTP method.
```

