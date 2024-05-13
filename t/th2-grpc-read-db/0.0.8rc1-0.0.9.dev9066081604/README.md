# Comparing `tmp/th2_grpc_read_db-0.0.8rc1.tar.gz` & `tmp/th2_grpc_read_db-0.0.9.dev9066081604.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_read_db-0.0.8rc1.tar", last modified: Wed Mar 20 12:06:11 2024, max compression
+gzip compressed data, was "dist/th2_grpc_read_db-0.0.9.dev9066081604.tar", last modified: Mon May 13 16:03:35 2024, max compression
```

## Comparing `th2_grpc_read_db-0.0.8rc1.tar` & `th2_grpc_read_db-0.0.9.dev9066081604.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-20 12:04:47.000000 th2_grpc_read_db-0.0.8rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-20 12:04:47.000000 th2_grpc_read_db-0.0.8rc1/package_info.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-03-20 12:04:47.000000 th2_grpc_read_db-0.0.8rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-03-20 12:04:47.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db.proto
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-03-20 12:06:10.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-03-20 12:06:10.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-20 12:06:10.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-20 12:05:48.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-20 12:06:11.000000 th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-13 16:02:02.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db.proto
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14492 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-13 16:03:34.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-13 16:03:17.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 16:03:35.000000 th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/top_level.txt
```

### Comparing `th2_grpc_read_db-0.0.8rc1/PKG-INFO` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2_grpc_read_db
-Version: 0.0.8rc1
+Name: th2-grpc-read-db
+Version: 0.0.9.dev9066081604
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db (0.0.8)
         
@@ -13,14 +13,17 @@
         
         + request data synchronously - `Execute` method. This method returns rows as stream.
         + run data loading synchronously - `Load` method. This method returns aggregated execution report.
         + submit pulling requests and stop them - `StartPulling` and `StopPulling` methods
         
         # Release notes:
         
+        ## 0.0.9
+        + updated grpc-common: `4.5.0-dev`
+        
         ## 0.0.8
         + added `Load` method
         
         ## 0.0.7
         + added execution_id to the QueryResponse
         + added parent_event_id to the QueryRequest
```

### Comparing `th2_grpc_read_db-0.0.8rc1/README.md` & `th2_grpc_read_db-0.0.9.dev9066081604/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 + request data synchronously - `Execute` method. This method returns rows as stream.
 + run data loading synchronously - `Load` method. This method returns aggregated execution report.
 + submit pulling requests and stop them - `StartPulling` and `StopPulling` methods
 
 # Release notes:
 
+## 0.0.9
++ updated grpc-common: `4.5.0-dev`
+
 ## 0.0.8
 + added `Load` method
 
 ## 0.0.7
 + added execution_id to the QueryResponse
 + added parent_event_id to the QueryRequest
```

### Comparing `th2_grpc_read_db-0.0.8rc1/setup.py` & `th2_grpc_read_db-0.0.9.dev9066081604/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     author='TH2-devs',
     author_email='th2-devs@exactprosystems.com',
     url='https://github.com/th2-net/th2-read-db',
     license='Apache License 2.0',
     python_requires='>=3.7',
     install_requires=[
         'grpcio-tools==1.56.0',
-        'th2-grpc-common==4.3.0.dev0',
+        'th2-grpc-common==4.5.0rc1',
         'mypy-protobuf==3.4'
     ],
     packages=packages,
     package_data=package_data,
     cmdclass={
         'generate': ProtoGenerator,
         'sdist': CustomDist
```

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db.proto` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2.py` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2.pyi` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2.pyi`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_pb2_grpc.py` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db/read_db_service.py` & `th2_grpc_read_db-0.0.9.dev9066081604/th2_grpc_read_db/read_db_service.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_read_db-0.0.8rc1/th2_grpc_read_db.egg-info/PKG-INFO` & `th2_grpc_read_db-0.0.9.dev9066081604/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: th2-grpc-read-db
-Version: 0.0.8rc1
+Name: th2_grpc_read_db
+Version: 0.0.9.dev9066081604
 Summary: th2_grpc_read_db
 Home-page: https://github.com/th2-net/th2-read-db
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
 Description: # gRPC for read-db (0.0.8)
         
@@ -13,14 +13,17 @@
         
         + request data synchronously - `Execute` method. This method returns rows as stream.
         + run data loading synchronously - `Load` method. This method returns aggregated execution report.
         + submit pulling requests and stop them - `StartPulling` and `StopPulling` methods
         
         # Release notes:
         
+        ## 0.0.9
+        + updated grpc-common: `4.5.0-dev`
+        
         ## 0.0.8
         + added `Load` method
         
         ## 0.0.7
         + added execution_id to the QueryResponse
         + added parent_event_id to the QueryRequest
```

