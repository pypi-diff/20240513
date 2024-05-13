# Comparing `tmp/fastapi_elasticsearch_middleware-1.0.4.tar.gz` & `tmp/fastapi_elasticsearch_middleware-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.4.tar", last modified: Mon May 13 18:19:51 2024, max compression
+gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.6.tar", last modified: Mon May 13 18:22:25 2024, max compression
```

## Comparing `fastapi_elasticsearch_middleware-1.0.4.tar` & `fastapi_elasticsearch_middleware-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/elasticsearch_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:25.968108 fastapi_elasticsearch_middleware-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 18:22:16.000000 fastapi_elasticsearch_middleware-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:22:25.968108 fastapi_elasticsearch_middleware-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-13 18:22:16.000000 fastapi_elasticsearch_middleware-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:25.968108 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:16.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-13 18:22:16.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware/elasticsearch_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:22:25.968108 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:22:25.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:22:25.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:22:25.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:22:25.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:22:25.000000 fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:22:25.968108 fastapi_elasticsearch_middleware-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 18:22:16.000000 fastapi_elasticsearch_middleware-1.0.6/setup.py
```

### Comparing `fastapi_elasticsearch_middleware-1.0.4/LICENSE` & `fastapi_elasticsearch_middleware-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_elasticsearch_middleware-1.0.4/PKG-INFO` & `fastapi_elasticsearch_middleware-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_elasticsearch_middleware
-Version: 1.0.4
+Version: 1.0.6
 Summary: Elasticsearch Logger Middleware for FastAPI
 Home-page: https://github.com/GGontijo/fastapi-elasticsearch-middleware.git
 Author: Gabriel Gontijo
 Author-email: gabrieldercilio08@gmail.com
 Keywords: python,middleware,fastapi,elasticsearch,kibana,logstash,fastapi-middleware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_elasticsearch_middleware-1.0.4/README.md` & `fastapi_elasticsearch_middleware-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/elasticsearch_middleware.py` & `fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware/elasticsearch_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/PKG-INFO` & `fastapi_elasticsearch_middleware-1.0.6/fastapi_elasticsearch_middleware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_elasticsearch_middleware
-Version: 1.0.4
+Version: 1.0.6
 Summary: Elasticsearch Logger Middleware for FastAPI
 Home-page: https://github.com/GGontijo/fastapi-elasticsearch-middleware.git
 Author: Gabriel Gontijo
 Author-email: gabrieldercilio08@gmail.com
 Keywords: python,middleware,fastapi,elasticsearch,kibana,logstash,fastapi-middleware
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fastapi_elasticsearch_middleware-1.0.4/setup.py` & `fastapi_elasticsearch_middleware-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
   
 setup( 
     name='fastapi_elasticsearch_middleware', 
-    version='1.0.4', 
+    version='1.0.6', 
     url='https://github.com/GGontijo/fastapi-elasticsearch-middleware.git',
     description='Elasticsearch Logger Middleware for FastAPI',
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
     author='Gabriel Gontijo', 
     author_email='gabrieldercilio08@gmail.com', 
     packages=find_packages(),
```

