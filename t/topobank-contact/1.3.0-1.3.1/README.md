# Comparing `tmp/topobank_contact-1.3.0.tar.gz` & `tmp/topobank_contact-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank_contact-1.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "topobank_contact-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `topobank_contact-1.3.0.tar` & `topobank_contact-1.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1129 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/LICENSE
--rw-r--r--   0        0        0      471 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/README.rst
--rw-r--r--   0        0        0     1454 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/pyproject.toml
--rw-r--r--   0        0        0       47 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/__init__.py
--rw-r--r--   0        0        0      987 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/apps.py
--rw-r--r--   0        0        0     6027 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/downloads.py
--rw-r--r--   0        0        0    19962 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/functions.py
--rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/migrations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/signals.py
--rw-r--r--   0        0        0        0 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/__init__.py
--rw-r--r--   0        0        0     2405 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/conftest.py
--rw-r--r--   0        0        0      236 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_api.py
--rw-r--r--   0        0        0     1852 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_downloads.py
--rw-r--r--   0        0        0     2436 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_functions.py
--rw-r--r--   0        0        0      832 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/test_views.py
--rw-r--r--   0        0        0      518 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/tests/urls.py
--rw-r--r--   0        0        0      683 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/urls.py
--rw-r--r--   0        0        0       97 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/version.py
--rw-r--r--   0        0        0     2179 2024-05-12 14:08:45.102548 topobank_contact-1.3.0/topobank_contact/views.py
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 topobank_contact-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1129 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/LICENSE
+-rw-r--r--   0        0        0      471 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/README.rst
+-rw-r--r--   0        0        0     1454 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/__init__.py
+-rw-r--r--   0        0        0      987 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/apps.py
+-rw-r--r--   0        0        0     6027 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/downloads.py
+-rw-r--r--   0        0        0    19962 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/functions.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/signals.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/__init__.py
+-rw-r--r--   0        0        0     2405 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/conftest.py
+-rw-r--r--   0        0        0      236 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/test_api.py
+-rw-r--r--   0        0        0     1852 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/test_downloads.py
+-rw-r--r--   0        0        0     2436 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/test_functions.py
+-rw-r--r--   0        0        0      832 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/test_views.py
+-rw-r--r--   0        0        0      518 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/tests/urls.py
+-rw-r--r--   0        0        0      683 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/urls.py
+-rw-r--r--   0        0        0       97 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/version.py
+-rw-r--r--   0        0        0     2179 2024-05-13 20:43:35.002528 topobank_contact-1.3.1/topobank_contact/views.py
+-rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 topobank_contact-1.3.1/PKG-INFO
```

### Comparing `topobank_contact-1.3.0/LICENSE` & `topobank_contact-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/pyproject.toml` & `topobank_contact-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/apps.py` & `topobank_contact-1.3.1/topobank_contact/apps.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/downloads.py` & `topobank_contact-1.3.1/topobank_contact/downloads.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/functions.py` & `topobank_contact-1.3.1/topobank_contact/functions.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/tests/conftest.py` & `topobank_contact-1.3.1/topobank_contact/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/tests/test_downloads.py` & `topobank_contact-1.3.1/topobank_contact/tests/test_downloads.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/tests/test_functions.py` & `topobank_contact-1.3.1/topobank_contact/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/tests/test_views.py` & `topobank_contact-1.3.1/topobank_contact/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/tests/urls.py` & `topobank_contact-1.3.1/topobank_contact/tests/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/urls.py` & `topobank_contact-1.3.1/topobank_contact/urls.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/topobank_contact/views.py` & `topobank_contact-1.3.1/topobank_contact/views.py`

 * *Files identical despite different names*

### Comparing `topobank_contact-1.3.0/PKG-INFO` & `topobank_contact-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topobank-contact
-Version: 1.3.0
+Version: 1.3.1
 Summary: Boundary-element method for "topobank"
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 Requires-Python: >=3.8.0
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

