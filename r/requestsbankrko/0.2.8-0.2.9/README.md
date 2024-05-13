# Comparing `tmp/requestsbankrko-0.2.8.tar.gz` & `tmp/requestsbankrko-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requestsbankrko-0.2.8.tar", last modified: Wed Jul 26 09:28:53 2023, max compression
+gzip compressed data, was "requestsbankrko-0.2.9.tar", last modified: Wed Jul 26 10:43:36 2023, max compression
```

## Comparing `requestsbankrko-0.2.8.tar` & `requestsbankrko-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29690 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/src/bank_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/src/open_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 09:28:53.000000 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 09:28:53.000000 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:28:53.000000 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 09:28:53.000000 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 09:28:53.000000 requestsbankrko-0.2.8/src/requestsbankrko.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/src/zip_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:28:53.421207 requestsbankrko-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    57358 2023-07-26 09:28:41.000000 requestsbankrko-0.2.8/tests/test_bank_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:43:36.392612 requestsbankrko-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 10:43:36.388612 requestsbankrko-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:43:36.392612 requestsbankrko-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:43:36.388612 requestsbankrko-0.2.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29758 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/src/bank_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/src/open_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:43:36.388612 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-26 10:43:36.000000 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-26 10:43:36.000000 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:43:36.000000 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 10:43:36.000000 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 10:43:36.000000 requestsbankrko-0.2.9/src/requestsbankrko.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/src/zip_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:43:36.388612 requestsbankrko-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    57358 2023-07-26 10:43:27.000000 requestsbankrko-0.2.9/tests/test_bank_methods.py
```

### Comparing `requestsbankrko-0.2.8/LICENSE` & `requestsbankrko-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.8/PKG-INFO` & `requestsbankrko-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.8
+Version: 0.2.9
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.8/pyproject.toml` & `requestsbankrko-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "requestsbankrko"
-version = "0.2.8"
+version = "0.2.9"
 description = "Гарантированно успешные web-запросы в Банки РКО"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = [ "requestsgarant>=0.0.7", "requests>=2.28", "jsoncustom>=0.0.2", "python-dotenv>=0.20.0",]
 [[project.authors]]
 name = "plp-kolyan"
```

### Comparing `requestsbankrko-0.2.8/src/bank_methods.py` & `requestsbankrko-0.2.9/src/bank_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,14 +768,17 @@
         return self.do_json_wrapper()
 
     def get_response_production(self):
         self.args_request.update({'url': f'{self.url}?access-token={self.get_token()}'})
         r = super().get_response_production()
         return r
 
+    def do_json_wrapper(self):
+        return self.response_json
+
 
 class PSBScoring(PSBParent):
 
 
     def __init__(self, json_dict, test=test):
         super().__init__(test)
         self.json = json_dict
@@ -796,14 +799,16 @@
 class PSBdfmqueue(PSBParent):
     def __init__(self, json_dict, test):
         super().__init__(test)
         self.json = json_dict
         self.endpoint = f'/dfm/queue'
         self.method = 'post'
 
+
+
 class PSBdfmqueueid(PSBParent):
     def __init__(self, id, test):
         super().__init__(test)
         self.method = 'get'
         self.endpoint = f'/dfm/queue/{id}'
```

### Comparing `requestsbankrko-0.2.8/src/open_methods.py` & `requestsbankrko-0.2.9/src/open_methods.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.8/src/requestsbankrko.egg-info/PKG-INFO` & `requestsbankrko-0.2.9/src/requestsbankrko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requestsbankrko
-Version: 0.2.8
+Version: 0.2.9
 Summary: Гарантированно успешные web-запросы в Банки РКО
 Author-email: plp-kolyan <plp-kolyan@mail.ru>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `requestsbankrko-0.2.8/src/zip_functions.py` & `requestsbankrko-0.2.9/src/zip_functions.py`

 * *Files identical despite different names*

### Comparing `requestsbankrko-0.2.8/tests/test_bank_methods.py` & `requestsbankrko-0.2.9/tests/test_bank_methods.py`

 * *Files identical despite different names*

