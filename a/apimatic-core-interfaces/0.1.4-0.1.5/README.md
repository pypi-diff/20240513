# Comparing `tmp/apimatic-core-interfaces-0.1.4.tar.gz` & `tmp/apimatic_core_interfaces-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimatic-core-interfaces-0.1.4.tar", last modified: Mon Jul 24 06:43:23 2023, max compression
+gzip compressed data, was "apimatic_core_interfaces-0.1.5.tar", last modified: Mon May 13 06:06:20 2024, max compression
```

## Comparing `apimatic-core-interfaces-0.1.4.tar` & `apimatic_core_interfaces-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/factories/response_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/http_method_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/union_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 06:43:23.000000 apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 06:43:23.497318 apimatic-core-interfaces-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-24 06:43:09.000000 apimatic-core-interfaces-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/client/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/factories/response_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/logger/api_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/http_method_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/union_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-13 06:06:20.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-13 06:06:20.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 06:06:20.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 06:06:20.000000 apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 06:06:20.762303 apimatic_core_interfaces-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 06:06:12.000000 apimatic_core_interfaces-0.1.5/setup.py
```

### Comparing `apimatic-core-interfaces-0.1.4/LICENSE` & `apimatic_core_interfaces-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.4/PKG-INFO` & `apimatic_core_interfaces-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core-interfaces
-Version: 0.1.4
+Version: 0.1.5
 Summary: An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter and APIMatic SDKs.
 Home-page: https://github.com/apimatic/core-interfaces-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,16 @@
 ## Interfaces
 | Name                                                                        | Description                                                                               |
 |-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
 | [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
 | [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
 | [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
 | [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
-
+| [`Logger`](apimatic_core_interfaces/logger/logger.py)                       | An interface for the generic logger facade                                                |
+| [`ApiLogger`](apimatic_core_interfaces/logger/api_logger.py)                | An interface for logging API requests and responses                                       |
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core-interfaces
```

### Comparing `apimatic-core-interfaces-0.1.4/README.md` & `apimatic_core_interfaces-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 ## Interfaces
 | Name                                                                        | Description                                                                               |
 |-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
 | [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
 | [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
 | [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
 | [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
-
+| [`Logger`](apimatic_core_interfaces/logger/logger.py)                       | An interface for the generic logger facade                                                |
+| [`ApiLogger`](apimatic_core_interfaces/logger/api_logger.py)                | An interface for logging API requests and responses                                       |
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core-interfaces
```

### Comparing `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/client/http_client.py` & `apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/client/http_client.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/http_method_enum.py` & `apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/http_method_enum.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces/types/union_type.py` & `apimatic_core_interfaces-0.1.5/apimatic_core_interfaces/types/union_type.py`

 * *Files identical despite different names*

### Comparing `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/PKG-INFO` & `apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimatic-core-interfaces
-Version: 0.1.4
+Version: 0.1.5
 Summary: An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter and APIMatic SDKs.
 Home-page: https://github.com/apimatic/core-interfaces-python
 Author: APIMatic
 Author-email: support@apimatic.io
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -28,15 +28,16 @@
 ## Interfaces
 | Name                                                                        | Description                                                                               |
 |-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------|
 | [`HttpClient`](apimatic_core_interfaces/client/http_client.py)              | To save both Request and Response after the completion of response                        |
 | [`ResponseFactory`](apimatic_core_interfaces/factories/response_factory.py) | To convert the client-adapter response into a custom HTTP response                        |
 | [`Authentication`](apimatic_core_interfaces/types/authentication.py)        | To setup methods for the validation and application of the required authentication scheme |
 | [`UnionType`](apimatic_core_interfaces/types/union_type.py)                 | To setup methods for the validation and deserialization of OneOf/AnyOf union types        |
-
+| [`Logger`](apimatic_core_interfaces/logger/logger.py)                       | An interface for the generic logger facade                                                |
+| [`ApiLogger`](apimatic_core_interfaces/logger/api_logger.py)                | An interface for logging API requests and responses                                       |
 
 ## Enumerations
 | Name                                                                          | Description                                                     |
 |-------------------------------------------------------------------------------|-----------------------------------------------------------------|
 | [`HttpMethodEnum`](apimatic_core_interfaces/types/http_method_enum.py )       | Enumeration containig HTTP Methods (GET, POST, PATCH, DELETE)   |
 
 [pypi-version]: https://img.shields.io/pypi/v/apimatic-core-interfaces
```

### Comparing `apimatic-core-interfaces-0.1.4/apimatic_core_interfaces.egg-info/SOURCES.txt` & `apimatic_core_interfaces-0.1.5/apimatic_core_interfaces.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,11 +7,14 @@
 apimatic_core_interfaces.egg-info/SOURCES.txt
 apimatic_core_interfaces.egg-info/dependency_links.txt
 apimatic_core_interfaces.egg-info/top_level.txt
 apimatic_core_interfaces/client/__init__.py
 apimatic_core_interfaces/client/http_client.py
 apimatic_core_interfaces/factories/__init__.py
 apimatic_core_interfaces/factories/response_factory.py
+apimatic_core_interfaces/logger/__init__.py
+apimatic_core_interfaces/logger/api_logger.py
+apimatic_core_interfaces/logger/logger.py
 apimatic_core_interfaces/types/__init__.py
 apimatic_core_interfaces/types/authentication.py
 apimatic_core_interfaces/types/http_method_enum.py
 apimatic_core_interfaces/types/union_type.py
```

### Comparing `apimatic-core-interfaces-0.1.4/setup.py` & `apimatic_core_interfaces-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         long_description = fh.read()
 else:
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 
 setup(
     name='apimatic-core-interfaces',
-    version='0.1.4',
+    version='0.1.5',
     description='An abstract layer of the functionalities provided by apimatic-core-library, requests-client-adapter '
                 'and APIMatic SDKs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='APIMatic',
     author_email='support@apimatic.io',
     license='MIT',
```

