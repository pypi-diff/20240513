# Comparing `tmp/superblocks-types-0.0.3.tar.gz` & `tmp/superblocks-types-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.3.tar", last modified: Mon May 13 13:59:56 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.4.tar", last modified: Mon May 13 14:09:43 2024, max compression
```

## Comparing `superblocks-types-0.0.3.tar` & `superblocks-types-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,433 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:59:56.271715 superblocks-types-0.0.3/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 13:59:56.271350 superblocks-types-0.0.3/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.3/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 13:59:56.271800 superblocks-types-0.0.3/setup.cfg
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:59:56.271029 superblocks-types-0.0.3/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)      173 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 13:59:56.000000 superblocks-types-0.0.3/superblocks_types.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.097593 superblocks-types-0.0.4/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:09:43.097317 superblocks-types-0.0.4/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.4/README.md
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.014417 superblocks-types-0.0.4/gen/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.029512 superblocks-types-0.0.4/gen/py/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.030640 superblocks-types-0.0.4/gen/py/agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.031551 superblocks-types-0.0.4/gen/py/agent/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11149 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4565 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.031890 superblocks-types-0.0.4/gen/py/ai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.034399 superblocks-types-0.0.4/gen/py/ai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8400 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/ai_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/ai_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3053 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4325 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5300 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/vector_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/vector_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.034581 superblocks-types-0.0.4/gen/py/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.038527 superblocks-types-0.0.4/gen/py/api/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    39242 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2900 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/blocks_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/blocks_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7262 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8593 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10701 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7444 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    27119 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    28883 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.038827 superblocks-types-0.0.4/gen/py/auth/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.039501 superblocks-types-0.0.4/gen/py/auth/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/auth_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.039772 superblocks-types-0.0.4/gen/py/buf/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.041183 superblocks-types-0.0.4/gen/py/buf/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/expression_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.041795 superblocks-types-0.0.4/gen/py/buf/validate/priv/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)   136639 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042116 superblocks-types-0.0.4/gen/py/cache/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042743 superblocks-types-0.0.4/gen/py/cache/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/cache_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/cache_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042944 superblocks-types-0.0.4/gen/py/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.046362 superblocks-types-0.0.4/gen/py/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3864 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/common_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/common_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/errors_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/errors_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/health_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/health_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/language_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/language_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/plugin_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.046575 superblocks-types-0.0.4/gen/py/event/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.048176 superblocks-types-0.0.4/gen/py/event/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5954 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.049130 superblocks-types-0.0.4/gen/py/event/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.049439 superblocks-types-0.0.4/gen/py/google/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.050459 superblocks-types-0.0.4/gen/py/google/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1591 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/http_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.050663 superblocks-types-0.0.4/gen/py/intake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.051146 superblocks-types-0.0.4/gen/py/intake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/logs_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/logs_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.051348 superblocks-types-0.0.4/gen/py/integration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.052214 superblocks-types-0.0.4/gen/py/integration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2657 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/configuration_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/configuration_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3690 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.052487 superblocks-types-0.0.4/gen/py/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053098 superblocks-types-0.0.4/gen/py/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/kafka_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/kafka_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053311 superblocks-types-0.0.4/gen/py/plugins/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053446 superblocks-types-0.0.4/gen/py/plugins/adls/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.054308 superblocks-types-0.0.4/gen/py/plugins/adls/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5374 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.054513 superblocks-types-0.0.4/gen/py/plugins/athena/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.055118 superblocks-types-0.0.4/gen/py/plugins/athena/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2940 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.055329 superblocks-types-0.0.4/gen/py/plugins/bigquery/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.056056 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.056364 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.057069 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.057356 superblocks-types-0.0.4/gen/py/plugins/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.060496 superblocks-types-0.0.4/gen/py/plugins/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/auth_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1325 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/common_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/common_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2574 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/oauth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/oauth_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_field_metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_field_metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6530 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.060705 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.061385 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6310 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.061579 superblocks-types-0.0.4/gen/py/plugins/couchbase/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.062110 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4120 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.062405 superblocks-types-0.0.4/gen/py/plugins/custom/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063056 superblocks-types-0.0.4/gen/py/plugins/custom/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063265 superblocks-types-0.0.4/gen/py/plugins/databricks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063963 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2601 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064264 superblocks-types-0.0.4/gen/py/plugins/dynamodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064741 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064966 superblocks-types-0.0.4/gen/py/plugins/email/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.065565 superblocks-types-0.0.4/gen/py/plugins/email/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.065779 superblocks-types-0.0.4/gen/py/plugins/gcs/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.066354 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.066609 superblocks-types-0.0.4/gen/py/plugins/graphql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.067180 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2008 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.067488 superblocks-types-0.0.4/gen/py/plugins/gsheets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068077 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068260 superblocks-types-0.0.4/gen/py/plugins/javascript/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068706 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068947 superblocks-types-0.0.4/gen/py/plugins/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.069582 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     9925 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.069797 superblocks-types-0.0.4/gen/py/plugins/mariadb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.070278 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.070483 superblocks-types-0.0.4/gen/py/plugins/mongodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.071170 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.071427 superblocks-types-0.0.4/gen/py/plugins/mssql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072045 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072289 superblocks-types-0.0.4/gen/py/plugins/mysql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072786 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072995 superblocks-types-0.0.4/gen/py/plugins/ocr/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.073620 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.073840 superblocks-types-0.0.4/gen/py/plugins/openai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.074396 superblocks-types-0.0.4/gen/py/plugins/openai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.074591 superblocks-types-0.0.4/gen/py/plugins/oracledb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075044 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2461 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075253 superblocks-types-0.0.4/gen/py/plugins/pinecone/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075726 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3186 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075923 superblocks-types-0.0.4/gen/py/plugins/postgresql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.076413 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.076601 superblocks-types-0.0.4/gen/py/plugins/python/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.077075 superblocks-types-0.0.4/gen/py/plugins/python/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.077389 superblocks-types-0.0.4/gen/py/plugins/redis/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078068 superblocks-types-0.0.4/gen/py/plugins/redis/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13989 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078292 superblocks-types-0.0.4/gen/py/plugins/redshift/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078845 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079079 superblocks-types-0.0.4/gen/py/plugins/restapi/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079746 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2103 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079992 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.080570 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2509 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.080799 superblocks-types-0.0.4/gen/py/plugins/rockset/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081301 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081493 superblocks-types-0.0.4/gen/py/plugins/s3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081967 superblocks-types-0.0.4/gen/py/plugins/s3/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082191 superblocks-types-0.0.4/gen/py/plugins/salesforce/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082775 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5293 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082991 superblocks-types-0.0.4/gen/py/plugins/smtp/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.083459 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2551 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.083668 superblocks-types-0.0.4/gen/py/plugins/snowflake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084141 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084336 superblocks-types-0.0.4/gen/py/plugins/workflow/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084775 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2680 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.085294 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1462 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.085476 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.086543 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2316 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.086728 superblocks-types-0.0.4/gen/py/secrets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.087873 superblocks-types-0.0.4/gen/py/secrets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7599 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/secrets_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/secrets_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4880 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.088174 superblocks-types-0.0.4/gen/py/security/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.089952 superblocks-types-0.0.4/gen/py/security/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3141 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1263 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/security_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/security_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4830 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4519 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.090160 superblocks-types-0.0.4/gen/py/store/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091231 superblocks-types-0.0.4/gen/py/store/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3608 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4413 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1671 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091516 superblocks-types-0.0.4/gen/py/superblocks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091949 superblocks-types-0.0.4/gen/py/superblocks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/options_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/options_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.092690 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11323 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)      176 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.092863 superblocks-types-0.0.4/gen/py/syncer/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.093968 superblocks-types-0.0.4/gen/py/syncer/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8935 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11806 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3390 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/syncer_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/syncer_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.094186 superblocks-types-0.0.4/gen/py/transport/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.094838 superblocks-types-0.0.4/gen/py/transport/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13244 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/transport_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/transport_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.095028 superblocks-types-0.0.4/gen/py/utils/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.095492 superblocks-types-0.0.4/gen/py/utils/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096184 superblocks-types-0.0.4/gen/py/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096389 superblocks-types-0.0.4/gen/py/worker/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096989 superblocks-types-0.0.4/gen/py/worker/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1980 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10056 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 14:09:43.097673 superblocks-types-0.0.4/setup.cfg
```

### Comparing `superblocks-types-0.0.3/PKG-INFO` & `superblocks-types-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.3/README.md` & `superblocks-types-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.3/superblocks_types.egg-info/PKG-INFO` & `superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

