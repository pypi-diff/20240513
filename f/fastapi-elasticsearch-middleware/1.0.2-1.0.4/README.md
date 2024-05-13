# Comparing `tmp/fastapi_elasticsearch_middleware-1.0.2.tar.gz` & `tmp/fastapi_elasticsearch_middleware-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.2.tar", last modified: Mon May 13 17:15:52 2024, max compression
+gzip compressed data, was "fastapi_elasticsearch_middleware-1.0.4.tar", last modified: Mon May 13 18:19:51 2024, max compression
```

## Comparing `fastapi_elasticsearch_middleware-1.0.2.tar` & `fastapi_elasticsearch_middleware-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/elasticsearch_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 17:15:52.000000 fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:15:52.629089 fastapi_elasticsearch_middleware-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 17:15:48.000000 fastapi_elasticsearch_middleware-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7480 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/elasticsearch_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 18:19:51.000000 fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:19:51.747539 fastapi_elasticsearch_middleware-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-13 18:19:47.000000 fastapi_elasticsearch_middleware-1.0.4/setup.py
```

### Comparing `fastapi_elasticsearch_middleware-1.0.2/LICENSE` & `fastapi_elasticsearch_middleware-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_elasticsearch_middleware-1.0.2/fastapi_elasticsearch_middleware/elasticsearch_middleware.py` & `fastapi_elasticsearch_middleware-1.0.4/fastapi_elasticsearch_middleware/elasticsearch_middleware.py`

 * *Files identical despite different names*

