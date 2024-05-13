# Comparing `tmp/superblocks-types-0.0.4.tar.gz` & `tmp/superblocks-types-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.4.tar", last modified: Mon May 13 14:09:43 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.5.tar", last modified: Mon May 13 14:35:16 2024, max compression
```

## Comparing `superblocks-types-0.0.4.tar` & `superblocks-types-0.0.5.tar`

### file list

```diff
@@ -1,433 +1,425 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.097593 superblocks-types-0.0.4/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:09:43.097317 superblocks-types-0.0.4/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.4/README.md
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.014417 superblocks-types-0.0.4/gen/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.029512 superblocks-types-0.0.4/gen/py/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.030640 superblocks-types-0.0.4/gen/py/agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.031551 superblocks-types-0.0.4/gen/py/agent/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11149 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4565 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/agent/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.031890 superblocks-types-0.0.4/gen/py/ai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.034399 superblocks-types-0.0.4/gen/py/ai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8400 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/ai_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/ai_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3053 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4325 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5300 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/vector_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/ai/v1/vector_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.034581 superblocks-types-0.0.4/gen/py/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.038527 superblocks-types-0.0.4/gen/py/api/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    39242 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2900 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/blocks_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/blocks_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7262 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8593 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10701 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7444 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    27119 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    28883 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/api/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.038827 superblocks-types-0.0.4/gen/py/auth/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.039501 superblocks-types-0.0.4/gen/py/auth/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/auth/v1/auth_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.039772 superblocks-types-0.0.4/gen/py/buf/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.041183 superblocks-types-0.0.4/gen/py/buf/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/expression_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.041795 superblocks-types-0.0.4/gen/py/buf/validate/priv/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/private_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)   136639 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042116 superblocks-types-0.0.4/gen/py/cache/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042743 superblocks-types-0.0.4/gen/py/cache/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/cache_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/cache/v1/cache_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.042944 superblocks-types-0.0.4/gen/py/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.046362 superblocks-types-0.0.4/gen/py/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3864 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/common_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/common_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/errors_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/errors_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/health_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/health_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/language_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/language_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/plugin_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/common/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.046575 superblocks-types-0.0.4/gen/py/event/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.048176 superblocks-types-0.0.4/gen/py/event/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5954 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.049130 superblocks-types-0.0.4/gen/py/event/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/event/v2/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.049439 superblocks-types-0.0.4/gen/py/google/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.050459 superblocks-types-0.0.4/gen/py/google/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1591 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/http_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.050663 superblocks-types-0.0.4/gen/py/intake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.051146 superblocks-types-0.0.4/gen/py/intake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/logs_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/intake/v1/logs_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.051348 superblocks-types-0.0.4/gen/py/integration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.052214 superblocks-types-0.0.4/gen/py/integration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2657 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/configuration_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/configuration_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3690 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/integration/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.052487 superblocks-types-0.0.4/gen/py/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053098 superblocks-types-0.0.4/gen/py/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/kafka_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/kafka/v1/kafka_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053311 superblocks-types-0.0.4/gen/py/plugins/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.053446 superblocks-types-0.0.4/gen/py/plugins/adls/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.054308 superblocks-types-0.0.4/gen/py/plugins/adls/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5374 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/adls/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.054513 superblocks-types-0.0.4/gen/py/plugins/athena/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.055118 superblocks-types-0.0.4/gen/py/plugins/athena/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2940 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/athena/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.055329 superblocks-types-0.0.4/gen/py/plugins/bigquery/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.056056 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.056364 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.057069 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.057356 superblocks-types-0.0.4/gen/py/plugins/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.060496 superblocks-types-0.0.4/gen/py/plugins/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/auth_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1325 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/common_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/common_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2574 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/oauth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/oauth_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_field_metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_field_metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6530 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.060705 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.061385 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6310 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.061579 superblocks-types-0.0.4/gen/py/plugins/couchbase/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.062110 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4120 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.062405 superblocks-types-0.0.4/gen/py/plugins/custom/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063056 superblocks-types-0.0.4/gen/py/plugins/custom/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/custom/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063265 superblocks-types-0.0.4/gen/py/plugins/databricks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.063963 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2601 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/databricks/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064264 superblocks-types-0.0.4/gen/py/plugins/dynamodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064741 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.064966 superblocks-types-0.0.4/gen/py/plugins/email/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.065565 superblocks-types-0.0.4/gen/py/plugins/email/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/email/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.065779 superblocks-types-0.0.4/gen/py/plugins/gcs/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.066354 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gcs/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.066609 superblocks-types-0.0.4/gen/py/plugins/graphql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.067180 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2008 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/graphql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.067488 superblocks-types-0.0.4/gen/py/plugins/gsheets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068077 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068260 superblocks-types-0.0.4/gen/py/plugins/javascript/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068706 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/javascript/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.068947 superblocks-types-0.0.4/gen/py/plugins/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.069582 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     9925 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/kafka/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.069797 superblocks-types-0.0.4/gen/py/plugins/mariadb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.070278 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.070483 superblocks-types-0.0.4/gen/py/plugins/mongodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.071170 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.071427 superblocks-types-0.0.4/gen/py/plugins/mssql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072045 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mssql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072289 superblocks-types-0.0.4/gen/py/plugins/mysql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072786 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/mysql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.072995 superblocks-types-0.0.4/gen/py/plugins/ocr/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.073620 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/ocr/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.073840 superblocks-types-0.0.4/gen/py/plugins/openai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.074396 superblocks-types-0.0.4/gen/py/plugins/openai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/openai/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.074591 superblocks-types-0.0.4/gen/py/plugins/oracledb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075044 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2461 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075253 superblocks-types-0.0.4/gen/py/plugins/pinecone/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075726 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3186 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.075923 superblocks-types-0.0.4/gen/py/plugins/postgresql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.076413 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.076601 superblocks-types-0.0.4/gen/py/plugins/python/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.077075 superblocks-types-0.0.4/gen/py/plugins/python/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/python/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.077389 superblocks-types-0.0.4/gen/py/plugins/redis/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078068 superblocks-types-0.0.4/gen/py/plugins/redis/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13989 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redis/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078292 superblocks-types-0.0.4/gen/py/plugins/redshift/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.078845 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/redshift/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079079 superblocks-types-0.0.4/gen/py/plugins/restapi/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079746 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2103 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapi/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.079992 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.080570 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2509 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.080799 superblocks-types-0.0.4/gen/py/plugins/rockset/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081301 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/rockset/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081493 superblocks-types-0.0.4/gen/py/plugins/s3/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.081967 superblocks-types-0.0.4/gen/py/plugins/s3/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/s3/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082191 superblocks-types-0.0.4/gen/py/plugins/salesforce/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082775 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5293 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.082991 superblocks-types-0.0.4/gen/py/plugins/smtp/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.083459 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2551 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/smtp/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.083668 superblocks-types-0.0.4/gen/py/plugins/snowflake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084141 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084336 superblocks-types-0.0.4/gen/py/plugins/workflow/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.084775 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2680 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.085294 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1462 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/plugins/workflow/v2/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.085476 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.086543 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2316 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.086728 superblocks-types-0.0.4/gen/py/secrets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.087873 superblocks-types-0.0.4/gen/py/secrets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7599 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/secrets_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/secrets_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4880 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.088174 superblocks-types-0.0.4/gen/py/security/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.089952 superblocks-types-0.0.4/gen/py/security/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3141 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1263 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/security_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/security_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4830 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4519 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/security/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.090160 superblocks-types-0.0.4/gen/py/store/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091231 superblocks-types-0.0.4/gen/py/store/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3608 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4413 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1671 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/store/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091516 superblocks-types-0.0.4/gen/py/superblocks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.091949 superblocks-types-0.0.4/gen/py/superblocks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/options_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/superblocks/v1/options_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.092690 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)    11323 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)      176 2024-05-13 14:09:42.000000 superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.092863 superblocks-types-0.0.4/gen/py/syncer/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.093968 superblocks-types-0.0.4/gen/py/syncer/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8935 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11806 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3390 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/syncer_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/syncer/v1/syncer_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.094186 superblocks-types-0.0.4/gen/py/transport/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.094838 superblocks-types-0.0.4/gen/py/transport/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13244 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/transport_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/transport/v1/transport_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.095028 superblocks-types-0.0.4/gen/py/utils/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.095492 superblocks-types-0.0.4/gen/py/utils/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/utils/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096184 superblocks-types-0.0.4/gen/py/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096389 superblocks-types-0.0.4/gen/py/worker/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:09:43.096989 superblocks-types-0.0.4/gen/py/worker/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1980 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10056 2024-05-13 13:58:28.000000 superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 14:09:43.097673 superblocks-types-0.0.4/setup.cfg
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.456428 superblocks-types-0.0.5/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:35:16.456225 superblocks-types-0.0.5/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.5/README.md
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.324968 superblocks-types-0.0.5/gen/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.325169 superblocks-types-0.0.5/gen/py/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.342275 superblocks-types-0.0.5/gen/py/superblocks_types/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.343747 superblocks-types-0.0.5/gen/py/superblocks_types/agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.344658 superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11149 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4565 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.345234 superblocks-types-0.0.5/gen/py/superblocks_types/ai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.354189 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8400 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/ai_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/ai_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3053 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4325 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5300 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/vector_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/vector_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.355359 superblocks-types-0.0.5/gen/py/superblocks_types/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.373675 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    39242 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2900 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/blocks_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/blocks_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7262 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8593 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10701 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7444 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    27119 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    28883 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.374148 superblocks-types-0.0.5/gen/py/superblocks_types/auth/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/auth/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.375331 superblocks-types-0.0.5/gen/py/superblocks_types/auth/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/auth/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/auth/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/auth/v1/auth_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.376311 superblocks-types-0.0.5/gen/py/superblocks_types/buf/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.378275 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/expression_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.380795 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/priv/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/priv/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)   136639 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.381116 superblocks-types-0.0.5/gen/py/superblocks_types/cache/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/cache/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.382082 superblocks-types-0.0.5/gen/py/superblocks_types/cache/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/cache/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/cache/v1/cache_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/cache/v1/cache_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.383325 superblocks-types-0.0.5/gen/py/superblocks_types/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.391946 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3864 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/common_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/common_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/errors_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/errors_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/health_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/health_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/language_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/language_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/plugin_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.393484 superblocks-types-0.0.5/gen/py/superblocks_types/event/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.396514 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5954 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.398063 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.398430 superblocks-types-0.0.5/gen/py/superblocks_types/google/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.401409 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1591 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/http_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.402146 superblocks-types-0.0.5/gen/py/superblocks_types/intake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/intake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.403071 superblocks-types-0.0.5/gen/py/superblocks_types/intake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/intake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/intake/v1/logs_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/intake/v1/logs_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.403404 superblocks-types-0.0.5/gen/py/superblocks_types/integration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/integration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.404380 superblocks-types-0.0.5/gen/py/superblocks_types/integration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/integration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3690 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/integration/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/integration/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.404690 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.405314 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/v1/kafka_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/kafka/v1/kafka_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.405547 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.405770 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.406535 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5374 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.406844 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.407755 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2940 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.408063 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.408882 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.409216 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.410008 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.410434 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.412518 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/auth_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6530 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.412843 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.413548 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6310 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.413860 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.414548 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4120 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.414837 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.415430 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.415692 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.416221 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2601 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.416473 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.417150 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.417487 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.418184 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.418524 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.419283 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.419596 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.420290 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2008 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.420544 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.421241 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.421494 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.422188 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.422471 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.423218 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     9925 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.423473 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.424024 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.424266 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.424856 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.425130 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.425716 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.425948 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.426686 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.426951 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.427533 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.427844 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.428507 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.428737 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.429290 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2461 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.429576 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.430219 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3186 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.430493 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.431020 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.431246 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.431760 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.431990 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.432766 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13989 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.433000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.433557 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.433894 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.434512 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2103 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.434762 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.435260 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2509 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.435507 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.436156 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.436388 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.436992 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.437254 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.438094 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5293 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.438369 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.438923 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2551 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.439146 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.439717 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.439934 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.440435 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2680 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.441001 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1462 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.441219 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.442967 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2316 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.443282 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.444710 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7599 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/secrets_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/secrets_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4880 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.445011 superblocks-types-0.0.5/gen/py/superblocks_types/security/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.446522 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3141 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4830 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4519 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.446833 superblocks-types-0.0.5/gen/py/superblocks_types/store/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.448246 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3608 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4413 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1671 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.448556 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.449249 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/v1/options_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.449529 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.451195 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8935 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11806 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3390 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/syncer_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.451625 superblocks-types-0.0.5/gen/py/superblocks_types/transport/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/transport/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.452584 superblocks-types-0.0.5/gen/py/superblocks_types/transport/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/transport/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13244 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/transport/v1/transport_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/transport/v1/transport_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.452904 superblocks-types-0.0.5/gen/py/superblocks_types/utils/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/utils/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.453651 superblocks-types-0.0.5/gen/py/superblocks_types/utils/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/utils/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/utils/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/utils/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.454708 superblocks-types-0.0.5/gen/py/superblocks_types/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.455023 superblocks-types-0.0.5/gen/py/superblocks_types/worker/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/worker/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.455682 superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1980 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/step_executor_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10056 2024-05-13 14:34:25.000000 superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-13 14:35:16.343528 superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-13 14:35:16.000000 superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)    16191 2024-05-13 14:35:16.000000 superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-13 14:35:16.000000 superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       18 2024-05-13 14:35:16.000000 superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/top_level.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-13 14:35:16.456505 superblocks-types-0.0.5/setup.cfg
```

### Comparing `superblocks-types-0.0.4/PKG-INFO` & `superblocks-types-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.4/README.md` & `superblocks-types-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/agent/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/agent/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/ai/v1/ai_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/ai_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/ai/v1/metadata_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/ai/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/ai/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/ai/v1/vector_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/ai/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/api_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/blocks_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/blocks_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/event_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/integration_auth_service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/requests_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/requests_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/api/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/api/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/auth/v1/auth_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/auth/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/buf/validate/expression_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/buf/validate/priv/private_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/buf/validate/validate_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/cache/v1/cache_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/cache/v1/cache_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/api_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/common_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/errors_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/health_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/language_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/language_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/common/v1/utils_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/common/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v1/cloudevent_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v1/event_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v2/cloudevent_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v2/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/event/v2/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/event/v2/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/google/api/annotations_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/google/api/http_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/intake/v1/logs_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/intake/v1/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/integration/v1/configuration_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/superblocks/v1/options_pb2.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: integration/v1/configuration.proto
+# source: superblocks/v1/options.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
-from gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.gen.api.v1 import service_pb2 as api_dot_v1_dot_service__pb2
+from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"integration/v1/configuration.proto\x12\x0eintegration.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x16\x63ommon/v1/errors.proto\x1a\x14\x61pi/v1/service.proto\"n\n\x18GetConfigurationsRequest\x12)\n\x07profile\x18\x01 \x01(\x0b\x32\x0f.api.v1.ProfileR\x07profile\x12\'\n\x0fintegration_ids\x18\x02 \x03(\tR\x0eintegrationIds\"\x86\x02\n\x19GetConfigurationsResponse\x12\x65\n\x0e\x63onfigurations\x18\x01 \x03(\x0b\x32=.integration.v1.GetConfigurationsResponse.ConfigurationsEntryR\x0e\x63onfigurations\x12&\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\x1aZ\n\x13\x43onfigurationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x05value:\x02\x38\x01\x42\x38Z6github.com/superblocksteam/types/gen/go/integration/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1csuperblocks/v1/options.proto\x12\x0esuperblocks.v1\x1a google/protobuf/descriptor.proto\"*\n\x0cIntegrations\x12\x1a\n\x08registry\x18\x01 \x01(\x08R\x08registry\":\n\x12IntegrationOptions\x12\x1e\n\npluginType\x18\x02 \x01(\tR\npluginTypeJ\x04\x08\x01\x10\x02:c\n\x0cintegrations\x12\x1f.google.protobuf.MessageOptions\x18\xd0\x86\x03 \x01(\x0b\x32\x1c.superblocks.v1.IntegrationsR\x0cintegrations:t\n\x13integration_options\x12\x1d.google.protobuf.FieldOptions\x18\xe0\xd4\x03 \x01(\x0b\x32\".superblocks.v1.IntegrationOptionsR\x12integrationOptionsB8Z6github.com/superblocksteam/types/gen/go/superblocks/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'integration.v1.configuration_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z6github.com/superblocksteam/types/gen/go/integration/v1'
-  _GETCONFIGURATIONSRESPONSE_CONFIGURATIONSENTRY._options = None
-  _GETCONFIGURATIONSRESPONSE_CONFIGURATIONSENTRY._serialized_options = b'8\001'
-  _globals['_GETCONFIGURATIONSREQUEST']._serialized_start=130
-  _globals['_GETCONFIGURATIONSREQUEST']._serialized_end=240
-  _globals['_GETCONFIGURATIONSRESPONSE']._serialized_start=243
-  _globals['_GETCONFIGURATIONSRESPONSE']._serialized_end=505
-  _globals['_GETCONFIGURATIONSRESPONSE_CONFIGURATIONSENTRY']._serialized_start=415
-  _globals['_GETCONFIGURATIONSRESPONSE_CONFIGURATIONSENTRY']._serialized_end=505
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'superblocks.v1.options_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z6github.com/superblocksteam/types/gen/go/superblocks/v1'
+  _globals['_INTEGRATIONS']._serialized_start=82
+  _globals['_INTEGRATIONS']._serialized_end=124
+  _globals['_INTEGRATIONOPTIONS']._serialized_start=126
+  _globals['_INTEGRATIONOPTIONS']._serialized_end=184
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/integration/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/integration/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/kafka/v1/kafka_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/kafka/v1/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/adls/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/athena/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/bigquery/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/cockroachdb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/auth_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/common_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/common/v1/common.proto
+# source: plugins/workflow/v2/plugin.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from gen.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eplugins/common/v1/common.proto\x12\x11plugins.common.v1\"T\n\x16SQLActionConfiguration\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12&\n\x0eusePreparedSql\x18\x02 \x01(\x08R\x0eusePreparedSqlB;Z9github.com/superblocksteam/types/gen/go/plugins/common/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/workflow/v2/plugin.proto\x12\x13plugins.workflow.v2\x1a\x16\x63ommon/v1/plugin.proto\"S\n\x06Plugin\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x39\n\nparameters\x18\x02 \x01(\x0b\x32\x19.common.v1.HttpParametersR\nparametersB=Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.common.v1.common_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/superblocksteam/types/gen/go/plugins/common/v1'
-  _globals['_SQLACTIONCONFIGURATION']._serialized_start=53
-  _globals['_SQLACTIONCONFIGURATION']._serialized_end=137
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.workflow.v2.plugin_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v2'
+  _globals['_PLUGIN']._serialized_start=81
+  _globals['_PLUGIN']._serialized_end=164
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/metadata_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/oauth_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/common/v1/oauth.proto
+# source: plugins/s3/v1/plugin.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dplugins/common/v1/oauth.proto\x12\x11plugins.common.v1\"\xbb\x02\n\x05OAuth\x1a\xaa\x01\n\x11PasswordGrantFlow\x12\x1b\n\tclient_id\x18\x02 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x03 \x01(\tR\x0c\x63lientSecret\x12\x1b\n\ttoken_url\x18\x04 \x01(\tR\x08tokenUrl\x12\x1a\n\x08username\x18\x05 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x06 \x01(\tR\x08password\x1a\x84\x01\n\x08\x43odeFlow\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\x12\x1b\n\ttoken_url\x18\x03 \x01(\tR\x08tokenUrl\x12\x19\n\x08\x61uth_url\x18\x04 \x01(\tR\x07\x61uthUrl\"?\n\x05\x42\x61sic\x12\x1a\n\x08username\x18\x01 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x02 \x01(\tR\x08password\"\xe0\x01\n\x04\x41uth\x12\\\n\x13password_grant_flow\x18\x01 \x01(\x0b\x32*.plugins.common.v1.OAuth.PasswordGrantFlowH\x00R\x11passwordGrantFlow\x12@\n\tcode_flow\x18\x02 \x01(\x0b\x32!.plugins.common.v1.OAuth.CodeFlowH\x00R\x08\x63odeFlow\x12\x30\n\x05\x62\x61sic\x18\x03 \x01(\x0b\x32\x18.plugins.common.v1.BasicH\x00R\x05\x62\x61sicB\x06\n\x04\x61uthB;Z9github.com/superblocksteam/types/gen/go/plugins/common/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aplugins/s3/v1/plugin.proto\x12\rplugins.s3.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"\xbe\x02\n\x08Property\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value\x12\x1a\n\x08\x65\x64itable\x18\x03 \x01(\x08R\x08\x65\x64itable\x12\x1a\n\x08internal\x18\x04 \x01(\x08R\x08internal\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x1c\n\tmandatory\x18\x06 \x01(\x08R\tmandatory\x12\x12\n\x04type\x18\x07 \x01(\tR\x04type\x12\"\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1a\n\x08minRange\x18\t \x01(\tR\x08minRange\x12\x1a\n\x08maxRange\x18\n \x01(\tR\x08maxRange\x12\"\n\x0cvalueOptions\x18\x0b \x03(\tR\x0cvalueOptions\"S\n\x06\x43ustom\x12I\n\x13presignedExpiration\x18\x01 \x01(\x0b\x32\x17.plugins.s3.v1.PropertyR\x13presignedExpiration\"\xaf\x02\n\x06Plugin\x12\x1a\n\x08resource\x18\x01 \x01(\tR\x08resource\x12\x16\n\x06\x61\x63tion\x18\x02 \x01(\tR\x06\x61\x63tion\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x12\n\x04\x62ody\x18\x04 \x01(\tR\x04\x62ody\x12 \n\x0b\x66ileObjects\x18\x05 \x01(\tR\x0b\x66ileObjects\x12\"\n\x0cresponseType\x18\x06 \x01(\tR\x0cresponseType\x12-\n\x06\x63ustom\x18\x07 \x01(\x0b\x32\x15.plugins.s3.v1.CustomR\x06\x63ustom\x12T\n\x13superblocksMetadata\x18\x08 \x01(\x0b\x32\".plugins.s3.v1.SuperblocksMetadataR\x13superblocksMetadataB7Z5github.com/superblocksteam/types/gen/go/plugins/s3/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.common.v1.oauth_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/superblocksteam/types/gen/go/plugins/common/v1'
-  _globals['_OAUTH']._serialized_start=53
-  _globals['_OAUTH']._serialized_end=368
-  _globals['_OAUTH_PASSWORDGRANTFLOW']._serialized_start=63
-  _globals['_OAUTH_PASSWORDGRANTFLOW']._serialized_end=233
-  _globals['_OAUTH_CODEFLOW']._serialized_start=236
-  _globals['_OAUTH_CODEFLOW']._serialized_end=368
-  _globals['_BASIC']._serialized_start=370
-  _globals['_BASIC']._serialized_end=433
-  _globals['_AUTH']._serialized_start=436
-  _globals['_AUTH']._serialized_end=660
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.s3.v1.plugin_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z5github.com/superblocksteam/types/gen/go/plugins/s3/v1'
+  _globals['_SUPERBLOCKSMETADATA']._serialized_start=45
+  _globals['_SUPERBLOCKSMETADATA']._serialized_end=104
+  _globals['_PROPERTY']._serialized_start=107
+  _globals['_PROPERTY']._serialized_end=425
+  _globals['_CUSTOM']._serialized_start=427
+  _globals['_CUSTOM']._serialized_end=510
+  _globals['_PLUGIN']._serialized_start=513
+  _globals['_PLUGIN']._serialized_end=816
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_field_metadata_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/common/v1/plugin_field_metadata.proto
+# source: plugins/javascript/v1/plugin.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n-plugins/common/v1/plugin_field_metadata.proto\x12\x11plugins.common.v1\x1a google/protobuf/descriptor.proto\"K\n\x0fPluginFieldMeta\x12\x1b\n\tis_public\x18\x01 \x01(\x08R\x08isPublic\x12\x1b\n\tis_secret\x18\x02 \x01(\x08R\x08isSecret:o\n\x11plugin_field_meta\x12\x1d.google.protobuf.FieldOptions\x18\xd1\x86\x03 \x01(\x0b\x32\".plugins.common.v1.PluginFieldMetaR\x0fpluginFieldMetaB;Z9github.com/superblocksteam/types/gen/go/plugins/common/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"plugins/javascript/v1/plugin.proto\x12\x15plugins.javascript.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"z\n\x06Plugin\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12\\\n\x13superblocksMetadata\x18\x02 \x01(\x0b\x32*.plugins.javascript.v1.SuperblocksMetadataR\x13superblocksMetadataB?Z=github.com/superblocksteam/types/gen/go/plugins/javascript/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.common.v1.plugin_field_metadata_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z9github.com/superblocksteam/types/gen/go/plugins/common/v1'
-  _globals['_PLUGINFIELDMETA']._serialized_start=102
-  _globals['_PLUGINFIELDMETA']._serialized_end=177
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.javascript.v1.plugin_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/superblocksteam/types/gen/go/plugins/javascript/v1'
+  _globals['_SUPERBLOCKSMETADATA']._serialized_start=61
+  _globals['_SUPERBLOCKSMETADATA']._serialized_end=120
+  _globals['_PLUGIN']._serialized_start=122
+  _globals['_PLUGIN']._serialized_end=244
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/common/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/cosmosdb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/couchbase/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/custom/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/databricks/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/dynamodb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/email/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/gcs/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/graphql/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/gsheets/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/javascript/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/javascript/v1/plugin.proto
+# source: plugins/python/v1/plugin.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"plugins/javascript/v1/plugin.proto\x12\x15plugins.javascript.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"z\n\x06Plugin\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12\\\n\x13superblocksMetadata\x18\x02 \x01(\x0b\x32*.plugins.javascript.v1.SuperblocksMetadataR\x13superblocksMetadataB?Z=github.com/superblocksteam/types/gen/go/plugins/javascript/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eplugins/python/v1/plugin.proto\x12\x11plugins.python.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"v\n\x06Plugin\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12X\n\x13superblocksMetadata\x18\x02 \x01(\x0b\x32&.plugins.python.v1.SuperblocksMetadataR\x13superblocksMetadataB;Z9github.com/superblocksteam/types/gen/go/plugins/python/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.javascript.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.python.v1.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z=github.com/superblocksteam/types/gen/go/plugins/javascript/v1'
-  _globals['_SUPERBLOCKSMETADATA']._serialized_start=61
-  _globals['_SUPERBLOCKSMETADATA']._serialized_end=120
-  _globals['_PLUGIN']._serialized_start=122
-  _globals['_PLUGIN']._serialized_end=244
+  _globals['DESCRIPTOR']._serialized_options = b'Z9github.com/superblocksteam/types/gen/go/plugins/python/v1'
+  _globals['_SUPERBLOCKSMETADATA']._serialized_start=53
+  _globals['_SUPERBLOCKSMETADATA']._serialized_end=112
+  _globals['_PLUGIN']._serialized_start=114
+  _globals['_PLUGIN']._serialized_end=232
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/kafka/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/mariadb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/mongodb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/mssql/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/mysql/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/ocr/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/openai/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/oracledb/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/pinecone/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/postgresql/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/python/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/python/v1/plugin.proto
+# source: plugins/restapi/v1/plugin.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from gen.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eplugins/python/v1/plugin.proto\x12\x11plugins.python.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"v\n\x06Plugin\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12X\n\x13superblocksMetadata\x18\x02 \x01(\x0b\x32&.plugins.python.v1.SuperblocksMetadataR\x13superblocksMetadataB;Z9github.com/superblocksteam/types/gen/go/plugins/python/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fplugins/restapi/v1/plugin.proto\x12\x12plugins.restapi.v1\x1a\x16\x63ommon/v1/plugin.proto\"\xc9\x03\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12/\n\x08\x66ormData\x18\x07 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\x08 \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\t \x01(\tR\x08\x66ileName\x12\x12\n\x04path\x18\n \x01(\tR\x04path\x12\x1a\n\x08jsonBody\x18\x0b \x01(\tR\x08jsonBody\x12P\n\x13superblocksMetadata\x18\x0c \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadataB<Z:github.com/superblocksteam/types/gen/go/plugins/restapi/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.python.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapi.v1.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z9github.com/superblocksteam/types/gen/go/plugins/python/v1'
-  _globals['_SUPERBLOCKSMETADATA']._serialized_start=53
-  _globals['_SUPERBLOCKSMETADATA']._serialized_end=112
-  _globals['_PLUGIN']._serialized_start=114
-  _globals['_PLUGIN']._serialized_end=232
+  _globals['DESCRIPTOR']._serialized_options = b'Z:github.com/superblocksteam/types/gen/go/plugins/restapi/v1'
+  _globals['_PLUGIN']._serialized_start=80
+  _globals['_PLUGIN']._serialized_end=537
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/redis/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/redshift/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/restapi/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/restapi/v1/plugin.proto
+# source: plugins/restapiintegration/v1/plugin.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from gen.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fplugins/restapi/v1/plugin.proto\x12\x12plugins.restapi.v1\x1a\x16\x63ommon/v1/plugin.proto\"\xc9\x03\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12/\n\x08\x66ormData\x18\x07 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\x08 \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\t \x01(\tR\x08\x66ileName\x12\x12\n\x04path\x18\n \x01(\tR\x04path\x12\x1a\n\x08jsonBody\x18\x0b \x01(\tR\x08jsonBody\x12P\n\x13superblocksMetadata\x18\x0c \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadataB<Z:github.com/superblocksteam/types/gen/go/plugins/restapi/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*plugins/restapiintegration/v1/plugin.proto\x12\x1dplugins.restapiintegration.v1\x1a\x16\x63ommon/v1/plugin.proto\"\x9c\x05\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12\x1a\n\x08jsonBody\x18\x07 \x01(\tR\x08jsonBody\x12/\n\x08\x66ormData\x18\x08 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\t \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\n \x01(\tR\x08\x66ileName\x12\x18\n\x07urlBase\x18\x0b \x01(\tR\x07urlBase\x12\x18\n\x07urlPath\x18\x0c \x01(\tR\x07urlPath\x12\x1a\n\x08\x61uthType\x18\r \x01(\tR\x08\x61uthType\x12P\n\x13superblocksMetadata\x18\x0e \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadata\x12$\n\ropenApiAction\x18\x0f \x01(\tR\ropenApiAction\x12&\n\x0eopenApiSpecRef\x18\x10 \x01(\tR\x0eopenApiSpecRef\x12\x31\n\x11openApiTenantName\x18\x11 \x01(\tH\x00R\x11openApiTenantName\x88\x01\x01\x42\x14\n\x12_openApiTenantNameBGZEgithub.com/superblocksteam/types/gen/go/plugins/restapiintegration/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapi.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapiintegration.v1.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z:github.com/superblocksteam/types/gen/go/plugins/restapi/v1'
-  _globals['_PLUGIN']._serialized_start=80
-  _globals['_PLUGIN']._serialized_end=537
+  _globals['DESCRIPTOR']._serialized_options = b'ZEgithub.com/superblocksteam/types/gen/go/plugins/restapiintegration/v1'
+  _globals['_PLUGIN']._serialized_start=102
+  _globals['_PLUGIN']._serialized_end=770
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/restapiintegration/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/restapiintegration/v1/plugin.proto
+# source: plugins/smtp/v1/plugin.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gen.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from gen.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*plugins/restapiintegration/v1/plugin.proto\x12\x1dplugins.restapiintegration.v1\x1a\x16\x63ommon/v1/plugin.proto\"\x9c\x05\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12\x1a\n\x08jsonBody\x18\x07 \x01(\tR\x08jsonBody\x12/\n\x08\x66ormData\x18\x08 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\t \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\n \x01(\tR\x08\x66ileName\x12\x18\n\x07urlBase\x18\x0b \x01(\tR\x07urlBase\x12\x18\n\x07urlPath\x18\x0c \x01(\tR\x07urlPath\x12\x1a\n\x08\x61uthType\x18\r \x01(\tR\x08\x61uthType\x12P\n\x13superblocksMetadata\x18\x0e \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadata\x12$\n\ropenApiAction\x18\x0f \x01(\tR\ropenApiAction\x12&\n\x0eopenApiSpecRef\x18\x10 \x01(\tR\x0eopenApiSpecRef\x12\x31\n\x11openApiTenantName\x18\x11 \x01(\tH\x00R\x11openApiTenantName\x88\x01\x01\x42\x14\n\x12_openApiTenantNameBGZEgithub.com/superblocksteam/types/gen/go/plugins/restapiintegration/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cplugins/smtp/v1/plugin.proto\x12\x0fplugins.smtp.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xdd\x04\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12\x46\n\nconnection\x18\x02 \x01(\x0b\x32&.plugins.smtp.v1.Plugin.SmtpConnectionR\nconnection\x12\x12\n\x04\x66rom\x18\x03 \x01(\tR\x04\x66rom\x12\x19\n\x08reply_to\x18\x04 \x01(\tR\x07replyTo\x12\x0e\n\x02to\x18\x05 \x01(\tR\x02to\x12\x0e\n\x02\x63\x63\x18\x06 \x01(\tR\x02\x63\x63\x12\x10\n\x03\x62\x63\x63\x18\x07 \x01(\tR\x03\x62\x63\x63\x12\x18\n\x07subject\x18\x08 \x01(\tR\x07subject\x12\x12\n\x04\x62ody\x18\t \x01(\tR\x04\x62ody\x12 \n\x0b\x61ttachments\x18\n \x01(\tR\x0b\x61ttachments\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x0b \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\x98\x01\n\x0eSmtpConnection\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12\x1a\n\x08username\x18\x03 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x04 \x01(\tR\x08password\x12\x1b\n\x06secure\x18\x05 \x01(\x08H\x00R\x06secure\x88\x01\x01\x42\t\n\x07_secureB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB9Z7github.com/superblocksteam/types/gen/go/plugins/smtp/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapiintegration.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.smtp.v1.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'ZEgithub.com/superblocksteam/types/gen/go/plugins/restapiintegration/v1'
-  _globals['_PLUGIN']._serialized_start=102
-  _globals['_PLUGIN']._serialized_end=770
+  _globals['DESCRIPTOR']._serialized_options = b'Z7github.com/superblocksteam/types/gen/go/plugins/smtp/v1'
+  _globals['_PLUGIN']._serialized_start=82
+  _globals['_PLUGIN']._serialized_end=687
+  _globals['_PLUGIN_SMTPCONNECTION']._serialized_start=491
+  _globals['_PLUGIN_SMTPCONNECTION']._serialized_end=643
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/rockset/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/s3/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/s3/v1/plugin.proto
+# source: plugins/workflow/v1/plugin.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from gen.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aplugins/s3/v1/plugin.proto\x12\rplugins.s3.v1\";\n\x13SuperblocksMetadata\x12$\n\rpluginVersion\x18\x01 \x01(\tR\rpluginVersion\"\xbe\x02\n\x08Property\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x05R\x05value\x12\x1a\n\x08\x65\x64itable\x18\x03 \x01(\x08R\x08\x65\x64itable\x12\x1a\n\x08internal\x18\x04 \x01(\x08R\x08internal\x12 \n\x0b\x64\x65scription\x18\x05 \x01(\tR\x0b\x64\x65scription\x12\x1c\n\tmandatory\x18\x06 \x01(\x08R\tmandatory\x12\x12\n\x04type\x18\x07 \x01(\tR\x04type\x12\"\n\x0c\x64\x65\x66\x61ultValue\x18\x08 \x01(\tR\x0c\x64\x65\x66\x61ultValue\x12\x1a\n\x08minRange\x18\t \x01(\tR\x08minRange\x12\x1a\n\x08maxRange\x18\n \x01(\tR\x08maxRange\x12\"\n\x0cvalueOptions\x18\x0b \x03(\tR\x0cvalueOptions\"S\n\x06\x43ustom\x12I\n\x13presignedExpiration\x18\x01 \x01(\x0b\x32\x17.plugins.s3.v1.PropertyR\x13presignedExpiration\"\xaf\x02\n\x06Plugin\x12\x1a\n\x08resource\x18\x01 \x01(\tR\x08resource\x12\x16\n\x06\x61\x63tion\x18\x02 \x01(\tR\x06\x61\x63tion\x12\x12\n\x04path\x18\x03 \x01(\tR\x04path\x12\x12\n\x04\x62ody\x18\x04 \x01(\tR\x04\x62ody\x12 \n\x0b\x66ileObjects\x18\x05 \x01(\tR\x0b\x66ileObjects\x12\"\n\x0cresponseType\x18\x06 \x01(\tR\x0cresponseType\x12-\n\x06\x63ustom\x18\x07 \x01(\x0b\x32\x15.plugins.s3.v1.CustomR\x06\x63ustom\x12T\n\x13superblocksMetadata\x18\x08 \x01(\x0b\x32\".plugins.s3.v1.SuperblocksMetadataR\x13superblocksMetadataB7Z5github.com/superblocksteam/types/gen/go/plugins/s3/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/workflow/v1/plugin.proto\x12\x13plugins.workflow.v1\x1a\x16\x63ommon/v1/plugin.proto\"/\n\x05Tuple\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"\xac\x03\n\x06Plugin\x12\x1a\n\x08workflow\x18\x01 \x01(\tR\x08workflow\x12?\n\x06\x63ustom\x18\x02 \x03(\x0b\x32\'.plugins.workflow.v1.Plugin.CustomEntryR\x06\x63ustom\x12N\n\x0bqueryParams\x18\x03 \x03(\x0b\x32,.plugins.workflow.v1.Plugin.QueryParamsEntryR\x0bqueryParams\x12P\n\x13superblocksMetadata\x18\x0c \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadata\x1aN\n\x0b\x43ustomEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x13.common.v1.PropertyR\x05value:\x02\x38\x01\x1aS\n\x10QueryParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x13.common.v1.PropertyR\x05value:\x02\x38\x01\x42=Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.s3.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.workflow.v1.plugin_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z5github.com/superblocksteam/types/gen/go/plugins/s3/v1'
-  _globals['_SUPERBLOCKSMETADATA']._serialized_start=45
-  _globals['_SUPERBLOCKSMETADATA']._serialized_end=104
-  _globals['_PROPERTY']._serialized_start=107
-  _globals['_PROPERTY']._serialized_end=425
-  _globals['_CUSTOM']._serialized_start=427
-  _globals['_CUSTOM']._serialized_end=510
-  _globals['_PLUGIN']._serialized_start=513
-  _globals['_PLUGIN']._serialized_end=816
+  _globals['DESCRIPTOR']._serialized_options = b'Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v1'
+  _globals['_PLUGIN_CUSTOMENTRY']._loaded_options = None
+  _globals['_PLUGIN_CUSTOMENTRY']._serialized_options = b'8\001'
+  _globals['_PLUGIN_QUERYPARAMSENTRY']._loaded_options = None
+  _globals['_PLUGIN_QUERYPARAMSENTRY']._serialized_options = b'8\001'
+  _globals['_TUPLE']._serialized_start=81
+  _globals['_TUPLE']._serialized_end=128
+  _globals['_PLUGIN']._serialized_start=131
+  _globals['_PLUGIN']._serialized_end=559
+  _globals['_PLUGIN_CUSTOMENTRY']._serialized_start=396
+  _globals['_PLUGIN_CUSTOMENTRY']._serialized_end=474
+  _globals['_PLUGIN_QUERYPARAMSENTRY']._serialized_start=476
+  _globals['_PLUGIN_QUERYPARAMSENTRY']._serialized_end=559
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/salesforce/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/plugins/smtp/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/requests_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: plugins/smtp/v1/plugin.proto
+# source: security/v1/requests.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from gen.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from gen.security.v1 import service_pb2 as security_dot_v1_dot_service__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cplugins/smtp/v1/plugin.proto\x12\x0fplugins.smtp.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xdd\x04\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12\x46\n\nconnection\x18\x02 \x01(\x0b\x32&.plugins.smtp.v1.Plugin.SmtpConnectionR\nconnection\x12\x12\n\x04\x66rom\x18\x03 \x01(\tR\x04\x66rom\x12\x19\n\x08reply_to\x18\x04 \x01(\tR\x07replyTo\x12\x0e\n\x02to\x18\x05 \x01(\tR\x02to\x12\x0e\n\x02\x63\x63\x18\x06 \x01(\tR\x02\x63\x63\x12\x10\n\x03\x62\x63\x63\x18\x07 \x01(\tR\x03\x62\x63\x63\x12\x18\n\x07subject\x18\x08 \x01(\tR\x07subject\x12\x12\n\x04\x62ody\x18\t \x01(\tR\x04\x62ody\x12 \n\x0b\x61ttachments\x18\n \x01(\tR\x0b\x61ttachments\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x0b \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\x98\x01\n\x0eSmtpConnection\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12\x1a\n\x08username\x18\x03 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x04 \x01(\tR\x08password\x12\x1b\n\x06secure\x18\x05 \x01(\x08H\x00R\x06secure\x88\x01\x01\x42\t\n\x07_secureB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB9Z7github.com/superblocksteam/types/gen/go/plugins/smtp/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asecurity/v1/requests.proto\x12\x0bsecurity.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19security/v1/service.proto\"O\n\x18ResourcesToResignRequest\x12\x1d\n\nclaimed_by\x18\x01 \x01(\tR\tclaimedBy\x12\x14\n\x05limit\x18\x02 \x01(\x05R\x05limit\"P\n\x19ResourcesToResignResponse\x12\x33\n\tresources\x18\x01 \x03(\x0b\x32\x15.security.v1.ResourceR\tresources\"\xfb\x02\n\x0bKeyRotation\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32\x1e.security.v1.KeyRotationStatusR\x06status\x12/\n\x13resources_completed\x18\x03 \x01(\x05R\x12resourcesCompleted\x12\'\n\x0fresources_total\x18\x04 \x01(\x05R\x0eresourcesTotal\x12$\n\x0esigning_key_id\x18\x05 \x01(\tR\x0csigningKeyId\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x34\n\x07updated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\x12\x38\n\tcompleted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcompleted\"U\n\x14KeyRotationsResponse\x12=\n\rkey_rotations\x18\x01 \x03(\x0b\x32\x18.security.v1.KeyRotationR\x0ckeyRotations*\xc2\x01\n\x11KeyRotationStatus\x12#\n\x1fKEY_ROTATION_STATUS_UNSPECIFIED\x10\x00\x12#\n\x1fKEY_ROTATION_STATUS_IN_PROGRESS\x10\x01\x12!\n\x1dKEY_ROTATION_STATUS_COMPLETED\x10\x02\x12\x1e\n\x1aKEY_ROTATION_STATUS_FAILED\x10\x03\x12 \n\x1cKEY_ROTATION_STATUS_CANCELED\x10\x04\x42\x35Z3github.com/superblocksteam/types/gen/go/security/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.smtp.v1.plugin_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'security.v1.requests_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z7github.com/superblocksteam/types/gen/go/plugins/smtp/v1'
-  _globals['_PLUGIN']._serialized_start=82
-  _globals['_PLUGIN']._serialized_end=687
-  _globals['_PLUGIN_SMTPCONNECTION']._serialized_start=491
-  _globals['_PLUGIN_SMTPCONNECTION']._serialized_end=643
+  _globals['DESCRIPTOR']._serialized_options = b'Z3github.com/superblocksteam/types/gen/go/security/v1'
+  _globals['_KEYROTATIONSTATUS']._serialized_start=736
+  _globals['_KEYROTATIONSTATUS']._serialized_end=930
+  _globals['_RESOURCESTORESIGNREQUEST']._serialized_start=103
+  _globals['_RESOURCESTORESIGNREQUEST']._serialized_end=182
+  _globals['_RESOURCESTORESIGNRESPONSE']._serialized_start=184
+  _globals['_RESOURCESTORESIGNRESPONSE']._serialized_end=264
+  _globals['_KEYROTATION']._serialized_start=267
+  _globals['_KEYROTATION']._serialized_end=646
+  _globals['_KEYROTATIONSRESPONSE']._serialized_start=648
+  _globals['_KEYROTATIONSRESPONSE']._serialized_end=733
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/plugins/snowflake/v1/plugin_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/annotations_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/secrets/v1/secrets_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/store_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/secrets/v1/store_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/security/v1/security_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/store_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: security/v1/security.proto
+# source: store/v1/store.proto
+# Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
+from gen.secrets.v1 import secrets_pb2 as secrets_dot_v1_dot_secrets__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asecurity/v1/security.proto\x12\x0bsecurity.v1\"1\n\tSignature\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x12\n\x04\x64\x61ta\x18\x02 \x01(\x0cR\x04\x64\x61taB5Z3github.com/superblocksteam/types/gen/go/security/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14store/v1/store.proto\x12\x08store.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x18secrets/v1/secrets.proto\"F\n\x04Pair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value\"5\n\x06Stores\x12+\n\x07secrets\x18\x01 \x03(\x0b\x32\x11.secrets.v1.StoreR\x07secretsB2Z0github.com/superblocksteam/types/gen/go/store/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'security.v1.security_pb2', _globals)
-if _descriptor._USE_C_DESCRIPTORS == False:
-  _globals['DESCRIPTOR']._options = None
-  _globals['DESCRIPTOR']._serialized_options = b'Z3github.com/superblocksteam/types/gen/go/security/v1'
-  _globals['_SIGNATURE']._serialized_start=43
-  _globals['_SIGNATURE']._serialized_end=92
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'store.v1.store_pb2', _globals)
+if not _descriptor._USE_C_DESCRIPTORS:
+  _globals['DESCRIPTOR']._loaded_options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z0github.com/superblocksteam/types/gen/go/store/v1'
+  _globals['_PAIR']._serialized_start=90
+  _globals['_PAIR']._serialized_end=160
+  _globals['_STORES']._serialized_start=162
+  _globals['_STORES']._serialized_end=215
 # @@protoc_insertion_point(module_scope)
```

### Comparing `superblocks-types-0.0.4/gen/py/security/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/security/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/security/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/store/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/store/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/store/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/superblocks_types.egg-info/PKG-INFO` & `superblocks-types-0.0.5/gen/py/superblocks_types.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/syncer/v1/service_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/syncer/v1/syncer_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/syncer/v1/syncer_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/transport/v1/transport_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/transport/v1/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/utils/v1/utils_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/utils/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/validate/validate_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/step_executor_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.4/gen/py/worker/v1/step_executor_pb2_grpc.py` & `superblocks-types-0.0.5/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py`

 * *Files identical despite different names*

