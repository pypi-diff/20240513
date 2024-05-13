# Comparing `tmp/fastapi_elasticsearch_middleware-1.0.1.tar.gz` & `tmp/fastapi_elasticsearch_middleware-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.1.tar", last modified: Mon May 13 16:52:10 2024, max compression
+gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.2.tar", last modified: Mon May 13 17:15:52 2024, max compression
```

## Comparing `fastapi_elasticsearch_middleware-1.0.1.tar` & `fastapi_elasticsearch_middleware-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:52:10.663292 fastapi_elasticsearch_middleware-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 16:52:10.663292 fastapi_elasticsearch_middleware-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 16:52:06.000000 fastapi_elasticsearch_middleware-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:52:10.663292 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-13 16:52:10.000000 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-13 16:52:10.000000 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:52:10.000000 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 16:52:10.000000 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:52:10.000000 fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:52:10.663292 fastapi_elasticsearch_middleware-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 16:52:06.000000 fastapi_elasticsearch_middleware-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/elasticsearch_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/setup.py
```

### Comparing `fastapi_elasticsearch_middleware-1.0.1/PKG-INFO` & `fastapi_elasticsearch_middleware-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi_elasticsearch_middleware
-Version: 1.0.1
+Version: 1.0.2
 Summary: Elasticsearch Logger Middleware for FastAPI
 Home-page: https://github.com/GGontijo/fastapi-elasticsearch-middleware.git
 Author: Gabriel Gontijo
 Author-email: gabrieldercilio08@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: elasticsearch
 
 # Elasticsearch Logger Middleware for FastAPI
 
 This middleware enables logging of requests and responses to Elasticsearch in a FastAPI application. It provides detailed logs including request method, URL path, query parameters, request and response headers, status code, and response body.
```

### Comparing `fastapi_elasticsearch_middleware-1.0.1/fastapi_elasticsearch_middleware.egg-info/PKG-INFO` & `fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: fastapi_elasticsearch_middleware
-Version: 1.0.1
+Version: 1.0.2
 Summary: Elasticsearch Logger Middleware for FastAPI
 Home-page: https://github.com/GGontijo/fastapi-elasticsearch-middleware.git
 Author: Gabriel Gontijo
 Author-email: gabrieldercilio08@gmail.com
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: fastapi
 Requires-Dist: elasticsearch
 
 # Elasticsearch Logger Middleware for FastAPI
 
 This middleware enables logging of requests and responses to Elasticsearch in a FastAPI application. It provides detailed logs including request method, URL path, query parameters, request and response headers, status code, and response body.
```

### Comparing `fastapi_elasticsearch_middleware-1.0.1/setup.py` & `fastapi_elasticsearch_middleware-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
   
 setup( 
     name='fastapi_elasticsearch_middleware', 
-    version='1.0.1', 
+    version='1.0.2', 
     url='https://github.com/GGontijo/fastapi-elasticsearch-middleware.git',
     description='Elasticsearch Logger Middleware for FastAPI',
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
     author='Gabriel Gontijo', 
     author_email='gabrieldercilio08@gmail.com', 
     packages=find_packages(),
```

